# Comparing `tmp/memfault_cli-1.0.0.tar.gz` & `tmp/memfault_cli-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memfault_cli-1.0.0.tar", max compression
+gzip compressed data, was "memfault_cli-1.0.1.tar", max compression
```

## Comparing `memfault_cli-1.0.0.tar` & `memfault_cli-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2877 2023-06-29 17:19:54.211920 memfault_cli-1.0.0/README.md
--rw-r--r--   0        0        0       79 2022-12-06 20:53:34.385268 memfault_cli-1.0.0/memfault_cli/__init__.py
--rw-r--r--   0        0        0      529 2023-04-27 16:08:38.128691 memfault_cli-1.0.0/memfault_cli/_version.py
--rw-r--r--   0        0        0     2579 2023-04-28 20:34:41.371280 memfault_cli-1.0.0/memfault_cli/authenticator.py
--rw-r--r--   0        0        0     3889 2023-04-27 16:08:38.128691 memfault_cli-1.0.0/memfault_cli/chunk.py
--rw-r--r--   0        0        0    27792 2023-06-29 12:58:48.735971 memfault_cli-1.0.0/memfault_cli/cli.py
--rw-r--r--   0        0        0     9759 2023-05-17 18:14:40.715182 memfault_cli-1.0.0/memfault_cli/console.py
--rw-r--r--   0        0        0    13111 2023-06-14 15:14:13.549689 memfault_cli-1.0.0/memfault_cli/context.py
--rw-r--r--   0        0        0     4762 2023-06-29 12:58:48.735971 memfault_cli-1.0.0/memfault_cli/deploy.py
--rw-r--r--   0        0        0     4115 2023-04-27 16:08:38.132691 memfault_cli-1.0.0/memfault_cli/elf.py
--rw-r--r--   0        0        0      633 2022-12-06 20:53:34.385268 memfault_cli-1.0.0/memfault_cli/functools_ext.py
--rw-r--r--   0        0        0    25379 2023-06-29 17:19:54.211920 memfault_cli-1.0.0/memfault_cli/upload.py
--rw-r--r--   0        0        0     7780 2023-04-28 20:34:41.371280 memfault_cli-1.0.0/memfault_cli/yocto.py
--rw-r--r--   0        0        0     3528 2023-06-29 17:19:54.211920 memfault_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 memfault_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3001 2023-07-06 15:16:06.787752 memfault_cli-1.0.1/README.md
+-rw-r--r--   0        0        0       79 2023-05-30 21:30:22.282085 memfault_cli-1.0.1/memfault_cli/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-30 21:30:22.282144 memfault_cli-1.0.1/memfault_cli/_version.py
+-rw-r--r--   0        0        0     2579 2023-05-30 21:30:22.282205 memfault_cli-1.0.1/memfault_cli/authenticator.py
+-rw-r--r--   0        0        0     3895 2023-07-05 14:30:20.686261 memfault_cli-1.0.1/memfault_cli/chunk.py
+-rw-r--r--   0        0        0    27792 2023-06-14 14:38:09.606809 memfault_cli-1.0.1/memfault_cli/cli.py
+-rw-r--r--   0        0        0     9759 2023-05-30 21:30:22.282483 memfault_cli-1.0.1/memfault_cli/console.py
+-rw-r--r--   0        0        0    13111 2023-06-22 19:07:02.890559 memfault_cli-1.0.1/memfault_cli/context.py
+-rw-r--r--   0        0        0     4765 2023-07-05 14:30:20.686386 memfault_cli-1.0.1/memfault_cli/deploy.py
+-rw-r--r--   0        0        0     4115 2023-05-30 21:30:22.282688 memfault_cli-1.0.1/memfault_cli/elf.py
+-rw-r--r--   0        0        0      633 2023-05-30 21:30:22.282740 memfault_cli-1.0.1/memfault_cli/functools_ext.py
+-rw-r--r--   0        0        0    26113 2023-07-06 15:16:06.788088 memfault_cli-1.0.1/memfault_cli/upload.py
+-rw-r--r--   0        0        0     7775 2023-07-05 13:14:43.930272 memfault_cli-1.0.1/memfault_cli/yocto.py
+-rw-r--r--   0        0        0     3528 2023-07-06 15:16:06.788346 memfault_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 memfault_cli-1.0.1/PKG-INFO
```

### Comparing `memfault_cli-1.0.0/README.md` & `memfault_cli-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 The purpose of the tool is to make integration with Memfault from other systems,
 like continuous integration servers, as easy as possible.
 
 Install the tool and run `memfault --help` for more info!
 
 ## Changes
 
