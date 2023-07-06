# Comparing `tmp/toolium-3.0.2.dev0.tar.gz` & `tmp/toolium-3.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolium-3.0.2.dev0.tar", last modified: Fri May 19 09:08:23 2023, max compression
+gzip compressed data, was "toolium-3.1.0.dev0.tar", last modified: Thu Jul  6 07:58:40 2023, max compression
```

## Comparing `toolium-3.0.2.dev0.tar` & `toolium-3.1.0.dev0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.986533 toolium-3.0.2.dev0/
--rw-rw-rw-   0        0        0    30389 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.2.dev0/LICENSE
--rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.2.dev0/MANIFEST.in
--rw-rw-rw-   0        0        0     5526 2023-05-19 09:08:22.986533 toolium-3.0.2.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/README.rst
--rw-rw-rw-   0        0        0       12 2023-05-09 09:50:47.000000 toolium-3.0.2.dev0/VERSION
--rw-rw-rw-   0        0        0      225 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/requirements.txt
--rw-rw-rw-   0        0        0      236 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/requirements_dev.txt
--rw-rw-rw-   0        0        0       70 2023-05-19 09:08:22.988535 toolium-3.0.2.dev0/setup.cfg
--rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.630532 toolium-3.0.2.dev0/toolium/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.669533 toolium-3.0.2.dev0/toolium/behave/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/behave/__init__.py
--rw-rw-rw-   0        0        0    12880 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/toolium/behave/env_utils.py
--rw-rw-rw-   0        0        0    11018 2023-05-17 13:54:12.000000 toolium-3.0.2.dev0/toolium/behave/environment.py
--rw-rw-rw-   0        0        0    21019 2023-05-08 11:36:54.000000 toolium-3.0.2.dev0/toolium/config_driver.py
--rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/config_files.py
--rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/config_parser.py
--rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/driver_wrapper.py
--rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/driver_wrappers_pool.py
--rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/jira.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.801534 toolium-3.0.2.dev0/toolium/pageelements/
--rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/button_page_element.py
--rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/checkbox_page_element.py
--rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/group_page_element.py
--rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/input_radio_page_element.py
--rw-rw-rw-   0        0        0     2731 2023-05-10 11:35:00.000000 toolium-3.0.2.dev0/toolium/pageelements/input_text_page_element.py
--rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/link_page_element.py
--rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/page_element.py
--rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/page_elements.py
--rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/select_page_element.py
--rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/text_page_element.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.852537 toolium-3.0.2.dev0/toolium/pageobjects/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/pageobjects/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/common_object.py
--rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/mobile_page_object.py
--rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/page_object.py
--rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pytest_fixtures.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.882536 toolium-3.0.2.dev0/toolium/resources/
--rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTests.css
--rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTests.js
--rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTestsTemplate.html
--rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/selenoid.py
--rw-rw-rw-   0        0        0     8733 2023-05-08 11:36:54.000000 toolium-3.0.2.dev0/toolium/test_cases.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.983535 toolium-3.0.2.dev0/toolium/utils/
--rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/data_generator.py
--rw-rw-rw-   0        0        0    31957 2023-05-05 08:33:04.000000 toolium-3.0.2.dev0/toolium/utils/dataset.py
--rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/download_files.py
--rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/driver_utils.py
--rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/driver_wait_utils.py
--rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/path_utils.py
--rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/poeditor.py
--rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.649538 toolium-3.0.2.dev0/toolium.egg-info/
--rw-rw-rw-   0        0        0     5526 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.620393 toolium-3.1.0.dev0/
+-rw-rw-rw-   0        0        0    30861 2023-06-29 08:59:47.000000 toolium-3.1.0.dev0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.1.0.dev0/LICENSE
+-rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.1.0.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5526 2023-07-06 07:58:40.620393 toolium-3.1.0.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/README.rst
+-rw-rw-rw-   0        0        0       12 2023-06-08 14:08:15.000000 toolium-3.1.0.dev0/VERSION
+-rw-rw-rw-   0        0        0      225 2023-05-29 15:01:04.000000 toolium-3.1.0.dev0/requirements.txt
+-rw-rw-rw-   0        0        0      236 2023-05-19 07:42:34.000000 toolium-3.1.0.dev0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       70 2023-07-06 07:58:40.621394 toolium-3.1.0.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.478392 toolium-3.1.0.dev0/toolium/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.1.0.dev0/toolium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.498396 toolium-3.1.0.dev0/toolium/behave/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.1.0.dev0/toolium/behave/__init__.py
+-rw-rw-rw-   0        0        0    12880 2023-05-19 07:42:34.000000 toolium-3.1.0.dev0/toolium/behave/env_utils.py
+-rw-rw-rw-   0        0        0    11018 2023-05-17 13:54:12.000000 toolium-3.1.0.dev0/toolium/behave/environment.py
+-rw-rw-rw-   0        0        0    21133 2023-06-28 14:48:58.000000 toolium-3.1.0.dev0/toolium/config_driver.py
+-rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/config_files.py
+-rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/config_parser.py
+-rw-rw-rw-   0        0        0    16649 2023-06-29 08:59:47.000000 toolium-3.1.0.dev0/toolium/driver_wrapper.py
+-rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/driver_wrappers_pool.py
+-rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/jira.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.552394 toolium-3.1.0.dev0/toolium/pageelements/
+-rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/button_page_element.py
+-rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/checkbox_page_element.py
+-rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/group_page_element.py
+-rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/input_radio_page_element.py
+-rw-rw-rw-   0        0        0     2731 2023-05-10 11:35:00.000000 toolium-3.1.0.dev0/toolium/pageelements/input_text_page_element.py
+-rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/link_page_element.py
+-rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/page_element.py
+-rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/page_elements.py
+-rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/select_page_element.py
+-rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageelements/text_page_element.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.570395 toolium-3.1.0.dev0/toolium/pageobjects/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.1.0.dev0/toolium/pageobjects/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageobjects/common_object.py
+-rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageobjects/mobile_page_object.py
+-rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pageobjects/page_object.py
+-rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/pytest_fixtures.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.581395 toolium-3.1.0.dev0/toolium/resources/
+-rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.1.0.dev0/toolium/resources/VisualTests.css
+-rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.1.0.dev0/toolium/resources/VisualTests.js
+-rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.1.0.dev0/toolium/resources/VisualTestsTemplate.html
+-rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/selenoid.py
+-rw-rw-rw-   0        0        0     8733 2023-05-08 11:36:54.000000 toolium-3.1.0.dev0/toolium/test_cases.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.618393 toolium-3.1.0.dev0/toolium/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/utils/__init__.py
+-rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/utils/data_generator.py
+-rw-rw-rw-   0        0        0    32908 2023-06-27 11:27:31.000000 toolium-3.1.0.dev0/toolium/utils/dataset.py
+-rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/utils/download_files.py
+-rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/utils/driver_utils.py
+-rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/utils/driver_wait_utils.py
+-rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/utils/path_utils.py
+-rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/utils/poeditor.py
+-rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.1.0.dev0/toolium/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-07-06 07:58:40.485393 toolium-3.1.0.dev0/toolium.egg-info/
+-rw-rw-rw-   0        0        0     5526 2023-07-06 07:58:40.000000 toolium-3.1.0.dev0/toolium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-07-06 07:58:40.000000 toolium-3.1.0.dev0/toolium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 07:58:40.000000 toolium-3.1.0.dev0/toolium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-07-06 07:58:40.000000 toolium-3.1.0.dev0/toolium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-06 07:58:40.000000 toolium-3.1.0.dev0/toolium.egg-info/top_level.txt
```

### Comparing `toolium-3.0.2.dev0/CHANGELOG.rst` & `toolium-3.1.0.dev0/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,29 @@
 Toolium Changelog
 =================
 
