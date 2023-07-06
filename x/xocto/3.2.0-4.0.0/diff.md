# Comparing `tmp/xocto-3.2.0.tar.gz` & `tmp/xocto-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xocto-3.2.0.tar", last modified: Wed Jun  7 08:36:17 2023, max compression
+gzip compressed data, was "xocto-4.0.0.tar", last modified: Thu Jul  6 08:59:46 2023, max compression
```

## Comparing `xocto-3.2.0.tar` & `xocto-4.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-07 08:36:06.000000 xocto-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 08:36:17.789391 xocto-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 08:36:06.000000 xocto-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-07 08:36:06.000000 xocto-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 08:36:17.789391 xocto-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-07 08:36:06.000000 xocto-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_health.py
--rw-r--r--   0 runner    (1001) docker     (123)    43618 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_localtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20696 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-06-07 08:36:06.000000 xocto-3.2.0/tests/test_settlement_periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto/events/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/events/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/events/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/health.py
--rw-r--r--   0 runner    (1001) docker     (123)    24848 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/localtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/pact_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29680 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/settlement_periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/s3_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    60238 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 08:36:06.000000 xocto-3.2.0/xocto/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:36:17.789391 xocto-3.2.0/xocto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 08:36:17.000000 xocto-3.2.0/xocto.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:46.833797 xocto-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-06 08:59:36.000000 xocto-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-06 08:59:46.833797 xocto-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 08:59:36.000000 xocto-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-06 08:59:36.000000 xocto-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-06 08:59:46.833797 xocto-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-06 08:59:36.000000 xocto-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:46.829797 xocto-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-06 08:59:36.000000 xocto-4.0.0/tests/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42927 2023-07-06 08:59:36.000000 xocto-4.0.0/tests/test_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-06 08:59:36.000000 xocto-4.0.0/tests/test_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20696 2023-07-06 08:59:36.000000 xocto-4.0.0/tests/test_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12312 2023-07-06 08:59:36.000000 xocto-4.0.0/tests/test_settlement_periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:46.833797 xocto-4.0.0/xocto/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:46.833797 xocto-4.0.0/xocto/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/events/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/events/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23954 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/pact_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29680 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/settlement_periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:46.833797 xocto-4.0.0/xocto/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/storage/s3_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60238 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-06 08:59:36.000000 xocto-4.0.0/xocto/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:59:46.833797 xocto-4.0.0/xocto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-06 08:59:46.000000 xocto-4.0.0/xocto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-06 08:59:46.000000 xocto-4.0.0/xocto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:59:46.000000 xocto-4.0.0/xocto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:59:46.000000 xocto-4.0.0/xocto.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-06 08:59:46.000000 xocto-4.0.0/xocto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 08:59:46.000000 xocto-4.0.0/xocto.egg-info/top_level.txt
```

### Comparing `xocto-3.2.0/LICENSE` & `xocto-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/PKG-INFO` & `xocto-4.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xocto
-Version: 3.2.0
+Version: 4.0.0
 Summary: Kraken Technologies Python service utilities
 Home-page: https://github.com/octoenergy/xocto
 Author: Kraken Technologies
 Author-email: talent@octopus.energy
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xocto-3.2.0/pyproject.toml` & `xocto-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -67,9 +67,10 @@
   "botocore.*",
   "django.*",
   "moto.*",
   "pact.*",
   "pandas.*",
   "setuptools.*",
   "xlrd.*",
+  "zoneinfo.*",
 ]
 ignore_missing_imports = true
```

### Comparing `xocto-3.2.0/setup.py` & `xocto-4.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from codecs import open
 from os import path
 
 from setuptools import setup
 
 REPO_ROOT = path.abspath(path.dirname(__file__))
 
