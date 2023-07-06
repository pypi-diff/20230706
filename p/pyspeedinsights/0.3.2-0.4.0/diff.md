# Comparing `tmp/pyspeedinsights-0.3.2.tar.gz` & `tmp/pyspeedinsights-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspeedinsights-0.3.2.tar", last modified: Tue Jul  4 14:43:57 2023, max compression
+gzip compressed data, was "pyspeedinsights-0.4.0.tar", last modified: Thu Jul  6 03:19:33 2023, max compression
```

## Comparing `pyspeedinsights-0.3.2.tar` & `pyspeedinsights-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.118915 pyspeedinsights-0.3.2/
--rw-r--r--   0 will       (501) staff       (20)     1080 2022-05-27 03:33:19.000000 pyspeedinsights-0.3.2/LICENSE
--rw-r--r--   0 will       (501) staff       (20)    14017 2023-07-04 14:43:57.119461 pyspeedinsights-0.3.2/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)    12820 2023-02-26 01:59:32.000000 pyspeedinsights-0.3.2/README.md
--rw-r--r--   0 will       (501) staff       (20)      651 2023-02-26 02:20:45.000000 pyspeedinsights-0.3.2/pyproject.toml
--rw-r--r--   0 will       (501) staff       (20)     1613 2023-07-04 14:43:57.121339 pyspeedinsights-0.3.2/setup.cfg
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.105097 pyspeedinsights-0.3.2/src/
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.108155 pyspeedinsights-0.3.2/src/pyspeedinsights/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 03:33:19.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/__init__.py
--rw-r--r--   0 will       (501) staff       (20)      142 2022-06-07 16:31:02.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/__main__.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.112614 pyspeedinsights-0.3.2/src/pyspeedinsights/api/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 04:37:52.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     1613 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/keys.py
--rw-r--r--   0 will       (501) staff       (20)     3990 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/request.py
--rw-r--r--   0 will       (501) staff       (20)     4871 2023-07-04 14:36:46.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/api/response.py
--rw-r--r--   0 will       (501) staff       (20)     3411 2023-02-26 04:24:39.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/app.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.114204 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     2778 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/choices.py
--rw-r--r--   0 will       (501) staff       (20)     4598 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/cli/commands.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.115661 pyspeedinsights-0.3.2/src/pyspeedinsights/core/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 20:34:15.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/core/__init__.py
--rw-r--r--   0 will       (501) staff       (20)     8497 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/core/excel.py
--rw-r--r--   0 will       (501) staff       (20)     4543 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/core/sitemap.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.118045 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/
--rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/__init__.py
--rw-r--r--   0 will       (501) staff       (20)      509 2022-11-04 03:53:30.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/generic.py
--rw-r--r--   0 will       (501) staff       (20)     1304 2023-07-03 22:00:41.000000 pyspeedinsights-0.3.2/src/pyspeedinsights/utils/urls.py
-drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-04 14:43:57.110589 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/
--rw-r--r--   0 will       (501) staff       (20)    14017 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/PKG-INFO
--rw-r--r--   0 will       (501) staff       (20)      855 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/SOURCES.txt
--rw-r--r--   0 will       (501) staff       (20)        1 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/dependency_links.txt
--rw-r--r--   0 will       (501) staff       (20)       49 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/entry_points.txt
--rw-r--r--   0 will       (501) staff       (20)      143 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/requires.txt
--rw-r--r--   0 will       (501) staff       (20)       16 2023-07-04 14:43:57.000000 pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/top_level.txt
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.918669 pyspeedinsights-0.4.0/
+-rw-r--r--   0 will       (501) staff       (20)     1080 2022-05-27 03:33:19.000000 pyspeedinsights-0.4.0/LICENSE
+-rw-r--r--   0 will       (501) staff       (20)    13978 2023-07-06 03:19:33.918898 pyspeedinsights-0.4.0/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)    12781 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/README.md
+-rw-r--r--   0 will       (501) staff       (20)      699 2023-07-04 16:04:18.000000 pyspeedinsights-0.4.0/pyproject.toml
+-rw-r--r--   0 will       (501) staff       (20)     1625 2023-07-06 03:19:33.919954 pyspeedinsights-0.4.0/setup.cfg
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.900952 pyspeedinsights-0.4.0/src/
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.904585 pyspeedinsights-0.4.0/src/pyspeedinsights/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 03:33:19.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)      142 2022-06-07 16:31:02.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/__main__.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.911060 pyspeedinsights-0.4.0/src/pyspeedinsights/api/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 04:37:52.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     2478 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/keys.py
+-rw-r--r--   0 will       (501) staff       (20)     5239 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/request.py
+-rw-r--r--   0 will       (501) staff       (20)     5946 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/api/response.py
+-rw-r--r--   0 will       (501) staff       (20)     6004 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/app.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.913115 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     2732 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/choices.py
+-rw-r--r--   0 will       (501) staff       (20)     4744 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/cli/commands.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.915038 pyspeedinsights-0.4.0/src/pyspeedinsights/core/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-05-27 20:34:15.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/core/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)     9243 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/core/excel.py
+-rw-r--r--   0 will       (501) staff       (20)     5471 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/core/sitemap.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.918090 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/
+-rw-r--r--   0 will       (501) staff       (20)        0 2022-06-06 20:47:32.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/__init__.py
+-rw-r--r--   0 will       (501) staff       (20)      174 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/exceptions.py
+-rw-r--r--   0 will       (501) staff       (20)      509 2022-11-04 03:53:30.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/generic.py
+-rw-r--r--   0 will       (501) staff       (20)     1685 2023-07-06 03:17:10.000000 pyspeedinsights-0.4.0/src/pyspeedinsights/utils/urls.py
+drwxr-xr-x   0 will       (501) staff       (20)        0 2023-07-06 03:19:33.907399 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/
+-rw-r--r--   0 will       (501) staff       (20)    13978 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/PKG-INFO
+-rw-r--r--   0 will       (501) staff       (20)      895 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/SOURCES.txt
+-rw-r--r--   0 will       (501) staff       (20)        1 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/dependency_links.txt
+-rw-r--r--   0 will       (501) staff       (20)       49 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/entry_points.txt
+-rw-r--r--   0 will       (501) staff       (20)      154 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/requires.txt
+-rw-r--r--   0 will       (501) staff       (20)       16 2023-07-06 03:19:33.000000 pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/top_level.txt
```

### Comparing `pyspeedinsights-0.3.2/LICENSE` & `pyspeedinsights-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspeedinsights-0.3.2/PKG-INFO` & `pyspeedinsights-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspeedinsights
-Version: 0.3.2
+Version: 0.4.0
 Summary: Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 Home-page: https://github.com/wjh18/pyspeedinsights
 Author: Will J. Holmes
 Author-email: will@wjholmes.com
 Project-URL: Documentation, https://github.com/wjh18/pyspeedinsights/blob/master/README.md
 Project-URL: Source, https://github.com/wjh18/pyspeedinsights
 Project-URL: Tracker, https://github.com/wjh18/pyspeedinsights/issues
