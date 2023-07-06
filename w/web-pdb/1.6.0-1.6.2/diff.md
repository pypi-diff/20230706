# Comparing `tmp/web-pdb-1.6.0.tar.gz` & `tmp/web-pdb-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-pdb-1.6.0.tar", last modified: Wed Apr 26 16:03:11 2023, max compression
+gzip compressed data, was "web-pdb-1.6.2.tar", last modified: Thu Jul  6 19:52:22 2023, max compression
```

## Comparing `web-pdb-1.6.0.tar` & `web-pdb-1.6.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.789504 web-pdb-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-26 16:03:02.000000 web-pdb-1.6.0/Changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 16:03:02.000000 web-pdb-1.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 16:03:02.000000 web-pdb-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-26 16:03:11.789504 web-pdb-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-04-26 16:03:02.000000 web-pdb-1.6.0/Readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 16:03:02.000000 web-pdb-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-26 16:03:11.789504 web-pdb-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-26 16:03:02.000000 web-pdb-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.785503 web-pdb-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 16:03:02.000000 web-pdb-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 16:03:02.000000 web-pdb-1.6.0/tests/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-26 16:03:02.000000 web-pdb-1.6.0/tests/db_i.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-26 16:03:02.000000 web-pdb-1.6.0/tests/db_pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-26 16:03:02.000000 web-pdb-1.6.0/tests/db_ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-04-26 16:03:02.000000 web-pdb-1.6.0/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.785503 web-pdb-1.6.0/web_pdb/
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.789504 web-pdb-1.6.0/web_pdb/static/
--rw-r--r--   0 runner    (1001) docker     (123)   160853 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/bundle.min.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.789504 web-pdb-1.6.0/web_pdb/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.789504 web-pdb-1.6.0/web_pdb/static/img/
--rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/img/debug.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     4052 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/img/debug.svg
--rw-r--r--   0 runner    (1001) docker     (123)   127453 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/static/styles.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.789504 web-pdb-1.6.0/web_pdb/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/web_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-26 16:03:02.000000 web-pdb-1.6.0/web_pdb/wsgi_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:03:11.789504 web-pdb-1.6.0/web_pdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-04-26 16:03:11.000000 web-pdb-1.6.0/web_pdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-26 16:03:11.000000 web-pdb-1.6.0/web_pdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:03:11.000000 web-pdb-1.6.0/web_pdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:03:11.000000 web-pdb-1.6.0/web_pdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 16:03:11.000000 web-pdb-1.6.0/web_pdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 16:03:11.000000 web-pdb-1.6.0/web_pdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.874395 web-pdb-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-06 19:52:19.000000 web-pdb-1.6.2/Changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-06 19:52:19.000000 web-pdb-1.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-06 19:52:19.000000 web-pdb-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-06 19:52:22.874395 web-pdb-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-07-06 19:52:19.000000 web-pdb-1.6.2/Readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-06 19:52:19.000000 web-pdb-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 19:52:22.878395 web-pdb-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-06 19:52:19.000000 web-pdb-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.870395 web-pdb-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 19:52:19.000000 web-pdb-1.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-06 19:52:19.000000 web-pdb-1.6.2/tests/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-06 19:52:19.000000 web-pdb-1.6.2/tests/db_i.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-06 19:52:19.000000 web-pdb-1.6.2/tests/db_pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 19:52:19.000000 web-pdb-1.6.2/tests/db_ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9191 2023-07-06 19:52:19.000000 web-pdb-1.6.2/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.870395 web-pdb-1.6.2/web_pdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.874395 web-pdb-1.6.2/web_pdb/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   160853 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/bundle.min.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.874395 web-pdb-1.6.2/web_pdb/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.874395 web-pdb-1.6.2/web_pdb/static/img/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/img/debug.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4052 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/img/debug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   127453 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/static/styles.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.874395 web-pdb-1.6.2/web_pdb/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/web_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-06 19:52:19.000000 web-pdb-1.6.2/web_pdb/wsgi_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:52:22.874395 web-pdb-1.6.2/web_pdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-06 19:52:22.000000 web-pdb-1.6.2/web_pdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-06 19:52:22.000000 web-pdb-1.6.2/web_pdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:52:22.000000 web-pdb-1.6.2/web_pdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:52:22.000000 web-pdb-1.6.2/web_pdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:52:22.000000 web-pdb-1.6.2/web_pdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 19:52:22.000000 web-pdb-1.6.2/web_pdb.egg-info/top_level.txt
```

### Comparing `web-pdb-1.6.0/Changelog.rst` & `web-pdb-1.6.2/Changelog.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 #########
 