-VERSION = "3.2.0"
+VERSION = "4.0.0"
 
 with open(path.join(REPO_ROOT, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xocto",
     version=VERSION,
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
     ],
     packages=["xocto", "xocto.events", "xocto.storage"],
     package_data={"xocto": ["py.typed"]},
     zip_safe=False,
     install_requires=[
         "ddtrace>=1.9.0",
-        "django>=3.2,<5.0",
+        "django>=4.0",
         "openpyxl>=3.1.0",
         "pact-python>=1.6.0",
         "pandas>=1.5.3",
         "pyarrow>=11.0.0",
         "python-dateutil>=2.8.2",
         "python-magic>=0.4.27",
         "pytz",
```

### Comparing `xocto-3.2.0/tests/test_localtime.py` & `xocto-4.0.0/tests/test_localtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 import datetime
 import decimal
+import zoneinfo
 
 import pytest
-import pytz
 import time_machine
 from dateutil import relativedelta
 from django.conf import settings
 from django.test import override_settings
 from django.utils import timezone
 
 from tests import factories
 from xocto import localtime
 
 
 class TestNow:
     def test_now_is_in_correct_timezone(self):
         now = localtime.now()
-        assert now.tzinfo.zone == settings.TIME_ZONE
+        assert str(now.tzinfo) == settings.TIME_ZONE
 
+
+class TestSecondsInTheFuture:
     def test_seconds_in_future(self):
         with time_machine.travel("2020-01-01 12:00:00.000", tick=False):
             assert localtime.seconds_in_the_future(1) == localtime.as_localtime(
                 localtime.datetime_.datetime(2020, 1, 1, 12, 0, 1, tzinfo=localtime.UTC)
             )
             assert localtime.seconds_in_the_future(1.5) == localtime.as_localtime(
                 localtime.datetime_.datetime(2020, 1, 1, 12, 0, 1, 500000, tzinfo=localtime.UTC)
             )
 
+
+class TestSecondsInThePast:
     def test_seconds_in_past(self):
         with time_machine.travel("2020-01-01 12:00:00.000", tick=False):
             assert localtime.seconds_in_the_past(1) == localtime.as_localtime(
                 localtime.datetime_.datetime(2020, 1, 1, 11, 59, 59, tzinfo=localtime.UTC)
             )
             assert localtime.seconds_in_the_past(1.5) == localtime.as_localtime(
                 localtime.datetime_.datetime(2020, 1, 1, 11, 59, 58, 500000, tzinfo=localtime.UTC)
             )
 
 
 class TestDate:
     def test_date_calculation_near_midnight_during_bst(self):
-        near_midnight_in_utc = datetime.datetime(2016, 6, 1, 23, 50, 0, tzinfo=pytz.utc)
+        near_midnight_in_utc = datetime.datetime(2016, 6, 1, 23, 50, 0, tzinfo=localtime.UTC)
         assert localtime.date(near_midnight_in_utc) == (
             near_midnight_in_utc.date() + datetime.timedelta(days=1)
         )
 
     def test_date_calculation_near_midnight_outside_of_bst(self):
-        near_midnight_in_utc = datetime.datetime(2016, 11, 1, 23, 50, 0, tzinfo=pytz.utc)
+        near_midnight_in_utc = datetime.datetime(2016, 11, 1, 23, 50, 0, tzinfo=localtime.UTC)
         assert localtime.date(near_midnight_in_utc) == near_midnight_in_utc.date()
 
-    @pytest.mark.parametrize("tz", (pytz.timezone("Etc/GMT-10"), pytz.utc))
+    @pytest.mark.parametrize("tz", (zoneinfo.ZoneInfo("Etc/GMT-10"), localtime.UTC))
     def test_date_calculation_specifying_other_timezone(self, tz):
         near_midnight = datetime.datetime(2016, 6, 1, 23, 50, 0, tzinfo=tz)
         assert localtime.date(near_midnight, tz=tz) == (near_midnight.date())
 
     def test_datetime_not_supplied(self):
         """
         Check that we do not fallback to today if a datetime is not passed to the function -
@@ -84,15 +88,15 @@
 class TestMidnight:
     def test_midnight_calculation_for_bst_date(self):
         date = datetime.date(2016, 7, 2)
         midnight = localtime.midnight(date)
         assert midnight.tzinfo is not None
         assert midnight.hour == 0
 
-        midnight_utc = midnight.astimezone(pytz.utc)
+        midnight_utc = midnight.astimezone(localtime.UTC)
         assert midnight_utc.hour == 23
 
     def test_midnight_calculation_for_utc_dt(self):
         dt = factories.utc.dt("2017-12-20T16:00")
 
         assert localtime.midnight(dt) == localtime.datetime(2017, 12, 20, 0, 0)
 
@@ -101,19 +105,19 @@
         assert midnight.date() == localtime.today()
         assert midnight.tzinfo is not None
         assert midnight.hour == 0
 
     def test_convert_date_to_midnight_and_back(self):
         date = datetime.date(2016, 7, 2)
         midnight = localtime.midnight(date)
-        midnight_utc = midnight.astimezone(pytz.utc)
+        midnight_utc = midnight.astimezone(localtime.UTC)
         assert localtime.date(midnight_utc) == date
 
     def test_midnight_in_different_timezone(self):
-        aus_time = pytz.timezone("Etc/GMT-10")
+        aus_time = zoneinfo.ZoneInfo("Etc/GMT-10")
 
         with time_machine.travel(datetime.datetime(2020, 2, 2, 1, tzinfo=aus_time), tick=False):
             result = localtime.midnight(tz=aus_time)
 
         assert result == datetime.datetime(2020, 2, 2, 0, 0, tzinfo=aus_time)
 
     def test_doesnt_change_date_of_already_midnight_datetime(self):
@@ -153,15 +157,15 @@
         """
         # attach the current Sydney timezone to the expected midnight
         expected_midnight = timezone.make_aware(expected_midnight)
 
         actual_midnight = localtime.midnight(naive_datetime)
 
         assert actual_midnight == expected_midnight
-        assert actual_midnight.tzinfo.zone == "Australia/Sydney"
+        assert str(actual_midnight.tzinfo) == "Australia/Sydney"
 
     @override_settings(TIME_ZONE="Australia/Sydney")  # set the django default/current timezone
     @pytest.mark.parametrize(
         "naive_datetime,specified_timezone,expected_midnight",
         [
             (
                 # this is assumed to be in the current django timezone (Sydney)
@@ -220,22 +224,22 @@
         this is the behaviour when tz argument is specified:
         1. the naive datetime is assumed to be in the current Django timezone
             (NOT the passed timezone)
         2. convert that moment in time to the specified timezone
         3. get the date of that datetime
         3. return midnight at the start of that date, in the specified timezone.
         """
-        specified_timezone_obj = pytz.timezone(specified_timezone)
+        specified_timezone_obj = zoneinfo.ZoneInfo(specified_timezone)
         # attach the specified timezone to the expected midnight
         expected_midnight = timezone.make_aware(expected_midnight, timezone=specified_timezone_obj)
 
         actual_midnight = localtime.midnight(naive_datetime, tz=specified_timezone_obj)
 
         assert actual_midnight == expected_midnight
-        assert actual_midnight.tzinfo.zone == specified_timezone
+        assert str(actual_midnight.tzinfo) == specified_timezone
 
 
 class TestMidday:
     def test_midday_calculation(self):
         date = datetime.date(2016, 7, 2)
         midday = localtime.midday(date)
         assert midday.tzinfo is not None
@@ -246,15 +250,15 @@
         midday = localtime.midday()
         assert midday.date() == localtime.today()
         assert midday.tzinfo is not None
         assert midday.hour == 12
         assert midday.minute == 0
 
     def test_midday_in_different_timezone(self):
-        aus_time = pytz.timezone("Etc/GMT-10")
+        aus_time = zoneinfo.ZoneInfo("Etc/GMT-10")
 
         with time_machine.travel(datetime.datetime(2020, 2, 2, 1, tzinfo=aus_time), tick=False):
             result = localtime.midday(tz=aus_time)
 
         assert result == datetime.datetime(2020, 2, 2, 12, 0, tzinfo=aus_time)
 
 
@@ -278,50 +282,40 @@
         assert latest.microsecond == 999999
 
 
 class TestDateTime:
     def test_datetime_creation(self):
         dt = localtime.datetime(2016, 8, 5)
         assert dt.hour == 0
-        utc_dt = dt.astimezone(pytz.utc)
+        utc_dt = dt.astimezone(localtime.UTC)
         assert utc_dt.hour == 23
 
-    # 2020-10-25T01:30 is an ambiguous dt as its in the period when clocks go back (so it
-    # occurs twice).
-
     def test_dst_ambiguity(self):
-        with pytest.raises(pytz.AmbiguousTimeError):
-            localtime.datetime(2020, 10, 25, 1, 30)
-
-    def test_passing_dst_value_resolves_ambiguity(self):
-        dt_dst = localtime.datetime(2020, 10, 25, 1, 30, is_dst=True)
-        assert dt_dst.hour == 1
-        assert dt_dst.minute == 30
-        assert dt_dst.dst()
-
-        dt_gmt = localtime.datetime(2020, 10, 25, 1, 30, is_dst=False)
-        assert dt_gmt.hour == 1
-        assert dt_gmt.minute == 30
-        assert not dt_gmt.dst()
-
-        assert dt_dst < dt_gmt
+        # 2020-10-25T01:30 is an ambiguous dt in Europe/London as its in the period when clocks go
+        # back (so it occurs twice).
+        dt = localtime.datetime(2020, 10, 25, 1, 30)
+        assert dt.hour == 1
+        assert dt.minute == 30
+        assert dt.dst() == datetime.timedelta(seconds=3600)
+        utc_dt = dt.astimezone(localtime.UTC)
+        assert utc_dt.hour == 0
 
 
 class TestAsLocaltime:
     def test_conversion_of_gmt_dt(self):
-        non_dst_datetime = datetime.datetime(2016, 1, 1, 23, 1, tzinfo=pytz.UTC)
+        non_dst_datetime = datetime.datetime(2016, 1, 1, 23, 1, tzinfo=localtime.UTC)
         converted_non_dst_datetime = localtime.as_localtime(non_dst_datetime)
 
         # The two dates are 'equal' and their day and hour attributes differ
         assert converted_non_dst_datetime == non_dst_datetime
         assert converted_non_dst_datetime.day == non_dst_datetime.day
         assert converted_non_dst_datetime.hour == non_dst_datetime.hour
 
     def test_conversion_of_bst_dt(self):
-        dst_datetime = datetime.datetime(2016, 5, 1, 23, 1, tzinfo=pytz.UTC)
+        dst_datetime = datetime.datetime(2016, 5, 1, 23, 1, tzinfo=localtime.UTC)
         converted_dst_datetime = localtime.as_localtime(dst_datetime)
 
         # The two dates are 'equal' but their day and hour attributes differ
         assert converted_dst_datetime == dst_datetime
         assert converted_dst_datetime.day == dst_datetime.day + 1
         assert converted_dst_datetime.hour == dst_datetime.hour - 23
 
@@ -330,169 +324,145 @@
         assert str(utc_dt.tzinfo) == "UTC"
 
         local_dt = localtime.as_localtime(utc_dt)
         assert str(local_dt.tzinfo) == "Europe/London"
 
 
 class TestIsUTC:
-    def test_is_utc(self):
-        # <UTC>
-        assert localtime.is_utc(timezone.now())
-
-    def test_is_utc_non_pytz_time_zone(self):
-        # datetime.timezone.utc
-        now = datetime.datetime.fromisoformat(timezone.now().isoformat())
+    @pytest.mark.parametrize("tzinfo", [datetime.timezone.utc, localtime.UTC])
+    def test_is_utc(self, tzinfo):
+        now = datetime.datetime(2020, 1, 1, tzinfo=tzinfo)
         assert localtime.is_utc(now)
 
     def test_is_not_utc(self):
-        # <DstTzInfo 'Europe/London' GMT0:00:00 STD>
-        assert not localtime.is_utc(localtime.now())
+        now = datetime.datetime(2020, 1, 1, tzinfo=localtime.LONDON)
+        assert not localtime.is_utc(now)
 
 
 class TestIsLocalime:
     def test_is_local_time(self):
-        dt = localtime.datetime(2016, 8, 5)
-        utc_dt = dt.astimezone(pytz.utc)
-        assert not localtime.is_local_time(utc_dt)
         assert localtime.is_local_time(localtime.now())
-        # Now for a tricky one: create a local datetime, and check that it passes `is_local_time`
-        local_dt = localtime.datetime(2016, 6, 2, 5, 1)
-        assert localtime.is_local_time(local_dt)
-        # Now take it back six months into a different timezone. It will fail:
-        local_dt -= datetime.timedelta(days=180)
-        assert not localtime.is_local_time(local_dt)
-        # Now `normalize` it, and it will pass again
-        local_dt = timezone.get_current_timezone().normalize(local_dt)
-        assert localtime.is_local_time(local_dt)
 
-    def test_datetime_utc(self):
+    def test_is_not_local_time(self):
         dt = datetime.datetime(2016, 8, 5, tzinfo=datetime.timezone.utc)
-        # Should not raise:
-        #     AttributeError: 'datetime.timezone' object has no attribute '_utcoffset'
         assert not localtime.is_local_time(dt)
 
 
-# Alias to make the pytest parameters fit on one line
-ldt = localtime.datetime
-
-
 class TestQuantise:
     @pytest.mark.parametrize(
         ("dt", "timedelta", "rounding_strategy", "result"),
         [
             (
-                ldt(2016, 12, 5, 11, 34, 59),
+                localtime.datetime(2016, 12, 5, 11, 34, 59),
                 datetime.timedelta(minutes=30),
                 None,
-                ldt(2016, 12, 5, 11, 30, 0),
+                localtime.datetime(2016, 12, 5, 11, 30, 0),
             ),
             (
-                ldt(2016, 12, 5, 11, 29, 59),
+                localtime.datetime(2016, 12, 5, 11, 29, 59),
                 datetime.timedelta(minutes=30),
                 None,
-                ldt(2016, 12, 5, 11, 30, 0),
+                localtime.datetime(2016, 12, 5, 11, 30, 0),
             ),
             (
-                ldt(2016, 12, 5, 11, 14, 59),
+                localtime.datetime(2016, 12, 5, 11, 14, 59),
                 datetime.timedelta(minutes=30),
                 None,
-                ldt(2016, 12, 5, 11, 0, 0),
+                localtime.datetime(2016, 12, 5, 11, 0, 0),
             ),
             (
-                ldt(2016, 12, 5, 11, 15, 59),
+                localtime.datetime(2016, 12, 5, 11, 15, 59),
                 datetime.timedelta(minutes=30),
                 None,
-                ldt(2016, 12, 5, 11, 30, 0),
+                localtime.datetime(2016, 12, 5, 11, 30, 0),
             ),
             (
-                ldt(2016, 12, 5, 11, 16, 0),
+                localtime.datetime(2016, 12, 5, 11, 16, 0),
                 datetime.timedelta(minutes=30),
                 None,
-                ldt(2016, 12, 5, 11, 30, 0),
+                localtime.datetime(2016, 12, 5, 11, 30, 0),
             ),
             (
-                ldt(2016, 12, 5, 10, 59, 59),
+                localtime.datetime(2016, 12, 5, 10, 59, 59),
                 datetime.timedelta(hours=2),
                 None,
-                ldt(2016, 12, 5, 10, 0, 0),
+                localtime.datetime(2016, 12, 5, 10, 0, 0),
             ),
             (
-                ldt(2016, 12, 5, 11, 0, 0),
+                localtime.datetime(2016, 12, 5, 11, 0, 0),
                 datetime.timedelta(hours=2),
                 None,
-                ldt(2016, 12, 5, 12, 0, 0),
+                localtime.datetime(2016, 12, 5, 12, 0, 0),
             ),
             (
-                ldt(2016, 12, 31, 13, 34, 59),
+                localtime.datetime(2016, 12, 31, 13, 34, 59),
                 datetime.timedelta(hours=24),
                 None,
-                ldt(2017, 1, 1, 0, 0, 0),
+                localtime.datetime(2017, 1, 1, 0, 0, 0),
             ),
             (
-                ldt(2016, 12, 31, 0, 0, 1),
+                localtime.datetime(2016, 12, 31, 0, 0, 1),
                 datetime.timedelta(days=1),
                 None,
-                ldt(2016, 12, 31, 0, 0, 0),
+                localtime.datetime(2016, 12, 31, 0, 0, 0),
             ),
             # CUSTOM ROUNDING STRATEGIES
             (
-                ldt(2016, 2, 2, 12, 30, 1),
+                localtime.datetime(2016, 2, 2, 12, 30, 1),
                 datetime.timedelta(minutes=30),
                 decimal.ROUND_UP,
-                ldt(2016, 2, 2, 13, 0, 0),
+                localtime.datetime(2016, 2, 2, 13, 0, 0),
             ),
             (
-                ldt(2016, 2, 2, 12, 45, 0),
+                localtime.datetime(2016, 2, 2, 12, 45, 0),
                 datetime.timedelta(minutes=30),
                 decimal.ROUND_HALF_UP,
-                ldt(2016, 2, 2, 13, 0, 0),
+                localtime.datetime(2016, 2, 2, 13, 0, 0),
             ),
             (
-                ldt(2016, 2, 2, 12, 45, 0),
+                localtime.datetime(2016, 2, 2, 12, 45, 0),
                 datetime.timedelta(minutes=30),
                 decimal.ROUND_HALF_DOWN,
-                ldt(2016, 2, 2, 12, 30, 0),
+                localtime.datetime(2016, 2, 2, 12, 30, 0),
             ),
             (
-                ldt(2016, 2, 2, 12, 0, 0),
+                localtime.datetime(2016, 2, 2, 12, 0, 0),
                 datetime.timedelta(days=1),
                 decimal.ROUND_HALF_DOWN,
-                ldt(2016, 2, 2, 0, 0, 0),
+                localtime.datetime(2016, 2, 2, 0, 0, 0),
             ),
             (
-                ldt(2016, 2, 2, 22, 0),
+                localtime.datetime(2016, 2, 2, 22, 0),
                 datetime.timedelta(days=1),
                 decimal.ROUND_HALF_UP,
-                ldt(2016, 2, 3, 0, 0, 0),
+                localtime.datetime(2016, 2, 3, 0, 0, 0),
             ),
             # Test doesn't round beyond limits
             (
-                ldt(2016, 2, 2, 12, 30, 0),
+                localtime.datetime(2016, 2, 2, 12, 30, 0),
                 datetime.timedelta(minutes=30),
                 decimal.ROUND_UP,
-                ldt(2016, 2, 2, 12, 30, 0),
+                localtime.datetime(2016, 2, 2, 12, 30, 0),
             ),
             (
-                ldt(2016, 2, 2, 12, 30, 0),
+                localtime.datetime(2016, 2, 2, 12, 30, 0),
                 datetime.timedelta(minutes=30),
                 decimal.ROUND_DOWN,
-                ldt(2016, 2, 2, 12, 30, 0),
+                localtime.datetime(2016, 2, 2, 12, 30, 0),
             ),
         ],
     )
     def test_quantise(self, dt, timedelta, rounding_strategy, result):
         args = (dt, timedelta)
         kwargs = dict(rounding=rounding_strategy) if rounding_strategy else {}
         assert localtime.quantise(*args, **kwargs) == result
 
 
 class TestDateBoundaries:
-    def test_date_boundaries_for_gmt_date(
-        self,
-    ):
+    def test_date_boundaries_for_gmt_date(self):
         date = datetime.date(2017, 1, 1)
 
         start, end = localtime.date_boundaries(date)
 
         assert localtime.is_local_time(start)
         assert localtime.is_local_time(end)
         assert (end - start) == datetime.timedelta(days=1)
@@ -513,26 +483,28 @@
     def test_date_boundaries_for_spring_dst_boundary(self):
         date = datetime.date(2017, 3, 26)
 
         start, end = localtime.date_boundaries(date)
 
         assert localtime.is_local_time(start)
         assert localtime.is_local_time(end)
-        assert (end - start) == datetime.timedelta(seconds=23 * 60 * 60)
+        delta = datetime.timedelta(seconds=(end.timestamp() - start.timestamp()))
+        assert delta == datetime.timedelta(seconds=23 * 60 * 60)
         assert localtime.datetime(2017, 3, 26) == start
         assert localtime.datetime(2017, 3, 27) == end
 
     def test_date_boundaries_for_autumn_dst_boundary(self):
         date = datetime.date(2017, 10, 29)
 
         start, end = localtime.date_boundaries(date)
 
         assert localtime.is_local_time(start)
         assert localtime.is_local_time(end)
-        assert (end - start) == datetime.timedelta(days=1, seconds=60 * 60)
+        delta = datetime.timedelta(seconds=(end.timestamp() - start.timestamp()))
+        assert delta == datetime.timedelta(seconds=25 * 60 * 60)
         assert localtime.datetime(2017, 10, 29) == start
         assert localtime.datetime(2017, 10, 30) == end
 
 
 class TestMonthBoundaries:
     def test_march_2021(self):
         assert localtime.month_boundaries(month=3, year=2021) == (
@@ -541,28 +513,31 @@
         )
 
 
 class TestStartOfMonth:
     @pytest.mark.parametrize(
         ("dt", "result"),
         [
-            (ldt(2016, 12, 5, 11, 34, 59), ldt(2016, 12, 1, 0, 0, 0)),
-            (ldt(2017, 3, 31, 11, 29, 59), ldt(2017, 3, 1, 0, 0, 0)),
+            (
+                localtime.datetime(2016, 12, 5, 11, 34, 59),
+                localtime.datetime(2016, 12, 1, 0, 0, 0),
+            ),
+            (localtime.datetime(2017, 3, 31, 11, 29, 59), localtime.datetime(2017, 3, 1, 0, 0, 0)),
         ],
     )
     def test_start_of_month(self, dt, result):
         assert localtime.start_of_month(dt) == result
 
 
 class TestEndOfMonth:
     @pytest.mark.parametrize(
         ("dt", "result"),
         [
-            (ldt(2016, 12, 5, 11, 34, 59), ldt(2017, 1, 1, 0, 0, 0)),
-            (ldt(2017, 3, 31, 11, 29, 59), ldt(2017, 4, 1, 0, 0, 0)),
+            (localtime.datetime(2016, 12, 5, 11, 34, 59), localtime.datetime(2017, 1, 1, 0, 0, 0)),
+            (localtime.datetime(2017, 3, 31, 11, 29, 59), localtime.datetime(2017, 4, 1, 0, 0, 0)),
         ],
     )
     def test_end_of_month(self, dt, result):
         assert localtime.end_of_month(dt) == result
 
 
 class TestAsRange:
@@ -592,31 +567,31 @@
             localtime.is_in_the_past(dt)
 
 
 class TestNextMidnight:
     def test_utc_date(self):
         dt = localtime.next_midnight(factories.date("2017-01-01"))
 
-        assert dt.tzinfo.zone == "Europe/London"
+        assert str(dt.tzinfo) == "Europe/London"
         assert dt == localtime.datetime(2017, 1, 2)
 
     def test_dst_start(self):
         dt = localtime.next_midnight(factories.date("2018-03-25"))
 
-        assert dt.tzinfo.zone == "Europe/London"
+        assert str(dt.tzinfo) == "Europe/London"
         assert dt == localtime.datetime(2018, 3, 26)
 
     def test_dst_end(self):
         dt = localtime.next_midnight(factories.date("2018-10-28"))
 
-        assert dt.tzinfo.zone == "Europe/London"
+        assert str(dt.tzinfo) == "Europe/London"
         assert dt == localtime.datetime(2018, 10, 29)
 
     def test_default_in_different_timezone(self):
-        aus_time = pytz.timezone("Etc/GMT-10")
+        aus_time = zoneinfo.ZoneInfo("Etc/GMT-10")
 
         with time_machine.travel(datetime.datetime(2020, 2, 2, 1, tzinfo=aus_time), tick=False):
             result = localtime.next_midnight(tz=aus_time)
 
         assert result == datetime.datetime(2020, 2, 3, 0, 0, tzinfo=aus_time)
 
     @pytest.mark.parametrize(
@@ -632,15 +607,15 @@
             (localtime.datetime(2018, 10, 29), localtime.datetime(2018, 10, 30)),
         ],
     )
     def test_dst_end_datetime(self, dt, expected):
         result = localtime.next_midnight(dt)
 
         assert result == expected
-        assert result.tzinfo.zone == "Europe/London"
+        assert str(result.tzinfo) == "Europe/London"
 
 
 class TestDaysInThePast:
     def test_is_sane(self):
         assert localtime.days_in_the_past(2) == datetime.date.today() - datetime.timedelta(days=2)
         assert localtime.days_in_the_past(-20) == datetime.date.today() + datetime.timedelta(
             days=20
@@ -761,55 +736,41 @@
         supplied_date = factories.date(supplied_date_str)
         with time_machine.travel(now, tick=False):
             assert localtime.is_within_the_last_week(supplied_date) == is_within_last_year
 
 
 class TestIsDST:
     @pytest.mark.parametrize(
-        "naive_datetime,tz_name,expected",
+        "naive_datetime,tz,expected",
         (
             # Test London timezone
-            (datetime.datetime(2019, 1, 1), "Europe/London", False),
-            (datetime.datetime(2019, 6, 1), "Europe/London", True),
+            (datetime.datetime(2019, 1, 1), zoneinfo.ZoneInfo("Europe/London"), False),
+            (datetime.datetime(2019, 6, 1), zoneinfo.ZoneInfo("Europe/London"), True),
             # Test London boundaries
-            (datetime.datetime(2017, 3, 26, 0, 0), "Europe/London", False),
-            (datetime.datetime(2017, 3, 26, 2, 0), "Europe/London", True),
-            (datetime.datetime(2017, 10, 29, 0, 0), "Europe/London", True),
-            (datetime.datetime(2017, 10, 29, 2, 0), "Europe/London", False),
+            (datetime.datetime(2017, 3, 26, 0, 0), zoneinfo.ZoneInfo("Europe/London"), False),
+            (datetime.datetime(2017, 3, 26, 2, 0), zoneinfo.ZoneInfo("Europe/London"), True),
+            (datetime.datetime(2017, 10, 29, 0, 0), zoneinfo.ZoneInfo("Europe/London"), True),
+            (datetime.datetime(2017, 10, 29, 2, 0), zoneinfo.ZoneInfo("Europe/London"), False),
             # UTC should never be DST
-            (datetime.datetime(2019, 1, 1), "UTC", False),
-            (datetime.datetime(2019, 6, 1), "UTC", False),
+            (datetime.datetime(2019, 1, 1), zoneinfo.ZoneInfo("UTC"), False),
+            (datetime.datetime(2019, 6, 1), zoneinfo.ZoneInfo("UTC"), False),
+            (datetime.datetime(2019, 1, 1), datetime.timezone.utc, False),
+            (datetime.datetime(2019, 6, 1), datetime.timezone.utc, False),
             # Test Eastern Australia timezone
-            (datetime.datetime(2019, 1, 1), "Australia/Sydney", True),
-            (datetime.datetime(2019, 6, 1), "Australia/Sydney", False),
+            (datetime.datetime(2019, 1, 1), zoneinfo.ZoneInfo("Australia/Sydney"), True),
+            (datetime.datetime(2019, 6, 1), zoneinfo.ZoneInfo("Australia/Sydney"), False),
             # Test Western Australia timezone (they don't have DST)
-            (datetime.datetime(2019, 1, 1), "Australia/Perth", False),
-            (datetime.datetime(2019, 6, 1), "Australia/Perth", False),
+            (datetime.datetime(2019, 1, 1), zoneinfo.ZoneInfo("Australia/Perth"), False),
+            (datetime.datetime(2019, 6, 1), zoneinfo.ZoneInfo("Australia/Perth"), False),
         ),
     )
-    def test_returns_correct_values(self, naive_datetime, tz_name, expected):
-        local_dt = timezone.make_aware(naive_datetime, timezone=pytz.timezone(tz_name))
+    def test_returns_correct_values(self, naive_datetime, tz, expected):
+        local_dt = timezone.make_aware(naive_datetime, timezone=tz)
         assert localtime.is_dst(local_dt) == expected
 
-    @pytest.mark.parametrize(
-        "naive_datetime,tz_name", ((datetime.datetime(2017, 3, 26, 1, 0), "Europe/London"),)
-    )
-    def test_non_existent_time_error(self, naive_datetime, tz_name):
-        with pytest.raises(pytz.exceptions.NonExistentTimeError):
-            local_dt = timezone.make_aware(naive_datetime, timezone=pytz.timezone(tz_name))
-            localtime.is_dst(local_dt)
-
-    @pytest.mark.parametrize(
-        "naive_datetime,tz_name", ((datetime.datetime(2017, 10, 29, 1, 0), "Europe/London"),)
-    )
-    def test_raises_ambiguous_time_error(self, naive_datetime, tz_name):
-        with pytest.raises(pytz.exceptions.AmbiguousTimeError):
-            local_dt = timezone.make_aware(naive_datetime, timezone=pytz.timezone(tz_name))
-            localtime.is_dst(local_dt)
-
     def test_raises_value_error_for_naive_dt(self):
         with pytest.raises(ValueError):
             localtime.is_dst(datetime.datetime(2008, 4, 5))
 
 
 class TestIsLocaltimeMidnight:
     @pytest.mark.parametrize(
@@ -836,50 +797,52 @@
     )
     def test_returns_false_for_non_localtime_midnights(self, dt):
         assert not localtime.is_localtime_midnight(dt)
 
     def test_returns_false_if_timezone_differs(self):
         assert not localtime.is_localtime_midnight(
             factories.utc.dt("2020-12-01 00:00"),
-            tz=pytz.timezone("Europe/Paris"),
+            tz=zoneinfo.ZoneInfo("Europe/Paris"),
         )
 
 
 class TestCombine:
     @pytest.mark.parametrize(
         "date, time, tz_name, expected",
         (
             (
                 factories.date("1 Jan 2020"),
                 factories.time("00:00"),
                 "UTC",
-                datetime.datetime(2020, 1, 1, tzinfo=pytz.UTC),
+                datetime.datetime(2020, 1, 1, tzinfo=localtime.UTC),
             ),
             (
                 factories.date("1 Jan 2020"),
                 factories.time("00:00"),
                 "UTC",
                 datetime.datetime(2020, 1, 1, tzinfo=datetime.timezone.utc),
             ),
             (
                 factories.date("1 Jun 2020"),
                 factories.time("01:00"),
                 "Europe/London",
-                datetime.datetime(2020, 6, 1, 1, 0).astimezone(pytz.timezone("Europe/London")),
+                datetime.datetime(2020, 6, 1, 1, 0).astimezone(zoneinfo.ZoneInfo("Europe/London")),
             ),
             (
                 factories.date("1 Jul 2021"),
                 factories.time("02:30"),
                 "Europe/London",
-                datetime.datetime(2021, 7, 1, 2, 30).astimezone(pytz.timezone("Europe/London")),
+                datetime.datetime(2021, 7, 1, 2, 30).astimezone(
+                    zoneinfo.ZoneInfo("Europe/London")
+                ),
             ),
         ),
     )
     def test_combines_as_expected(self, date, time, tz_name, expected):
-        tz = pytz.timezone(tz_name)
+        tz = zoneinfo.ZoneInfo(tz_name)
         assert localtime.combine(date, time, tz) == expected
 
 
 class TestNextDateWithDayOfMonth:
     @pytest.mark.parametrize(
         "current_date, day_of_month, expected",
         (
@@ -937,15 +900,15 @@
     @override_settings(TIME_ZONE="Etc/GMT-10")
     def test_timestamp_in_aus_timezone(self):
         timestamp = 1605804900
         dt = localtime.datetime_from_epoch_timestamp(timestamp)
         assert dt == localtime.datetime(2020, 11, 20, 2, 55)
 
     def test_timestamp_with_timestamp_argument(self):
-        aus_time = pytz.timezone("Etc/GMT-10")
+        aus_time = zoneinfo.ZoneInfo("Etc/GMT-10")
         timestamp = 1605804900
 
         dt = localtime.datetime_from_epoch_timestamp(timestamp, tz=aus_time)
         assert dt == datetime.datetime(2020, 11, 20, 2, 55, tzinfo=aus_time)
 
     @override_settings(TIME_ZONE="Europe/London")
     def test_timestamp_british_summer_time_before_clocks_move_forward(self):
```

### Comparing `xocto-3.2.0/tests/test_numbers.py` & `xocto-4.0.0/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/tests/test_ranges.py` & `xocto-4.0.0/tests/test_ranges.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/tests/test_settlement_periods.py` & `xocto-4.0.0/tests/test_settlement_periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import datetime
 
 import pytest
 import pytz
 
 from xocto import settlement_periods
 
-UTC_TZ = pytz.utc
+UTC_TZ = datetime.timezone.utc
 GB_TZ = pytz.timezone("Europe/London")
 
 
 @pytest.mark.parametrize(
     "sp,date,expected",
     [
         # British time is GMT
```

### Comparing `xocto-3.2.0/xocto/events/core.py` & `xocto-4.0.0/xocto/events/core.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/health.py` & `xocto-4.0.0/xocto/health.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/localtime.py` & `xocto-4.0.0/xocto/localtime.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 from __future__ import annotations
 
 import calendar
 import datetime as datetime_
 import decimal
+import zoneinfo
 from typing import Generator, Optional, Sequence, Tuple, Union
 
-import pytz
 from dateutil import tz
 from dateutil.relativedelta import relativedelta
 from django.utils import timezone
 
 from . import numbers, ranges
 
-# Convenience type aliases for referencing from other modules. The 'Union` is redundant and just
-# to help mypy realise that these are type aliases, not assignments.
-Date = Union[datetime_.date]
-DateTime = Union[datetime_.datetime]
-DateOrDatetime = Union[Date, DateTime]
-Time = Union[datetime_.time]
-TimeDelta = Union[datetime_.timedelta]
-
 # Timezone aware datetime in the far future.
 far_future = timezone.make_aware(datetime_.datetime.max - datetime_.timedelta(days=2))
 
 # Timezone aware datetime in the far past.
 far_past = timezone.make_aware(datetime_.datetime.min + datetime_.timedelta(days=2))
 
 UTC = datetime_.timezone.utc
-LONDON = pytz.timezone("Europe/London")
+LONDON = zoneinfo.ZoneInfo("Europe/London")
 
 ONE_DAY = datetime_.timedelta(days=1)
 ONE_HOUR = datetime_.timedelta(hours=1)
 
 MIDNIGHT_TIME = datetime_.time(0, 0)
 
 
@@ -46,15 +38,15 @@
     return timezone.localtime(dt, timezone=tz)
 
 
 def as_utc(dt: datetime_.datetime) -> datetime_.datetime:
     """
     Wrapper for normalizing a datetime aware object into UTC.
     """
-    return as_localtime(dt, datetime_.timezone.utc)
+    return as_localtime(dt, UTC)
 
 
 def now() -> datetime_.datetime:
     """
     Return the current datetime in the local timezone.
     """
     return as_localtime(timezone.now())
@@ -64,24 +56,20 @@
     year: int,
     month: int,
     day: int,
     hour: int = 0,
     minute: int = 0,
     second: int = 0,
     microsecond: int = 0,
-    is_dst: bool | None = None,
 ) -> datetime_.datetime:
     """
     Return a datetime in the local timezone.
-
-    A boolean value is required for is_dst to unambiguously determine the appropriate dt during the
-    window when the hour goes back.
     """
     dt = datetime_.datetime(year, month, day, hour, minute, second, microsecond)
-    return timezone.make_aware(dt, is_dst=is_dst)
+    return timezone.make_aware(dt)
 
 
 # Returning dates
 
 
 def date(dt: datetime_.datetime, tz: timezone.zoneinfo.ZoneInfo | None = None) -> datetime_.date:
     """
@@ -203,24 +191,25 @@
     return now() - relativedelta(seconds=n)
 
 
 # Converting dates into datetimes
 
 
 def midnight(
-    date_or_datetime: Optional[DateOrDatetime] = None, tz: Optional[datetime_.tzinfo] = None
+    date_or_datetime: Optional[Union[datetime_.date, datetime_.datetime]] = None,
+    tz: Optional[datetime_.tzinfo] = None,
 ) -> datetime_.datetime:
     """
     Return a TZ-aware datetime for midnight of the passed date.
 
     If date is None then the current date in the passed timezone is used (if no timezone is
     supplied then we use the local timezone).
     """
     if date_or_datetime is None:
-        date_: Date = today(tz)
+        date_: datetime_.date = today(tz)
     elif isinstance(date_or_datetime, datetime_.datetime):
         # Although this function is meant to be used on dates, we want to handle datetimes
         # properly as well, as these are frequently passed in as a way of 'truncating' them to
         # midnight on that date.
         if timezone.is_naive(date_or_datetime):
             # Default to localtime if no tz provided, as_localtime takes tz aware args.
             date_ = date(timezone.make_aware(date_or_datetime), tz)
@@ -230,23 +219,24 @@
         date_ = date_or_datetime
 
     naive_midnight = datetime_.datetime.combine(date_, datetime_.datetime.min.time())
     return timezone.make_aware(naive_midnight, timezone=tz)
 
 
 def next_midnight(
-    date_or_datetime: Optional[DateOrDatetime] = None, tz: Optional[datetime_.tzinfo] = None
+    date_or_datetime: Optional[Union[datetime_.date, datetime_.datetime]] = None,
+    tz: Optional[datetime_.tzinfo] = None,
 ) -> datetime_.datetime:
     """
     Return the datetime for midnight of the following day to the date passed in.
 
     This is intuitively what people think of as midnight.
     """
     if date_or_datetime is None:
-        date_: Date = today(tz)
+        date_: datetime_.date = today(tz)
     elif isinstance(date_or_datetime, datetime_.datetime):
         # Although this function is meant to be used on dates, we want to handle datetimes
         # properly as well
         if timezone.is_naive(date_or_datetime):
             # Default to localtime if no tz provided, as_localtime takes tz aware args
             date_ = date(timezone.make_aware(date_or_datetime), tz)
         else:
@@ -310,25 +300,23 @@
 def combine(_date: datetime_.date, _time: datetime_.time, tz: timezone.zone) -> datetime_.datetime:
     """
     Return a TZ-aware datetime obtained by combining the given date and time.
 
     It's a TZ-aware wrapper around datetime.datetime.combine.
     """
     combined_dt = datetime_.datetime.combine(_date, _time)
-    if tz is datetime_.timezone.utc:
-        return combined_dt.replace(tzinfo=tz)
-    return tz.localize(combined_dt)
+    return timezone.make_aware(combined_dt, timezone=tz)
 
 
 # Converting dates into datetime pairs
 
 
 def date_boundaries(
-    _date: Optional[Date], tz: Optional[datetime_.tzinfo] = None
-) -> Tuple[DateTime, DateTime]:
+    _date: Optional[datetime_.date], tz: Optional[datetime_.tzinfo] = None
+) -> Tuple[datetime_.datetime, datetime_.datetime]:
     """
     Return a 2-tuple with the start and ending dt for the given date in the local timezone.
 
     Note, be careful of using this with __range ORM queries as such queries are INCLUSIVE on the
     boundaries.
     """
     return midnight(_date, tz), next_midnight(_date, tz)
@@ -343,61 +331,57 @@
     For example:
 
         >>> month_boundaries(1, 2020)
         ((datetime.datetime(2020, 1, 1, 0, 0), datetime.datetime(2020, 2, 1, 0, 0))
     """
     start_date = datetime_.date(year, month, 1)
     end_date = start_date + relativedelta(months=1)
-    return (midnight(start_date), midnight(end_date))
+    return midnight(start_date), midnight(end_date)
 
 
 def as_range(
-    _date: Optional[Date], tz: Optional[datetime_.tzinfo] = None
-) -> Tuple[DateTime, DateTime]:
+    _date: Optional[datetime_.date], tz: Optional[datetime_.tzinfo] = None
+) -> Tuple[datetime_.datetime, datetime_.datetime]:
     """
     Return a 2-tuple of the min and max datetimes for the given date.
 
     This gives values that can be passed to the ORM __range filter.
     """
     return midnight(_date, tz), latest(_date, tz)
 
 
 def make_aware_assuming_local(dt: datetime_.datetime) -> datetime_.datetime:
     """
     Just a wrapper for Django's method, which will takes a naive datetime, and makes it timezone
     aware, assuming the current timezone if none is passed (which it isn't from this wrapper
     function). It will also raise an exception if the passed datetime is already timezone-aware.
     """
-    return timezone.make_aware(dt, is_dst=True)
+    return timezone.make_aware(dt)
 
 
 def make_aware_assuming_utc(dt: datetime_.datetime) -> datetime_.datetime:
     """
     Return a timezone-aware datetime (in UTC) given a naive datetime.
     """
     return timezone.make_aware(dt, timezone=UTC)
 
 
 def is_utc(dt: datetime_.datetime) -> bool:
     """
     Test whether a given (timezone-aware) datetime is in UTC time or not.
     """
-    assert dt.tzinfo, "Must be an aware datetime"
-    timezone_name = dt.tzinfo.tzname(None) or str(dt.tzinfo)
-    return timezone_name.upper() == "UTC"
+    return str(dt.tzinfo) == "UTC"
 
 
 def is_local_time(dt: datetime_.datetime) -> bool:
     """
     Test whether a given (timezone-aware) datetime is in local time or not.
     """
-    if dt.tzinfo is datetime_.timezone.utc:
-        dt = dt.replace(tzinfo=pytz.utc)
     current_timezone = timezone.get_current_timezone()
-    return current_timezone.normalize(dt).tzinfo == dt.tzinfo
+    return dt.tzinfo == current_timezone
 
 
 def within_date_range(
     first_date: datetime_.date, second_date: datetime_.date, days: int = 3
 ) -> bool:
     """
     Check if two dates are within a range from each other.
@@ -622,24 +606,20 @@
 
 
 def is_dst(local_time: datetime_.datetime) -> bool:
     """
     Indicate whether the given time (and timezone is in daylight savings time (DST or not).
 
     Raises:
-        pytz.exceptions.NonExistentTimeError if the time doesn't exist.
-        pytz.exceptions.AmbiguousTimeError if the time exists in both DST and non-DST
-        ValueError if `local_time` doesn't have any timezone information
+        ValueError if `local_time` is a naive datetime.
     """
-    if not local_time.tzinfo:
+    if timezone.is_naive(local_time):
         raise ValueError("Can't determine DST for a naive datetime")
 
-    localised_dt = local_time.tzinfo.normalize(local_time)  # type: ignore[attr-defined]
-
-    return bool(localised_dt.dst())
+    return bool(local_time.dst())
 
 
 def is_localtime_midnight(dt: datetime_.datetime, tz: Optional[datetime_.tzinfo] = None) -> bool:
     """
     Return whether the supplied datetime is at midnight (in the site's local time zone).
 
     Note, the supplied datetime, which should be timezone aware, may be in any timezone,
@@ -653,15 +633,17 @@
 ) -> bool:
     """
     Return whether this range is aligned to localtime midnight.
     """
     return all([is_localtime_midnight(range.start, tz), is_localtime_midnight(range.end, tz)])
 
 
-def consolidate_into_intervals(dates: Sequence[Date]) -> Sequence[Tuple[Date, Date]]:
+def consolidate_into_intervals(
+    dates: Sequence[datetime_.date],
+) -> Sequence[Tuple[datetime_.date, datetime_.date]]:
     """
     Given a sequence of dates, return tuples of (inclusive) boundaries of the sub-sequences where
     the dates are consecutive.
 
     If a date does not form a continuous interval with any other dates - i.e. it is separated by at
     least a day before and after the others - it forms an interval with itself as both boundaries.
 
@@ -717,15 +699,15 @@
         "October": "octubre",
         "November": "noviembre",
         "December": "deciembre",
     }
     return month_name_lookup[month_name]
 
 
-def period_exceeds_one_year(start_at: DateTime, end_at: DateTime) -> bool:
+def period_exceeds_one_year(start_at: datetime_.datetime, end_at: datetime_.datetime) -> bool:
     """
     Returns true if the passed period exceeds one year.
 
     Edge cases such as leap years and daylight savings time are handled, where a simple approach
     using only relativedelta would not be sufficient.
     """
```

### Comparing `xocto-3.2.0/xocto/numbers.py` & `xocto-4.0.0/xocto/numbers.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/pact_testing.py` & `xocto-4.0.0/xocto/pact_testing.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/ranges.py` & `xocto-4.0.0/xocto/ranges.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/settlement_periods.py` & `xocto-4.0.0/xocto/settlement_periods.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 def convert_sp_and_date_to_utc(
     sp: int, date: datetime.date, timezone_str: str = GB_TZ, is_wholesale: bool = False
 ) -> datetime.datetime:
     """
     Return an UTC-aware datetime for the start of a given settlement period.
     """
     local_time = convert_sp_and_date_to_local(sp, date, timezone_str, is_wholesale)
-    return _to_timezone(local_time, UTC_TZ)
+    return _to_timezone(local_time, UTC_TZ).replace(tzinfo=datetime.timezone.utc)
 
 
 def convert_local_to_sp_and_date(
     local_time: datetime.datetime, is_wholesale: bool = False
 ) -> typing.Tuple[int, datetime.date]:
     """
     Return the date and settlement period from a given tz-aware datetime.
```

### Comparing `xocto-3.2.0/xocto/storage/files.py` & `xocto-4.0.0/xocto/storage/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 import csv
 import hashlib
 import io
 import os
 import tempfile
 from typing import IO, Any, AnyStr, Callable
 
-import pandas as pd
-import xlrd
-
 XLRD_FLOAT_TYPE = 2
 
 
 def size(file: IO[AnyStr]) -> int:
     """
     Return the size of the file in bytes.
     """
@@ -100,14 +97,16 @@
                             file will be created if this arg is not present.
         encoding:           Encoding scheme for csv file.
         errors:             How file object should handle encoding errors.
         quoting:            The type of quoting the CSV file should have
         delimiter:          The delimiter the output CSV file should have
 
     """
+    import xlrd
+
     workbook = xlrd.open_workbook(xls_filepath)
     sheet = workbook.sheet_by_index(0)
 
     csv_file, wr = _get_csv_file_and_writer(csv_filepath, encoding, errors, quoting, delimiter)
     for rownum in range(sheet.nrows):
         row = sheet.row(rownum)
         values = []
@@ -188,14 +187,16 @@
     :param data: bytes contents for/from a CSV file
     :param na_values: Additional strings to recognize as NA/NaN. If dict passed, specific
     per-column NA values.
     :param data_type: Data type for data or columns. You can Use str, object or a dict with
     the column names and types. E.g. {‘a’: np.float64, ‘b’: np.int32, ‘c’: ‘Int64’}
     :return: bytes for a Parquet file
     """
+    import pandas as pd
+
     dataframe = pd.read_csv(
         io.BytesIO(data),
         dtype=data_type,
         na_values=na_values,
         parse_dates=parse_dates,
         thousands=",",
     )
```

### Comparing `xocto-3.2.0/xocto/storage/s3_select.py` & `xocto-4.0.0/xocto/storage/s3_select.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/storage/storage.py` & `xocto-4.0.0/xocto/storage/storage.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/tracing.py` & `xocto-4.0.0/xocto/tracing.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto/types.py` & `xocto-4.0.0/xocto/types.py`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto.egg-info/PKG-INFO` & `xocto-4.0.0/xocto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xocto
-Version: 3.2.0
+Version: 4.0.0
 Summary: Kraken Technologies Python service utilities
 Home-page: https://github.com/octoenergy/xocto
 Author: Kraken Technologies
 Author-email: talent@octopus.energy
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xocto-3.2.0/xocto.egg-info/SOURCES.txt` & `xocto-4.0.0/xocto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xocto-3.2.0/xocto.egg-info/requires.txt` & `xocto-4.0.0/xocto.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ddtrace>=1.9.0
-django<5.0,>=3.2
+django>=4.0
 openpyxl>=3.1.0
 pact-python>=1.6.0
 pandas>=1.5.3
 pyarrow>=11.0.0
 python-dateutil>=2.8.2
 python-magic>=0.4.27
 pytz
```

