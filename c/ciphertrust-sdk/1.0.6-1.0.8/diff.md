# Comparing `tmp/ciphertrust-sdk-1.0.6.tar.gz` & `tmp/ciphertrust-sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciphertrust-sdk-1.0.6.tar", last modified: Wed Jun 28 00:52:54 2023, max compression
+gzip compressed data, was "ciphertrust-sdk-1.0.8.tar", last modified: Thu Jul  6 17:02:36 2023, max compression
```

## Comparing `ciphertrust-sdk-1.0.6.tar` & `ciphertrust-sdk-1.0.8.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-28 00:52:54.573445 ciphertrust-sdk-1.0.6/
--rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/LICENSE
--rw-r--r--   0 adamt      (501) staff       (20)     5520 2023-06-28 00:52:54.572741 ciphertrust-sdk-1.0.6/PKG-INFO
--rw-rw-r--   0 adamt      (501) staff       (20)     3837 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/README.md
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-28 00:52:54.563877 ciphertrust-sdk-1.0.6/ciphertrust_sdk.egg-info/
--rw-r--r--   0 adamt      (501) staff       (20)     5520 2023-06-28 00:52:54.000000 ciphertrust-sdk-1.0.6/ciphertrust_sdk.egg-info/PKG-INFO
--rw-r--r--   0 adamt      (501) staff       (20)      492 2023-06-28 00:52:54.000000 ciphertrust-sdk-1.0.6/ciphertrust_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 adamt      (501) staff       (20)        1 2023-06-28 00:52:54.000000 ciphertrust-sdk-1.0.6/ciphertrust_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 adamt      (501) staff       (20)       94 2023-06-28 00:52:54.000000 ciphertrust-sdk-1.0.6/ciphertrust_sdk.egg-info/requires.txt
--rw-r--r--   0 adamt      (501) staff       (20)       12 2023-06-28 00:52:54.000000 ciphertrust-sdk-1.0.6/ciphertrust_sdk.egg-info/top_level.txt
--rw-rw-r--   0 adamt      (501) staff       (20)     1054 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/pyproject.toml
--rw-r--r--   0 adamt      (501) staff       (20)       38 2023-06-28 00:52:54.573683 ciphertrust-sdk-1.0.6/setup.cfg
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-28 00:52:54.558964 ciphertrust-sdk-1.0.6/src/
-drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-06-28 00:52:54.571627 ciphertrust-sdk-1.0.6/src/ciphertrust/
--rw-rw-r--   0 adamt      (501) staff       (20)      134 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/__init__.py
--rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/_version.py
--rw-rw-r--   0 adamt      (501) staff       (20)     6593 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/api.py
--rw-rw-r--   0 adamt      (501) staff       (20)     8102 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/auth.py
--rw-rw-r--   0 adamt      (501) staff       (20)      248 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/config.py
--rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/exceptions.py
--rw-rw-r--   0 adamt      (501) staff       (20)     3752 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/models.py
--rw-rw-r--   0 adamt      (501) staff       (20)    12567 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/requestapi.py
--rw-rw-r--   0 adamt      (501) staff       (20)      417 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/static.py
--rw-rw-r--   0 adamt      (501) staff       (20)     7111 2023-06-28 00:46:57.000000 ciphertrust-sdk-1.0.6/src/ciphertrust/utils.py
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.921940 ciphertrust-sdk-1.0.8/
+-rw-rw-r--   0 adamt      (501) staff       (20)     1064 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/LICENSE
+-rw-r--r--   0 adamt      (501) staff       (20)    17591 2023-07-06 17:02:36.921300 ciphertrust-sdk-1.0.8/PKG-INFO
+-rw-rw-r--   0 adamt      (501) staff       (20)    15908 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/README.md
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.914054 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/
+-rw-r--r--   0 adamt      (501) staff       (20)    17591 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 adamt      (501) staff       (20)      509 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 adamt      (501) staff       (20)        1 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       94 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/requires.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       12 2023-07-06 17:02:36.000000 ciphertrust-sdk-1.0.8/ciphertrust_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 adamt      (501) staff       (20)     1021 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/pyproject.toml
+-rw-rw-r--   0 adamt      (501) staff       (20)       93 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/requirements.txt
+-rw-r--r--   0 adamt      (501) staff       (20)       38 2023-07-06 17:02:36.922103 ciphertrust-sdk-1.0.8/setup.cfg
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.909491 ciphertrust-sdk-1.0.8/src/
+drwxr-xr-x   0 adamt      (501) staff       (20)        0 2023-07-06 17:02:36.920490 ciphertrust-sdk-1.0.8/src/ciphertrust/
+-rw-rw-r--   0 adamt      (501) staff       (20)     1376 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/__init__.py
+-rw-rw-r--   0 adamt      (501) staff       (20)       42 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/_version.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     7953 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/api.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    13595 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/auth.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     1472 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/config.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      471 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/exceptions.py
+-rw-rw-r--   0 adamt      (501) staff       (20)     9482 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/models.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    15234 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/requestapi.py
+-rw-rw-r--   0 adamt      (501) staff       (20)      729 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/static.py
+-rw-rw-r--   0 adamt      (501) staff       (20)    10643 2023-07-06 16:49:06.000000 ciphertrust-sdk-1.0.8/src/ciphertrust/utils.py
```

### Comparing `ciphertrust-sdk-1.0.6/LICENSE` & `ciphertrust-sdk-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ciphertrust-sdk-1.0.6/pyproject.toml` & `ciphertrust-sdk-1.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 [build-system]
 build-backend= "setuptools.build_meta"