+v.1.6.2
+=======
+* Rewrite tests with the latest Selenium version.
+* Bump asyncore-wsgi version in dependencies.
+
 v.1.6.0
 =======
 
 * Removed Python 2 support.
 * Moved to the modern Python package layout.
 
 v.1.5.7
```

### Comparing `web-pdb-1.6.0/LICENSE.txt` & `web-pdb-1.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/PKG-INFO` & `web-pdb-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-pdb
-Version: 1.6.0
+Version: 1.6.2
 Summary: Web interface for Python's built-in PDB debugger
 Home-page: https://github.com/romanvm/python-web-pdb
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
 License: MIT License
 Keywords: pdb remote web debugger'
 Platform: any
```

### Comparing `web-pdb-1.6.0/Readme.rst` & `web-pdb-1.6.2/Readme.rst`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/setup.cfg` & `web-pdb-1.6.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = web-pdb
-version = 1.6.0
+version = 1.6.2
 author = Roman Miroshnychenko
 author_email = roman1972@gmail.com
 url = https://github.com/romanvm/python-web-pdb
 description = Web interface for Python's built-in PDB debugger
 long_description = file: Readme.rst
 long_description_content_type = text/x-rst
 keywords = pdb remote web debugger'
@@ -25,16 +25,16 @@
 packages = 
 	web_pdb
 zip_safe = False
 include_package_data = True
 python_requires = >=3.6
 install_requires = 
 	bottle>=0.12.25
-	asyncore-wsgi>=0.0.4
+	asyncore-wsgi>=0.0.11
 test_suite = tests.tests
 tests_require = 
-	selenium==3.141.0
+	selenium==4.10.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `web-pdb-1.6.0/setup.py` & `web-pdb-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/tests/db_i.py` & `web-pdb-1.6.2/tests/db_i.py`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/tests/tests.py` & `web-pdb-1.6.2/tests/tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,42 +17,43 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-import os
 import sys
 import time
+from pathlib import Path
 from subprocess import Popen
 from unittest import TestCase, main, skipIf
 
 from selenium import webdriver
+from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 
-cwd = os.path.dirname(os.path.abspath(__file__))
-db_py = os.path.join(cwd, 'db.py')
+CWD = Path(__file__).resolve().parent
+DB_PY = CWD / 'db.py'
 
 
 class SeleniumTestCase(TestCase):
     @classmethod
     def setUpClass(cls):
         if sys.platform == 'win32':
             cls.browser = webdriver.Firefox()
         else:
             options = webdriver.ChromeOptions()
             options.add_argument('headless')
             options.add_argument('disable-gpu')
             cls.browser = webdriver.Chrome(options=options)
         cls.browser.implicitly_wait(10)
         cls.browser.get('http://127.0.0.1:5555')
-        cls.stdin = cls.browser.find_element_by_id('stdin')
-        cls.send_btn = cls.browser.find_element_by_id('send_btn')
-        cls.stdout_tag = cls.browser.find_element_by_id('stdout')
+        cls.stdin = cls.browser.find_element(By.ID, 'stdin')
+        cls.send_btn = cls.browser.find_element(By.ID, 'send_btn')
+        cls.stdout_tag = cls.browser.find_element(By.ID, 'stdout')
 
     @classmethod
     def tearDownClass(cls):
         cls.stdin.clear()
         cls.stdin.send_keys('q')
         cls.send_btn.click()
         time.sleep(1)
@@ -62,46 +63,46 @@
 
 class WebPdbTestCase(SeleniumTestCase):
     """
     This class provides basic functionality testing for Web-PDB
     """
     @classmethod
     def setUpClass(cls):
-        cls.db_proc = Popen(['python', db_py], shell=False)
+        cls.db_proc = Popen(['python', str(DB_PY)], shell=False)
         super(WebPdbTestCase, cls).setUpClass()
 
     def test_1_set_trace(self):
         """
         Test back-end/front-end interaction during debugging
         """
         time.sleep(1)
-        filename_tag = self.browser.find_element_by_id('filename')
+        filename_tag = self.browser.find_element(By.ID, 'filename')
         self.assertEqual(filename_tag.text, 'db.py')
-        curr_line_tag = self.browser.find_element_by_id('curr_line')
+        curr_line_tag = self.browser.find_element(By.ID, 'curr_line')
         self.assertEqual(curr_line_tag.text, '14')
-        curr_file_tag = self.browser.find_element_by_id('curr_file_code')
+        curr_file_tag = self.browser.find_element(By.ID, 'curr_file_code')
         self.assertIn('foo = \'foo\'', curr_file_tag.text)
-        globals_tag = self.browser.find_element_by_id('globals')
+        globals_tag = self.browser.find_element(By.ID, 'globals')
         self.assertIn('foo = \'foo\'', globals_tag.text)
         self.assertIn('-> bar = \'bar\'', self.stdout_tag.text)
         # Test if Prismjs syntax coloring actually works
         self.assertIn('foo <span class="token operator">=</span> <span class="token string">\'foo\'</span>',
                       self.browser.page_source)
 
     def test_2_next_command(self):
         """
         Test sending PDB commands
         """
         self.stdin.clear()
         self.stdin.send_keys('n')
         self.send_btn.click()
         time.sleep(1)
-        curr_line_tag = self.browser.find_element_by_id('curr_line')
+        curr_line_tag = self.browser.find_element(By.ID, 'curr_line')
         self.assertEqual(curr_line_tag.text, '15')
-        globals_tag = self.browser.find_element_by_id('globals')
+        globals_tag = self.browser.find_element(By.ID, 'globals')
         self.assertIn('bar = \'bar\'', globals_tag.text)
         self.assertIn('-> ham = \'spam\'', self.stdout_tag.text)
         self.assertEqual(self.stdin.get_attribute('value'), '')
 
     def test_3_history(self):
         """
         Test for the recent commands history
@@ -119,16 +120,16 @@
         """
         Test for highlighting breakpoints
         """
         self.stdin.clear()
         self.stdin.send_keys('b 20')
         self.send_btn.click()
         time.sleep(1)
-        line_numbers_rows = self.browser.find_element_by_css_selector('span.line-numbers-rows')
-        line_spans = line_numbers_rows.find_elements_by_tag_name('span')
+        line_numbers_rows = self.browser.find_element(By.CSS_SELECTOR, 'span.line-numbers-rows')
+        line_spans = line_numbers_rows.find_elements(By.TAG_NAME, 'span')
         self.assertEqual(line_spans[19].get_attribute('class'), 'breakpoint')
 
     def test_5_unicode_literal(self):
         """
         Test for displaying unicode literals
         """
         self.stdin.clear()
@@ -141,38 +142,38 @@
         """
         Test for entering unicode literal via console
         """
         self.stdin.clear()
         self.stdin.send_keys('p u\'python - питон\'')
         self.send_btn.click()
         time.sleep(1)
-        stdout_tag = self.browser.find_element_by_id('stdout')
+        stdout_tag = self.browser.find_element(By.ID, 'stdout')
         self.assertIn('u\'python - питон\'', stdout_tag.text)
 
     def test_7_local_vars(self):
         """
         Test for displaying local variables
         """
         self.stdin.clear()
         self.stdin.send_keys('c')
         self.send_btn.click()
         time.sleep(1)
-        locals_tag = self.browser.find_element_by_id('locals')
+        locals_tag = self.browser.find_element(By.ID, 'locals')
         self.assertIn('spam = \'spam\'', locals_tag.text)
-        globals_tag = self.browser.find_element_by_id('globals')
+        globals_tag = self.browser.find_element(By.ID, 'globals')
         self.assertNotEqual(globals_tag.text, locals_tag.text)
 
 
 class PatchStdStreamsTestCase(SeleniumTestCase):
     """
     This class tests patching sys.std* streams
     """
     @classmethod
     def setUpClass(cls):
-        cls.db_proc = Popen(['python', os.path.join(cwd, 'db_ps.py')], shell=False)
+        cls.db_proc = Popen(['python', str(CWD / 'db_ps.py')], shell=False)
         super(PatchStdStreamsTestCase, cls).setUpClass()
 
     def test_patching_std_streams(self):
         """
         Test if std streams are correctly redirected to the web-console
         """
         time.sleep(1)
@@ -194,37 +195,37 @@
         'This test fails on Python 3.10+ for some mysterious reason')
 class CatchPostMortemTestCase(SeleniumTestCase):
     """
     This class for catching exceptions
     """
     @classmethod
     def setUpClass(cls):
-        cls.db_proc = Popen(['python', os.path.join(cwd, 'db_pm.py')], shell=False)
+        cls.db_proc = Popen(['python', str(CWD / 'db_pm.py')], shell=False)
         super(CatchPostMortemTestCase, cls).setUpClass()
 
     def test_catch_post_mortem(self):
         """
         Test if catch_post_mortem context manager catches exceptions
         """
         time.sleep(1)
-        curr_line_tag = self.browser.find_element_by_id('curr_line')
+        curr_line_tag = self.browser.find_element(By.ID, 'curr_line')
         self.assertEqual(curr_line_tag.text, '14')
-        curr_file_tag = self.browser.find_element_by_id('curr_file_code')
+        curr_file_tag = self.browser.find_element(By.ID, 'curr_file_code')
         self.assertIn('assert False, \'Oops!\'', curr_file_tag.text)
-        stdout_tag = self.browser.find_element_by_id('stdout')
+        stdout_tag = self.browser.find_element(By.ID, 'stdout')
         self.assertIn('AssertionError', stdout_tag.text)
 
 
 class InspectCommandTestCase(SeleniumTestCase):
     """
     Test for inspect command
     """
     @classmethod
     def setUpClass(cls):
-        cls.db_proc = Popen(['python', os.path.join(cwd, 'db_i.py')], shell=False)
+        cls.db_proc = Popen(['python', str(CWD / 'db_i.py')], shell=False)
         super(InspectCommandTestCase, cls).setUpClass()
 
     def test_inspect_existing_object(self):
         """
         Test inspecting existing object
         """
         time.sleep(1)
```

