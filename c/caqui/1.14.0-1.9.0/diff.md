# Comparing `tmp/caqui-1.14.0.tar.gz` & `tmp/caqui-1.9.0.tar.gz`

## Comparing `caqui-1.14.0.tar` & `caqui-1.9.0.tar`

### file list

```diff
@@ -1,39 +1,34 @@
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.14.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.14.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 caqui-1.14.0/sample-appium.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 caqui-1.14.0/sample-win-app-driver.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 caqui-1.14.0/sample-winium.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 caqui-1.14.0/sample.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 caqui-1.14.0/test-requirements.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 caqui-1.14.0/tox.ini
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.14.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.14.0/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.14.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.14.0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.14.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.14.0/.vscode/settings.json
--rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.14.0/caqui/__init__.py
--rw-r--r--   0        0        0    17569 2020-02-02 00:00:00.000000 caqui-1.14.0/caqui/asynchronous.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.14.0/caqui/constants.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.14.0/caqui/exceptions.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.14.0/caqui/helper.py
--rw-r--r--   0        0        0    16967 2020-02-02 00:00:00.000000 caqui-1.14.0/caqui/synchronous.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/constants.py
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/fake_responses.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/test_sniffer.py
--rw-r--r--   0        0        0  5466526 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/apk/app-debug.apk
--rw-r--r--   0        0        0    15895 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/feature/test_sync_and_async.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/html/playground.html
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/integration/test_async_scenarios.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/integration/test_sync_scenarios.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/unit/__initi__.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/unit/test_async_unit.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/unit/test_helper.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 caqui-1.14.0/tests/unit/test_sync_unit.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.14.0/utils/coverage.sh
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 caqui-1.14.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.14.0/LICENSE
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 caqui-1.14.0/README.md
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 caqui-1.14.0/pyproject.toml
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 caqui-1.14.0/PKG-INFO
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 caqui-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 caqui-1.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 caqui-1.9.0/sample.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 caqui-1.9.0/test-requirements.txt
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 caqui-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 caqui-1.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0    43559 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/__init__.py
+-rw-r--r--   0        0        0    10603 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/asynchronous.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/constants.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/exceptions.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/helper.py
+-rw-r--r--   0        0        0    10062 2020-02-02 00:00:00.000000 caqui-1.9.0/caqui/synchronous.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/constants.py
+-rw-r--r--   0        0        0     5333 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/fake_responses.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/test_sniffer.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/feature/test_sync_and_async.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/html/playground.html
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/integration/test_async_scenarios.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/integration/test_sync_scenarios.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/__initi__.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_async_unit.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_helper.py
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 caqui-1.9.0/tests/unit/test_sync_unit.py
+-rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 caqui-1.9.0/utils/coverage.sh
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 caqui-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 caqui-1.9.0/LICENSE
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 caqui-1.9.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 caqui-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10401 2020-02-02 00:00:00.000000 caqui-1.9.0/PKG-INFO
```

### Comparing `caqui-1.14.0/CODE_OF_CONDUCT.md` & `caqui-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/sample.py` & `caqui-1.9.0/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# It opens the WebDriver, navigate to a page and get all links
 import asyncio
 import time
 from caqui import synchronous, asynchronous
 from os import getcwd
 from tests.constants import PAGE_URL
 
 BASE_DIR = getcwd()
