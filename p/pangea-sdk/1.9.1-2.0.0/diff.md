# Comparing `tmp/pangea_sdk-1.9.1.tar.gz` & `tmp/pangea_sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangea_sdk-1.9.1.tar", max compression
+gzip compressed data, was "pangea_sdk-2.0.0.tar", max compression
```

## Comparing `pangea_sdk-1.9.1.tar` & `pangea_sdk-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     7767 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/README.md
--rw-r--r--   0        0        0      146 2023-06-08 12:11:20.163141 pangea_sdk-1.9.1/pangea/__init__.py
--rw-r--r--   0        0        0     3778 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/audit_logger.py
--rw-r--r--   0        0        0     1059 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/config.py
--rw-r--r--   0        0        0     8343 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/deep_verify.py
--rw-r--r--   0        0        0      604 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/deprecated.py
--rw-r--r--   0        0        0     6511 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/dump_audit.py
--rw-r--r--   0        0        0     4458 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/exceptions.py
--rw-r--r--   0        0        0     9922 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/request.py
--rw-r--r--   0        0        0     3891 2023-06-08 19:01:01.397510 pangea_sdk-1.9.1/pangea/response.py
--rw-r--r--   0        0        0      221 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/services/__init__.py
--rw-r--r--   0        0        0    24530 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/audit.py
--rw-r--r--   0        0        0      451 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/services/audit/exceptions.py
--rw-r--r--   0        0        0    12093 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/models.py
--rw-r--r--   0        0        0     5265 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/signing.py
--rw-r--r--   0        0        0     7638 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/audit/util.py
--rw-r--r--   0        0        0    37055 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/authn/authn.py
--rw-r--r--   0        0        0    16758 2023-06-02 19:28:58.018357 pangea_sdk-1.9.1/pangea/services/authn/models.py
--rw-r--r--   0        0        0      956 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/base.py
--rw-r--r--   0        0        0     4034 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/embargo.py
--rw-r--r--   0        0        0    35748 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/intel.py
--rw-r--r--   0        0        0     7440 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/redact.py
--rw-r--r--   0        0        0     1450 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/services/vault/models/asymmetric.py
--rw-r--r--   0        0        0     8463 2023-06-06 18:59:31.171699 pangea_sdk-1.9.1/pangea/services/vault/models/common.py
--rw-r--r--   0        0        0      481 2023-04-28 12:40:26.182902 pangea_sdk-1.9.1/pangea/services/vault/models/secret.py
--rw-r--r--   0        0        0     1330 2023-05-04 12:20:49.539533 pangea_sdk-1.9.1/pangea/services/vault/models/symmetric.py
--rw-r--r--   0        0        0    44423 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/services/vault/vault.py
--rw-r--r--   0        0        0     5547 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/tools.py
--rw-r--r--   0        0        0      974 2023-06-08 12:11:20.163141 pangea_sdk-1.9.1/pangea/utils.py
--rw-r--r--   0        0        0    10616 2023-06-08 19:01:01.401511 pangea_sdk-1.9.1/pangea/verify_audit.py
--rw-r--r--   0        0        0      840 2023-06-08 12:11:20.163141 pangea_sdk-1.9.1/pyproject.toml
--rw-r--r--   0        0        0     8760 1970-01-01 00:00:00.000000 pangea_sdk-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     5248 2023-06-26 19:51:02.843422 pangea_sdk-2.0.0/README.md
+-rw-r--r--   0        0        0      146 2023-07-05 17:23:11.946254 pangea_sdk-2.0.0/pangea/__init__.py
+-rw-r--r--   0        0        0     3778 2023-06-15 17:19:16.333159 pangea_sdk-2.0.0/pangea/audit_logger.py
+-rw-r--r--   0        0        0     1036 2023-07-03 18:24:49.215977 pangea_sdk-2.0.0/pangea/config.py
+-rw-r--r--   0        0        0     8343 2023-07-06 20:33:55.287182 pangea_sdk-2.0.0/pangea/deep_verify.py
+-rw-r--r--   0        0        0      604 2023-07-06 20:33:55.287182 pangea_sdk-2.0.0/pangea/deprecated.py
+-rw-r--r--   0        0        0     6511 2023-07-06 20:33:55.287182 pangea_sdk-2.0.0/pangea/dump_audit.py
+-rw-r--r--   0        0        0     4605 2023-07-03 18:24:49.215977 pangea_sdk-2.0.0/pangea/exceptions.py
+-rw-r--r--   0        0        0    11835 2023-07-06 20:33:55.287182 pangea_sdk-2.0.0/pangea/request.py
+-rw-r--r--   0        0        0     4151 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/response.py
+-rw-r--r--   0        0        0      221 2023-07-03 18:49:22.305783 pangea_sdk-2.0.0/pangea/services/__init__.py
+-rw-r--r--   0        0        0    26053 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/audit/audit.py
+-rw-r--r--   0        0        0      451 2023-06-15 17:19:16.333159 pangea_sdk-2.0.0/pangea/services/audit/exceptions.py
+-rw-r--r--   0        0        0    11350 2023-07-05 17:23:11.946254 pangea_sdk-2.0.0/pangea/services/audit/models.py
+-rw-r--r--   0        0        0     5265 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/audit/signing.py
+-rw-r--r--   0        0        0     7568 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/audit/util.py
+-rw-r--r--   0        0        0    69734 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/authn/authn.py
+-rw-r--r--   0        0        0    16331 2023-06-30 17:54:47.327521 pangea_sdk-2.0.0/pangea/services/authn/models.py
+-rw-r--r--   0        0        0     1347 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/base.py
+-rw-r--r--   0        0        0     3905 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/embargo.py
+-rw-r--r--   0        0        0    27563 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/intel.py
+-rw-r--r--   0        0        0     7322 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/redact.py
+-rw-r--r--   0        0        0     1450 2023-06-15 17:19:16.333159 pangea_sdk-2.0.0/pangea/services/vault/models/asymmetric.py
+-rw-r--r--   0        0        0     8468 2023-07-03 18:24:49.219977 pangea_sdk-2.0.0/pangea/services/vault/models/common.py
+-rw-r--r--   0        0        0      481 2023-06-15 17:19:16.333159 pangea_sdk-2.0.0/pangea/services/vault/models/secret.py
+-rw-r--r--   0        0        0     1330 2023-06-15 17:19:16.333159 pangea_sdk-2.0.0/pangea/services/vault/models/symmetric.py
+-rw-r--r--   0        0        0    41847 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/services/vault/vault.py
+-rw-r--r--   0        0        0     6403 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/tools.py
+-rw-r--r--   0        0        0     2347 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/utils.py
+-rw-r--r--   0        0        0    10616 2023-07-06 20:33:55.291182 pangea_sdk-2.0.0/pangea/verify_audit.py
+-rw-r--r--   0        0        0      840 2023-07-05 17:23:11.946254 pangea_sdk-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6241 1970-01-01 00:00:00.000000 pangea_sdk-2.0.0/PKG-INFO
```

### Comparing `pangea_sdk-1.9.1/pangea/audit_logger.py` & `pangea_sdk-2.0.0/pangea/audit_logger.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pangea/config.py` & `pangea_sdk-2.0.0/pangea/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 @dataclass
 class PangeaConfig:
     """Holds run time configuration information used by SDK components."""
 
     domain: str = "aws.us.pangea.cloud"
     environment: str = "production"
 
+    config_id: Optional[str] = None
+
     """
     Set to true to use plain http
 
     """
     insecure: bool = False
 
     """
@@ -33,23 +35,22 @@
     """
     Timeout used on initial request attempts
 
     """
     request_timeout: int = 5
 
     """
-    Enable queued request retry support
-    """
-    queued_retry_enabled: bool = True
+    Timeout used to poll results after 202 (in secs)
 
     """
-    Number of queued request retry attempts, with exponential
-    backoff (4 -> 1 + 4 + 9 + 16  = 30 seconds of sleep)
+    poll_result_timeout: int = 30
 
     """
-    queued_retries: int = 4
+    Enable queued request retry support
+    """
+    queued_retry_enabled: bool = True
 
     """
     Extra user agent to be added to request user agent
 
     """
     custom_user_agent: Optional[str] = None
```

### Comparing `pangea_sdk-1.9.1/pangea/deep_verify.py` & `pangea_sdk-2.0.0/pangea/deep_verify.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pangea/deprecated.py` & `pangea_sdk-2.0.0/pangea/deprecated.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pangea/dump_audit.py` & `pangea_sdk-2.0.0/pangea/dump_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pangea/exceptions.py` & `pangea_sdk-2.0.0/pangea/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,33 +84,37 @@
     def __init__(self, service_name: str, response: PangeaResponse):
         super(MissingConfigID, self).__init__(
             f"Token did not contain a config scope for service {service_name}. Create a new token or provide a config ID explicitly in the service base",
             response,
         )
 
 
-class NotFound(PangeaAPIException):
-    """Resource not found"""
-
-    def __init__(self, url: str, response: PangeaResponse):
-        super(NotFound, self).__init__(f"Resource not found: {url}", response)
-
-
 class ProviderErrorException(PangeaAPIException):
     """Downstream provider error"""
 
 
 class InternalServerError(PangeaAPIException):
     """A pangea server error"""
 
     def __init__(self, response: PangeaResponse):
         message = f"summary: {response.summary}. request_id: {response.request_id}. request_time: {response.request_time}. response_time: ${response.response_time}"
         super().__init__(message, response)
 
 
+class AcceptedRequestException(PangeaAPIException):
+    """Accepted request exception. Async response"""
+
+    request_id: str
+
+    def __init__(self, response: PangeaResponse):
+        message = f"summary: {response.summary}. request_id: {response.request_id}."
+        super().__init__(message, response)
+        self.request_id = response.request_id
+
+
 class ServiceNotAvailableException(PangeaAPIException):
     """Service is not currently available"""
 
 
 # Embargo specific exceptions
 class EmbargoAPIException(PangeaAPIException):
     """Embargo service specific exceptions"""
```

### Comparing `pangea_sdk-1.9.1/pangea/request.py` & `pangea_sdk-2.0.0/pangea/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 
 import copy
 import json
 import logging
 import time
-from typing import Dict, Union
+from typing import Dict, List, Optional, Tuple, Type, Union
 
 import pangea
 import requests
 from pangea import exceptions
 from pangea.config import PangeaConfig
-from pangea.response import PangeaResponse, ResponseStatus
+from pangea.response import PangeaResponse, PangeaResponseResult, ResponseStatus
 from pangea.utils import default_encoder
 from requests.adapters import HTTPAdapter, Retry
 
 
 class PangeaRequest(object):
     """An object that makes direct calls to Pangea Service APIs.
 
     Wraps Get/Post calls to support both API requests. If `queued_retry_enabled`
     is enabled, the progress of long running Post requests will queried until
-    completion or until the `queued_retries` limit is reached. Both values can
+    completion or until the `poll_result_timeout` is reached. Both values can
     be set in PangeaConfig.
     """
 