-v3.0.2
+v3.1.0
 ------
 
 *Release date: In development*
 
+- Update `[CONTEXT:a.b.c]` replacement to allow lists access, e.g. [CONTEXT:list.1] to access the second element of list
+- Add capabilities configured in `[Capabilities]` section also to Appium tests to use `platformName` and `browserName`
+ w3c capabilities instead of Appium ones
+- `platformVersion` Appium capability must be a string
+
+v3.0.2
+------
+
+*Release date: 2023-06-08*
+
 - `context.storage` must be initialized before dynamic environment steps in `before_feature` method
 - Mark scenario as failed when a dynamic environment step fails in `before_scenario`
 - Mark all feature scenarios as failed when a dynamic environment step fails in `before_feature` and `after_feature`
+- Configure minimal Appium-Python-Client version to 2.3.0 to avoid import errors
 
 v3.0.1
 ------
 
 *Release date: 2023-05-09*
 
 - Allow to search in `context.storage` using `[CONTEXT:a.b.c]` replacement when `before_feature` method is not used
```

### Comparing `toolium-3.0.2.dev0/LICENSE` & `toolium-3.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/PKG-INFO` & `toolium-3.1.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.2.dev0
+Version: 3.1.0.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.2.dev0/README.rst` & `toolium-3.1.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/setup.py` & `toolium-3.1.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/behave/env_utils.py` & `toolium-3.1.0.dev0/toolium/behave/env_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/behave/environment.py` & `toolium-3.1.0.dev0/toolium/behave/environment.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/config_driver.py` & `toolium-3.1.0.dev0/toolium/config_driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         server_url = f"{self.utils.get_server_url()}{self.config.get_optional('Server', 'base_path', '')}"
 
         driver_name = self.utils.get_driver_name()
         if driver_name in ('android', 'ios', 'iphone'):
             # Get driver options
             options = AppiumOptions()
             self._add_capabilities_from_properties(capabilities, 'AppiumCapabilities')