@@ -235,15 +235,14 @@
 * `psi https://example.com -f excel` - no metrics
 * `psi https://example.com -f excel -m all` - all available metrics
 * `psi https://example.com -f excel -m speedIndex` - just speedIndex
 * `psi https://example.com -f excel -m speedIndex totalBlockingTime` - just speedIndex and totalBlockingTime
 
 Full list of available metrics:
 
-* `observedTotalCumulativeLayoutShift`
 * `observedCumulativeLayoutShift`
 * `observedLargestContentfulPaintAllFrames`
 * `maxPotentialFID`
 * `observedSpeedIndexTs`
 * `observedFirstContentfulPaintTs`
 * `observedTimeOrigin`
 * `observedFirstPaint`
```

### Comparing `pyspeedinsights-0.3.2/README.md` & `pyspeedinsights-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,14 @@
 * `psi https://example.com -f excel` - no metrics
 * `psi https://example.com -f excel -m all` - all available metrics
 * `psi https://example.com -f excel -m speedIndex` - just speedIndex
 * `psi https://example.com -f excel -m speedIndex totalBlockingTime` - just speedIndex and totalBlockingTime
 
 Full list of available metrics:
 
-* `observedTotalCumulativeLayoutShift`
 * `observedCumulativeLayoutShift`
 * `observedLargestContentfulPaintAllFrames`
 * `maxPotentialFID`
 * `observedSpeedIndexTs`
 * `observedFirstContentfulPaintTs`
 * `observedTimeOrigin`
 * `observedFirstPaint`
```

### Comparing `pyspeedinsights-0.3.2/pyproject.toml` & `pyspeedinsights-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 [tool.mypy]
 # warn_return_any = true
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
 module = [
     "xlsxwriter",
-    "xlsxwriter.format"
+    "xlsxwriter.format",
+    "defusedxml",
+    "defusedxml.ElementTree"
 ]
 ignore_missing_imports = true
 
 [tool.bandit]
 targets = ["src/pyspeedinsights"]
 exclude_dirs = [".venv", "tests"]
```

### Comparing `pyspeedinsights-0.3.2/setup.cfg` & `pyspeedinsights-0.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyspeedinsights
-version = 0.3.2
+version = 0.4.0
 author = Will J. Holmes
 author_email = will@wjholmes.com
 description = Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = google, google-apis, psi-api, page-speed-insights, page-speed-insights-api, pagespeedinsightsapi, python, cli
 url = https://github.com/wjh18/pyspeedinsights
@@ -29,14 +29,15 @@
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	requests
 	XlsxWriter
 	keyring
 	aiohttp[speedups]
+	defusedxml
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 dev = 
 	pytest
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/api/keys.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/api/keys.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,47 +3,68 @@
 Storing an API key in keyring: `keyring set system psikey`
 Verifying an API key is stored: `keyring get system psikey`
 Removing an API key from keyring: `keyring del system psikey`
 
 If no key is set in keyring, the user will be manually prompted for their key.
 """
 
+import logging
+
 import keyring
 from keyring.errors import KeyringError
 
+logger = logging.getLogger(__name__)
+
+
+class RetryLimitExceededError(KeyringError):
+    """Exception if the user has exceeded the retry limit for entering an API key."""
+
+
+class InputTerminatedError(KeyringError):
+    """Exception if the user manually terminates retry for entering an API key."""
+
 
 def get_api_key() -> str:
     """Gets the user's PSI API key from their keyring store.
 
     Allows manual entry of the key if nonexistent or keystore errors occur.
     Reprompts for keys read in as empty strings. Otherwise, key validation should be
     lenient with errors handled at request time (in case Google changes the key format).
 
     Returns:
         A str representing the PSI API key.
     Raises:
-        SystemExit: The user terminated the reprompt.
+        InputTerminatedError: The user terminated the reprompt.
+        RetryLimitExceededError: The reprompt limit was exceeded.
     """
+    logger.info("Attempting to retrieve API key from keystore.")
     try:
         # get_password() returns None for an empty key
         psi_api_key = keyring.get_password("system", "psikey")
-    except KeyringError:
-        print("There was an error retrieving your API key from the keystore.")
+    except KeyringError as err:
+        logger.error(
+            f"There was an error retrieving your API key from the keystore: {err}",
+            exc_info=True,
+        )
         psi_api_key = None
 
     if psi_api_key is None:
-        psi_api_key = input("No API key found. Enter it manually:\n")
+        logger.warning("No API key found. Defaulting to manual input.")
+        psi_api_key = input("No API key found. Enter your key manually:\n")
 
     retry_limit = 5
     while not psi_api_key:
+        logger.warning("Empty API key supplied. Reprompting user for key.")
         reprompt = input(
             "Empty API key supplied. Please re-enter your key or Q to quit:\n"
         )
+        # Below errors logged as CRITICAL in main() before exit
         if reprompt in ("Q", "q"):
-            raise SystemExit
+            raise InputTerminatedError("API key input cancelled.")
         elif retry_limit < 1:
-            raise SystemExit("Retry limit exceeded.")
+            raise RetryLimitExceededError("Retry limit for entering API key exceeded.")
         else:
             psi_api_key = reprompt
         retry_limit -= 1
 
+    logger.info("API key retrieval successful.")
     return psi_api_key
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/api/request.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/api/request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,83 +1,88 @@
 """Async request preparation and processing for PSI API calls."""
 
 import asyncio
+import logging
+import ssl
 from collections import Counter
-from typing import Any, Coroutine, Union
+from typing import Any, Coroutine, Optional, Union
 
 import aiohttp
 
 from ..utils.generic import remove_nonetype_dict_items
-from ..utils.urls import validate_url
-from .keys import get_api_key
+from ..utils.urls import InvalidURLError, validate_url
+from .keys import KeyringError, get_api_key
 
+logger = logging.getLogger(__name__)
 next_delay = 1  # Global for applying a 1s delay between requests
 
 
 async def get_response(
+    key: str,
     url: str,
-    category: str = None,
-    locale: str = None,
-    strategy: str = None,
-    utm_campaign: str = None,
-    utm_source: str = None,
-    captcha_token: str = None,
+    category: Optional[str] = None,
+    locale: Optional[str] = None,
+    strategy: Optional[str] = None,
+    utm_campaign: Optional[str] = None,
+    utm_source: Optional[str] = None,
+    captcha_token: Optional[str] = None,
 ) -> dict:
     """Makes async GET calls to the PSI API for the requested page's URL.
 
     Args of NoneType will not be added as query params. They'll use PSI API defaults.
 
     Returns:
         The awaited json response from the server as a str.
     Raises:
         aiohttp.ClientError: The retry limit was reached for failed requests.
     """
     base_url = "https://www.googleapis.com/pagespeedonline/v5/runPagespeed"
     url = validate_url(url)
     params = {
+        "key": key,
         "url": url,
         "category": category,
         "locale": locale,
         "strategy": strategy,
         "utm_campaign": utm_campaign,
         "utm_source": utm_source,
         "captcha_token": captcha_token,
     }
     # Use API defaults instead of passing None values as query params.
     params = remove_nonetype_dict_items(params)
-    params["key"] = get_api_key()
     req_url = params["url"]
 
     # Add a 1s delay between calls to avoid 500 errors from server.
     global next_delay
     next_delay += 1
+    logger.debug("Sleeping request to prevent server errors.")
     await asyncio.sleep(next_delay)
 
-    print(f"Sending request... ({req_url})")
+    logger.info(f"Sending request... ({req_url})")
     # Make async call with query params to PSI API and await response.
     async with aiohttp.ClientSession() as session:
         async with session.get(url=base_url, params=params) as resp:
             json_resp = None
             retry_attempts = 5
             while json_resp is None:
                 try:
                     resp.raise_for_status()
                     json_resp = await resp.json()
-                    print(f"Request successful! ({req_url})")
+                    logger.info(f"Request successful! ({req_url})")
                 except aiohttp.ClientError as err_c:
                     if retry_attempts < 1:
-                        print(err_c)
-                        print(f"Retry limit reached. Skipping ({req_url})")
+                        logger.error(err_c, exc_info=True)
+                        logger.warning(
+                            f"Retry limit for URL reached. Skipping ({req_url})"
+                        )
                         raise aiohttp.ClientError(err_c)
                     else:
                         retry_attempts -= 1
-                        print(
-                            "Request failed. Retrying... ",
-                            f"{retry_attempts} retries left ({req_url})",
-                        )
+                        logger.warning("Request failed. Retrying.")
+                        logger.info(f"{retry_attempts} retries left ({req_url})")
                         await asyncio.sleep(1)
     return json_resp
 
 
 def run_requests(
     request_urls: list[str], api_args_dict: dict[str, Union[str, None]]
 ) -> list[dict]:
@@ -87,30 +92,57 @@
     """
     tasks = get_tasks(request_urls, api_args_dict)
     return asyncio.run(gather_responses(tasks))
 
 
 async def gather_responses(tasks: list[Coroutine]) -> list[dict]:
     """Gathers tasks and awaits the return of the responses for processing."""