-    def __init__(self, config: PangeaConfig, token: str, service: str, logger: logging.Logger):
+    def __init__(
+        self, config: PangeaConfig, token: str, service: str, logger: logging.Logger, check_config_id: bool = False
+    ):
         self.config = copy.deepcopy(config)
         self.token = token
         self.service = service
 
         # Queued request retry support flag
         self._queued_retry_enabled = config.queued_retry_enabled
 
         # Custom headers
         self._extra_headers = {}
         self._user_agent = ""
         self.set_custom_user_agent(config.custom_user_agent)
         self.session: requests.Session = self._init_session()
+        self._check_config_id = check_config_id
 
         self.logger = logger
 
     def __del__(self):
         self.session.close()
 
     def set_extra_headers(self, headers: dict):
@@ -69,101 +72,141 @@
         Args:
             value (bool): true - enable queued request retry mode, false - to disable
         """
         self._queued_retry_enabled = value
 
         return self._queued_retry_enabled
 
-    def post(self, endpoint: str = "", data: Union[str, Dict] = {}) -> PangeaResponse:
+    def post(
+        self,
+        endpoint: str,
+        result_class: Type[PangeaResponseResult],
+        data: Union[str, Dict] = {},
+        files: Optional[List[Tuple]] = None,
+        poll_result: bool = True,
+    ) -> PangeaResponse:
         """Makes the POST call to a Pangea Service endpoint.
 
-        If queued_support mode is enabled, progress checks will be made for
-        queued requests until processing is completed or until exponential
-        backoff `queued_retries` have been reached.
-
         Args:
             endpoint(str): The Pangea Service API endpoint.
             data(dict): The POST body payload object
 
         Returns:
             PangeaResponse which contains the response in its entirety and
                various properties to retrieve individual fields
         """
         url = self._url(endpoint)
+        # Set config ID if available
+        if self._check_config_id and self.config.config_id and data.pop("config_id", None) is None:
+            data["config_id"] = self.config.config_id
+
         data_send = json.dumps(data, default=default_encoder) if isinstance(data, dict) else data
         self.logger.debug(
             json.dumps({"service": self.service, "action": "post", "url": url, "data": data}, default=default_encoder)
         )
 
-        requests_response = self.session.post(url, headers=self._headers(), data=data_send)
-
-        if self._queued_retry_enabled and requests_response.status_code == 202:
-            response_json = requests_response.json()
-            self.logger.debug(
-                json.dumps(
-                    {"service": self.service, "action": "post", "url": url, "response": response_json},
-                    default=default_encoder,
-                )
-            )
-            request_id = response_json.get("request_id", None)
-
-            if not request_id:
-                raise Exception("Queue error: response did not include a 'request_id'")
-
-            pangea_response = self._handle_queued(request_id)
-        else:
-            pangea_response = PangeaResponse(requests_response)
+        if files:
+            multi = [("request", (None, data_send, "application/json"))]
+            multi.extend(files)
+            files = multi
+            data_send = None
+
+        requests_response = self.session.post(url, headers=self._headers(), data=data_send, files=files)
+        pangea_response = PangeaResponse(requests_response, result_class=result_class)
+        if poll_result:
+            pangea_response = self._handle_queued_result(pangea_response)
 
         self.logger.debug(
             json.dumps(
                 {"service": self.service, "action": "post", "url": url, "response": pangea_response.json},
                 default=default_encoder,
             )
         )
         self._check_response(pangea_response)
         return pangea_response
 
-    def get(self, endpoint: str, path: str) -> PangeaResponse:
+    def _handle_queued_result(self, response: PangeaResponse) -> PangeaResponse:
+        if self._queued_retry_enabled and response.raw_response.status_code == 202:
+            self.logger.debug(
+                json.dumps(
+                    {"service": self.service, "action": "poll_result", "response": response.json},
+                    default=default_encoder,
+                )
+            )
+            response = self._poll_result_retry(response)
+
+        return response
+
+    def get(self, path: str, result_class: Type[PangeaResponseResult], check_response: bool = True) -> PangeaResponse:
         """Makes the GET call to a Pangea Service endpoint.
 
         Args:
             endpoint(str): The Pangea Service API endpoint.
             path(str): Additional URL path
 
         Returns:
             PangeaResponse which contains the response in its entirety and
                various properties to retrieve individual fields
         """
-        url = self._url(f"{endpoint}/{path}")
 
-        self.logger.debug(json.dupms({"service": self.service, "action": "get", "url": url}))
+        url = self._url(path)
+        self.logger.debug(json.dumps({"service": self.service, "action": "get", "url": url}))
         requests_response = self.session.get(url, headers=self._headers())
-
-        pangea_response = PangeaResponse(requests_response)
+        pangea_response = PangeaResponse(requests_response, result_class=result_class)
 
         self.logger.debug(
             json.dumps(
-                {"service": self.service, "action": "post", "url": url, "response": pangea_response.json},
+                {"service": self.service, "action": "get", "url": url, "response": pangea_response.json},
                 default=default_encoder,
             )
         )
-        self._check_response(pangea_response)
-        return pangea_response
 
-    def _handle_queued(self, request_id: str) -> PangeaResponse:
+        if check_response is False:
+            return pangea_response
+
+        return self._check_response(pangea_response)
+
+    def _get_delay(self, retry_count, start):
+        delay = retry_count * retry_count
+        now = time.time()
+        # if with this delay exceed timeout, reduce delay
+        if now - start + delay >= self.config.poll_result_timeout:
+            delay = start + self.config.poll_result_timeout - now
+
+        return delay
+
+    def _reach_timeout(self, start):
+        return time.time() - start >= self.config.poll_result_timeout
+
+    def _get_poll_path(self, request_id: str):
+        return f"request/{request_id}"
+
+    def poll_result_once(self, response: PangeaResponse, check_response: bool = True):
+        request_id = response.request_id
+        if not request_id:
+            raise exceptions.PangeaException("Poll result error error: response did not include a 'request_id'")
+
+        if response.status != ResponseStatus.ACCEPTED.value:
+            raise exceptions.PangeaException("Response already proccesed")
+
+        path = self._get_poll_path(request_id)
+        self.logger.debug(json.dumps({"service": self.service, "action": "poll_result_once", "url": path}))
+        return self.get(path, response.result_class, check_response=check_response)
+
+    def _poll_result_retry(self, response: PangeaResponse) -> PangeaResponse:
         retry_count = 1
+        start = time.time()
 
-        while True:
-            time.sleep(retry_count * retry_count)
-            pangea_response = self.get("request", request_id)
-
-            if pangea_response.code == 202 and retry_count <= self.config.queued_retries:
-                retry_count += 1
-            else:
-                return pangea_response
+        while response.status == ResponseStatus.ACCEPTED.value and not self._reach_timeout(start):
+            time.sleep(self._get_delay(retry_count, start))
+            response = self.poll_result_once(response, check_response=False)
+            retry_count += 1
+
+        self.logger.debug(json.dumps({"service": self.service, "action": "poll_result_retry", "step": "exit"}))
+        return self._check_response(response)
 
     def _init_session(self) -> requests.Session:
         retry_config = Retry(
             total=self.config.request_retries,
             backoff_factor=self.config.request_backoff,
             status_forcelist=[500, 502, 503, 504],
         )
@@ -188,31 +231,28 @@
                 self.config.domain if self.config.environment == "local" else f"{self.service}.{self.config.domain}"
             )
             url = f"{schema}{domain}/{path}"
         return url
 
     def _headers(self) -> dict:
         headers = {
-            "Content-Type": "application/json",
             "User-Agent": self._user_agent,
             "Authorization": f"Bearer {self.token}",
         }
 
         # We want to ignore previous headers if user tryed to set them, so we will overwrite them.
         self._extra_headers.update(headers)
         return self._extra_headers
 
     def _check_response(self, response: PangeaResponse):
         status = response.status
         summary = response.summary
 
         if status == ResponseStatus.SUCCESS.value:
-            return
-        else:
-            response.result = None
+            return response
 
         self.logger.error(
             json.dumps(
                 {
                     "service": self.service,
                     "action": "api_error",
                     "url": response.raw_response.url,
@@ -249,8 +289,10 @@
             raise exceptions.ForbiddenVaultOperation(summary, response)
         elif status == ResponseStatus.VAULT_ITEM_NOT_FOUND.value:
             raise exceptions.VaultItemNotFound(summary, response)
         elif status == ResponseStatus.NOT_FOUND.value:
             raise exceptions.NotFound(response.raw_response.url if response.raw_response is not None else "", response)
         elif status == ResponseStatus.INTERNAL_SERVER_ERROR.value:
             raise exceptions.InternalServerError(response)
+        elif status == ResponseStatus.ACCEPTED.value:
+            raise exceptions.AcceptedRequestException(response)
         raise exceptions.PangeaAPIException(f"{summary} ", response)
```

### Comparing `pangea_sdk-1.9.1/pangea/response.py` & `pangea_sdk-2.0.0/pangea/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 import datetime
 import enum
-from typing import Any, Dict, Generic, List, Optional, TypeVar
+from typing import Any, Dict, Generic, List, Optional, Type, TypeVar
 
 import requests
 from pangea.utils import format_datetime
 from pydantic import BaseModel
 
 T = TypeVar("T")
 
@@ -71,14 +71,15 @@
     TREE_NOT_FOUND = "TreeNotFound"
     IP_NOT_FOUND = "IPNotFound"
     BAD_OFFSET = "BadOffset"
     FORBIDDEN_VAULT_OPERATION = "ForbiddenVaultOperation"
     VAULT_ITEM_NOT_FOUND = "VaultItemNotFound"
     NOT_FOUND = "NotFound"
     INTERNAL_SERVER_ERROR = "InternalError"
+    ACCEPTED = "Accepted"
 
 
 class ResponseHeader(APIResponseModel):
     """
     Pangea response API header.
 
     Arguments:
@@ -97,25 +98,29 @@
 
 
 class PangeaResponse(Generic[T], ResponseHeader):
     raw_result: Optional[Dict[str, Any]] = None
     raw_response: Optional[requests.Response] = None
     result: Optional[T] = None
     pangea_error: Optional[PangeaError] = None
+    result_class: Type[PangeaResponseResult] = PangeaResponseResult
     _json: Any
 
-    def __init__(self, response: requests.Response):
+    def __init__(self, response: requests.Response, result_class: Type[PangeaResponseResult]):
         _json = response.json()
         super(PangeaResponse, self).__init__(**_json)
         self._json = _json
         self.raw_response = response
         self.raw_result = self._json["result"]
+        self.result_class = result_class
         self.result = (
-            T(**self._json["result"])
-            if issubclass(type(T), PangeaResponseResult) and self.status == ResponseStatus.SUCCESS.value
+            self.result_class(**self.raw_result)
+            if self.raw_result is not None
+            and issubclass(self.result_class, PangeaResponseResult)
+            and self.status == ResponseStatus.SUCCESS.value
             else None
         )
         if not self.success:
             self.pangea_error = PangeaError(**self.raw_result) if self.raw_result is not None else None
 
     @property
     def success(self) -> bool:
```

### Comparing `pangea_sdk-1.9.1/pangea/services/audit/audit.py` & `pangea_sdk-2.0.0/pangea/services/audit/audit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 import datetime
 import json
-from typing import Dict, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from pangea.response import PangeaResponse
 from pangea.services.audit.exceptions import AuditException, EventCorruption
 from pangea.services.audit.models import (
     Event,
     EventEnvelope,
-    EventSigning,
     EventVerification,
     LogRequest,
     LogResult,
     PublishedRoot,
     Root,
     RootRequest,
     RootResult,
@@ -36,14 +35,15 @@
     get_arweave_published_roots,
     get_public_key,
     verify_consistency_proof,
     verify_envelope_hash,
     verify_membership_proof,
 )
 from pangea.services.base import ServiceBase
+from pangea.utils import canonicalize_nested_json
 
 
 class Audit(ServiceBase):
     """Audit service client.
 
     Provides methods to interact with the [Pangea Audit Service](https://pangea.cloud/docs/api/audit).
 
@@ -61,15 +61,16 @@
         PANGEA_TOKEN = os.getenv("PANGEA_AUDIT_TOKEN")
         audit_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Audit service
         audit = Audit(token=PANGEA_TOKEN, config=audit_config)
     """
 
-    service_name: str = "audit"
+    service_name = "audit"
+    _support_multi_config = True
 
     def __init__(
         self,
         token,
         config=None,
         private_key_file: str = "",
         public_key_info: Dict[str, str] = {},
@@ -96,15 +97,15 @@
         new: Optional[Union[str, dict]] = None,
         old: Optional[Union[str, dict]] = None,
         source: Optional[str] = None,
         status: Optional[str] = None,
         target: Optional[str] = None,
         timestamp: Optional[datetime.datetime] = None,
         verify: bool = False,
-        signing: EventSigning = EventSigning.NONE,
+        sign_local: bool = False,
         verbose: Optional[bool] = None,
     ) -> PangeaResponse[LogResult]:
         """
         Log an entry
 
         Create a log entry in the Secure Audit Log.
 
@@ -117,15 +118,15 @@
             new (str, dict, optional): The value of a record after it was changed.
             old (str, dict, optional): The value of a record before it was changed.
             source (str, optional): Used to record the location from where an activity occurred.
             status (str, optional): Record whether or not the activity was successful.
             target (str, optional): Used to record the specific record that was targeted by the auditable activity.
             timestamp (datetime, optional): An optional client-supplied timestamp.
             verify (bool, optional): True to verify logs consistency after response.
-            signing (bool, optional): True to sign event.
+            sign_local (bool, optional): True to sign event with local key.
             verbose (bool, optional): True to get a more verbose response.
             tenant_id (string, optional): Used to record the tenant associated with this activity.
         Raises:
             AuditException: If an audit based api exception happens
             PangeaAPIException: If an API Error happens
 
         Returns:
@@ -150,23 +151,65 @@
             action=action,
             new=new,
             old=old,
             source=source,
             status=status,
             target=target,
             timestamp=timestamp,
-            tenant_id=self.tenant_id,
         )
 
-        if signing == EventSigning.LOCAL and self.signer is None:
+        return self.log_event(event=event, verify=verify, sign_local=sign_local, verbose=verbose)
+
+    def log_event(
+        self,
+        event: Dict[str, Any],
+        verify: bool = False,
+        sign_local: bool = False,
+        verbose: Optional[bool] = None,
+    ) -> PangeaResponse[LogResult]:
+        """
+        Log an entry
+
+        Create a log entry in the Secure Audit Log.
+        Args:
+            event (dict[str, Any]): event to be logged
+            verify (bool, optional): True to verify logs consistency after response.
+            sign_local (bool, optional): True to sign event with local key.
+            verbose (bool, optional): True to get a more verbose response.
+        Raises:
+            AuditException: If an audit based api exception happens
+            PangeaAPIException: If an API Error happens
+
+        Returns:
+            A PangeaResponse where the hash of event data and optional verbose
+                results are returned in the response.result field.
+                Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/audit#log-an-entry).
+
+        Examples:
+            try:
+                log_response = audit.log({"message"="Hello world"}, verbose=False)
+                print(f"Response. Hash: {log_response.result.hash}")
+            except pe.PangeaAPIException as e:
+                print(f"Request Error: {e.response.summary}")
+                for err in e.errors:
+                    print(f"\\t{err.detail} \\n")
+        """
+
+        if event.get("tenant_id", None) is None and self.tenant_id:
+            event["tenant_id"] = self.tenant_id
+
+        event = {k: v for k, v in event.items() if v is not None}
+        event = canonicalize_nested_json(event)
+
+        if sign_local is True and self.signer is None:
             raise AuditException("Error: the `signing` parameter set, but `signer` is not configured")
 
-        input = LogRequest(event=event.get_stringified_copy(), verbose=verbose)
+        input = LogRequest(event=event, verbose=verbose)
 
-        if signing == EventSigning.LOCAL:
+        if sign_local is True:
             data2sign = canonicalize_event(event)
             signature = self.signer.sign(data2sign)
             if signature is not None:
                 input.signature = signature
             else:
                 raise AuditException("Error: failure signing message")
 
@@ -174,22 +217,21 @@
             self.set_public_key(input, self.signer, self.public_key_info)
 
         if verify:
             input.verbose = True
             if self.prev_unpublished_root_hash:
                 input.prev_root = self.prev_unpublished_root_hash
 
-        response = self.request.post("v1/log", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/log", LogResult, data=input.dict(exclude_none=True))
         return self.handle_log_response(response, verify=verify)
 
     def handle_log_response(self, response: PangeaResponse, verify: bool) -> PangeaResponse[LogResult]:
         if not response.success:
             return response
 
-        response.result = LogResult(**response.raw_result)
         new_unpublished_root_hash = response.result.unpublished_root
 
         if verify:
             if response.result.envelope:
                 # verify event hash
                 if response.result.hash and not verify_envelope_hash(response.result.envelope, response.result.hash):
                     # it's a extreme case, it's OK to raise an exception
@@ -294,15 +336,15 @@
             end=format_datetime(end) if isinstance(end, datetime.datetime) else end,
             limit=limit,
             max_results=max_results,
             search_restriction=search_restriction,
             verbose=verbose,
         )
 
-        response = self.request.post("v1/search", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/search", SearchOutput, data=input.dict(exclude_none=True))
         return self.handle_search_response(response, verify_consistency, verify_events)
 
     def results(
         self,
         id: str,
         limit: Optional[int] = 20,
         offset: Optional[int] = 0,
@@ -347,33 +389,31 @@
             raise AuditException("The 'offset' argument must be a positive integer")
 
         input = SearchResultRequest(
             id=id,
             limit=limit,
             offset=offset,
         )
-        response = self.request.post("v1/results", data=input.dict(exclude_none=True))
+        response = self.request.post("v1/results", SearchResultOutput, data=input.dict(exclude_none=True))
         return self.handle_results_response(response, verify_consistency, verify_events)
 
     def handle_results_response(
         self, response: PangeaResponse[SearchResultOutput], verify_consistency: bool = False, verify_events: bool = True
     ) -> PangeaResponse[SearchResultOutput]:
         if not response.success:
             return response
 
-        response.result = SearchResultOutput(**response.raw_result)
         return self.process_search_results(response, verify_consistency, verify_events)
 
     def handle_search_response(
         self, response: PangeaResponse[SearchOutput], verify_consistency: bool = False, verify_events: bool = True
     ) -> PangeaResponse[SearchOutput]:
         if not response.success:
             return response
 
-        response.result = SearchOutput(**response.raw_result)
         return self.process_search_results(response, verify_consistency, verify_events)
 
     def process_search_results(
         self, response: PangeaResponse[SearchResultOutput], verify_consistency: bool = False, verify_events: bool = True
     ) -> PangeaResponse[SearchResultOutput]:
         if verify_events:
             for event_search in response.result.events:
@@ -598,10 +638,8 @@
             AuditException: If an audit based api exception happens
             PangeaAPIException: If an API Error happens
 
         Examples:
             response = audit.root(tree_size=7)
         """
         input = RootRequest(tree_size=tree_size)
-        response = self.request.post("v1/root", data=input.dict(exclude_none=True))
-        response.result = RootResult(**response.raw_result)
-        return response
+        return self.request.post("v1/root", RootResult, data=input.dict(exclude_none=True))
```

### Comparing `pangea_sdk-1.9.1/pangea/services/audit/models.py` & `pangea_sdk-2.0.0/pangea/services/audit/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
-import copy
 import datetime
 import enum
-import json
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional
 
 from pangea.response import APIRequestModel, APIResponseModel, PangeaResponseResult
 
 
 class EventVerification(str, enum.Enum):
     NONE = "none"
     PASS = "pass"
@@ -17,98 +15,117 @@
     def __str__(self):
         return str(self.value)
 
     def __repr__(self):
         return str(self.value)
 
 
-class EventSigning(enum.Enum):
-    NONE = 0
-    LOCAL = 1
-
-    def __str__(self):
-        return str(self.value)
-
-    def __repr__(self):
-        return str(self.value)
-
-
-class Event(APIResponseModel):
-    """Event to perform an auditable activity
-
-    Arguments:
-    message -- A message describing a detailed account of what happened.
-    actor -- who performed the auditable activity.
-    action -- auditable action that occurred.
-    new -- The value of a record after it was changed.
-    old -- The value of a record before it was changed.
-    source -- Used to record the location from where an activity occurred.
-    status -- Record whether or not the activity was successful.
-    target -- Used to record the specific record that was targeted by the auditable activity.
-    timestamp -- An optional client-supplied timestamp.
-    """
-
-    message: Union[str, dict]
-    actor: Optional[str] = None
-    action: Optional[str] = None
-    new: Optional[Union[str, dict]] = None
-    old: Optional[Union[str, dict]] = None
-    source: Optional[str] = None
-    status: Optional[str] = None
-    target: Optional[str] = None
-    timestamp: Optional[datetime.datetime] = None
-    tenant_id: Optional[str] = None
+class Event(dict):
+    """
+    Event to perform an auditable activity
 
-    _JSON_SUPPORTED_FIELDS = ["message", "new", "old"]
+    Auxiliary class to be compatible with older SDKs
+    """
 
     def __init__(self, **data):
         super().__init__(**data)
-        self.parse_json_fields()
 