-requires = ["setuptools", "wheel", "attrs"]
+requires = [
+    "setuptools",
+    "wheel",
+    "attrs",
+    "PyYAML==6.0",
+    "py-easy-logger==0.0.3"
+]
 
 [project]
 name = "ciphertrust-sdk"
 authors = [
     {name = "atav928", email = "dev@tavnets.com"}
 ]
 description = "Thales CipherTrust SDK RestAPI"
@@ -12,25 +18,18 @@
 license = {file = "LICENSE", content-type = "text"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: Implementation",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
-dynamic = ["version", "readme"]
-dependencies = [
-    "orjson==3.8.*",
-    "PyJWT==2.7.*",
-    "requests==2.31.*",
-    "dataclasses==0.6",
-    "validators==0.20.*",
-    "httpx==0.24.*"
-]
+dynamic = ["version", "readme", "dependencies"]
 
 [tool.setuptools.dynamic]
+dependencies = {file = "requirements.txt"}
 readme = {file = ["README.md"], content-type = "text/markdown"}
 version = {attr = "ciphertrust.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src", "tests"]
 include = ["ciphertrust"]
 exclude = ["*.xml"]
```

### Comparing `ciphertrust-sdk-1.0.6/src/ciphertrust/requestapi.py` & `ciphertrust-sdk-1.0.8/src/ciphertrust/requestapi.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,143 +1,162 @@
 """Request API"""
 
 from typing import Any, Dict, List
+import re
 import json
 import os
-import time
 import datetime
 import statistics
 import asyncio
 import copy
 from functools import reduce
 from pathlib import Path
 import urllib.parse
+from dateutil import parser
 
 import orjson
 import httpx
 import requests
-from requests import HTTPError, Response
+from requests import HTTPError, Response, ReadTimeout
 
+from easy_logger.log_format import splunk_format
+
+from ciphertrust import logger
 from ciphertrust.auth import (Auth, refresh_token)  # type: ignore
-from ciphertrust.exceptions import (CipherAPIError, CipherMissingParam)
-from ciphertrust.static import (DEFAULT_HEADERS, ENCODE,
+from ciphertrust.exceptions import (CipherMissingParam)
+from ciphertrust.static import (DEFAULT_HEADERS, ENCODE, REGEX_NUM,
                                 DEFAULT_LIMITS_OVERRIDE, DEFAULT_TIMEOUT_CONFIG_OVERRIDE)
-from ciphertrust.utils import (reformat_exception, concat_resources,  # type: ignore
-                               verify_path_exists)
+from ciphertrust.utils import (convert_to_epoch, reformat_exception, concat_resources,  # type: ignore
+                               verify_path_exists, return_time, create_error_response)
+
+cipher_log = logger.getLogger(__name__)
 
 
-def format_request(response: Response) -> dict[str, Any]:
+def format_request(request: Response, **kwargs: Any) -> dict[Any, Any]:
     """Reformat request.
 
     :param response: _description_
     :type response: Response
     :return: _description_
     :rtype: dict[str,Any]
     """
-    api_raise_error(response=response)
-    json_response = {
-        "exec_time": response.elapsed.total_seconds(),
-        "headers": json.loads(orjson.dumps(response.headers.__dict__["_store"]).decode('utf-8')),  # pylint: disable=no-member
-        "exec_time_end": datetime.datetime.utcnow().isoformat()
+    start_time: float = convert_to_epoch(kwargs['start_time'])
+    headers: Any = json.loads(orjson.dumps(request.headers.__dict__[
+                              "_store"]).decode(ENCODE)),  # pylint: disable=no-member
+    json_response: dict[str, Any] = {
+        "headers": headers,
+        "response_statistics": {
+            "iterations": kwargs.get("iterations", 1),
+            "status_code": request.status_code,
+            "exec_time_total": request.elapsed.total_seconds(),
+            "exec_time_elapsed": request.elapsed.total_seconds(),
+            "exec_time_end": datetime.datetime.utcnow().timestamp(),
+            "exec_time_start": start_time,
+            "x_proccessing_time": float(request.headers.get("X-Processing-Time")) if request.headers.get("X-Processing-Time") else None,
+        },
+        "request_parameters": {
+            "hostname": urllib.parse.urlparse(request.url).hostname,
+            "url": request.url,
+            "method": kwargs.get("method"),
+            "timeout": kwargs.get("timeout"),
+            "json": orjson.dumps(kwargs.get("json", {})).decode(ENCODE),  # pylint: disable=no-member
+            "verify": bool(kwargs.get("verify")),
+            "params": orjson.dumps(kwargs.get("params", {})).decode(ENCODE)  # pylint: disable=no-member
+        }
     }
+    if len(kwargs.get("exec_time_elapsed_list", [])) > 1:
+        json_response["response_statistics"]["exec_time_stdev"] = statistics.stdev(
+            kwargs.get("exec_time_elapsed_list"))  # type: ignore
     return json_response
 
 
-def standard_request(**kwargs: Any) -> dict[str, Any]:
+def standard_request(request: Response, **kwargs: Any) -> dict[str, Any]:
     """Call standard Request.
 
     :return: Adjusted Request Response
     :rtype: dict[str,Any]
     """
-    # Pop out saved_dir value to ensure doesn't get passed
-    kwargs.pop("saved_dir", "")
-    resp: Response = requests.request(**kwargs)  # pylint: disable=missing-timeout
-    response: dict[str, Any] = {**resp.json(), **format_request(resp)}
-    return response
+    req: dict[str, Any] = {**request.json(), **format_request(request, **kwargs)}
+    return req
 
 
-def download_request(**kwargs: Any) -> dict[str, Any]:
+def delete_request(request: Response, **kwargs: Any) -> dict[str, Any]:
+    """Deleteed request response.
+
+    :param request: _description_
+    :type request: Response
+    :return: _description_
+    :rtype: dict[str,Any]
+    """
+    ident: str = urllib.parse.urlparse(request.url).path.split('/')[-1]
+    value_type: str = re.sub(REGEX_NUM, "", urllib.parse.urlparse(request.url).path.split('/')[-2])
+    delete_response: dict[str, Any] = {
+        "id": ident,
+        "message": f"Deleted {value_type} with ID {ident}"
+    }
+    req: dict[str, Any] = {**delete_response, **format_request(request, **kwargs)}
+    return req
+
+
+def download_request(request: Response, **kwargs: Any) -> dict[str, Any]:
     """Use to Download Tar files. Only supports tar.gz can update.
 
     :return: Adjusted Request Ressponse
     :rtype: dict[str,Any]
     """
     chunk_size: int = kwargs.pop("chunk_size", 128)
     save_path: str = kwargs.pop("save_dir", os.path.expanduser('~'))
     if not verify_path_exists(path_dir=save_path):
         raise FileExistsError(f"{save_path} does not exist")
-    req: Response = requests.request(stream=True, **kwargs)  # pylint: disable=missing-timeout
-    parsed_url: urllib.parse.ParseResult = urllib.parse.urlparse(kwargs["url"])  # type: ignore
+    parsed_url: urllib.parse.ParseResult = urllib.parse.urlparse(request.url)  # type: ignore
     save_filename: Path = Path.joinpath(
         Path(save_path) /
         f"{datetime.datetime.now().strftime('%Y%m%dT%H%M%S')}_ciphertrust_log_{parsed_url.hostname}.tar.gz")  # pylint: disable=line-too-long,unknown-option-value
     with open(save_filename, 'wb') as fild:
-        for chunk in req.iter_content(chunk_size=chunk_size):
+        for chunk in request.iter_content(chunk_size=chunk_size):
             fild.write(chunk)
-    response: dict[str, str] = {
-        "message": "downloaded request completed",
+    response: dict[str, Any] = {
+        "message": "downloaded system logs completed",
         "location": str(save_filename)
     }
-    response = {**response, **format_request(req)}
+    response = {**response, **format_request(request, **kwargs)}
     return response
 
 
 @refresh_token
-def ctm_request(auth: Auth, **kwargs: Any) -> Dict[str, Any]:  # pylint: disable=too-many-locals
+def ctm_request(auth: Auth, **kwargs: Any) -> Response:  # pylint: disable=too-many-locals
     """_summary_
 
     Args:
         token (Auth): Auth class that is used to refresh bearer token upon expiration.
         url_type (str): specify the api call
         method (str): specifies the type of HTTPS method used
         params (dict, optional): specifies parameters passed to request
         data (str, optional): specifies the data being sent
         verify (str|bool, optional): sets request to verify with a custom
          cert bypass verification or verify with standard library. Defaults to True
         timeout (int, optional): sets API call timeout. Defaults to 60
-        delete_object (str, required|optional): Required if method is DELETE
-        put_object (str, required|optional): Required if method is PUT
         limit (int, Optional): The maximum number of results
         offset (int, Optional): The offset of the result entry
         get_object (str, Optional): Used if method is "GET", but additional path parameters required
     Returns:
         _type_: _description_
     """
+    kwargs.get("headers", {}).update({"Authorization": f"Bearer {auth.token}"})
+    start_time: float = datetime.datetime.utcnow().timestamp()
     try:
-        method: str = kwargs.pop('method')  # type: ignore
-        url: str = kwargs.pop('url')  # type: ignore
-        timeout: int = kwargs.pop('timeout', 60)  # type: ignore
-        verify: Any = kwargs.pop('verify', True)
-        params: Dict[str, Any] = kwargs.pop('params', {})
-        data: Any = kwargs.pop('data', None)  # type: ignore
-        stream: bool = kwargs.pop("stream", False)
-        headers: Dict[str, Any] = kwargs.pop("headers", DEFAULT_HEADERS)
-    except KeyError as err:
-        error: str = reformat_exception(err)
-        raise CipherMissingParam(error)  # pylint: disable=raise-missing-from
-    if data:
-        data: str = orjson.dumps(data).decode(ENCODE)  # pylint: disable=no-member
-    # Add auth to header
-    headers["Authorization"] = f"Bearer {auth.token}"
-    request_type = {
-        "download": download_request,
-        "standard": standard_request
-    }
-    start_time: str = datetime.datetime.utcnow().isoformat()
-    response: dict[str, Any] = request_type["standard" if not stream else "download"](
-        method=method,
-        url=url,
-        headers=headers,
-        data=data,
-        params=params,
-        verify=verify,
-        timeout=timeout,
-        **kwargs)
-    # Adds start time to response
-    response["exec_time_start"] = start_time
+        response: Response = requests.request(**kwargs)  # pylint: disable=missing-timeout
+    except ReadTimeout as err:
+        error = reformat_exception(err)
+        end_time: float = datetime.datetime.utcnow().timestamp()
+        response: Response = create_error_response(error=error,
+                                                   status_code=598,
+                                                   start_time=start_time,
+                                                   end_time=end_time,
+                                                   **kwargs)
     return response
 
 
 @refresh_token
 async def ctm_request_async(auth: Auth, **kwargs: Any) -> Dict[str, Any]:  # pylint: disable=too-many-locals
     """_summary_
 
@@ -169,17 +188,17 @@
     # Add auth to header
     # auth = refresh_token(auth=auth)
     headers["Authorization"] = f"Bearer {auth.token}"
     response: httpx.Response = await client.get(url=url,
                                                 params=params,
                                                 headers=headers)
     json_response = {
-        "exec_time": response.elapsed.total_seconds(),
-        "headers": response.headers,
-        "exec_time_end": time.time()
+        "exec_time_total": response.elapsed.total_seconds(),
+        "headers": json.loads(orjson.dumps(response.headers.__dict__["_store"]).decode(ENCODE)),  # pylint: disable=no-member
+        "exec_time_end": return_time()
     }
     return {**json_response, **response.json()}
 
 
 # TODO: Cannot do as we are talking about hundreds of calls due to the millions of certs stored.
 @refresh_token
 async def ctm_request_list_all(auth: Auth, **kwargs: Any) -> Dict[str, Any]:
@@ -189,20 +208,16 @@
         auth (Auth): _description_
 
     Returns:
         Dict[str,Any]: _description_
     """
     # inital response
     kwargs["params"] = {"limit": 1}
-    # refresh for 5 min timer
-    # auth.gen_refresh_token()
-    # print(f"token_expires={auth.expiration}")
-    start_time: float = time.time()
+    start_time: str = return_time()
     resp: dict[str, Any] = ctm_request(auth=auth, **kwargs)
-    # print(f"{resp=}")
     limit: int = 1000
     total: int = resp["total"]
     # set the total amount of iterations required to get full response
     # works when limit is already reached
     # TODO: This will send full iterations, but too many calls.
     # Reduce the amount of calls to prevent excessive calls.
     iterations: int = int(total/limit) if (total % limit == 0) else (total//limit + 1)
@@ -217,20 +232,19 @@
         send_iterations = 10 if iterations <= 10 else iterations
         tmp_listed_resp = await split_up_req(auth=auth,
                                              iterations=send_iterations,  # type: ignore
                                              limit=limit,  # type: ignore
                                              **kwargs)
         full_listed_resp: Any = full_listed_resp + tmp_listed_resp
         iterations -= 10
-        print(f"One loop iteration completed new_iterations={iterations}")
+        # print(f"One loop iteration completed new_iterations={iterations}")
     response = {**response, **build_responsde(full_listed_resp=full_listed_resp)}  # type: ignore
-    response["exec_time"] = response["exec_time_end"] - start_time
-    response["exec_time_end"] = datetime.datetime.utcfromtimestamp(
-        response["exec_time_end"]).isoformat()
-    response["exec_time_start"] = datetime.datetime.utcfromtimestamp(start_time).isoformat()
+    response["exec_time_total"] = (parser.isoparse(
+        response["exec_time_end"]) - parser.isoparse(start_time)).total_seconds()
+    response["exec_time_start"] = start_time
     return response
 
 
 @refresh_token
 async def split_up_req(auth: Auth,
                        iterations: int,
                        limit: int,
@@ -254,19 +268,18 @@
         for number in range(iterations):
             # Set the parameters and increase per run
             kwargs["params"] = {
                 "limit": limit,
                 "skip": (number*limit+1) if (number != 0) else 0
             }
             kwargs["client"] = client
-            print(f"{number=}|{kwargs=}")
+            # print(f"{number=}|{kwargs=}")
             tasks.append(asyncio.ensure_future(ctm_request_async(auth=auth, **kwargs)))
         full_listed_resp: List[Dict[str, Any]] = await asyncio.gather(*tasks)  # type: ignore
     return full_listed_resp  # type: ignore
-    # print(f"{full_listed_resp=}")
 
 
 def build_responsde(full_listed_resp: list[dict[str, Any]]) -> dict[str, Any]:
     """Build Returned Reponse with statistics.
 
     :param full_listed_resp: _description_
     :type full_listed_resp: list[dict[str, Any]]
@@ -276,16 +289,16 @@
     response: Dict[str, Any] = {
         "exec_time_end": 0.0,
         "exec_time_min": 0.0,
         "exec_time_max": 0.0,
         "exec_time_stdev": 0.0,
         "resources": []
     }
-    end_time: float = time.time()
-    elapsed_times: list[float] = [value["exec_time"] for value in full_listed_resp]
+    end_time: float = datetime.datetime.utcnow().timestamp()
+    elapsed_times: list[float] = [value["exec_time_total"] for value in full_listed_resp]
     response["elapsed_times"] = elapsed_times
     response["exec_time_end"] = end_time
     response["exec_time_min"] = min(elapsed_times)
     response["exec_time_max"] = max(elapsed_times)
     response["exec_time_stdev"] = statistics.stdev(elapsed_times)
     response["resources"] = reduce(concat_resources, full_listed_resp)["resources"]  # type: ignore
     return response
@@ -298,22 +311,58 @@
     :type auth: Auth
     :return: _description_
     :rtype: dict[str, Any]
     """
     return asyncio.run(ctm_request_list_all(auth=auth, **kwargs))
 
 
-def api_raise_error(response: Response) -> None:
+def api_raise_error(response: Response,
+                    method_type: str = "standard",
+                    **kwargs: Any) -> dict[str, Any]:
     """Raises error if response not what was expected
 
     Args:
         response (Response): _description_
 
     Raises:
         CipherPermission: _description_
         CipherAPIError: _description_
     """
+    formats: dict[str, Any] = {
+        "standard": standard_request,
+        "download": download_request,
+        "delete": delete_request
+    }
     try:
         response.raise_for_status()
-    except HTTPError as err:
+        return_response = formats[method_type](response, **kwargs)
+        # print(return_response)
+        cipher_log.info(
+            splunk_format(
+                source="ciphertrust-sdk", message="CipherTrust API Request", **
+                {**return_response["response_statistics"],
+                 **return_response["request_parameters"]}))
+    except (HTTPError) as err:
         error: str = reformat_exception(err)
-        raise CipherAPIError(f"{error=}|response={response.text}")
+        error_message = {
+            "error": error,
+            "error_type": "CipherAPIError",
+            "error_response": f"{response.text if response.text else response.reason}"
+        }
+        # Reformat response due to how codes are not returned properly
+        start_time: str = kwargs.pop('start_time')
+        response = create_error_response(error=error,
+                                         status_code=response.status_code,
+                                         start_time=convert_to_epoch(date=start_time),
+                                         end_time=datetime.datetime.utcnow().timestamp(),
+                                         **kwargs)
+        return_response = {
+            **error_message, **
+            standard_request(request=response, start_time=start_time, **kwargs)}
+        cipher_log.error(
+            splunk_format(
+                source="ciphertrust-sdk", **
+                {**return_response["response_statistics"],
+                 **return_response["request_parameters"],
+                 **error_message}))  # type: ignore
+    cipher_log.debug(splunk_format(**return_response))
+    return return_response
```

### Comparing `ciphertrust-sdk-1.0.6/src/ciphertrust/utils.py` & `ciphertrust-sdk-1.0.8/src/ciphertrust/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 """Utilities"""
 
+import datetime
 from typing import Dict, Any
 from pathlib import Path
+import time
+import urllib.parse
+import re
 
 import validators
+from requests.models import Response
+import orjson
 
 from ciphertrust.exceptions import CipherValueError
+from ciphertrust.static import ENCODE
 
 
 def concat_resources(dict1, dict2) -> list[dict[str, Any]]:  # type: ignore
     """Use reduce to generate a list of resources
 
     :param dict1: _description_
     :type dict1: _type_
     :param dict2: _description_
     :type dict2: _type_
-    :return: _description_
+    :return: Concatenated Resources Results
     :rtype: list[dict[str,Any]]
     """
     for key in dict2:  # type: ignore
         if key in dict1 and key == "resources":
             dict1[key] += dict2[key]
     return dict1  # type: ignore
 
@@ -57,17 +64,17 @@
     response: Dict[str, Any] = {}
     if kwargs.get("refresh_token_lifetime"):
         response["refresh_token_lifetime"] = kwargs.get("refresh_token_lifetime")
     return response
 
 
 def set_refresh_token_revoke_unused_in(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
-    """Sets refresh_token_revoke_unused_in if exists
+    """Sets refresh_token_revoke_unused_in if exists.
 
-    :return: _description_
+    :return: returns refresh token revoke
     :rtype: Dict[str,Any]
     """
     response: Dict[str, Any] = {}
     if kwargs.get("refresh_token_revoke_unused_in"):
         response["refresh_token_revoke_unused_in"] = kwargs.get("refresh_token_revoke_unused_in")
     return response
 
@@ -86,15 +93,15 @@
 def set_user_cert(**kwargs: Dict[str, Any]) -> Dict[str, Any]:
     """Sets User Certificate when specified in grant type
 
     :raises CipherValueError: _description_
     :return: _description_
     :rtype: Dict[str,Any]
     """
-    response: Dict[str,Any] = {}
+    response: Dict[str, Any] = {}
     try:
         # TODO: Confirm tuple value for (cert,key)
         response["cert"] = kwargs["cert"]
     except KeyError:
         raise CipherValueError("Required missing Cert for User Cert Auth")
     return response
 
@@ -222,11 +229,98 @@
     :type path_dir: str
     :return: _description_
     :rtype: bool
     """
     return Path(path_dir).exists()
 
 
+def verify_file_exists(filename: str) -> None:
+    """Verifies that a file being passed actually exists.
+
+    :param filename: Full Path Filename
+    :type path_dir: str
+    :raise: CipherValueError
+    """
+    if not Path(filename).is_file():
+        raise CipherValueError(f"Filen does not exist: {filename}")
+
+
+def return_time() -> str:
+    """Gets the current time and returns it in isoformt UTC.
+
+    :return: _description_
+    :rtype: str
+    """
+    return f"{datetime.datetime.utcnow().isoformat()}Z"
+
+
+def convert_to_epoch(date: str) -> float:
+    """Convert the returned time in ISO format to epoch.
+
+    :param date: _description_
+    :type date: str
+    :return: _description_
+    :rtype: float
+    """
+    date = re.sub(r"Z", "", date, re.IGNORECASE)
+    return datetime.datetime.fromisoformat(date).timestamp()
+
+
+def create_error_response(error: str,
+                          status_code: int,
+                          start_time: float,
+                          end_time: float,
+                          **kwargs: Any) -> Response:
+    """Creates an error response when no response comes back from request instead of raising an error.
+
+    :param error: _description_
+    :type error: str
+    :param status_code: _description_
+    :type status_code: int
+    :param start_time: _description_
+    :type start_time: float
+    :param end_time: _description_
+    :type end_time: float
+    :return: _description_
+    :rtype: Response
+    """
+    response = Response()
+    response.encoding = ENCODE
+    content: dict[str, Any] = {
+        "error": error,
+        "total": 0,
+        "request_parameters": {
+            "hostname": urllib.parse.urlparse(kwargs["url"]).hostname,
+            "method": kwargs.get("method"),
+            "timeout": kwargs.get("timeout"),
+            "json": orjson.dumps(kwargs.get("json", {})).decode(ENCODE),  # pylint: disable=no-member
+            "data": orjson.dumps(kwargs.get("data", {})).decode(ENCODE),  # pylint: disable=no-member
+            "verify": bool(kwargs.get("verify")),
+            "params": orjson.dumps(kwargs.get("params", {})).decode(ENCODE)  # pylint: disable=no-member
+        }
+    }
+    response.status_code = status_code
+    response.url = f"https://{urllib.parse.urlparse(kwargs['url']).hostname}/"
+    response.elapsed = (datetime.datetime.fromtimestamp(
+        end_time) - datetime.datetime.fromtimestamp(start_time))
+    response.headers.update({
+        "Date": time.strftime("%a, %d %b %Y %H:%M:%S GMT", time.gmtime(start_time)),
+        "Content-Type": "application/json; charset=UTF-8",
+        "Access-Control-Allow-Headers": "DNT,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type,Range",
+        "X-Processing-Time": f"{str(response.elapsed.total_seconds())}",
+        "Transfer-Encoding": "chunked",
+        "Connection": "keep-alive",
+        "Expires": time.strftime("%a, %d %b %Y %H:%M:%S GMT", time.gmtime(start_time+kwargs["timeout"])),
+        "Access-Control-Expose-Headers": "Content-Length,Content-Range",
+        "Access-Control-Allow-Methods": "GET, POST, OPTIONS",
+        "Cache-Control": "no-cache",
+        "X-Krakend": "Version undefined",
+        "X-Krakend-Completed": "false",
+        "Link": kwargs["url"]})
+    response._content = orjson.dumps(content)  # pylint: disable=no-member,protected-access
+    return response
+
+
 if __name__ == "__main__":
     valididate_list: list[str] = ["invalid", "valid-domain.example.com", "invalid_domain*.com"]
     for _ in valididate_list:
         is_valid = validate_domain(_)
```