+### 1.0.1
+
+- Fix `upload-custom-data-recording` to print a more helpful error message when
+  exceeding device rate limits.
+
 ### 1.0.0
 
 _Note: this release is marked as `1.0.0` but does not contain any breaking
 changes! The version number was bumped to reflect the maturity of the tool._
 
 - Fix `upload-mcu-symbols` to skip uploading if the symbol file has already been
   uploaded, and return a zero exit code in this case
```

### Comparing `memfault_cli-1.0.0/memfault_cli/_version.py` & `memfault_cli-1.0.1/memfault_cli/_version.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.0/memfault_cli/authenticator.py` & `memfault_cli-1.0.1/memfault_cli/authenticator.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.0/memfault_cli/chunk.py` & `memfault_cli-1.0.1/memfault_cli/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return f"{self.ctx.chunks_url}/api/v0/chunks/{self.ctx.device_serial}"
 
     def post(self, chunk: bytes):
         request_args = self.authenticator.requests_auth_params()
         request_args["headers"]["Content-Type"] = "application/octet-stream"
         response = requests.post(self.url, data=chunk, **request_args)
         if response.status_code >= 400:
-            raise Exception(
+            raise RuntimeError(
                 f"Request failed with HTTP status {response.status_code}\nResponse"
                 f" body:\n{response.content.decode()}"
             )
 
     def do_batch_post(self, files: List):
         """Issue a post with a batch of files (HTTP Multipart)"""
         request_args = self.authenticator.requests_auth_params()
@@ -47,15 +47,15 @@
         request.prepare(method="POST", url=self.url, files=files, headers=headers, **request_args)
         content_type: str = request.headers["content-type"]
         request.headers["content-type"] = content_type.replace("form-data", "mixed")
 
         session = requests.Session()
         response = session.send(request)
         if response.status_code >= 400:
-            raise Exception(
+            raise RuntimeError(
                 f"Request failed with HTTP status {response.status_code}\nResponse"
                 f" body:\n{response.content.decode()}"
             )
 
     def batch_post(self, chunks: List[bytes]):
         """
         Post a batch of chunks to the Memfault Chunk API. Will break the request
```

### Comparing `memfault_cli-1.0.0/memfault_cli/cli.py` & `memfault_cli-1.0.1/memfault_cli/cli.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.0/memfault_cli/console.py` & `memfault_cli-1.0.1/memfault_cli/console.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.0/memfault_cli/context.py` & `memfault_cli-1.0.1/memfault_cli/context.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.0/memfault_cli/deploy.py` & `memfault_cli-1.0.1/memfault_cli/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         if deployment_type == "staged_rollout":
             json_d["rollout_percent"] = rollout_percent
 
         response = self.session.post(
             self.deployment_url, json=json_d, **self.authenticator.requests_auth_params()
         )
         if response.status_code >= 400:
-            raise Exception(
+            raise RuntimeError(
                 f"Request failed with HTTP status {response.status_code}\nResponse"
                 f" body:\n{response.content.decode()}"
             )
         log.info("Release %s successfully deployed to Cohort %s", release_version, cohort)
 
     def deactivate(self, *, release_version: Union[str, Tuple[str, str]], cohort: str) -> None:
         """
```

### Comparing `memfault_cli-1.0.0/memfault_cli/elf.py` & `memfault_cli-1.0.1/memfault_cli/elf.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.0/memfault_cli/functools_ext.py` & `memfault_cli-1.0.1/memfault_cli/functools_ext.py`

 * *Files identical despite different names*

### Comparing `memfault_cli-1.0.0/memfault_cli/upload.py` & `memfault_cli-1.0.1/memfault_cli/upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import logging
 import os
 import re
 import urllib.parse
 from abc import abstractmethod
 from concurrent.futures import ThreadPoolExecutor
 from glob import glob
-from typing import IO, Dict, Iterable, List, Optional, Tuple, Type, Union
+from typing import IO, Dict, Iterable, Optional, Sequence, Tuple, Type, Union
 from zipfile import is_zipfile
 
 import click
 import requests
 from elftools.elf.elffile import ELFFile
 from mflt_build_id import BuildIdInspectorAndPatcher
-from requests import Response, Session
+from requests import HTTPError, Response, Session
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
 from .authenticator import (
     Authenticator,
@@ -41,14 +41,18 @@
     pass
 
 
 class UploadIsTooLargeError(Exception):
     pass
 
 
+class TooManyRequestsError(Exception):
+    pass
+
+
 class MemfaultAPIErrorResponse:
     kind: str
     message: str
 
     def __init__(self, response: Response):
         self.message = response.json()["error"]["message"]
         self.kind = response.json()["error"]["type"]
@@ -69,26 +73,26 @@
             break
         h.update(chunk)
     return h.hexdigest()
 
 
 def check_response(response: Response):
     if response.status_code >= 400:
-        raise Exception(
+        raise HTTPError(
             f"Request failed with HTTP status {response.status_code}\n"
             f"Response body:\n{response.content.decode() if response.content else '(empty)'}"
         )
 
 
 def url_quote(value: str) -> str:
     return urllib.parse.quote(value, safe="", encoding="utf-8")
 
 
 class Uploader(metaclass=abc.ABCMeta):
-    authenticator_types: List[Type[Authenticator]]
+    authenticator_types: Sequence[Type[Authenticator]]
 
     def __init__(
         self,
         *,
         ctx: MemfaultCliClickContext,
         file_path: Union[str, os.PathLike],
         authenticator: Authenticator,
@@ -102,14 +106,15 @@
     @staticmethod
     def _create_requests_session() -> Session:
         retry_strategy = Retry(
             total=5,
             backoff_factor=2,  # Sleep for 2s, 4s, 8s, 16s, 32s, Stop
             status_forcelist=[429, 500, 502, 503, 504],
             allowed_methods=["HEAD", "GET", "POST", "PUT"],
+            raise_on_status=False,
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
         session = requests.Session()
         session.mount("https://", adapter)
         session.mount("http://", adapter)
         return session
 
@@ -186,25 +191,29 @@
         extra_request_data = self.post_token_extra_request_data()
         if extra_request_data:
             json_d.update(extra_request_data)
 
         response = self.session.post(
             self.entity_url(), json=json_d, **self.authenticator.requests_auth_params()
         )
+
         # This file had already uploaded (maybe concurrently). Gracefully ignore the error then.
         if response.status_code == 409:
             log.info("%s: was already uploaded.", self.file_path)
             raise UploadedAlreadyExistsError("%s: was already uploaded." % self.file_path)
 
         if response.status_code == 400:
             error = MemfaultAPIErrorResponse(response)
             if UPLOAD_IS_TOO_BIG_RESPONSE in error.message:
                 # Need to grab the max file size from the error response, so we have to print the real message
                 raise UploadIsTooLargeError(error.message + f" ({self.file_path!r})")
 
+        if response.status_code == 429:
+            raise TooManyRequestsError("Too many requests")
+
         check_response(response)
 
     @property
     def qcomm_project(self):
         response = self.session.get(
             self._projects_base_url(base_url_override=self.ctx.api_url),
             **self.authenticator.requests_auth_params(),
@@ -222,14 +231,26 @@
             self._post_token(token)
             log.info("%s: uploaded!", self.file_path)
         except UploadIsTooLargeError as e:
             log.warning(str(e))
             return False
         except UploadedAlreadyExistsError:
             pass
+        except TooManyRequestsError as e:
+            log.warning(str(e))
+            log.info(
+                "Rate limit exceeded, you can enable server side developer mode to temporarily remove this limit "
+                "for testing or development by accessing this URL: "
+                "%s/organizations/%s/projects/%s/devices/%s?tab=developer-mode",
+                self.app_url,
+                self.ctx.org,
+                self.ctx.project,
+                self.ctx.device_serial,
+            )
+            return False
 
         if self.ui_url():
             click.echo(f"You can view in the UI here:\n   {self.ui_url()}")
         return True
 
     @cached_property
     def file_md5(self):
@@ -238,19 +259,19 @@
 
     @property
     def file_basename(self):
         return os.path.basename(self.file_path)
 
 
 class BugreportUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         ProjectKeyAuthenticator,
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         if not is_zipfile(self.file_path):
             log.error("%s is not a valid zip file!", self.file_path)
             return False
         return True
 
@@ -258,19 +279,19 @@
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/bugreport"
         else:
             return f"{self._projects_base_url()}/bugreports"
 
 
 class CoredumpUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         ProjectKeyAuthenticator,
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         with open(self.file_path, "rb") as f:
             hdr = f.read(4).decode("ascii", errors="ignore")
             if hdr != "CORE":
                 log.error("%s is not a Memfault Coredump", self.file_path)
                 return False
@@ -288,19 +309,19 @@
             return {
                 "device_serial": self.ctx.core_info.device_serial,
             }
         return None
 
 
 class XedUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         ProjectKeyAuthenticator,
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         return True
 
     def entity_url(self) -> str:
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/qc/x"
@@ -315,19 +336,19 @@
             "trace_attributes": [
                 {"string_key": a.string_key, "value": a.value} for a in self.ctx.attributes
             ],
         }
 
 
 class MarUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         ProjectKeyAuthenticator,
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         if not is_zipfile(self.file_path):
             log.error("%s is not a valid zip file!", self.file_path)
             return False
         return True
 
@@ -344,19 +365,19 @@
             "hardware_version": info.hardware_version,
             "software_type": info.software_type,
             "software_version": info.software_version,
         }
 
 
 class CustomDataRecordingUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         ProjectKeyAuthenticator,
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         return True
 
     def entity_url(self) -> str:
         if self.authenticator.project_key_auth():
             return f"{self._api_base_url()}/upload/custom-data-recording"
@@ -377,18 +398,18 @@
                 "software_type": device_traits.software_type,
                 "software_version": device_traits.software_version,
             },
         }
 
 
 class ElfSymbolUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     gnu_build_id: Optional[str] = ""
 
     def can_upload_file(self) -> bool:
         if os.path.islink(self.file_path) and not os.path.exists(self.file_path):
             return False
 
@@ -430,18 +451,18 @@
         return True
 
     def entity_url(self) -> str:
         return f"{self._projects_base_url()}/symbols"
 
 
 class McuSdkElfSymbolUploader(ElfSymbolUploader, Uploader):
-    authenticator_types = [
+    authenticator_types = (
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         with open(self.file_path, "rb") as file:
             if file.read(4) != b"\x7FELF":
                 log.info("%s: Not an ELF file", self.file_path)
                 return False
             file.seek(0)
@@ -497,18 +518,18 @@
                 "software_type": info.software_type,
                 **({"revision": info.revision} if info.revision else {}),
             },
         }
 
 
 class ReleaseArtifactUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         # There are no restrictions for the type of binary a customer uses for
         # a release
         return True
 
     def _is_already_uploaded(self) -> bool:
@@ -612,25 +633,25 @@
 
     def entity_url(self) -> str:
         raise NotImplementedError
 
 
 class ElfSymbolDirectoryUploader(ParallelUploader):
     uploader_cls = ElfSymbolUploader
-    authenticator_types = [
+    authenticator_types = (
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
 
 class ProguardMappingUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def __init__(
         self,
         *,
         ctx: MemfaultCliClickContext,
         file_path: str,
         authenticator: Authenticator,
@@ -652,18 +673,18 @@
                 "version": f"{self.package_info.version_name}:{self.package_info.version_code}",
                 "software_type": self.package_info.name,
             },
         }
 
 
 class AndroidAppSymbolsUploader(Uploader):
-    authenticator_types = [
+    authenticator_types = (
         OrgTokenAuthenticator,
         BasicAuthenticator,
-    ]
+    )
 
     def can_upload_file(self) -> bool:
         if not os.path.isdir(self.file_path):
             log.error(
                 '%s is not a directory. Please specify the Android app\'s root "build" path instead!',
                 self.file_path,
             )
@@ -694,19 +715,19 @@
 
     def _find_mapping_txt(self) -> Optional[str]:
         if self.ctx.android_mapping_txt:
             return self.ctx.android_mapping_txt
         # In older version, the default folder was called "proguard", later it got renamed to "mapping":
         subdirs = ("mapping", "proguard")
         paths_to_check = tuple(
-            map(
-                lambda subdir: os.path.join(
+            (
+                os.path.join(
                     self.file_path, "outputs", "mapping", self.ctx.build_variant, "mapping.txt"
-                ),
-                subdirs,
+                )
+                for subdir in subdirs
             )
         )
         for path in paths_to_check:
             if os.path.isfile(path):
                 return path
         log.info("No mapping.txt found in default locations, assuming ProGuard/R8 is disabled...")
         return None
```

### Comparing `memfault_cli-1.0.0/memfault_cli/yocto.py` & `memfault_cli-1.0.1/memfault_cli/yocto.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 
 class OeInitBuildEnvNotSourcedError(Exception):
     pass
 
 
 def get_from_bitbake_build_env(variables: List[str]) -> List[Optional[str]]:
-    grep_pattern = "|".join(map(lambda variable: f"^{variable}", variables))
+    grep_pattern = "|".join((f"^{variable}" for variable in variables))
 
     try:
         bitbake_environment_process = subprocess.Popen(
             ("bitbake", "--environment"), stdout=subprocess.PIPE
         )
         output = subprocess.check_output(
             ("grep", "-E", grep_pattern), stdin=bitbake_environment_process.stdout
```

### Comparing `memfault_cli-1.0.0/pyproject.toml` & `memfault_cli-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "memfault-cli"
-version = "1.0.0"
+version = "1.0.1"
 description = "Memfault CLI tool"
 homepage = "https://docs.memfault.com"
 documentation = "https://docs.memfault.com/docs/ci/install-memfault-cli"
 authors = ["Memfault Inc <hello@memfault.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `memfault_cli-1.0.0/PKG-INFO` & `memfault_cli-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memfault-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Memfault CLI tool
 Home-page: https://docs.memfault.com
 Author: Memfault Inc
 Author-email: hello@memfault.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -35,14 +35,19 @@
 The purpose of the tool is to make integration with Memfault from other systems,
 like continuous integration servers, as easy as possible.
 
 Install the tool and run `memfault --help` for more info!
 
 ## Changes
 
+### 1.0.1
+
+- Fix `upload-custom-data-recording` to print a more helpful error message when
+  exceeding device rate limits.
+
 ### 1.0.0
 
 _Note: this release is marked as `1.0.0` but does not contain any breaking
 changes! The version number was bumped to reflect the maturity of the tool._
 
 - Fix `upload-mcu-symbols` to skip uploading if the symbol file has already been
   uploaded, and return a zero exit code in this case
```