-    def parse_json_fields(self):
-        """Parse JSON supported fields from string to dict"""
-        for f in self._JSON_SUPPORTED_FIELDS:
-            v = getattr(self, f)
-            if type(v) is str:
-                try:
-                    obj = json.loads(v)
-                    setattr(self, f, obj)
-                except:
-                    pass
-
-    def get_stringified_copy(self):
-        """Return object copy with JSON supported fields in string format"""
-        aux = copy.deepcopy(self)
-        for f in self._JSON_SUPPORTED_FIELDS:
-            v = getattr(aux, f, None)
-            if v is not None and type(v) is dict:
-                setattr(aux, f, self._dict_to_canonicalized_str(v))
-
-        if isinstance(aux.timestamp, (datetime.datetime, datetime.date)):
-            aux.timestamp = aux.timestamp.isoformat().replace("+00:00", "Z")
-
-        return aux
-
-    def _dict_to_canonicalized_str(self, message: dict) -> str:
-        """Convert dict to canonical str"""
-        return json.dumps(message, ensure_ascii=False, allow_nan=False, separators=(",", ":"))
+    @property
+    def message(self):
+        return self.get("message")
+
+    @message.setter
+    def message(self, value):
+        self["message"] = value
+
+    @property
+    def actor(self):
+        return self.get("actor")
+
+    @actor.setter
+    def actor(self, value):
+        self["actor"] = value
+
+    @property
+    def action(self):
+        return self.get("action")
+
+    @action.setter
+    def action(self, value):
+        self["action"] = value
+
+    @property
+    def new(self):
+        return self.get("new")
+
+    @new.setter
+    def new(self, value):
+        self["new"] = value
+
+    @property
+    def old(self):
+        return self.get("old")
+
+    @old.setter
+    def old(self, value):
+        self["old"] = value
+
+    @property
+    def status(self):
+        return self.get("status")
+
+    @status.setter
+    def status(self, value):
+        self["status"] = value
+
+    @property
+    def source(self):
+        return self.get("source")
+
+    @source.setter
+    def source(self, value):
+        self["source"] = value
+
+    @property
+    def target(self):
+        return self.get("target")
+
+    @target.setter
+    def target(self, value):
+        self["target"] = value
+
+    @property
+    def timestamp(self):
+        return self.get("timestamp")
+
+    @timestamp.setter
+    def timestamp(self, value):
+        self["timestamp"] = value
+
+    @property
+    def tenant_id(self):
+        return self.get("tenant_id")
+
+    @tenant_id.setter
+    def tenant_id(self, value):
+        self["tenant_id"] = value
 
 
 class EventEnvelope(APIResponseModel):
     """
     Contain extra information about an event.
 
     Arguments:
     event -- Event describing auditable activity.
     signature -- An optional client-side signature for forgery protection.
     public_key -- The base64-encoded ed25519 public key used for the signature, if one is provided
     received_at -- A server-supplied timestamp
     """
 
-    event: Event
+    event: Dict[str, Any]
     signature: Optional[str] = None
     public_key: Optional[str] = None
     received_at: datetime.datetime
 
 
 class LogRequest(APIRequestModel):
     """
@@ -118,15 +135,15 @@
     event -- A structured event describing an auditable activity.
     verbose -- If true, be verbose in the response; include membership proof, unpublished root and consistency proof, etc.
     signature -- An optional client-side signature for forgery protection.
     public_key -- The base64-encoded ed25519 public key used for the signature, if one is provided.
     prev_root -- Unpublished root hash that was returned from the last log API call that was made. If the user does not provide prev_root, the consistency proof from the last known unpublished root will be provided.
     """
 
-    event: Event
+    event: Dict[str, Any]
     verbose: Optional[bool] = None
     signature: Optional[str] = None
     public_key: Optional[str] = None
     prev_root: Optional[str] = None
 
 
 class LogResult(PangeaResponseResult):
```

### Comparing `pangea_sdk-1.9.1/pangea/services/audit/signing.py` & `pangea_sdk-2.0.0/pangea/services/audit/signing.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pangea/services/audit/util.py` & `pangea_sdk-2.0.0/pangea/services/audit/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 import base64
-import copy
 import json
 import logging
-import os
 from binascii import hexlify, unhexlify
 from dataclasses import dataclass
 from datetime import datetime
 from hashlib import sha256
 from typing import Dict, List, Optional
 
 import requests
 from pangea.services.audit.models import Event, EventEnvelope, PublishedRoot
-from pangea.utils import format_datetime
+from pangea.utils import default_encoder, format_datetime
 
 Hash = bytes
 
 
 JSON_TYPES = [int, float, str, bool]
 JSON_SUPPORTED_FIELDS = ["message", "new", "old"]
 
@@ -58,22 +56,21 @@
 
 
 def verify_hash(hash1: str, hash2: str) -> bool:
     return hash1 == hash2
 
 
 def verify_envelope_hash(envelope: EventEnvelope, hash: str):
-    env_tmp = copy.deepcopy(envelope)
-    env_tmp.event = env_tmp.event.get_stringified_copy()
-    return verify_hash(hash_dict(normalize_log(env_tmp.dict(exclude_none=True))), hash)
+    return verify_hash(hash_dict(normalize_log(envelope.dict(exclude_none=True))), hash)
 
 
 def canonicalize_event(event: Event) -> bytes:
-    tpm_event = event.get_stringified_copy()
-    return canonicalize_json(normalize_log(tpm_event.dict(exclude_none=True)))
+    return json.dumps(
+        event, ensure_ascii=False, allow_nan=False, separators=(",", ":"), sort_keys=True, default=default_encoder
+    ).encode("utf-8")
 
 
 def b64encode(data: bytes) -> str:
     ret = None
     if data is not None:
         ret = base64.b64encode(data).decode("utf-8")
     return ret
@@ -150,23 +147,23 @@
 def verify_membership_proof(node_hash: Hash, root_hash: Hash, proof: MembershipProof) -> bool:
     for proof_item in proof:
         proof_hash = proof_item.node_hash
         node_hash = hash_pair(proof_hash, node_hash) if proof_item.side == "left" else hash_pair(node_hash, proof_hash)
     return root_hash == node_hash
 
 
-def normalize_log(audit: dict) -> dict:
+def normalize_log(data: dict) -> dict:
     ans = {}
-    for key in audit:
-        if type(audit[key]) == datetime:
-            ans[key] = format_datetime(audit[key])
-        elif type(audit[key]) == dict:
-            ans[key] = normalize_log(audit[key])
+    for key in data:
+        if type(data[key]) == datetime:
+            ans[key] = format_datetime(data[key])
+        elif type(data[key]) == dict:
+            ans[key] = normalize_log(data[key])
         else:
-            ans[key] = audit[key]
+            ans[key] = data[key]
     return ans
 
 
 def canonicalize_json(message: dict) -> bytes:
     """Convert log to valid JSON types and apply RFC-7159 (Canonical JSON)"""
 
     return json.dumps(message, ensure_ascii=False, allow_nan=False, separators=(",", ":"), sort_keys=True).encode(
```

### Comparing `pangea_sdk-1.9.1/pangea/services/authn/models.py` & `pangea_sdk-2.0.0/pangea/services/authn/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 class ClientTokenCheckResult(PangeaResponseResult):
     id: str
     type: str
     life: int
     expire: str
     identity: str
     email: str
-    scopes: Scopes
+    scopes: Optional[Scopes] = None
     profile: Profile
     created_at: str
 
 
 class IDProvider(str, enum.Enum):
     FACEBOOK = "facebook"
     GITHUB = "github"
@@ -119,15 +119,15 @@
     def __str__(self):
         return self.value
 
     def __repr__(self):
         return self.value
 
 
-# https://dev.pangea.cloud/docs/api/authn#create-user
+# https://pangea.cloud/docs/api/authn#create-user
 class UserCreateRequest(APIRequestModel):
     email: str
     authenticator: str
     id_provider: IDProvider
     verified: Optional[bool] = None
     require_mfa: Optional[bool] = None
     profile: Optional[Profile] = None
@@ -148,15 +148,15 @@
 
 class UserDeleteRequest(APIRequestModel):
     email: Optional[str] = None
     id: Optional[str] = None
 
 
 class UserDeleteResult(PangeaResponseResult):
-    # https://dev.pangea.cloud/docs/api/authn#delete-a-user
+    # https://pangea.cloud/docs/api/authn#delete-user
     pass
 
 
 class UserInviteRequest(APIRequestModel):
     inviter: str
     email: str
     callback: str
@@ -215,15 +215,14 @@
 
 
 class UserInviteDeleteResult(PangeaResponseResult):
     pass
 
 
 class UserListRequest(APIRequestModel):
-    use_new: bool = True  # Temporary field, need to be true
     filter: Optional[Dict] = None
     last: Optional[str] = None
     order: Optional[ItemOrder] = None
     order_by: Optional[UserListOrderBy] = None
     size: Optional[int] = None
 
 
@@ -358,27 +357,27 @@
     code: str
 
 
 class ClientJWKSResult(PangeaResponseResult):
     keys: List[Union[JWKec, JWKrsa, JWK]]
 
 
-#   - path: authn::/v1/flow/complete
-# https://dev.pangea.cloud/docs/api/authn#complete-a-login-or-signup-flow
+# - path: authn::/v1/flow/complete
+# https://pangea.cloud/docs/api/authn#complete-sign-up-in
 class FlowCompleteRequest(APIRequestModel):
     flow_id: str
 
 
 class FlowCompleteResult(PangeaResponseResult):
     refresh_token: LoginToken
     login_token: LoginToken
 
 
-#   - path: authn::/v1/flow/enroll/mfa/complete
-# https://dev.pangea.cloud/docs/api/authn#complete-mfa-enrollment-by-verifying-a-trial-mfa-code
+# - path: authn::/v1/flow/enroll/mfa/complete
+# https://pangea.cloud/docs/api/authn#complete-mfa-enrollment
 class FlowEnrollMFACompleteRequest(APIRequestModel):
     flow_id: str
     code: str
     cancel: Optional[bool] = None
 
 
 class EnrollMFAStart:
@@ -447,171 +446,170 @@
     verify_social: Optional[VerifySocial] = None
 
 
 class FlowResetPasswordRequest(APIRequestModel):
     flow_id: str
     password: str
     cancel: Optional[bool] = None
-    cb_state: Optional[str] = None
-    cb_code: Optional[str] = None
 
 
 class FlowResetPasswordResult(CommonFlowResult):
     pass
 
 
 class FlowEnrollMFAcompleteResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/enroll/mfa/start
-# https://dev.pangea.cloud/docs/api/authn#start-the-process-of-enrolling-an-mfa
+# - path: authn::/v1/flow/enroll/mfa/start
+# https://pangea.cloud/docs/api/authn#start-mfa-enrollment
 class FlowEnrollMFAStartRequest(APIRequestModel):
     flow_id: str
     mfa_provider: MFAProvider
     phone: Optional[str] = None
 
 
 class FlowEnrollMFAStartResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/signup/password
-# https://dev.pangea.cloud/docs/api/authn#signup-a-new-account-using-a-password
+# - path: authn::/v1/flow/signup/password
+# https://pangea.cloud/docs/api/authn#password-sign-up
 class FlowSignupPasswordRequest(APIRequestModel):
     flow_id: str
     password: str
     first_name: str
     last_name: str
 
 
 class FlowSignupPasswordResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/signup/social
-# https://dev.pangea.cloud/docs/api/authn#signup-a-new-account-using-a-social-provider
+# - path: authn::/v1/flow/signup/social
+# https://pangea.cloud/docs/api/authn#social-sign-up
 class FlowSignupSocialRequest(APIRequestModel):
     flow_id: str
     cb_state: str
     cb_code: str
 
 
 class FlowSignupSocialResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/start
-# https://dev.pangea.cloud/docs/api/authn#start-a-new-signup-or-signin-flow
+# - path: authn::/v1/flow/start
+# https://pangea.cloud/docs/api/authn#start-a-sign-up-in
 class FlowStartRequest(APIRequestModel):
     cb_uri: Optional[str] = None
     email: Optional[str] = None
     flow_types: Optional[List[FlowType]] = None
     provider: Optional[IDProvider] = None
+    invitation: Optional[str] = None
 
 
 class FlowStartResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/verify/captcha
-# https://dev.pangea.cloud/docs/api/authn#verify-a-captcha-during-a-signup-or-signin-flow
+# - path: authn::/v1/flow/verify/captcha
+# https://pangea.cloud/docs/api/authn#verify-captcha
 class FlowVerifyCaptchaRequest(APIRequestModel):
     flow_id: str
     code: str
 
 
 class FlowVerifyCaptchaResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/verify/email
-# https://dev.pangea.cloud/docs/api/authn#verify-an-email-address-during-a-signup-or-signin-flow
+# - path: authn::/v1/flow/verify/email
+# https://pangea.cloud/docs/api/authn#verify-email-address
 class FlowVerifyEmailRequest(APIRequestModel):
     flow_id: str
     cb_state: Optional[str] = None
     cb_code: Optional[str] = None
 
 
 class FlowVerifyEmailResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/verify/mfa/complete
-# https://dev.pangea.cloud/docs/api/authn#complete-mfa-verification
+# - path: authn::/v1/flow/verify/mfa/complete
+# https://pangea.cloud/docs/api/authn#complete-mfa-verification
 class FlowVerifyMFACompleteRequest(APIRequestModel):
     flow_id: str
     code: Optional[str] = None
     cancel: Optional[bool] = None
 
 
 class FlowVerifyMFACompleteResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/verify/mfa/start
-# https://dev.pangea.cloud/docs/api/authn#start-the-process-of-mfa-verification
+# - path: authn::/v1/flow/verify/mfa/start
+# https://pangea.cloud/docs/api/authn#start-mfa-verification
 class FlowVerifyMFAStartRequest(APIRequestModel):
     flow_id: str
     mfa_provider: MFAProvider
 
 
 class FlowVerifyMFAStartResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/verify/password
-# https://dev.pangea.cloud/docs/api/authn#sign-in-with-a-password
+# - path: authn::/v1/flow/verify/password
+# https://pangea.cloud/docs/api/authn#password-sign-in
 class FlowVerifyPasswordRequest(APIRequestModel):
     flow_id: str
     password: Optional[str] = None
     cancel: Optional[bool] = None
 
 
 class FlowVerifyPasswordResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/flow/verify/social
-# https://dev.pangea.cloud/docs/api/authn#signin-with-a-social-provider
+# - path: authn::/v1/flow/verify/social
+# https://pangea.cloud/docs/api/authn#social-sign-in
 class FlowVerifySocialRequest(APIRequestModel):
     flow_id: str
     cb_state: str
     cb_code: str
 
 
 class FlowVerifySocialResult(CommonFlowResult):
     pass
 
 
-#   - path: authn::/v1/user/mfa/delete
-# https://dev.pangea.cloud/docs/api/authn#delete-mfa-enrollment-for-a-user
+# - path: authn::/v1/user/mfa/delete
+# https://pangea.cloud/docs/api/authn#delete-mfa-enrollment
 class UserMFADeleteRequest(APIRequestModel):
     user_id: str
     mfa_provider: MFAProvider
 
 
 class UserMFADeleteResult(PangeaResponseResult):
     pass
 
 
-#   - path: authn::/v1/user/mfa/enroll
-# https://dev.pangea.cloud/docs/api/authn#enroll-mfa-for-a-user
+# - path: authn::/v1/user/mfa/enroll
+# https://pangea.cloud/docs/api/authn#enroll-in-mfa
 class UserMFAEnrollRequest(APIRequestModel):
     user_id: str
     mfa_provider: MFAProvider
     code: str
 
 
 class UserMFAEnrollResult(PangeaResponseResult):
     pass
 
 
-#   - path: authn::/v1/user/mfa/start
-# https://dev.pangea.cloud/docs/api/authn#start-mfa-verification-for-a-user
+# - path: authn::/v1/user/mfa/start
+# https://pangea.cloud/docs/api/authn#start-mfa-verification
 class UserMFAStartRequest(APIRequestModel):
     user_id: str
     mfa_provider: MFAProvider
     enroll: Optional[bool] = None
     phone: Optional[str] = None
 
 
@@ -620,39 +618,39 @@
     secret: str
 
 
 class UserMFAStartResult(PangeaResponseResult):
     totp_secret: Optional[UserMFAStartTOTPSecret] = None
 
 
-#   - path: authn::/v1/user/mfa/verify
-# https://dev.pangea.cloud/docs/api/authn#verify-an-mfa-code
+# - path: authn::/v1/user/mfa/verify
+# https://pangea.cloud/docs/api/authn#verify-an-mfa-code
 class UserMFAverifyRequest(APIRequestModel):
     user_id: str
     mfa_provider: MFAProvider
     code: str
 
 
 class UserMFAVerifyResult(PangeaResponseResult):
     pass
 
 
-#   - path: authn::/v1/user/verify
-# https://dev.pangea.cloud/docs/api/authn#verify-a-user
+# - path: authn::/v1/user/verify
+# https://pangea.cloud/docs/api/authn#verify-user
 class UserVerifyRequest(APIRequestModel):
     id_provider: IDProvider
     email: str
     authenticator: str
 
 
 class UserVerifyResult(PangeaResponseResult):
     id: str
     email: str
     profile: Profile
-    scopes: Scopes
+    scopes: Optional[Scopes] = None
     id_providers: Optional[List[str]] = None
     mfa_providers: List[str]
     require_mfa: bool
     verified: bool
     disabled: bool
     last_login_at: Optional[str] = None
     created_at: str
@@ -679,25 +677,24 @@
 class SessionToken(APIResponseModel):
     id: str
     type: str
     life: int
     expire: str
     identity: str
     email: str
-    scopes: Scopes
+    scopes: Optional[Scopes] = None
     profile: Profile
     created_at: str
 
 
 class SessionItem(APIResponseModel):
     id: str
     type: str
     life: int
     expire: str
-    id: str
     email: str
     scopes: Optional[Scopes] = None
     profile: Profile
     created_at: str
     active_token: Optional[SessionToken] = None
```

### Comparing `pangea_sdk-1.9.1/pangea/services/embargo.py` & `pangea_sdk-2.0.0/pangea/services/embargo.py`

 * *Files 12% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         embargo_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Embargo service
         embargo = Embargo(token=PANGEA_TOKEN, config=embargo_config)
     """
 
     service_name = "embargo"
+    _support_multi_config = False
 
     def ip_check(self, ip: str) -> PangeaResponse[EmbargoResult]:
         """
         Check IP
 
         Check an IP against known sanction and trade embargo lists.
 
@@ -100,18 +101,15 @@
                 response.result field.  Available response fields can be found
                 in our [API Documentation](https://pangea.cloud/docs/api/embargo).
 
         Examples:
             response = embargo.ip_check("190.6.64.94")
         """
         input = IPCheckRequest(ip=ip)
-        response = self.request.post("v1/ip/check", data=input.dict())
-        result = EmbargoResult(**response.raw_result)
-        response.result = result
-        return response
+        return self.request.post("v1/ip/check", EmbargoResult, data=input.dict())
 
     def iso_check(self, iso_code: str) -> PangeaResponse[EmbargoResult]:
         """
         ISO Code Check
 
         Check this country against known sanction and trade embargo lists.
 
@@ -130,10 +128,8 @@
                 response.result field.  Available response fields can be found
                 in our [API Documentation](https://pangea.cloud/docs/api/embargo).
 
         Examples:
             response = embargo.iso_check("CU")
         """
         input = ISOCheckRequest(iso_code=iso_code)
-        response = self.request.post("v1/iso/check", data=input.dict())
-        response.result = EmbargoResult(**response.raw_result)
-        return response
+        return self.request.post("v1/iso/check", result_class=EmbargoResult, data=input.dict())
```

### Comparing `pangea_sdk-1.9.1/pangea/services/intel.py` & `pangea_sdk-2.0.0/pangea/services/intel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright 2022 Pangea Cyber Corporation
 # Author: Pangea Cyber Corporation
 import enum
 import hashlib
+import io
 from typing import Dict, List, Optional
 
-from pangea.deprecated import pangea_deprecated
 from pangea.exceptions import PangeaException
-from pangea.response import APIRequestModel, APIResponseModel, PangeaResponse, PangeaResponseResult
+from pangea.response import APIRequestModel, PangeaResponse, PangeaResponseResult
 
 from .base import ServiceBase
 
 
 class IntelCommonRequest(APIRequestModel):
     """
     Intel common request data
@@ -42,15 +42,15 @@
     hash_type (str): Type of hash, can be "sha256", "sha" or "md5"
     """
 
     hash: str
     hash_type: str
 
 
-class FileReputationData(APIResponseModel):
+class FileReputationData(PangeaResponseResult):
     """
     File reputation information
     """
 
     category: List[str]
     score: int
     verdict: str
@@ -78,15 +78,15 @@
     IP reputation request data
 
     """
 
     pass
 
 
-class IPReputationData(APIResponseModel):
+class IPReputationData(PangeaResponseResult):
     """
     IP reputation information
     """
 
     category: List[str]
     score: int
     verdict: str
@@ -204,15 +204,15 @@
     """
     Domain reputation request data
     """
 
     pass
 
 
-class DomainReputationData(APIResponseModel):
+class DomainReputationData(PangeaResponseResult):
     """
     Domain Reputation information
     """
 
     category: List[str]
     score: int
     verdict: str
@@ -240,15 +240,15 @@
     """
     URL reputation request data
     """
 
     pass
 
 
-class URLReputationData(APIResponseModel):
+class URLReputationData(PangeaResponseResult):
     """
     URL reputation information
     """
 
     category: List[str]
     score: int
     verdict: str
@@ -295,52 +295,17 @@
         file_intel_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea File Intel service
         file_intel = FileIntel(token=PANGEA_TOKEN, config=file_intel_config)
     """
 
     service_name = "file-intel"
+    _support_multi_config = False
 
-    @pangea_deprecated(version="1.2.0", reason="Should use FileIntel.hashReputation()")
-    def lookup(
-        self,
-        hash: str,
-        hash_type: str,
-        provider: Optional[str] = None,
-        verbose: Optional[bool] = None,
-        raw: Optional[bool] = None,
-    ) -> PangeaResponse[FileReputationResult]:
-        """
-        Reputation check
-
-        Retrieve hash-based file reputation from a provider, including an optional detailed report.
-
-        Args:
-            hash (str): The hash of the file to be looked up
-            hash_type (str): One of "sha256", "sha", "md5"
-            provider (str, optional): Use reputation data from these providers: "reversinglabs" or "crowdstrike"
-            verbose (bool, optional): Echo the API parameters in the response
-            raw (bool, optional): Include raw data from this provider
-
-        Raises:
-            PangeaAPIException: If an API Error happens
-
-        Returns:
-            A PangeaResponse where the sanctioned source(s) are in the
-                response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/file-intel).
-
-        Examples:
-            response = file_intel.lookup(hash="142b638c6a60b60c7f9928da4fb85a5a8e1422a9ffdc9ee49e17e56ccca9cf6e", hash_type="sha256", provider="reversinglabs")
-        """
-        input = FileReputationRequest(hash=hash, hash_type=hash_type, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = FileReputationResult(**response.raw_result)
-        return response
-
-    def hashReputation(
+    def hash_reputation(
         self,
         hash: str,
         hash_type: str,
         provider: Optional[str] = None,
         verbose: Optional[bool] = None,
         raw: Optional[bool] = None,
     ) -> PangeaResponse[FileReputationResult]:
@@ -364,57 +329,17 @@
                 response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/file-intel).
 
         Examples:
             response = file_intel.hashReputation(hash="142b638c6a60b60c7f9928da4fb85a5a8e1422a9ffdc9ee49e17e56ccca9cf6e", hash_type="sha256", provider="reversinglabs")
 
         """
         input = FileReputationRequest(hash=hash, hash_type=hash_type, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = FileReputationResult(**response.raw_result)
-        return response
-
-    @pangea_deprecated(version="1.2.0", reason="Should use FileIntel.filepathReputation()")
-    def lookupFilepath(
-        self,
-        filepath: str,
-        provider: Optional[str] = None,
-        verbose: Optional[bool] = None,
-        raw: Optional[bool] = None,
-    ) -> PangeaResponse[FileReputationResult]:
-        """
-        Reputation, from filepath
-
-        Retrieve hash-based file reputation from a provider, including an optional detailed report.
-
-        Args:
-            filepath (str): The path to the file to be looked up
-            provider (str, optional): Use reputation data from these providers: "reversinglabs" or "crowdstrike"
-            verbose (bool, optional): Echo the API parameters in the response
-            raw (bool, optional): Include raw data from this provider
-
-        Raises:
-            PangeaAPIException: If an API Error happens
-
-        Returns:
-            A PangeaResponse where the sanctioned source(s) are in the
-                response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/file-intel).
-
-        Examples:
-            response = file_intel.lookupFilepath(filepath="./myfile.exe", provider="reversinglabs"))
-        """
-
-        data = open(filepath, "rb")
-        hash = hashlib.sha256(data.read()).hexdigest()
+        return self.request.post("v1/reputation", FileReputationResult, data=input.dict(exclude_none=True))
 
-        input = FileReputationRequest(hash=hash, hash_type="sha256", verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = FileReputationResult(**response.raw_result)
-        return response
-
-    def filepathReputation(
+    def filepath_reputation(
         self,
         filepath: str,
         provider: Optional[str] = None,
         verbose: Optional[bool] = None,
         raw: Optional[bool] = None,
     ) -> PangeaResponse[FileReputationResult]:
         """