+            self._add_capabilities_from_properties(capabilities, 'Capabilities')
             self._update_dict(options.capabilities, capabilities)
 
             # Create remote appium driver
             driver = appiumdriver.Remote(command_executor=server_url, options=options)
         else:
             # Get driver options
             if driver_name == 'firefox':
@@ -188,17 +189,18 @@
 
         :param capabilities: capabilities object
         :param section: properties section
         """
         cap_type = {'Capabilities': 'server', 'AppiumCapabilities': 'Appium server'}
         try:
             for cap, cap_value in dict(self.config.items(section)).items():
+                if cap not in ['browserVersion', 'platformVersion']:
+                    cap_value = self._convert_property_type(cap_value)
                 cap = f'appium:{cap}' if section == 'AppiumCapabilities' else cap
                 self.logger.debug("Added %s capability: %s = %s", cap_type[section], cap, cap_value)
-                cap_value = cap_value if cap == 'browserVersion' else self._convert_property_type(cap_value)
                 self._update_dict(capabilities, {cap: cap_value}, initial_key=cap)
         except NoSectionError:
             pass
 
     def _setup_firefox(self):
         """Setup Firefox webdriver
```

### Comparing `toolium-3.0.2.dev0/toolium/config_files.py` & `toolium-3.1.0.dev0/toolium/config_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/config_parser.py` & `toolium-3.1.0.dev0/toolium/config_parser.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/driver_wrapper.py` & `toolium-3.1.0.dev0/toolium/driver_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
         return self.is_android_test() or self.is_ios_test()
 
     def is_web_test(self):
         """Check if actual test must be executed in a browser
 
         :returns: True if test must be executed in a browser
         """
-        appium_browser_name = self.config.get_optional('AppiumCapabilities', 'browserName')
+        appium_browser_name = self.config.get_optional('Capabilities', 'browserName')
         return not self.is_mobile_test() or appium_browser_name not in (None, '')
 
     def is_android_web_test(self):
         """Check if actual test must be executed in a browser of an Android mobile
 
         :returns: True if test must be executed in a browser of an Android mobile
         """
