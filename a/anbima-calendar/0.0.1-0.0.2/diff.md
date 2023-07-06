# Comparing `tmp/anbima_calendar-0.0.1.tar.gz` & `tmp/anbima_calendar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anbima_calendar-0.0.1.tar", last modified: Fri Nov 25 18:24:24 2022, max compression
+gzip compressed data, was "anbima_calendar-0.0.2.tar", last modified: Thu Jul  6 19:36:32 2023, max compression
```

## Comparing `anbima_calendar-0.0.1.tar` & `anbima_calendar-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-25 18:24:24.071781 anbima_calendar-0.0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11364 2022-11-25 17:20:07.000000 anbima_calendar-0.0.1/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      705 2022-11-25 18:24:24.071781 anbima_calendar-0.0.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-25 17:19:23.000000 anbima_calendar-0.0.1/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-25 18:24:24.071781 anbima_calendar-0.0.1/anbima_calendar/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      133 2022-11-25 18:19:47.000000 anbima_calendar-0.0.1/anbima_calendar/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1576 2022-11-25 18:19:48.000000 anbima_calendar-0.0.1/anbima_calendar/date.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3647 2022-11-25 18:22:17.000000 anbima_calendar-0.0.1/anbima_calendar/holidays.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2022-11-25 18:24:24.071781 anbima_calendar-0.0.1/anbima_calendar.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      705 2022-11-25 18:24:24.000000 anbima_calendar-0.0.1/anbima_calendar.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      277 2022-11-25 18:24:24.000000 anbima_calendar-0.0.1/anbima_calendar.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2022-11-25 18:24:24.000000 anbima_calendar-0.0.1/anbima_calendar.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       16 2022-11-25 18:24:24.000000 anbima_calendar-0.0.1/anbima_calendar.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      472 2022-11-25 17:26:50.000000 anbima_calendar-0.0.1/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2022-11-25 18:24:24.071781 anbima_calendar-0.0.1/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1023 2022-11-25 17:24:05.000000 anbima_calendar-0.0.1/setup.py
+drwxr-xr-x   0 rizidoro   (501) staff       (20)        0 2023-07-06 19:36:32.556055 anbima_calendar-0.0.2/
+-rw-r--r--   0 rizidoro   (501) staff       (20)    11364 2023-07-06 19:31:21.000000 anbima_calendar-0.0.2/LICENSE
+-rw-r--r--   0 rizidoro   (501) staff       (20)      677 2023-07-06 19:36:32.555891 anbima_calendar-0.0.2/PKG-INFO
+-rw-r--r--   0 rizidoro   (501) staff       (20)        0 2023-07-06 19:31:21.000000 anbima_calendar-0.0.2/README.md
+drwxr-xr-x   0 rizidoro   (501) staff       (20)        0 2023-07-06 19:36:32.554593 anbima_calendar-0.0.2/anbima_calendar/
+-rw-r--r--   0 rizidoro   (501) staff       (20)      133 2023-07-06 19:31:21.000000 anbima_calendar-0.0.2/anbima_calendar/__init__.py
+-rw-r--r--   0 rizidoro   (501) staff       (20)     1576 2023-07-06 19:31:21.000000 anbima_calendar-0.0.2/anbima_calendar/date.py
+-rw-r--r--   0 rizidoro   (501) staff       (20)     4248 2023-07-06 19:35:28.000000 anbima_calendar-0.0.2/anbima_calendar/holidays.py
+drwxr-xr-x   0 rizidoro   (501) staff       (20)        0 2023-07-06 19:36:32.555363 anbima_calendar-0.0.2/anbima_calendar.egg-info/
+-rw-r--r--   0 rizidoro   (501) staff       (20)      677 2023-07-06 19:36:32.000000 anbima_calendar-0.0.2/anbima_calendar.egg-info/PKG-INFO
+-rw-r--r--   0 rizidoro   (501) staff       (20)      296 2023-07-06 19:36:32.000000 anbima_calendar-0.0.2/anbima_calendar.egg-info/SOURCES.txt
+-rw-r--r--   0 rizidoro   (501) staff       (20)        1 2023-07-06 19:36:32.000000 anbima_calendar-0.0.2/anbima_calendar.egg-info/dependency_links.txt
+-rw-r--r--   0 rizidoro   (501) staff       (20)       16 2023-07-06 19:36:32.000000 anbima_calendar-0.0.2/anbima_calendar.egg-info/top_level.txt
+-rw-r--r--   0 rizidoro   (501) staff       (20)      472 2023-07-06 19:35:41.000000 anbima_calendar-0.0.2/pyproject.toml
+-rw-r--r--   0 rizidoro   (501) staff       (20)       38 2023-07-06 19:36:32.556100 anbima_calendar-0.0.2/setup.cfg
+-rw-r--r--   0 rizidoro   (501) staff       (20)     1023 2023-07-06 19:35:38.000000 anbima_calendar-0.0.2/setup.py
+drwxr-xr-x   0 rizidoro   (501) staff       (20)        0 2023-07-06 19:36:32.555560 anbima_calendar-0.0.2/tests/
+-rw-r--r--   0 rizidoro   (501) staff       (20)     1633 2023-07-06 19:31:21.000000 anbima_calendar-0.0.2/tests/test_date.py
```

### Comparing `anbima_calendar-0.0.1/LICENSE` & `anbima_calendar-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anbima_calendar-0.0.1/PKG-INFO` & `anbima_calendar-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: anbima_calendar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ambima Calendar - Helper functions to handle banking holidays in Brazil
 Home-page: https://github.com/risparfinance/anbima_calendar
 Author: Rispar
 Author-email: tecnologia@rispar.com.br
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `anbima_calendar-0.0.1/anbima_calendar/date.py` & `anbima_calendar-0.0.2/anbima_calendar/date.py`

 * *Files identical despite different names*