@@ -445,17 +370,15 @@
             )
         """
 
         data = open(filepath, "rb")
         hash = hashlib.sha256(data.read()).hexdigest()
 
         input = FileReputationRequest(hash=hash, hash_type="sha256", verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = FileReputationResult(**response.raw_result)
-        return response
+        return self.request.post("v1/reputation", FileReputationResult, data=input.dict(exclude_none=True))
 
 
 class DomainIntel(ServiceBase):
     """Domain Intel service client
 
     Provides methods to interact with [Pangea Domain Intel Service](https://pangea.cloud/docs/api/domain-intel)
 
@@ -475,44 +398,15 @@
         domain_intel_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Domain Intel service
         domain_intel = DomainIntel(token=PANGEA_TOKEN, config=domain_intel_config)
     """
 
     service_name = "domain-intel"
-
-    @pangea_deprecated(version="1.2.0", reason="Should use DomainIntel.reputation()")
-    def lookup(
-        self, domain: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
-    ) -> PangeaResponse[DomainReputationResult]:
-        """
-        Reputation check
-
-        Retrieve reputation for a domain from a provider, including an optional detailed report.
-
-        Args:
-            domain (str): The domain to be looked up
-            provider (str, optional): Use reputation data from these providers: "domaintools" or "crowdstrike"
-            verbose (bool, optional): Echo the API parameters in the response
-            raw (bool, optional): Include raw data from this provider
-
-        Raises:
-            PangeaAPIException: If an API Error happens
-
-        Returns:
-            A PangeaResponse where the sanctioned source(s) are in the
-                response.result field.  Available response fields can be found in our [API documentation](https://pangea.cloud/docs/api/domain-intel).
-
-        Examples:
-            response = domain_intel.lookup(domain="737updatesboeing.com", provider="domaintools")
-        """
-        input = DomainReputationRequest(domain=domain, verbose=verbose, provider=provider, raw=raw)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = DomainReputationResult(**response.raw_result)
-        return response
+    _support_multi_config = False
 
     def reputation(
         self, domain: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[DomainReputationResult]:
         """
         Reputation
 
@@ -536,17 +430,15 @@
         Examples:
             response = domain_intel.lookup(
                 domain="737updatesboeing.com",
                 provider="domaintools",
             )
         """
         input = DomainReputationRequest(domain=domain, verbose=verbose, provider=provider, raw=raw)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = DomainReputationResult(**response.raw_result)
-        return response
+        return self.request.post("v1/reputation", DomainReputationResult, data=input.dict(exclude_none=True))
 
 
 class IpIntel(ServiceBase):
     """IP Intel service client
 
     Provides methods to interact with [Pangea IP Intel Service](/docs/api/ip-intel)
 
@@ -566,45 +458,15 @@
         ip_intel_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea IP Intel service
         ip_intel = IpIntel(token=PANGEA_TOKEN, config=ip_intel_config)
     """
 
     service_name = "ip-intel"
-
-    @pangea_deprecated(version="1.2.0", reason="Should use IpIntel.reputation()")
-    def lookup(
-        self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
-    ) -> PangeaResponse[IPReputationResult]:
-        """
-        Reputation
-
-        Retrieve a reputation score for an IP address from a provider, including an optional detailed report.
-
-        Args:
-            ip (str): The IP to be looked up
-            verbose (bool, optional): Echo the API parameters in the response
-            raw (bool, optional): Include raw data from this provider
-            provider (str, optional): Use reputation data from this provider: "crowdstrike"
-
-        Raises:
-            PangeaAPIException: If an API Error happens
-
-        Returns:
-            A PangeaResponse where the sanctioned source(s) are in the
-                response.result field.  Available response fields can be found in our [API documentation](/docs/api/ip-intel)
-
-        Examples:
-            response = ip_intel.lookup(ip="93.231.182.110", provider="crowdstrike")
-
-        """
-        input = IPRepurationRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = IPReputationResult(**response.raw_result)
-        return response
+    _support_multi_config = False
 
     def reputation(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPReputationResult]:
         """
         Reputation
 
@@ -628,17 +490,15 @@
         Examples:
             response = ip_intel.reputation(
                 ip="93.231.182.110",
                 provider="crowdstrike",
             )
         """
         input = IPRepurationRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = IPReputationResult(**response.raw_result)
-        return response
+        return self.request.post("v1/reputation", IPReputationResult, data=input.dict(exclude_none=True))
 
     def geolocate(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPGeolocateResult]:
         """
         Geolocate
 
@@ -662,17 +522,15 @@
         Examples:
             response = ip_intel.geolocate(
                 ip="93.231.182.110",
                 provider="digitalelement",
             )
         """
         input = IPGeolocateRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/geolocate", data=input.dict(exclude_none=True))
-        response.result = IPGeolocateResult(**response.raw_result)
-        return response
+        return self.request.post("v1/geolocate", IPGeolocateResult, data=input.dict(exclude_none=True))
 
     def get_domain(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPDomainResult]:
         """
         Domain
 
@@ -696,17 +554,15 @@
         Examples:
             response = ip_intel.get_domain(
                 ip="93.231.182.110",
                 provider="digitalelement",
             )
         """
         input = IPDomainRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/domain", data=input.dict(exclude_none=True))
-        response.result = IPDomainResult(**response.raw_result)
-        return response
+        return self.request.post("v1/domain", IPDomainResult, data=input.dict(exclude_none=True))
 
     def is_vpn(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPVPNResult]:
         """
         VPN
 
@@ -730,17 +586,15 @@
         Examples:
             response = ip_intel.is_vpn(
                 ip="93.231.182.110",
                 provider="digitalelement",
             )
         """
         input = IPVPNRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/vpn", data=input.dict(exclude_none=True))
-        response.result = IPVPNResult(**response.raw_result)
-        return response
+        return self.request.post("v1/vpn", IPVPNResult, data=input.dict(exclude_none=True))
 
     def is_proxy(
         self, ip: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[IPProxyResult]:
         """
         Proxy
 
@@ -764,17 +618,15 @@
         Examples:
             response = ip_intel.is_proxy(
                 ip="93.231.182.110",
                 provider="digitalelement",
             )
         """
         input = IPProxyRequest(ip=ip, verbose=verbose, raw=raw, provider=provider)
-        response = self.request.post("v1/proxy", data=input.dict(exclude_none=True))
-        response.result = IPProxyResult(**response.raw_result)
-        return response
+        return self.request.post("v1/proxy", IPProxyResult, data=input.dict(exclude_none=True))
 
 
 class UrlIntel(ServiceBase):
     """URL Intel service client.
 
     Provides methods to interact with [Pangea URL Intel Service](/docs/api/url-intel)
 
@@ -794,45 +646,15 @@
         url_intel_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea URL Intel service
         url_intel = UrlIntel(token=PANGEA_TOKEN, config=url_intel_config)
     """
 
     service_name = "url-intel"
-
-    @pangea_deprecated(version="1.2.0", reason="Should use UrlIntel.reputation()")
-    def lookup(
-        self, url: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
-    ) -> PangeaResponse[URLReputationResult]:
-        """
-        Reputation check
-
-        Retrieve URL address reputation from a provider.
-
-        Args:
-            url (str): The URL to be looked up
-            verbose (bool, optional): Echo the API parameters in the response
-            raw (bool, optional): Include raw data from this provider
-            provider (str, optional): Use reputation data from this provider: "crowdstrike"
-
-        Raises:
-            PangeaAPIException: If an API Error happens
-
-        Returns:
-            A PangeaResponse where the sanctioned source(s) are in the
-                response.result field.  Available response fields can be found in our [API documentation](/docs/api/url-intel)
-
-        Examples:
-            response = url_intel.lookup(url="http://113.235.101.11:54384", provider="crowdstrike")
-        """
-
-        input = URLReputationRequest(url=url, provider=provider, verbose=verbose, raw=raw)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = URLReputationResult(**response.raw_result)
-        return response
+    _support_multi_config = False
 
     def reputation(
         self, url: str, verbose: Optional[bool] = None, raw: Optional[bool] = None, provider: Optional[str] = None
     ) -> PangeaResponse[URLReputationResult]:
         """
         Reputation
 
@@ -857,17 +679,15 @@
             response = url_intel.reputation(
                 url="http://113.235.101.11:54384",
                 provider="crowdstrike",
             )
         """
 
         input = URLReputationRequest(url=url, provider=provider, verbose=verbose, raw=raw)
-        response = self.request.post("v1/reputation", data=input.dict(exclude_none=True))
-        response.result = URLReputationResult(**response.raw_result)
-        return response
+        return self.request.post("v1/reputation", URLReputationResult, data=input.dict(exclude_none=True))
 
 
 class UserBreachedRequest(IntelCommonRequest):
     """
     User breached common request data
 
     email (str): An email address to search for
@@ -882,15 +702,15 @@
     username: Optional[str] = None
     ip: Optional[str] = None
     phone_number: Optional[str] = None
     start: Optional[str] = None
     end: Optional[str] = None
 
 
-class UserBreachedCommonData(APIResponseModel):
+class UserBreachedCommonData(PangeaResponseResult):
     """
     User breached common information
     """
 
     found_in_breach: bool
     breach_count: int
 
@@ -960,14 +780,15 @@
         user_intel_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea User Intel service
         user_intel = UserIntel(token=PANGEA_TOKEN, config=user_intel_config)
     """
 
     service_name = "user-intel"
+    _support_multi_config = False
 
     def user_breached(
         self,
         email: Optional[str] = None,
         username: Optional[str] = None,
         ip: Optional[str] = None,
         phone_number: Optional[str] = None,
@@ -1018,17 +839,15 @@
             ip=ip,
             provider=provider,
             start=start,
             end=end,
             verbose=verbose,
             raw=raw,
         )
-        response = self.request.post("v1/user/breached", data=input.dict(exclude_none=True))
-        response.result = UserBreachedResult(**response.raw_result)
-        return response
+        return self.request.post("v1/user/breached", UserBreachedResult, data=input.dict(exclude_none=True))
 
     def password_breached(
         self,
         hash_type: HashType,
         hash_prefix: str,
         verbose: Optional[bool] = None,
         raw: Optional[bool] = True,
@@ -1062,17 +881,15 @@
                 provider="spycloud",
             )
         """
 
         input = UserPasswordBreachedRequest(
             hash_type=hash_type, hash_prefix=hash_prefix, provider=provider, verbose=verbose, raw=raw
         )
-        response = self.request.post("v1/password/breached", data=input.dict(exclude_none=True))
-        response.result = UserPasswordBreachedResult(**response.raw_result)
-        return response
+        return self.request.post("v1/password/breached", UserPasswordBreachedResult, data=input.dict(exclude_none=True))
 
     class PasswordStatus(enum.Enum):
         BREACHED = 0
         UNBREACHED = 1
         INCONCLUSIVE = 2
 
     @staticmethod
```

### Comparing `pangea_sdk-1.9.1/pangea/services/redact.py` & `pangea_sdk-2.0.0/pangea/services/redact.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         redact_config = PangeaConfig(domain="aws.us.pangea.cloud")
 
         # Setup Pangea Redact service client
         redact = Redact(token=PANGEA_TOKEN, config=redact_config)
     """
 
     service_name = "redact"
+    _support_multi_config = False
 
     def __init__(
         self,
         token,
         config=None,
         logger_name="pangea",
     ):
@@ -170,17 +171,15 @@
                 [API Documentation](https://pangea.cloud/docs/api/redact#redact).
 
         Examples:
             response = redact.redact(text="Jenny Jenny... 555-867-5309")
         """
 
         input = RedactRequest(text=text, debug=debug, rules=rules, return_result=return_result)
-        response = self.request.post("v1/redact", data=input.dict(exclude_none=True))
-        response.result = RedactResult(**response.raw_result)
-        return response
+        return self.request.post("v1/redact", RedactResult, data=input.dict(exclude_none=True))
 
     def redact_structured(
         self,
         data: Union[Dict, str],
         jsonp: Optional[List[str]] = None,
         format: Optional[RedactFormat] = None,
         debug: Optional[bool] = None,
@@ -221,10 +220,8 @@
 
             response = redact.redact_structured(data=data, redact_format="json")
         """
 
         input = StructuredRequest(
             data=data, jsonp=jsonp, format=format, debug=debug, rules=rules, return_result=return_result
         )
-        response = self.request.post("v1/redact_structured", data=input.dict(exclude_none=True))
-        response.result = StructuredResult(**response.raw_result)
-        return response
+        return self.request.post("v1/redact_structured", StructuredResult, data=input.dict(exclude_none=True))
```

### Comparing `pangea_sdk-1.9.1/pangea/services/vault/models/asymmetric.py` & `pangea_sdk-2.0.0/pangea/services/vault/models/asymmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pangea/services/vault/models/common.py` & `pangea_sdk-2.0.0/pangea/services/vault/models/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,15 +280,15 @@
     rotation_frequency: Optional[str] = None
     rotation_state: Optional[ItemVersionState] = None
     rotation_grace_period: Optional[str] = None
     expiration: Optional[datetime.datetime] = None
     item_state: Optional[ItemState] = None
 
 
-class UpdateResult(APIRequestModel):
+class UpdateResult(PangeaResponseResult):
     id: str
 
 
 class JWKGetRequest(APIRequestModel):
     id: str
     version: Optional[str] = None
```

### Comparing `pangea_sdk-1.9.1/pangea/services/vault/models/symmetric.py` & `pangea_sdk-2.0.0/pangea/services/vault/models/symmetric.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pangea/services/vault/vault.py` & `pangea_sdk-2.0.0/pangea/services/vault/vault.py`

 * *Files 15% similar despite different names*

```diff
@@ -85,15 +85,16 @@
         PANGEA_VAULT_TOKEN = os.getenv("PANGEA_VAULT_TOKEN")
         vault_config = PangeaConfig(domain="pangea.cloud")
 
         # Setup Pangea Vault service
         vault = Vault(token=PANGEA_VAULT_TOKEN, config=audit_config)
     """
 
-    service_name: str = "vault"
+    service_name = "vault"
+    _support_multi_config = False
 
     def __init__(
         self,
         token,
         config=None,
         logger_name="pangea",
     ):
@@ -120,18 +121,15 @@
 
         Examples:
             vault.delete(id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5")
         """
         input = DeleteRequest(
             id=id,
         )
-        response = self.request.post("v1/delete", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = DeleteResult(**response.raw_result)
-        return response
+        return self.request.post("v1/delete", DeleteResult, data=input.dict(exclude_none=True))
 
     # Get endpoint
     def get(
         self,
         id: str,
         version: Optional[Union[str, int]] = None,
         version_state: Optional[ItemVersionState] = None,
@@ -170,18 +168,15 @@
         """
         input = GetRequest(
             id=id,
             version=version,
             verbose=verbose,
             version_state=version_state,
         )
-        response = self.request.post("v1/get", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = GetResult(**response.raw_result)
-        return response
+        return self.request.post("v1/get", GetResult, data=input.dict(exclude_none=True))
 
     # List endpoint
     def list(
         self,
         filter: Optional[Dict[str, str]] = None,
         last: Optional[str] = None,
         order: Optional[ItemOrder] = None,
@@ -229,19 +224,15 @@
                 last="WyIvdGVzdF8yMDdfc3ltbWV0cmljLyJd",
                 order=ItemOrder.ASC,
                 order_by=ItemOrderBy.NAME,
                 size=20,
             )
         """
         input = ListRequest(filter=filter, last=last, order=order, order_by=order_by, size=size)
-        response = self.request.post("v1/list", data=input.dict(exclude_none=True))
-
-        if response.raw_result is not None:
-            response.result = ListResult(**response.raw_result)
-        return response
+        return self.request.post("v1/list", ListResult, data=input.dict(exclude_none=True))
 
     # Update endpoint
     def update(
         self,
         id: str,
         name: Optional[str] = None,
         folder: Optional[str] = None,
@@ -314,18 +305,15 @@
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             rotation_grace_period=rotation_grace_period,
             expiration=expiration,
             item_state=item_state,
         )
-        response = self.request.post("v1/update", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = UpdateResult(**response.raw_result)
-        return response
+        return self.request.post("v1/update", UpdateResult, data=input.dict(exclude_none=True))
 
     def secret_store(
         self,
         secret: str,
         name: str,
         folder: Optional[str] = None,
         metadata: Optional[Metadata] = None,
@@ -387,18 +375,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("v1/secret/store", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = SecretStoreResult(**response.raw_result)
-        return response
+        return self.request.post("v1/secret/store", SecretStoreResult, data=input.dict(exclude_none=True))
 
     def pangea_token_store(
         self,
         pangea_token: str,
         name: str,
         folder: Optional[str] = None,
         metadata: Optional[Metadata] = None,
@@ -460,18 +445,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("v1/secret/store", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = SecretStoreResult(**response.raw_result)
-        return response
+        return self.request.post("v1/secret/store", SecretStoreResult, data=input.dict(exclude_none=True))
 
     # Rotate endpoint
     def secret_rotate(
         self, id: str, secret: str, rotation_state: Optional[ItemVersionState] = None
     ) -> PangeaResponse[SecretRotateResult]:
         """
         Secret rotate
@@ -503,18 +485,15 @@
             response = vault.secret_rotate(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 secret="12sdfgs4543qv@#%$casd",
                 rotation_state=ItemVersionState.DEACTIVATED,
             )
         """
         input = SecretRotateRequest(id=id, secret=secret, rotation_state=rotation_state)
-        response = self.request.post("v1/secret/rotate", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = SecretRotateResult(**response.raw_result)
-        return response
+        return self.request.post("v1/secret/rotate", SecretRotateResult, data=input.dict(exclude_none=True))
 
     # Rotate endpoint
     def pangea_token_rotate(self, id: str) -> PangeaResponse[SecretRotateResult]:
         """
         Token rotate
 
         Rotate a Pangea token
@@ -534,18 +513,15 @@
 
         Examples:
             response = vault.pangea_token_rotate(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
             )
         """
         input = SecretRotateRequest(id=id)
-        response = self.request.post("v1/secret/rotate", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = SecretRotateResult(**response.raw_result)
-        return response
+        return self.request.post("v1/secret/rotate", SecretRotateResult, data=input.dict(exclude_none=True))
 
     def symmetric_generate(
         self,
         algorithm: SymmetricAlgorithm,
         purpose: KeyPurpose,
         name: Optional[str] = None,
         folder: Optional[str] = None,
@@ -611,18 +587,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("v1/key/generate", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = SymmetricGenerateResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/generate", SymmetricGenerateResult, data=input.dict(exclude_none=True))
 
     def asymmetric_generate(
         self,
         algorithm: AsymmetricAlgorithm,
         purpose: KeyPurpose,
         name: Optional[str] = None,
         folder: Optional[str] = None,
@@ -688,18 +661,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("v1/key/generate", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = AsymmetricGenerateResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/generate", AsymmetricGenerateResult, data=input.dict(exclude_none=True))
 
     # Store endpoints
     def asymmetric_store(
         self,
         private_key: EncodedPrivateKey,
         public_key: EncodedPublicKey,
         algorithm: AsymmetricAlgorithm,
@@ -774,18 +744,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("v1/key/store", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = AsymmetricStoreResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/store", AsymmetricStoreResult, data=input.dict(exclude_none=True))
 
     def symmetric_store(
         self,
         key: str,
         algorithm: SymmetricAlgorithm,
         purpose: KeyPurpose,
         name: str,
@@ -855,18 +822,15 @@
             folder=folder,
             metadata=metadata,
             tags=tags,
             rotation_frequency=rotation_frequency,
             rotation_state=rotation_state,
             expiration=expiration,
         )
-        response = self.request.post("v1/key/store", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = SymmetricStoreResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/store", SymmetricStoreResult, data=input.dict(exclude_none=True))
 
     # Rotate endpoint
     def key_rotate(
         self,
         id: str,
         rotation_state: ItemVersionState,
         public_key: Optional[EncodedPublicKey] = None,
@@ -907,18 +871,15 @@
                 rotation_state=ItemVersionState.DEACTIVATED,
                 key="lJkk0gCLux+Q+rPNqLPEYw==",
             )
         """
         input = KeyRotateRequest(
             id=id, public_key=public_key, private_key=private_key, key=key, rotation_state=rotation_state
         )
-        response = self.request.post("v1/key/rotate", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = KeyRotateResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/rotate", KeyRotateResult, data=input.dict(exclude_none=True))
 
     # Encrypt
     def encrypt(self, id: str, plain_text: str, version: Optional[int] = None) -> PangeaResponse[EncryptResult]:
         """
         Encrypt
 
         Encrypt a message using a key
@@ -942,18 +903,15 @@
             response = vault.encrypt(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 plain_text="lJkk0gCLux+Q+rPNqLPEYw==",
                 version=1,
             )
         """
         input = EncryptRequest(id=id, plain_text=plain_text, version=version)
-        response = self.request.post("v1/key/encrypt", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = EncryptResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/encrypt", EncryptResult, data=input.dict(exclude_none=True))
 
     # Decrypt
     def decrypt(self, id: str, cipher_text: str, version: Optional[int] = None) -> PangeaResponse[DecryptResult]:
         """
         Decrypt
 
         Decrypt a message using a key
@@ -977,18 +935,15 @@
             response = vault.decrypt(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 cipher_text="lJkk0gCLux+Q+rPNqLPEYw==",
                 version=1,
             )
         """
         input = DecryptRequest(id=id, cipher_text=cipher_text, version=version)
-        response = self.request.post("v1/key/decrypt", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = DecryptResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/decrypt", DecryptResult, data=input.dict(exclude_none=True))
 
     # Sign
     def sign(self, id: str, message: str, version: Optional[int] = None) -> PangeaResponse[SignResult]:
         """
         Sign
 
         Sign a message using a key
@@ -1012,18 +967,15 @@
             response = vault.sign(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 message="lJkk0gCLux+Q+rPNqLPEYw==",
                 version=1,
             )
         """
         input = SignRequest(id=id, message=message, version=version)
-        response = self.request.post("v1/key/sign", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = SignResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/sign", SignResult, data=input.dict(exclude_none=True))
 
     # Verify
     def verify(
         self, id: str, message: str, signature: str, version: Optional[int] = None
     ) -> PangeaResponse[VerifyResult]:
         """
         Verify
@@ -1056,18 +1008,15 @@
         """
         input = VerifyRequest(
             id=id,
             message=message,
             signature=signature,
             version=version,
         )
-        response = self.request.post("v1/key/verify", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = VerifyResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/verify", VerifyResult, data=input.dict(exclude_none=True))
 
     def jwt_verify(self, jws: str) -> PangeaResponse[JWTVerifyResult]:
         """
         JWT Verify
 
         Verify the signature of a JSON Web Token (JWT)
 
@@ -1086,18 +1035,15 @@
 
         Examples:
             response = vault.jwt_verify(
                 jws="ewogICJhbGciO...",
             )
         """
         input = JWTVerifyRequest(jws=jws)
-        response = self.request.post("v1/key/verify/jwt", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = JWTVerifyResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/verify/jwt", JWTVerifyResult, data=input.dict(exclude_none=True))
 
     def jwt_sign(self, id: str, payload: str) -> PangeaResponse[JWTSignResult]:
         """
         JWT Sign
 
         Sign a JSON Web Token (JWT) using a key
 
@@ -1118,18 +1064,15 @@
         Examples:
             response = vault.jwt_sign(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 payload="{\\"sub\\": \\"1234567890\\",\\"name\\": \\"John Doe\\",\\"admin\\": true}"
             )
         """
         input = JWTSignRequest(id=id, payload=payload)
-        response = self.request.post("v1/key/sign/jwt", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = JWTSignResult(**response.raw_result)
-        return response
+        return self.request.post("v1/key/sign/jwt", JWTSignResult, data=input.dict(exclude_none=True))
 
     # Get endpoint
     def jwk_get(self, id: str, version: Optional[str] = None) -> PangeaResponse[JWKGetResult]:
         """
         JWT Retrieve
 
         Retrieve a key in JWK format
@@ -1152,18 +1095,15 @@
 
         Examples:
             response = vault.jwk_get(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
             )
         """
         input = JWKGetRequest(id=id, version=version)
-        response = self.request.post("v1/get/jwk", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = JWKGetResult(**response.raw_result)
-        return response
+        return self.request.post("v1/get/jwk", JWKGetResult, data=input.dict(exclude_none=True))
 
     # State change
     def state_change(
         self, id: str, state: ItemVersionState, version: Optional[int] = None, destroy_period: Optional[str] = None
     ) -> PangeaResponse[StateChangeResult]:
         """
         State change
@@ -1194,11 +1134,8 @@
         Examples:
             response = vault.state_change(
                 id="pvi_p6g5i3gtbvqvc3u6zugab6qs6r63tqf5",
                 state=ItemVersionState.DEACTIVATED,
             )
         """
         input = StateChangeRequest(id=id, state=state, version=version, destroy_period=destroy_period)
-        response = self.request.post("v1/state/change", data=input.dict(exclude_none=True))
-        if response.raw_result is not None:
-            response.result = StateChangeResult(**response.raw_result)
-        return response
+        return self.request.post("v1/state/change", StateChangeResult, data=input.dict(exclude_none=True))
```

### Comparing `pangea_sdk-1.9.1/pangea/tools.py` & `pangea_sdk-2.0.0/pangea/tools.py`

 * *Files 23% similar despite different names*

```diff
@@ -112,34 +112,59 @@
         return d
 
 
 def filter_deep_none(data: t.Dict) -> t.Dict:
     return {k: v if not isinstance(v, t.Dict) else filter_deep_none(v) for k, v in data.items() if v is not None}
 
 
-def get_test_domain(environment: TestEnvironment):
-    env_var_name = f"PANGEA_INTEGRATION_DOMAIN_{environment}"
+def _load_env_var(env_var_name: str):
     value = os.getenv(env_var_name)
     if not value:
         raise PangeaException(f"{env_var_name} env var need to be set")
 
     return value
 
 
+def get_test_domain(environment: TestEnvironment):
+    env_var_name = f"PANGEA_INTEGRATION_DOMAIN_{environment}"
+    return _load_env_var(env_var_name)
+
+
 def get_test_token(environment: TestEnvironment):
     env_var_name = f"PANGEA_INTEGRATION_TOKEN_{environment}"
+    return _load_env_var(env_var_name)
+
+
+def get_vault_signature_test_token(environment: TestEnvironment):
+    env_var_name = f"PANGEA_INTEGRATION_VAULT_TOKEN_{environment}"
+    return _load_env_var(env_var_name)
+
+
+def get_multi_config_test_token(environment: TestEnvironment):
+    env_var_name = f"PANGEA_INTEGRATION_MULTI_CONFIG_TOKEN_{environment}"
+    return _load_env_var(env_var_name)
+
+
+def get_config_id(environment: TestEnvironment, service: str, config_number: int):
+    service = service.upper()
+    env_var_name = f"PANGEA_{service}_CONFIG_ID_{config_number}_{environment}"
+    return _load_env_var(env_var_name)
+
+
+def get_custom_schema_test_token(environment: TestEnvironment):
+    env_var_name = f"PANGEA_INTEGRATION_CUSTOM_SCHEMA_TOKEN_{environment}"
     value = os.getenv(env_var_name)
     if not value:
         raise PangeaException(f"{env_var_name} env var need to be set")
 
     return value
 
 
-def get_vault_signature_test_token(environment: TestEnvironment):
-    env_var_name = f"PANGEA_INTEGRATION_VAULT_TOKEN_{environment}"
+def get_custom_schema_vault_test_token(environment: TestEnvironment):
+    env_var_name = f"PANGEA_INTEGRATION_CUSTOM_SCHEMA_TOKEN_{environment}"
     value = os.getenv(env_var_name)
     if not value:
         raise PangeaException(f"{env_var_name} env var need to be set")
 
     return value
```

### Comparing `pangea_sdk-1.9.1/pangea/verify_audit.py` & `pangea_sdk-2.0.0/pangea/verify_audit.py`

 * *Files identical despite different names*

### Comparing `pangea_sdk-1.9.1/pyproject.toml` & `pangea_sdk-2.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pangea-sdk"
-version = "1.9.1"
+version = "2.0.0"
 description = "Pangea API SDK"
 authors = ["Glenn Gallien <glenn.gallien@pangea.cloud>"]
 license = "MIT"
 readme = "README.md"
 homepage = ""
 repository = ""
 keywords = ["Pangea", "SDK", "Audit"]
@@ -15,15 +15,15 @@
 packages = [
     { include = "pangea" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
 requests = "^2.31.0"
-cryptography = "39.0.1"
+cryptography = "41.0.0"
 schema = "^0.7.5"
 python-dateutil = "^2.8.2"
 alive-progress = "^2.4.1"
 pydantic = "^1.10.2"
 pytest = "^7.2.0"
 deprecated = "^1.2.13"
```

