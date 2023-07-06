# Comparing `tmp/captchaai-0.0.2.tar.gz` & `tmp/captchaai-0.0.3.tar.gz`

## Comparing `captchaai-0.0.2.tar` & `captchaai-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/__init__.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/api.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/setup.py
--rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 captchaai-0.0.2/src/captchaai/solver.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 captchaai-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 captchaai-0.0.2/README.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 captchaai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     8433 2020-02-02 00:00:00.000000 captchaai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 captchaai-0.0.3/src/captchaai/__init__.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 captchaai-0.0.3/src/captchaai/api.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 captchaai-0.0.3/src/captchaai/setup.py
+-rw-r--r--   0        0        0     8855 2020-02-02 00:00:00.000000 captchaai-0.0.3/src/captchaai/solver.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 captchaai-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     7464 2020-02-02 00:00:00.000000 captchaai-0.0.3/README.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 captchaai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 captchaai-0.0.3/PKG-INFO
```

### Comparing `captchaai-0.0.2/src/captchaai/api.py` & `captchaai-0.0.3/src/captchaai/api.py`

 * *Files identical despite different names*

### Comparing `captchaai-0.0.2/src/captchaai/setup.py` & `captchaai-0.0.3/src/captchaai/setup.py`

 * *Files identical despite different names*

### Comparing `captchaai-0.0.2/src/captchaai/solver.py` & `captchaai-0.0.3/src/captchaai/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,14 +184,15 @@
         if not file:
             raise ValidationException('File required')
 
         if not '.' in file and len(file) > 50:
             return {'method': 'base64', 'body': file}
 
         if file.startswith('http'):
+            print('file starts with http')
             img_resp = requests.get(file)
             if img_resp.status_code != 200:
                 raise ValidationException(f'File could not be downloaded from url: {file}')
             return {'method': 'base64', 'body': b64encode(img_resp.content).decode('utf-8')}
 
         if not os.path.exists(file):
             raise ValidationException(f'File not found: {file}')
```

### Comparing `captchaai-0.0.2/LICENSE.txt` & `captchaai-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `captchaai-0.0.2/README.md` & `captchaai-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,34 +36,29 @@
 solver = captchaAI('YOUR_API_KEY')
 ```
 Also there are few options that can be configured:
 
 ```python 
 config = {
             'apiKey':           'YOUR_API_KEY',
-            'softId':            123,
-            'callback':         'https://your.site/result-receiver',
             'defaultTimeout':    120,
-            'recaptchaTimeout':  600,
+            'recaptchaTimeout':  240,
             'pollingInterval':   10,
         }
 solver = captchaAI(**config)
 ```
 
 ### captchaAI instance options
 
 | Option           | Default value  | Description                                                                                                                                        |
 | ---------------- | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
-| softId           | -              | your software ID obtained after publishing in [captchaAI sofware catalog]                                                                           |
 | defaultTimeout   | 120            | Polling timeout in seconds for all captcha types except ReCaptcha. Defines how long the module tries to get the answer from `res.php` API endpoint |
 | recaptchaTimeout | 240            | Polling timeout for ReCaptcha in seconds. Defines how long the module tries to get the answer from `res.php` API endpoint                          |
 | pollingInterval  | 10             | Interval in seconds between requests to `res.php` API endpoint, setting values less than 5 seconds is not recommended                              |
 
->  **IMPORTANT:** once `callback` is defined for `captchaAI` instance, all methods return only the captcha ID and DO NOT poll the API to get the result. The result will be sent to the callback URL.
-To get the answer manually use [getResult method](#send--getresult)
 
 ## Solve captcha
 When you submit any image-based captcha use can provide additional options to help captchaAI workers to solve it properly.
 
 ### Captcha options
 | Option        | Default Value | Description                                                                                        |
 | ------------- | ------------- | -------------------------------------------------------------------------------------------------- |
@@ -142,15 +137,15 @@
 solver.report(id, False) # captcha solved incorrectly
 ```
 
 ### Error handling
 In case of an error, the captcha solver throws an exception. It's important to properly handle these cases. We recommend using `try except` to handle exceptions. 
 ```python
 try:
-    result = solver.text('If tomorrow is Saturday, what day is today?')
+    result = solver.recaptcha(sitekey=site_key,url=url)
 except ValidationException as e:
     # invalid parameters passed
 	print(e)
 except NetworkException as e:
 	# network error occurred
 	print(e)
 except ApiException as e:
```

### Comparing `captchaai-0.0.2/pyproject.toml` & `captchaai-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "captchaai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="captchaai developers", email="dev@captchaai.com" },
 ]
 description = "A package to enable interacting with the api of captchaai.com by python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `captchaai-0.0.2/PKG-INFO` & `captchaai-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captchaai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package to enable interacting with the api of captchaai.com by python.
 Project-URL: Homepage, https://github.com/captchaai-developers/captchaai
 Project-URL: Bug Tracker, https://github.com/captchaai-developers/captchaai/issues
 Author-email: captchaai developers <dev@captchaai.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -50,34 +50,29 @@
 solver = captchaAI('YOUR_API_KEY')
 ```
 Also there are few options that can be configured:
 
 ```python 
 config = {
             'apiKey':           'YOUR_API_KEY',
-            'softId':            123,
-            'callback':         'https://your.site/result-receiver',
             'defaultTimeout':    120,
-            'recaptchaTimeout':  600,
+            'recaptchaTimeout':  240,
             'pollingInterval':   10,
         }
 solver = captchaAI(**config)
 ```
 
 ### captchaAI instance options
 
 | Option           | Default value  | Description                                                                                                                                        |
 | ---------------- | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
-| softId           | -              | your software ID obtained after publishing in [captchaAI sofware catalog]                                                                           |
 | defaultTimeout   | 120            | Polling timeout in seconds for all captcha types except ReCaptcha. Defines how long the module tries to get the answer from `res.php` API endpoint |
 | recaptchaTimeout | 240            | Polling timeout for ReCaptcha in seconds. Defines how long the module tries to get the answer from `res.php` API endpoint                          |
 | pollingInterval  | 10             | Interval in seconds between requests to `res.php` API endpoint, setting values less than 5 seconds is not recommended                              |
 
->  **IMPORTANT:** once `callback` is defined for `captchaAI` instance, all methods return only the captcha ID and DO NOT poll the API to get the result. The result will be sent to the callback URL.
-To get the answer manually use [getResult method](#send--getresult)
 
 ## Solve captcha
 When you submit any image-based captcha use can provide additional options to help captchaAI workers to solve it properly.
 
 ### Captcha options
 | Option        | Default Value | Description                                                                                        |
 | ------------- | ------------- | -------------------------------------------------------------------------------------------------- |
@@ -156,15 +151,15 @@
 solver.report(id, False) # captcha solved incorrectly
 ```
 
 ### Error handling
 In case of an error, the captcha solver throws an exception. It's important to properly handle these cases. We recommend using `try except` to handle exceptions. 
 ```python
 try:
-    result = solver.text('If tomorrow is Saturday, what day is today?')
+    result = solver.recaptcha(sitekey=site_key,url=url)
 except ValidationException as e:
     # invalid parameters passed
 	print(e)
 except NetworkException as e:
 	# network error occurred
 	print(e)
 except ApiException as e:
```