-    print(f"Preparing {len(tasks)} URL(s)...")
+    logger.info(f"Gathering {len(tasks)} URL(s) and scheduling tasks.")
     responses = await asyncio.gather(*tasks, return_exceptions=True)
 
+    # Generator expression for bubbling up critical exceptions (handled in main())
+    # Purposefully explicit here to avoid raising exceptions for aiohttp.ClientError,
+    # as we don't want a single client failure to invalidate the entire run.
+    # OSError and ssl errors are all subclassed by aiohttp exceptions.
+    critical_exception = next(
+        (
+            r
+            for r in responses
+            if isinstance(
+                r,
+                (
+                    KeyringError,
+                    InvalidURLError,
+                    OSError,
+                    ssl.SSLError,
+                    ssl.CertificateError,
+                ),
+            )
+        ),
+        None,
+    )
+
+    if critical_exception is not None:
+        raise critical_exception
+
     type_counts = Counter(type(r) for r in responses)
     c_success, c_fail = type_counts[dict], type_counts[aiohttp.ClientError]
-    print(
-        f"{c_success}/{len(tasks)} URL(s) processed successfully. ",
-        f"{c_fail} skipped due to errors.",
-    )
+    logger.info(f"{c_success}/{len(tasks)} URL(s) processed successfully. ")
+    logger.warning(f"{c_fail} skipped due to errors. Removing failed URL(s).")
+
     # Remove failures for response processing
     responses = [r for r in responses if type(r) == dict]
     return responses
 
 
 def get_tasks(
     request_urls: list[str], api_args_dict: dict[str, Any]
 ) -> list[Coroutine]:
     """Creates a list of tasks that call get_response() with request params."""
+    logger.info("Creating list of tasks based on parsed URL(s).")
+    key = get_api_key()
     tasks = []
     for url in request_urls:
         api_args_dict["url"] = url
+        api_args_dict["key"] = key
         tasks.append(get_response(**api_args_dict))
     return tasks
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/api/response.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/api/response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,76 @@
 """Response processing and parsing for PSI API results."""
 
 import copy
 import json
+import logging
 from datetime import datetime
 from typing import Optional, Union
 
 from ..cli.choices import COMMAND_CHOICES
+from ..utils.exceptions import JSONKeyError
 from ..utils.generic import sort_dict_alpha
 
+logger = logging.getLogger(__name__)
+
 
 def process_json(json_resp: dict, category: str, strategy: str) -> None:
     """Dumps raw json response to a file in the working directory.
 
     Called within main() in pyspeedinsights.app.
     If json format is selected this is where program execution ends.
     """
     date = _get_timestamp(json_resp)
     filename = f"psi-s-{strategy}-c-{category}-{date}.json"
 
     with open(filename, "w", encoding="utf-8") as f:
         json.dump(json_resp, f, ensure_ascii=False, indent=4)
-        print("JSON processed. Check your current directory.")
+        logger.info("JSON processed. Check your current working directory.")
 
 
 def process_excel(
     json_resp: dict, category: str, metrics: Optional[list[str]]
 ) -> dict[str, Union[dict, None]]:
     """Calls various parsing operations for Excel / Sitemap formats.
 
     Called within main() in pyspeedinsights.app.
     Metrics results are only included if the category is performance.
     """
-    audits_base = _get_audits_base(json_resp)  # Location of audits in json response
-    metadata = _parse_metadata(json_resp, category)
-    audit_results = _parse_audits(audits_base)
+    json_err = "Malformed JSON response. Skipping Excel processing for URL: "
+    try:
+        audits_base = _get_audits_base(json_resp)  # Location of audits in json response
+        metadata = _parse_metadata(json_resp, category)
+        audit_results = _parse_audits(audits_base)
+    except JSONKeyError as err:
+        logger.error(f"{json_err}{err}", exc_info=True)
+        return {}
+
     if metrics is not None and category == "performance":
-        metrics_results = _parse_metrics(audits_base, metrics)
+        try:
+            metrics_results = _parse_metrics(audits_base, metrics)
+        except JSONKeyError as err:
+            logger.error(f"{json_err}{err}", exc_info=True)
+            return {}
     else:
+        logger.warning("Skipping metrics (not chosen or non-performance category)")
         metrics_results = None
 
     results: dict[str, Union[dict, None]] = {
         "metadata": metadata,
         "audit_results": audit_results,
         "metrics_results": metrics_results,
     }
+    logger.info("Response data processed for URL.")
     return results
 
 
 def _parse_metadata(json_resp: dict, category: str) -> dict[str, Union[str, int]]:
     """Parses various metadata from the JSON response to write to Excel."""
