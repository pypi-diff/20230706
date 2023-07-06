# Comparing `tmp/pybenutils-3.1.0.tar.gz` & `tmp/pybenutils-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybenutils-3.1.0.tar", last modified: Mon Oct  3 19:59:51 2022, max compression
+gzip compressed data, was "pybenutils-3.2.2.tar", last modified: Thu Jul  6 12:21:00 2023, max compression
```

## Comparing `pybenutils-3.1.0.tar` & `pybenutils-3.2.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.231918 pybenutils-3.1.0/
--rw-r--r--   0 bemoskov   (501) staff       (20)     1071 2022-10-02 20:30:27.000000 pybenutils-3.1.0/LICENSE
--rw-r--r--   0 bemoskov   (501) staff       (20)       26 2022-10-02 20:30:27.000000 pybenutils-3.1.0/MANIFEST.in
--rw-r--r--   0 bemoskov   (501) staff       (20)     2963 2022-10-03 19:59:51.236307 pybenutils-3.1.0/PKG-INFO
--rw-r--r--   0 bemoskov   (501) staff       (20)     2384 2022-10-03 19:49:38.000000 pybenutils-3.1.0/README.md
--rw-r--r--   0 bemoskov   (501) staff       (20)       54 2022-10-02 20:30:27.000000 pybenutils-3.1.0/deploy_requirements.txt
--rw-r--r--   0 bemoskov   (501) staff       (20)      543 2022-10-02 20:30:27.000000 pybenutils-3.1.0/deployment_checklist.md
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.140923 pybenutils-3.1.0/pybenutils/
--rw-r--r--   0 bemoskov   (501) staff       (20)      149 2022-10-02 20:31:51.000000 pybenutils-3.1.0/pybenutils/__init__.py
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.148763 pybenutils-3.1.0/pybenutils/amazon_boto3/
--rw-r--r--   0 bemoskov   (501) staff       (20)        0 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/amazon_boto3/__init__.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     7543 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/amazon_boto3/amazon_obj.py
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.152137 pybenutils-3.1.0/pybenutils/autogui/
--rw-r--r--   0 bemoskov   (501) staff       (20)        0 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/autogui/__init__.py
--rw-r--r--   0 bemoskov   (501) staff       (20)      988 2022-10-03 19:34:33.000000 pybenutils-3.1.0/pybenutils/autogui/__main__.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     5332 2022-10-03 19:45:07.000000 pybenutils-3.1.0/pybenutils/autogui/auto_gui_cls.py
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.168817 pybenutils-3.1.0/pybenutils/browsers/
--rw-r--r--   0 bemoskov   (501) staff       (20)        0 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/browsers/__init__.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     1531 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/browsers/chrome.py
--rw-r--r--   0 bemoskov   (501) staff       (20)      916 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/browsers/firefox.py
--rw-r--r--   0 bemoskov   (501) staff       (20)    23223 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/browsers/selenium_utils.py
--rw-r--r--   0 bemoskov   (501) staff       (20)    18629 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/browsers/simple_browser_controller_cls.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     2091 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/browsers/web_driver.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     9218 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/browsers/windows_browsers_keywords.py
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.192000 pybenutils-3.1.0/pybenutils/network/
--rw-r--r--   0 bemoskov   (501) staff       (20)        0 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/network/__init__.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     1880 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/network/download_manager.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     3250 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/network/http_cert_info.py
--rw-r--r--   0 bemoskov   (501) staff       (20)    10435 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/network/s3_bucket_cls.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     6897 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/network/ssh_helper.py
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.226573 pybenutils-3.1.0/pybenutils/os_operations/
--rw-r--r--   0 bemoskov   (501) staff       (20)        0 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/os_operations/__init__.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     1241 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/os_operations/files_and_directories.py
--rw-r--r--   0 bemoskov   (501) staff       (20)    18345 2022-10-02 20:55:15.000000 pybenutils-3.1.0/pybenutils/os_operations/mac_application_control.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     1418 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/os_operations/mac_input_control.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     5380 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/os_operations/mac_operations.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     3670 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/os_operations/mac_popup_handler.py
--rw-r--r--   0 bemoskov   (501) staff       (20)    11465 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/os_operations/process.py
--rw-r--r--   0 bemoskov   (501) staff       (20)    10048 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/os_operations/window_operations.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     2250 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/useful.py
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.230658 pybenutils-3.1.0/pybenutils/utils_logger/
--rw-r--r--   0 bemoskov   (501) staff       (20)        0 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/utils_logger/__init__.py
--rw-r--r--   0 bemoskov   (501) staff       (20)     1351 2022-10-02 20:30:27.000000 pybenutils-3.1.0/pybenutils/utils_logger/config_logger.py
-drwxr-xr-x   0 bemoskov   (501) staff       (20)        0 2022-10-03 19:59:51.145498 pybenutils-3.1.0/pybenutils.egg-info/
--rw-r--r--   0 bemoskov   (501) staff       (20)     2963 2022-10-03 19:59:50.000000 pybenutils-3.1.0/pybenutils.egg-info/PKG-INFO
--rw-r--r--   0 bemoskov   (501) staff       (20)     1373 2022-10-03 19:59:50.000000 pybenutils-3.1.0/pybenutils.egg-info/SOURCES.txt
--rw-r--r--   0 bemoskov   (501) staff       (20)        1 2022-10-03 19:59:50.000000 pybenutils-3.1.0/pybenutils.egg-info/dependency_links.txt
--rw-r--r--   0 bemoskov   (501) staff       (20)      213 2022-10-03 19:59:50.000000 pybenutils-3.1.0/pybenutils.egg-info/requires.txt
--rw-r--r--   0 bemoskov   (501) staff       (20)       11 2022-10-03 19:59:50.000000 pybenutils-3.1.0/pybenutils.egg-info/top_level.txt
--rw-r--r--   0 bemoskov   (501) staff       (20)      256 2022-10-02 20:30:27.000000 pybenutils-3.1.0/requirements.txt
--rw-r--r--   0 bemoskov   (501) staff       (20)      232 2022-10-03 19:59:51.242669 pybenutils-3.1.0/setup.cfg
--rw-r--r--   0 bemoskov   (501) staff       (20)     1910 2022-10-02 20:30:27.000000 pybenutils-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.955077 pybenutils-3.2.2/
+-rw-rw-rw-   0        0        0     1092 2023-07-06 12:04:25.000000 pybenutils-3.2.2/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-07-06 12:04:25.000000 pybenutils-3.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4061 2023-07-06 12:21:00.955077 pybenutils-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3465 2023-07-06 12:04:25.000000 pybenutils-3.2.2/README.md
+-rw-rw-rw-   0        0        0       60 2023-07-06 12:04:25.000000 pybenutils-3.2.2/deploy_requirements.txt
+-rw-rw-rw-   0        0        0      559 2023-07-06 12:04:25.000000 pybenutils-3.2.2/deployment_checklist.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.861329 pybenutils-3.2.2/pybenutils/
+-rw-rw-rw-   0        0        0      153 2023-07-06 12:12:38.000000 pybenutils-3.2.2/pybenutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.881276 pybenutils-3.2.2/pybenutils/amazon_boto3/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/amazon_boto3/__init__.py
+-rw-rw-rw-   0        0        0     7692 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/amazon_boto3/amazon_obj.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.889255 pybenutils-3.2.2/pybenutils/autogui/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/autogui/__init__.py
+-rw-rw-rw-   0        0        0     1468 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/autogui/__main__.py
+-rw-rw-rw-   0        0        0     5874 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/autogui/auto_gui_cls.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.910197 pybenutils-3.2.2/pybenutils/browsers/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/__init__.py
+-rw-rw-rw-   0        0        0     1562 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/chrome.py
+-rw-rw-rw-   0        0        0      939 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/firefox.py
+-rw-rw-rw-   0        0        0    25553 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/selenium_utils.py
+-rw-rw-rw-   0        0        0    19074 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/simple_browser_controller_cls.py
+-rw-rw-rw-   0        0        0     2156 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/web_driver.py
+-rw-rw-rw-   0        0        0     9474 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/browsers/windows_browsers_keywords.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.926155 pybenutils-3.2.2/pybenutils/network/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/__init__.py
+-rw-rw-rw-   0        0        0     1926 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/download_manager.py
+-rw-rw-rw-   0        0        0     3340 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/http_cert_info.py
+-rw-rw-rw-   0        0        0    10654 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/s3_bucket_cls.py
+-rw-rw-rw-   0        0        0     7073 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/network/ssh_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.946102 pybenutils-3.2.2/pybenutils/os_operations/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/__init__.py
+-rw-rw-rw-   0        0        0     1279 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/files_and_directories.py
+-rw-rw-rw-   0        0        0    18745 2023-07-06 12:12:38.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_application_control.py
+-rw-rw-rw-   0        0        0     1467 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_input_control.py
+-rw-rw-rw-   0        0        0     5506 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_operations.py
+-rw-rw-rw-   0        0        0     3749 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/mac_popup_handler.py
+-rw-rw-rw-   0        0        0    11748 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/process.py
+-rw-rw-rw-   0        0        0    10361 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/os_operations/window_operations.py
+-rw-rw-rw-   0        0        0     3103 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/useful.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.950091 pybenutils-3.2.2/pybenutils/utils_logger/
+-rw-rw-rw-   0        0        0        0 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/utils_logger/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-07-06 12:04:25.000000 pybenutils-3.2.2/pybenutils/utils_logger/config_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.876289 pybenutils-3.2.2/pybenutils.egg-info/
+-rw-rw-rw-   0        0        0     4061 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1399 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-06 12:21:00.000000 pybenutils-3.2.2/pybenutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      273 2023-07-06 12:04:25.000000 pybenutils-3.2.2/requirements.txt
+-rw-rw-rw-   0        0        0      243 2023-07-06 12:21:00.957073 pybenutils-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1965 2023-07-06 12:04:25.000000 pybenutils-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:21:00.953083 pybenutils-3.2.2/tests/
+-rw-rw-rw-   0        0        0      317 2023-07-06 12:04:25.000000 pybenutils-3.2.2/tests/test_self_import.py
```

### Comparing `pybenutils-3.1.0/LICENSE` & `pybenutils-3.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Ben Moskovitch
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Ben Moskovitch
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pybenutils-3.1.0/PKG-INFO` & `pybenutils-3.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,85 @@
-Metadata-Version: 2.1
-Name: pybenutils
-Version: 3.1.0
-Summary: PyBEN Utilities repository
-Home-page: https://github.com/DarkFlameBEN/pybenutils.git
-Author: Ben Moskovitch
-Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
-License: MIT License
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pybenutils
-PyBEN Utilities repository, Contains a variety of useful methods and classes designed to allow easy access to high level operations 
-
-### Installation
-> python -m pip install pybenutils -U
-> python3 -m pip install pybenutils -U
-
-### AutoGUI module
-PyBenAutoGui - Class to automate cross platform GUI interactions.
-```
-options:
-  -h, --help            show this help message and exit
-  -t TITLE, --title TITLE
-                        Window title
-  -a APP_PATH, --app_path APP_PATH
-                        Application/Exe path
-  -b PYWINAUTO_BACKEND, --pywinauto_backend PYWINAUTO_BACKEND
-                        A name of used back-end in Windows OS (values: "win32", "uia")
-  -c COMMAND, --command COMMAND
-                        Function name to execute in the AutoGui Class
-```
-
-> python -m pybenutils.autogui -t "Calculator" -a calc.exe -c get_object_details -b uia
-
-> python3 -m pybenutils.autogui -t "Calculator" -a /Application/Calculator.app -c get_object_details
-
-```
-class AutoGui(builtins.object)
- |  AutoGui(title, app_path, pywinauto_backend='uia')
- |  
- |  Methods defined here:
- |  
- |  __init__(self, title, app_path, pywinauto_backend='uia')
- |      Unified interface to interact with Gui Elements
- |      
- |      :param title: Window title
- |      :param app_path: Application/Exe path
- |      :param pywinauto_backend: A name of used back-end in Windows OS (values: "win32", "uia")
- |  
- |  click_on_text(self, text: str)
- |      Clicks on text object location using pyautogui
- |  
- |  find_objects(self, text='', control_type='')
- |      Returns an iterable containing the matching object
- |      
- |      :param text: Text to search, In windows can also be the automation_id
- |      :param control_type: Filter by control type
- |      :return: An iterable containing the matching object
- |  
- |  focus_on_window(self)
- |      Focus on the app window - bring to front
- |  
- |  get_object_details(self, text='', control_type='')
- |      Returns an iterable containing dicts of matching objects properties
- |      
- |      :param text: Text to search, In windows can also be the automation_id
- |      :param control_type: Filter by control type
- |      :return: An iterable containing dicts of matching objects properties
- |  
- |  get_object_position_by_text(self, text)
- |      Return position as tuple (xl, yt, xr, yb) in windows / (x, y) in mac
-```
+Metadata-Version: 2.1
+Name: pybenutils
+Version: 3.2.2
+Summary: PyBEN Utilities repository
+Home-page: https://github.com/DarkFlameBEN/pybenutils.git
+Author: Ben Moskovitch
+Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
+License: MIT License
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pybenutils
+PyBEN Utilities repository, Contains a variety of useful methods and classes designed to allow easy access to high level operations 
+
+### Installation
+Win:
+> python -m pip install pybenutils -U
+
+macOS:
+> python3 -m pip install pybenutils -U
+
+### AutoGUI module
+PyBenAutoGui - Class to automate cross platform GUI interactions.
+```
+options:                                                                                                                   
+  -h, --help            show this help message and exit                                                                    
+  -t TITLE, --title TITLE                                                                                                  
+                        Window title                                                                                       
+  -a APP_PATH, --app_path APP_PATH                                                                                         
+                        Application/Exe path                                                                               
+  -b PYWINAUTO_BACKEND, --pywinauto_backend PYWINAUTO_BACKEND                                                              
+                        A name of used back-end in Windows OS (values: "win32", "uia")                                     
+  -c COMMAND, --command COMMAND                                                                                            
+                        Function name to execute in the AutoGui Class                                                      
+  -eh, --extra_help, --no-extra_help                                                                                       
+                        Display extra help about the class and its functions (default: False)
+
+```
+
+> python -m pybenutils.autogui -t "Calculator" -a calc.exe -c get_object_details -b uia
+
+> python3 -m pybenutils.autogui -t "Calculator" -a /Application/Calculator.app -c get_object_details
+
+```
+class AutoGui(builtins.object)
+ |  AutoGui(title, app_path, pywinauto_backend='uia')
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, title, app_path, pywinauto_backend='uia')
+ |      Unified interface to interact with Gui Elements
+ |      
+ |      :param title: Window title
+ |      :param app_path: Application/Exe path
+ |      :param pywinauto_backend: A name of used back-end in Windows OS (values: "win32", "uia")
+ |  
+ |  click_on_text(self, text: str)
+ |      Clicks on text object location using pyautogui
+ |  
+ |  find_objects(self, text='', control_type='')
+ |      Returns an iterable containing the matching object
+ |      
+ |      :param text: Text to search, In windows can also be the automation_id
+ |      :param control_type: Filter by control type
+ |      :return: An iterable containing the matching object
+ |  
+ |  focus_on_window(self)
+ |      Focus on the app window - bring to front
+ |  
+ |  get_object_details(self, text='', control_type='')
+ |      Returns an iterable containing dicts of matching objects properties
+ |      
+ |      :param text: Text to search, In windows can also be the automation_id
+ |      :param control_type: Filter by control type
+ |      :return: An iterable containing dicts of matching objects properties
+ |  
+ |  get_object_position_by_text(self, text)
+ |      Return position as tuple (xl, yt, xr, yb) in windows / (x, y) in mac
+```
```

### Comparing `pybenutils-3.1.0/deployment_checklist.md` & `pybenutils-3.2.2/deployment_checklist.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-### Deployment check list
-- Install deployment requirements
-  - > python -m pip install -r deploy_requirements.txt -U
-- Test the package
-  - > pytest .
-  - > pytest . --pep8
-- Build the package
-  - > python setup.py sdist
-- README.md description test
- - > twine check dist/*
-- Deploy to repo (testpypi)
-  - > python -m twine upload --repository testpypi dist/*
-- Test installation
-  - > python -m pip install --index-url https://test.pypi.org/simple/ pybenutils -U
-- Deploy to repo (pypi)
-  - > python -m twine upload --repository pypi dist/*
+### Deployment check list
+- Install deployment requirements
+  - > python -m pip install -r deploy_requirements.txt -U
+- Test the package
+  - > pytest .
+  - > pytest . --pep8
+- Build the package
+  - > python setup.py sdist
+- README.md description test
+ - > twine check dist/*
+- Deploy to repo (testpypi)
+  - > python -m twine upload --repository testpypi dist/*
+- Test installation
+  - > python -m pip install --index-url https://test.pypi.org/simple/ pybenutils -U
+- Deploy to repo (pypi)
+  - > python -m twine upload --repository pypi dist/*
```

### Comparing `pybenutils-3.1.0/pybenutils/amazon_boto3/amazon_obj.py` & `pybenutils-3.2.2/pybenutils/amazon_boto3/amazon_obj.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import boto3
-import datetime
-from pybenutils.utils_logger.config_logger import get_logger
-
-logger = get_logger()
-
-
-class AmazonEC2Obj:
-    def __init__(self, aws_access_key_id, aws_secret_access_key, region_name, dalek_mode=False):
-        """Amazon EC2 Object declaration
-
-        :param aws_access_key_id: AWS access key id
-        :param aws_secret_access_key: AWS secret access key
-        :param region_name: AWS region to connect too
-        :param dalek_mode: Debug mode (dr who reference)
-        """
-        self.ec2 = boto3.client('ec2',
-                                region_name=region_name,
-                                aws_access_key_id=aws_access_key_id,
-                                aws_secret_access_key=aws_secret_access_key
-                                )
-        self.dalek_mode = dalek_mode
-        if self.dalek_mode:
-            logger.debug('EC2 is connected, I demand orders!')
-
-    def get_instances(self, search_filter_dict):
-        """Returns an ec2 collection object containing all the ec2 instances matching the search dict
-
-        :param search_filter_dict: Dict of key:[value] to filter the ec2 instances search
-        :return: Ec2 instances collection obj
-        """
-        filters_list = [{'Name': key, 'Values': value} for key, value in search_filter_dict.items()]
-        if self.dalek_mode:
-            logger.debug('Filtering by: {filter}'.format(filter=filters_list))
-        response = self.ec2.describe_instances(Filters=filters_list)
-        instances_list = []
-        for reservation in (response["Reservations"]):
-            instances_list += reservation["Instances"]
-        return instances_list
-
-    def terminate_instances_by_id(self, instances_ids_list):
-        """Terminates an instance by ID list
-
-        :param instances_ids_list: An EC2 instances id list
-        :return: True if successful
-        """
-        returned_result_dict = {'success': True, 'terminated_instances_ids': [], 'error_ids': []}
-        remained_instances_ids_to_terminate = instances_ids_list
-        try:
-            terminated_instances_dict = self.ec2.terminate_instances(InstanceIds=remained_instances_ids_to_terminate)
-
-            terminated_instances_ids = [x['InstanceId'] for x in terminated_instances_dict['TerminatingInstances']]
-            print('Following instances ids were terminated: {inst_ids}'.format(inst_ids=terminated_instances_ids))
-            if terminated_instances_ids:
-                returned_result_dict['terminated_instances_ids'].extend(terminated_instances_ids)
-
-            remained_instances_ids_to_terminate = [n for n in remained_instances_ids_to_terminate
-                                                   if n not in terminated_instances_ids]
-            if remained_instances_ids_to_terminate:
-                raise Exception('Following instances Ids failed to be terminated: "{inst_ids}"'.
-                                format(inst_ids=remained_instances_ids_to_terminate))
-        except Exception as e:
-            print(str(e))
-            print('Exception while trying terminated list of instances ids. Will try terminated one by one')
-
-            for instance_id in remained_instances_ids_to_terminate:
-                try:
-                    terminated_instances_dict = self.ec2.terminate_instances(
-                        InstanceIds=[instance_id])
-                    terminated_instances_ids = [x['InstanceId'] for x in
-                                                terminated_instances_dict['TerminatingInstances']]
-                    print('instance id "{inst_id}" terminated'.format(inst_id=terminated_instances_ids))
-
-                    returned_result_dict['terminated_instances_ids'].append(instance_id)
-                except Exception as e:
-                    returned_result_dict['success'] = False
-                    print('Exception while trying to terminate instance id: "{inst_id}. Exception is: "{exp}"'.format(
-                        inst_id=instance_id, exp=str(e)))
-                    returned_result_dict['error_ids'].append({'id': instance_id, 'error': str(e)})
-
-        return returned_result_dict
-
-    def terminate_instance_by_name(self, instance_name):
-        """Terminates an instance by it's Name tag
-
-        :param instance_name:
-        :return: True if successful
-        """
-        if not instance_name:
-            logger.error('ABORTING: I do not permit the deletion of an empty Name tag search')
-            return False
-        id_list = self.get_instance_ids_by_name(instance_name)
-        if id_list:
-            self.terminate_instances_by_id(id_list)
-        else:
-            logger.error('ABORTING: The id list for the given name is empty')
-            if self.dalek_mode:
-                logger.debug('EXPLAIN! EXPLAIN!')
-            return False
-        return True
-
-    def terminate_old_instances(self, minutes_to_keep_instances=1440, terminate_running_instances=False,
-                                excluded_tags=None):
-        """Search and terminate "stopped" instances that are older than the given int in seconds
-
-        :param minutes_to_keep_instances: The number (int) of minutes to keep an instance
-        :param terminate_running_instances: True: running & stopped instances. False: only stopped instances.
-        :param excluded_tags: List of excluded tags. Any machine tagged with one of these tags will not be terminated.
-        :return: True if successful
-        """
-        instances_state_filter = ['stopped', 'running'] if terminate_running_instances else ['stopped']
-        search_filter_dict = {'instance-state-name': instances_state_filter}
-        instances_list = self.get_instances(search_filter_dict)
-
-        uid_list_for_deletion = []
-        script_time = datetime.datetime.utcnow()
-        seconds_to_keep_instances = minutes_to_keep_instances * 60
-        for instance in instances_list:
-            if excluded_tags and any(
-                    item in excluded_tags for item in [tag['Key'] for tag in instance.get('Tags', [])]):
-                continue
-            time_diff = script_time - instance['LaunchTime'].replace(tzinfo=None)
-            time_diff_in_seconds = time_diff.days * 86400 + time_diff.seconds
-            if time_diff_in_seconds >= seconds_to_keep_instances and not self.verify_termination_protection(
-                    instance['InstanceId']):
-                uid_list_for_deletion.append(instance['InstanceId'])
-        return self.terminate_instances_by_id(instances_ids_list=uid_list_for_deletion)
-
-    def get_instance_ids_by_name(self, instance_name):
-        """Get instances id list by an instance Name tag
-
-        :param instance_name: An instance Name tag value to search
-        :return: Instances id list
-        """
-        search_filter_dict = {'tag:Name': [instance_name]}
-        instances_list = self.get_instances(search_filter_dict)
-        instance_id_list = []
-        for instance in instances_list:
-            instance_id_list.append(instance['InstanceId'])
-            logger.debug('ID:{id}, Name:{name}'.format(id=instance['InstanceId'], name=instance_name))
-        return instance_id_list
-
-    def verify_termination_protection(self, instance_id):
-        """Returns the termination protection attribute value
-
-        :param instance_id: The instance id
-        :return: Termination protection value
-        """
-        attribute_dict = self.ec2.describe_instance_attribute(Attribute='disableApiTermination', InstanceId=instance_id)
-        return attribute_dict['DisableApiTermination']['Value']
+import boto3
+import datetime
+from pybenutils.utils_logger.config_logger import get_logger
+
+logger = get_logger()
+
+
+class AmazonEC2Obj:
+    def __init__(self, aws_access_key_id, aws_secret_access_key, region_name, dalek_mode=False):
+        """Amazon EC2 Object declaration
+
+        :param aws_access_key_id: AWS access key id
+        :param aws_secret_access_key: AWS secret access key
+        :param region_name: AWS region to connect to
+        :param dalek_mode: Debug mode (dr who reference)
+        """
+        self.ec2 = boto3.client('ec2',
+                                region_name=region_name,
+                                aws_access_key_id=aws_access_key_id,
+                                aws_secret_access_key=aws_secret_access_key
+                                )
+        self.dalek_mode = dalek_mode
+        if self.dalek_mode:
+            logger.debug('EC2 is connected, I demand orders!')
+
+    def get_instances(self, search_filter_dict):
+        """Returns an ec2 collection object containing all the ec2 instances matching the search dict
+
+        :param search_filter_dict: Dict of key:[value] to filter the ec2 instances search
+        :return: Ec2 instances collection obj
+        """
+        filters_list = [{'Name': key, 'Values': value} for key, value in search_filter_dict.items()]
+        if self.dalek_mode:
+            logger.debug('Filtering by: {filter}'.format(filter=filters_list))
+        response = self.ec2.describe_instances(Filters=filters_list)
+        instances_list = []
+        for reservation in (response["Reservations"]):
+            instances_list += reservation["Instances"]
+        return instances_list
+
+    def terminate_instances_by_id(self, instances_ids_list):
+        """Terminates an instance by ID list
+
+        :param instances_ids_list: An EC2 instances id list
+        :return: True if successful
+        """
+        returned_result_dict = {'success': True, 'terminated_instances_ids': [], 'error_ids': []}
+        remained_instances_ids_to_terminate = instances_ids_list
+        try:
+            terminated_instances_dict = self.ec2.terminate_instances(InstanceIds=remained_instances_ids_to_terminate)
+
+            terminated_instances_ids = [x['InstanceId'] for x in terminated_instances_dict['TerminatingInstances']]
+            print('Following instances ids were terminated: {inst_ids}'.format(inst_ids=terminated_instances_ids))
+            if terminated_instances_ids:
+                returned_result_dict['terminated_instances_ids'].extend(terminated_instances_ids)
+
+            remained_instances_ids_to_terminate = [n for n in remained_instances_ids_to_terminate
+                                                   if n not in terminated_instances_ids]
+            if remained_instances_ids_to_terminate:
+                raise Exception('Following instances Ids failed to be terminated: "{inst_ids}"'.
+                                format(inst_ids=remained_instances_ids_to_terminate))
+        except Exception as e:
+            print(str(e))
+            print('Exception while trying terminated list of instances ids. Will try terminated one by one')
+
+            for instance_id in remained_instances_ids_to_terminate:
+                try:
+                    terminated_instances_dict = self.ec2.terminate_instances(
+                        InstanceIds=[instance_id])
+                    terminated_instances_ids = [x['InstanceId'] for x in
+                                                terminated_instances_dict['TerminatingInstances']]
+                    print('instance id "{inst_id}" terminated'.format(inst_id=terminated_instances_ids))
+
+                    returned_result_dict['terminated_instances_ids'].append(instance_id)
+                except Exception as e:
+                    returned_result_dict['success'] = False
+                    print('Exception while trying to terminate instance id: "{inst_id}. Exception is: "{exp}"'.format(
+                        inst_id=instance_id, exp=str(e)))
+                    returned_result_dict['error_ids'].append({'id': instance_id, 'error': str(e)})
+
+        return returned_result_dict
+
+    def terminate_instance_by_name(self, instance_name):
+        """Terminates an instance by it's Name tag
+
+        :param instance_name:
+        :return: True if successful
+        """
+        if not instance_name:
+            logger.error('ABORTING: I do not permit the deletion of an empty Name tag search')
+            return False
+        id_list = self.get_instance_ids_by_name(instance_name)
+        if id_list:
+            self.terminate_instances_by_id(id_list)
+        else:
+            logger.error('ABORTING: The id list for the given name is empty')
+            if self.dalek_mode:
+                logger.debug('EXPLAIN! EXPLAIN!')
+            return False
+        return True
+
+    def terminate_old_instances(self, minutes_to_keep_instances=1440, terminate_running_instances=False,
+                                excluded_tags=None):
+        """Search and terminate "stopped" instances that are older than the given int in seconds
+
+        :param minutes_to_keep_instances: The number (int) of minutes to keep an instance
+        :param terminate_running_instances: True: running & stopped instances. False: only stopped instances.
+        :param excluded_tags: List of excluded tags. Any machine tagged with one of these tags will not be terminated.
+        :return: True if successful
+        """
+        instances_state_filter = ['stopped', 'running'] if terminate_running_instances else ['stopped']
+        search_filter_dict = {'instance-state-name': instances_state_filter}
+        instances_list = self.get_instances(search_filter_dict)
+
+        uid_list_for_deletion = []
+        script_time = datetime.datetime.utcnow()
+        seconds_to_keep_instances = minutes_to_keep_instances * 60
+        for instance in instances_list:
+            if excluded_tags and any(
+                    item in excluded_tags for item in [tag['Key'] for tag in instance.get('Tags', [])]):
+                continue
+            time_diff = script_time - instance['LaunchTime'].replace(tzinfo=None)
+            time_diff_in_seconds = time_diff.days * 86400 + time_diff.seconds
+            if time_diff_in_seconds >= seconds_to_keep_instances and not self.verify_termination_protection(
+                    instance['InstanceId']):
+                uid_list_for_deletion.append(instance['InstanceId'])
+        return self.terminate_instances_by_id(instances_ids_list=uid_list_for_deletion)
+
+    def get_instance_ids_by_name(self, instance_name):
+        """Get instances id list by an instance Name tag
+
+        :param instance_name: An instance Name tag value to search
+        :return: Instances id list
+        """
+        search_filter_dict = {'tag:Name': [instance_name]}
+        instances_list = self.get_instances(search_filter_dict)
+        instance_id_list = []
+        for instance in instances_list:
+            instance_id_list.append(instance['InstanceId'])
+            logger.debug('ID:{id}, Name:{name}'.format(id=instance['InstanceId'], name=instance_name))
+        return instance_id_list
+
+    def verify_termination_protection(self, instance_id):
+        """Returns the termination protection attribute value
+
+        :param instance_id: The instance id
+        :return: Termination protection value
+        """
+        attribute_dict = self.ec2.describe_instance_attribute(Attribute='disableApiTermination', InstanceId=instance_id)
+        return attribute_dict['DisableApiTermination']['Value']
```

### Comparing `pybenutils-3.1.0/pybenutils/autogui/__main__.py` & `pybenutils-3.2.2/pybenutils/autogui/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,34 @@
-import sys
-from pybenutils.autogui.auto_gui_cls import AutoGui
-import argparse
-
-print(sys.argv)
-parser = argparse.ArgumentParser(description='PyBenAutoGui - Class to automate cross platform GUI interactions.')
-parser.add_argument('-t', '--title', help='Window title')
-parser.add_argument('-a', '--app_path', help='Application/Exe path')
-parser.add_argument('-b', '--pywinauto_backend', default='uia', required=False,
-                    help='A name of used back-end in Windows OS (values: "win32", "uia")')
-parser.add_argument('-c', '--command', default='uia',
-                    help='Function name to execute in the AutoGui Class')
-args = parser.parse_known_args()
-title = args[0].title
-app_path = args[0].app_path
-pywinauto_backend = args[0].pywinauto_backend
-command = args[0].command
-parameters = args[1]
-command_function = getattr(AutoGui(title=title, app_path=app_path, pywinauto_backend=pywinauto_backend), command)
-if command_function:
-    print(command_function(*parameters))
+import sys
+import argparse
+
+from pybenutils.autogui.auto_gui_cls import AutoGui
+from pybenutils.useful import smart_cmd_input_eval
+
+print(sys.argv)
+parser = argparse.ArgumentParser(description='PyBenAutoGui - Class to automate cross platform GUI interactions.')
+parser.add_argument('-t', '--title', help='Window title')
+parser.add_argument('-a', '--app_path', help='Application/Exe path')
+parser.add_argument('-b', '--pywinauto_backend', default='uia', required=False,
+                    help='A name of used back-end in Windows OS (values: "win32", "uia")')
+parser.add_argument('-c', '--command', help='Function name to execute in the AutoGui Class')
+parser.add_argument('-eh', '--extra_help', help='Display extra help about the class and its functions', required=False,
+                    default=False, action=argparse.BooleanOptionalAction)
+args = parser.parse_known_args()
+title = args[0].title
+app_path = args[0].app_path
+pywinauto_backend = args[0].pywinauto_backend
+command = args[0].command
+parameters = args[1]
+extra_help = args[0].extra_help
+
+if extra_help:
+    if command:
+        help(getattr(AutoGui, command))
+    else:
+        help(AutoGui)
+    exit(0)
+
+command_function = getattr(AutoGui(title=title, app_path=app_path, pywinauto_backend=pywinauto_backend), command)
+if command_function:
+    parameters, parameters_dict = smart_cmd_input_eval(parameters)
+    print(command_function(*parameters, **parameters_dict))
```

### Comparing `pybenutils-3.1.0/pybenutils/autogui/auto_gui_cls.py` & `pybenutils-3.2.2/pybenutils/autogui/auto_gui_cls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,126 +1,131 @@
-import re
-import pyautogui
-import sys
-from pybenutils.os_operations.mac_application_control import ApplicationControl
-from pybenutils.os_operations.mac_operations import run_apple_script
-from pybenutils.utils_logger.config_logger import get_logger
-if sys.platform == 'win32':
-    from pywinauto import application
-    from pywinauto.timings import TimeoutError as pywinautoTimeoutError
-
-logger = get_logger()
-
-
-class AutoGui:
-    def __init__(self, title, app_path, pywinauto_backend='uia'):
-        """Unified interface to interact with Gui Elements
-
-        :param title: Window title
-        :param app_path: Application/Exe path
-        :param pywinauto_backend: A name of used back-end in Windows OS (values: "win32", "uia")
-        """
-        self.title = title
-        self.app_path = app_path
-        if sys.platform == 'win32':
-            self.app = application.Application(backend=pywinauto_backend)
-            try:
-                self.app.connect(title=self.title, timeout=10)
-            except pywinautoTimeoutError:
-                logger.debug('Failed to connect to a live window. Will start a new instance')
-                self.app.start(self.app_path)
-            self.main_window = self.app.window(title=self.title)
-        elif sys.platform == 'darwin':
-            self.app = ApplicationControl(self.app_path)
-            self.app.application_process_name = self.title
-        else:
-            raise Exception('Method not implemented for this OS')
-        self.elements = self.find_objects()
-
-    def click_on_text(self, text: str):
-        """Clicks on text object location using pyautogui"""
-        cord = self.get_object_position_by_text(text)
-        self.focus_on_window()
-        pyautogui.FAILSAFE = False
-        pyautogui.click(cord[0] + 5, cord[1] + 5)
-
-    def find_objects(self, text='', control_type=''):
-        """Returns an iterable containing the matching object
-
-        :param text: Text to search, In windows can also be the automation_id
-        :param control_type: Filter by control type
-        :return: An iterable containing the matching object
-        """
-        if sys.platform == 'win32':
-            elements = []
-            if not text:
-                elements = self.main_window.descendants()
-            for element in self.main_window.descendants():
-                if text == element.element_info.name:
-                    elements.append(element)
-                elif re.search(rf'.*{text}.*', element.element_info.automation_id):
-                    elements.append(element)
-            if control_type:
-                return [i for i in elements if i.element_info.control_type.lower() == control_type.lower()]
-            return elements
-
-        elif sys.platform == 'darwin':
-            elements = self.app.get_elements_in_view()
-            if not text:
-                return elements
-            return [element for element in elements if text == element.__dict__()['value']]
-
-        else:
-            raise Exception('Method not implemented for this OS')
-
-    def get_object_details(self, text='', control_type=''):
-        """Returns an iterable containing dicts of matching objects properties
-
-        :param text: Text to search, In windows can also be the automation_id
-        :param control_type: Filter by control type
-        :return: An iterable containing dicts of matching objects properties
-        """
-        if sys.platform == 'win32':
-            elements = []
-            for element in self.find_objects(text, control_type):
-                element_info_dict = element.element_info.dump_window()
-                for element_info in dir(element.element_info):
-                    if not element_info.startswith('_'):
-                        try:
-                            element_info_dict[element_info] = getattr(element.element_info, element_info)
-                        except Exception:
-                            pass
-                elements.append(element_info_dict)
-            return elements
-        elif sys.platform == 'darwin':
-            elements = []
-            for element in self.find_objects(text, control_type):
-                elements.append(element.__dict__())
-            return elements
-        else:
-            raise Exception('Method not implemented for this OS')
-
-    def get_object_position_by_text(self, text):
-        """Return position as tuple (xl, yt, xr, yb) in windows / (x, y) in mac"""
-        if sys.platform == 'win32':
-            pos = self.get_object_details(text)[0]['rectangle']
-            return pos.left, pos.top, pos.right, pos.bottom
-        elif sys.platform == 'darwin':
-            return self.app.get_text_position(text)
-        else:
-            raise Exception('Method not implemented for this OS')
-
-    def focus_on_window(self):
-        """Focus on the app window - bring to front"""
-        if sys.platform == 'win32':
-            self.main_window.set_focus()
-        elif sys.platform == 'darwin':
-            script = f"""
-                tell application "System Events"
-                    tell (application process "{self.title}")
-                        set frontmost to true
-                    end tell
-                end tell
-                """
-            run_apple_script(script)
-        else:
-            raise Exception('Method not implemented for this OS')
+import re
+import pyautogui
+import sys
+from pybenutils.os_operations.mac_application_control import ApplicationControl
+from pybenutils.os_operations.mac_operations import run_apple_script
+from pybenutils.utils_logger.config_logger import get_logger
+if sys.platform == 'win32':
+    from pywinauto import application
+    from pywinauto.timings import TimeoutError as pywinautoTimeoutError
+
+logger = get_logger()
+
+
+class AutoGui:
+    def __init__(self, title, app_path, pywinauto_backend='uia'):
+        """Unified interface to interact with Gui Elements
+
+        :param title: Window title
+        :param app_path: Application/Exe path
+        :param pywinauto_backend: A name of used back-end in Windows OS (values: "win32", "uia")
+        """
+        self.title = title
+        self.app_path = app_path
+        assert title or app_path, 'Please provide a title or application path to connect to.\n' \
+                                  '\n----------\n' \
+                                  'Run "python(3) -m pybenutils.autogui -h" for more information.\n' \
+                                  'Run "python(3) -m pybenutils.autogui -eh" for even more information' \
+                                  '\n----------\n'
+        if sys.platform == 'win32':
+            self.app = application.Application(backend=pywinauto_backend)
+            try:
+                self.app.connect(title=self.title, timeout=10)
+            except pywinautoTimeoutError:
+                logger.debug('Failed to connect to a live window. Will start a new instance')
+                self.app.start(self.app_path)
+            self.main_window = self.app.window(title=self.title)
+        elif sys.platform == 'darwin':
+            self.app = ApplicationControl(self.app_path)
+            self.app.application_process_name = self.title
+        else:
+            raise Exception('Method not implemented for this OS')
+        self.elements = self.find_objects()
+
+    def click_on_text(self, text: str):
+        """Clicks on text object location using pyautogui"""
+        cord = self.get_object_position_by_text(text)
+        self.focus_on_window()
+        pyautogui.FAILSAFE = False
+        pyautogui.click(cord[0] + 5, cord[1] + 5)
+
+    def find_objects(self, text='', control_type=''):
+        """Returns an iterable containing the matching object
+
+        :param text: Text to search, In windows can also be the automation_id
+        :param control_type: Filter by control type
+        :return: An iterable containing the matching object
+        """
+        if sys.platform == 'win32':
+            elements = []
+            if not text:
+                elements = self.main_window.descendants()
+            for element in self.main_window.descendants():
+                if text == element.element_info.name:
+                    elements.append(element)
+                elif re.search(rf'.*{text}.*', element.element_info.automation_id):
+                    elements.append(element)
+            if control_type:
+                return [i for i in elements if i.element_info.control_type.lower() == control_type.lower()]
+            return elements
+
+        elif sys.platform == 'darwin':
+            elements = self.app.get_elements_in_view()
+            if not text:
+                return elements
+            return [element for element in elements if text == element.__dict__()['value']]
+
+        else:
+            raise Exception('Method not implemented for this OS')
+
+    def get_object_details(self, text='', control_type=''):
+        """Returns an iterable containing dicts of matching objects properties
+
+        :param text: Text to search, In windows can also be the automation_id
+        :param control_type: Filter by control type
+        :return: An iterable containing dicts of matching objects properties
+        """
+        if sys.platform == 'win32':
+            elements = []
+            for element in self.find_objects(text, control_type):
+                element_info_dict = element.element_info.dump_window()
+                for element_info in dir(element.element_info):
+                    if not element_info.startswith('_'):
+                        try:
+                            element_info_dict[element_info] = getattr(element.element_info, element_info)
+                        except Exception:
+                            pass
+                elements.append(element_info_dict)
+            return elements
+        elif sys.platform == 'darwin':
+            elements = []
+            for element in self.find_objects(text, control_type):
+                elements.append(element.__dict__())
+            return elements
+        else:
+            raise Exception('Method not implemented for this OS')
+
+    def get_object_position_by_text(self, text):
+        """Return position as tuple (xl, yt, xr, yb) in windows / (x, y) in mac"""
+        if sys.platform == 'win32':
+            pos = self.get_object_details(text)[0]['rectangle']
+            return pos.left, pos.top, pos.right, pos.bottom
+        elif sys.platform == 'darwin':
+            return self.app.get_text_position(text)
+        else:
+            raise Exception('Method not implemented for this OS')
+
+    def focus_on_window(self):
+        """Focus on the app window - bring to front"""
+        if sys.platform == 'win32':
+            self.main_window.set_focus()
+        elif sys.platform == 'darwin':
+            script = f"""
+                tell application "System Events"
+                    tell (application process "{self.title}")
+                        set frontmost to true
+                    end tell
+                end tell
+                """
+            run_apple_script(script)
+        else:
+            raise Exception('Method not implemented for this OS')
```

### Comparing `pybenutils-3.1.0/pybenutils/browsers/chrome.py` & `pybenutils-3.2.2/pybenutils/browsers/chrome.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import os
-import subprocess
-import sys
-from subprocess import Popen
-from pybenutils.network.download_manager import download_url
-from pybenutils.utils_logger.config_logger import get_logger
-
-logger = get_logger()
-
-
-def update_chrome_browser():
-    """Updating Chrome browser to its latest version. Returns True if successful, Raise exception on fail"""
-    if sys.platform == 'win32':
-        logger.info('Downloading chrome standalone 64 bit version')
-        download_url('https://dl.google.com/tag/s/appguid%3D%7B8A69D345-D564-463C-AFF1-A69D9E530F96%7D%26iid%3'
-                     'D%7B2FBBE98E-4188-4D38-EB51-8DC406611FB1%7D%26lang%3Den%26browser%3D3%26usagestats%3D0%2'
-                     '6appname%3DGoogle%2520Chrome%26needsadmin%3Dprefers%26ap%3Dx64-stable-statsdef_1%26insta'
-                     'lldataindex%3Dempty/chrome/install/ChromeStandaloneSetup64.exe')
-
-        process = Popen(f'"{os.path.realpath("ChromeStandaloneSetup64.exe")}" /silent /install', shell=True)
-        process.communicate()
-        logger.info('Chrome installer finished')
-    else:
-        download_url('https://dl.google.com/dl/chrome/mac/universal/stable/gcea/googlechrome.dmg')
-
-        cmd = r'hdiutil attach googlechrome.dmg ' \
-              r'&& rm -R /Applications/Google Chrome.app ' \
-              r'&& cp -pPR "/Volumes/Google Chrome/Google Chrome.app" /Applications/'
-        p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE)
-        p.communicate()
-    return True
+import os
+import subprocess
+import sys
+from subprocess import Popen
+from pybenutils.network.download_manager import download_url
+from pybenutils.utils_logger.config_logger import get_logger
+
+logger = get_logger()
+
+
+def update_chrome_browser():
+    """Updating Chrome browser to its latest version. Returns True if successful, Raise exception on fail"""
+    if sys.platform == 'win32':
+        logger.info('Downloading chrome standalone 64 bit version')
+        download_url('https://dl.google.com/tag/s/appguid%3D%7B8A69D345-D564-463C-AFF1-A69D9E530F96%7D%26iid%3'
+                     'D%7B2FBBE98E-4188-4D38-EB51-8DC406611FB1%7D%26lang%3Den%26browser%3D3%26usagestats%3D0%2'
+                     '6appname%3DGoogle%2520Chrome%26needsadmin%3Dprefers%26ap%3Dx64-stable-statsdef_1%26insta'
+                     'lldataindex%3Dempty/chrome/install/ChromeStandaloneSetup64.exe')
+
+        process = Popen(f'"{os.path.realpath("ChromeStandaloneSetup64.exe")}" /silent /install', shell=True)
+        process.communicate()
+        logger.info('Chrome installer finished')
+    else:
+        download_url('https://dl.google.com/dl/chrome/mac/universal/stable/gcea/googlechrome.dmg')
+
+        cmd = r'hdiutil attach googlechrome.dmg ' \
+              r'&& rm -R /Applications/Google Chrome.app ' \
+              r'&& cp -pPR "/Volumes/Google Chrome/Google Chrome.app" /Applications/'
+        p = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, stdin=subprocess.PIPE)
+        p.communicate()
+    return True
```

### Comparing `pybenutils-3.1.0/pybenutils/browsers/selenium_utils.py` & `pybenutils-3.2.2/pybenutils/browsers/selenium_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,482 +1,520 @@
-import os
-import re
-import sys
-import time
-import zipfile
-import tarfile
-import platform
-import logging
-import requests
-from getpass import getuser
-from selenium.webdriver import ActionChains
-from selenium.webdriver.common.keys import Keys
-from typing import List
-from selenium import webdriver
-from selenium.common.exceptions import WebDriverException, SessionNotCreatedException
-from selenium.webdriver.remote.remote_connection import LOGGER as SELENIUM_LOGGER
-from pybenutils.network.download_manager import download_url
-from pybenutils.utils_logger.config_logger import get_logger
-
-logger = get_logger()
-
-
-class DriverTools:
-    """Meant to be inherited by webdriver sub-classes to add general tools and tricks, can be used on all browsers"""
-    LOGGER_DEFAULT_LEVEL = 'DEBUG'
-
-    def __bool__(self):
-        """Returns True only if there are open browser windows / tabs"""
-        return bool(self.get_number_open_tabs())
-
-    # noinspection PyBroadException
-    def get_number_open_tabs(self):
-        """Returns the number of open browser windows and tabs"""
-        try:
-            return len(self.window_handles)
-        except Exception:
-            return 0
-
-    def is_site_displayed(self) -> bool:
-        """Returns True if the current page is displaying a web-page (page might not be fully loaded)"""
-        if not self:
-            return False
-        original_log_level = self.get_logs_levels().get('selenium', self.LOGGER_DEFAULT_LEVEL)
-        self.set_selenium_log_level('WARNING')
-        if 'about:blank' in str(self.current_url):
-            return False
-        body = self.find_element_by_tag_name('body')
-        content = body.text
-        self.set_selenium_log_level(original_log_level)
-        return not [i for i in ['This site can’t be reached',
-                                'Requests to the server have been blocked by an extension',
-                                '404. That’s an error.\nThe requested URL was not found on this server.'] if
-                    i in content]
-
-    @staticmethod
-    def set_selenium_log_level(log_level: str):
-        """Sets the log level of selenium and urllib3
-
-        :param log_level: log level (CRITICAL / FATAL / ERROR / WARNING / INFO / DEBUG / NOTSET)
-        """
-        SELENIUM_LOGGER.setLevel(vars(logging)[log_level.upper()])
-        logging.getLogger("urllib3").setLevel(vars(logging)[log_level.upper()])
-
-    @staticmethod
-    def get_logs_levels():
-        """Returns a dict of the current log levels.
-
-        {'selenium': selenium_log_level, 'urllib3': urllib3_log_level, 'main_logger': utils_log_level}
-        """
-        selenium_log_level = logging._levelToName.get(SELENIUM_LOGGER.getEffectiveLevel())
-        urllib3_log_level = logging._levelToName.get(logging.getLogger("urllib3").getEffectiveLevel())
-        utils_log_level = logging._levelToName.get(logger.getEffectiveLevel())
-        return {'selenium': selenium_log_level,
-                'urllib3': urllib3_log_level,
-                'main_logger': utils_log_level}
-
-    def gracefully_quit(self):
-        """Closing the chrome web driver window, than quitting the webdriver
-              - Support for missing Chrome window
-              - Support for missing driver object
-        """
-        if self:
-            logger.debug('Closing driver')
-            try:
-                self.close()
-            except WebDriverException:
-                logger.error('The chrome browser window was closed unexpectedly')
-            self.quit()
-
-    def switch_to_first_tab(self):
-        """Switches to control the first tab or window opened"""
-        self._switch_to.window(self.window_handles[0])
-
-    def switch_to_last_tab(self):
-        """Switches to control the last tab or window opened"""
-        self._switch_to.window(self.window_handles[-1])
-
-    def close_secondary_tabs(self):
-        """Closes all tabs except the first one in the webdriver window"""
-        while len(self.window_handles) > 1:
-            self.switch_to_last_tab()
-            self.close()
-        self.switch_to_first_tab()
-
-    def open_new_tab(self, url=''):
-        """Attempting to open a new tab with the given URL.
-
-        :param url: URL to open in a new tab. Leave empty for new tab with about:blank
-        """
-        self.execute_script(f'window.open("{url}")')
-
-    def open_and_navigate_to_a_new_tab(self):
-        """Opens a new tab, switched to it and navigates to the new tab address"""
-        self.open_new_tab()
-        self.switch_to_last_tab()
-        self.get(self.NEW_TAB_ADDRESS)
-
-    def is_scrollbar_exist(self):
-        """Returns True if the current web page main window has a vertical scrollbar (Not checking inner elements)"""
-        return self.execute_script(
-            'return document.documentElement.scrollHeight > document.documentElement.clientHeight;')
-
-    def is_element_visible_in_viewpoint(self, element) -> bool:
-        """Return True if the given element is showing the user view point (can be seen on the screen)"""
-        # Calculates the elements position relative position against the user current point of view (see on screen)
-        # Element.is_visible() will return True even if the element is not currently in the user view point
-        return self.execute_script("var elem = arguments[0],                 "
-                                   "  box = elem.getBoundingClientRect(),    "
-                                   "  cx = box.left + box.width / 2,         "
-                                   "  cy = box.top + box.height / 2,         "
-                                   "  e = document.elementFromPoint(cx, cy); "
-                                   "for (; e; e = e.parentElement) {         "
-                                   "  if (e === elem)                        "
-                                   "    return true;                         "
-                                   "}                                        "
-                                   "return false;                            "
-                                   , element)
-
-
-class ChromeDriver(webdriver.Chrome, DriverTools):
-    chrome_default_profile_path = None
-    NEW_TAB_ADDRESS = 'chrome://newtab'
-
-    def __init__(self, *args, **kwargs):
-        """
-        Creates a new instance of the chrome driver.
-        Starts the service and then creates new instance of chrome driver.
-
-         - default_user - [Boolean] Use the default Chrome user installed on the OS (user-data-dir)
-         - fullscreen - [Boolean] Open window at fullscreen (--start-maximized)
-         - excludeSwitches - [List] of switches to exclude (options.add_experimental_option("excludeSwitches", [x]))
-         - crx_path - [Str] Open with extension pre-installed (options.add_extension)
-         - option_args - [List] of arguments to be added to options (options.add_argument(x))
-         - log_level - [Str] Selenium and urllib3 log level (CRITICAL / FATAL / ERROR / WARNING / INFO / DEBUG / NOTSET)
-         - launch_attempts - [int] Permitted number of attempts to launch the selenium web driver
-         - headless - [Boolean] Open the Chrome instance without visible gui (--headless)
-        ----------
-         - executable_path - path to the executable. If the default is used it assumes the executable is in the $PATH
-         - port - port you would like the service to run, if left as 0, a free port will be found.
-         - options - this takes an instance of ChromeOptions
-         - service_args - List of args to pass to the driver service
-         - desired_capabilities - Dictionary object with non-browser specific
-           capabilities only, such as "proxy" or "loggingPref".
-         - service_log_path - Where to log information from the driver.
-         - chrome_options - Deprecated argument for options
-         - keep_alive - Whether to configure ChromeRemoteConnection to use HTTP keep-alive.
-        """
-        self.launch_attempts = kwargs.pop('launch_attempts', 2)
-        self._platform_release = platform.release()
-
-        if kwargs.get('log_level'):
-            self.set_selenium_log_level(kwargs.pop('log_level', self.LOGGER_DEFAULT_LEVEL))
-
-        self.__init_options_object(args, kwargs)
-
-        logger.info('Launching Chrome webdriver')
-        last_exception = None
-        for i in range(self.launch_attempts):
-            try:
-                super().__init__(
-                    *args,
-                    **{'desired_capabilities' if self._platform_release == 'XP' else 'options': self.options},
-                    **kwargs
-                )
-                break
-            except WebDriverException as ex:
-                logger.error(ex)
-                last_exception = ex
-                if type(ex) == SessionNotCreatedException or "executable needs to be in PATH" in str(ex):
-                    self.update()
-            except Exception as ex:
-                logger.error(ex)
-                last_exception = ex
-        else:
-            raise last_exception
-        logger.info('Chrome webdriver launched successfully')
-
-    def __init_options_object(self, args, kwargs):
-        """Handles the creation of Chrome options object"""
-        if self._platform_release == 'XP':
-            self.options = kwargs.pop('options', {"chromeOptions": {
-                "args": [self.get_chrome_profile_path()],
-                "excludeSwitches": ["disable-default-apps", "restore-last-session", "disable-web-resources"]}})
-
-            if kwargs.pop('default_user', False):
-                self.options['chromeOptions']['args'] = [self.get_chrome_profile_path()]
-
-        else:
-            self.options = kwargs.pop('options', webdriver.ChromeOptions())
-            if kwargs.pop('fullscreen', False):
-                self.options.add_argument('--start-maximized')
-
-            if kwargs.pop('headless', False):
-                self.options.add_argument('--headless')
-
-            if kwargs.pop('default_user', False):
-                self.options.add_argument(f"user-data-dir={self.get_chrome_profile_path()}")
-
-            if kwargs.get('excludeSwitches'):
-                switches_to_exclude = kwargs.pop('excludeSwitches', [])
-                self.options.add_experimental_option("excludeSwitches", switches_to_exclude)
-
-            if kwargs.get('crx_path'):
-                self.options.add_extension(kwargs.pop('crx_path', ''))
-
-            for arg in kwargs.pop('option_args', []):
-                self.options.add_argument(arg)
-        return self.options
-
-    def get_chrome_profile_path(self) -> str:
-        """Returns the chrome default profile path"""
-        if not self.chrome_default_profile_path:
-            local_user_name = getuser()
-            if sys.platform != 'win32':  # mac
-                path = f'/Users/{local_user_name}/Library/Application Support/Google/Chrome/'
-            elif self._platform_release == 'XP':  # Winxp path
-                path = r'C:\Documents and Settings\automation\Local Settings\Application Data\Google\Chrome\User Data'
-            else:  # Win OS newer than xp
-                path = f'C:\\Users\\{local_user_name}\\AppData\\Local\\Google\\Chrome\\User Data'
-            self.chrome_default_profile_path = path
-        return self.chrome_default_profile_path
-
-    @staticmethod
-    def update(web_drivers_folder_path=''):
-        """Downloads the latest chrome webdriver
-
-        :param web_drivers_folder_path: Leave empty to download_url to the workspace
-        :return: True if downloaded successfully
-        """
-        # Handling output folder for the new webdriver file
-        if not web_drivers_folder_path:
-            web_drivers_folder_path = os.getcwd()
-        if not os.path.isdir(web_drivers_folder_path):
-            logger.error('The folder you are trying to download_url to does not exist. '
-                         'Please create it and add it to the system path to be recognised correctly')
-            return False
-
-        # Sorting which file to download_url depending on the OS
-        if sys.platform == 'win32':
-            web_driver_zip_file_name = 'chromedriver_win32.zip'
-        elif sys.platform == 'darwin':
-            web_driver_zip_file_name = 'chromedriver_mac64.zip'
-        else:
-            web_driver_zip_file_name = 'chromedriver_linux64.zip'
-
-        logger.info('Getting chrome driver latest stable version number from api')
-        for i in range(3):
-            try:
-                response = requests.get('http://chromedriver.storage.googleapis.com/LATEST_RELEASE')
-                if response.status_code < 400:
-                    latest_version = response.content.decode()
-                    break
-                else:
-                    logger.warning(f'Response status code: {response.status_code}')
-            except Exception as ex:
-                logger.error(ex)
-        else:
-            return False
-
-        logger.info(f'Downloading chrome driver version: {latest_version}')
-        download_url(f'http://chromedriver.storage.googleapis.com/{latest_version}/{web_driver_zip_file_name}')
-
-        logger.info(f'Extracting {web_driver_zip_file_name} to {web_drivers_folder_path}')
-        with zipfile.ZipFile(web_driver_zip_file_name, 'r') as zip_ref:
-            zip_ref.extractall(web_drivers_folder_path)
-
-        logger.info('Webdriver deployed successfully')
-        return True
-
-
-class FirefoxDriver(webdriver.Firefox, DriverTools):
-    NEW_TAB_ADDRESS = 'about:newtab'
-
-    def __init__(self, *args, **kwargs):
-        """Starts a new local session of Firefox.
-
-        Based on the combination and specificity of the various keyword arguments,
-        a capabilities dictionary will be constructed that is passed to the remote end.
-
-        The keyword arguments given to this constructor are helpers to more easily allow Firefox WebDriver sessions
-        to be customised with different options.  They are mapped on to a capabilities dictionary that is passed on
-        to the remote end.
-
-        As some of the options, such as `firefox_profile` and `options.profile` are mutually exclusive,
-        precedence is given from how specific the setting is.  `capabilities` is the least specific keyword argument,
-        followed by `options`, followed by `firefox_binary` and `firefox_profile`.
-
-        In practice this means that if `firefox_profile` and `options.profile` are both set,
-        the selected profile instance will always come from the most specific variable.
-        In this case that would be `firefox_profile`.  This will result in `options.profile` to be ignored because it
-        is considered a less specific setting than the top-level `firefox_profile` keyword argument.
-        Similarly, if you had specified a `capabilities["moz:firefoxOptions"]["profile"]` Base64 string,
-        this would rank below `options.profile`.
-
-         - option_args - [List] of arguments to be added to options (options.add_argument(x))
-         - log_level - [Str] Selenium and urllib3 log level (CRITICAL / FATAL / ERROR / WARNING / INFO / DEBUG / NOTSET)
-         - launch_attempts - [int] Permitted number of attempts to launch the selenium web driver
-        -----------
-         - firefox_profile - Instance of ``FirefoxProfile`` object or a string.
-           If undefined, a fresh profile will be created in a temporary location on the system.
-         - firefox_binary - Instance of ``FirefoxBinary`` or full path to the Firefox binary.
-           If undefined, the system default Firefox installation will  be used.
-         - timeout - Time to wait for Firefox to launch when using the extension connection.
-         - capabilities - Dictionary of desired capabilities.
-         - proxy - The proxy settings to us when communicating with Firefox via the extension connection.
-         - executable_path - Full path to override which geckodriver binary to use for Firefox 47.0.1 and greater,
-           which defaults to picking up the binary from the system path.
-         - options - Instance of ``options.Options``.
-         - service_log_path - Where to log information from the driver.
-         - firefox_options - Deprecated argument for options
-         - service_args - List of args to pass to the driver service
-         - desired_capabilities - alias of capabilities. In future versions of this library,
-           this will replace 'capabilities'. This will make the signature consistent with RemoteWebDriver.
-         - log_path - Deprecated argument for service_log_path
-         - keep_alive - Whether to configure remote_connection.RemoteConnection to use HTTP keep-alive.
-        """
-        self.launch_attempts = kwargs.pop('launch_attempts', 2)
-        self._platform_release = platform.release()
-
-        if kwargs.get('log_level'):
-            self.set_selenium_log_level(kwargs.pop('log_level', self.LOGGER_DEFAULT_LEVEL))
-
-        self.options = kwargs.pop('options', webdriver.FirefoxOptions())
-
-        for arg in kwargs.pop('option_args', []):
-            self.options.add_argument(arg)
-
-        logger.info('Launching Chrome webdriver')
-        last_exception = None
-        for i in range(self.launch_attempts):
-            try:
-                super().__init__(
-                    *args,
-                    **{'desired_capabilities' if self._platform_release == 'XP' else 'options': self.options},
-                    **kwargs
-                )
-                break
-            except WebDriverException as ex:
-                logger.error(ex)
-                last_exception = ex
-                if type(ex) == SessionNotCreatedException or "executable needs to be in PATH" in str(ex):
-                    self.update()
-            except Exception as ex:
-                logger.error(ex)
-                last_exception = ex
-        else:
-            raise last_exception
-        logger.info('Firefox webdriver launched successfully')
-
-    @staticmethod
-    def update(web_drivers_folder_path=''):
-        """Downloads the latest gecko (firefox) webdriver
-
-        :param web_drivers_folder_path: Leave empty to download_url to the workspace
-        :return: True if downloaded successfully
-        """
-        if not web_drivers_folder_path:
-            web_drivers_folder_path = os.getcwd()
-        if not os.path.isdir(web_drivers_folder_path):
-            logger.error('The folder you are trying to download_url to does not exist. '
-                         'Please create it and add it to the system path to be recognised correctly')
-            return False
-
-        # Creating a list of archive files appearing in this page to get the latest webdriver archive file name.
-        response = requests.get('https://github.com/mozilla/geckodriver/releases')
-        body = response.content.decode()
-        archives = []
-        for i in body.splitlines():
-            match = re.search('>(geckodriver-v.*)<', i)
-            if match:
-                archives.append(match.group(1))
-
-        if sys.platform == 'win32':
-            os_keyword = 'win{os_bit_count}'.format(
-                os_bit_count='64' if os.path.exists(r'C:\Program Files (x86)') else '32')
-        elif sys.platform == 'darwin':
-            os_keyword = 'mac'
-        else:
-            os_keyword = 'linux64'
-
-        for file_name in archives:
-            if os_keyword in file_name:
-                installer_file_name = file_name
-                installer_path = f'http://github.com/mozilla/geckodriver/releases/download/' \
-                                 f'{file_name.split("-")[1]}/{file_name}'
-                break
-        else:
-            logger.error('Failed to extract the appropriate web driver from the github gecko driver page')
-            return False
-
-        if not download_url(installer_path, raise_failure=False):
-            return False
-
-        file_ext = os.path.splitext(installer_file_name)[-1]
-        if file_ext == '.zip':
-            logger.info(f'Extracting {installer_file_name} to {web_drivers_folder_path}')
-            with zipfile.ZipFile(installer_file_name, 'r') as zip_ref:
-                zip_ref.extractall(web_drivers_folder_path)
-        elif file_ext == '.gz':
-            with tarfile.open(installer_file_name, "r:gz") as tar:
-                tar.extractall(web_drivers_folder_path)
-        elif file_ext == '.tar':
-            with tarfile.open(installer_file_name, "r:") as tar:
-                tar.extractall(web_drivers_folder_path)
-        else:
-            logger.error(f'Extraction method for file {installer_file_name} is not implemented')
-            return False
-
-        logger.info('Webdriver deployed successfully')
-        return True
-
-
-def full_page_image(url, file_path, page_load_time=5):
-    """Opens the given url in a headless Chrome instance and takes a full page body image
-
-    :param url: Page URL to load and image
-    :param file_path: Image path. Has to be .png file. Existing file will be overwritten
-    :param page_load_time: Time to delay between navigation and screenshot attempt
-    """
-    driver = ChromeDriver(headless=True, fullscreen=True)
-    try:
-        driver.get(url)
-        time.sleep(page_load_time)
-        # Ref: https://stackoverflow.com/a/52572919/
-        required_width = driver.execute_script('return document.body.parentNode.scrollWidth')
-        required_height = driver.execute_script('return document.body.parentNode.scrollHeight')
-        driver.set_window_size(required_width, required_height)
-        # driver.save_screenshot(path)  # has scrollbar
-        driver.find_element_by_tag_name('body').screenshot(file_path)  # avoids scrollbar
-    finally:
-        if driver:
-            driver.quit()
-
-
-def chrome_app_store_full_page_screenshots(driver, base_image_path: str) -> List[str]:
-    """Uses page down to take several screenshots of an entire google chrome app store page
-
-    :param driver: Selenium webdriver live instance (Already on page)
-    :param base_image_path: File path to save the new image. Only support .png files. Existing file will be overwritten.
-     Final path will be <base_image_path>01.png, <base_image_path>02.png etc...
-    :return: List of saved images
-    """
-    saved_images = []  # To store the saved image
-
-    # File type restriction comes from the driver implementation. Only .png file type supported
-    base_image_path = f'{os.path.splitext(base_image_path)[0]}.png'
-    # Scroll to top of the page
-    actions = ActionChains(driver)
-    actions.send_keys(Keys.HOME).perform()
-    # Finds the second "Add to chrome" button as a marker to the end of the page
-    second_add_to_chrome_button = driver.find_elements_by_xpath("//*[text()='Add to Chrome']")[1]
-
-    # Loops page down and saving screenshots of the page
-    for i in range(1, 20):  # Assuming the page will not be longer than 20 page downs length and ensures an exit point
-        image_path = f'{base_image_path[:-4:]}{i:02}.png'
-        driver.get_screenshot_as_file(image_path)
-        saved_images.append(image_path)
-        if driver.is_element_visible_in_viewpoint(second_add_to_chrome_button):
-            break  # Assuming we reached the end of the page if we see the second "Add to chrome" button
-        actions.send_keys(Keys.PAGE_DOWN).perform()
-
-    return saved_images  # Returns the list of taken images
+import os
+import re
+import sys
+import time
+import zipfile
+import tarfile
+import platform
+import logging
+import requests
+from getpass import getuser
+from selenium.webdriver import ActionChains
+from selenium.webdriver.common.keys import Keys
+from typing import List
+from selenium import webdriver
+from selenium.common.exceptions import WebDriverException, SessionNotCreatedException
+from selenium.webdriver.remote.remote_connection import LOGGER as SELENIUM_LOGGER
+from pybenutils.network.download_manager import download_url
+from pybenutils.utils_logger.config_logger import get_logger
+
+logger = get_logger()
+
+
+class DriverTools:
+    """Meant to be inherited by webdriver sub-classes to add general tools and tricks, can be used on all browsers"""
+    LOGGER_DEFAULT_LEVEL = 'DEBUG'
+
+    def __bool__(self):
+        """Returns True only if there are open browser windows / tabs"""
+        return bool(self.get_number_open_tabs())
+
+    # noinspection PyBroadException
+    def get_number_open_tabs(self):
+        """Returns the number of open browser windows and tabs"""
+        try:
+            return len(self.window_handles)
+        except Exception:
+            return 0
+
+    def is_site_displayed(self) -> bool:
+        """Returns True if the current page is displaying a web-page (page might not be fully loaded)"""
+        if not self:
+            return False
+        original_log_level = self.get_logs_levels().get('selenium', self.LOGGER_DEFAULT_LEVEL)
+        self.set_selenium_log_level('WARNING')
+        if 'about:blank' in str(self.current_url):
+            return False
+        body = self.find_element_by_tag_name('body')
+        content = body.text
+        self.set_selenium_log_level(original_log_level)
+        return not [i for i in ['This site can’t be reached',
+                                'Requests to the server have been blocked by an extension',
+                                '404. That’s an error.\nThe requested URL was not found on this server.'] if
+                    i in content]
+
+    @staticmethod
+    def set_selenium_log_level(log_level: str):
+        """Sets the log level of selenium and urllib3
+
+        :param log_level: log level (CRITICAL / FATAL / ERROR / WARNING / INFO / DEBUG / NOTSET)
+        """
+        SELENIUM_LOGGER.setLevel(vars(logging)[log_level.upper()])
+        logging.getLogger("urllib3").setLevel(vars(logging)[log_level.upper()])
+
+    @staticmethod
+    def get_logs_levels():
+        """Returns a dict of the current log levels.
+
+        {'selenium': selenium_log_level, 'urllib3': urllib3_log_level, 'main_logger': utils_log_level}
+        """
+        selenium_log_level = logging._levelToName.get(SELENIUM_LOGGER.getEffectiveLevel())
+        urllib3_log_level = logging._levelToName.get(logging.getLogger("urllib3").getEffectiveLevel())
+        utils_log_level = logging._levelToName.get(logger.getEffectiveLevel())
+        return {'selenium': selenium_log_level,
+                'urllib3': urllib3_log_level,
+                'main_logger': utils_log_level}
+
+    def gracefully_quit(self):
+        """Closing the chrome web driver window, than quitting the webdriver
+              - Support for missing Chrome window
+              - Support for missing driver object
+        """
+        if self:
+            logger.debug('Closing driver')
+            try:
+                self.close()
+            except WebDriverException:
+                logger.error('The chrome browser window was closed unexpectedly')
+            self.quit()
+
+    def switch_to_first_tab(self):
+        """Switches to control the first tab or window opened"""
+        self._switch_to.window(self.window_handles[0])
+
+    def switch_to_last_tab(self):
+        """Switches to control the last tab or window opened"""
+        self._switch_to.window(self.window_handles[-1])
+
+    def close_secondary_tabs(self):
+        """Closes all tabs except the first one in the webdriver window"""
+        while len(self.window_handles) > 1:
+            self.switch_to_last_tab()
+            self.close()
+        self.switch_to_first_tab()
+
+    def open_new_tab(self, url=''):
+        """Attempting to open a new tab with the given URL.
+
+        :param url: URL to open in a new tab. Leave empty for new tab with about:blank
+        """
+        self.execute_script(f'window.open("{url}")')
+
+    def open_and_navigate_to_a_new_tab(self):
+        """Opens a new tab, switched to it and navigates to the new tab address"""
+        self.open_new_tab()
+        self.switch_to_last_tab()
+        self.get(self.NEW_TAB_ADDRESS)
+
+    def is_scrollbar_exist(self):
+        """Returns True if the current web page main window has a vertical scrollbar (Not checking inner elements)"""
+        return self.execute_script(
+            'return document.documentElement.scrollHeight > document.documentElement.clientHeight;')
+
+    def is_element_visible_in_viewpoint(self, element) -> bool:
+        """Return True if the given element is showing the user view point (can be seen on the screen)"""
+        # Calculates the elements position relative position against the user current point of view (see on screen)
+        # Element.is_visible() will return True even if the element is not currently in the user view point
+        return self.execute_script("var elem = arguments[0],                 "
+                                   "  box = elem.getBoundingClientRect(),    "
+                                   "  cx = box.left + box.width / 2,         "
+                                   "  cy = box.top + box.height / 2,         "
+                                   "  e = document.elementFromPoint(cx, cy); "
+                                   "for (; e; e = e.parentElement) {         "
+                                   "  if (e === elem)                        "
+                                   "    return true;                         "
+                                   "}                                        "
+                                   "return false;                            "
+                                   , element)
+
+
+class ChromeDriver(webdriver.Chrome, DriverTools):
+    chrome_default_profile_path = None
+    NEW_TAB_ADDRESS = 'chrome://newtab'
+
+    def __init__(self, *args, **kwargs):
+        """
+        Creates a new instance of the chrome driver.
+        Starts the service and then creates new instance of chrome driver.
+
+         - default_user - [Boolean] Use the default Chrome user installed on the OS (user-data-dir)
+         - fullscreen - [Boolean] Open window at fullscreen (--start-maximized)
+         - excludeSwitches - [List] of switches to exclude (options.add_experimental_option("excludeSwitches", [x]))
+         - crx_path - [Str] Open with extension pre-installed (options.add_extension)
+         - option_args - [List] of arguments to be added to options (options.add_argument(x))
+         - log_level - [Str] Selenium and urllib3 log level (CRITICAL / FATAL / ERROR / WARNING / INFO / DEBUG / NOTSET)
+         - launch_attempts - [int] Permitted number of attempts to launch the selenium web driver
+         - headless - [Boolean] Open the Chrome instance without visible gui (--headless)
+        ----------
+         - executable_path - path to the executable. If the default is used it assumes the executable is in the $PATH
+         - port - port you would like the service to run, if left as 0, a free port will be found.
+         - options - this takes an instance of ChromeOptions
+         - service_args - List of args to pass to the driver service
+         - desired_capabilities - Dictionary object with non-browser specific
+           capabilities only, such as "proxy" or "loggingPref".
+         - service_log_path - Where to log information from the driver.
+         - chrome_options - Deprecated argument for options
+         - keep_alive - Whether to configure ChromeRemoteConnection to use HTTP keep-alive.
+        """
+        self.launch_attempts = kwargs.pop('launch_attempts', 2)
+        self._platform_release = platform.release()
+
+        if kwargs.get('log_level'):
+            self.set_selenium_log_level(kwargs.pop('log_level', self.LOGGER_DEFAULT_LEVEL))
+
+        self.__init_options_object(args, kwargs)
+
+        logger.info('Launching Chrome webdriver')
+        last_exception = None
+        for i in range(self.launch_attempts):
+            try:
+                super().__init__(
+                    *args,
+                    **{'desired_capabilities' if self._platform_release == 'XP' else 'options': self.options},
+                    **kwargs
+                )
+                break
+            except WebDriverException as ex:
+                logger.error(ex)
+                last_exception = ex
+                if type(ex) == SessionNotCreatedException or "executable needs to be in PATH" in str(ex):
+                    self.update()
+            except Exception as ex:
+                logger.error(ex)
+                last_exception = ex
+        else:
+            raise last_exception
+        logger.info('Chrome webdriver launched successfully')
+
+    def __init_options_object(self, args, kwargs):
+        """Handles the creation of Chrome options object"""
+        if self._platform_release == 'XP':
+            self.options = kwargs.pop('options', {"chromeOptions": {
+                "args": [self.get_chrome_profile_path()],
+                "excludeSwitches": ["disable-default-apps", "restore-last-session", "disable-web-resources"]}})
+
+            if kwargs.pop('default_user', False):
+                self.options['chromeOptions']['args'] = [self.get_chrome_profile_path()]
+
+        else:
+            self.options = kwargs.pop('options', webdriver.ChromeOptions())
+            if kwargs.pop('fullscreen', False):
+                self.options.add_argument('--start-maximized')
+
+            if kwargs.pop('headless', False):
+                self.options.add_argument('--headless')
+
+            if kwargs.pop('default_user', False):
+                self.options.add_argument(f"user-data-dir={self.get_chrome_profile_path()}")
+
+            if kwargs.get('excludeSwitches'):
+                switches_to_exclude = kwargs.pop('excludeSwitches', [])
+                self.options.add_experimental_option("excludeSwitches", switches_to_exclude)
+
+            if kwargs.get('crx_path'):
+                self.options.add_extension(kwargs.pop('crx_path', ''))
+
+            for arg in kwargs.pop('option_args', []):
+                self.options.add_argument(arg)
+        return self.options
+
+    def get_chrome_profile_path(self) -> str:
+        """Returns the chrome default profile path"""
+        if not self.chrome_default_profile_path:
+            local_user_name = getuser()
+            if sys.platform != 'win32':  # mac
+                path = f'/Users/{local_user_name}/Library/Application Support/Google/Chrome/'
+            elif self._platform_release == 'XP':  # Winxp path
+                path = r'C:\Documents and Settings\automation\Local Settings\Application Data\Google\Chrome\User Data'
+            else:  # Win OS newer than xp
+                path = f'C:\\Users\\{local_user_name}\\AppData\\Local\\Google\\Chrome\\User Data'
+            self.chrome_default_profile_path = path
+        return self.chrome_default_profile_path
+
+    @staticmethod
+    def update(web_drivers_folder_path=''):
+        """Downloads the latest chrome webdriver
+
+        :param web_drivers_folder_path: Leave empty to download_url to the workspace
+        :return: True if downloaded successfully
+        """
+        # Handling output folder for the new webdriver file
+        if not web_drivers_folder_path:
+            web_drivers_folder_path = os.getcwd()
+        if not os.path.isdir(web_drivers_folder_path):
+            logger.error('The folder you are trying to download_url to does not exist. '
+                         'Please create it and add it to the system path to be recognised correctly')
+            return False
+
+        # Sorting which file to download_url depending on the OS
+        if sys.platform == 'win32':
+            web_driver_zip_file_name = 'chromedriver_win32.zip'
+        elif sys.platform == 'darwin':
+            web_driver_zip_file_name = 'chromedriver_mac64.zip'
+        else:
+            web_driver_zip_file_name = 'chromedriver_linux64.zip'
+
+        logger.info('Getting chrome driver latest stable version number from api')
+        for i in range(3):
+            try:
+                response = requests.get('http://chromedriver.storage.googleapis.com/LATEST_RELEASE')
+                if response.status_code < 400:
+                    latest_version = response.content.decode()
+                    break
+                else:
+                    logger.warning(f'Response status code: {response.status_code}')
+            except Exception as ex:
+                logger.error(ex)
+        else:
+            return False
+
+        logger.info(f'Downloading chrome driver version: {latest_version}')
+        download_url(f'http://chromedriver.storage.googleapis.com/{latest_version}/{web_driver_zip_file_name}')
+
+        logger.info(f'Extracting {web_driver_zip_file_name} to {web_drivers_folder_path}')
+        with zipfile.ZipFile(web_driver_zip_file_name, 'r') as zip_ref:
+            zip_ref.extractall(web_drivers_folder_path)
+
+        logger.info('Webdriver deployed successfully')
+        return True
+
+
+class FirefoxDriver(webdriver.Firefox, DriverTools):
+    NEW_TAB_ADDRESS = 'about:newtab'
+
+    def __init__(self, *args, **kwargs):
+        """Starts a new local session of Firefox.
+
+        Based on the combination and specificity of the various keyword arguments,
+        a capabilities dictionary will be constructed that is passed to the remote end.
+
+        The keyword arguments given to this constructor are helpers to more easily allow Firefox WebDriver sessions
+        to be customised with different options.  They are mapped on to a capabilities dictionary that is passed on
+        to the remote end.
+
+        As some of the options, such as `firefox_profile` and `options.profile` are mutually exclusive,
+        precedence is given from how specific the setting is.  `capabilities` is the least specific keyword argument,
+        followed by `options`, followed by `firefox_binary` and `firefox_profile`.
+
+        In practice this means that if `firefox_profile` and `options.profile` are both set,
+        the selected profile instance will always come from the most specific variable.
+        In this case that would be `firefox_profile`.  This will result in `options.profile` to be ignored because it
+        is considered a less specific setting than the top-level `firefox_profile` keyword argument.
+        Similarly, if you had specified a `capabilities["moz:firefoxOptions"]["profile"]` Base64 string,
+        this would rank below `options.profile`.
+
+         - option_args - [List] of arguments to be added to options (options.add_argument(x))
+         - log_level - [Str] Selenium and urllib3 log level (CRITICAL / FATAL / ERROR / WARNING / INFO / DEBUG / NOTSET)
+         - launch_attempts - [int] Permitted number of attempts to launch the selenium web driver
+        -----------
+         - firefox_profile - Instance of ``FirefoxProfile`` object or a string.
+           If undefined, a fresh profile will be created in a temporary location on the system.
+         - firefox_binary - Instance of ``FirefoxBinary`` or full path to the Firefox binary.
+           If undefined, the system default Firefox installation will  be used.
+         - timeout - Time to wait for Firefox to launch when using the extension connection.
+         - capabilities - Dictionary of desired capabilities.
+         - proxy - The proxy settings to us when communicating with Firefox via the extension connection.
+         - executable_path - Full path to override which geckodriver binary to use for Firefox 47.0.1 and greater,
+           which defaults to picking up the binary from the system path.
+         - options - Instance of ``options.Options``.
+         - service_log_path - Where to log information from the driver.
+         - firefox_options - Deprecated argument for options
+         - service_args - List of args to pass to the driver service
+         - desired_capabilities - alias of capabilities. In future versions of this library,
+           this will replace 'capabilities'. This will make the signature consistent with RemoteWebDriver.
+         - log_path - Deprecated argument for service_log_path
+         - keep_alive - Whether to configure remote_connection.RemoteConnection to use HTTP keep-alive.
+        """
+        self.launch_attempts = kwargs.pop('launch_attempts', 2)
+        self._platform_release = platform.release()
+
+        if kwargs.get('log_level'):
+            self.set_selenium_log_level(kwargs.pop('log_level', self.LOGGER_DEFAULT_LEVEL))
+
+        self.options = kwargs.pop('options', webdriver.FirefoxOptions())
+
+        for arg in kwargs.pop('option_args', []):
+            self.options.add_argument(arg)
+
+        logger.info('Launching Chrome webdriver')
+        last_exception = None
+        for i in range(self.launch_attempts):
+            try:
+                super().__init__(
+                    *args,
+                    **{'desired_capabilities' if self._platform_release == 'XP' else 'options': self.options},
+                    **kwargs
+                )
+                break
+            except WebDriverException as ex:
+                logger.error(ex)
+                last_exception = ex
+                if type(ex) == SessionNotCreatedException or "executable needs to be in PATH" in str(ex):
+                    self.update()
+            except Exception as ex:
+                logger.error(ex)
+                last_exception = ex
+        else:
+            raise last_exception
+        logger.info('Firefox webdriver launched successfully')
+
+    @staticmethod
+    def update(web_drivers_folder_path=''):
+        """Downloads the latest gecko (firefox) webdriver
+
+        :param web_drivers_folder_path: Leave empty to download_url to the workspace
+        :return: True if downloaded successfully
+        """
+        if not web_drivers_folder_path:
+            web_drivers_folder_path = os.getcwd()
+        if not os.path.isdir(web_drivers_folder_path):
+            logger.error('The folder you are trying to download_url to does not exist. '
+                         'Please create it and add it to the system path to be recognised correctly')
+            return False
+
+        # Creating a list of archive files appearing in this page to get the latest webdriver archive file name.
+        response = requests.get('https://github.com/mozilla/geckodriver/releases')
+        body = response.content.decode()
+        archives = []
+        for i in body.splitlines():
+            match = re.search('>(geckodriver-v.*)<', i)
+            if match:
+                archives.append(match.group(1))
+
+        if sys.platform == 'win32':
+            os_keyword = 'win{os_bit_count}'.format(
+                os_bit_count='64' if os.path.exists(r'C:\Program Files (x86)') else '32')
+        elif sys.platform == 'darwin':
+            os_keyword = 'mac'
+        else:
+            os_keyword = 'linux64'
+
+        for file_name in archives:
+            if os_keyword in file_name:
+                installer_file_name = file_name
+                installer_path = f'http://github.com/mozilla/geckodriver/releases/download/' \
+                                 f'{file_name.split("-")[1]}/{file_name}'
+                break
+        else:
+            logger.error('Failed to extract the appropriate web driver from the github gecko driver page')
+            return False
+
+        if not download_url(installer_path, raise_failure=False):
+            return False
+
+        file_ext = os.path.splitext(installer_file_name)[-1]
+        if file_ext == '.zip':
+            logger.info(f'Extracting {installer_file_name} to {web_drivers_folder_path}')
+            with zipfile.ZipFile(installer_file_name, 'r') as zip_ref:
+                zip_ref.extractall(web_drivers_folder_path)
+        elif file_ext == '.gz':
+            with tarfile.open(installer_file_name, "r:gz") as tar:
+                def is_within_directory(directory, target):
+                    
+                    abs_directory = os.path.abspath(directory)
+                    abs_target = os.path.abspath(target)
+                
+                    prefix = os.path.commonprefix([abs_directory, abs_target])
+                    
+                    return prefix == abs_directory
+                
+                def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+                
+                    for member in tar.getmembers():
+                        member_path = os.path.join(path, member.name)
+                        if not is_within_directory(path, member_path):
+                            raise Exception("Attempted Path Traversal in Tar File")
+                
+                    tar.extractall(path, members, numeric_owner=numeric_owner) 
+                    
+                
+                safe_extract(tar, web_drivers_folder_path)
+        elif file_ext == '.tar':
+            with tarfile.open(installer_file_name, "r:") as tar:
+                def is_within_directory(directory, target):
+                    
+                    abs_directory = os.path.abspath(directory)
+                    abs_target = os.path.abspath(target)
+                
+                    prefix = os.path.commonprefix([abs_directory, abs_target])
+                    
+                    return prefix == abs_directory
+                
+                def safe_extract(tar, path=".", members=None, *, numeric_owner=False):
+                
+                    for member in tar.getmembers():
+                        member_path = os.path.join(path, member.name)
+                        if not is_within_directory(path, member_path):
+                            raise Exception("Attempted Path Traversal in Tar File")
+                
+                    tar.extractall(path, members, numeric_owner=numeric_owner) 
+                    
+                
+                safe_extract(tar, web_drivers_folder_path)
+        else:
+            logger.error(f'Extraction method for file {installer_file_name} is not implemented')
+            return False
+
+        logger.info('Webdriver deployed successfully')
+        return True
+
+
+def full_page_image(url, file_path, page_load_time=5):
+    """Opens the given url in a headless Chrome instance and takes a full page body image
+
+    :param url: Page URL to load and image
+    :param file_path: Image path. Has to be .png file. Existing file will be overwritten
+    :param page_load_time: Time to delay between navigation and screenshot attempt
+    """
+    driver = ChromeDriver(headless=True, fullscreen=True)
+    try:
+        driver.get(url)
+        time.sleep(page_load_time)
+        # Ref: https://stackoverflow.com/a/52572919/
+        required_width = driver.execute_script('return document.body.parentNode.scrollWidth')
+        required_height = driver.execute_script('return document.body.parentNode.scrollHeight')
+        driver.set_window_size(required_width, required_height)
+        # driver.save_screenshot(path)  # has scrollbar
+        driver.find_element_by_tag_name('body').screenshot(file_path)  # avoids scrollbar
+    finally:
+        if driver:
+            driver.quit()
+
+
+def chrome_app_store_full_page_screenshots(driver, base_image_path: str) -> List[str]:
+    """Uses page down to take several screenshots of an entire google chrome app store page
+
+    :param driver: Selenium webdriver live instance (Already on page)
+    :param base_image_path: File path to save the new image. Only support .png files. Existing file will be overwritten.
+     Final path will be <base_image_path>01.png, <base_image_path>02.png etc...
+    :return: List of saved images
+    """
+    saved_images = []  # To store the saved image
+
+    # File type restriction comes from the driver implementation. Only .png file type supported
+    base_image_path = f'{os.path.splitext(base_image_path)[0]}.png'
+    # Scroll to top of the page
+    actions = ActionChains(driver)
+    actions.send_keys(Keys.HOME).perform()
+    # Finds the second "Add to chrome" button as a marker to the end of the page
+    second_add_to_chrome_button = driver.find_elements_by_xpath("//*[text()='Add to Chrome']")[1]
+
+    # Loops page down and saving screenshots of the page
+    for i in range(1, 20):  # Assuming the page will not be longer than 20 page downs length and ensures an exit point
+        image_path = f'{base_image_path[:-4:]}{i:02}.png'
+        driver.get_screenshot_as_file(image_path)
+        saved_images.append(image_path)
+        if driver.is_element_visible_in_viewpoint(second_add_to_chrome_button):
+            break  # Assuming we reached the end of the page if we see the second "Add to chrome" button
+        actions.send_keys(Keys.PAGE_DOWN).perform()
+
+    return saved_images  # Returns the list of taken images
```

### Comparing `pybenutils-3.1.0/pybenutils/browsers/simple_browser_controller_cls.py` & `pybenutils-3.2.2/pybenutils/browsers/simple_browser_controller_cls.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,445 +1,445 @@
-import sys
-import time
-from typing import List
-from getpass import getuser
-from psutil import NoSuchProcess
-from pybenutils.utils_logger.config_logger import get_logger
-from pybenutils.os_operations.process import ProcessHandler
-from pybenutils.os_operations.window_operations import get_hwnds_by_class, click_on_point
-from pybenutils.browsers.windows_browsers_keywords import set_browser_url, close_browser, get_to_home_page, \
-    open_browser_windows
-if sys.platform == 'win32':
-    import win32com.client
-    import win32gui
-else:
-    from pybenutils.os_operations.mac_operations import run_apple_script
-
-logger = get_logger()
-
-
-def kill_all_browsers(browsers_list=('iexplore.exe', 'IEDriverServer.exe', 'chrome', 'firefox', 'chromedriver',
-                                     'safari', 'chromium', 'geckodriver', 'msedge'),
-                      attempt_graceful_shutdown=True):
-    """Closes and kills all the process sharing the given process names in the input list
-
-    :param browsers_list: Browsers process name to kill
-    :param attempt_graceful_shutdown: Attempts to close the browser before killing its processes
-    """
-    if type(browsers_list) == str:
-        browsers_list = [browsers_list]
-    for browser in browsers_list:
-        brw = SimpleBrowserController(browser)
-        brw.kill(attempt_graceful_shutdown=attempt_graceful_shutdown)
-        time.sleep(5)
-
-
-def close_all_browsers(browsers_list=('iexplore.exe', 'IEDriverServer.exe', 'chrome', 'firefox', 'chromedriver',
-                                      'safari', 'chromium', 'geckodriver', 'msedge')):
-    """Closes all the process sharing the given process names in the input list
-
-    :param browsers_list: Browsers process name to kill
-    """
-    if type(browsers_list) == str:
-        browsers_list = [browsers_list]
-    for browser in browsers_list:
-        brw = SimpleBrowserController(browser)
-        brw.close()
-        time.sleep(5)
-
-
-class SimpleBrowserController:
-    def __init__(self, browser_name):
-        """Initiates the class
-
-        :param browser_name: In Windows, process name. In mac: Full application path OR one of the pre-supported apps.
-         Supported apps: safari, chrome, chromium, firefox, msedge
-        """
-        process_names_mac_conversion_table = {
-            'safari': '/Applications/Safari.app',
-            'chrome': '/Applications/Google Chrome.app',
-            'chromium': '/Users/{u_name}/Applications/Chromium.app'.format(u_name=getuser()),
-            'firefox': '/Applications/Firefox.app',
-            'msedge': '/Applications/Microsoft Edge.app'
-        }
-        class_name_windows_conversion_table = {
-            'chromedriver.exe': 'Chrome_WidgetWin_1',
-            'chrome.exe': 'Chrome_WidgetWin_1',
-            'firefox.exe': 'MozillaWindowClass',
-            'geckodriver.exe': 'MozillaWindowClass',
-            'iexplore.exe': 'IEFrame',
-            'IEDriverServer.exe': 'IEFrame',
-            'msedge.exe': 'Chrome_WidgetWin_1'
-        }
-        self.browser_name = browser_name
-        if sys.platform != 'win32' and browser_name in process_names_mac_conversion_table:
-            self.browser_name = process_names_mac_conversion_table[browser_name]
-
-        self.browser_process_name = self.browser_name
-        if self.browser_name in ['chrome', 'chrome.exe', 'chromium', 'chromium.exe']:
-            self.browser_process_name = 'chrome.exe'
-        elif sys.platform == 'win32' and not self.browser_process_name.endswith('.exe'):
-            self.browser_process_name = '{brw}.exe'.format(brw=self.browser_process_name)
-
-        self.hwnd = []
-        self.app_obj = None
-        if sys.platform != 'win32':
-            from pybenutils.os_operations.mac_application_control import ApplicationControl
-            self.app_obj = ApplicationControl(self.browser_name)
-        else:
-            self.class_name = class_name_windows_conversion_table[self.browser_process_name] if \
-                self.browser_process_name in class_name_windows_conversion_table else ''
-
-    def launch(self, arguments=()) -> bool:
-        """Launching the app
-        :param arguments: launch shell arguments
-        """
-        logger.info('Launching browser: {brw}{arg}'.format(
-            brw=self.browser_name, arg=f' With args: {arguments}' if arguments else ''))
-        if sys.platform == 'win32':
-            new_handler = open_browser_windows(browser=self.browser_name, arguments=arguments)
-            if not new_handler:
-                return False
-            self.hwnd.append(new_handler)
-            return True
-        else:
-            return self.app_obj.launch(arguments=arguments)
-
-    def kill(self, attempt_graceful_shutdown=True):
-        """Killing the browser processes
-        :param attempt_graceful_shutdown: Try to gracefully close the browser before killing it
-        """
-        if attempt_graceful_shutdown:
-            self.close()
-            time.sleep(20)
-        logger.info('Killing {brw} browser instances'.format(brw=self.browser_process_name))
-        if sys.platform == 'win32':
-            p_handler = ProcessHandler(self.browser_process_name)
-            try:
-                p_handler.kill_process()
-            except NoSuchProcess as ex:
-                logger.warning(ex)
-                time.sleep(20)
-                self.kill(attempt_graceful_shutdown=attempt_graceful_shutdown)
-            self.hwnd = []
-        else:
-            self.app_obj.kill()
-        time.sleep(10)
-        if ProcessHandler(self.browser_process_name).proc_list:
-            logger.warning('Some processes of {na} stayed alive'.format(na=self.browser_process_name))
-
-    def close(self) -> bool:
-        """Try to gracefully close the browser
-        :return: True if successful
-        """
-        logger.info('Trying to close the {brw} browser instances'.format(brw=self.browser_name))
-        if sys.platform == 'win32':
-            if close_browser(self.browser_name):
-                self.hwnd = []
-                return True
-            self.press_enter_button()
-            time.sleep(3)
-            if close_browser(self.browser_name):
-                self.hwnd = []
-                return True
-            logger.warning('{n} could not be gracefully closed'.format(n=self.browser_name))
-            return False
-        else:
-            self.app_obj.close()
-            time.sleep(3)
-            return True
-
-    def refresh_hwnd_list(self) -> List:
-        self.hwnd = get_hwnds_by_class(self.class_name)
-        return self.hwnd
-
-    def get_hwnd(self) -> List:
-        """Returns the hwnd list parameter"""
-        return self.hwnd
-
-    def press_key_combination_on_mac_browser(self, key_command) -> bool:
-        """Attempts to press the requested command on the keyboard
-
-        :return: True if successful
-        """
-        try:
-            if sys.platform == 'win32':
-                logger.warning('You are trying to use a mac function on a windows os')
-                return False
-            else:
-                cmd = 'tell application "{app_name}" to activate\ntell application "System Events" to' \
-                      ' {key_combination}'.format(app_name=self.browser_name, key_combination=key_command)
-                result = run_apple_script(cmd)
-                if not result:
-                    raise Exception('The Apple script has failed')
-        except Exception as ex:
-            logger.error('Failed to press requested keys for error: {err}'.format(err=str(ex)))
-            return False
-        return True
-
-    def get_to_home_page(self) -> bool:
-        """Attempts to navigate to the home page using the keyboard shortcut keys
-
-        :return: True if successful
-        """
-        try:
-            if sys.platform == 'win32':
-                errors = []
-                if not self.hwnd:
-                    self.refresh_hwnd_list()
-                for hwnd in self.hwnd:
-                    try:
-                        get_to_home_page(hwnd)
-                        break
-                    except Exception as ex:
-                        errors.append(str(ex))
-                else:
-                    logger.error('Failed to click on HOME button for errors: {err}'.format(err=errors))
-            else:
-                if 'firefox' in self.browser_name.lower():
-                    return self.press_key_combination_on_mac_browser('key code 115 using option down')
-                else:
-                    return self.press_key_combination_on_mac_browser('key code 4 using {command down, shift down}')
-        except Exception as ex:
-            logger.error(f'Failed to press on the HOME button for error: {ex}')
-            return False
-        return True
-
-    def press_esc_button(self) -> bool:
-        """Attempts to press the ESC button on the keyboard
-
-        :return: True if successful
-        """
-        try:
-            if sys.platform == 'win32':
-                shell = win32com.client.Dispatch("WScript.Shell")
-                shell.SendKeys("{ESC}", 1)
-            else:
-                return self.press_key_combination_on_mac_browser('key code 53 using option down')
-        except Exception as ex:
-            logger.error(f'Failed to press on the ESC button for error: {ex}')
-            return False
-        return True
-
-    def press_enter_button(self) -> bool:
-        """Attempts to press the ENTER button on the keyboard
-
-        :return: True if successful
-        """
-        try:
-            if sys.platform == 'win32':
-                shell = win32com.client.Dispatch("WScript.Shell")
-                shell.SendKeys("{ENTER}", 1)
-            else:
-                return self.press_key_combination_on_mac_browser('key code 76')
-        except Exception as ex:
-            logger.error(f'Failed to press on the ENTER button for error: {ex}')
-            return False
-        return True
-
-    def send_keyboard_keys(self, text) -> bool:
-        """Attempts to send the given text trough the keyboard
-        :param text: The text to send to the browser
-        :return: True if successful
-        """
-        try:
-            if sys.platform == 'win32':
-                shell = win32com.client.Dispatch("WScript.Shell")
-                shell.SendKeys(text, 1)
-            else:
-                self.press_key_combination_on_mac_browser('keystroke "{text}"'.format(text=text))
-        except Exception as ex:
-            logger.error(f'Failed to send keys for error: {ex}')
-            return False
-        return True
-
-    def set_browser_url(self, url) -> bool:
-        """Input the given url into the browser search line and press ENTER
-
-        :param url: Text to be searched / Site url
-        :return: True if successful
-        """
-        try:
-            if sys.platform == 'win32':
-                errors = []
-                if not self.hwnd:
-                    self.refresh_hwnd_list()
-                for hwnd in self.hwnd:
-                    try:
-                        set_browser_url(hwnd, url)
-                        break
-                    except Exception as ex:
-                        errors.append(str(ex))
-                else:
-                    logger.error('Failed to set browser url for errors: {err}'.format(err=errors))
-
-            else:
-                self.press_key_combination_on_mac_browser('key code 37 using command down')
-                self.send_keyboard_keys(url)
-                self.press_enter_button()
-
-        except Exception as ex:
-            logger.error(f'Failed to set the browser url for error: {ex}')
-            return False
-        return True
-
-    def switch_tab(self) -> bool:
-        """Attempts to switch a tab using the keyboard
-        :return: True if successful
-        """
-        try:
-            if sys.platform == 'win32':
-                shell = win32com.client.Dispatch("WScript.Shell")
-                shell.SendKeys("^{TAB}", 1)
-            else:
-                return self.press_key_combination_on_mac_browser('key code 48 using control down')
-        except Exception as ex:
-            logger.error(f'Failed to switch tabs for error: {ex}')
-            return False
-        return True
-
-    def set_focus_by_mouse_click(self):
-        """Set focus on browser window by clicking on it with the mouse
-
-        :return: True if no exception had occurred assuming success
-        """
-        if sys.platform == 'win32':
-            self.refresh_hwnd_list()
-            for i in self.get_hwnd():
-                try:
-                    rect = win32gui.GetWindowRect(i)  # The window (0.0.0.0) point is at the top left corner
-                    start_menu_safe_zone = win32gui.GetWindowRect(win32gui.GetDesktopWindow())[3] - rect[1] - 130 > 40
-                    if rect != (0, 0, 0, 0) and win32gui.IsWindowVisible(i) and start_menu_safe_zone:
-                        # Avoid trying to click on background processes
-                        click_on_point(i, rect[0] + 10, rect[1] + 130)
-                        return True
-                except Exception as ex:
-                    print(ex)
-                    return False
-        else:
-            print('Not yet implemented')
-            return False
-
-    def send_console_command(self, command: str):
-        """Sends console commands to the browser using keyboard navigation"""
-        shell_send_keys_replacements = {'+': '{+}', '^': '{^}', '%': '{%}', '~': '{~}', '(': '{(}', ')': '{)}',
-                                        '{': '{{}', '}': '{}}', '[': '{[}', ']': '{]}'}
-        if sys.platform == 'win32':
-            command = ''.join([shell_send_keys_replacements.get(c, c) for c in command])
-            if 'firefox' in self.browser_name:
-                self.send_keyboard_keys('^+{K}')
-                time.sleep(1)
-                self.set_focus_by_mouse_click()
-                self.send_keyboard_keys('^+{K}')
-                time.sleep(1)
-                self.send_keyboard_keys(command)
-                time.sleep(1)
-                self.press_enter_button()
-                time.sleep(1)
-                self.send_keyboard_keys('{F12}')
-            elif 'chrome' in self.browser_name:
-                self.send_keyboard_keys('^+{j}')
-                time.sleep(2)
-                self.send_keyboard_keys(command)
-                time.sleep(1)
-                self.press_enter_button()
-                time.sleep(1)
-                self.send_keyboard_keys('{F12}')
-            else:
-                raise AssertionError(f'The requested operation is not yet implemented for {self.browser_name}')
-        else:
-            raise AssertionError(f'The requested operation is only implemented for windows')
-
-    def is_running(self):
-        """Returns True if an instance of the browser is open"""
-        if sys.platform == 'win32':
-            self.refresh_hwnd_list()
-            return bool(self.get_hwnd())
-        else:
-            return self.app_obj.is_running()
-
-    def press_tab_button(self):
-        """Using the keyboard, press the TAB button"""
-        result = self.send_keyboard_keys("{TAB}") if sys.platform == 'win32' else \
-            self.press_key_combination_on_mac_browser('key code 48')
-        return result
-
-    def approve_chrome_changed_assets_alert(self, tab_presses=4):
-        """Using the keyboard to click on "keep changes" at chrome's "accept asset change" popup
-
-        :param tab_presses: Number of times to press the tab key before pressing Enter. Set to 4 to support Chrome ver83
-        """
-        logger.debug(f'Pressing {tab_presses} "tab" an an "enter" to click on "keep changes"')
-        for key_press in range(tab_presses):
-            self.press_tab_button()
-            time.sleep(1)  # Time for the button to register correctly in the OS
-        self.press_enter_button()
-        time.sleep(1)  # Time for the button to register correctly in the OS
-
-    def open_a_new_tab(self):
-        """Press the Ctrl + t combination using keyboard keys to open a new tab"""
-        logger.debug('Attempting to open a new tab')
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('^t')
-        else:
-            self.press_key_combination_on_mac_browser('key code 17 using command down')
-
-    def reset_zoom_level(self):
-        """Press the combination ctrl/command + '0' keyboard keys - reset zoom level to 100%"""
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('^0')
-        else:
-            self.press_key_combination_on_mac_browser('key code 82 using command down')
-
-    def decrease_zoom_level(self):
-        """Press the combination ctrl/command + '-' keyboard keys - zoom out"""
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('^{-}')
-        else:
-            self.press_key_combination_on_mac_browser('key code 78 using command down')
-
-    def increase_zoom_level(self):
-        """Press the combination ctrl/command + '+' keyboard keys - zoom in"""
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('^{+}')
-        else:
-            self.press_key_combination_on_mac_browser('key code 69 using command down')
-
-    def set_zoom_level_to_max(self):
-        """Press the combination ctrl/command + '+' keyboard keys 10 times - zoom in all the way"""
-        self.reset_zoom_level()
-        for i in range(10):
-            self.increase_zoom_level()
-
-    def set_zoom_level_to_min(self):
-        """Press the combination ctrl/command + '-' keyboard keys 10 times - zoom out all the way"""
-        self.reset_zoom_level()
-        for i in range(10):
-            self.decrease_zoom_level()
-
-    def press_page_down(self):
-        """Press the page down key"""
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('{PGDN}')
-        else:
-            self.press_key_combination_on_mac_browser('key code 121')
-
-    def press_page_up(self):
-        """Press the page up key"""
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('{PGUP}')
-        else:
-            self.press_key_combination_on_mac_browser('key code 116')
-
-    def press_ctrl_home(self):
-        """Press the combination ctrl/command + home keyboard keys - Scroll to top of the page"""
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('^{HOME}')
-        else:
-            self.press_key_combination_on_mac_browser('key code 115 using command down')
-
-    def press_ctrl_end(self):
-        """Press the combination ctrl/command + end keyboard keys - Scroll to end of the page"""
-        if sys.platform == 'win32':
-            self.send_keyboard_keys('^{END}')
-        else:
-            self.press_key_combination_on_mac_browser('key code 119 using command down')
+import sys
+import time
+from typing import List
+from getpass import getuser
+from psutil import NoSuchProcess
+from pybenutils.utils_logger.config_logger import get_logger
+from pybenutils.os_operations.process import ProcessHandler
+from pybenutils.os_operations.window_operations import get_hwnds_by_class, click_on_point
+from pybenutils.browsers.windows_browsers_keywords import set_browser_url, close_browser, get_to_home_page, \
+    open_browser_windows
+if sys.platform == 'win32':
+    import win32com.client
+    import win32gui
+else:
+    from pybenutils.os_operations.mac_operations import run_apple_script
+
+logger = get_logger()
+
+
+def kill_all_browsers(browsers_list=('iexplore.exe', 'IEDriverServer.exe', 'chrome', 'firefox', 'chromedriver',
+                                     'safari', 'chromium', 'geckodriver', 'msedge'),
+                      attempt_graceful_shutdown=True):
+    """Closes and kills all the process sharing the given process names in the input list
+
+    :param browsers_list: Browsers process name to kill
+    :param attempt_graceful_shutdown: Attempts to close the browser before killing its processes
+    """
+    if type(browsers_list) == str:
+        browsers_list = [browsers_list]
+    for browser in browsers_list:
+        brw = SimpleBrowserController(browser)
+        brw.kill(attempt_graceful_shutdown=attempt_graceful_shutdown)
+        time.sleep(5)
+
+
+def close_all_browsers(browsers_list=('iexplore.exe', 'IEDriverServer.exe', 'chrome', 'firefox', 'chromedriver',
+                                      'safari', 'chromium', 'geckodriver', 'msedge')):
+    """Closes all the process sharing the given process names in the input list
+
+    :param browsers_list: Browsers process name to kill
+    """
+    if type(browsers_list) == str:
+        browsers_list = [browsers_list]
+    for browser in browsers_list:
+        brw = SimpleBrowserController(browser)
+        brw.close()
+        time.sleep(5)
+
+
+class SimpleBrowserController:
+    def __init__(self, browser_name):
+        """Initiates the class
+
+        :param browser_name: In Windows, process name. In mac: Full application path OR one of the pre-supported apps.
+         Supported apps: safari, chrome, chromium, firefox, msedge
+        """
+        process_names_mac_conversion_table = {
+            'safari': '/Applications/Safari.app',
+            'chrome': '/Applications/Google Chrome.app',
+            'chromium': '/Users/{u_name}/Applications/Chromium.app'.format(u_name=getuser()),
+            'firefox': '/Applications/Firefox.app',
+            'msedge': '/Applications/Microsoft Edge.app'
+        }
+        class_name_windows_conversion_table = {
+            'chromedriver.exe': 'Chrome_WidgetWin_1',
+            'chrome.exe': 'Chrome_WidgetWin_1',
+            'firefox.exe': 'MozillaWindowClass',
+            'geckodriver.exe': 'MozillaWindowClass',
+            'iexplore.exe': 'IEFrame',
+            'IEDriverServer.exe': 'IEFrame',
+            'msedge.exe': 'Chrome_WidgetWin_1'
+        }
+        self.browser_name = browser_name
+        if sys.platform != 'win32' and browser_name in process_names_mac_conversion_table:
+            self.browser_name = process_names_mac_conversion_table[browser_name]
+
+        self.browser_process_name = self.browser_name
+        if self.browser_name in ['chrome', 'chrome.exe', 'chromium', 'chromium.exe']:
+            self.browser_process_name = 'chrome.exe'
+        elif sys.platform == 'win32' and not self.browser_process_name.endswith('.exe'):
+            self.browser_process_name = '{brw}.exe'.format(brw=self.browser_process_name)
+
+        self.hwnd = []
+        self.app_obj = None
+        if sys.platform != 'win32':
+            from pybenutils.os_operations.mac_application_control import ApplicationControl
+            self.app_obj = ApplicationControl(self.browser_name)
+        else:
+            self.class_name = class_name_windows_conversion_table[self.browser_process_name] if \
+                self.browser_process_name in class_name_windows_conversion_table else ''
+
+    def launch(self, arguments=()) -> bool:
+        """Launching the app
+        :param arguments: launch shell arguments
+        """
+        logger.info('Launching browser: {brw}{arg}'.format(
+            brw=self.browser_name, arg=f' With args: {arguments}' if arguments else ''))
+        if sys.platform == 'win32':
+            new_handler = open_browser_windows(browser=self.browser_name, arguments=arguments)
+            if not new_handler:
+                return False
+            self.hwnd.append(new_handler)
+            return True
+        else:
+            return self.app_obj.launch(arguments=arguments)
+
+    def kill(self, attempt_graceful_shutdown=True):
+        """Killing the browser processes
+        :param attempt_graceful_shutdown: Try to gracefully close the browser before killing it
+        """
+        if attempt_graceful_shutdown:
+            self.close()
+            time.sleep(20)
+        logger.info('Killing {brw} browser instances'.format(brw=self.browser_process_name))
+        if sys.platform == 'win32':
+            p_handler = ProcessHandler(self.browser_process_name)
+            try:
+                p_handler.kill_process()
+            except NoSuchProcess as ex:
+                logger.warning(ex)
+                time.sleep(20)
+                self.kill(attempt_graceful_shutdown=attempt_graceful_shutdown)
+            self.hwnd = []
+        else:
+            self.app_obj.kill()
+        time.sleep(10)
+        if ProcessHandler(self.browser_process_name).proc_list:
+            logger.warning('Some processes of {na} stayed alive'.format(na=self.browser_process_name))
+
+    def close(self) -> bool:
+        """Try to gracefully close the browser
+        :return: True if successful
+        """
+        logger.info('Trying to close the {brw} browser instances'.format(brw=self.browser_name))
+        if sys.platform == 'win32':
+            if close_browser(self.browser_name):
+                self.hwnd = []
+                return True
+            self.press_enter_button()
+            time.sleep(3)
+            if close_browser(self.browser_name):
+                self.hwnd = []
+                return True
+            logger.warning('{n} could not be gracefully closed'.format(n=self.browser_name))
+            return False
+        else:
+            self.app_obj.close()
+            time.sleep(3)
+            return True
+
+    def refresh_hwnd_list(self) -> List:
+        self.hwnd = get_hwnds_by_class(self.class_name)
+        return self.hwnd
+
+    def get_hwnd(self) -> List:
+        """Returns the hwnd list parameter"""
+        return self.hwnd
+
+    def press_key_combination_on_mac_browser(self, key_command) -> bool:
+        """Attempts to press the requested command on the keyboard
+
+        :return: True if successful
+        """
+        try:
+            if sys.platform == 'win32':
+                logger.warning('You are trying to use a mac function on a windows os')
+                return False
+            else:
+                cmd = 'tell application "{app_name}" to activate\ntell application "System Events" to' \
+                      ' {key_combination}'.format(app_name=self.browser_name, key_combination=key_command)
+                result = run_apple_script(cmd)
+                if not result:
+                    raise Exception('The Apple script has failed')
+        except Exception as ex:
+            logger.error('Failed to press requested keys for error: {err}'.format(err=str(ex)))
+            return False
+        return True
+
+    def get_to_home_page(self) -> bool:
+        """Attempts to navigate to the home page using the keyboard shortcut keys
+
+        :return: True if successful
+        """
+        try:
+            if sys.platform == 'win32':
+                errors = []
+                if not self.hwnd:
+                    self.refresh_hwnd_list()
+                for hwnd in self.hwnd:
+                    try:
+                        get_to_home_page(hwnd)
+                        break
+                    except Exception as ex:
+                        errors.append(str(ex))
+                else:
+                    logger.error('Failed to click on HOME button for errors: {err}'.format(err=errors))
+            else:
+                if 'firefox' in self.browser_name.lower():
+                    return self.press_key_combination_on_mac_browser('key code 115 using option down')
+                else:
+                    return self.press_key_combination_on_mac_browser('key code 4 using {command down, shift down}')
+        except Exception as ex:
+            logger.error(f'Failed to press on the HOME button for error: {ex}')
+            return False
+        return True
+
+    def press_esc_button(self) -> bool:
+        """Attempts to press the ESC button on the keyboard
+
+        :return: True if successful
+        """
+        try:
+            if sys.platform == 'win32':
+                shell = win32com.client.Dispatch("WScript.Shell")
+                shell.SendKeys("{ESC}", 1)
+            else:
+                return self.press_key_combination_on_mac_browser('key code 53 using option down')
+        except Exception as ex:
+            logger.error(f'Failed to press on the ESC button for error: {ex}')
+            return False
+        return True
+
+    def press_enter_button(self) -> bool:
+        """Attempts to press the ENTER button on the keyboard
+
+        :return: True if successful
+        """
+        try:
+            if sys.platform == 'win32':
+                shell = win32com.client.Dispatch("WScript.Shell")
+                shell.SendKeys("{ENTER}", 1)
+            else:
+                return self.press_key_combination_on_mac_browser('key code 76')
+        except Exception as ex:
+            logger.error(f'Failed to press on the ENTER button for error: {ex}')
+            return False
+        return True
+
+    def send_keyboard_keys(self, text) -> bool:
+        """Attempts to send the given text trough the keyboard
+        :param text: The text to send to the browser
+        :return: True if successful
+        """
+        try:
+            if sys.platform == 'win32':
+                shell = win32com.client.Dispatch("WScript.Shell")
+                shell.SendKeys(text, 1)
+            else:
+                self.press_key_combination_on_mac_browser('keystroke "{text}"'.format(text=text))
+        except Exception as ex:
+            logger.error(f'Failed to send keys for error: {ex}')
+            return False
+        return True
+
+    def set_browser_url(self, url) -> bool:
+        """Input the given url into the browser search line and press ENTER
+
+        :param url: Text to be searched / Site url
+        :return: True if successful
+        """
+        try:
+            if sys.platform == 'win32':
+                errors = []
+                if not self.hwnd:
+                    self.refresh_hwnd_list()
+                for hwnd in self.hwnd:
+                    try:
+                        set_browser_url(hwnd, url)
+                        break
+                    except Exception as ex:
+                        errors.append(str(ex))
+                else:
+                    logger.error('Failed to set browser url for errors: {err}'.format(err=errors))
+
+            else:
+                self.press_key_combination_on_mac_browser('key code 37 using command down')
+                self.send_keyboard_keys(url)
+                self.press_enter_button()
+
+        except Exception as ex:
+            logger.error(f'Failed to set the browser url for error: {ex}')
+            return False
+        return True
+
+    def switch_tab(self) -> bool:
+        """Attempts to switch a tab using the keyboard
+        :return: True if successful
+        """
+        try:
+            if sys.platform == 'win32':
+                shell = win32com.client.Dispatch("WScript.Shell")
+                shell.SendKeys("^{TAB}", 1)
+            else:
+                return self.press_key_combination_on_mac_browser('key code 48 using control down')
+        except Exception as ex:
+            logger.error(f'Failed to switch tabs for error: {ex}')
+            return False
+        return True
+
+    def set_focus_by_mouse_click(self):
+        """Set focus on browser window by clicking on it with the mouse
+
+        :return: True if no exception had occurred assuming success
+        """
+        if sys.platform == 'win32':
+            self.refresh_hwnd_list()
+            for i in self.get_hwnd():
+                try:
+                    rect = win32gui.GetWindowRect(i)  # The window (0.0.0.0) point is at the top left corner
+                    start_menu_safe_zone = win32gui.GetWindowRect(win32gui.GetDesktopWindow())[3] - rect[1] - 130 > 40
+                    if rect != (0, 0, 0, 0) and win32gui.IsWindowVisible(i) and start_menu_safe_zone:
+                        # Avoid trying to click on background processes
+                        click_on_point(i, rect[0] + 10, rect[1] + 130)
+                        return True
+                except Exception as ex:
+                    print(ex)
+                    return False
+        else:
+            print('Not yet implemented')
+            return False
+
+    def send_console_command(self, command: str):
+        """Sends console commands to the browser using keyboard navigation"""
+        shell_send_keys_replacements = {'+': '{+}', '^': '{^}', '%': '{%}', '~': '{~}', '(': '{(}', ')': '{)}',
+                                        '{': '{{}', '}': '{}}', '[': '{[}', ']': '{]}'}
+        if sys.platform == 'win32':
+            command = ''.join([shell_send_keys_replacements.get(c, c) for c in command])
+            if 'firefox' in self.browser_name:
+                self.send_keyboard_keys('^+{K}')
+                time.sleep(1)
+                self.set_focus_by_mouse_click()
+                self.send_keyboard_keys('^+{K}')
+                time.sleep(1)
+                self.send_keyboard_keys(command)
+                time.sleep(1)
+                self.press_enter_button()
+                time.sleep(1)
+                self.send_keyboard_keys('{F12}')
+            elif 'chrome' in self.browser_name:
+                self.send_keyboard_keys('^+{j}')
+                time.sleep(2)
+                self.send_keyboard_keys(command)
+                time.sleep(1)
+                self.press_enter_button()
+                time.sleep(1)
+                self.send_keyboard_keys('{F12}')
+            else:
+                raise AssertionError(f'The requested operation is not yet implemented for {self.browser_name}')
+        else:
+            raise AssertionError(f'The requested operation is only implemented for windows')
+
+    def is_running(self):
+        """Returns True if an instance of the browser is open"""
+        if sys.platform == 'win32':
+            self.refresh_hwnd_list()
+            return bool(self.get_hwnd())
+        else:
+            return self.app_obj.is_running()
+
+    def press_tab_button(self):
+        """Using the keyboard, press the TAB button"""
+        result = self.send_keyboard_keys("{TAB}") if sys.platform == 'win32' else \
+            self.press_key_combination_on_mac_browser('key code 48')
+        return result
+
+    def approve_chrome_changed_assets_alert(self, tab_presses=4):
+        """Using the keyboard to click on "keep changes" at chrome's "accept asset change" popup
+
+        :param tab_presses: Number of times to press the tab key before pressing Enter. Set to 4 to support Chrome ver83
+        """
+        logger.debug(f'Pressing {tab_presses} "tab" an an "enter" to click on "keep changes"')
+        for key_press in range(tab_presses):
+            self.press_tab_button()
+            time.sleep(1)  # Time for the button to register correctly in the OS
+        self.press_enter_button()
+        time.sleep(1)  # Time for the button to register correctly in the OS
+
+    def open_a_new_tab(self):
+        """Press the Ctrl + t combination using keyboard keys to open a new tab"""
+        logger.debug('Attempting to open a new tab')
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('^t')
+        else:
+            self.press_key_combination_on_mac_browser('key code 17 using command down')
+
+    def reset_zoom_level(self):
+        """Press the combination ctrl/command + '0' keyboard keys - reset zoom level to 100%"""
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('^0')
+        else:
+            self.press_key_combination_on_mac_browser('key code 82 using command down')
+
+    def decrease_zoom_level(self):
+        """Press the combination ctrl/command + '-' keyboard keys - zoom out"""
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('^{-}')
+        else:
+            self.press_key_combination_on_mac_browser('key code 78 using command down')
+
+    def increase_zoom_level(self):
+        """Press the combination ctrl/command + '+' keyboard keys - zoom in"""
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('^{+}')
+        else:
+            self.press_key_combination_on_mac_browser('key code 69 using command down')
+
+    def set_zoom_level_to_max(self):
+        """Press the combination ctrl/command + '+' keyboard keys 10 times - zoom in all the way"""
+        self.reset_zoom_level()
+        for i in range(10):
+            self.increase_zoom_level()
+
+    def set_zoom_level_to_min(self):
+        """Press the combination ctrl/command + '-' keyboard keys 10 times - zoom out all the way"""
+        self.reset_zoom_level()
+        for i in range(10):
+            self.decrease_zoom_level()
+
+    def press_page_down(self):
+        """Press the page down key"""
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('{PGDN}')
+        else:
+            self.press_key_combination_on_mac_browser('key code 121')
+
+    def press_page_up(self):
+        """Press the page up key"""
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('{PGUP}')
+        else:
+            self.press_key_combination_on_mac_browser('key code 116')
+
+    def press_ctrl_home(self):
+        """Press the combination ctrl/command + home keyboard keys - Scroll to top of the page"""
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('^{HOME}')
+        else:
+            self.press_key_combination_on_mac_browser('key code 115 using command down')
+
+    def press_ctrl_end(self):
+        """Press the combination ctrl/command + end keyboard keys - Scroll to end of the page"""
+        if sys.platform == 'win32':
+            self.send_keyboard_keys('^{END}')
+        else:
+            self.press_key_combination_on_mac_browser('key code 119 using command down')
```

### Comparing `pybenutils-3.1.0/pybenutils/browsers/web_driver.py` & `pybenutils-3.2.2/pybenutils/browsers/web_driver.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import os
-import sys
-from selenium import webdriver
-from selenium.webdriver.remote.webdriver import WebDriver as RemoteWebDriver
-
-
-def attach_to_driver_session(session_id, executor_url, capabilities=None):
-    """
-    Allows to reconnect opened web driver session
-
-    :param session_id: web driver session id
-    :param executor_url: web driver url
-    :param capabilities: browser capabilities
-    :return: web driver which attached to open session
-    """
-
-    # Save the original function, so we can revert our patch
-    org_command_execute = RemoteWebDriver.execute
-
-    def new_command_execute(self, command, params=None):
-        if command == "newSession":
-            # Mock the response
-
-            if not capabilities or capabilities['browserName'].lower() == 'chrome':
-                return {'success': 0, 'value': capabilities, 'sessionId': session_id, 'status': 0}
-            else:
-                return {'success': 0, 'value': capabilities, 'sessionId': session_id}
-        else:
-            return org_command_execute(self, command, params)
-
-    # Patch the function before creating the driver object
-    RemoteWebDriver.execute = new_command_execute
-
-    new_driver = webdriver.Remote(command_executor=executor_url, desired_capabilities=capabilities)
-    new_driver.session_id = session_id
-    new_driver._is_remote = False
-
-    # Replace the patched function with original function
-    RemoteWebDriver.execute = org_command_execute
-
-    return new_driver
-
-
-def close_driver(session_id, driver_url):
-    """
-    Close webdriver and kill its process for the safe side
-    :param session_id:
-    :param driver_url:
-    :return:
-    """
-    try:
-        driver_pid = None
-        driver = attach_to_driver_session(session_id, driver_url)
-        driver_pid = driver.service.process.pid
-    except:
-        pass
-    finally:
-        driver.quit()
-
-    if driver_pid:
-        # if run on MAC
-        if sys.platform != 'win32':
-            os.system('kill -9 {pid}'.format(pid=driver_pid))
-        else:
-            os.system('taskkill /F /PID {pid}'.format(pid=driver_pid))
+import os
+import sys
+from selenium import webdriver
+from selenium.webdriver.remote.webdriver import WebDriver as RemoteWebDriver
+
+
+def attach_to_driver_session(session_id, executor_url, capabilities=None):
+    """
+    Allows to reconnect opened web driver session
+
+    :param session_id: web driver session id
+    :param executor_url: web driver url
+    :param capabilities: browser capabilities
+    :return: web driver which attached to open session
+    """
+
+    # Save the original function, so we can revert our patch
+    org_command_execute = RemoteWebDriver.execute
+
+    def new_command_execute(self, command, params=None):
+        if command == "newSession":
+            # Mock the response
+
+            if not capabilities or capabilities['browserName'].lower() == 'chrome':
+                return {'success': 0, 'value': capabilities, 'sessionId': session_id, 'status': 0}
+            else:
+                return {'success': 0, 'value': capabilities, 'sessionId': session_id}
+        else:
+            return org_command_execute(self, command, params)
+
+    # Patch the function before creating the driver object
+    RemoteWebDriver.execute = new_command_execute
+
+    new_driver = webdriver.Remote(command_executor=executor_url, desired_capabilities=capabilities)
+    new_driver.session_id = session_id
+    new_driver._is_remote = False
+
+    # Replace the patched function with original function
+    RemoteWebDriver.execute = org_command_execute
+
+    return new_driver
+
+
+def close_driver(session_id, driver_url):
+    """
+    Close webdriver and kill its process for the safe side
+    :param session_id:
+    :param driver_url:
+    :return:
+    """
+    try:
+        driver_pid = None
+        driver = attach_to_driver_session(session_id, driver_url)
+        driver_pid = driver.service.process.pid
+    except:
+        pass
+    finally:
+        driver.quit()
+
+    if driver_pid:
+        # if run on MAC
+        if sys.platform != 'win32':
+            os.system('kill -9 {pid}'.format(pid=driver_pid))
+        else:
+            os.system('taskkill /F /PID {pid}'.format(pid=driver_pid))
```

### Comparing `pybenutils-3.1.0/pybenutils/browsers/windows_browsers_keywords.py` & `pybenutils-3.2.2/pybenutils/browsers/windows_browsers_keywords.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-import os
-import sys
-import time
-import psutil
-import subprocess
-from datetime import datetime
-from pybenutils.utils_logger.config_logger import get_logger
-from pybenutils.os_operations.window_operations import get_hwnd_by_class, get_hwnds_by_class, get_window_text
-if sys.platform == 'win32':
-    import win32gui
-    import win32com.client
-    import win32con
-    import win32api
-    import win32process
-
-logger = get_logger()
-
-
-def open_browser_windows(browser: str, arguments=()):
-    """Open selected browser by name
-
-    :param browser: Name of the browser (chrome, chromium, firefox, iexplore, edge)
-    :param arguments: Launch shell arguments
-    :return: Hwnd if browser window exist else None
-    """
-    cmd = []
-    shell = False
-
-    # Setting the program cmd line
-    if browser.lower() in ["iexplore", "ie", "iexplore"]:
-        frame_class = "IEFrame"
-        cmd += ["start", "iexplore.exe"]
-        shell = True
-    elif browser.lower() == "firefox":
-        frame_class = "MozillaWindowClass"
-        cmd += ["start", "firefox.exe"]
-        shell = True
-    elif browser.lower() == "edge":
-        frame_class = "ApplicationFrameWindow"
-        cmd += ["start", "microsoft-edge:"]
-        shell = True
-    elif browser.lower() in ['chrome', 'chromedriver']:
-        frame_class = "Chrome_WidgetWin_1"
-        cmd += ["start", "chrome.exe"]
-        shell = True
-    elif browser == "chromium":
-        frame_class = "Chrome_WidgetWin_1"
-        user_name = os.getenv("USERNAME")
-        chrome_non_xp_path = r"C:\\Users\\" + user_name + "\\AppData\\Local\\Chromium\\Application\\chrome.exe"
-        chromium_xp_path = "C:\\Documents and Settings\\" + user_name + \
-                           "\\Local Settings\\Application Data\\Chromium\\Application\\chrome.exe"
-        if os.path.isfile(chrome_non_xp_path):
-            cmd.append(chrome_non_xp_path)
-        elif os.path.isfile(chromium_xp_path):
-            cmd.append(chromium_xp_path)
-        else:
-            raise Exception('Chromium installation folder could not be located on the machine')
-    elif browser == 'msedge':
-        frame_class = "Chrome_WidgetWin_1"
-        cmd += ["start", "msedge.exe"]
-        shell = True
-    else:
-        raise Exception('Browser {brw} is not yet supported'.format(brw=browser))
-
-    # Adding the args to the cmd
-    if arguments:
-        if type(arguments) in [str, bytes]:
-            cmd.append(arguments)
-        else:
-            cmd += list(arguments)
-
-    # Launching the browser
-    try:
-        sub_process = subprocess.Popen(args=cmd, shell=shell)
-    except WindowsError as ex:
-        logger.warning(f'First attempt to launch browser failed for error: {ex}')
-        time.sleep(20)
-        sub_process = subprocess.Popen(args=cmd, shell=shell)
-
-    time.sleep(5)
-    logger.debug(f'Launch return code: {sub_process.returncode}')
-
-    # Verify the browser window detected and extracting the hwnd
-    hwnd = get_hwnd_by_class(frame_class)
-    logger.debug(f'Checking for an open {frame_class} window for 60 seconds')
-    end_time = time.time() + 60
-    while hwnd is None and time.time() < end_time:
-        time.sleep(1)
-        hwnd = get_hwnd_by_class(frame_class)
-    logger.debug('browser: {browser} hwnd: {hwnd}'.format(browser=browser, hwnd=hwnd))
-    return hwnd
-
-
-def set_browser_url(hwnd: int, text: str):
-    """Open desired browser and ser text into url line and press enter.
-
-    :param hwnd: hwnd of the browser.
-    :param text: The text or the url that will set to browser url line.
-    """
-    win32gui.ShowWindow(hwnd, win32con.SW_MAXIMIZE)
-    window_focus_by_hwnd(hwnd)
-    time.sleep(5)  # Waiting for browser redirection
-    shell = win32com.client.Dispatch("WScript.Shell")
-    shell.SendKeys("^l", 1)
-    time.sleep(1)
-    shell.SendKeys("%d", 1)
-    time.sleep(1)
-    shell.SendKeys(text, 1)
-    time.sleep(4)
-    shell.SendKeys("{ENTER}", 1)
-    time.sleep(4)
-
-
-def get_to_home_page(hwnd: int):
-    """Description: Navigate to home page in the browser
-
-    :param hwnd: Browser's hwnd
-    """
-    shell = win32com.client.Dispatch("WScript.Shell")
-    window_focus_by_hwnd(hwnd)
-    win32api.keybd_event(0xAC, 0, 0, 0)
-    shell.SendKeys("%{HOME}", 1)
-    time.sleep(1)
-    shell.SendKeys("%{HOME}", 1)
-
-
-def close_browser(browser: str) -> bool:
-    """ close browser by name
-
-    :param browser: Browser or process name
-    :return: True if all the browser window closed successfully
-    """
-    if 'chrom' in browser.lower():
-        return close_all_browser_windows_by_class("Chrome_WidgetWin_1")
-    elif 'firefox' in browser.lower():
-        return close_all_browser_windows_by_class("MozillaWindowClass")
-    elif browser.lower() == 'ie' or 'explore' in browser.lower():
-        return close_all_browser_windows_by_class("IEFrame")
-    elif 'safari' in browser.lower():
-        logger.debug('The browser Safari is not installed on Win OS. Skipping.')
-        return True
-    else:
-        logger.warn("Failed to close browser because \"{brw}\" is not yet supported".format(brw=browser))
-
-
-def close_browser_by_hwnd(hwnd: int, handle_multiple_ie_tabs=True) -> bool:
-    """Close browser window by hwnd
-
-    :param hwnd: Hwnd of the browser window
-    :param handle_multiple_ie_tabs: Will attempt to press the close all tabs in IE
-    :return: True if the browser window closed successfully
-    """
-    if not hwnd:
-        logger.debug('No active hwnd was given, returns True')
-        return True
-    try:
-        thread_id, pid = win32process.GetWindowThreadProcessId(hwnd)
-        shell = win32com.client.Dispatch("WScript.Shell")
-        if not window_focus_by_hwnd(hwnd):
-            return True
-        shell.SendKeys("%", 0)
-        time.sleep(1)
-        window_title = get_window_text(hwnd)
-        if not window_title:
-            return True
-        logger.debug("Closing hwnd: {hw}, with title: {title}, time: {t}".format(hw=hwnd, title=window_title,
-                                                                                 t=datetime.now()))
-        # win32gui.SendMessage(hwnd, 0x10, 0, 0)
-        flags = win32con.SMTO_BLOCK + win32con.SMTO_NOTIMEOUTIFNOTHUNG
-        win32gui.SendMessageTimeout(hwnd, 0x10, 0, 0, flags, 1000)
-        time.sleep(2)
-        if handle_multiple_ie_tabs:
-            logger.debug('Checking for "close all tabs" popup')
-            ie_close_all_tabs_window_hwnds = get_hwnds_by_class("#32770")
-            for msg_hwnd in ie_close_all_tabs_window_hwnds:
-                btn_hwnd = win32gui.FindWindowEx(msg_hwnd, 0, "Button", "Close all &tabs")
-                if btn_hwnd > 0:
-                    win32api.PostMessage(btn_hwnd, win32con.WM_LBUTTONDOWN, 0, 0)
-                    time.sleep(0.3)
-                    win32api.PostMessage(btn_hwnd, win32con.WM_LBUTTONUP, 0, 0)
-        end_time = time.time() + 20
-        while psutil.pid_exists(pid) and time.time() < end_time:
-            time.sleep(2)
-        if time.time() > end_time:
-            logger.error('Failed to close window {title} with pid {pid}'.format(title=window_title, pid=pid))
-            return False
-        return True
-    except Exception as ex:
-        logger.error(f'Got an error when trying to close a window with error: {ex}')
-        return False
-
-
-def close_browser_by_class(class_name: str) -> bool:
-    """ close browser by class name
-
-    :param class_name: browser class name
-    :return: True if all the browser window closed successfully
-    """
-    handle_multiple_ie_tabs = class_name == 'IEFrame'
-    return close_browser_by_hwnd(hwnd=get_hwnd_by_class(class_name), handle_multiple_ie_tabs=handle_multiple_ie_tabs)
-
-
-def close_all_browser_windows_by_class(class_name: str) -> bool:
-    """ close browser by class name
-
-    :param class_name: browser class name
-    :return: True if all the browser window closed successfully
-    """
-    hwnd_list = get_hwnds_by_class(class_name)
-    closed_all_windows = True
-    handle_multiple_ie_tabs = class_name == 'IEFrame'
-    for hwnd in hwnd_list:
-        if not close_browser_by_hwnd(hwnd=hwnd, handle_multiple_ie_tabs=handle_multiple_ie_tabs):
-            closed_all_windows = False
-    return closed_all_windows
-
-
-def window_set_foreground(hwnd):
-    """Bring a window to the foreground and activate it.
-
-    :param hwnd: Hwnd of window
-    """
-    try:
-        win32gui.SetForegroundWindow(hwnd)
-        win32gui.BringWindowToTop(hwnd)
-        win32gui.SetActiveWindow(hwnd)
-    except Exception as ex:
-        logger.warning(ex)
-
-
-def key_down_and_key_up(hwnd, key):
-    """Send Virtual-Key to window specific
-
-    :param hwnd: window to send key
-    :param key: Hexadecimal key
-    """
-    rc = win32api.PostMessage(hwnd, win32con.WM_KEYDOWN, key, 0)
-    if rc == 0:
-        raise AssertionError("Down click failed")
-    rc = win32api.PostMessage(hwnd, win32con.WM_KEYUP, key, 0)
-    if rc == 0:
-        raise AssertionError("Up click failed")
-
-
-def window_focus_by_hwnd(hwnd):
-    """Set focus to window by hwnd
-
-    :param hwnd: Window Hwnd
-    """
-    try:
-        window_set_foreground(hwnd)
-        key_down_and_key_up(hwnd, 0x12)
-        logger.debug("window_focus_by_hwnd")
-        window_set_foreground(hwnd)
-    except Exception as ex:
-        logger.warning(ex)
+import os
+import sys
+import time
+import psutil
+import subprocess
+from datetime import datetime
+from pybenutils.utils_logger.config_logger import get_logger
+from pybenutils.os_operations.window_operations import get_hwnd_by_class, get_hwnds_by_class, get_window_text
+if sys.platform == 'win32':
+    import win32gui
+    import win32com.client
+    import win32con
+    import win32api
+    import win32process
+
+logger = get_logger()
+
+
+def open_browser_windows(browser: str, arguments=()):
+    """Open selected browser by name
+
+    :param browser: Name of the browser (chrome, chromium, firefox, iexplore, edge)
+    :param arguments: Launch shell arguments
+    :return: Hwnd if browser window exist else None
+    """
+    cmd = []
+    shell = False
+
+    # Setting the program cmd line
+    if browser.lower() in ["iexplore", "ie", "iexplore"]:
+        frame_class = "IEFrame"
+        cmd += ["start", "iexplore.exe"]
+        shell = True
+    elif browser.lower() == "firefox":
+        frame_class = "MozillaWindowClass"
+        cmd += ["start", "firefox.exe"]
+        shell = True
+    elif browser.lower() == "edge":
+        frame_class = "ApplicationFrameWindow"
+        cmd += ["start", "microsoft-edge:"]
+        shell = True
+    elif browser.lower() in ['chrome', 'chromedriver']:
+        frame_class = "Chrome_WidgetWin_1"
+        cmd += ["start", "chrome.exe"]
+        shell = True
+    elif browser == "chromium":
+        frame_class = "Chrome_WidgetWin_1"
+        user_name = os.getenv("USERNAME")
+        chrome_non_xp_path = r"C:\\Users\\" + user_name + "\\AppData\\Local\\Chromium\\Application\\chrome.exe"
+        chromium_xp_path = "C:\\Documents and Settings\\" + user_name + \
+                           "\\Local Settings\\Application Data\\Chromium\\Application\\chrome.exe"
+        if os.path.isfile(chrome_non_xp_path):
+            cmd.append(chrome_non_xp_path)
+        elif os.path.isfile(chromium_xp_path):
+            cmd.append(chromium_xp_path)
+        else:
+            raise Exception('Chromium installation folder could not be located on the machine')
+    elif browser == 'msedge':
+        frame_class = "Chrome_WidgetWin_1"
+        cmd += ["start", "msedge.exe"]
+        shell = True
+    else:
+        raise Exception('Browser {brw} is not yet supported'.format(brw=browser))
+
+    # Adding the args to the cmd
+    if arguments:
+        if type(arguments) in [str, bytes]:
+            cmd.append(arguments)
+        else:
+            cmd += list(arguments)
+
+    # Launching the browser
+    try:
+        sub_process = subprocess.Popen(args=cmd, shell=shell)
+    except WindowsError as ex:
+        logger.warning(f'First attempt to launch browser failed for error: {ex}')
+        time.sleep(20)
+        sub_process = subprocess.Popen(args=cmd, shell=shell)
+
+    time.sleep(5)
+    logger.debug(f'Launch return code: {sub_process.returncode}')
+
+    # Verify the browser window detected and extracting the hwnd
+    hwnd = get_hwnd_by_class(frame_class)
+    logger.debug(f'Checking for an open {frame_class} window for 60 seconds')
+    end_time = time.time() + 60
+    while hwnd is None and time.time() < end_time:
+        time.sleep(1)
+        hwnd = get_hwnd_by_class(frame_class)
+    logger.debug('browser: {browser} hwnd: {hwnd}'.format(browser=browser, hwnd=hwnd))
+    return hwnd
+
+
+def set_browser_url(hwnd: int, text: str):
+    """Open desired browser and ser text into url line and press enter.
+
+    :param hwnd: hwnd of the browser.
+    :param text: The text or the url that will set to browser url line.
+    """
+    win32gui.ShowWindow(hwnd, win32con.SW_MAXIMIZE)
+    window_focus_by_hwnd(hwnd)
+    time.sleep(5)  # Waiting for browser redirection
+    shell = win32com.client.Dispatch("WScript.Shell")
+    shell.SendKeys("^l", 1)
+    time.sleep(1)
+    shell.SendKeys("%d", 1)
+    time.sleep(1)
+    shell.SendKeys(text, 1)
+    time.sleep(4)
+    shell.SendKeys("{ENTER}", 1)
+    time.sleep(4)
+
+
+def get_to_home_page(hwnd: int):
+    """Description: Navigate to home page in the browser
+
+    :param hwnd: Browser's hwnd
+    """
+    shell = win32com.client.Dispatch("WScript.Shell")
+    window_focus_by_hwnd(hwnd)
+    win32api.keybd_event(0xAC, 0, 0, 0)
+    shell.SendKeys("%{HOME}", 1)
+    time.sleep(1)
+    shell.SendKeys("%{HOME}", 1)
+
+
+def close_browser(browser: str) -> bool:
+    """ close browser by name
+
+    :param browser: Browser or process name
+    :return: True if all the browser window closed successfully
+    """
+    if 'chrom' in browser.lower():
+        return close_all_browser_windows_by_class("Chrome_WidgetWin_1")
+    elif 'firefox' in browser.lower():
+        return close_all_browser_windows_by_class("MozillaWindowClass")
+    elif browser.lower() == 'ie' or 'explore' in browser.lower():
+        return close_all_browser_windows_by_class("IEFrame")
+    elif 'safari' in browser.lower():
+        logger.debug('The browser Safari is not installed on Win OS. Skipping.')
+        return True
+    else:
+        logger.warn("Failed to close browser because \"{brw}\" is not yet supported".format(brw=browser))
+
+
+def close_browser_by_hwnd(hwnd: int, handle_multiple_ie_tabs=True) -> bool:
+    """Close browser window by hwnd
+
+    :param hwnd: Hwnd of the browser window
+    :param handle_multiple_ie_tabs: Will attempt to press the close all tabs in IE
+    :return: True if the browser window closed successfully
+    """
+    if not hwnd:
+        logger.debug('No active hwnd was given, returns True')
+        return True
+    try:
+        thread_id, pid = win32process.GetWindowThreadProcessId(hwnd)
+        shell = win32com.client.Dispatch("WScript.Shell")
+        if not window_focus_by_hwnd(hwnd):
+            return True
+        shell.SendKeys("%", 0)
+        time.sleep(1)
+        window_title = get_window_text(hwnd)
+        if not window_title:
+            return True
+        logger.debug("Closing hwnd: {hw}, with title: {title}, time: {t}".format(hw=hwnd, title=window_title,
+                                                                                 t=datetime.now()))
+        # win32gui.SendMessage(hwnd, 0x10, 0, 0)
+        flags = win32con.SMTO_BLOCK + win32con.SMTO_NOTIMEOUTIFNOTHUNG
+        win32gui.SendMessageTimeout(hwnd, 0x10, 0, 0, flags, 1000)
+        time.sleep(2)
+        if handle_multiple_ie_tabs:
+            logger.debug('Checking for "close all tabs" popup')
+            ie_close_all_tabs_window_hwnds = get_hwnds_by_class("#32770")
+            for msg_hwnd in ie_close_all_tabs_window_hwnds:
+                btn_hwnd = win32gui.FindWindowEx(msg_hwnd, 0, "Button", "Close all &tabs")
+                if btn_hwnd > 0:
+                    win32api.PostMessage(btn_hwnd, win32con.WM_LBUTTONDOWN, 0, 0)
+                    time.sleep(0.3)
+                    win32api.PostMessage(btn_hwnd, win32con.WM_LBUTTONUP, 0, 0)
+        end_time = time.time() + 20
+        while psutil.pid_exists(pid) and time.time() < end_time:
+            time.sleep(2)
+        if time.time() > end_time:
+            logger.error('Failed to close window {title} with pid {pid}'.format(title=window_title, pid=pid))
+            return False
+        return True
+    except Exception as ex:
+        logger.error(f'Got an error when trying to close a window with error: {ex}')
+        return False
+
+
+def close_browser_by_class(class_name: str) -> bool:
+    """ close browser by class name
+
+    :param class_name: browser class name
+    :return: True if all the browser window closed successfully
+    """
+    handle_multiple_ie_tabs = class_name == 'IEFrame'
+    return close_browser_by_hwnd(hwnd=get_hwnd_by_class(class_name), handle_multiple_ie_tabs=handle_multiple_ie_tabs)
+
+
+def close_all_browser_windows_by_class(class_name: str) -> bool:
+    """ close browser by class name
+
+    :param class_name: browser class name
+    :return: True if all the browser window closed successfully
+    """
+    hwnd_list = get_hwnds_by_class(class_name)
+    closed_all_windows = True
+    handle_multiple_ie_tabs = class_name == 'IEFrame'
+    for hwnd in hwnd_list:
+        if not close_browser_by_hwnd(hwnd=hwnd, handle_multiple_ie_tabs=handle_multiple_ie_tabs):
+            closed_all_windows = False
+    return closed_all_windows
+
+
+def window_set_foreground(hwnd):
+    """Bring a window to the foreground and activate it.
+
+    :param hwnd: Hwnd of window
+    """
+    try:
+        win32gui.SetForegroundWindow(hwnd)
+        win32gui.BringWindowToTop(hwnd)
+        win32gui.SetActiveWindow(hwnd)
+    except Exception as ex:
+        logger.warning(ex)
+
+
+def key_down_and_key_up(hwnd, key):
+    """Send Virtual-Key to window specific
+
+    :param hwnd: window to send key
+    :param key: Hexadecimal key
+    """
+    rc = win32api.PostMessage(hwnd, win32con.WM_KEYDOWN, key, 0)
+    if rc == 0:
+        raise AssertionError("Down click failed")
+    rc = win32api.PostMessage(hwnd, win32con.WM_KEYUP, key, 0)
+    if rc == 0:
+        raise AssertionError("Up click failed")
+
+
+def window_focus_by_hwnd(hwnd):
+    """Set focus to window by hwnd
+
+    :param hwnd: Window Hwnd
+    """
+    try:
+        window_set_foreground(hwnd)
+        key_down_and_key_up(hwnd, 0x12)
+        logger.debug("window_focus_by_hwnd")
+        window_set_foreground(hwnd)
+    except Exception as ex:
+        logger.warning(ex)
```

### Comparing `pybenutils-3.1.0/pybenutils/network/download_manager.py` & `pybenutils-3.2.2/pybenutils/network/download_manager.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import os
-import time
-import requests
-from urllib.parse import urlparse
-from pybenutils.utils_logger.config_logger import get_logger
-
-logger = get_logger()
-
-
-def download_url(url: str, file_path='', attempts=2, raise_failure=True, verify_ssl=True):
-    """Downloads a URL content into a file (with large file support by streaming)
-
-    :param url: URL to download_url
-    :param file_path: Local file name to contain the data downloaded
-    :param attempts: Number of attempts
-    :param raise_failure: Raise Exception on failure
-    :param verify_ssl: Verify the domain ssl
-    :return: New file path. Empty string if the download_url failed
-    """
-    if not file_path:
-        file_path = os.path.realpath(os.path.basename(url))
-    logger.info(f'Downloading {url} content to {file_path}')
-    url_sections = urlparse(url)
-    if not url_sections.scheme:
-        logger.debug('The given url is missing a scheme. Adding http scheme')
-        url = f'http://{url}'
-        logger.debug(f'New url: {url}')
-    last_exception = None
-    for attempt in range(1, attempts+1):
-        try:
-            if attempt > 1:
-                time.sleep(10)  # 10 seconds wait time between downloads
-            with requests.get(url, stream=True, verify=verify_ssl) as response:
-                logger.debug(f'Response status code: {response.status_code}')
-                response.raise_for_status()
-                with open(file_path, 'wb') as out_file:
-                    for chunk in response.iter_content(chunk_size=1024*1024):  # 1MB chunks
-                        out_file.write(chunk)
-                logger.info('Download finished successfully')
-                return file_path
-        except Exception as ex:
-            logger.error(f'Attempt #{attempt} failed with error: {ex}')
-            last_exception = ex
-    if raise_failure:
-        raise last_exception
-    return ''
+import os
+import time
+import requests
+from urllib.parse import urlparse
+from pybenutils.utils_logger.config_logger import get_logger
+
+logger = get_logger()
+
+
+def download_url(url: str, file_path='', attempts=2, raise_failure=True, verify_ssl=True):
+    """Downloads a URL content into a file (with large file support by streaming)
+
+    :param url: URL to download_url
+    :param file_path: Local file name to contain the data downloaded
+    :param attempts: Number of attempts
+    :param raise_failure: Raise Exception on failure
+    :param verify_ssl: Verify the domain ssl
+    :return: New file path. Empty string if the download_url failed
+    """
+    if not file_path:
+        file_path = os.path.realpath(os.path.basename(url))
+    logger.info(f'Downloading {url} content to {file_path}')
+    url_sections = urlparse(url)
+    if not url_sections.scheme:
+        logger.debug('The given url is missing a scheme. Adding http scheme')
+        url = f'http://{url}'
+        logger.debug(f'New url: {url}')
+    last_exception = None
+    for attempt in range(1, attempts+1):
+        try:
+            if attempt > 1:
+                time.sleep(10)  # 10 seconds wait time between downloads
+            with requests.get(url, stream=True, verify=verify_ssl) as response:
+                logger.debug(f'Response status code: {response.status_code}')
+                response.raise_for_status()
+                with open(file_path, 'wb') as out_file:
+                    for chunk in response.iter_content(chunk_size=1024*1024):  # 1MB chunks
+                        out_file.write(chunk)
+                logger.info('Download finished successfully')
+                return file_path
+        except Exception as ex:
+            logger.error(f'Attempt #{attempt} failed with error: {ex}')
+            last_exception = ex
+    if raise_failure:
+        raise last_exception
+    return ''
```

### Comparing `pybenutils-3.1.0/pybenutils/network/http_cert_info.py` & `pybenutils-3.2.2/pybenutils/network/http_cert_info.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from OpenSSL import SSL
-from cryptography import x509
-from cryptography.x509.oid import NameOID
-import idna
-from collections import namedtuple
-# noinspection PyPackageRequirements
-import socks  # pysocks
-
-HostInfo = namedtuple(field_names='cert hostname peername', typename='HostInfo')
-
-
-class HttpDomainCertificateInfo(dict):
-    def __init__(self, host_name: str, port: int, proxy_ip='', proxy_port=8080):
-        super().__init__()
-        self.hostinfo = self.get_certificate(host_name, port, proxy_ip, proxy_port)
-        self.update({
-            'hostname': self.hostinfo.hostname,
-            'peer_name': self.hostinfo.peername,
-            'common_name': self.get_common_name(),
-            'SAN': self.get_alt_names(),
-            'issuer': self.get_issuer(),
-            'not_before': self.hostinfo.cert.not_valid_before,
-            'not_after': self.hostinfo.cert.not_valid_after
-        })
-
-    @staticmethod
-    def get_certificate(host_name, port, proxy_ip='', proxy_port=8080):
-        sock = socks.socksocket()  # Same API as socket.socket in the standard lib
-        if proxy_ip:
-            sock.set_proxy(socks.HTTP, proxy_ip, proxy_port)
-
-        hostname_idna = idna.encode(host_name)
-        # sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        # sock = socket.socket()
-
-        sock.connect((host_name, port))
-        peer_name = sock.getpeername()
-        ctx = SSL.Context(SSL.SSLv23_METHOD)  # most compatible
-        ctx.check_hostname = False
-        ctx.verify_mode = SSL.VERIFY_NONE
-
-        sock_ssl = SSL.Connection(ctx, sock)
-        sock_ssl.set_connect_state()
-        sock_ssl.set_tlsext_host_name(hostname_idna)
-        sock_ssl.do_handshake()
-        cert = sock_ssl.get_peer_certificate()
-        crypto_cert = cert.to_cryptography()
-        sock_ssl.close()
-        sock.close()
-
-        return HostInfo(cert=crypto_cert, peername=peer_name, hostname=host_name)
-
-    def get_alt_names(self):
-        try:
-            ext = self.hostinfo.cert.extensions.get_extension_for_class(x509.SubjectAlternativeName)
-            return ext.value.get_values_for_type(x509.DNSName)
-        except x509.ExtensionNotFound:
-            return None
-
-    def get_common_name(self):
-        try:
-            names = self.hostinfo.cert.subject.get_attributes_for_oid(NameOID.COMMON_NAME)
-            return names[0].value
-        except x509.ExtensionNotFound:
-            return None
-
-    def get_issuer(self):
-        try:
-            names = self.hostinfo.cert.issuer.get_attributes_for_oid(NameOID.COMMON_NAME)
-            return names[0].value
-        except x509.ExtensionNotFound:
-            return None
-
-    def get_basic_info(self):
-        s = '''» {hostname} « … {peername}
-        \tcommonName: {commonname}
-        \tSAN: {SAN}
-        \tissuer: {issuer}
-        \tnotBefore: {notbefore}
-        \tnotAfter:  {notafter}
-        '''.format(
-            hostname=self.hostinfo.hostname,
-            peername=self.hostinfo.peername,
-            commonname=self.get_common_name(),
-            SAN=self.get_alt_names(),
-            issuer=self.get_issuer(),
-            notbefore=self.hostinfo.cert.not_valid_before,
-            notafter=self.hostinfo.cert.not_valid_after
-        )
-        return s
+from OpenSSL import SSL
+from cryptography import x509
+from cryptography.x509.oid import NameOID
+import idna
+from collections import namedtuple
+# noinspection PyPackageRequirements
+import socks  # pysocks
+
+HostInfo = namedtuple(field_names='cert hostname peername', typename='HostInfo')
+
+
+class HttpDomainCertificateInfo(dict):
+    def __init__(self, host_name: str, port: int, proxy_ip='', proxy_port=8080):
+        super().__init__()
+        self.hostinfo = self.get_certificate(host_name, port, proxy_ip, proxy_port)
+        self.update({
+            'hostname': self.hostinfo.hostname,
+            'peer_name': self.hostinfo.peername,
+            'common_name': self.get_common_name(),
+            'SAN': self.get_alt_names(),
+            'issuer': self.get_issuer(),
+            'not_before': self.hostinfo.cert.not_valid_before,
+            'not_after': self.hostinfo.cert.not_valid_after
+        })
+
+    @staticmethod
+    def get_certificate(host_name, port, proxy_ip='', proxy_port=8080):
+        sock = socks.socksocket()  # Same API as socket.socket in the standard lib
+        if proxy_ip:
+            sock.set_proxy(socks.HTTP, proxy_ip, proxy_port)
+
+        hostname_idna = idna.encode(host_name)
+        # sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        # sock = socket.socket()
+
+        sock.connect((host_name, port))
+        peer_name = sock.getpeername()
+        ctx = SSL.Context(SSL.SSLv23_METHOD)  # most compatible
+        ctx.check_hostname = False
+        ctx.verify_mode = SSL.VERIFY_NONE
+
+        sock_ssl = SSL.Connection(ctx, sock)
+        sock_ssl.set_connect_state()
+        sock_ssl.set_tlsext_host_name(hostname_idna)
+        sock_ssl.do_handshake()
+        cert = sock_ssl.get_peer_certificate()
+        crypto_cert = cert.to_cryptography()
+        sock_ssl.close()
+        sock.close()
+
+        return HostInfo(cert=crypto_cert, peername=peer_name, hostname=host_name)
+
+    def get_alt_names(self):
+        try:
+            ext = self.hostinfo.cert.extensions.get_extension_for_class(x509.SubjectAlternativeName)
+            return ext.value.get_values_for_type(x509.DNSName)
+        except x509.ExtensionNotFound:
+            return None
+
+    def get_common_name(self):
+        try:
+            names = self.hostinfo.cert.subject.get_attributes_for_oid(NameOID.COMMON_NAME)
+            return names[0].value
+        except x509.ExtensionNotFound:
+            return None
+
+    def get_issuer(self):
+        try:
+            names = self.hostinfo.cert.issuer.get_attributes_for_oid(NameOID.COMMON_NAME)
+            return names[0].value
+        except x509.ExtensionNotFound:
+            return None
+
+    def get_basic_info(self):
+        s = '''» {hostname} « … {peername}
+        \tcommonName: {commonname}
+        \tSAN: {SAN}
+        \tissuer: {issuer}
+        \tnotBefore: {notbefore}
+        \tnotAfter:  {notafter}
+        '''.format(
+            hostname=self.hostinfo.hostname,
+            peername=self.hostinfo.peername,
+            commonname=self.get_common_name(),
+            SAN=self.get_alt_names(),
+            issuer=self.get_issuer(),
+            notbefore=self.hostinfo.cert.not_valid_before,
+            notafter=self.hostinfo.cert.not_valid_after
+        )
+        return s
```

### Comparing `pybenutils-3.1.0/pybenutils/network/s3_bucket_cls.py` & `pybenutils-3.2.2/pybenutils/network/s3_bucket_cls.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-import os
-import time
-import posixpath
-import threading
-from glob import glob
-from boto.s3.key import Key
-from typing import List, Union
-from boto import log as boto_log
-from pybenutils.utils_logger.config_logger import get_logger
-from boto.exception import S3ResponseError
-from boto.s3.connection import S3Connection
-from multiprocessing.dummy import Pool as ThreadPool
-from pybenutils.os_operations.files_and_directories import get_files_in_folder
-
-logger = get_logger()
-lock = threading.Lock()
-boto_log.setLevel('WARNING')  # Added because boto prints passwords
-
-
-class S3BucketManager(object):
-    """A manager that helps with upload and download to/from s3 bucket"""
-    DOWNLOAD_THREADS_NUM = 5
-    UPLOAD_THREADS_NUM = 5
-    DOWNLOAD_ATTEMPTS = 3
-
-    def __init__(self, key, password, bucket_name):
-        """
-        :param key: Aws key
-        :param password:  Aws password
-        :param bucket_name: Bucket name
-        """
-        self.conn = S3Connection(aws_access_key_id=key, aws_secret_access_key=password)
-        self.bucket_name = bucket_name
-        try:
-            self.bucket_obj = self.conn.get_bucket(self.bucket_name)
-        except S3ResponseError as conn_err:
-            if conn_err.message.lower() == 'access denied':
-                raise AssertionError(f'Access denied for bucket "{bucket_name}": {str(conn_err)}')
-            else:
-                raise conn_err
-
-    def upload_file(self, source, destination, public=True):
-        """Upload source to s3 server.
-         The uploaded file path will be '{}/{}'.format(destination, os.path.basename(source))
-
-        :param source: Path of the local file to upload
-        :param destination: Destination dir
-        :param public: If we need to set the upload as public
-        :return: Uploaded file path within the bucket
-        """
-        attempts = S3BucketManager.DOWNLOAD_ATTEMPTS
-        for attempt in range(attempts):
-            try:
-                logger.info(f"upload from {source} to {destination}")
-                k = self.bucket_obj.new_key(posixpath.join(destination, os.path.basename(source.strip())))
-                k.set_contents_from_filename(source)
-                if public:
-                    k.make_public()
-                uploaded_file_url = 'http://{bucket}.s3.amazonaws.com/{key}'.format(bucket=self.bucket_name, key=k.key)
-                logger.info('Successfully uploaded to {url}'.format(url=uploaded_file_url))
-                return uploaded_file_url
-            except Exception as ex:
-                logger.error('Attempt {num}/{max_attempts} failed with error:{err}'.format(
-                    num=attempt + 1, max_attempts=attempts, err=str(ex)))
-                if attempt + 1 < attempts:
-                    time.sleep(10)
-                else:
-                    raise ex
-
-    def upload(self, source_list: Union[str, List[str]],
-               destination: str,
-               public=True,
-               exclude_list: Union[str, List[str]] = '') -> List[str]:
-        """An improved method to upload multiple sources to Amazon s3 server. The list can contain a file path to upload
-         or a folder to upload all its content. If the source is a file, it will be uploaded directly to the s3
-         destination dir. If the source is a folder, its content will be uploaded with the same hierarchical order
-         (without the root dir) in the s3 destination dir.
-
-        :param source_list: A list sources to upload (Files & Folders). Supports glob string patterns
-        :param destination: Destination folder (Inside the bucket)
-        :param public: Adds read permission to Everyone for the file uploaded
-        :param exclude_list: List of paths to exclude (Files & Folders). Supports glob string patterns
-        :return: A list of urls pointing to the uploaded files
-        """
-
-        def _upload_file_wrapper(tup):
-            """A wrapper to self.upload_file_to_s3 that allows to use it in pool.map. Takes a tuple of variables and
-             invokes self.upload_file_to_s3 with them as single args
-
-            :param tup: a tuple of argument
-            :return: the result of self.upload_file_to_s3 with the given input
-            """
-            return self.upload_file(*tup)
-
-        source_list = source_list if type(source_list) == list else [source_list]
-        if exclude_list:
-            exclude_list = exclude_list if type(exclude_list) == list else [exclude_list]
-        else:
-            exclude_list = []  # Handling cases of empty / None exclude list
-
-        # Building the extended files exclude list
-        extended_exclude_list = []
-        for exclude_item in exclude_list:
-            for source in glob(exclude_item):
-                source = os.path.realpath(source)
-                extended_exclude_list.append(source)
-                if os.path.isdir(source):
-                    upload_list_from_folder = get_files_in_folder(source)
-                    for file_path in upload_list_from_folder:
-                        extended_exclude_list.append(file_path)
-
-        # Building the upload details list - excluding paths as needed
-        upload_details_list = []
-        for unfiltered_source in source_list:
-            for source in glob(unfiltered_source):
-                source = os.path.realpath(source)
-                if os.path.isfile(source):
-                    if source not in extended_exclude_list:
-                        upload_details = (source, destination, public)
-                        upload_details_list.append(upload_details)
-                elif os.path.isdir(source):
-                    upload_list_from_folder = get_files_in_folder(source)
-                    for file_path in upload_list_from_folder:
-                        if file_path in extended_exclude_list:
-                            continue
-                        relative_path = os.path.dirname(file_path.split(source)[-1])
-                        destination = '{base}{rel}'.format(base=destination, rel=relative_path.replace('\\', '/'))
-                        upload_details = (file_path, destination, public)
-                        upload_details_list.append(upload_details)
-                else:
-                    logger.info('Could not validate source for {source}. Skipping...'.format(source=source))
-
-        pool = ThreadPool(S3BucketManager.UPLOAD_THREADS_NUM)
-        uploaded_files_list = pool.map(_upload_file_wrapper, upload_details_list)
-        pool.close()
-        pool.join()
-        return uploaded_files_list
-
-    def get_s3_folder_content(self, s3_folder):
-        """Returns the relative paths of all the objects in the given s3 folder, files and directories, recursively.
-         The paths includes the root dir (s3_folder input). Directories ends with '/'
-
-        :param s3_folder: S3 folder to examine
-        :return: A list of relative paths of the objects insides the input folder
-        """
-        return [key.key for key in self.bucket_obj.list(prefix=s3_folder)]
-
-    def download_file(self, source, destination):
-        """Download source from s3 server. if destination is a file, the download file path will be the same. If it's a
-         folder, the download file path will be '{}/{}'.format(destination, os.path.basename(source))
-
-        :param source: Relative path of the file inside the bucket
-        :param destination: Local path of the directory or file the file should be downloaded to
-        """
-        if '.' in destination[-5:]:  # the destination is a file path and not a folder
-            dest_file_path = destination
-        else:
-            dest_file_path = os.path.join(destination, os.path.basename(source))
-        logger.info(f'Download file from "{source}" to "{dest_file_path}"')
-
-        destination_dir = os.path.dirname(dest_file_path)
-        if not destination_dir:
-            destination_dir = os.getcwd()
-        with lock:
-            if not os.path.exists(destination_dir):
-                os.makedirs(destination_dir)
-        if not os.path.exists(destination_dir):
-            return
-
-        k = Key(self.bucket_obj)
-        k.key = source
-        k.get_contents_to_filename(dest_file_path)
-        return dest_file_path
-
-    def download(self, source_list, destination):
-        """Download folder content from s3 server. The list can contain an s3 folder name or an s3 file relative path.
-        If the source is a folder, its content will be downloaded with the same hierarchical order (without the root
-        dir) in the destination dir. if the source is a file, it will be downloaded directly to the destination dir
-
-        :param source_list: List of s3 sources, files and folders
-        :param destination: Destination dir
-        :return: A list of the newly added files paths
-        """
-
-        def _download_file_wrapper(tup):
-            """A wrapper to self.download_file_from_s3 that allows to use it in pool.map. Takes a tuple of variables
-             and invokes self.download_file_from_s3 with them as single args
-
-            :param tup: Tuple of argument
-            :return: The result of self.download_file_from_s3 with the given input
-            """
-            return self.download_file(*tup)
-
-        source_list = source_list if isinstance(source_list, list) else [source_list]
-        download_details_list = []
-        for source in source_list:
-            source = source.strip('/')
-            k = self.bucket_obj.get_key(source)  # check if source is a file (s3 key) or a folder
-            if k:
-                download_details_list.append((source, destination))
-            else:  # source is a folder
-                for key in self.bucket_obj.list(prefix=source):
-                    relative_url = key.key
-                    sub_folder = os.path.dirname(relative_url).split(source)[-1].strip('/')
-                    destination = os.path.join(destination, sub_folder) if sub_folder else destination
-                    download_details_list.append((relative_url, destination))
-
-        pool = ThreadPool(S3BucketManager.DOWNLOAD_THREADS_NUM)
-        download_list = pool.map(_download_file_wrapper, download_details_list)
-        pool.close()
-        pool.join()
-        return download_list
-
-    def delete_key_from_bucket(self, key_to_delete):
-        """Delete file or folder from given s3 path
-
-        :param key_to_delete: Folder or file path to delete
-        """
-        self.bucket_obj.delete_key(key_to_delete)
+import os
+import time
+import posixpath
+import threading
+from glob import glob
+from boto.s3.key import Key
+from typing import List, Union
+from boto import log as boto_log
+from pybenutils.utils_logger.config_logger import get_logger
+from boto.exception import S3ResponseError
+from boto.s3.connection import S3Connection
+from multiprocessing.dummy import Pool as ThreadPool
+from pybenutils.os_operations.files_and_directories import get_files_in_folder
+
+logger = get_logger()
+lock = threading.Lock()
+boto_log.setLevel('WARNING')  # Added because boto prints passwords
+
+
+class S3BucketManager(object):
+    """A manager that helps with upload and download to/from s3 bucket"""
+    DOWNLOAD_THREADS_NUM = 5
+    UPLOAD_THREADS_NUM = 5
+    DOWNLOAD_ATTEMPTS = 3
+
+    def __init__(self, key, password, bucket_name):
+        """
+        :param key: Aws key
+        :param password:  Aws password
+        :param bucket_name: Bucket name
+        """
+        self.conn = S3Connection(aws_access_key_id=key, aws_secret_access_key=password)
+        self.bucket_name = bucket_name
+        try:
+            self.bucket_obj = self.conn.get_bucket(self.bucket_name)
+        except S3ResponseError as conn_err:
+            if conn_err.message.lower() == 'access denied':
+                raise AssertionError(f'Access denied for bucket "{bucket_name}": {str(conn_err)}')
+            else:
+                raise conn_err
+
+    def upload_file(self, source, destination, public=True):
+        """Upload source to s3 server.
+         The uploaded file path will be '{}/{}'.format(destination, os.path.basename(source))
+
+        :param source: Path of the local file to upload
+        :param destination: Destination dir
+        :param public: If we need to set the upload as public
+        :return: Uploaded file path within the bucket
+        """
+        attempts = S3BucketManager.DOWNLOAD_ATTEMPTS
+        for attempt in range(attempts):
+            try:
+                logger.info(f"upload from {source} to {destination}")
+                k = self.bucket_obj.new_key(posixpath.join(destination, os.path.basename(source.strip())))
+                k.set_contents_from_filename(source)
+                if public:
+                    k.make_public()
+                uploaded_file_url = 'http://{bucket}.s3.amazonaws.com/{key}'.format(bucket=self.bucket_name, key=k.key)
+                logger.info('Successfully uploaded to {url}'.format(url=uploaded_file_url))
+                return uploaded_file_url
+            except Exception as ex:
+                logger.error('Attempt {num}/{max_attempts} failed with error:{err}'.format(
+                    num=attempt + 1, max_attempts=attempts, err=str(ex)))
+                if attempt + 1 < attempts:
+                    time.sleep(10)
+                else:
+                    raise ex
+
+    def upload(self, source_list: Union[str, List[str]],
+               destination: str,
+               public=True,
+               exclude_list: Union[str, List[str]] = '') -> List[str]:
+        """An improved method to upload multiple sources to Amazon s3 server. The list can contain a file path to upload
+         or a folder to upload all its content. If the source is a file, it will be uploaded directly to the s3
+         destination dir. If the source is a folder, its content will be uploaded with the same hierarchical order
+         (without the root dir) in the s3 destination dir.
+
+        :param source_list: A list sources to upload (Files & Folders). Supports glob string patterns
+        :param destination: Destination folder (Inside the bucket)
+        :param public: Adds read permission to Everyone for the file uploaded
+        :param exclude_list: List of paths to exclude (Files & Folders). Supports glob string patterns
+        :return: A list of urls pointing to the uploaded files
+        """
+
+        def _upload_file_wrapper(tup):
+            """A wrapper to self.upload_file_to_s3 that allows to use it in pool.map. Takes a tuple of variables and
+             invokes self.upload_file_to_s3 with them as single args
+
+            :param tup: a tuple of argument
+            :return: the result of self.upload_file_to_s3 with the given input
+            """
+            return self.upload_file(*tup)
+
+        source_list = source_list if type(source_list) == list else [source_list]
+        if exclude_list:
+            exclude_list = exclude_list if type(exclude_list) == list else [exclude_list]
+        else:
+            exclude_list = []  # Handling cases of empty / None exclude list
+
+        # Building the extended files exclude list
+        extended_exclude_list = []
+        for exclude_item in exclude_list:
+            for source in glob(exclude_item):
+                source = os.path.realpath(source)
+                extended_exclude_list.append(source)
+                if os.path.isdir(source):
+                    upload_list_from_folder = get_files_in_folder(source)
+                    for file_path in upload_list_from_folder:
+                        extended_exclude_list.append(file_path)
+
+        # Building the upload details list - excluding paths as needed
+        upload_details_list = []
+        for unfiltered_source in source_list:
+            for source in glob(unfiltered_source):
+                source = os.path.realpath(source)
+                if os.path.isfile(source):
+                    if source not in extended_exclude_list:
+                        upload_details = (source, destination, public)
+                        upload_details_list.append(upload_details)
+                elif os.path.isdir(source):
+                    upload_list_from_folder = get_files_in_folder(source)
+                    for file_path in upload_list_from_folder:
+                        if file_path in extended_exclude_list:
+                            continue
+                        relative_path = os.path.dirname(file_path.split(source)[-1])
+                        destination = '{base}{rel}'.format(base=destination, rel=relative_path.replace('\\', '/'))
+                        upload_details = (file_path, destination, public)
+                        upload_details_list.append(upload_details)
+                else:
+                    logger.info('Could not validate source for {source}. Skipping...'.format(source=source))
+
+        pool = ThreadPool(S3BucketManager.UPLOAD_THREADS_NUM)
+        uploaded_files_list = pool.map(_upload_file_wrapper, upload_details_list)
+        pool.close()
+        pool.join()
+        return uploaded_files_list
+
+    def get_s3_folder_content(self, s3_folder):
+        """Returns the relative paths of all the objects in the given s3 folder, files and directories, recursively.
+         The paths includes the root dir (s3_folder input). Directories ends with '/'
+
+        :param s3_folder: S3 folder to examine
+        :return: A list of relative paths of the objects insides the input folder
+        """
+        return [key.key for key in self.bucket_obj.list(prefix=s3_folder)]
+
+    def download_file(self, source, destination):
+        """Download source from s3 server. if destination is a file, the download file path will be the same. If it's a
+         folder, the download file path will be '{}/{}'.format(destination, os.path.basename(source))
+
+        :param source: Relative path of the file inside the bucket
+        :param destination: Local path of the directory or file the file should be downloaded to
+        """
+        if '.' in destination[-5:]:  # the destination is a file path and not a folder
+            dest_file_path = destination
+        else:
+            dest_file_path = os.path.join(destination, os.path.basename(source))
+        logger.info(f'Download file from "{source}" to "{dest_file_path}"')
+
+        destination_dir = os.path.dirname(dest_file_path)
+        if not destination_dir:
+            destination_dir = os.getcwd()
+        with lock:
+            if not os.path.exists(destination_dir):
+                os.makedirs(destination_dir)
+        if not os.path.exists(destination_dir):
+            return
+
+        k = Key(self.bucket_obj)
+        k.key = source
+        k.get_contents_to_filename(dest_file_path)
+        return dest_file_path
+
+    def download(self, source_list, destination):
+        """Download folder content from s3 server. The list can contain an s3 folder name or an s3 file relative path.
+        If the source is a folder, its content will be downloaded with the same hierarchical order (without the root
+        dir) in the destination dir. if the source is a file, it will be downloaded directly to the destination dir
+
+        :param source_list: List of s3 sources, files and folders
+        :param destination: Destination dir
+        :return: A list of the newly added files paths
+        """
+
+        def _download_file_wrapper(tup):
+            """A wrapper to self.download_file_from_s3 that allows to use it in pool.map. Takes a tuple of variables
+             and invokes self.download_file_from_s3 with them as single args
+
+            :param tup: Tuple of argument
+            :return: The result of self.download_file_from_s3 with the given input
+            """
+            return self.download_file(*tup)
+
+        source_list = source_list if isinstance(source_list, list) else [source_list]
+        download_details_list = []
+        for source in source_list:
+            source = source.strip('/')
+            k = self.bucket_obj.get_key(source)  # check if source is a file (s3 key) or a folder
+            if k:
+                download_details_list.append((source, destination))
+            else:  # source is a folder
+                for key in self.bucket_obj.list(prefix=source):
+                    relative_url = key.key
+                    sub_folder = os.path.dirname(relative_url).split(source)[-1].strip('/')
+                    destination = os.path.join(destination, sub_folder) if sub_folder else destination
+                    download_details_list.append((relative_url, destination))
+
+        pool = ThreadPool(S3BucketManager.DOWNLOAD_THREADS_NUM)
+        download_list = pool.map(_download_file_wrapper, download_details_list)
+        pool.close()
+        pool.join()
+        return download_list
+
+    def delete_key_from_bucket(self, key_to_delete):
+        """Delete file or folder from given s3 path
+
+        :param key_to_delete: Folder or file path to delete
+        """
+        self.bucket_obj.delete_key(key_to_delete)
```

### Comparing `pybenutils-3.1.0/pybenutils/network/ssh_helper.py` & `pybenutils-3.2.2/pybenutils/network/ssh_helper.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-import os
-import time
-import json
-import paramiko
-import tempfile
-import argparse
-import threading
-
-
-results_list = []
-example_dict = {
-    "connections": [
-        {
-            "host": "192.168.0.10",  # The target server ip
-            "host_user": "qa",  # The target server local admin user name
-            "host_pass": "1234",  # The target server local admin user password
-            "cmd_list": [
-                "python3 -m pip install pip -U",
-                "echo 1234 > pass.txt",
-                "GET_FILE pass.txt",  # Copy the requested file from the mac vm to the windows vm
-                # Notice: Everything in "/tmp" directory will be lost when the machine shuts down
-            ]
-        }
-    ]
-}
-
-
-class SshHelper:
-    def __init__(self, host, user_name, password):
-        self.user = user_name
-        self.password = password
-        self.host = host
-        self.port = 22
-        self.timeout = 120
-        self.bufsize = -1
-        self.client = None
-
-    def connect(self):
-        self.client = paramiko.SSHClient()
-        self.client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
-        self.client.connect(hostname=self.host, port=self.port, username=self.user, password=self.password,
-                            banner_timeout=10)
-
-    def run(self, command):
-        if not self.client:
-            self.connect()
-        chan = self.client.get_transport().open_session()
-        chan.settimeout(self.timeout)
-        chan.set_combine_stderr(True)
-        chan.get_pty()
-        chan.exec_command(command)
-        stdout = chan.makefile('r', self.bufsize)
-        stdout_text = stdout.read()
-        status = int(chan.recv_exit_status())
-        return stdout_text, status
-
-    def run_in_terminal(self, command, outputfile='outfile'):
-        tempdir = tempfile.gettempdir()  # prints the current temporary directory
-        temp_file_name = os.path.join(tempdir, 't_{ts}.txt'.format(ts=str(time.time()).replace('.', '')))
-        with open(temp_file_name, mode='w+') as f:
-            f.write(r'{cmd} 2>&1 | tee {output} ;'.format(cmd=command, output=outputfile) + '\n')
-            f.write("osascript -e 'tell application \"Terminal\" to quit' ;" + '\n')
-
-            f.seek(0)  # return to beginning of file
-            print(f.read())  # reads data back from the file
-
-        try:
-            if not self.client:
-                self.connect()
-
-            sftp = self.client.open_sftp()
-            sftp.put(temp_file_name, '/tmp/tmp.sh')
-
-            chan = self.client.get_transport().open_session()
-            chan.settimeout(self.timeout)
-            chan.set_combine_stderr(True)
-            chan.get_pty()
-            chan.exec_command(r'chmod +x /tmp/tmp.sh ;'
-                              r'open -W -a Terminal /tmp/tmp.sh ;'.format(cmd=command))
-            # stdout = chan.makefile('r', self.bufsize)
-            # stdout_text = stdout.read()
-            status = int(chan.recv_exit_status())
-
-            stdout_text, stam = self.run(r'cat {output}'.format(output=outputfile))
-
-            return stdout_text, status
-        finally:
-            self.close()
-
-    def close(self):
-        self.client.close()
-
-    def copy_to_remote(self, source, destination):
-        """ Copy file from local to remote
-
-        :param source: local file
-        :param destination: Full path on remote machine
-        """
-        if not self.client:
-            self.connect()
-        sftp = self.client.open_sftp()
-        sftp.put(os.path.realpath(source), destination)
-        self.close()
-
-    def get_from_remote(self, source, destination):
-        if not self.client:
-            self.connect()
-        sftp = self.client.open_sftp()
-        sftp.get(source, destination)
-        self.close()
-
-
-def run_cmd(conf):
-    global results_list
-    thread_log = '---THREAD_START---\n'
-    for idx, cmd in enumerate(conf['cmd_list']):
-        thread_log += '*****\n'
-        cmd = str(cmd).replace("'", "\\'")
-        thread_log += 'Running cmd: {}\n'.format(cmd)
-        open_connection = SshHelper(host=conf['host'], user_name=conf['host_user'], password=conf['host_pass'])
-        status = 'DONE'
-        output = ''
-        if cmd.startswith('COPY_FILE'):
-            thread_log += 'Trying to copy {s} to {t}\n'.format(s=cmd.split()[1], t=cmd.split()[2])
-            try:
-                open_connection.copy_to_remote(source=cmd.split()[1], destination=cmd.split()[2])
-            except Exception as err:
-                thread_log += 'Failed to perform copy function for error: {e}\n'.format(e=err)
-        elif cmd.startswith('GET_FILE'):
-            thread_log += 'Trying to copy {s} to {t}\n'.format(s=cmd.split()[1], t=cmd.split()[2])
-            try:
-                open_connection.get_from_remote(source=cmd.split()[1], destination=cmd.split()[2])
-            except Exception as err2:
-                thread_log += 'Failed to perform get function for error: {e}\n'.format(e=err2)
-        else:
-            try:
-                output_file_path = '/Automation/output_{ind}.txt'.format(ind=idx)
-                output, status = open_connection.run_in_terminal(cmd, outputfile=output_file_path)
-            except Exception as err3:
-                thread_log += 'Failed to perform run command function for error: {e}\n'.format(e=err3)
-                thread_log += 'Stopping the commands flow due to connection problem\n'
-                break
-        thread_log += 'Finished with status code: {s}. Run-time log: {log}\n'.format(s=status, log=str(output))
-
-        time.sleep(5)
-    thread_log += '---THREAD_END---\n'
-    with open(args.out, 'w+') as out_file:
-        out_file.write(thread_log)
-
-
-if __name__ == '__main__':
-    parser = argparse.ArgumentParser(description='Mac script activator trough SSH connection')
-    parser.add_argument('-c', '--config_file',
-                        help=f'Parameters json file for the ssh connection\n{json.dumps(example_dict)}',
-                        required=False,
-                        default='')
-    parser.add_argument('-o', '--out', help='Output log file path', required=False, nargs='?',
-                        default='output_{ts}.txt'.format(ts=str(time.time()).replace('.', '')))
-    args = parser.parse_args()
-
-    if not os.path.isfile(args.config_file):
-        print(f'Missing input "--config_file" Please run {__file__} --help to see input details.\n'
-              f'Example config file:\n{json.dumps(example_dict, indent=4)}')
-        exit(1)
-
-    with open(args.config_file, 'r') as config_file_source:
-        ssh_config_dict = json.load(config_file_source)
-    with open(args.out, 'w') as output_file:
-        output_file.write('')
-    threads = []
-    for connection in ssh_config_dict['connections']:
-        t = threading.Thread(target=run_cmd, args=(connection,))
-        threads.append(t)
-        t.start()
-    for thread in threads:
-        thread.join()
+import os
+import time
+import json
+import paramiko
+import tempfile
+import argparse
+import threading
+
+
+results_list = []
+example_dict = {
+    "connections": [
+        {
+            "host": "192.168.0.10",  # The target server ip
+            "host_user": "qa",  # The target server local admin user name
+            "host_pass": "1234",  # The target server local admin user password
+            "cmd_list": [
+                "python3 -m pip install pip -U",
+                "echo 1234 > pass.txt",
+                "GET_FILE pass.txt",  # Copy the requested file from the mac vm to the windows vm
+                # Notice: Everything in "/tmp" directory will be lost when the machine shuts down
+            ]
+        }
+    ]
+}
+
+
+class SshHelper:
+    def __init__(self, host, user_name, password):
+        self.user = user_name
+        self.password = password
+        self.host = host
+        self.port = 22
+        self.timeout = 120
+        self.bufsize = -1
+        self.client = None
+
+    def connect(self):
+        self.client = paramiko.SSHClient()
+        self.client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+        self.client.connect(hostname=self.host, port=self.port, username=self.user, password=self.password,
+                            banner_timeout=10)
+
+    def run(self, command):
+        if not self.client:
+            self.connect()
+        chan = self.client.get_transport().open_session()
+        chan.settimeout(self.timeout)
+        chan.set_combine_stderr(True)
+        chan.get_pty()
+        chan.exec_command(command)
+        stdout = chan.makefile('r', self.bufsize)
+        stdout_text = stdout.read()
+        status = int(chan.recv_exit_status())
+        return stdout_text, status
+
+    def run_in_terminal(self, command, outputfile='outfile'):
+        tempdir = tempfile.gettempdir()  # prints the current temporary directory
+        temp_file_name = os.path.join(tempdir, 't_{ts}.txt'.format(ts=str(time.time()).replace('.', '')))
+        with open(temp_file_name, mode='w+') as f:
+            f.write(r'{cmd} 2>&1 | tee {output} ;'.format(cmd=command, output=outputfile) + '\n')
+            f.write("osascript -e 'tell application \"Terminal\" to quit' ;" + '\n')
+
+            f.seek(0)  # return to beginning of file
+            print(f.read())  # reads data back from the file
+
+        try:
+            if not self.client:
+                self.connect()
+
+            sftp = self.client.open_sftp()
+            sftp.put(temp_file_name, '/tmp/tmp.sh')
+
+            chan = self.client.get_transport().open_session()
+            chan.settimeout(self.timeout)
+            chan.set_combine_stderr(True)
+            chan.get_pty()
+            chan.exec_command(r'chmod +x /tmp/tmp.sh ;'
+                              r'open -W -a Terminal /tmp/tmp.sh ;'.format(cmd=command))
+            # stdout = chan.makefile('r', self.bufsize)
+            # stdout_text = stdout.read()
+            status = int(chan.recv_exit_status())
+
+            stdout_text, stam = self.run(r'cat {output}'.format(output=outputfile))
+
+            return stdout_text, status
+        finally:
+            self.close()
+
+    def close(self):
+        self.client.close()
+
+    def copy_to_remote(self, source, destination):
+        """ Copy file from local to remote
+
+        :param source: local file
+        :param destination: Full path on remote machine
+        """
+        if not self.client:
+            self.connect()
+        sftp = self.client.open_sftp()
+        sftp.put(os.path.realpath(source), destination)
+        self.close()
+
+    def get_from_remote(self, source, destination):
+        if not self.client:
+            self.connect()
+        sftp = self.client.open_sftp()
+        sftp.get(source, destination)
+        self.close()
+
+
+def run_cmd(conf):
+    global results_list
+    thread_log = '---THREAD_START---\n'
+    for idx, cmd in enumerate(conf['cmd_list']):
+        thread_log += '*****\n'
+        cmd = str(cmd).replace("'", "\\'")
+        thread_log += 'Running cmd: {}\n'.format(cmd)
+        open_connection = SshHelper(host=conf['host'], user_name=conf['host_user'], password=conf['host_pass'])
+        status = 'DONE'
+        output = ''
+        if cmd.startswith('COPY_FILE'):
+            thread_log += 'Trying to copy {s} to {t}\n'.format(s=cmd.split()[1], t=cmd.split()[2])
+            try:
+                open_connection.copy_to_remote(source=cmd.split()[1], destination=cmd.split()[2])
+            except Exception as err:
+                thread_log += 'Failed to perform copy function for error: {e}\n'.format(e=err)
+        elif cmd.startswith('GET_FILE'):
+            thread_log += 'Trying to copy {s} to {t}\n'.format(s=cmd.split()[1], t=cmd.split()[2])
+            try:
+                open_connection.get_from_remote(source=cmd.split()[1], destination=cmd.split()[2])
+            except Exception as err2:
+                thread_log += 'Failed to perform get function for error: {e}\n'.format(e=err2)
+        else:
+            try:
+                output_file_path = '/Automation/output_{ind}.txt'.format(ind=idx)
+                output, status = open_connection.run_in_terminal(cmd, outputfile=output_file_path)
+            except Exception as err3:
+                thread_log += 'Failed to perform run command function for error: {e}\n'.format(e=err3)
+                thread_log += 'Stopping the commands flow due to connection problem\n'
+                break
+        thread_log += 'Finished with status code: {s}. Run-time log: {log}\n'.format(s=status, log=str(output))
+
+        time.sleep(5)
+    thread_log += '---THREAD_END---\n'
+    with open(args.out, 'w+') as out_file:
+        out_file.write(thread_log)
+
+
+if __name__ == '__main__':
+    parser = argparse.ArgumentParser(description='Mac script activator trough SSH connection')
+    parser.add_argument('-c', '--config_file',
+                        help=f'Parameters json file for the ssh connection\n{json.dumps(example_dict)}',
+                        required=False,
+                        default='')
+    parser.add_argument('-o', '--out', help='Output log file path', required=False, nargs='?',
+                        default='output_{ts}.txt'.format(ts=str(time.time()).replace('.', '')))
+    args = parser.parse_args()
+
+    if not os.path.isfile(args.config_file):
+        print(f'Missing input "--config_file" Please run {__file__} --help to see input details.\n'
+              f'Example config file:\n{json.dumps(example_dict, indent=4)}')
+        exit(1)
+
+    with open(args.config_file, 'r') as config_file_source:
+        ssh_config_dict = json.load(config_file_source)
+    with open(args.out, 'w') as output_file:
+        output_file.write('')
+    threads = []
+    for connection in ssh_config_dict['connections']:
+        t = threading.Thread(target=run_cmd, args=(connection,))
+        threads.append(t)
+        t.start()
+    for thread in threads:
+        thread.join()
```

### Comparing `pybenutils-3.1.0/pybenutils/os_operations/mac_application_control.py` & `pybenutils-3.2.2/pybenutils/os_operations/mac_application_control.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,389 +1,389 @@
-import os
-import re
-import sys
-import time
-from pybenutils.utils_logger.config_logger import get_logger
-
-if sys.platform != 'win32':
-    from pybenutils.os_operations.mac_operations import get_bundle_id_by_name, run_apple_script
-
-logger = get_logger()
-
-
-class AppElement:
-    def __init__(self, element_type, element_value, element_path):
-        self.type = element_type
-        self.value = element_value
-        self.path = element_path
-
-    @property
-    def type(self):
-        return self.__type
-
-    @type.setter
-    def type(self, element_type):
-        self.__type = element_type
-
-    @property
-    def value(self):
-        return self.__value
-
-    @value.setter
-    def value(self, element_value):
-        self.__value = element_value
-
-    @property
-    def path(self):
-        return self.__path
-
-    @path.setter
-    def path(self, element_path):
-        self.__path = element_path
-
-    def __dict__(self):
-        return {"type": self.type, "value": self.value, "path": self.path}
-
-    def __str__(self):
-        return str(self.__dict__)
-
-
-class ApplicationControl:
-    def __init__(self, application_file_path, system_level_application='System Events'):
-        self.application_path = application_file_path
-        self.app_name = os.path.basename(application_file_path).split('.app')[0]
-        self.application_process_name = None  # dynamically inserted in the launch method
-        self.bundle_id = None
-        self.system_level_application_name = system_level_application
-        self.elements_in_current_view = []
-
-    def get_application_process_name(self):
-        if not self.application_process_name:
-            get_application_process_name_script = \
-                'tell application "{sys_app}" \n set application_id to (get the id of application "{app_name}" as ' \
-                'string) \n set process_name to name of (application processes where bundle identifier is ' \
-                'application_id) \n end tell'.format(sys_app=self.system_level_application_name, app_name=self.app_name)
-            name = run_apple_script(get_application_process_name_script).strip()
-            if name:
-                logger.debug('Application process name is: {}'.format(name))
-                self.application_process_name = name
-        return self.application_process_name
-
-    def launch(self, arguments=None, timeout=60):
-        """Launches the Installer with the specified path.
-        :param arguments: Execution arguments
-        :param timeout: Seconds to wait for the installer to initiate
-        :return: True if the installer window is detected and has content
-        """
-        # Adding the args to the cmd
-        if arguments and type(arguments) in [str, bytes]:
-            arguments = [arguments]
-
-        args_str = ' --args {params}'.format(params=' '.join(arguments)) if arguments else ''
-        cmd = 'open "{file_path}"{params}'.format(file_path=self.application_path, params=args_str)
-        if not os.path.exists(self.application_path):
-            logger.error('No file was found at {fp}'.format(fp=self.application_path))
-            return False
-        error_code = os.system(cmd)
-        if int(error_code) != 0:
-            logger.error('The installer\'s launch command failed with error code {}'.format(error_code))
-            return False
-        final_timeout = time.time() + timeout
-        while time.time() < final_timeout:
-            if not self.application_process_name:
-                self.application_process_name = self.get_application_process_name()
-            else:
-                if self.is_running() and self.is_window_content_accessible():
-                    break
-            time.sleep(5)
-        else:
-            logger.error('Application was not launched')
-            return False
-        return True
-
-    def is_elements_exists(self, use_cache=True, *expected_values):
-        """Verifies all the expected Values/Titles strings exists in the application
-
-        :param expected_values: Values and titles to search for
-        :param use_cache: the check will be done using the known elements from previous check of the view. if the cache
-        is empty, a new check of the view will be done
-        :return: True if all are found
-        """
-        logger.debug('Checking if the following elements exist: {}'.format(expected_values))
-        if use_cache and self.elements_in_current_view:
-            logger.debug('Checking in the cached elements')
-            elements_in_view = self.elements_in_current_view
-        else:
-            logger.debug('Checking in the view elements')
-            elements_in_view = self.get_elements_in_view()
-            if not elements_in_view:  # handle a scenario where the self.get_elements_in_view() method fail
-                logger.error('Failed to get view elements. Retrying')
-                elements_in_view = self.get_elements_in_view()
-            if not elements_in_view:
-                logger.error('Failed to get view elements. Aborting the check')
-                return
-
-        existing_values_list = list(set([element_value.value for element_value in elements_in_view if element_value]))
-        for expected_value in list(set(expected_values)):
-            expected_value = expected_value
-            logger.debug('Checking if the following element exist: {}'.format(expected_value))
-            for existing_element_str_value in existing_values_list:
-                if existing_element_str_value == str(expected_value):
-                    break
-            else:
-                return False
-        return True
-
-    def get_elements_in_view(self):
-        """Returns a list of detected elements within the application current view
-
-        :return: List of objects [{"type": 'the element role, "value": 'value or title', "path": 'position path'}]
-        """
-        logger.debug('Getting all elements in the view of "{}"'.format(self.get_application_process_name()))
-        window_objects_dict_list = []
-
-        # get all elements paths
-        get_elements_apple_script = \
-            'tell application "{sys_app}" to tell front window of application process "{app_name}" to return entire ' \
-            'contents'.format(sys_app=self.system_level_application_name, app_name=self.get_application_process_name())
-        result = run_apple_script(get_elements_apple_script)
-        if not result:
-            logger.error('Failed to get elements when running {}'.format(get_elements_apple_script))
-            return
-        application_process_name = re.findall('application process (.+?),', result)[0]
-        elements_list = re.findall('(.+? application process {}), '.format(application_process_name), result)
-        paths_list = [item[item.index('of'):] for item in elements_list]
-        if not paths_list:
-            logger.error('Failed to get elements\' paths')
-            return
-        application_process_name = re.findall('application process (.+)', paths_list[0])[0]
-        for index, path in enumerate(paths_list):  # wrap the main application process name with ""
-            paths_list[index] = path.replace(application_process_name, '"{}"'.format(application_process_name))
-
-        # get all elements names and classes
-        get_elements_details_apple_script = \
-            'set final to {{}}\n tell application "{sys_app}" \n tell front window of application process ' \
-            '"{app_name}" \n repeat with ui_element in entire contents as list \n set current_ui to name of ' \
-            'ui_element as string & ";" & class of ui_element as string & "$"\n set final to final & current_ui \n ' \
-            'end repeat \n return final \n end tell \n end tell'.format(sys_app=self.system_level_application_name,
-                                                                        app_name=self.get_application_process_name())
-        result = run_apple_script(get_elements_details_apple_script)
-        if not result:
-            logger.error('Failed to get elements when running {}'.format(get_elements_details_apple_script))
-            return
-        elements_details_list = re.findall(r'(.+?)\$, ', result)
-        elements_details_dict_list = [{'value': item.split(';')[0].strip(), 'class': item.split(';')[1]} for item in
-                                      elements_details_list]
-        if not elements_details_dict_list:
-            logger.error('Failed to get elements\' details')
-            return
-        if len(paths_list) != len(elements_details_dict_list):
-            logger.error('There\'s a Mismatch between the number of element\'s paths ({num_p}) and the number of '
-                         'elements details ({num_d})'.format(num_p=len(paths_list),
-                                                             num_d=len(elements_details_dict_list)))
-            return
-
-        # initiate an AppElement instance with the element's class, value and path
-        for index, element_details in enumerate(elements_details_dict_list):
-            element_class = element_details['class']
-            try:
-                element_value = str(element_details['value'])
-            except UnicodeEncodeError:
-                element_value = str(element_details['value'].encode('utf8'))
-            element_value = element_value if element_value != 'missing value' else ''
-
-            element_path = paths_list[index]
-            #  wrap the parent window with "" if it exists and if it's not an integer
-            reg_obj = re.findall('of window (.+?) of', element_path)
-            parent_window = reg_obj[0] if reg_obj else ''
-            if parent_window and not parent_window.isdigit():
-                element_path = element_path.replace(parent_window, '"{}"'.format(parent_window))
-
-            window_objects_dict_list.append(AppElement(element_type=element_class,
-                                                       element_value=element_value,
-                                                       element_path=element_path))
-        self.elements_in_current_view = window_objects_dict_list
-        return self.elements_in_current_view
-
-    def wait_for_element(self, title, timeout=60, use_cache=True):
-        """Wait for an element with the given title to be on view
-
-        :param title: Title of the searched element
-        :param timeout: Timeout in seconds for the operation
-        :param use_cache: If True, will first search in the data from latest view update
-        :return: The requested element if found
-        """
-        try:
-            title = str(title)
-        except UnicodeEncodeError:
-            title = str(title.encode('utf-8'))
-        logger.debug('Waiting for an element with the title "{}"'.format(title))
-        if use_cache:
-            known_elements_with_value = [element for element in self.elements_in_current_view if element.value]
-            for obj in known_elements_with_value:
-                if obj.value == title:
-                    return obj
-            logger.debug('Failed to get the element from the cache, trying to refresh the element list')
-        cmd = ''
-        seconds_wait_before_retry = int(timeout / 10) if int(timeout / 10) > 0 else 1
-        final_timeout = time.time() + timeout
-        while not cmd and time.time() < final_timeout:
-            found_elements = self.get_elements_in_view()
-            if found_elements:
-                found_elements_with_value = [element for element in found_elements if element.value]
-                for obj in found_elements_with_value:
-                    if obj.value == title:
-                        return obj
-            time.sleep(seconds_wait_before_retry)
-        if not cmd:
-            return None
-
-    def set_element_value(self, element_role, element_position_path, new_value):
-        """Set value of element_role of element_position_path to new_value
-
-        :param element_role: The element role like "button"
-        :param element_position_path: The element position inside the application view
-        :param new_value: The new requested value
-        :return: True if successful
-        """
-        cmd = '''on run {}
-                tell application "''' + self.system_level_application_name + '''"
-                tell application process "''' + self.get_application_process_name() + '''"
-                set value of ''' + element_role + ''' of ''' + element_position_path + ''' to "''' + new_value + '''"
-                end tell
-                end tell
-                end run'''
-        result = run_apple_script(cmd)
-        return bool(result)
-
-    def get_bundle_id(self):
-        """Returns the application bundle id"""
-        if self.bundle_id:
-            return self.bundle_id
-        self.bundle_id = get_bundle_id_by_name(self.app_name)
-        logger.debug(self.bundle_id)
-        return self.bundle_id
-
-    def get_text_position(self, text):
-        """Return the position of a text in the application (upper left corner)
-        :param text: Text to locate
-        :return: (pos_x, pos_y)
-        """
-        obj = self.wait_for_element(title=text)
-        if not obj:
-            return False
-        cmd = 'tell application "{sys_app_name}" to return position of {xtype} "{xvalue}" {xpath}'.format(
-            sys_app_name=self.system_level_application_name,
-            xtype=obj.type,
-            xvalue=obj.value,
-            xpath=obj.path)
-        time.sleep(1)
-        result = run_apple_script(cmd)
-        if not result:
-            return False
-        pos_x = int(result.split(",")[0].strip())
-        pos_y = int(result.split(",")[-1].split("\n")[0].strip())
-        return pos_x, pos_y
-
-    def click_by_title(self, title, timeout=60, use_cache=True):
-        """Clicks on an object by its title / text / name. Trying twice as default.
-
-        :param title: Title / text / name
-        :param timeout: Timeout in seconds for object to appear
-        :param use_cache: Try first on the last known location of the requested element
-        :return: True if success
-        """
-        start_time = time.time()
-        estimated_end_time = start_time + timeout
-        obj = self.wait_for_element(title=title, timeout=timeout, use_cache=True)
-        if not obj:
-            return False
-        cmd = 'tell application "{sys_app_name}" to click {xtype} "{xvalue}" {xpath}'.format(
-            sys_app_name=self.system_level_application_name,
-            xtype=obj.type,
-            xvalue=obj.value,
-            xpath=obj.path)
-        time.sleep(1)
-        logger.debug('Trying to click on {cmd}'.format(cmd=cmd))
-        result = run_apple_script(cmd)
-        if not result:
-            if use_cache:
-                # We want to try again without cache:
-                # 1. Its possible that because of cache we are trying to press a ghost element
-                # 2. We want to try again to eliminate mac voodoo (Didn't load, Didn't respond, etc..)
-                return self.click_by_title(title=title, timeout=int(estimated_end_time - time.time()), use_cache=False)
-            else:
-                return False
-        return True
-
-    def close(self):
-        """Closes the installer gracefully"""
-        terminal_command = 'osascript -e \'quit app "' + self.application_path + '"\''
-        os.system(terminal_command)
-
-    def kill(self):
-        """Kills the app"""
-        process_name = self.get_application_process_name()
-        os.system(f'pkill {process_name}')
-        time.sleep(1)
-
-    def get_app_name(self):
-        """Returns the app name"""
-        return self.app_name
-
-    def is_running(self):
-        """Returns True if the application is running"""
-        app_name = self.application_process_name if self.get_application_process_name() else self.app_name
-        cmd = 'tell application "{sys_app_name}" to (name of processes) contains "{app_name}"'.format(
-            sys_app_name=self.system_level_application_name, app_name=app_name)
-        time.sleep(1)
-        result = run_apple_script(cmd).strip()
-        return result == 'true'
-
-    def is_window_content_accessible(self):
-        """Checks if the application is alive its window content is accessible"""
-        get_elements_apple_script = \
-            'tell application "{sys_app}" to tell front window of application process "{app_name}" to return entire ' \
-            'contents'.format(sys_app=self.system_level_application_name, app_name=self.get_application_process_name())
-        objects_list = run_apple_script(get_elements_apple_script)
-        return bool(objects_list)
-
-    def get_window_position(self):
-        """Returns a tuple with the window (x,y) position"""
-        cmd = 'tell application "{sys_app_name}" to return position of window 1 of application process' \
-              ' "{app_name}"'.format(sys_app_name=self.system_level_application_name,
-                                     app_name=self.get_application_process_name())
-        result = run_apple_script(cmd)
-        if result:
-            pos_x = result.split(",")[0].strip()
-            pos_y = result.split(",")[-1].split("\n")[0].strip()
-            return pos_x, pos_y
-
-    def get_short_version(self):
-        """Returns the CFBundleShortVersionString from the package info.plist
-
-        :return: Application version or an empty sting if not found
-        """
-        version = ''
-        plist_file_path = '{app}/Contents/Info.plist'.format(app=self.application_path)
-        if os.path.exists(plist_file_path):
-            with open(plist_file_path, 'r') as plist_file:
-                lines = plist_file.read()
-            re_match = re.search(r'.*<key>CFBundleShortVersionString</key>\n\s<string>(.*)</string>', lines)
-            if re_match:
-                version = re_match.group(1)
-        return version
-
-    def get_bundle_id_from_package(self):
-        """Returns the CFBundleIdentifier from the package info.plist
-
-        :return: Application bundle id or an empty sting if not found
-        """
-        version = ''
-        plist_file_path = '{app}/Contents/Info.plist'.format(app=self.application_path)
-        if os.path.exists(plist_file_path):
-            with open(plist_file_path, 'r') as plist_file:
-                lines = plist_file.read()
-            re_match = re.search(r'.*<key>CFBundleIdentifier</key>\n\s<string>(.*)</string>', lines)
-            if re_match:
-                version = re_match.group(1)
-        return version
+import os
+import re
+import sys
+import time
+from pybenutils.utils_logger.config_logger import get_logger
+
+if sys.platform != 'win32':
+    from pybenutils.os_operations.mac_operations import get_bundle_id_by_name, run_apple_script
+
+logger = get_logger()
+
+
+class AppElement:
+    def __init__(self, element_type, element_value, element_path):
+        self.type = element_type
+        self.value = element_value
+        self.path = element_path
+
+    @property
+    def type(self):
+        return self.__type
+
+    @type.setter
+    def type(self, element_type):
+        self.__type = element_type
+
+    @property
+    def value(self):
+        return self.__value
+
+    @value.setter
+    def value(self, element_value):
+        self.__value = element_value
+
+    @property
+    def path(self):
+        return self.__path
+
+    @path.setter
+    def path(self, element_path):
+        self.__path = element_path
+
+    def __dict__(self):
+        return {"type": self.type, "value": self.value, "path": self.path}
+
+    def __str__(self):
+        return str(self.__dict__)
+
+
+class ApplicationControl:
+    def __init__(self, application_file_path, system_level_application='System Events'):
+        self.application_path = application_file_path
+        self.app_name = os.path.basename(application_file_path).split('.app')[0]
+        self.application_process_name = None  # dynamically inserted in the launch method
+        self.bundle_id = None
+        self.system_level_application_name = system_level_application
+        self.elements_in_current_view = []
+
+    def get_application_process_name(self):
+        if not self.application_process_name:
+            get_application_process_name_script = \
+                'tell application "{sys_app}" \n set application_id to (get the id of application "{app_name}" as ' \
+                'string) \n set process_name to name of (application processes where bundle identifier is ' \
+                'application_id) \n end tell'.format(sys_app=self.system_level_application_name, app_name=self.app_name)
+            name = run_apple_script(get_application_process_name_script)
+            if name:
+                logger.debug('Application process name is: {}'.format(name))
+                self.application_process_name = name.strip()
+        return self.application_process_name
+
+    def launch(self, arguments=None, timeout=60):
+        """Launches the Installer with the specified path.
+        :param arguments: Execution arguments
+        :param timeout: Seconds to wait for the installer to initiate
+        :return: True if the installer window is detected and has content
+        """
+        # Adding the args to the cmd
+        if arguments and type(arguments) in [str, bytes]:
+            arguments = [arguments]
+
+        args_str = ' --args {params}'.format(params=' '.join(arguments)) if arguments else ''
+        cmd = 'open "{file_path}"{params}'.format(file_path=self.application_path, params=args_str)
+        if not os.path.exists(self.application_path):
+            logger.error('No file was found at {fp}'.format(fp=self.application_path))
+            return False
+        error_code = os.system(cmd)
+        if int(error_code) != 0:
+            logger.error('The installer\'s launch command failed with error code {}'.format(error_code))
+            return False
+        final_timeout = time.time() + timeout
+        while time.time() < final_timeout:
+            if not self.application_process_name:
+                self.application_process_name = self.get_application_process_name()
+            else:
+                if self.is_running() and self.is_window_content_accessible():
+                    break
+            time.sleep(5)
+        else:
+            logger.error('Application was not launched')
+            return False
+        return True
+
+    def is_elements_exists(self, use_cache=True, *expected_values):
+        """Verifies all the expected Values/Titles strings exists in the application
+
+        :param expected_values: Values and titles to search for
+        :param use_cache: the check will be done using the known elements from previous check of the view. if the cache
+        is empty, a new check of the view will be done
+        :return: True if all are found
+        """
+        logger.debug('Checking if the following elements exist: {}'.format(expected_values))
+        if use_cache and self.elements_in_current_view:
+            logger.debug('Checking in the cached elements')
+            elements_in_view = self.elements_in_current_view
+        else:
+            logger.debug('Checking in the view elements')
+            elements_in_view = self.get_elements_in_view()
+            if not elements_in_view:  # handle a scenario where the self.get_elements_in_view() method fail
+                logger.error('Failed to get view elements. Retrying')
+                elements_in_view = self.get_elements_in_view()
+            if not elements_in_view:
+                logger.error('Failed to get view elements. Aborting the check')
+                return
+
+        existing_values_list = list(set([element_value.value for element_value in elements_in_view if element_value]))
+        for expected_value in list(set(expected_values)):
+            expected_value = expected_value
+            logger.debug('Checking if the following element exist: {}'.format(expected_value))
+            for existing_element_str_value in existing_values_list:
+                if existing_element_str_value == str(expected_value):
+                    break
+            else:
+                return False
+        return True
+
+    def get_elements_in_view(self):
+        """Returns a list of detected elements within the application current view
+
+        :return: List of objects [{"type": 'the element role, "value": 'value or title', "path": 'position path'}]
+        """
+        logger.debug('Getting all elements in the view of "{}"'.format(self.get_application_process_name()))
+        window_objects_dict_list = []
+
+        # get all elements paths
+        get_elements_apple_script = \
+            'tell application "{sys_app}" to tell front window of application process "{app_name}" to return entire ' \
+            'contents'.format(sys_app=self.system_level_application_name, app_name=self.get_application_process_name())
+        result = run_apple_script(get_elements_apple_script)
+        if not result:
+            logger.error('Failed to get elements when running {}'.format(get_elements_apple_script))
+            return
+        application_process_name = re.findall('application process (.+?),', result)[0]
+        elements_list = re.findall('(.+? application process {}), '.format(application_process_name), result)
+        paths_list = [item[item.index('of'):] for item in elements_list]
+        if not paths_list:
+            logger.error('Failed to get elements\' paths')
+            return
+        application_process_name = re.findall('application process (.+)', paths_list[0])[0]
+        for index, path in enumerate(paths_list):  # wrap the main application process name with ""
+            paths_list[index] = path.replace(application_process_name, '"{}"'.format(application_process_name))
+
+        # get all elements names and classes
+        get_elements_details_apple_script = \
+            'set final to {{}}\n tell application "{sys_app}" \n tell front window of application process ' \
+            '"{app_name}" \n repeat with ui_element in entire contents as list \n set current_ui to name of ' \
+            'ui_element as string & ";" & class of ui_element as string & "$"\n set final to final & current_ui \n ' \
+            'end repeat \n return final \n end tell \n end tell'.format(sys_app=self.system_level_application_name,
+                                                                        app_name=self.get_application_process_name())
+        result = run_apple_script(get_elements_details_apple_script)
+        if not result:
+            logger.error('Failed to get elements when running {}'.format(get_elements_details_apple_script))
+            return
+        elements_details_list = re.findall(r'(.+?)\$, ', result)
+        elements_details_dict_list = [{'value': item.split(';')[0].strip(), 'class': item.split(';')[1]} for item in
+                                      elements_details_list]
+        if not elements_details_dict_list:
+            logger.error('Failed to get elements\' details')
+            return
+        if len(paths_list) != len(elements_details_dict_list):
+            logger.error('There\'s a Mismatch between the number of element\'s paths ({num_p}) and the number of '
+                         'elements details ({num_d})'.format(num_p=len(paths_list),
+                                                             num_d=len(elements_details_dict_list)))
+            return
+
+        # initiate an AppElement instance with the element's class, value and path
+        for index, element_details in enumerate(elements_details_dict_list):
+            element_class = element_details['class']
+            try:
+                element_value = str(element_details['value'])
+            except UnicodeEncodeError:
+                element_value = str(element_details['value'].encode('utf8'))
+            element_value = element_value if element_value != 'missing value' else ''
+
+            element_path = paths_list[index]
+            #  wrap the parent window with "" if it exists and if it's not an integer
+            reg_obj = re.findall('of window (.+?) of', element_path)
+            parent_window = reg_obj[0] if reg_obj else ''
+            if parent_window and not parent_window.isdigit():
+                element_path = element_path.replace(parent_window, '"{}"'.format(parent_window))
+
+            window_objects_dict_list.append(AppElement(element_type=element_class,
+                                                       element_value=element_value,
+                                                       element_path=element_path))
+        self.elements_in_current_view = window_objects_dict_list
+        return self.elements_in_current_view
+
+    def wait_for_element(self, title, timeout=60, use_cache=True):
+        """Wait for an element with the given title to be on view
+
+        :param title: Title of the searched element
+        :param timeout: Timeout in seconds for the operation
+        :param use_cache: If True, will first search in the data from latest view update
+        :return: The requested element if found
+        """
+        try:
+            title = str(title)
+        except UnicodeEncodeError:
+            title = str(title.encode('utf-8'))
+        logger.debug('Waiting for an element with the title "{}"'.format(title))
+        if use_cache:
+            known_elements_with_value = [element for element in self.elements_in_current_view if element.value]
+            for obj in known_elements_with_value:
+                if obj.value == title:
+                    return obj
+            logger.debug('Failed to get the element from the cache, trying to refresh the element list')
+        cmd = ''
+        seconds_wait_before_retry = int(timeout / 10) if int(timeout / 10) > 0 else 1
+        final_timeout = time.time() + timeout
+        while not cmd and time.time() < final_timeout:
+            found_elements = self.get_elements_in_view()
+            if found_elements:
+                found_elements_with_value = [element for element in found_elements if element.value]
+                for obj in found_elements_with_value:
+                    if obj.value == title:
+                        return obj
+            time.sleep(seconds_wait_before_retry)
+        if not cmd:
+            return None
+
+    def set_element_value(self, element_role, element_position_path, new_value):
+        """Set value of element_role of element_position_path to new_value
+
+        :param element_role: The element role like "button"
+        :param element_position_path: The element position inside the application view
+        :param new_value: The new requested value
+        :return: True if successful
+        """
+        cmd = '''on run {}
+                tell application "''' + self.system_level_application_name + '''"
+                tell application process "''' + self.get_application_process_name() + '''"
+                set value of ''' + element_role + ''' of ''' + element_position_path + ''' to "''' + new_value + '''"
+                end tell
+                end tell
+                end run'''
+        result = run_apple_script(cmd)
+        return bool(result)
+
+    def get_bundle_id(self):
+        """Returns the application bundle id"""
+        if self.bundle_id:
+            return self.bundle_id
+        self.bundle_id = get_bundle_id_by_name(self.app_name)
+        logger.debug(self.bundle_id)
+        return self.bundle_id
+
+    def get_text_position(self, text):
+        """Return the position of a text in the application (upper left corner)
+        :param text: Text to locate
+        :return: (pos_x, pos_y)
+        """
+        obj = self.wait_for_element(title=text)
+        if not obj:
+            return False
+        cmd = 'tell application "{sys_app_name}" to return position of {xtype} "{xvalue}" {xpath}'.format(
+            sys_app_name=self.system_level_application_name,
+            xtype=obj.type,
+            xvalue=obj.value,
+            xpath=obj.path)
+        time.sleep(1)
+        result = run_apple_script(cmd)
+        if not result:
+            return False
+        pos_x = int(result.split(",")[0].strip())
+        pos_y = int(result.split(",")[-1].split("\n")[0].strip())
+        return pos_x, pos_y
+
+    def click_by_title(self, title, timeout=60, use_cache=True):
+        """Clicks on an object by its title / text / name. Trying twice as default.
+
+        :param title: Title / text / name
+        :param timeout: Timeout in seconds for object to appear
+        :param use_cache: Try first on the last known location of the requested element
+        :return: True if success
+        """
+        start_time = time.time()
+        estimated_end_time = start_time + timeout
+        obj = self.wait_for_element(title=title, timeout=timeout, use_cache=True)
+        if not obj:
+            return False
+        cmd = 'tell application "{sys_app_name}" to click {xtype} "{xvalue}" {xpath}'.format(
+            sys_app_name=self.system_level_application_name,
+            xtype=obj.type,
+            xvalue=obj.value,
+            xpath=obj.path)
+        time.sleep(1)
+        logger.debug('Trying to click on {cmd}'.format(cmd=cmd))
+        result = run_apple_script(cmd)
+        if not result:
+            if use_cache:
+                # We want to try again without cache:
+                # 1. Its possible that because of cache we are trying to press a ghost element
+                # 2. We want to try again to eliminate mac voodoo (Didn't load, Didn't respond, etc..)
+                return self.click_by_title(title=title, timeout=int(estimated_end_time - time.time()), use_cache=False)
+            else:
+                return False
+        return True
+
+    def close(self):
+        """Closes the installer gracefully"""
+        terminal_command = 'osascript -e \'quit app "' + self.application_path + '"\''
+        os.system(terminal_command)
+
+    def kill(self):
+        """Kills the app"""
+        process_name = self.get_application_process_name()
+        os.system(f'pkill {process_name}')
+        time.sleep(1)
+
+    def get_app_name(self):
+        """Returns the app name"""
+        return self.app_name
+
+    def is_running(self):
+        """Returns True if the application is running"""
+        app_name = self.application_process_name if self.get_application_process_name() else self.app_name
+        cmd = 'tell application "{sys_app_name}" to (name of processes) contains "{app_name}"'.format(
+            sys_app_name=self.system_level_application_name, app_name=app_name)
+        time.sleep(1)
+        result = run_apple_script(cmd)
+        return result and result.strip() == 'true'
+
+    def is_window_content_accessible(self):
+        """Checks if the application is alive its window content is accessible"""
+        get_elements_apple_script = \
+            'tell application "{sys_app}" to tell front window of application process "{app_name}" to return entire ' \
+            'contents'.format(sys_app=self.system_level_application_name, app_name=self.get_application_process_name())
+        objects_list = run_apple_script(get_elements_apple_script)
+        return bool(objects_list)
+
+    def get_window_position(self):
+        """Returns a tuple with the window (x,y) position"""
+        cmd = 'tell application "{sys_app_name}" to return position of window 1 of application process' \
+              ' "{app_name}"'.format(sys_app_name=self.system_level_application_name,
+                                     app_name=self.get_application_process_name())
+        result = run_apple_script(cmd)
+        if result:
+            pos_x = result.split(",")[0].strip()
+            pos_y = result.split(",")[-1].split("\n")[0].strip()
+            return pos_x, pos_y
+
+    def get_short_version(self):
+        """Returns the CFBundleShortVersionString from the package info.plist
+
+        :return: Application version or an empty sting if not found
+        """
+        version = ''
+        plist_file_path = '{app}/Contents/Info.plist'.format(app=self.application_path)
+        if os.path.exists(plist_file_path):
+            with open(plist_file_path, 'r') as plist_file:
+                lines = plist_file.read()
+            re_match = re.search(r'.*<key>CFBundleShortVersionString</key>\n\s<string>(.*)</string>', lines)
+            if re_match:
+                version = re_match.group(1)
+        return version
+
+    def get_bundle_id_from_package(self):
+        """Returns the CFBundleIdentifier from the package info.plist
+
+        :return: Application bundle id or an empty sting if not found
+        """
+        version = ''
+        plist_file_path = '{app}/Contents/Info.plist'.format(app=self.application_path)
+        if os.path.exists(plist_file_path):
+            with open(plist_file_path, 'r') as plist_file:
+                lines = plist_file.read()
+            re_match = re.search(r'.*<key>CFBundleIdentifier</key>\n\s<string>(.*)</string>', lines)
+            if re_match:
+                version = re_match.group(1)
+        return version
```

### Comparing `pybenutils-3.1.0/pybenutils/os_operations/mac_input_control.py` & `pybenutils-3.2.2/pybenutils/os_operations/mac_input_control.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import time
-from pynput.mouse import Button, Controller
-
-
-def mouse_click_on_point(x_position, y_position):
-    """moves the mouse corsair to the wanted position and clicking on it
-
-    :param x_position: x position
-    :param y_position: y position
-    :return:
-    """
-    mouse = Controller()
-
-    # Read pointer position
-    print('The current pointer position is {0}'.format(mouse.position))
-
-    # Set pointer position
-    mouse.position = (x_position, y_position)
-    print('Now we have moved it to {0}'.format(mouse.position))
-
-    # Move pointer relative to current position
-    mouse.move(5, -5)
-
-    # Press and release
-    mouse.press(Button.left)
-    mouse.release(Button.left)
-
-    # Double click; this is different from pressing and releasing
-    # twice on Mac OSX
-    mouse.click(Button.left, 2)
-
-    # Scroll two steps down
-    mouse.scroll(0, 2)
-
-
-def mouse_drag(initial_x_pos, initial_y_pos, final_x_pos, final_y_pos):
-    """Dragging an object from initial position to its final position
-
-    :param initial_x_pos: Initial x position
-    :param initial_y_pos: Initial y position
-    :param final_x_pos: Final x position
-    :param final_y_pos: Final y position
-    """
-    mouse = Controller()
-    mouse.position = (initial_x_pos, initial_y_pos)
-    mouse.press(Button.left)
-    mouse.move(final_x_pos - initial_x_pos, final_y_pos - initial_y_pos)
-    time.sleep(1)
-    mouse.release(Button.left)
+import time
+from pynput.mouse import Button, Controller
+
+
+def mouse_click_on_point(x_position, y_position):
+    """moves the mouse corsair to the wanted position and clicking on it
+
+    :param x_position: x position
+    :param y_position: y position
+    :return:
+    """
+    mouse = Controller()
+
+    # Read pointer position
+    print('The current pointer position is {0}'.format(mouse.position))
+
+    # Set pointer position
+    mouse.position = (x_position, y_position)
+    print('Now we have moved it to {0}'.format(mouse.position))
+
+    # Move pointer relative to current position
+    mouse.move(5, -5)
+
+    # Press and release
+    mouse.press(Button.left)
+    mouse.release(Button.left)
+
+    # Double click; this is different from pressing and releasing
+    # twice on Mac OSX
+    mouse.click(Button.left, 2)
+
+    # Scroll two steps down
+    mouse.scroll(0, 2)
+
+
+def mouse_drag(initial_x_pos, initial_y_pos, final_x_pos, final_y_pos):
+    """Dragging an object from initial position to its final position
+
+    :param initial_x_pos: Initial x position
+    :param initial_y_pos: Initial y position
+    :param final_x_pos: Final x position
+    :param final_y_pos: Final y position
+    """
+    mouse = Controller()
+    mouse.position = (initial_x_pos, initial_y_pos)
+    mouse.press(Button.left)
+    mouse.move(final_x_pos - initial_x_pos, final_y_pos - initial_y_pos)
+    time.sleep(1)
+    mouse.release(Button.left)
```

### Comparing `pybenutils-3.1.0/pybenutils/os_operations/mac_operations.py` & `pybenutils-3.2.2/pybenutils/os_operations/mac_operations.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-import os
-import subprocess
-import multiprocess
-from pybenutils.utils_logger.config_logger import get_logger
-
-logger = get_logger()
-
-
-def get_network_services():
-    """Displays the network services in the order they are contacted for a connection, along with the
-    corresponding port and device for each. An asterisk (*) next to a service means the service is inactive.
-
-    :return: list of dicts
-    :rtype: list
-    """
-    cmd = 'networksetup -listnetworkserviceorder'
-    result_list = []
-    info_dict = {}
-    result = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE)
-    for line in iter(result.stdout.readline, "".encode()):
-        decoded_line = line.decode()
-        if decoded_line.split() and decoded_line.split()[0][0].startswith('('):
-            if decoded_line.split()[0][1].isdigit():
-                info_dict['index'] = decoded_line.split()[0][1]
-                info_dict['name'] = decoded_line[3:].strip()
-            else:
-                hardware = 'Hardware Port: '
-                hardware_index = decoded_line.index(hardware)
-                device = 'Device: '
-                device_index = decoded_line.index(device)
-                info_dict['hardware_port'] = decoded_line[hardware_index + len(hardware):device_index - 2]
-                info_dict['device'] = decoded_line.strip()[device_index + len(device):-1]
-                result_list.append(dict(info_dict))
-    return result_list
-
-
-def get_bundle_id_by_name(app_name):
-    """Returns the apple bundle id of an application by its name
-    :param app_name: Application name
-    :return: Bundle id or None
-    """
-    cmd = '''id of app "{name}"'''.format(name=app_name)
-    logger.debug(cmd)
-    return run_apple_script(cmd)
-
-
-def create_folder_as_admin(folder_path, admin_password):
-    """Creates a new folder with terminal command as admin
-
-    :param folder_path: Full folder path
-    :param admin_password: The admin user password
-    :return: True if successful (or already exists)
-    """
-    if not os.path.isdir(folder_path):
-        cmd = 'echo {pwd} | sudo -S mkdir "{name}"'.format(pwd=admin_password, name=folder_path)
-        p = subprocess.Popen([cmd], shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
-                             text=True)
-        stdout, stderr = p.communicate()
-        if stderr and stderr != 'Password:':
-            logger.error(stderr)
-            return False
-    return True
-
-
-def kill_java_process(admin_password):
-    logger.debug('Killing "java" process')
-    cmd = 'echo {sudo_pass} | sudo -S killall java'.format(sudo_pass=admin_password)
-    subprocess.Popen([cmd],
-                     shell=True,
-                     stdin=subprocess.PIPE,
-                     stdout=subprocess.PIPE,
-                     stderr=subprocess.PIPE)
-
-
-def restore_default_proxy_settings(ethernet_name='Ethernet', admin_password='1234'):
-    """Restoring system proxy settings to "off" and killing the "java" process
-
-    :param ethernet_name: The ethernet device name
-    :param admin_password: Local user admin password
-    """
-    logger.debug('Changing network proxy state to off by cmd')
-    cmd = 'echo {sudo_pass} | sudo -S networksetup -setwebproxystate {adaptor} off ; ' \
-          'echo {sudo_pass2} | sudo -S networksetup -setsecurewebproxystate {adaptor2} off'.format(
-           sudo_pass=admin_password, adaptor=ethernet_name, sudo_pass2=admin_password, adaptor2=ethernet_name)
-    subprocess.Popen([cmd],
-                     shell=True,
-                     stdin=subprocess.PIPE,
-                     stdout=subprocess.PIPE,
-                     stderr=subprocess.PIPE)
-
-
-def run_apple_script(cmd, timeout=300):
-    """
-    run apple script and return result. the script will run in a different process so if python crashes we will not
-    fail. if the apple script doesn't return answer within the timeout, it will be terminated
-    :param cmd: apple script
-    :param timeout: timeout to end the apple script process
-    :return: apple script result if exist
-    """
-
-    def _run_apple_script_in_another_process(cmd, stdout_queue, stderr_queue):
-        apple_script_process = subprocess.Popen(['osascript'], shell=True, stdin=subprocess.PIPE,
-                                                stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
-        p_stdout, p_stderr = apple_script_process.communicate(cmd)
-        if p_stdout:
-            stdout_queue.put(p_stdout)
-        if p_stderr:
-            stderr_queue.put(p_stderr)
-
-    # logger.debug('Going to run the apple script: {}'.format(cmd))
-    stdout_queue_obj = multiprocess.Queue()
-    stderr_queue_obj = multiprocess.Queue()
-    p = multiprocess.Process(target=_run_apple_script_in_another_process, args=(cmd, stdout_queue_obj,
-                                                                                stderr_queue_obj))
-    p.start()
-    p.join(timeout=timeout)
-    if p.is_alive():
-        logger.error('The process that runs the apple script was terminated after reaching the timeout')
-        p.terminate()
-    if not stderr_queue_obj.empty():  # if stderr, log the error and return None
-        logger.error(stderr_queue_obj.get())
-        return
-    if not stdout_queue_obj.empty():
-        stdout = stdout_queue_obj.get()
-        # logger.debug('Apple script result is: {}'.format(stdout))
-        return stdout
+import os
+import subprocess
+import multiprocess
+from pybenutils.utils_logger.config_logger import get_logger
+
+logger = get_logger()
+
+
+def get_network_services():
+    """Displays the network services in the order they are contacted for a connection, along with the
+    corresponding port and device for each. An asterisk (*) next to a service means the service is inactive.
+
+    :return: list of dicts
+    :rtype: list
+    """
+    cmd = 'networksetup -listnetworkserviceorder'
+    result_list = []
+    info_dict = {}
+    result = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE)
+    for line in iter(result.stdout.readline, "".encode()):
+        decoded_line = line.decode()
+        if decoded_line.split() and decoded_line.split()[0][0].startswith('('):
+            if decoded_line.split()[0][1].isdigit():
+                info_dict['index'] = decoded_line.split()[0][1]
+                info_dict['name'] = decoded_line[3:].strip()
+            else:
+                hardware = 'Hardware Port: '
+                hardware_index = decoded_line.index(hardware)
+                device = 'Device: '
+                device_index = decoded_line.index(device)
+                info_dict['hardware_port'] = decoded_line[hardware_index + len(hardware):device_index - 2]
+                info_dict['device'] = decoded_line.strip()[device_index + len(device):-1]
+                result_list.append(dict(info_dict))
+    return result_list
+
+
+def get_bundle_id_by_name(app_name):
+    """Returns the apple bundle id of an application by its name
+    :param app_name: Application name
+    :return: Bundle id or None
+    """
+    cmd = '''id of app "{name}"'''.format(name=app_name)
+    logger.debug(cmd)
+    return run_apple_script(cmd)
+
+
+def create_folder_as_admin(folder_path, admin_password):
+    """Creates a new folder with terminal command as admin
+
+    :param folder_path: Full folder path
+    :param admin_password: The admin user password
+    :return: True if successful (or already exists)
+    """
+    if not os.path.isdir(folder_path):
+        cmd = 'echo {pwd} | sudo -S mkdir "{name}"'.format(pwd=admin_password, name=folder_path)
+        p = subprocess.Popen([cmd], shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.PIPE,
+                             text=True)
+        stdout, stderr = p.communicate()
+        if stderr and stderr != 'Password:':
+            logger.error(stderr)
+            return False
+    return True
+
+
+def kill_java_process(admin_password):
+    logger.debug('Killing "java" process')
+    cmd = 'echo {sudo_pass} | sudo -S killall java'.format(sudo_pass=admin_password)
+    subprocess.Popen([cmd],
+                     shell=True,
+                     stdin=subprocess.PIPE,
+                     stdout=subprocess.PIPE,
+                     stderr=subprocess.PIPE)
+
+
+def restore_default_proxy_settings(ethernet_name='Ethernet', admin_password='1234'):
+    """Restoring system proxy settings to "off" and killing the "java" process
+
+    :param ethernet_name: The ethernet device name
+    :param admin_password: Local user admin password
+    """
+    logger.debug('Changing network proxy state to off by cmd')
+    cmd = 'echo {sudo_pass} | sudo -S networksetup -setwebproxystate {adaptor} off ; ' \
+          'echo {sudo_pass2} | sudo -S networksetup -setsecurewebproxystate {adaptor2} off'.format(
+           sudo_pass=admin_password, adaptor=ethernet_name, sudo_pass2=admin_password, adaptor2=ethernet_name)
+    subprocess.Popen([cmd],
+                     shell=True,
+                     stdin=subprocess.PIPE,
+                     stdout=subprocess.PIPE,
+                     stderr=subprocess.PIPE)
+
+
+def run_apple_script(cmd, timeout=300):
+    """
+    run apple script and return result. the script will run in a different process so if python crashes we will not
+    fail. if the apple script doesn't return answer within the timeout, it will be terminated
+    :param cmd: apple script
+    :param timeout: timeout to end the apple script process
+    :return: apple script result if exist
+    """
+
+    def _run_apple_script_in_another_process(cmd, stdout_queue, stderr_queue):
+        apple_script_process = subprocess.Popen(['osascript'], shell=True, stdin=subprocess.PIPE,
+                                                stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
+        p_stdout, p_stderr = apple_script_process.communicate(cmd)
+        if p_stdout:
+            stdout_queue.put(p_stdout)
+        if p_stderr:
+            stderr_queue.put(p_stderr)
+
+    # logger.debug('Going to run the apple script: {}'.format(cmd))
+    stdout_queue_obj = multiprocess.Queue()
+    stderr_queue_obj = multiprocess.Queue()
+    p = multiprocess.Process(target=_run_apple_script_in_another_process, args=(cmd, stdout_queue_obj,
+                                                                                stderr_queue_obj))
+    p.start()
+    p.join(timeout=timeout)
+    if p.is_alive():
+        logger.error('The process that runs the apple script was terminated after reaching the timeout')
+        p.terminate()
+    if not stderr_queue_obj.empty():  # if stderr, log the error and return None
+        logger.error(stderr_queue_obj.get())
+        return
+    if not stdout_queue_obj.empty():
+        stdout = stdout_queue_obj.get()
+        # logger.debug('Apple script result is: {}'.format(stdout))
+        return stdout
```

### Comparing `pybenutils-3.1.0/pybenutils/os_operations/process.py` & `pybenutils-3.2.2/pybenutils/os_operations/process.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-import os
-import time
-import psutil
-from psutil import AccessDenied
-from psutil import process_iter
-from pybenutils.utils_logger.config_logger import get_logger
-from typing import Callable, Any, List
-
-logger = get_logger()
-
-
-class ProcessHandler(object):
-    def __init__(self, process_name):
-        self.proc_list = self.get_processes_by_name(process_name)
-        self.process_name = process_name
-
-    @staticmethod
-    def get_processes_by_name(process_name: str) -> List:
-        """Return processes object list
-
-        :param process_name: Process name
-        :return: Process object list
-        """
-        processes_list = []
-        process_name = os.path.basename(process_name)
-        for p in process_iter():
-            try:
-                name = p.name()
-                if name.lower() == process_name.lower():
-                    processes_list.append(p)
-            except (AccessDenied, psutil.NoSuchProcess):
-                pass
-        return processes_list
-
-    def get_processes_child_process_name_list(self):
-        """Get children processes"""
-        processes = []
-        process_name = os.path.basename(self.process_name)
-
-        excluded_list = ["searindexer", "java", "services", "winlogon", "csrss", "smss", "audiodg", "System", "sppsvc",
-                         "dllhost", "conhost", "SearchFilterHost", "SearchProtocolHost", "svchost"]
-
-        for p in psutil.process_iter():
-            try:
-                if process_name.lower() == p.parent().name().lower():
-                    name = p.name()
-                    if not any(True for w in excluded_list if w in name):
-                        processes.append(name)
-            except Exception:
-                pass
-        logger.debug(', '.join(processes))
-        return processes
-
-    def close_process(self):
-        """Free all associated of this process"""
-        for proc in self.proc_list:
-            proc.kill()
-
-    def kill_process(self):
-        """Immediately stop the associated process"""
-        for proc in self.proc_list:
-            proc.kill()
-
-    def process_exists(self) -> bool:
-        """Return True if process exist
-
-        :return: If process exists
-        """
-        if self.proc_list:
-            return True
-        else:
-            return False
-
-    @staticmethod
-    def get_loaded_dll_list_in_file(process_obj=None, pid=None, process_name=None):
-        """Returns a list of dll loaded in the process. Input can be given for the inspected process in 3 ways:
-        process name, pid and process object (psutil.Process instance). Only one will be used, according to the order
-        in the method's signature
-
-        :param process_obj: Psutil.Process instance of the process to inspect
-        :param pid: Pid of the process to inspect
-        :param process_name: Process name to inspect, if no processes are running with the given name, an assertion
-        error will be raised and if more than one is running, the first found will be used
-        :return: List of dll names that were loaded in the process
-        """
-        assert bool(process_obj) | bool(pid) | bool(process_name), 'Dll inspection aborted, no input was given'
-        if not process_obj and not pid:
-            process_list = ProcessHandler.get_processes_by_name(process_name)
-            assert process_list, f'Dll inspection aborted, no running processes were for "{process_name}"'
-            process_obj = process_list[0]
-        if not process_obj:
-            process_obj = psutil.Process(pid)
-        dll_list = sorted([os.path.basename(dll.path.lower()) for dll in process_obj.memory_maps()])
-        logger.debug('The installer loaded the following dlls: {}'.format(dll_list))
-        return dll_list
-
-
-def wait_for_process_to_close(process_name: str, timeout=10):
-    """Returns True if a process closed within the given timeout
-
-    :param process_name: Process name
-    :param timeout: Timeout in seconds
-    :return: True if a process closed within the given timeout
-    """
-    end_time = time.time() + int(timeout) * 60
-    while time.time() < end_time:
-        if not ProcessHandler(process_name).process_exists():
-            logger.debug(f"The process: {process_name} was closed")
-            return True
-        time.sleep(1)
-    else:
-        logger.error(f"Time-out accorded before the process: {process_name} was closed")
-        return False
-
-
-def kill_process(process_obj):
-    """Kill a given process and return result
-
-    :param process_obj: Psutil.process object
-    :return: True if the process was killed
-    """
-    process_killed = False
-    try:
-        process_obj.kill()
-        check_time = 5
-        timeout = time.time() + check_time
-        while time.time() < timeout:
-            if not process_obj.is_running():
-                process_killed = True
-                logger.debug('The process was killed')
-                break
-            time.sleep(1)
-        else:
-            logger.error(f'The kill command was sent for the process but it\'s still alive after {check_time} '
-                         f'seconds')
-    # ignore race-condition cases when the process was found but terminated before the function killed it
-    except psutil.NoSuchProcess:
-        logger.debug('The process was terminated by another thread')
-        process_killed = True
-    return process_killed
-
-
-def process_should_not_be_running(process_name, error=True):
-    """Check if a process is still running
-
-    :param process_name: process name or path
-    :param error: raise error (True) or return result (False)
-    :type error: bool
-    :return: if "error" is set to "False" will return process result
-    """
-    exists = ProcessHandler(os.path.basename(process_name)).process_exists()
-    if not exists:
-        logger.info('process {} is not running'.format(os.path.basename(process_name)))
-        return True
-
-    message = 'process {} is still running'.format(os.path.basename(process_name))
-    if error:
-        raise AssertionError(message)
-
-    logger.error(message)
-    return False
-
-
-def process_should_be_running(process_name, error=True):
-    """Check if a process is not running
-
-    :param process_name: process name or path
-    :param error: raise error (True) or return result (False)
-    :type error: bool
-    :return: if "error" is set to "False" will return process result
-    """
-    exists = ProcessHandler(os.path.basename(process_name)).process_exists()
-    if exists:
-        logger.info('process {} is still running'.format(os.path.basename(process_name)))
-        return True
-
-    message = 'process {} is not running'.format(os.path.basename(process_name))
-    if error:
-        raise AssertionError(message)
-
-    logger.error(message)
-    return False
-
-
-def kill_process_by(condition: Callable[[Any], bool], kill_children=False, kill_all_instances=False):
-    """Kill process by boolean condition
-
-    :param condition: Any boolean condition for the process to kill (Using lambda is advised)
-    :param kill_children: True/False
-    :param kill_children: Kill child processes along with the main one
-    :param kill_all_instances: Don't finish after the first found process was killed
-    :returns True if any processes were killed
-    """
-    process_killed = False
-    found = 0
-    killed = 0
-    for p in psutil.process_iter():
-        try:
-            condition_result = condition(p)
-        except Exception as ex:
-            logger.error(ex)
-            continue
-
-        if condition_result:
-            found += 1
-            if kill_children:
-                logger.debug('Kill child processes')
-                for child in p.children(recursive=True):
-                    kill_process(child)
-                logger.debug('All child processes were killed')
-            if kill_process(p):
-                killed += 1
-            if not kill_all_instances:
-                break
-    if found == 0:
-        logger.debug(f'No process was found matching the input condition')
-    else:
-        logger.debug(f'{"A process was" if found == 1 else f"{found} process were"} found matching the input condition')
-        if found != killed:
-            logger.error(f'{" Only" if killed != 0 else ""} {killed} of the processes '
-                         f'{"was" if killed in [1 ,0] else "were"} killed successfully')
-        else:
-            logger.debug(f'{"The process was" if killed == 1 else "All found process were"} killed successfully')
-            process_killed = True
-    return process_killed
-
-
-def kill_process_by_cmd(partial_cmd_line: str, kill_children=False, kill_all_instances=False):
-    """Kills all processes which cmdline attribute contains the given input
-
-    :param partial_cmd_line: Text to be searched in the running processes cmdline attribute
-    :param kill_children: Kill child processes along with the main one
-    :param kill_all_instances: Don't finish after the first found process was killed
-    :return True if all processes killed successfully
-    """
-    logger.debug(f'Looking for a process who\'s cmd line contains "{partial_cmd_line}" to kill')
-    return kill_process_by(condition=lambda p: partial_cmd_line in ' '.join(p.cmdline()),
-                           kill_children=kill_children,
-                           kill_all_instances=kill_all_instances)
-
-
-def kill_process_by_name(process_name: str, kill_children=False, kill_all_instances=False, add_ext_to_file=True):
-    """Kill process by name
-
-    :param add_ext_to_file: Add or don't add ".exe" to the tested file process name.
-    :param process_name: Name of the process to kill
-    :param kill_children: Kill child processes along with the main one
-    :param kill_all_instances: Don't finish after the first found process was killed
-    :return True if all processes killed successfully
-    """
-    process_name = os.path.basename(process_name)
-    if add_ext_to_file and ".exe" not in process_name and "." not in process_name:
-        process_name = process_name + ".exe"
-    process_name_to_find = process_name.lower()
-    logger.debug(f'Looking for a process with the name "{process_name_to_find}" to kill')
-    return kill_process_by(condition=lambda p: p.name().lower() == process_name_to_find,
-                           kill_children=kill_children,
-                           kill_all_instances=kill_all_instances)
-
-
-def kill_process_by_pid(pid: int, kill_children=False):
-    """Kill process by pid
-
-    :param pid: the pid to kill
-    :param kill_children: Kill child processes along with the main one
-    :return True if all processes killed successfully
-    """
-    logger.debug(f'Looking for a process with the pid "{pid}" to kill')
-    return kill_process_by(condition=lambda p: p.pid == pid,
-                           kill_children=kill_children)
-
-
-def get_all_running_processes(attrs_filter=('pid', 'name')):
-    """The function returns information on all currently running processes
-
-    :param attrs_filter: List of attribute that will be returned for each process. Pass empty to get all attributes.
-        Example attributes: 'name', 'pid', 'ppid', 'cmdline', 'cpu_num', 'open_files', 'threads', 'uids', 'username'.
-        For a list of all available attributes see: https://psutil.readthedocs.io/en/latest/#psutil.Process.as_dict
-    :return: List of Dictionaries, each representing the requested attributes of the running process
-    """
-    if not attrs_filter:
-        attrs_filter = ()
-    return [process.info for process in psutil.process_iter(attrs_filter)]
+import os
+import time
+import psutil
+from psutil import AccessDenied
+from psutil import process_iter
+from pybenutils.utils_logger.config_logger import get_logger
+from typing import Callable, Any, List
+
+logger = get_logger()
+
+
+class ProcessHandler(object):
+    def __init__(self, process_name):
+        self.proc_list = self.get_processes_by_name(process_name)
+        self.process_name = process_name
+
+    @staticmethod
+    def get_processes_by_name(process_name: str) -> List:
+        """Return processes object list
+
+        :param process_name: Process name
+        :return: Process object list
+        """
+        processes_list = []
+        process_name = os.path.basename(process_name)
+        for p in process_iter():
+            try:
+                name = p.name()
+                if name.lower() == process_name.lower():
+                    processes_list.append(p)
+            except (AccessDenied, psutil.NoSuchProcess):
+                pass
+        return processes_list
+
+    def get_processes_child_process_name_list(self):
+        """Get children processes"""
+        processes = []
+        process_name = os.path.basename(self.process_name)
+
+        excluded_list = ["searindexer", "java", "services", "winlogon", "csrss", "smss", "audiodg", "System", "sppsvc",
+                         "dllhost", "conhost", "SearchFilterHost", "SearchProtocolHost", "svchost"]
+
+        for p in psutil.process_iter():
+            try:
+                if process_name.lower() == p.parent().name().lower():
+                    name = p.name()
+                    if not any(True for w in excluded_list if w in name):
+                        processes.append(name)
+            except Exception:
+                pass
+        logger.debug(', '.join(processes))
+        return processes
+
+    def close_process(self):
+        """Free all associated of this process"""
+        for proc in self.proc_list:
+            proc.kill()
+
+    def kill_process(self):
+        """Immediately stop the associated process"""
+        for proc in self.proc_list:
+            proc.kill()
+
+    def process_exists(self) -> bool:
+        """Return True if process exist
+
+        :return: If process exists
+        """
+        if self.proc_list:
+            return True
+        else:
+            return False
+
+    @staticmethod
+    def get_loaded_dll_list_in_file(process_obj=None, pid=None, process_name=None):
+        """Returns a list of dll loaded in the process. Input can be given for the inspected process in 3 ways:
+        process name, pid and process object (psutil.Process instance). Only one will be used, according to the order
+        in the method's signature
+
+        :param process_obj: Psutil.Process instance of the process to inspect
+        :param pid: Pid of the process to inspect
+        :param process_name: Process name to inspect, if no processes are running with the given name, an assertion
+        error will be raised and if more than one is running, the first found will be used
+        :return: List of dll names that were loaded in the process
+        """
+        assert bool(process_obj) | bool(pid) | bool(process_name), 'Dll inspection aborted, no input was given'
+        if not process_obj and not pid:
+            process_list = ProcessHandler.get_processes_by_name(process_name)
+            assert process_list, f'Dll inspection aborted, no running processes were for "{process_name}"'
+            process_obj = process_list[0]
+        if not process_obj:
+            process_obj = psutil.Process(pid)
+        dll_list = sorted([os.path.basename(dll.path.lower()) for dll in process_obj.memory_maps()])
+        logger.debug('The installer loaded the following dlls: {}'.format(dll_list))
+        return dll_list
+
+
+def wait_for_process_to_close(process_name: str, timeout=10):
+    """Returns True if a process closed within the given timeout
+
+    :param process_name: Process name
+    :param timeout: Timeout in seconds
+    :return: True if a process closed within the given timeout
+    """
+    end_time = time.time() + int(timeout) * 60
+    while time.time() < end_time:
+        if not ProcessHandler(process_name).process_exists():
+            logger.debug(f"The process: {process_name} was closed")
+            return True
+        time.sleep(1)
+    else:
+        logger.error(f"Time-out accorded before the process: {process_name} was closed")
+        return False
+
+
+def kill_process(process_obj):
+    """Kill a given process and return result
+
+    :param process_obj: Psutil.process object
+    :return: True if the process was killed
+    """
+    process_killed = False
+    try:
+        process_obj.kill()
+        check_time = 5
+        timeout = time.time() + check_time
+        while time.time() < timeout:
+            if not process_obj.is_running():
+                process_killed = True
+                logger.debug('The process was killed')
+                break
+            time.sleep(1)
+        else:
+            logger.error(f'The kill command was sent for the process but it\'s still alive after {check_time} '
+                         f'seconds')
+    # ignore race-condition cases when the process was found but terminated before the function killed it
+    except psutil.NoSuchProcess:
+        logger.debug('The process was terminated by another thread')
+        process_killed = True
+    return process_killed
+
+
+def process_should_not_be_running(process_name, error=True):
+    """Check if a process is still running
+
+    :param process_name: process name or path
+    :param error: raise error (True) or return result (False)
+    :type error: bool
+    :return: if "error" is set to "False" will return process result
+    """
+    exists = ProcessHandler(os.path.basename(process_name)).process_exists()
+    if not exists:
+        logger.info('process {} is not running'.format(os.path.basename(process_name)))
+        return True
+
+    message = 'process {} is still running'.format(os.path.basename(process_name))
+    if error:
+        raise AssertionError(message)
+
+    logger.error(message)
+    return False
+
+
+def process_should_be_running(process_name, error=True):
+    """Check if a process is not running
+
+    :param process_name: process name or path
+    :param error: raise error (True) or return result (False)
+    :type error: bool
+    :return: if "error" is set to "False" will return process result
+    """
+    exists = ProcessHandler(os.path.basename(process_name)).process_exists()
+    if exists:
+        logger.info('process {} is still running'.format(os.path.basename(process_name)))
+        return True
+
+    message = 'process {} is not running'.format(os.path.basename(process_name))
+    if error:
+        raise AssertionError(message)
+
+    logger.error(message)
+    return False
+
+
+def kill_process_by(condition: Callable[[Any], bool], kill_children=False, kill_all_instances=False):
+    """Kill process by boolean condition
+
+    :param condition: Any boolean condition for the process to kill (Using lambda is advised)
+    :param kill_children: True/False
+    :param kill_children: Kill child processes along with the main one
+    :param kill_all_instances: Don't finish after the first found process was killed
+    :returns True if any processes were killed
+    """
+    process_killed = False
+    found = 0
+    killed = 0
+    for p in psutil.process_iter():
+        try:
+            condition_result = condition(p)
+        except Exception as ex:
+            logger.error(ex)
+            continue
+
+        if condition_result:
+            found += 1
+            if kill_children:
+                logger.debug('Kill child processes')
+                for child in p.children(recursive=True):
+                    kill_process(child)
+                logger.debug('All child processes were killed')
+            if kill_process(p):
+                killed += 1
+            if not kill_all_instances:
+                break
+    if found == 0:
+        logger.debug(f'No process was found matching the input condition')
+    else:
+        logger.debug(f'{"A process was" if found == 1 else f"{found} process were"} found matching the input condition')
+        if found != killed:
+            logger.error(f'{" Only" if killed != 0 else ""} {killed} of the processes '
+                         f'{"was" if killed in [1 ,0] else "were"} killed successfully')
+        else:
+            logger.debug(f'{"The process was" if killed == 1 else "All found process were"} killed successfully')
+            process_killed = True
+    return process_killed
+
+
+def kill_process_by_cmd(partial_cmd_line: str, kill_children=False, kill_all_instances=False):
+    """Kills all processes which cmdline attribute contains the given input
+
+    :param partial_cmd_line: Text to be searched in the running processes cmdline attribute
+    :param kill_children: Kill child processes along with the main one
+    :param kill_all_instances: Don't finish after the first found process was killed
+    :return True if all processes killed successfully
+    """
+    logger.debug(f'Looking for a process who\'s cmd line contains "{partial_cmd_line}" to kill')
+    return kill_process_by(condition=lambda p: partial_cmd_line in ' '.join(p.cmdline()),
+                           kill_children=kill_children,
+                           kill_all_instances=kill_all_instances)
+
+
+def kill_process_by_name(process_name: str, kill_children=False, kill_all_instances=False, add_ext_to_file=True):
+    """Kill process by name
+
+    :param add_ext_to_file: Add or don't add ".exe" to the tested file process name.
+    :param process_name: Name of the process to kill
+    :param kill_children: Kill child processes along with the main one
+    :param kill_all_instances: Don't finish after the first found process was killed
+    :return True if all processes killed successfully
+    """
+    process_name = os.path.basename(process_name)
+    if add_ext_to_file and ".exe" not in process_name and "." not in process_name:
+        process_name = process_name + ".exe"
+    process_name_to_find = process_name.lower()
+    logger.debug(f'Looking for a process with the name "{process_name_to_find}" to kill')
+    return kill_process_by(condition=lambda p: p.name().lower() == process_name_to_find,
+                           kill_children=kill_children,
+                           kill_all_instances=kill_all_instances)
+
+
+def kill_process_by_pid(pid: int, kill_children=False):
+    """Kill process by pid
+
+    :param pid: the pid to kill
+    :param kill_children: Kill child processes along with the main one
+    :return True if all processes killed successfully
+    """
+    logger.debug(f'Looking for a process with the pid "{pid}" to kill')
+    return kill_process_by(condition=lambda p: p.pid == pid,
+                           kill_children=kill_children)
+
+
+def get_all_running_processes(attrs_filter=('pid', 'name')):
+    """The function returns information on all currently running processes
+
+    :param attrs_filter: List of attribute that will be returned for each process. Pass empty to get all attributes.
+        Example attributes: 'name', 'pid', 'ppid', 'cmdline', 'cpu_num', 'open_files', 'threads', 'uids', 'username'.
+        For a list of all available attributes see: https://psutil.readthedocs.io/en/latest/#psutil.Process.as_dict
+    :return: List of Dictionaries, each representing the requested attributes of the running process
+    """
+    if not attrs_filter:
+        attrs_filter = ()
+    return [process.info for process in psutil.process_iter(attrs_filter)]
```

### Comparing `pybenutils-3.1.0/pybenutils/os_operations/window_operations.py` & `pybenutils-3.2.2/pybenutils/os_operations/window_operations.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,313 +1,313 @@
-import sys
-from typing import List, Union
-from pybenutils.utils_logger.config_logger import get_logger
-if sys.platform == 'win32':
-    import win32gui
-    import win32api
-    import win32process
-    import win32con
-
-logger = get_logger()
-
-
-def is_process_running_by_path(file_path: str):
-    """Check if process running by its exe path
-    >>> is_process_running_by_path('C:\\Windows\\explorer.exe')
-    True
-    :param file_path: file path
-    """
-    processes = win32process.EnumProcesses()
-    for pid in processes:
-        try:
-            handle = win32api.OpenProcess(win32con.PROCESS_ALL_ACCESS, False, pid)
-            exe = win32process.GetModuleFileNameEx(handle, 0)
-            if exe.lower() == file_path.lower():
-                return True
-        except:
-            pass
-    return False
-
-
-def close_window_by_hwnd(hwnd: int):
-    """Close window by window handle (HWND)
-
-    :param hwnd: HWND in decimal
-    """
-    if window_exist_by_hwnd(hwnd):
-        try:
-            set_focus_on_window(hwnd)
-        except Exception:
-            logger.debug('Could not set focus on window. continue...')
-        try:
-            flags = win32con.SMTO_BLOCK + win32con.SMTO_ABORTIFHUNG + win32con.SMTO_NOTIMEOUTIFNOTHUNG
-            win32gui.SendMessageTimeout(hwnd, 0x10, 0, 0, flags, 1000)
-            win32gui.SendMessageTimeout(hwnd, 0x10, 0, 0, flags, 1000)
-        except Exception as e:
-            logger.debug('Got error while trying to close the window, details:{error}'.format(error=e))
-        return True
-    else:
-        logger.debug('Could not find the HWND: {}'.format(hwnd))
-        return False
-
-
-def get_window_text(hwnd: int) -> str:
-    """Get window text (title) by window handle (HWND).
-
-    :param hwnd: HWND in decimal
-    """
-    return win32gui.GetWindowText(hwnd)
-
-
-def find_window(window_class: str = None, window_title: str = None):
-    """Get window handle (HWND) by class or/and title.
-
-    :param window_class: Window class name
-    :param window_title: Window title name
-    :return: Window handle (HWND)
-    """
-    hwnd = win32gui.FindWindowEx(0, 0, window_class, window_title)
-    if window_exist_by_hwnd(hwnd):
-        return hwnd
-    else:
-        logger.debug('Could not find the window with class "{w_class}" and title "{w_title}"'.format(
-            w_class=window_class, w_title=window_title))
-        return False
-
-
-def get_process_id_by_hwnd(hwnd: int):
-    """Get process id by window handle (HWND).
-
-    :param hwnd: Window handle (HWND)
-    :return: HWND process ID
-    """
-    if window_exist_by_hwnd(hwnd):
-        return win32gui.GetDlgCtrlID(hwnd)
-    else:
-        logger.debug('Could not find the HWND: {}'.format(hwnd))
-        return False
-
-
-def get_hwnd_by_class(window_class: str) -> int:
-    """Get window handle (HWND) by class. Will return the last top-level window from the class.
-
-    :param window_class: Window class name
-    :return: Window handle (HWND)
-    """
-    def callback(hwnd, inputs):
-        try:
-            if inputs['equals'] == win32gui.GetClassName(hwnd):
-                inputs['res'] = hwnd
-        except:  # Skipping protected, unavailable & unresponsive window handles
-            pass
-
-    extra = {'res': None, 'equals': window_class}
-    win32gui.EnumWindows(callback, extra)
-    return extra['res']
-
-
-def get_hwnds_by_class(window_class: str) -> List[int]:
-    """Returns a list of  window handles (HWND) by class
-
-    :param window_class: Window class name
-    :return: List of window handles (HWND)
-    :rtype: list
-    """
-    def callback(hwnd, inputs):
-        if inputs['equals'] == win32gui.GetClassName(hwnd):
-            inputs['res'].append(hwnd)
-
-    extra = {'res': [], 'equals': window_class}
-    win32gui.EnumWindows(callback, extra)
-    return extra['res']
-
-
-def get_child_hwnd_by_class(hwnd: int, window_class: str) -> int:
-    """Enumerates the child windows that belong to the specified parent window by passing the handle to
-     each child window.
-
-    :param hwnd: HWND in decimal
-    :param window_class: window class name
-    :return: window handle (HWND)
-    """
-    def callback(hwnd, extra):
-        if extra['equals'] == win32gui.GetClassName(hwnd):
-            extra['res'] = hwnd
-
-    extra = {'res': None, 'equals': window_class}
-    win32gui.EnumChildWindows(hwnd, callback, extra)
-    return extra['res']
-
-
-def download_folder_focus():
-    """ Set focus on download folder
-
-    """
-    hwnd = win32gui.FindWindow("CabinetWClass", "Downloads")
-    if hwnd != 0 and hwnd is not None:
-        try:
-            set_focus_on_window(hwnd)
-        except Exception as e:
-            logger.debug('could not set focus on window. continue...')
-        click_on_point(hwnd, 1, 1)
-        return hwnd
-    else:
-        logger.debug('Could not find Download folder window')
-        return False
-
-
-def close_download_folder():
-    """Close download folder"""
-    hwnd = win32gui.FindWindow("CabinetWClass", "Downloads")
-    if hwnd != 0 and hwnd is not None:
-        win32api.SendMessage(hwnd, 0x10, 0, 0)
-        return hwnd
-    else:
-        logger.debug('Could not find Download folder window')
-        return False
-
-
-def set_focus_on_window(hwnd):
-    """Bring a window to the foreground
-
-    :param hwnd: hwnd of window
-    """
-    if window_exist_by_hwnd(hwnd):
-        win32gui.SetForegroundWindow(hwnd)
-        win32gui.BringWindowToTop(hwnd)
-        win32gui.SetActiveWindow(hwnd)
-        return True
-    else:
-        logger.debug('Could not find the HWND: {}'.format(hwnd))
-        return False
-
-
-def window_exist(window_class, window_title):
-    """Return bool if window exist by its class and title
-
-    :param window_class: window class
-    :param window_title: window title
-    :return: True/False
-    :type window_class: str
-    :type window_title: str
-    :rtype: bool
-    """
-    hwnd = win32gui.FindWindow(window_class, window_title)
-    return True if hwnd != 0 and hwnd is not None else False
-
-
-def window_exist_by_hwnd(hwnd: int) -> bool:
-    """ Return bool if window exist by its HWND
-
-    :param hwnd: HWND in decimal
-    :return: True/False
-    :rtype: bool
-    """
-    result = win32gui.IsWindowVisible(hwnd)
-    return True if result != 0 else False
-
-
-def get_hwnds_by_pid(pid: Union[int, str], only_enabled_visible_windows=False):
-    """Get all the window handles (HWND) associated with the given pid
-
-    :param pid: Process ID
-    :param only_enabled_visible_windows: Return only hwnd which are visible and enabled
-    :return: List of window handles (HWND)
-    """
-    def callback(hwnd, parameters_dict):
-        try:
-            thread_id, process_id = win32process.GetWindowThreadProcessId(hwnd)
-            if parameters_dict['pid'] == process_id:
-                if not only_enabled_visible_windows:
-                    parameters_dict['hwnd_list'].append(hwnd)
-                elif win32gui.IsWindowVisible(hwnd) and win32gui.IsWindowEnabled(hwnd):
-                    parameters_dict['hwnd_list'].append(hwnd)
-        except:  # Skipping protected, unavailable & unresponsive window handles
-            pass
-
-    extra = {'hwnd_list': [], 'pid': int(pid)}
-    win32gui.EnumWindows(callback, extra)
-    return extra['hwnd_list']
-
-
-def get_hwnd_details(hwnd: Union[int, str]):
-    """Returns a dict with details about the given hwnd (From the win32gui lib)
-
-    Details:
-      -  hwnd
-      -  GetWindowText
-      -  GetWindowRect
-      -  IsWindowVisible - Windows can be hidden behind other windows
-      -  IsWindowEnabled
-      -  IsWindow
-
-    :param hwnd: A Windows window handle number
-    :return: Dict with details about the given hwnd.
-     Errors will be logged. Failing functions will return with None value
-    """
-    def callback(hwnd, parameters_dict):
-        functions = [win32gui.GetWindowText, win32gui.GetWindowRect, win32gui.IsWindowVisible,
-                     win32gui.IsWindowEnabled, win32gui.IsWindow]
-        if int(hwnd) == int(parameters_dict['hwnd']):
-            for func in functions:
-                func_name = func.__name__
-                try:
-                    parameters_dict[func_name] = func(hwnd)
-                except Exception as ex:
-                    # Since the handle was being requested by the user, its appropriate to display errors
-                    logger.error(f'Failed to execute "{func_name}({hwnd})" for error: {ex}')
-                    parameters_dict[func_name] = None
-
-    results_dict = {'hwnd': hwnd}
-    win32gui.EnumWindows(callback, results_dict)
-    return results_dict
-
-
-def get_visible_enabled_windows_details(pid: Union[int, str]):
-    """Returns a list of dicts with details of enabled visible windows. Windows can be hidden behind other windows
-
-    Details:
-      -  hwnd
-      -  GetWindowText
-      -  GetWindowRect
-      -  IsWindowVisible - Will always be 1
-      -  IsWindowEnabled - Will always be 1
-      -  IsWindow
-
-    :param pid: A Windows process id
-    :return: list of dicts with details of visible windows
-    """
-    return [get_hwnd_details(hwnd) for hwnd in get_hwnds_by_pid(pid, only_enabled_visible_windows=True)]
-
-
-def click_on_point(hwnd, x, y):
-    """Click on point inside a window
-
-    :param hwnd: window hwnd
-    :param x: x position
-    :param y: y position
-    """
-    set_focus_on_window(hwnd)
-    old_pos = win32gui.GetCursorPos()
-    # Get window x,y position
-    rect = win32gui.GetWindowRect(hwnd)
-    win32api.SetCursorPos((rect[0] + x + 2, rect[1] + y + 2))
-    win32api.mouse_event(0x00000002, 0, 0, 0, 0)  # left mouse button up
-    win32api.mouse_event(0x00000004, 0, 0, 0, 0)  # left mouse button up
-    # Set to old position
-    win32api.SetCursorPos(old_pos)
-
-
-def mouse_click(x: int, y: int):
-    """Click on screen by x & y position
-
-    :param x: X position
-    :param y: Y position
-    """
-    win32api.SetCursorPos((x, y))
-    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN, x, y, 0, 0)
-    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP, x, y, 0, 0)
-
-
-def get_cursor_position():
-    """Get mouse cursor (x, y) position"""
-    return win32api.GetCursorPos()
+import sys
+from typing import List, Union
+from pybenutils.utils_logger.config_logger import get_logger
+if sys.platform == 'win32':
+    import win32gui
+    import win32api
+    import win32process
+    import win32con
+
+logger = get_logger()
+
+
+def is_process_running_by_path(file_path: str):
+    """Check if process running by its exe path
+    >>> is_process_running_by_path('C:\\Windows\\explorer.exe')
+    True
+    :param file_path: file path
+    """
+    processes = win32process.EnumProcesses()
+    for pid in processes:
+        try:
+            handle = win32api.OpenProcess(win32con.PROCESS_ALL_ACCESS, False, pid)
+            exe = win32process.GetModuleFileNameEx(handle, 0)
+            if exe.lower() == file_path.lower():
+                return True
+        except:
+            pass
+    return False
+
+
+def close_window_by_hwnd(hwnd: int):
+    """Close window by window handle (HWND)
+
+    :param hwnd: HWND in decimal
+    """
+    if window_exist_by_hwnd(hwnd):
+        try:
+            set_focus_on_window(hwnd)
+        except Exception:
+            logger.debug('Could not set focus on window. continue...')
+        try:
+            flags = win32con.SMTO_BLOCK + win32con.SMTO_ABORTIFHUNG + win32con.SMTO_NOTIMEOUTIFNOTHUNG
+            win32gui.SendMessageTimeout(hwnd, 0x10, 0, 0, flags, 1000)
+            win32gui.SendMessageTimeout(hwnd, 0x10, 0, 0, flags, 1000)
+        except Exception as e:
+            logger.debug('Got error while trying to close the window, details:{error}'.format(error=e))
+        return True
+    else:
+        logger.debug('Could not find the HWND: {}'.format(hwnd))
+        return False
+
+
+def get_window_text(hwnd: int) -> str:
+    """Get window text (title) by window handle (HWND).
+
+    :param hwnd: HWND in decimal
+    """
+    return win32gui.GetWindowText(hwnd)
+
+
+def find_window(window_class: str = None, window_title: str = None):
+    """Get window handle (HWND) by class or/and title.
+
+    :param window_class: Window class name
+    :param window_title: Window title name
+    :return: Window handle (HWND)
+    """
+    hwnd = win32gui.FindWindowEx(0, 0, window_class, window_title)
+    if window_exist_by_hwnd(hwnd):
+        return hwnd
+    else:
+        logger.debug('Could not find the window with class "{w_class}" and title "{w_title}"'.format(
+            w_class=window_class, w_title=window_title))
+        return False
+
+
+def get_process_id_by_hwnd(hwnd: int):
+    """Get process id by window handle (HWND).
+
+    :param hwnd: Window handle (HWND)
+    :return: HWND process ID
+    """
+    if window_exist_by_hwnd(hwnd):
+        return win32gui.GetDlgCtrlID(hwnd)
+    else:
+        logger.debug('Could not find the HWND: {}'.format(hwnd))
+        return False
+
+
+def get_hwnd_by_class(window_class: str) -> int:
+    """Get window handle (HWND) by class. Will return the last top-level window from the class.
+
+    :param window_class: Window class name
+    :return: Window handle (HWND)
+    """
+    def callback(hwnd, inputs):
+        try:
+            if inputs['equals'] == win32gui.GetClassName(hwnd):
+                inputs['res'] = hwnd
+        except:  # Skipping protected, unavailable & unresponsive window handles
+            pass
+
+    extra = {'res': None, 'equals': window_class}
+    win32gui.EnumWindows(callback, extra)
+    return extra['res']
+
+
+def get_hwnds_by_class(window_class: str) -> List[int]:
+    """Returns a list of  window handles (HWND) by class
+
+    :param window_class: Window class name
+    :return: List of window handles (HWND)
+    :rtype: list
+    """
+    def callback(hwnd, inputs):
+        if inputs['equals'] == win32gui.GetClassName(hwnd):
+            inputs['res'].append(hwnd)
+
+    extra = {'res': [], 'equals': window_class}
+    win32gui.EnumWindows(callback, extra)
+    return extra['res']
+
+
+def get_child_hwnd_by_class(hwnd: int, window_class: str) -> int:
+    """Enumerates the child windows that belong to the specified parent window by passing the handle to
+     each child window.
+
+    :param hwnd: HWND in decimal
+    :param window_class: window class name
+    :return: window handle (HWND)
+    """
+    def callback(hwnd, extra):
+        if extra['equals'] == win32gui.GetClassName(hwnd):
+            extra['res'] = hwnd
+
+    extra = {'res': None, 'equals': window_class}
+    win32gui.EnumChildWindows(hwnd, callback, extra)
+    return extra['res']
+
+
+def download_folder_focus():
+    """ Set focus on download folder
+
+    """
+    hwnd = win32gui.FindWindow("CabinetWClass", "Downloads")
+    if hwnd != 0 and hwnd is not None:
+        try:
+            set_focus_on_window(hwnd)
+        except Exception as e:
+            logger.debug('could not set focus on window. continue...')
+        click_on_point(hwnd, 1, 1)
+        return hwnd
+    else:
+        logger.debug('Could not find Download folder window')
+        return False
+
+
+def close_download_folder():
+    """Close download folder"""
+    hwnd = win32gui.FindWindow("CabinetWClass", "Downloads")
+    if hwnd != 0 and hwnd is not None:
+        win32api.SendMessage(hwnd, 0x10, 0, 0)
+        return hwnd
+    else:
+        logger.debug('Could not find Download folder window')
+        return False
+
+
+def set_focus_on_window(hwnd):
+    """Bring a window to the foreground
+
+    :param hwnd: hwnd of window
+    """
+    if window_exist_by_hwnd(hwnd):
+        win32gui.SetForegroundWindow(hwnd)
+        win32gui.BringWindowToTop(hwnd)
+        win32gui.SetActiveWindow(hwnd)
+        return True
+    else:
+        logger.debug('Could not find the HWND: {}'.format(hwnd))
+        return False
+
+
+def window_exist(window_class, window_title):
+    """Return bool if window exist by its class and title
+
+    :param window_class: window class
+    :param window_title: window title
+    :return: True/False
+    :type window_class: str
+    :type window_title: str
+    :rtype: bool
+    """
+    hwnd = win32gui.FindWindow(window_class, window_title)
+    return True if hwnd != 0 and hwnd is not None else False
+
+
+def window_exist_by_hwnd(hwnd: int) -> bool:
+    """ Return bool if window exist by its HWND
+
+    :param hwnd: HWND in decimal
+    :return: True/False
+    :rtype: bool
+    """
+    result = win32gui.IsWindowVisible(hwnd)
+    return True if result != 0 else False
+
+
+def get_hwnds_by_pid(pid: Union[int, str], only_enabled_visible_windows=False):
+    """Get all the window handles (HWND) associated with the given pid
+
+    :param pid: Process ID
+    :param only_enabled_visible_windows: Return only hwnd which are visible and enabled
+    :return: List of window handles (HWND)
+    """
+    def callback(hwnd, parameters_dict):
+        try:
+            thread_id, process_id = win32process.GetWindowThreadProcessId(hwnd)
+            if parameters_dict['pid'] == process_id:
+                if not only_enabled_visible_windows:
+                    parameters_dict['hwnd_list'].append(hwnd)
+                elif win32gui.IsWindowVisible(hwnd) and win32gui.IsWindowEnabled(hwnd):
+                    parameters_dict['hwnd_list'].append(hwnd)
+        except:  # Skipping protected, unavailable & unresponsive window handles
+            pass
+
+    extra = {'hwnd_list': [], 'pid': int(pid)}
+    win32gui.EnumWindows(callback, extra)
+    return extra['hwnd_list']
+
+
+def get_hwnd_details(hwnd: Union[int, str]):
+    """Returns a dict with details about the given hwnd (From the win32gui lib)
+
+    Details:
+      -  hwnd
+      -  GetWindowText
+      -  GetWindowRect
+      -  IsWindowVisible - Windows can be hidden behind other windows
+      -  IsWindowEnabled
+      -  IsWindow
+
+    :param hwnd: A Windows window handle number
+    :return: Dict with details about the given hwnd.
+     Errors will be logged. Failing functions will return with None value
+    """
+    def callback(hwnd, parameters_dict):
+        functions = [win32gui.GetWindowText, win32gui.GetWindowRect, win32gui.IsWindowVisible,
+                     win32gui.IsWindowEnabled, win32gui.IsWindow]
+        if int(hwnd) == int(parameters_dict['hwnd']):
+            for func in functions:
+                func_name = func.__name__
+                try:
+                    parameters_dict[func_name] = func(hwnd)
+                except Exception as ex:
+                    # Since the handle was being requested by the user, its appropriate to display errors
+                    logger.error(f'Failed to execute "{func_name}({hwnd})" for error: {ex}')
+                    parameters_dict[func_name] = None
+
+    results_dict = {'hwnd': hwnd}
+    win32gui.EnumWindows(callback, results_dict)
+    return results_dict
+
+
+def get_visible_enabled_windows_details(pid: Union[int, str]):
+    """Returns a list of dicts with details of enabled visible windows. Windows can be hidden behind other windows
+
+    Details:
+      -  hwnd
+      -  GetWindowText
+      -  GetWindowRect
+      -  IsWindowVisible - Will always be 1
+      -  IsWindowEnabled - Will always be 1
+      -  IsWindow
+
+    :param pid: A Windows process id
+    :return: list of dicts with details of visible windows
+    """
+    return [get_hwnd_details(hwnd) for hwnd in get_hwnds_by_pid(pid, only_enabled_visible_windows=True)]
+
+
+def click_on_point(hwnd, x, y):
+    """Click on point inside a window
+
+    :param hwnd: window hwnd
+    :param x: x position
+    :param y: y position
+    """
+    set_focus_on_window(hwnd)
+    old_pos = win32gui.GetCursorPos()
+    # Get window x,y position
+    rect = win32gui.GetWindowRect(hwnd)
+    win32api.SetCursorPos((rect[0] + x + 2, rect[1] + y + 2))
+    win32api.mouse_event(0x00000002, 0, 0, 0, 0)  # left mouse button up
+    win32api.mouse_event(0x00000004, 0, 0, 0, 0)  # left mouse button up
+    # Set to old position
+    win32api.SetCursorPos(old_pos)
+
+
+def mouse_click(x: int, y: int):
+    """Click on screen by x & y position
+
+    :param x: X position
+    :param y: Y position
+    """
+    win32api.SetCursorPos((x, y))
+    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN, x, y, 0, 0)
+    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP, x, y, 0, 0)
+
+
+def get_cursor_position():
+    """Get mouse cursor (x, y) position"""
+    return win32api.GetCursorPos()
```

### Comparing `pybenutils-3.1.0/pybenutils/useful.py` & `pybenutils-3.2.2/pybenutils/useful.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,80 @@
-from pybenutils.utils_logger.config_logger import get_logger
-
-logger = get_logger()
-
-
-def compare_nested_objects(obj1, obj2):
-    """Compare two nested objects and returns the number of mismatched nodes between them
-
-    :param obj1: First object
-    :param obj2: Second object
-    :return: Number of mismatched nodes between the objects
-    """
-    total_of_mismatched_found = 0
-    if type(obj1) != type(obj2):
-        logger.info('obj types do not match. obj1:{}, type:{} do not match obj2:{}, type:{}'.format(
-            obj1, type(obj1), obj2, type(obj2)))
-        return 1
-    if type(obj1) == str:
-        if obj1 != obj2:
-            logger.info('string "{}" do not match "{}"'.format(obj1, obj2))
-            return 1
-        else:
-            return 0
-    if len(obj2) > len(obj1):
-        temp_obj = obj1
-        obj1 = obj2
-        obj2 = temp_obj
-    if type(obj1) == list:
-        if not obj1:  # checks if the list is empty
-            if not obj2:  # checks if the list is empty
-                return 0
-            else:
-                logger.info('List "{}" is empty on the second list'.format(obj2))
-                return 1
-        if not obj2:  # checks if the list is empty
-            logger.info('List "{}" is empty on the second list'.format(obj1))
-            return 1
-        mismatched_counter_in_list = 0
-        for obj_in_list_a, obj_in_list_b in zip(obj1, obj2):
-            mismatched_counter_in_list += compare_nested_objects(obj_in_list_a, obj_in_list_b)
-        return mismatched_counter_in_list
-    if type(obj1) == dict:
-        if not obj1:  # checks if the dict is empty
-            if not obj2:
-                return 0
-            else:
-                logger.info('Dict {} is empty on the second dict'.format(obj2))
-                return 1
-        for obj1_key, value_of_obj1_key in obj1.items():
-            if obj1_key not in obj2:
-                logger.info('Dict key "{}" appears on one obj and missing from the other'.format(obj1_key))
-                total_of_mismatched_found += 1
-            else:
-                if value_of_obj1_key != obj2[obj1_key]:
-                    total_of_mismatched_found += compare_nested_objects(obj1[obj1_key], obj2[obj1_key])
-    return total_of_mismatched_found
+from typing import List
+
+from pybenutils.utils_logger.config_logger import get_logger
+
+logger = get_logger()
+
+
+def compare_nested_objects(obj1, obj2):
+    """Compare two nested objects and returns the number of mismatched nodes between them
+
+    :param obj1: First object
+    :param obj2: Second object
+    :return: Number of mismatched nodes between the objects
+    """
+    total_of_mismatched_found = 0
+    if type(obj1) != type(obj2):
+        logger.info('obj types do not match. obj1:{}, type:{} do not match obj2:{}, type:{}'.format(
+            obj1, type(obj1), obj2, type(obj2)))
+        return 1
+    if type(obj1) == str:
+        if obj1 != obj2:
+            logger.info('string "{}" do not match "{}"'.format(obj1, obj2))
+            return 1
+        else:
+            return 0
+    if len(obj2) > len(obj1):
+        temp_obj = obj1
+        obj1 = obj2
+        obj2 = temp_obj
+    if type(obj1) == list:
+        if not obj1:  # checks if the list is empty
+            if not obj2:  # checks if the list is empty
+                return 0
+            else:
+                logger.info('List "{}" is empty on the second list'.format(obj2))
+                return 1
+        if not obj2:  # checks if the list is empty
+            logger.info('List "{}" is empty on the second list'.format(obj1))
+            return 1
+        mismatched_counter_in_list = 0
+        for obj_in_list_a, obj_in_list_b in zip(obj1, obj2):
+            mismatched_counter_in_list += compare_nested_objects(obj_in_list_a, obj_in_list_b)
+        return mismatched_counter_in_list
+    if type(obj1) == dict:
+        if not obj1:  # checks if the dict is empty
+            if not obj2:
+                return 0
+            else:
+                logger.info('Dict {} is empty on the second dict'.format(obj2))
+                return 1
+        for obj1_key, value_of_obj1_key in obj1.items():
+            if obj1_key not in obj2:
+                logger.info('Dict key "{}" appears on one obj and missing from the other'.format(obj1_key))
+                total_of_mismatched_found += 1
+            else:
+                if value_of_obj1_key != obj2[obj1_key]:
+                    total_of_mismatched_found += compare_nested_objects(obj1[obj1_key], obj2[obj1_key])
+    return total_of_mismatched_found
+
+
+def smart_cmd_input_eval(input_params: List):
+    """Evaluate the given input list (sys.argv[:]) and returns (unnamed_params_list, named_params_dict)"""
+    unnamed_params_list = []
+    named_params_dict = {}
+    for i in input_params:
+        if '=' in i:
+            key = i.split('=', 1)[0]
+            value = i.split('=', 1)[-1]
+            if value.lower() in ['yes', 'true']:
+                value = True
+            elif value.lower() in ['no', 'false']:
+                value = False
+            try:
+                value = eval(value)
+            except Exception:
+                pass
+            named_params_dict[key] = value
+        else:
+            unnamed_params_list.append(i)
+    return unnamed_params_list, named_params_dict
```

### Comparing `pybenutils-3.1.0/pybenutils.egg-info/PKG-INFO` & `pybenutils-3.2.2/pybenutils.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,85 @@
-Metadata-Version: 2.1
-Name: pybenutils
-Version: 3.1.0
-Summary: PyBEN Utilities repository
-Home-page: https://github.com/DarkFlameBEN/pybenutils.git
-Author: Ben Moskovitch
-Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
-License: MIT License
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pybenutils
-PyBEN Utilities repository, Contains a variety of useful methods and classes designed to allow easy access to high level operations 
-
-### Installation
-> python -m pip install pybenutils -U
-> python3 -m pip install pybenutils -U
-
-### AutoGUI module
-PyBenAutoGui - Class to automate cross platform GUI interactions.
-```
-options:
-  -h, --help            show this help message and exit
-  -t TITLE, --title TITLE
-                        Window title
-  -a APP_PATH, --app_path APP_PATH
-                        Application/Exe path
-  -b PYWINAUTO_BACKEND, --pywinauto_backend PYWINAUTO_BACKEND
-                        A name of used back-end in Windows OS (values: "win32", "uia")
-  -c COMMAND, --command COMMAND
-                        Function name to execute in the AutoGui Class
-```
-
-> python -m pybenutils.autogui -t "Calculator" -a calc.exe -c get_object_details -b uia
-
-> python3 -m pybenutils.autogui -t "Calculator" -a /Application/Calculator.app -c get_object_details
-
-```
-class AutoGui(builtins.object)
- |  AutoGui(title, app_path, pywinauto_backend='uia')
- |  
- |  Methods defined here:
- |  
- |  __init__(self, title, app_path, pywinauto_backend='uia')
- |      Unified interface to interact with Gui Elements
- |      
- |      :param title: Window title
- |      :param app_path: Application/Exe path
- |      :param pywinauto_backend: A name of used back-end in Windows OS (values: "win32", "uia")
- |  
- |  click_on_text(self, text: str)
- |      Clicks on text object location using pyautogui
- |  
- |  find_objects(self, text='', control_type='')
- |      Returns an iterable containing the matching object
- |      
- |      :param text: Text to search, In windows can also be the automation_id
- |      :param control_type: Filter by control type
- |      :return: An iterable containing the matching object
- |  
- |  focus_on_window(self)
- |      Focus on the app window - bring to front
- |  
- |  get_object_details(self, text='', control_type='')
- |      Returns an iterable containing dicts of matching objects properties
- |      
- |      :param text: Text to search, In windows can also be the automation_id
- |      :param control_type: Filter by control type
- |      :return: An iterable containing dicts of matching objects properties
- |  
- |  get_object_position_by_text(self, text)
- |      Return position as tuple (xl, yt, xr, yb) in windows / (x, y) in mac
-```
+Metadata-Version: 2.1
+Name: pybenutils
+Version: 3.2.2
+Summary: PyBEN Utilities repository
+Home-page: https://github.com/DarkFlameBEN/pybenutils.git
+Author: Ben Moskovitch
+Author-email: "Ben Moskovitch" <darkflameben@gmail.com>
+License: MIT License
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pybenutils
+PyBEN Utilities repository, Contains a variety of useful methods and classes designed to allow easy access to high level operations 
+
+### Installation
+Win:
+> python -m pip install pybenutils -U
+
+macOS:
+> python3 -m pip install pybenutils -U
+
+### AutoGUI module
+PyBenAutoGui - Class to automate cross platform GUI interactions.
+```
+options:                                                                                                                   
+  -h, --help            show this help message and exit                                                                    
+  -t TITLE, --title TITLE                                                                                                  
+                        Window title                                                                                       
+  -a APP_PATH, --app_path APP_PATH                                                                                         
+                        Application/Exe path                                                                               
+  -b PYWINAUTO_BACKEND, --pywinauto_backend PYWINAUTO_BACKEND                                                              
+                        A name of used back-end in Windows OS (values: "win32", "uia")                                     
+  -c COMMAND, --command COMMAND                                                                                            
+                        Function name to execute in the AutoGui Class                                                      
+  -eh, --extra_help, --no-extra_help                                                                                       
+                        Display extra help about the class and its functions (default: False)
+
+```
+
+> python -m pybenutils.autogui -t "Calculator" -a calc.exe -c get_object_details -b uia
+
+> python3 -m pybenutils.autogui -t "Calculator" -a /Application/Calculator.app -c get_object_details
+
+```
+class AutoGui(builtins.object)
+ |  AutoGui(title, app_path, pywinauto_backend='uia')
+ |  
+ |  Methods defined here:
+ |  
+ |  __init__(self, title, app_path, pywinauto_backend='uia')
+ |      Unified interface to interact with Gui Elements
+ |      
+ |      :param title: Window title
+ |      :param app_path: Application/Exe path
+ |      :param pywinauto_backend: A name of used back-end in Windows OS (values: "win32", "uia")
+ |  
+ |  click_on_text(self, text: str)
+ |      Clicks on text object location using pyautogui
+ |  
+ |  find_objects(self, text='', control_type='')
+ |      Returns an iterable containing the matching object
+ |      
+ |      :param text: Text to search, In windows can also be the automation_id
+ |      :param control_type: Filter by control type
+ |      :return: An iterable containing the matching object
+ |  
+ |  focus_on_window(self)
+ |      Focus on the app window - bring to front
+ |  
+ |  get_object_details(self, text='', control_type='')
+ |      Returns an iterable containing dicts of matching objects properties
+ |      
+ |      :param text: Text to search, In windows can also be the automation_id
+ |      :param control_type: Filter by control type
+ |      :return: An iterable containing dicts of matching objects properties
+ |  
+ |  get_object_position_by_text(self, text)
+ |      Return position as tuple (xl, yt, xr, yb) in windows / (x, y) in mac
+```
```

### Comparing `pybenutils-3.1.0/pybenutils.egg-info/SOURCES.txt` & `pybenutils-3.2.2/pybenutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,8 +35,9 @@
 pybenutils/os_operations/mac_application_control.py
 pybenutils/os_operations/mac_input_control.py
 pybenutils/os_operations/mac_operations.py
 pybenutils/os_operations/mac_popup_handler.py
 pybenutils/os_operations/process.py
 pybenutils/os_operations/window_operations.py
 pybenutils/utils_logger/__init__.py
-pybenutils/utils_logger/config_logger.py
+pybenutils/utils_logger/config_logger.py
+tests/test_self_import.py
```

### Comparing `pybenutils-3.1.0/setup.py` & `pybenutils-3.2.2/setup.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from setuptools import setup, find_packages
-from codecs import open
-import platform
-import pybenutils
-
-
-with open(r'requirements.txt') as req_file:
-    requirements_list = [line.strip() for line in req_file.readlines() if
-                         not line.strip().startswith('#') and not line.strip().startswith('-') and line.strip()]
-
-final_requirements_list = list(requirements_list)
-
-# XP workaround for psutil
-if platform.release() == 'XP':
-    psutil_index = None
-    for index, req in enumerate(final_requirements_list):
-        if req.startswith('psutil'):
-            psutil_index = index
-            break
-    if psutil_index:
-        final_requirements_list[psutil_index] = 'psutil==3.4.2'
-
-with open('README.md', 'r') as readme_file:
-    readme_content = readme_file.read()
-
-
-setup(
-    name='pybenutils',
-    version=pybenutils.__version__,
-    description='PyBEN Utilities repository',
-    long_description=readme_content,
-    long_description_content_type='text/markdown',
-    url='https://github.com/DarkFlameBEN/pybenutils.git',
-    author=pybenutils.__author__,
-    author_email=pybenutils.__author_email__,
-    license='MIT License',
-    classifiers=[
-        # "Development Status :: 1 - Planning",
-        "Development Status :: 2 - Pre-Alpha",
-        # "Development Status :: 3 - Alpha",
-        # "Development Status :: 4 - Beta",
-        # "Development Status :: 5 - Production/Stable",
-        # "Development Status :: 6 - Mature",
-        # "Development Status :: 7 - Inactive",
-        "Intended Audience :: Developers",
-        'Topic :: Software Development :: Libraries',
-        'License :: OSI Approved :: MIT License',
-        # 'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.7',
-    ],
-    install_requires=final_requirements_list,
-    include_package_data=True,
-    packages=find_packages(exclude=['tests']),
-    python_requires='>3'
-)
+from setuptools import setup, find_packages
+from codecs import open
+import platform
+import pybenutils
+
+
+with open(r'requirements.txt') as req_file:
+    requirements_list = [line.strip() for line in req_file.readlines() if
+                         not line.strip().startswith('#') and not line.strip().startswith('-') and line.strip()]
+
+final_requirements_list = list(requirements_list)
+
+# XP workaround for psutil
+if platform.release() == 'XP':
+    psutil_index = None
+    for index, req in enumerate(final_requirements_list):
+        if req.startswith('psutil'):
+            psutil_index = index
+            break
+    if psutil_index:
+        final_requirements_list[psutil_index] = 'psutil==3.4.2'
+
+with open('README.md', 'r') as readme_file:
+    readme_content = readme_file.read()
+
+
+setup(
+    name='pybenutils',
+    version=pybenutils.__version__,
+    description='PyBEN Utilities repository',
+    long_description=readme_content,
+    long_description_content_type='text/markdown',
+    url='https://github.com/DarkFlameBEN/pybenutils.git',
+    author=pybenutils.__author__,
+    author_email=pybenutils.__author_email__,
+    license='MIT License',
+    classifiers=[
+        # "Development Status :: 1 - Planning",
+        "Development Status :: 2 - Pre-Alpha",
+        # "Development Status :: 3 - Alpha",
+        # "Development Status :: 4 - Beta",
+        # "Development Status :: 5 - Production/Stable",
+        # "Development Status :: 6 - Mature",
+        # "Development Status :: 7 - Inactive",
+        "Intended Audience :: Developers",
+        'Topic :: Software Development :: Libraries',
+        'License :: OSI Approved :: MIT License',
+        # 'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3.7',
+    ],
+    install_requires=final_requirements_list,
+    include_package_data=True,
+    packages=find_packages(exclude=['tests']),
+    python_requires='>3'
+)
```