```

### Comparing `caqui-1.14.0/.github/ISSUE_TEMPLATE/bug_report.md` & `caqui-1.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/.github/ISSUE_TEMPLATE/feature_request.md` & `caqui-1.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/.github/workflows/python-app.yml` & `caqui-1.9.0/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/.github/workflows/python-publish.yml` & `caqui-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/caqui/__init__.py` & `caqui-1.9.0/caqui/__init__.py`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/tests/fake_responses.py` & `caqui-1.9.0/tests/fake_responses.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,33 +4,20 @@
 class Dictionary:
     def __init__(self, dictionary) -> None:
         self.dictionary = dictionary
 
     def json(self):
         return self.dictionary
 
-    # used by sync functions
-    def get(self, key, *args):
+    def get(self, key):
         return self.dictionary.get(key)
 
 
 def dict_to_json(dictionary):
-    class MockResponse:
-        @property
-        def status_code(self):
-            return 200
-
-        # used by async functions
-        def get(self, argument, *args):
-            return dictionary.get(argument)
-
-        def json(self):
-            return Dictionary(dictionary)
-
-    return MockResponse()
+    return Dictionary(dictionary)
 
 
 DEFAULT = dict_to_json(
     {
         "sessionId": "4358a5b53794586af59678fc1653dc40",
         "status": 0,
         "value": {"ELEMENT": "0.8851292311864847-1"},
@@ -39,51 +26,22 @@
 
 FIND_ELEMENT = DEFAULT
 SEND_KEYS = DEFAULT
 CLICK = DEFAULT
 CLOSE_SESSION = DEFAULT
 GO_TO_PAGE = DEFAULT
 
-GET_RECT = dict_to_json(
-    {
-        "sessionId": "a9d6e77726f3eda12e92b06b5066dbb4",
-        "status": 0,
-        "value": {"height": 23, "width": 183, "x": 10, "y": 9652.12},
-    }
-)
-
-ACTIONS = dict_to_json(
-    {"sessionId": "449dbd1df001e9a9e13b3bac5babe809", "status": 0, "value": "null"}
-)
-
-EXECUTE_SCRIPT = dict_to_json(
-    {"sessionId": "9f4a4a9420663d0c0cc18957ab463b90", "status": 0, "value": "any"}
-)
-
-GET_PAGE_SOURCE = dict_to_json(
-    {
-        "sessionId": "e34234d1445ed6d4833370d1d8019282",
-        "status": 0,
-        "value": "<html><head><title>Sample page</title></head><body><h1>Basic page</h1></body></html>",
-    }
-)
-
-GET_ALERT_TEXT = dict_to_json(
-    {"sessionId": "171ba19c927e0b95e1a53dbbdcfcdc19", "status": 0, "value": "any warn"}
-)
-
 GET_WINDOW_RECTANGLE = dict_to_json(
     {
         "sessionId": "79e4bd950a886e0119e3760d201b059e",
         "status": 0,
         "value": {"height": 600, "width": 800, "x": 0, "y": 0},
     }
 )
 
-GET_ACTIVE_ELEMENT = DEFAULT
 
 CLEAR_ELEMENT = dict_to_json(
     {"sessionId": "486fa32a9876b4519e149b39135edcb5", "status": 0, "value": None}
 )
 
 IS_ELEMENT_ENABLED = dict_to_json(
     {"sessionId": "e0e43cd1ce532b5aa62b6df0de11e3bd", "status": 0, "value": True}
@@ -142,16 +100,15 @@
         "value": {
             "build": {
                 "version": "113.0.5672.63 (0e1a4471d5ae5bf128b1bd8f4d627c8cbd55f70c-refs/branch-heads/5672@{#912})"
             },
             "message": "ChromeDriver ready for new sessions.",
             "os": {"arch": "x86_64", "name": "Linux", "version": "5.4.0-150-generic"},
             "ready": True,
-        },
-        "status": "0",  # fake status fro mock purposes. Not present in real response
+        }
     }
 )
 
 GET_TITLE = dict_to_json(
     {
         "sessionId": "07b00b2e94be84920495d83890c82b60",
         "status": 0,
```

### Comparing `caqui-1.14.0/tests/test_sniffer.py` & `caqui-1.9.0/tests/test_sniffer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 #### File used to figure out requests format and parameters ####
 
 from selenium import webdriver
 from pytest import fixture, mark
 from tests.constants import PAGE_URL
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.action_chains import ActionChains
-from selenium.webdriver.chrome.service import Service
-from selenium.webdriver.chrome.options import Options
-import os
 
 
 @fixture
 def setup():
     desired_capabilities = {
         # 'deviceName': 'Device',
         "deviceName": "Emulator",
@@ -27,70 +22,14 @@
     )
     driver.get(PAGE_URL)
     driver
     yield driver
     driver.quit()
 
 
-@fixture
-def setup_binary():
-    homedir = os.path.expanduser("~")
-    service = Service(f"/home/douglas/web_drivers/chromedriver.113")
-    options = Options()
-    # options.add_argument('--headless')
-    options.add_argument("window-size=1920,1080")
-    browser = webdriver.Chrome(service=service, options=options)
-    browser.get(PAGE_URL)
-    yield browser
-    # browser.quit()
-
-
-@mark.skip("used just to discover request data")
-def test_submit(setup):
-    driver = setup
-    search_button = driver.find_element("name", "my-form")
-    search_button.submit()
-
-
-@mark.skip("used just to discover request data")
-def test_sniffer_is_displayed(setup_binary):
-    driver = setup_binary
-    search_button = driver.find_element("xpath", "//button")
-    search_button.is_displayed()
-
-
-@mark.skip("used just to discover request data")
-def test_sniffer_actions_scroll_to_element(setup_binary):
-    driver = setup_binary
-    search_button = driver.find_element("xpath", "//button")
-    ActionChains(driver).scroll_to_element(search_button).perform()
-
-
-@mark.skip("used just to discover request data")
-def test_sniffer_actions_click(setup):
-    driver = setup
-    search_button = driver.find_element("xpath", "//button")
-    ActionChains(driver).click(search_button).perform()
-
-
-@mark.skip("used just to discover request data")
-def test_sniffer_find_children_elements(setup):
-    driver = setup
-    element = driver.find_element(By.XPATH, '//div[@class="parent"]')
-    elements = element.find_elements(By.XPATH, "//div")
-    for e in elements:
-        print("element_text:", e.text)
-
-
-@mark.skip("used just to discover request data")
-def test_exec_script(setup):
-    driver = setup
-    assert driver.execute_script("return document.body.scrollHeight") == "any"
-
-
 @mark.skip("used just to discover request data")
 def test_clear(setup):
     driver = setup
     element = driver.find_element("xpath", "//input")
     assert element.clear() == "any"