```

### Comparing `toolium-3.0.2.dev0/toolium/driver_wrappers_pool.py` & `toolium-3.1.0.dev0/toolium/driver_wrappers_pool.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/jira.py` & `toolium-3.1.0.dev0/toolium/jira.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/__init__.py` & `toolium-3.1.0.dev0/toolium/pageelements/__init__.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/button_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/button_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/checkbox_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/checkbox_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/group_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/group_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/input_radio_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/input_radio_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/input_text_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/input_text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/link_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/link_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/page_elements.py` & `toolium-3.1.0.dev0/toolium/pageelements/page_elements.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/select_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/select_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageelements/text_page_element.py` & `toolium-3.1.0.dev0/toolium/pageelements/text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageobjects/common_object.py` & `toolium-3.1.0.dev0/toolium/pageobjects/common_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageobjects/mobile_page_object.py` & `toolium-3.1.0.dev0/toolium/pageobjects/mobile_page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pageobjects/page_object.py` & `toolium-3.1.0.dev0/toolium/pageobjects/page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/pytest_fixtures.py` & `toolium-3.1.0.dev0/toolium/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/resources/VisualTests.css` & `toolium-3.1.0.dev0/toolium/resources/VisualTests.css`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/resources/VisualTests.js` & `toolium-3.1.0.dev0/toolium/resources/VisualTests.js`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/resources/VisualTestsTemplate.html` & `toolium-3.1.0.dev0/toolium/resources/VisualTestsTemplate.html`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/selenoid.py` & `toolium-3.1.0.dev0/toolium/selenoid.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/test_cases.py` & `toolium-3.1.0.dev0/toolium/test_cases.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/utils/data_generator.py` & `toolium-3.1.0.dev0/toolium/utils/data_generator.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/utils/dataset.py` & `toolium-3.1.0.dev0/toolium/utils/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -577,43 +577,64 @@
     Find the value of the given param using it as a key in the context storage dictionaries (context.storage or
     context.feature_storage) or in the context object itself. The key might be comprised of dotted tokens. In such case,
     the searched key is the first token. The rest of the tokens are considered nested properties/objects.
     So, for example, in the basic case, "last_request_result" could be used as key that would be searched into context
     storages or the context object itself. In a dotted case, "last_request.result" is searched as a "last_request" key
     in the context storages or as a property of the context object whose name is last_request. In both cases, when
     found, "result" is considered (and resolved) as a property or a key into the returned value.
+    If the resolved element at one of the tokens is a list, then the next token (if present) is used as the index
+    to select one of its elements, e.g. "list.1" returns the second element of the list "list".
 
     There is not limit in the nested levels of dotted tokens, so a key like a.b.c.d will be tried to be resolved as:
 
     context.storage['a'].b.c.d
         or
     context.a.b.c.d
 
     :param param: key to be searched (e.g. "last_request_result" / "last_request.result")
     :param context: behave context
     :return: mapped value
     """
     parts = param.split('.')
     value = _get_initial_value_from_context(parts[0], context)
+    msg = None
 
     for part in parts[1:]:
         if isinstance(value, dict) and part in value:
             value = value[part]
+        elif isinstance(value, list) and part.isdigit() and int(part) < len(value):
+            value = value[int(part)]
         elif hasattr(value, part):
             value = getattr(value, part)
         else:
-            if isinstance(value, dict):
-                msg = f"'{part}' key not found in {value} value in context"
-            else:
-                msg = f"'{part}' attribute not found in {type(value).__name__} class in context"
+            msg = _get_value_context_error_msg(value, part)
             logger.error(msg)
             raise Exception(msg)
     return value
 
 
+def _get_value_context_error_msg(value, part):
+    """
+    Returns an appropriate error message when an error occurs resolving a CONTEXT reference.
+
+    :param value: last value that has been correctly resolved
+    :param part: token that is causing the error
+    :return: a string with the error message
+    """
+    if isinstance(value, dict):
+        return f"'{part}' key not found in {value} value in context"
+    elif isinstance(value, list):
+        if part.isdigit():
+            return f"Invalid index '{part}', list size is '{len(value)}'. {part} >= {len(value)}."
+        else:
+            return f"the index '{part}' must be a numeric index"
+    else:
+        return f"'{part}' attribute not found in {type(value).__name__} class in context"
+
+
 def _get_initial_value_from_context(initial_key, context):
     """
     Find the value of the given initial_key using it as a key in the context storage dictionaries (context.storage or
     context.feature_storage) or in the context object itself.
 
     :param initial_key: key to be searched in context
     :param context: behave context
@@ -713,15 +734,15 @@
 
 
 def get_file(file_path):
     """
     Return the content of a file given its path. If a base path was previously set by using
     the set_file_path() function, the file path specified must be relative to that path.
 
-    :param file path: file path using slash as separator (e.g. "resources/files/doc.txt")
+    :param file_path: file path using slash as separator (e.g. "resources/files/doc.txt")
     :return: string with the file content
     """
     file_path_parts = (base_file_path + file_path).split("/")
     file_path = os.path.abspath(os.path.join(*file_path_parts))
     if not os.path.exists(file_path):
         raise Exception(f' ERROR - Cannot read file "{file_path}". Does not exist.')
 
@@ -730,15 +751,15 @@
 
 
 def convert_file_to_base64(file_path):
     """
     Return the content of a file given its path encoded in Base64. If a base path was previously set by using
     the set_file_path() function, the file path specified must be relative to that path.
 
-    :param file path: file path using slash as separator (e.g. "resources/files/doc.txt")
+    :param file_path: file path using slash as separator (e.g. "resources/files/doc.txt")
     :return: string with the file content encoded in Base64
     """
     file_path_parts = (base_base64_path + file_path).split("/")
     file_path = os.path.abspath(os.path.join(*file_path_parts))
     if not os.path.exists(file_path):
         raise Exception(f' ERROR - Cannot read file "{file_path}". Does not exist.')
```

### Comparing `toolium-3.0.2.dev0/toolium/utils/download_files.py` & `toolium-3.1.0.dev0/toolium/utils/download_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/utils/driver_utils.py` & `toolium-3.1.0.dev0/toolium/utils/driver_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/utils/driver_wait_utils.py` & `toolium-3.1.0.dev0/toolium/utils/driver_wait_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/utils/path_utils.py` & `toolium-3.1.0.dev0/toolium/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/utils/poeditor.py` & `toolium-3.1.0.dev0/toolium/utils/poeditor.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium/visual_test.py` & `toolium-3.1.0.dev0/toolium/visual_test.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2.dev0/toolium.egg-info/PKG-INFO` & `toolium-3.1.0.dev0/toolium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.2.dev0
+Version: 3.1.0.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.2.dev0/toolium.egg-info/SOURCES.txt` & `toolium-3.1.0.dev0/toolium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