### Comparing `web-pdb-1.6.0/web_pdb/__init__.py` & `web-pdb-1.6.2/web_pdb/__init__.py`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/bundle.min.js` & `web-pdb-1.6.2/web_pdb/static/bundle.min.js`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/bundle.min.js.LICENSE.txt` & `web-pdb-1.6.2/web_pdb/static/bundle.min.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.eot` & `web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.svg` & `web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.ttf` & `web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.woff` & `web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/fonts/glyphicons-halflings-regular.woff2` & `web-pdb-1.6.2/web_pdb/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/img/debug.png` & `web-pdb-1.6.2/web_pdb/static/img/debug.png`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/img/debug.svg` & `web-pdb-1.6.2/web_pdb/static/img/debug.svg`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/static/styles.min.css` & `web-pdb-1.6.2/web_pdb/static/styles.min.css`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/templates/index.html` & `web-pdb-1.6.2/web_pdb/templates/index.html`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/web_console.py` & `web-pdb-1.6.2/web_pdb/web_console.py`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb/wsgi_app.py` & `web-pdb-1.6.2/web_pdb/wsgi_app.py`

 * *Files identical despite different names*

### Comparing `web-pdb-1.6.0/web_pdb.egg-info/PKG-INFO` & `web-pdb-1.6.2/web_pdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-pdb
-Version: 1.6.0
+Version: 1.6.2
 Summary: Web interface for Python's built-in PDB debugger
 Home-page: https://github.com/romanvm/python-web-pdb
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
 License: MIT License
 Keywords: pdb remote web debugger'
 Platform: any
```

### Comparing `web-pdb-1.6.0/web_pdb.egg-info/SOURCES.txt` & `web-pdb-1.6.2/web_pdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