### Comparing `anbima_calendar-0.0.1/anbima_calendar/holidays.py` & `anbima_calendar-0.0.2/anbima_calendar/holidays.py`

 * *Files 12% similar despite different names*

```diff
@@ -81,8 +81,22 @@
         "Corpus Christi": date(2025, 6, 19),
         "Independência do Brasil": date(2025, 9, 7),
         "Nossa Sr.a Aparecida - Padroeira do Brasil": date(2025, 10, 12),
         "Finados": date(2025, 11, 2),
         "Proclamação da República": date(2025, 11, 15),
         "Natal": date(2025, 12, 25),
     },
+    "2026": {
+        "Confraternização Universal": date(2026, 1, 1),
+        "Carnaval 1": date(2026, 2, 16),
+        "Carnaval 2": date(2026, 2, 17),
+        "Paixão de Cristo": date(2026, 4, 3),
+        "Tiradentes": date(2026, 4, 21),
+        "Dia do Trabalho": date(2026, 5, 1),
+        "Corpus Christi": date(2026, 6, 19),
+        "Independência do Brasil": date(2026, 9, 7),
+        "Nossa Sr.a Aparecida - Padroeira do Brasil": date(2026, 10, 12),
+        "Finados": date(2026, 11, 2),
+        "Proclamação da República": date(2026, 11, 15),
+        "Natal": date(2026, 12, 25),
+    },
 }
```

### Comparing `anbima_calendar-0.0.1/anbima_calendar.egg-info/PKG-INFO` & `anbima_calendar-0.0.2/anbima_calendar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: anbima-calendar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ambima Calendar - Helper functions to handle banking holidays in Brazil
 Home-page: https://github.com/risparfinance/anbima_calendar
 Author: Rispar
 Author-email: tecnologia@rispar.com.br
 License: Apache License 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `anbima_calendar-0.0.1/setup.py` & `anbima_calendar-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 setuptools.setup(
     author="Rispar",
     author_email="tecnologia@rispar.com.br",
     url="https://github.com/risparfinance/anbima_calendar",
     name="anbima_calendar",
-    version="0.0.1",
+    version="0.0.2",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     package_data={"anbima_calendar": ["LICENSE"]},
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="Ambima Calendar - Helper functions to handle banking holidays in Brazil",
     license="Apache License 2.0",
```

