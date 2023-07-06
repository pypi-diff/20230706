# Comparing `tmp/pymorningstar-0.20.tar.gz` & `tmp/pymorningstar-0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymorningstar-0.20.tar", last modified: Wed Sep 21 10:44:39 2022, max compression
+gzip compressed data, was "pymorningstar-0.21.tar", last modified: Thu Jul  6 16:04:22 2023, max compression
```

## Comparing `pymorningstar-0.20.tar` & `pymorningstar-0.21.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-21 10:44:39.172010 pymorningstar-0.20/
--rw-rw-rw-   0        0        0       41 2022-09-08 19:02:29.000000 pymorningstar-0.20/MANIFEST.in
--rw-rw-rw-   0        0        0      489 2022-09-21 10:44:39.171014 pymorningstar-0.20/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-09-21 10:44:39.159028 pymorningstar-0.20/pymorningstar/
--rw-rw-rw-   0        0        0        0 2022-08-13 19:43:51.000000 pymorningstar-0.20/pymorningstar/README.md
--rw-rw-rw-   0        0        0        0 2022-09-08 17:48:16.000000 pymorningstar-0.20/pymorningstar/__init__.py
--rw-rw-rw-   0        0        0     7642 2022-09-21 10:34:04.000000 pymorningstar-0.20/pymorningstar/excel.py
--rw-rw-rw-   0        0        0     5244 2021-11-22 08:29:25.000000 pymorningstar-0.20/pymorningstar/morning_limit.png
-drwxrwxrwx   0        0        0        0 2022-09-21 10:44:39.170012 pymorningstar-0.20/pymorningstar.egg-info/
--rw-rw-rw-   0        0        0      489 2022-09-21 10:44:39.000000 pymorningstar-0.20/pymorningstar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2022-09-21 10:44:39.000000 pymorningstar-0.20/pymorningstar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-21 10:44:39.000000 pymorningstar-0.20/pymorningstar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-19 20:07:58.000000 pymorningstar-0.20/pymorningstar.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2022-09-21 10:44:39.000000 pymorningstar-0.20/pymorningstar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-09-21 10:44:39.000000 pymorningstar-0.20/pymorningstar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-21 10:44:39.172010 pymorningstar-0.20/setup.cfg
--rw-rw-rw-   0        0        0      707 2022-09-21 10:44:12.000000 pymorningstar-0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 16:04:22.070987 pymorningstar-0.21/
+-rw-rw-rw-   0        0        0       41 2022-09-08 19:02:29.000000 pymorningstar-0.21/MANIFEST.in
+-rw-rw-rw-   0        0        0      431 2023-07-06 16:04:22.069985 pymorningstar-0.21/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 16:04:22.060664 pymorningstar-0.21/pymorningstar/
+-rw-rw-rw-   0        0        0        0 2022-09-08 17:48:16.000000 pymorningstar-0.21/pymorningstar/__init__.py
+-rw-rw-rw-   0        0        0     7636 2023-07-06 15:55:22.000000 pymorningstar-0.21/pymorningstar/excel.py
+-rw-rw-rw-   0        0        0     5244 2021-11-22 08:29:25.000000 pymorningstar-0.21/pymorningstar/morning_limit.png
+drwxrwxrwx   0        0        0        0 2023-07-06 16:04:22.068987 pymorningstar-0.21/pymorningstar.egg-info/
+-rw-rw-rw-   0        0        0      431 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-19 20:07:58.000000 pymorningstar-0.21/pymorningstar.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-06 16:04:21.000000 pymorningstar-0.21/pymorningstar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2023-07-06 15:57:32.000000 pymorningstar-0.21/readme.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 16:04:22.071074 pymorningstar-0.21/setup.cfg
+-rw-rw-rw-   0        0        0      683 2023-07-06 16:03:37.000000 pymorningstar-0.21/setup.py
```

### Comparing `pymorningstar-0.20/pymorningstar/excel.py` & `pymorningstar-0.21/pymorningstar/excel.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     
     def initialize_morning(self):
         self.wb = xw.Book()
         time.sleep(0.5)
         self.wb.app.api.WindowState = xw.constants.WindowState.xlMaximized
         self.wb.app.activate(steal_focus=True)
         time.sleep(5)
-        self.sheet = self.wb.sheets['Hoja1']
+        self.sheet = self.wb.sheets[0]
          
              
     def get_holding (self, isin_fund, inception_date, obsolete_date, asset_id, holding_type='ALL',data_type = 'WEIGHT', 
                      frequency = 'A', show_holding_type = True, show_country=False, 
                      show_currency=False, show_maturity=False, show_coupon=False, wait_time=0, months_frac=12):
                         # asset_id = SecID / Ticker / ISIN /CUSIP
                         # holding_type = STOCKS / BONDS / FUNDS / ETFS / ALL
```

### Comparing `pymorningstar-0.20/pymorningstar/morning_limit.png` & `pymorningstar-0.21/pymorningstar/morning_limit.png`

 * *Files identical despite different names*

### Comparing `pymorningstar-0.20/setup.py` & `pymorningstar-0.21/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from setuptools import setup
 
 setup(
     name='pymorningstar', 
-    version='0.20', 
+    version='0.21',
     description = "Automating the download of information from Morningstar's Excel Add-In API",
     author = 'Pablo Vilas',
     author_email='pablo.vilas.naval@gmail.com',
     packages = ['pymorningstar'],
     install_requires=['xlwings','pandas','pyautogui', 'opencv-python', 'Pillow'],
-    url='https://https://github.com/VilasPablo/pymorningstar',
+    url='https://github.com/VilasPablo/pymorningstar',
     classifiers=[ 
         'Intended Audience :: Science/Research',
         'Intended Audience :: Financial and Insurance Industry',
         'Programming Language :: Python :: 3',  ],
     include_package_data=True,
     zip_safe = False)
 
-
-# MANIFEST.in
```

