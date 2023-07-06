# Comparing `tmp/google_play_developer_api-0.5.2.tar.gz` & `tmp/google_play_developer_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_play_developer_api-0.5.2.tar", max compression
+gzip compressed data, was "google_play_developer_api-0.6.0.tar", max compression
```

## Comparing `google_play_developer_api-0.5.2.tar` & `google_play_developer_api-0.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/LICENSE
--rw-r--r--   0        0        0      858 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/README.md
--rw-r--r--   0        0        0       78 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/google_play_developer_api/__init__.py
--rw-r--r--   0        0        0    10876 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/google_play_developer_api/reporting.py
--rw-r--r--   0        0        0     2697 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       37 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/tests/__init__.py
--rw-r--r--   0        0        0     2337 2023-07-04 04:15:15.761397 google_play_developer_api-0.5.2/tests/test_reporting_apis.py
--rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 google_play_developer_api-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/LICENSE
+-rw-r--r--   0        0        0      858 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/README.md
+-rw-r--r--   0        0        0       78 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/google_play_developer_api/__init__.py
+-rw-r--r--   0        0        0    16184 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/google_play_developer_api/reporting.py
+-rw-r--r--   0        0        0     2697 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     4037 2023-07-06 10:22:25.838872 google_play_developer_api-0.6.0/tests/test_reporting_apis.py
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 google_play_developer_api-0.6.0/PKG-INFO
```

### Comparing `google_play_developer_api-0.5.2/LICENSE` & `google_play_developer_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.5.2/README.md` & `google_play_developer_api-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.5.2/google_play_developer_api/reporting.py` & `google_play_developer_api-0.6.0/google_play_developer_api/reporting.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def _get_report_data(
         self,
         app_package_name: str = "",
         timeline_spec: dict = {},
         dimensions: list[str] = [],
         metrics: list[str] = [],
         metric_set: str = "",
-        page_size: int = 100000,
+        page_size: int = 50000,
     ) -> list[dict]:
         """
         Get report data from Google Play Developer API
 
         Note: Read this doc
         https://developers.google.com/play/developer/reporting/reference/rest/v1beta1/vitals.crashrate/query#request-body
 
@@ -325,10 +325,184 @@
             },
         }
 
         return self._get_report_data(
             app_package_name=app_package_name,
             timeline_spec=timeline_spec,
             dimensions=dimensions,
+            metrics=metrics,
+            metric_set=metric_set,
+        )
+
+    def get_anr_rate_report_daily(
+        self,
+        app_package_name: str = "",
+        start_time: str = "YYYY-MM-DD",
+        end_time: str = "YYYY-MM-DD",
+        dimensions: list[str] = [],
+        metrics: list[str] = [],
+    ) -> list[dict]:
+        """
+        Get ANR rate report daily
+
+        Note:
+            Read this doc https://developers.google.com/play/developer/reporting/reference/rest/v1beta1/vitals.anrrate
+
+        Args:
+            app_package_name: App package name
+            start_time: Start time (format YYYY-MM-DD)
+            end_time: End time (format YYYY-MM-DD)
+            dimensions: Dimensions (see docs above)
+            metrics: Metrics (see docs above)
+
+        Returns:
+            List of dicts with report data
+        """
+        dimensions = (
+            [
+                "apiLevel",
+                "deviceBrand",
+                "versionCode",
+                "countryCode",
+                "deviceType",
+                "deviceModel",
+                "deviceRamBucket",
+                "deviceSocMake",
+                "deviceSocModel",
+                "deviceCpuMake",
+                "deviceCpuModel",
+                "deviceGpuMake",
+                "deviceGpuModel",
+                "deviceGpuVersion",
+                "deviceVulkanVersion",
+                "deviceGlEsVersion",
+                "deviceScreenSize",
+                "deviceScreenDpi",
+            ]
+            if not dimensions
+            else dimensions
+        )
+
+        metrics = (
+            [
+                "anrRate",
+                "userPerceivedAnrRate",
+                "distinctUsers",
+            ]
+            if not metrics
+            else metrics
+        )
+        metric_set = "anrRateMetricSet"
+
+        start_time = datetime.datetime.strptime(start_time, "%Y-%m-%d")
+        end_time = datetime.datetime.strptime(end_time, "%Y-%m-%d")
+
+        timeline_spec = {
+            "aggregationPeriod": "DAILY",
+            "startTime": {
+                "year": start_time.year,
+                "month": start_time.month,
+                "day": start_time.day,
+                "timeZone": {"id": "America/Los_Angeles"}
+            },
+            "endTime": {
+                "year": end_time.year,
+                "month": end_time.month,
+                "day": end_time.day,
+                "timeZone": {"id": "America/Los_Angeles"}
+            },
+        }
+
+        return self._get_report_data(
+            app_package_name=app_package_name,
+            timeline_spec=timeline_spec,
+            dimensions=dimensions,
+            metrics=metrics,
+            metric_set=metric_set,
+        )
+
+    def get_crash_rate_report_daily(
+        self,
+        app_package_name: str = "",
+        start_time: str = "YYYY-MM-DD",
+        end_time: str = "YYYY-MM-DD",
+        dimensions: list[str] = [],
+        metrics: list[str] = [],
+    ) -> list[dict]:
+        """
+        Get crash rate report daily
+
+        Note:
+            Read this doc https://developers.google.com/play/developer/reporting/reference/rest/v1beta1/vitals.crashrate/query#request-body
+
+        Args:
+            app_package_name: App package name
+            start_time: Start time (format YYYY-MM-DD)
+            end_time: End time (format YYYY-MM-DD)
+            dimensions: Dimensions (see docs above)
+            metrics: Metrics (see docs above)
+
+        Returns:
+            List of dicts with report data
+        """
+        dimensions = (
+            [
+                "apiLevel",
+                "deviceBrand",
+                "versionCode",
+                "countryCode",
+                "deviceType",
+                "deviceModel",
+                "deviceRamBucket",
+                "deviceSocMake",
+                "deviceSocModel",
+                "deviceCpuMake",
+                "deviceCpuModel",
+                "deviceGpuMake",
+                "deviceGpuModel",
+                "deviceGpuVersion",
+                "deviceVulkanVersion",
+                "deviceGlEsVersion",
+                "deviceScreenSize",
+                "deviceScreenDpi",
+            ]
+            if not dimensions
+            else dimensions
+        )
+
+        metrics = (
+            [
+                "crashRate",
+                "userPerceivedCrashRate",
+                "distinctUsers",
+            ]
+            if not metrics
+            else metrics
+        )
+        metric_set = "crashRateMetricSet"
+
+        start_time = datetime.datetime.strptime(start_time, "%Y-%m-%d")
+        end_time = datetime.datetime.strptime(end_time, "%Y-%m-%d")
+
+        timeline_spec = {
+            "aggregationPeriod": "DAILY",
+            "startTime": {
+                "year": start_time.year,
+                "month": start_time.month,
+                "day": start_time.day,
+                "timeZone": {"id": "America/Los_Angeles"},
+            },
+            "endTime": {
+                "year": end_time.year,
+                "month": end_time.month,
+                "day": end_time.day,
+                "timeZone": {"id": "America/Los_Angeles"},
+            },
+        }
+
+        return self._get_report_data(
+            app_package_name=app_package_name,
+            timeline_spec=timeline_spec,
+            dimensions=dimensions,
             metrics=metrics,
             metric_set=metric_set,
         )
```

### Comparing `google_play_developer_api-0.5.2/pyproject.toml` & `google_play_developer_api-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "google-play-developer-api"
-version = "0.5.2"
+version = "0.6.0"
 homepage = "https://github.com/ikameglobal/google-play-developer-api"
 description = "Wrapper for APIs"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `google_play_developer_api-0.5.2/PKG-INFO` & `google_play_developer_api-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-play-developer-api
-Version: 0.5.2
+Version: 0.6.0
 Summary: Wrapper for APIs
 Home-page: https://github.com/ikameglobal/google-play-developer-api
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

