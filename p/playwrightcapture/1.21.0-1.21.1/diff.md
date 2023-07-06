# Comparing `tmp/playwrightcapture-1.21.0.tar.gz` & `tmp/playwrightcapture-1.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.21.0.tar", max compression
+gzip compressed data, was "playwrightcapture-1.21.1.tar", max compression
```

## Comparing `playwrightcapture-1.21.0.tar` & `playwrightcapture-1.21.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.21.0/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.21.0/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.21.0/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    37664 2023-06-26 17:28:11.136863 playwrightcapture-1.21.0/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.21.0/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.21.0/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.21.0/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1826 2023-06-30 14:13:31.901153 playwrightcapture-1.21.0/pyproject.toml
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 playwrightcapture-1.21.0/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.21.1/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.21.1/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.21.1/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    37961 2023-07-04 14:22:13.898654 playwrightcapture-1.21.1/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.21.1/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     1734 2023-06-06 09:15:52.098307 playwrightcapture-1.21.1/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.21.1/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1840 2023-07-06 13:08:27.903638 playwrightcapture-1.21.1/pyproject.toml
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 playwrightcapture-1.21.1/PKG-INFO
```

### Comparing `playwrightcapture-1.21.0/LICENSE` & `playwrightcapture-1.21.1/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.21.0/README.md` & `playwrightcapture-1.21.1/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.21.0/playwrightcapture/capture.py` & `playwrightcapture-1.21.1/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,29 +588,35 @@
                 self.should_retry = True
             else:
                 # Unexpected ones
                 self.logger.exception(f'Something went poorly with {url}: {e.message}')
         except Exception as e:
             # we may get a non-playwright exception to.
             # The ones we try to handle here should be treated as if they were.
-            if str(e) in ['Connection closed while reading from the driver']:
+            to_return['error'] = str(e)
+            if to_return['error'] in ['Connection closed while reading from the driver']:
                 self.logger.info(f'Issue with {url} (retrying): {e}')
                 self.should_retry = True
             else:
                 raise e
         finally:
             if not capturing_sub:
-                to_return['cookies'] = await self.context.cookies()
+                try:
+                    to_return['cookies'] = await self.context.cookies()
+                except Exception as e:
+                    if 'error' not in to_return:
+                        to_return['error'] = f'Unable to get the cookies: {e}'
                 # frames_tree = self.make_frame_tree(page.main_frame)
                 try:
                     await self.context.close()  # context needs to be closed to generate the HAR
                     with open(self._temp_harfile.name) as _har:
                         to_return['har'] = json.load(_har)
                 except Exception as e:
-                    to_return['error'] = f'Unable to generate HAR file: {e}'
+                    if 'error' not in to_return:
+                        to_return['error'] = f'Unable to generate HAR file: {e}'
         self.logger.debug('Capture done')
         return to_return
 
     async def _failsafe_get_screenshot(self, page: Page) -> bytes:
         try:
             return await page.screenshot(full_page=True)
         except Error as e:
```

### Comparing `playwrightcapture-1.21.0/playwrightcapture/helpers.py` & `playwrightcapture-1.21.1/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.21.0/pyproject.toml` & `playwrightcapture-1.21.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.21.0"
+version = "1.21.1"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
@@ -19,17 +19,16 @@
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 playwright = "^1.35.0"
 dateparser = "^1.1.8"
-beautifulsoup4 = "^4.12.2"
+beautifulsoup4 = {version= "^4.12.2", extras = ["lxml"]}
 w3lib = "^2.1.1"
-lxml = "^4.9.2"
 requests = {version = "^2.31.0", optional = true}
 pydub = {version = "^0.25.1", optional = true}
 SpeechRecognition = {version = "^3.10.0", optional = true}
 pytz = {"version" = "^2023.3", python = "<3.9"}
 tzdata = "^2023.3"
 
 [tool.poetry.extras]
```

### Comparing `playwrightcapture-1.21.0/PKG-INFO` & `playwrightcapture-1.21.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.21.0
+Version: 1.21.1
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -16,17 +16,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: recaptcha
 Requires-Dist: SpeechRecognition (>=3.10.0,<4.0.0) ; extra == "recaptcha"
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: beautifulsoup4[lxml] (>=4.12.2,<5.0.0)
 Requires-Dist: dateparser (>=1.1.8,<2.0.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
 Requires-Dist: playwright (>=1.35.0,<2.0.0)
 Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "recaptcha"
 Requires-Dist: pytz (>=2023.3,<2024.0) ; python_version < "3.9"
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "recaptcha"
 Requires-Dist: tzdata (>=2023.3,<2024.0)
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/Lookyloo/PlaywrightCapture
```