```

### Comparing `caqui-1.14.0/tests/feature/test_sync_and_async.py` & `caqui-1.9.0/tests/feature/test_sync_and_async.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from pytest import fixture, mark, raises
+from pytest import fixture, mark
 from caqui import asynchronous, synchronous
 from tests.constants import PAGE_URL
-from caqui.exceptions import WebDriverError
 
 
 @fixture
 def __setup():
     driver_url = "http://127.0.0.1:9999"
     capabilities = {
         "desiredCapabilities": {
             "name": "webdriver",
-            "browserName": "chrome",
+            "browserName": "firefox",
             "marionette": True,
             "acceptInsecureCerts": True,
             "goog:chromeOptions": {"extensions": [], "args": ["--headless"]},
         }
     }
     session = synchronous.get_session(driver_url, capabilities)
     synchronous.go_to_page(
@@ -23,211 +22,14 @@
         PAGE_URL,
     )
     yield driver_url, session
     synchronous.close_session(driver_url, session)
 
 
 @mark.asyncio
-async def test_get_rect(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-    locator_value = "//input"
-    expected = {"height": 21, "width": 185, "x": 8, "y": 100.4375}
-
-    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
-
-    assert synchronous.get_rect(driver_url, session, element) == expected
-
-    assert await asynchronous.get_rect(driver_url, session, element) == expected
-
-
-@mark.asyncio
-async def test_actions_scroll_to_element(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-    locator_value = "//button"
-
-    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
-    assert synchronous.actions_scroll_to_element(driver_url, session, element) is True
-    assert (
-        await asynchronous.actions_scroll_to_element(driver_url, session, element)
-        is True
-    )
-
-
-@mark.asyncio
-async def test_submit(__setup):
-    driver_url, session = __setup
-    locator_type = "name"
-    locator_value = "my-form"
-
-    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
-    assert synchronous.submit(driver_url, session, element) is True
-
-    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
-    assert await asynchronous.submit(driver_url, session, element) is True
-
-
-@mark.asyncio
-async def test_actions_click(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-    locator_value = "//button"
-
-    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
-    assert synchronous.actions_click(driver_url, session, element) is True
-    assert await asynchronous.actions_click(driver_url, session, element) is True
-
-
-@mark.asyncio
-async def test_raise_exception_when_element_not_found(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-    locator_value = "//invalid-tag"
-
-    with raises(WebDriverError):
-        synchronous.find_element(driver_url, session, locator_type, locator_value)
-
-    with raises(WebDriverError):
-        await asynchronous.find_element(
-            driver_url, session, locator_type, locator_value
-        )
-
-
-@mark.asyncio
-async def test_set_timeouts(__setup):
-    driver_url, session = __setup
-    timeouts_1 = 5000  # milliseconds
-    timeouts_2 = 3000  # milliseconds
-
-    synchronous.set_timeouts(driver_url, session, timeouts_1)
-
-    assert synchronous.get_timeouts(driver_url, session).get("implicit") == timeouts_1
-
-    await asynchronous.set_timeouts(driver_url, session, timeouts_2)
-
-    assert synchronous.get_timeouts(driver_url, session).get("implicit") == timeouts_2
-
-
-@mark.asyncio
-async def test_find_children_elements(__setup):
-    driver_url, session = __setup
-    expected = 5  # parent inclusive
-    locator_type = "xpath"
-    locator_value = "//div"
-
-    parent_element = synchronous.find_element(
-        driver_url, session, locator_type, '//div[@class="parent"]'
-    )
-
-    children_elements = synchronous.find_children_elements(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-
-    assert len(children_elements) == expected
-
-    children_elements = await asynchronous.find_children_elements(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-
-    assert len(children_elements) == expected
-
-
-@mark.asyncio
-async def test_find_child_element(__setup):
-    driver_url, session = __setup
-    expected = "any4"
-    locator_type = "xpath"
-    locator_value = '//div[@class="child4"]'
-
-    parent_element = synchronous.find_element(
-        driver_url, session, locator_type, '//div[@class="parent"]'
-    )
-
-    child_element = synchronous.find_child_element(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-
-    text = synchronous.get_text(driver_url, session, child_element)
-
-    assert text == expected
-    child_element = await asynchronous.find_child_element(
-        driver_url, session, parent_element, locator_type, locator_value
-    )
-    text = synchronous.get_text(driver_url, session, child_element)
-    assert text == expected
-
-
-@mark.asyncio
-async def test_get_page_source(__setup):
-    driver_url, session = __setup
-    expected = "Sample page"
-
-    assert expected in synchronous.get_page_source(driver_url, session)
-    assert expected in await asynchronous.get_page_source(driver_url, session)
-
-
-@mark.asyncio
-async def test_execute_script_asynchronous(__setup):
-    driver_url, session = __setup
-    script = "alert('any warn')"
-
-    assert await asynchronous.execute_script(driver_url, session, script) == None
-
-
-def test_execute_script_synchronous(__setup):
-    driver_url, session = __setup
-    script = "alert('any warn')"
-
-    assert synchronous.execute_script(driver_url, session, script) == None
-
-
-@mark.asyncio
-async def test_get_alert_text(__setup):
-    driver_url, session = __setup
-    locator_type = "css selector"
-    locator_value = "#alert-button"
-    expected = "any warn"
-
-    alert_button = synchronous.find_element(
-        driver_url, session, locator_type, locator_value
-    )
-    synchronous.click(driver_url, session, alert_button)
-
-    assert synchronous.get_alert_text(driver_url, session) == expected
-    assert await asynchronous.get_alert_text(driver_url, session) == expected
-
-
-@mark.asyncio
-async def test_get_active_element(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-    locator_value = "//input"
-
-    element = synchronous.find_element(driver_url, session, locator_type, locator_value)
-    synchronous.send_keys(driver_url, session, element, "any")
-
-    assert synchronous.get_active_element(driver_url, session) == element
-    assert await asynchronous.get_active_element(driver_url, session) == element
-
-
-@mark.asyncio
-async def test_clear_element_fails_when_invalid_inputs(__setup):
-    driver_url, session = __setup
-    text = "any"
-    element = "invalid"
-
-    with raises(WebDriverError):
-        synchronous.clear_element(driver_url, session, element) is True
-
-    with raises(WebDriverError):
-        await asynchronous.clear_element(driver_url, session, element)
-
-
-@mark.asyncio
 async def test_clear_element(__setup):
     driver_url, session = __setup
     locator_type = "xpath"
     locator_value = "//input"
     text = "any"
 
     element = synchronous.find_element(driver_url, session, locator_type, locator_value)
@@ -319,27 +121,14 @@
     driver_url, session = __setup
 
     assert synchronous.get_window(driver_url, session) is not None
     assert await asynchronous.get_window(driver_url, session) is not None
 
 
 @mark.asyncio
-async def test_get_attribute_fails_when_invalid_attribute(__setup):
-    driver_url, session = __setup
-    attribute = "href"
-    element = "invalid"
-
-    with raises(WebDriverError):
-        synchronous.get_attribute(driver_url, session, element, attribute)
-
-    with raises(WebDriverError):
-        await asynchronous.get_attribute(driver_url, session, element, attribute)
-
-
-@mark.asyncio
 async def test_get_attribute(__setup):
     driver_url, session = __setup
     attribute = "href"
     element = synchronous.find_element(driver_url, session, "xpath", "//a[@id='a1']")
 
     assert (
         synchronous.get_attribute(driver_url, session, element, attribute)
@@ -401,29 +190,14 @@
     expected = "Sample page"
 
     assert synchronous.get_title(driver_url, session) == expected
     assert await asynchronous.get_title(driver_url, session) == expected
 
 
 @mark.asyncio
-async def test_find_elements_fails_when_invalid_data_input(__setup):
-    driver_url, session = __setup
-    locator_type = "invalid"
-    locator_value = "//input"
-
-    with raises(WebDriverError):
-        synchronous.find_elements(driver_url, session, locator_type, locator_value)
-
-    with raises(WebDriverError):
-        await asynchronous.find_elements(
-            driver_url, session, locator_type, locator_value
-        )
-
-
-@mark.asyncio
 async def test_find_elements(__setup):
     driver_url, session = __setup
     locator_type = "xpath"
     locator_value = "//input"
 
     elements = synchronous.find_elements(
         driver_url, session, locator_type, locator_value
@@ -433,29 +207,14 @@
     )
 
     assert len(elements) > 0
     assert len(async_elements) > 0
 
 
 @mark.asyncio
-async def test_find_element_fails_when_invalid_data_input(__setup):
-    driver_url, session = __setup
-    locator_type = "invalid"
-    locator_value = "//input"
-
-    with raises(WebDriverError):
-        synchronous.find_element(driver_url, session, locator_type, locator_value)
-
-    with raises(WebDriverError):
-        await asynchronous.find_element(
-            driver_url, session, locator_type, locator_value
-        )
-
-
-@mark.asyncio
 async def test_find_element(__setup):
     driver_url, session = __setup
     locator_type = "xpath"
     locator_value = "//input"
 
     assert (
         synchronous.find_element(driver_url, session, locator_type, locator_value)
```

### Comparing `caqui-1.14.0/tests/integration/test_async_scenarios.py` & `caqui-1.9.0/tests/integration/test_async_scenarios.py`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/tests/integration/test_sync_scenarios.py` & `caqui-1.9.0/tests/integration/test_sync_scenarios.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,14 @@
     click,
     send_keys,
     get_text,
     close_session,
     go_to_page,
     get_property,
     clear_element,
-    get_rect,
-    get_css_value,
-    get_attribute,
 )
 from tests.constants import PAGE_URL
 from pytest import fixture
 
 
 @fixture
 def __setup():
@@ -33,31 +30,14 @@
         session,
         PAGE_URL,
     )
     yield driver_url, session
     close_session(driver_url, session)
 
 
-def test_get_data_from_hidden_button(__setup):
-    driver_url, session = __setup
-    locator_type = "xpath"
-
-    hidden_button = find_element(
-        driver_url, session, locator_type, locator_value="//*[@id='hidden-button']"
-    )
-
-    assert "width" in get_rect(driver_url, session, hidden_button)
-    assert "visible" == get_css_value(driver_url, session, hidden_button, "visibility")
-    assert True == get_property(driver_url, session, hidden_button, "hidden")
-    assert ["display"] == get_property(driver_url, session, hidden_button, "style")
-    assert "display: none;" == get_attribute(
-        driver_url, session, hidden_button, "style"
-    )
-
-
 def test_add_text__click_button_and_get_properties(__setup):
     driver_url, session = __setup
     expected = "end"
     locator_type = "xpath"
 
     input = find_element(driver_url, session, locator_type, locator_value="//input")
     send_keys(driver_url, session, input, "any")
```

### Comparing `caqui-1.14.0/tests/unit/test_async_unit.py` & `caqui-1.9.0/tests/unit/test_async_unit.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,127 +8,14 @@
 
 
 async def mock_request(*args):
     pass
 
 
 @mark.asyncio
-async def test_get_rect():
-    expected = {"height": 23, "width": 183, "x": 10, "y": 9652.12}
-
-    async def mock_request(*args):
-        return fake_responses.GET_RECT
-
-    with patch("caqui.asynchronous.__get", mock_request):
-        assert await asynchronous.get_rect("", "", "") == expected
-
-
-@mark.asyncio
-async def test_actions_scroll_to_element():
-    async def mock_request(*args):
-        return fake_responses.ACTIONS
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.actions_scroll_to_element("", "", "") == True
-
-
-@mark.asyncio
-async def test_submit():
-    async def mock_request(*args):
-        return fake_responses.CLICK
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.submit("", "", "") == True
-
-
-@mark.asyncio
-async def test_actions_click():
-    async def mock_request(*args):
-        return fake_responses.ACTIONS
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.actions_click("", "", "") == True
-
-
-@mark.asyncio
-async def test_set_timeouts():
-    async def mock_request(*args):
-        return fake_responses.GET_TIMEOUTS
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.set_timeouts("", "", "") == True
-
-
-@mark.asyncio
-async def test_find_children_elements():
-    element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
-
-    async def mock_request(*args):
-        return fake_responses.FIND_ELEMENTS
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert element in await asynchronous.find_children_elements("", "", "", "", "")
-
-
-@mark.asyncio
-async def test_find_child_element():
-    element = "0.8851292311864847-1"
-
-    async def mock_request(*args):
-        return fake_responses.FIND_ELEMENT
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.find_child_element("", "", "", "", "") == element
-
-
-@mark.asyncio
-async def test_execute_script():
-    expected = "any"
-
-    async def mock_request(*args):
-        return fake_responses.EXECUTE_SCRIPT
-
-    with patch("caqui.asynchronous.__post", mock_request):
-        assert await asynchronous.execute_script("", "", "", "") == expected
-
-
-@mark.asyncio
-async def test_get_page_source():
-    expected = "Sample page"
-
-    async def mock_request(*args):
-        return fake_responses.GET_PAGE_SOURCE
-
-    with patch("caqui.asynchronous.__get", mock_request):
-        assert expected in await asynchronous.get_page_source("", "")
-
-
-@mark.asyncio
-async def test_get_alert_text():
-    expected = "any warn"
-
-    async def mock_request(*args):
-        return fake_responses.GET_ALERT_TEXT
-
-    with patch("caqui.asynchronous.__get", mock_request):
-        assert await asynchronous.get_alert_text("", "") == expected
-
-
-@mark.asyncio
-async def test_get_active_element():
-    expected = "0.8851292311864847-1"
-
-    async def mock_request(*args):
-        return fake_responses.GET_ACTIVE_ELEMENT
-
-    with patch("caqui.asynchronous.__get", mock_request):
-        assert await asynchronous.get_active_element("", "") == expected
-
-
-@mark.asyncio
 async def test_clear_element():
     async def mock_request(*args):
         return fake_responses.CLEAR_ELEMENT
 
     with patch("caqui.asynchronous.__post", mock_request):
         assert await asynchronous.clear_element("", "", "") is True
```

### Comparing `caqui-1.14.0/tests/unit/test_helper.py` & `caqui-1.9.0/tests/unit/test_helper.py`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/tests/unit/test_sync_unit.py` & `caqui-1.9.0/tests/unit/test_sync_unit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,12 @@
 from unittest.mock import patch
 from caqui import synchronous
 from tests import fake_responses
 
 
-@patch("requests.request", return_value=fake_responses.GET_RECT)
-def test_get_rect(*args):
-    expected = {"height": 23, "width": 183, "x": 10, "y": 9652.12}
-    assert synchronous.get_rect("", "", "") == expected
-
-
-@patch("requests.request", return_value=fake_responses.ACTIONS)
-def test_actions_scroll_to_element(*args):
-    assert synchronous.actions_scroll_to_element("", "", "") == True
-
-
-@patch("requests.request", return_value=fake_responses.CLICK)
-def test_submit(*args):
-    assert synchronous.submit("", "", "") == True
-
-
-@patch("requests.request", return_value=fake_responses.ACTIONS)
-def test_actions_click(*args):
-    assert synchronous.actions_click("", "", "") == True
-
-
-@patch("requests.request", return_value=fake_responses.GET_TIMEOUTS)
-def test_set_timeouts(*args):
-    assert synchronous.set_timeouts("", "", "") == True
-
-
-@patch("requests.request", return_value=fake_responses.FIND_ELEMENTS)
-def test_find_children_elements(*args):
-    element = "C230605181E69CB2C4C36B8E83FE1245_element_2"
-
-    elements = synchronous.find_children_elements("", "", "", "", "")
-
-    assert element in elements
-    assert len(elements) == 3
-
-
-@patch("requests.request", return_value=fake_responses.FIND_ELEMENT)
-def test_find_child_element(*args):
-    expected = "0.8851292311864847-1"
-
-    assert synchronous.find_child_element("", "", "", "", "") == expected
-
-
-@patch("requests.request", return_value=fake_responses.EXECUTE_SCRIPT)
-def test_execute_script(*args):
-    expected = "any"
-
-    assert synchronous.execute_script("", "", "", "") == expected
-
-
-@patch("requests.request", return_value=fake_responses.GET_PAGE_SOURCE)
-def test_get_page_source(*args):
-    expected = "Sample page"
-    assert expected in synchronous.get_page_source("", "")
-
-
-@patch("requests.request", return_value=fake_responses.GET_ALERT_TEXT)
-def test_get_alert_text(*args):
-    expected = "any warn"
-    assert synchronous.get_alert_text("", "") == expected
-
-
-@patch("requests.request", return_value=fake_responses.GET_ACTIVE_ELEMENT)
-def test_get_active_element(*args):
-    expected = "0.8851292311864847-1"
-    assert synchronous.get_active_element("", "") == expected
-
-
 @patch("requests.request", return_value=fake_responses.CLEAR_ELEMENT)
 def test_clear_element(*args):
     assert synchronous.clear_element("", "", "") is True
 
 
 @patch("requests.request", return_value=fake_responses.IS_ELEMENT_ENABLED)
 def test_is_element_enabled(*args):
```

### Comparing `caqui-1.14.0/.gitignore` & `caqui-1.9.0/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -118,15 +118,14 @@
 
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
 .venv
-venv*
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
 # Spyder project settings
```

### Comparing `caqui-1.14.0/LICENSE` & `caqui-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caqui-1.14.0/README.md` & `caqui-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,40 @@
+Metadata-Version: 2.1
+Name: caqui
+Version: 1.9.0
+Summary: Run asynchronous commands in WebDrivers
+Project-URL: Homepage, https://github.com/douglasdcm/caqui
+Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
+Author-email: Douglas Cardoso <noemail@noemail.com>
+License-File: LICENSE
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: aiohttp
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # Caqui
 
 **Caqui** is intended to command executions against Drivers synchronously and asynchronously. Launch the Driver as a server and send requests to it. The intention is that the user does not worry about which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/Winium.Desktop).
 
 The process **Caqui** follows is similar of the one described in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However, the motivation to create **Caqui** was feed by the inspiration in [Arsenic](https://github.com/HENNGE/arsenic) library.
 
 **Caqui** is planned to be Driver agnostic, so the user can start any Driver as a server and just inform the server URL. Hence, the code is decoupled from the chosen Driver.
 
 **Caqui** can be used in remote calls. As it needs just the server URL, the user can start the Driver as a server in any host and provide the URL to **Caqui** clients.
 
 # Tested WebDrivers
 
-| WebDriver               | Version       | Remote* | Comment |
-| ----------------------- | ------------- | ------- |-------- |
-| Appium                  | 2.0.0         | Y       | Accepts remote calls by default. Tested with Appium in Docker container |
-| Firefox (geckodriver)   | 113           | Y       | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome           | 113, 114      | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78" |
-| Opera                   | 99            | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome |
-| WinAppDriver            | 1.2.1         | Y       | Need to define the host ip, e.g. "WinAppDriver.exe 10.0.0.10 4723" |
-| Winium Desktop          | 1.6.0         | Y       | Accepts remote calls by default |
-
-* Accepts remote requests when running as servers
+| WebDriver               | Version       |
+| ----------------------- | ------------- |
+| Google Chrome           | 113, 114      |
+| Firefox (geckodriver)   | 113           |
 
 # Simple start
 Install the lastest version of **Caqui**
 
 ```
 pip install caqui
 ```
```

#### html2text {}

```diff
@@ -1,37 +1,37 @@
-# Caqui **Caqui** is intended to command executions against Drivers
-synchronously and asynchronously. Launch the Driver as a server and send
-requests to it. The intention is that the user does not worry about which
-Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
+Metadata-Version: 2.1 Name: caqui Version: 1.9.0 Summary: Run asynchronous
+commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
+caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
+Author-email: Douglas Cardoso
+noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
+Python: >=3.7 Requires-Dist: aiohttp Requires-Dist: requests Description-
+Content-Type: text/markdown # Caqui **Caqui** is intended to command executions
+against Drivers synchronously and asynchronously. Launch the Driver as a server
+and send requests to it. The intention is that the user does not worry about
+which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
 www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/
 2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/
 Winium.Desktop). The process **Caqui** follows is similar of the one described
 in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-
 http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with
 [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However,
 the motivation to create **Caqui** was feed by the inspiration in [Arsenic]
 (https://github.com/HENNGE/arsenic) library. **Caqui** is planned to be Driver
 agnostic, so the user can start any Driver as a server and just inform the
 server URL. Hence, the code is decoupled from the chosen Driver. **Caqui** can
 be used in remote calls. As it needs just the server URL, the user can start
 the Driver as a server in any host and provide the URL to **Caqui** clients. #
-Tested WebDrivers | WebDriver | Version | Remote* | Comment | | ---------------
--------- | ------------- | ------- |-------- | | Appium | 2.0.0 | Y | Accepts
-remote calls by default. Tested with Appium in Docker container | | Firefox
-(geckodriver) | 113 | Y | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome | 113, 114 | Y | Need to inform allowed ips to connect, e.g "--
-allowed-ips=123.45.6.78" | | Opera | 99 | Y | Need to inform allowed ips to
-connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome | |
-WinAppDriver | 1.2.1 | Y | Need to define the host ip, e.g. "WinAppDriver.exe
-10.0.0.10 4723" | | Winium Desktop | 1.6.0 | Y | Accepts remote calls by
-default | * Accepts remote requests when running as servers # Simple start
-Install the lastest version of **Caqui** ``` pip install caqui ``` Download the
-same [ChromeDriver](https://chromedriver.chromium.org/downloads) version as
-your installed Chrome and start the Driver as a server using the port "9999"
-``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
+Tested WebDrivers | WebDriver | Version | | ----------------------- | ---------
+---- | | Google Chrome | 113, 114 | | Firefox (geckodriver) | 113 | # Simple
+start Install the lastest version of **Caqui** ``` pip install caqui ```
+Download the same [ChromeDriver](https://chromedriver.chromium.org/downloads)
+version as your installed Chrome and start the Driver as a server using the
+port "9999" ``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
 (418b78f5838ed0b1c69bb4e51ea0252171854915-refs/branch-heads/4606@{#1204}) on
 port 9999 Only local connections are allowed. Please see https://
 chromedriver.chromium.org/security-considerations for suggestions on keeping
 ChromeDriver safe. ChromeDriver was started successfully. ``` Given the HTML
 content in `playground.html` ```
 ****** Basic page ******
 This is a sample page to be used to sanity check
```

### Comparing `caqui-1.14.0/pyproject.toml` & `caqui-1.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 [tool.setuptools.packages.find]
 include = ["caqui*"]
 exclude = ["tests*", "utils", ".vscode", ".git*", "dist"]
 
 [project]
 name = "caqui"
-version = "1.14.0"
+version = "1.9.0"
 authors = [
   { name="Douglas Cardoso", email="noemail@noemail.com" },
 ]
 description = "Run asynchronous commands in WebDrivers"
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `caqui-1.14.0/PKG-INFO` & `caqui-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,23 @@
-Metadata-Version: 2.1
-Name: caqui
-Version: 1.14.0
-Summary: Run asynchronous commands in WebDrivers
-Project-URL: Homepage, https://github.com/douglasdcm/caqui
-Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
-Author-email: Douglas Cardoso <noemail@noemail.com>
-License-File: LICENSE
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Requires-Dist: aiohttp
-Requires-Dist: requests
-Description-Content-Type: text/markdown
-
 # Caqui
 
 **Caqui** is intended to command executions against Drivers synchronously and asynchronously. Launch the Driver as a server and send requests to it. The intention is that the user does not worry about which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/Winium.Desktop).
 
 The process **Caqui** follows is similar of the one described in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However, the motivation to create **Caqui** was feed by the inspiration in [Arsenic](https://github.com/HENNGE/arsenic) library.
 
 **Caqui** is planned to be Driver agnostic, so the user can start any Driver as a server and just inform the server URL. Hence, the code is decoupled from the chosen Driver.
 
 **Caqui** can be used in remote calls. As it needs just the server URL, the user can start the Driver as a server in any host and provide the URL to **Caqui** clients.
 
 # Tested WebDrivers
 
-| WebDriver               | Version       | Remote* | Comment |
-| ----------------------- | ------------- | ------- |-------- |
-| Appium                  | 2.0.0         | Y       | Accepts remote calls by default. Tested with Appium in Docker container |
-| Firefox (geckodriver)   | 113           | Y       | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome           | 113, 114      | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78" |
-| Opera                   | 99            | Y       | Need to inform allowed ips to connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome |
-| WinAppDriver            | 1.2.1         | Y       | Need to define the host ip, e.g. "WinAppDriver.exe 10.0.0.10 4723" |
-| Winium Desktop          | 1.6.0         | Y       | Accepts remote calls by default |
-
-* Accepts remote requests when running as servers
+| WebDriver               | Version       |
+| ----------------------- | ------------- |
+| Google Chrome           | 113, 114      |
+| Firefox (geckodriver)   | 113           |
 
 # Simple start
 Install the lastest version of **Caqui**
 
 ```
 pip install caqui
 ```
```

#### html2text {}

```diff
@@ -1,45 +1,29 @@
-Metadata-Version: 2.1 Name: caqui Version: 1.14.0 Summary: Run asynchronous
-commands in WebDrivers Project-URL: Homepage, https://github.com/douglasdcm/
-caqui Project-URL: Bug Tracker, https://github.com/douglasdcm/caqui/issues
-Author-email: Douglas Cardoso
-noemail.com> License-File: LICENSE Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Requires-
-Python: >=3.6 Requires-Dist: aiohttp Requires-Dist: requests Description-
-Content-Type: text/markdown # Caqui **Caqui** is intended to command executions
-against Drivers synchronously and asynchronously. Launch the Driver as a server
-and send requests to it. The intention is that the user does not worry about
-which Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
+# Caqui **Caqui** is intended to command executions against Drivers
+synchronously and asynchronously. Launch the Driver as a server and send
+requests to it. The intention is that the user does not worry about which
+Driver he/she is using. It can be **Web**Drivers like [Selenium](https://
 www.selenium.dev/), **Mobile**Drivers like [Appium](http://appium.io/docs/en/
 2.0/), or **Desktop**Drivers like [Winium](https://github.com/2gis/
 Winium.Desktop). The process **Caqui** follows is similar of the one described
 in this [article](https://medium.com/@douglas.dcm/testing-windows-apps-with-
 http-rest-b4e8f80f8b7e) that experiments Drivers as servers together with
 [Jmeter](https://jmeter.apache.org/) to test the Windows Calculator. However,
 the motivation to create **Caqui** was feed by the inspiration in [Arsenic]
 (https://github.com/HENNGE/arsenic) library. **Caqui** is planned to be Driver
 agnostic, so the user can start any Driver as a server and just inform the
 server URL. Hence, the code is decoupled from the chosen Driver. **Caqui** can
 be used in remote calls. As it needs just the server URL, the user can start
 the Driver as a server in any host and provide the URL to **Caqui** clients. #
-Tested WebDrivers | WebDriver | Version | Remote* | Comment | | ---------------
--------- | ------------- | ------- |-------- | | Appium | 2.0.0 | Y | Accepts
-remote calls by default. Tested with Appium in Docker container | | Firefox
-(geckodriver) | 113 | Y | Need to add the host ip, e.g. "--host 123.45.6.78" |
-| Google Chrome | 113, 114 | Y | Need to inform allowed ips to connect, e.g "--
-allowed-ips=123.45.6.78" | | Opera | 99 | Y | Need to inform allowed ips to
-connect, e.g "--allowed-ips=123.45.6.78". Similar to Google Chrome | |
-WinAppDriver | 1.2.1 | Y | Need to define the host ip, e.g. "WinAppDriver.exe
-10.0.0.10 4723" | | Winium Desktop | 1.6.0 | Y | Accepts remote calls by
-default | * Accepts remote requests when running as servers # Simple start
-Install the lastest version of **Caqui** ``` pip install caqui ``` Download the
-same [ChromeDriver](https://chromedriver.chromium.org/downloads) version as
-your installed Chrome and start the Driver as a server using the port "9999"
-``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
+Tested WebDrivers | WebDriver | Version | | ----------------------- | ---------
+---- | | Google Chrome | 113, 114 | | Firefox (geckodriver) | 113 | # Simple
+start Install the lastest version of **Caqui** ``` pip install caqui ```
+Download the same [ChromeDriver](https://chromedriver.chromium.org/downloads)
+version as your installed Chrome and start the Driver as a server using the
+port "9999" ``` $ ./chromedriver --port=9999 Starting ChromeDriver 94.0.4606.61
 (418b78f5838ed0b1c69bb4e51ea0252171854915-refs/branch-heads/4606@{#1204}) on
 port 9999 Only local connections are allowed. Please see https://
 chromedriver.chromium.org/security-considerations for suggestions on keeping
 ChromeDriver safe. ChromeDriver was started successfully. ``` Given the HTML
 content in `playground.html` ```
 ****** Basic page ******
 This is a sample page to be used to sanity check
```