+    logger.info("Parsing metadata from JSON response.")
+
     json_base = json_resp["lighthouseResult"]
     strategy = json_base["configSettings"]["formFactor"]
     category_score = json_base["categories"][category]["score"]
     timestamp = _get_timestamp(json_resp)
 
     metadata = {
         "category": category,
@@ -68,14 +86,16 @@
 
     Scores from 0-100 are given for the numeric value of each audit.
 
     Returns:
         A dict of audit results with audit names as keys and tuples of length 2
         as values containing the audit scores and numeric values, respectively.
     """
+    logger.info("Parsing audit data from JSON response.")
+
     audit_results = {}
     # Create results dict with scores and numerical values for each audit.
     for k in audits_base.keys():
         score = audits_base[k].get("score")
         if score is not None:
             num_value = audits_base[k].get("numericValue", "n/a")
             audit_results[k] = (score * 100, num_value)
@@ -93,19 +113,21 @@
     Metrics have no scores associated with them.
 
     Returns:
         A dict of metrics results with metric names as keys
         and int or float metrics as values.
     """
     if "all" in metrics:
+        logger.info("Parsing all metrics.")
         metrics_to_use = copy.copy(COMMAND_CHOICES["metrics"])
         # Remove 'all' to avoid key errors, as it doesn't exist in JSON resp.
         if type(metrics_to_use) == list:
             metrics_to_use.remove("all")
     else:
+        logger.info("Parsing chosen metrics.")
         metrics_to_use = metrics
 
     # Create new dict of metrics based on user's chosen metrics.
     metrics_results = {}
     metrics_loc = audits_base["metrics"]["details"]["items"][0]
     metrics_results = {field: metrics_loc[field] for field in metrics_to_use}
     # Sort dict alphabetically so each metric is written to Excel in the same order.
@@ -121,14 +143,23 @@
     """Parses the timestamp of the analysis from the JSON response.
 
     Converts the timestamp to a Python datetime object.
 
     Returns:
         A str in format year-month-day_hour.minute.second.
     """
-    timestamp = json_resp["analysisUTCTimestamp"]
+    logger.info("Parsing timestamp from JSON response.")
+    time_format = "%Y-%m-%d_%H.%M.%S"
+
+    try:
+        timestamp = json_resp["analysisUTCTimestamp"]
+    except JSONKeyError:
+        logger.warning("Unable to parse timestamp. Falling back to local time.")
+        date = datetime.now().strftime(time_format)
+        return date
+
     ts_no_fractions = timestamp.split(".")[0]  # Remove fraction
     if ts_no_fractions[-1] != "Z":
         ts_no_fractions += "Z"  # Add Z back after fraction removal
     dt_object = datetime.strptime(ts_no_fractions, "%Y-%m-%dT%H:%M:%SZ")
-    date = dt_object.strftime("%Y-%m-%d_%H.%M.%S")
+    date = dt_object.strftime(time_format)
     return date
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/cli/choices.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/cli/choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         "vi",
     ),
     "format": ("json", "excel", "sitemap"),
     # `all` is used as an arg to include all metrics in the Excel output
     # This must be a list instead of tuple so "all" can be removed from it
     "metrics": [
         "all",
-        "observedTotalCumulativeLayoutShift",
         "observedCumulativeLayoutShift",
         "observedLargestContentfulPaintAllFrames",
         "maxPotentialFID",
         "observedSpeedIndexTs",
         "observedFirstContentfulPaintTs",
         "observedTimeOrigin",
         "observedFirstPaint",
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/cli/commands.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/cli/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,30 +3,33 @@
 Typical usage example:
     parser = set_up_arg_parser()
     args = parse_args(parser)
     arg_groups = create_arg_groups(parser, args)
     arg_group_dict = arg_group_to_dict(arg_groups, "Group Name")
 """
 
+import logging
 from argparse import ArgumentParser, Namespace
 from typing import Any, TypeAlias, Union
 
 from .choices import COMMAND_CHOICES
 
 ArgGroups: TypeAlias = dict[str, Namespace]
+logger = logging.getLogger(__name__)
 
 
 def set_up_arg_parser() -> ArgumentParser:
     """Sets up argument parser with grouped command line arguments.
 
     Commands are used in PSI API request query params and response processing.
 
     Returns:
         An argparse.ArgumentParser instance with 2 argument groups.
     """
+    logger.info("Setting up CLI arguments.")
     parser = ArgumentParser(prog="pyspeedinsights")
 
     # Add argument options for default API call query params.
     api_group = parser.add_argument_group("API Group")
     api_group.add_argument(
         "url", help="The URL or sitemap URL of the site being analyzed."
     )
@@ -118,14 +121,15 @@
     """Creates separate namespaces for each arg group.
 
     Allows for separately passing each arg group as kwargs to a func or cls.
 
     Returns:
         A dict with group names as keys and argparse.Namespace instances as values.
     """
+    logger.info("Creating CLI argument groups.")
     arg_groups = {}
     for group in parser._action_groups:
         group_dict = {a.dest: getattr(args, a.dest, None) for a in group._group_actions}
         title = group.title
         if title:
             arg_groups[title] = Namespace(**group_dict)
     return arg_groups
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/core/excel.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/core/excel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Excel workbook operations for writing PSI API results to Excel."""
 
+import logging
 from dataclasses import dataclass, field
 from typing import Any, TypeAlias, Union, cast
 
 from xlsxwriter import Workbook
 from xlsxwriter.format import Format
 
 AuditResults: TypeAlias = dict[str, tuple[Union[int, float]]]
 MetricsResults: TypeAlias = Union[dict[str, Union[int, float]], None]
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class ExcelWorkbook:
     """Class for creating an Excel Workbook and writing the PSI API results to it."""
 
     url: str
     metadata: dict[str, Any]
@@ -23,20 +26,23 @@
     cur_cell: list[int] = field(default_factory=list)
     category_scores: list[int] = field(default_factory=list)
 
     def set_up_worksheet(self) -> None:
         """Creates the workbook, adds a worksheet, and sets up column headings."""
         self._create_workbook()
         self.worksheet = self.workbook.add_worksheet()
+        logger.info("Excel worksheet created in workbook.")
+
         self.cur_cell = [0, 0]
         row, col = self.cur_cell  # First cell
         column_format = self._column_format()
         metadata_format = self._metadata_format()
 
         # Add metadata to the first cell of the Excel sheet.
+        logger.info("Writing metadata to worksheet.")
         category = self.metadata["category"].upper()
         strategy = self.metadata["strategy"].upper()
         metadata_value = f"{strategy} {category} REPORT"
         self.worksheet.write(row, col, metadata_value, metadata_format)
 
         # Add the URL heading with a wider column of merged cells.
         row += 2
@@ -50,79 +56,87 @@
         # Add a column heading to record each page's overall category score.
         col += url_col_width + 1
         self.worksheet.write(row, col, "OVR", column_format)
         self.cur_cell = [row, col]  # Set current cell for later use
 
     def write_to_worksheet(self, first_resp: bool) -> None:
         """Writes the URL, OVR page score, audit and metrics results to the sheet."""
-        if self.worksheet is not None:
-            self._write_page_url()
-            self._write_overall_category_score()
-            self._write_audit_results(self.audit_results, first_resp)
-            self._write_metrics_results(self.metrics_results, first_resp)
-
-            self.cur_cell[0] += 1  # Move down 1 row for next page's results
-            self.cur_cell[1] = 5  # Reset to first results column
-        else:
-            raise ValueError("The worksheet is not set up.")
+        if self.worksheet is None:
+            # Fallback if worksheet doesn't exist for some reason
+            logger.warning("Worksheet not found. Creating.")
+            self.set_up_worksheet()
+
+        self._write_page_url()
+        self._write_overall_category_score()
+        self._write_audit_results(self.audit_results, first_resp)
+        self._write_metrics_results(self.metrics_results, first_resp)
+
+        self.cur_cell[0] += 1  # Move down 1 row for next page's results
+        self.cur_cell[1] = 5  # Reset to first results column
 
     def finalize_and_save(self) -> None:
-        """Writes the average score to the workbook and saves/closes it."""
+        """Writes the average score to the worksheet and saves/closes it."""
         self._write_average_score()
         self.workbook.close()
-        print("Workbook saved. Check your current directory!")
+        logger.info("Workbook saved. Check your current directory!")
 
     def _create_workbook(self) -> None:
         """Creates an Excel workbook with a unique and descriptive name."""
         strategy = self.metadata["strategy"]
         category = self.metadata["category"]
         date = self.metadata["timestamp"]
         self.workbook = Workbook(f"psi-s-{strategy}-c-{category}-{date}.xlsx")
+        logger.info("Excel workbook created.")
 
     def _write_page_url(self) -> None:
         """Writes the requested page URL being analyzed to the sheet."""
+        logger.info("Writing page URL to worksheet.")
         url_format = self._url_format()
         row = self.cur_cell[0] + 2
         self.worksheet.merge_range(
             row, 0, row, self.cur_cell[1] - 1, self.url, url_format
         )
 
     def _write_overall_category_score(self) -> None:
         """Writes the OVR category score for the page to the sheet."""
+        logger.info("Writing overall category score to worksheet.")
         category_score = self.metadata["category_score"] * 100
         cat_score_format = self._score_format(category_score)
 
         self.worksheet.write(
             self.cur_cell[0] + 2, self.cur_cell[1], category_score, cat_score_format
         )
         self.cur_cell[1] += 2
         # Add the score to a list so they can all be averaged at the end.
         self.category_scores.append(category_score)
 
     def _write_average_score(self) -> None:
         """Writes the average score next to the worksheet metadata."""
+        logger.info("Writing average score to worksheet.")
         scores = self.category_scores
         avg_score = sum(scores) / len(scores)
         avg_score = round(avg_score, 2)
         format = self._metadata_format()
         self.worksheet.write(0, 4, f"Avg Score: {avg_score}", format)
 
     def _write_audit_results(
         self, audit_results: AuditResults, first_resp: bool
     ) -> None:
         """Iterates through the audit results and writes them to the worksheet."""
         column_format = self._column_format()
         row, col = self.cur_cell
 
+        logger.info("Writing audit results to worksheet.")
         for title, scores in audit_results.items():
             self.worksheet.set_column(col, col + 1, 15)
             # cast() is a mypy workaround for issue #1178
             score, value = cast(tuple[Any, Any], scores)
             score_format = self._score_format(score)
             if first_resp:
+                logger.debug("Writing audit result headings to worksheet.")
                 self._write_results_headings(
                     row, col, title, column_format, result_type="audit"
                 )
             self.worksheet.write(row + 2, col, score, score_format)
             self.worksheet.write(row + 2, col + 1, value, score_format)
             col += 2
 
@@ -133,17 +147,19 @@
     ) -> None:
         """Iterates through the metrics results and writes them to the worksheet."""
         column_format = self._column_format()
         data_format = self._data_format()
         row, col = self.cur_cell
 
         if metrics_results is not None:
+            logger.info("Writing metrics results to worksheet.")
             for title, score in metrics_results.items():
                 self.worksheet.set_column(col, col, 30)
                 if first_resp:
+                    logger.debug("Writing metrics result headings to worksheet.")
                     self._write_results_headings(
                         row, col, title, column_format, result_type="metrics"
                     )
                 self.worksheet.write(row + 2, col, score, data_format)
                 col += 1
 
     def _write_results_headings(
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/core/sitemap.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/core/sitemap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,156 @@
 """Requesting and parsing of sitemaps to obtain request URLs for API calls.
 
 Includes support for recursive parsing of multiple sitemaps via a sitemap index.
 """
 
-import xml.etree.ElementTree as ET
+import logging
 from os.path import splitext
-from typing import Optional
+from typing import Any, Optional, TypeAlias
 from urllib.parse import urlsplit
 
+import defusedxml.ElementTree as ET
 import requests
 
 from ..utils.urls import validate_url
 
+XMLElement: TypeAlias = Any
+logger = logging.getLogger(__name__)
+
+
+class SitemapError(Exception):
+    """A base class for Sitemap exceptions."""
+
+
+class SitemapRetrievalError(SitemapError):
+    """A class for Sitemap retrieval exceptions."""
+
+
+class SitemapParseError(SitemapError):
+    """A class for Sitemap parsing exceptions."""
+
 
 def request_sitemap(url: str) -> str:
     """Retrieves the sitemap from the given URL.
 
     Validates the url format and whether the url is a valid sitemap.
     Makes a get request to retrieve the sitemap content in XML format.
 
     Returns:
         A str with XML sitemap text content.
     Raises:
-        SystemExit: The sitemap URL is invalid or a request failed.
+        SitemapRetrievalError: The sitemap URL is invalid or a request failed.
     """
     url = validate_url(url)
     # Set a dummy user agent to avoid bot detection by firewalls
     # e.g. CloudFlare issues a 403 if it detects the default requests module user-agent
     dummy_user_agent = (
         "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) "
         "AppleWebKit/537.36 (KHTML, like Gecko) "
         "Chrome/104.0.5112.79 Safari/537.36"
     )
     headers = {"user-agent": dummy_user_agent}
 
+    # Below errors logged as CRITICAL in main() before exit
+    logger.info("Checking if sitemap URL is a valid sitemap URL.")
     if not validate_sitemap_url(url):
         err = (
             "Invalid sitemap URL provided. Please provide a URL to a valid XML sitemap."
         )
-        raise SystemExit(err)
+        raise SitemapRetrievalError(err)
     try:
-        print(f"Requesting sitemap... ({url})")
-        resp = requests.get(url, headers=headers)
+        logger.info(f"Requesting sitemap ({url})")
+        resp = requests.get(url, headers=headers, timeout=(3.05, 5))
         resp.raise_for_status()
     except requests.exceptions.HTTPError as errh:
-        raise SystemExit(f"HTTP Error: {errh}")
+        raise SitemapRetrievalError(f"HTTP Error: {errh}")
     except requests.exceptions.ConnectionError as errc:
-        raise SystemExit(f"Connection Error: {errc}")
+        raise SitemapRetrievalError(f"Connection Error: {errc}")
     except requests.exceptions.Timeout as errt:
-        raise SystemExit(f"Timeout Error: {errt}")
+        raise SitemapRetrievalError(f"Timeout Error: {errt}")
     except requests.exceptions.RequestException as err:
-        raise SystemExit(f"Request Error: {err}")
+        raise SitemapRetrievalError(f"Request Error: {err}")
 
     sitemap = resp.text
-    print("Sitemap retrieval successful!")
+    logger.info("Sitemap retrieval successful.")
     return sitemap
 
 
 def validate_sitemap_url(url: str) -> bool:
     """Checks that the sitemap URL is valid (.xml format)."""
     u = urlsplit(url)
     ext = splitext(u.path)[-1]
     return ext == ".xml"
 
 
-def get_sitemap_root(sitemap: str) -> ET.Element:
+def get_sitemap_root(sitemap: str) -> XMLElement:
     """Gets the root element of the sitemap."""
+    logger.info("Locating sitemap root.")
     return ET.fromstring(sitemap)
 
 
-def get_sitemap_type(root: ET.Element) -> str:
+def get_sitemap_type(root: XMLElement) -> str:
     """Gets the tag value of the root element to determine sitemap type."""
+    logger.info("Getting sitemap type.")
     return root.tag.split("}")[-1]
 
 
 def process_sitemap(sitemap: str) -> list[Optional[str]]:
     """Processes a sitemap or sitemap index based on type.
 
     Multiple sitemaps are processed recursively via a sitemap index.
 
     Returns:
         A full list of request URLs for use in requests.
     Raises:
-        SystemExit: The sitemap type couldn't be parsed from the root element.
+        SitemapParseError: The sitemap type couldn't be parsed from the root element.
                     The sitemap type parsed from the root element is invalid.
                     No URLs were parsed from the sitemap(s) successfully.
     """
     err = "Sitemap format invalid."
+    logger.info("Processing sitemap.")
 
     try:
         root = get_sitemap_root(sitemap)
         sitemap_type = get_sitemap_type(root)
     except ET.ParseError:
-        raise SystemExit(err)
+        raise SitemapParseError(err)  # Logged in main()
 
     if sitemap_type == "sitemapindex":
+        logger.info("Sitemap index detected. Recursively parsing children.")
         request_urls = []
         sitemap_urls = _parse_sitemap_index(root)
         for sm_url in sitemap_urls:
             if sm_url is not None:
                 sitemap = request_sitemap(sm_url)
                 request_urls.extend(process_sitemap(sitemap))
     elif sitemap_type == "urlset":
+        logger.info("Standard sitemap detected.")
         request_urls = _parse_sitemap_urls(root)
     else:
-        raise SystemExit(err)
+        raise SitemapParseError(err)  # Logged in main()
 
     if not request_urls:
-        raise SystemExit("No URLs found in the sitemap(s).")
+        raise SitemapParseError("No URLs found in the sitemap(s).")  # Logged in main()
     return request_urls
 
 
-def _parse_sitemap_index(root: ET.Element) -> list[Optional[str]]:
+def _parse_sitemap_index(root: XMLElement) -> list[Optional[str]]:
     """Parse sitemap URLs from the sitemap index and return them as a list."""
-    print("Sitemap index found. Parsing sitemap URLs...")
+    logger.info("Parsing child sitemap URLs from index.")
     return _parse_urls_from_root(root, type="sitemap")
 
 
-def _parse_sitemap_urls(root: ET.Element) -> list[Optional[str]]:
+def _parse_sitemap_urls(root: XMLElement) -> list[Optional[str]]:
     """Parse URLs from the XML sitemap and return a list of request URLs."""
-    print("Parsing URLs from sitemap...")
+    logger.info("Parsing URLs from sitemap.")
     return _parse_urls_from_root(root)
 
 
-def _parse_urls_from_root(root: ET.Element, type: str = "url") -> list[Optional[str]]:
+def _parse_urls_from_root(root: XMLElement, type: str = "url") -> list[Optional[str]]:
     """Parse URL locs from root xml element."""
     namespace = "{http://www.sitemaps.org/schemas/sitemap/0.9}"
     urls = []
     for el in root.findall(f"{namespace}{type}"):
         loc = el.find(f"{namespace}loc")
         if loc is not None:
             urls.append(loc.text)
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights/utils/urls.py` & `pyspeedinsights-0.4.0/src/pyspeedinsights/utils/urls.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,39 +1,51 @@
 """Utilities for URL processing."""
 
+import logging
 from urllib.parse import urlsplit
 
+logger = logging.getLogger(__name__)
+
+
+class InvalidURLError(Exception):
+    """A base exception for an invalid URL format."""
+
 
 def validate_url(url: str) -> str:
     """Checks that a URL is valid and fully-qualified.
 
     Adds a scheme to the URL if missing.
     The hostname is stored in u.path instead of u.netloc when the URL str has no path.
     In this scenario, checking the u.path is necessary to ensure the URL has a domain
     and the path doesn't precede the hostname (e.g. path/example.com).
 
     Returns:
         The sanitized URL as a str.
     Raises:
-        SystemExit: The user entered a URL without a path that has no domain
+        InvalidURLError: The user entered a URL without a path that has no domain
         or a URL whose path precedes the hostname (e.g. path/example.com).
     """
+    logger.info("Checking if request URL is a valid URL.")
     err = "Invalid URL. Please enter a valid fully-qualified URL."
+
     replacements = {}
     u = urlsplit(url)
 
     if not u.scheme:
         replacements["scheme"] = "https"
     if not u.netloc:
         p_sep, dot = u.path.find("/"), u.path.find(".")
         path_before_host = p_sep < dot and p_sep > 0
         no_host = "." not in u.path
         if path_before_host or no_host:
-            raise SystemExit(err)
+            raise InvalidURLError(err)  # Logged as CRITICAL in main()
         else:
             replacements["netloc"] = u.path
             replacements["path"] = ""
+    elif "." not in u.netloc:
+        # URLs with schemes but no TLD
+        raise InvalidURLError(err)  # Logged as CRITICAL in main()
 
     replacements["fragment"] = ""
     replacements["query"] = ""
     u = u._replace(**replacements)
     return u.geturl()
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/PKG-INFO` & `pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspeedinsights
-Version: 0.3.2
+Version: 0.4.0
 Summary: Measure your site speed, performance, accessibility and SEO in bulk from the command line with Python and the PageSpeed Insights API.
 Home-page: https://github.com/wjh18/pyspeedinsights
 Author: Will J. Holmes
 Author-email: will@wjholmes.com
 Project-URL: Documentation, https://github.com/wjh18/pyspeedinsights/blob/master/README.md
 Project-URL: Source, https://github.com/wjh18/pyspeedinsights
 Project-URL: Tracker, https://github.com/wjh18/pyspeedinsights/issues
@@ -235,15 +235,14 @@
 * `psi https://example.com -f excel` - no metrics
 * `psi https://example.com -f excel -m all` - all available metrics
 * `psi https://example.com -f excel -m speedIndex` - just speedIndex
 * `psi https://example.com -f excel -m speedIndex totalBlockingTime` - just speedIndex and totalBlockingTime
 
 Full list of available metrics:
 
-* `observedTotalCumulativeLayoutShift`
 * `observedCumulativeLayoutShift`
 * `observedLargestContentfulPaintAllFrames`
 * `maxPotentialFID`
 * `observedSpeedIndexTs`
 * `observedFirstContentfulPaintTs`
 * `observedTimeOrigin`
 * `observedFirstPaint`
```

### Comparing `pyspeedinsights-0.3.2/src/pyspeedinsights.egg-info/SOURCES.txt` & `pyspeedinsights-0.4.0/src/pyspeedinsights.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -18,9 +18,10 @@
 src/pyspeedinsights/cli/__init__.py
 src/pyspeedinsights/cli/choices.py
 src/pyspeedinsights/cli/commands.py
 src/pyspeedinsights/core/__init__.py
 src/pyspeedinsights/core/excel.py
 src/pyspeedinsights/core/sitemap.py
 src/pyspeedinsights/utils/__init__.py
+src/pyspeedinsights/utils/exceptions.py
 src/pyspeedinsights/utils/generic.py
 src/pyspeedinsights/utils/urls.py
```

