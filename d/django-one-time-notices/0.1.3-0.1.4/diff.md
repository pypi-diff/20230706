# Comparing `tmp/django_one_time_notices-0.1.3.tar.gz` & `tmp/django_one_time_notices-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_one_time_notices-0.1.3.tar", max compression
+gzip compressed data, was "django_one_time_notices-0.1.4.tar", max compression
```

## Comparing `django_one_time_notices-0.1.3.tar` & `django_one_time_notices-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2441 2023-07-06 07:39:23.982751 django_one_time_notices-0.1.3/README.md
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/__init__.py
--rw-r--r--   0        0        0      141 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/admin.py
--rw-r--r--   0        0        0      146 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/apps.py
--rw-r--r--   0        0        0     1078 2023-07-05 10:24:30.076861 django_one_time_notices-0.1.3/notices/context_processors.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/migrations/__init__.py
--rw-r--r--   0        0        0      553 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/templates/example_app/home.html
--rw-r--r--   0        0        0      123 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/views.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/__init__.py
--rw-r--r--   0        0        0      401 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/asgi.py
--rw-r--r--   0        0        0     2888 2022-10-17 17:43:23.021443 django_one_time_notices-0.1.3/notices/example_project/example_project/settings.py
--rw-r--r--   0        0        0      811 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/urls.py
--rw-r--r--   0        0        0      404 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/wsgi.py
--rwxr-xr-x   0        0        0      671 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/manage.py
--rw-r--r--   0        0        0      865 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/migrations/0001_initial.py
--rw-r--r--   0        0        0      397 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/migrations/0002_alter_notice_version.py
--rw-r--r--   0        0        0      414 2023-07-05 08:34:05.713146 django_one_time_notices-0.1.3/notices/migrations/0003_notice_timeout_seconds.py
--rw-r--r--   0        0        0      403 2023-07-06 07:11:27.361085 django_one_time_notices-0.1.3/notices/migrations/0004_notice_starts_at.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/migrations/__init__.py
--rw-r--r--   0        0        0     2447 2023-07-06 07:45:06.517339 django_one_time_notices-0.1.3/notices/models.py
--rw-r--r--   0        0        0      864 2022-10-17 17:34:52.769745 django_one_time_notices-0.1.3/notices/static/notices/css/notices.css
--rw-r--r--   0        0        0     1101 2023-07-05 08:24:49.738939 django_one_time_notices-0.1.3/notices/static/notices/js/notices.js
--rw-r--r--   0        0        0      909 2023-07-05 08:53:25.144794 django_one_time_notices-0.1.3/notices/templates/notices/notices.html
--rw-r--r--   0        0        0       29 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/templates/notices/notices_clear.html
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/templatetags/__init__.py
--rw-r--r--   0        0        0     1678 2023-07-06 07:56:14.270567 django_one_time_notices-0.1.3/notices/templatetags/notices_tags.py
--rw-r--r--   0        0        0     1550 2023-07-06 07:58:53.929902 django_one_time_notices-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 django_one_time_notices-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2622 2023-07-06 09:02:29.912774 django_one_time_notices-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/__init__.py
+-rw-r--r--   0        0        0      141 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/admin.py
+-rw-r--r--   0        0        0      146 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/apps.py
+-rw-r--r--   0        0        0     1238 2023-07-06 09:19:40.240769 django_one_time_notices-0.1.4/notices/context_processors.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_app/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_app/migrations/__init__.py
+-rw-r--r--   0        0        0      553 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_app/templates/example_app/home.html
+-rw-r--r--   0        0        0      123 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_app/views.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_project/__init__.py
+-rw-r--r--   0        0        0      401 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_project/asgi.py
+-rw-r--r--   0        0        0     2888 2022-10-17 17:43:23.021443 django_one_time_notices-0.1.4/notices/example_project/example_project/settings.py
+-rw-r--r--   0        0        0      811 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_project/urls.py
+-rw-r--r--   0        0        0      404 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/example_project/wsgi.py
+-rwxr-xr-x   0        0        0      671 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/example_project/manage.py
+-rw-r--r--   0        0        0      865 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/migrations/0001_initial.py
+-rw-r--r--   0        0        0      397 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/migrations/0002_alter_notice_version.py
+-rw-r--r--   0        0        0      414 2023-07-05 08:34:05.713146 django_one_time_notices-0.1.4/notices/migrations/0003_notice_timeout_seconds.py
+-rw-r--r--   0        0        0      403 2023-07-06 07:11:27.361085 django_one_time_notices-0.1.4/notices/migrations/0004_notice_starts_at.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/migrations/__init__.py
+-rw-r--r--   0        0        0     2525 2023-07-06 09:25:26.640733 django_one_time_notices-0.1.4/notices/models.py
+-rw-r--r--   0        0        0      864 2022-10-17 17:34:52.769745 django_one_time_notices-0.1.4/notices/static/notices/css/notices.css
+-rw-r--r--   0        0        0     1101 2023-07-05 08:24:49.738939 django_one_time_notices-0.1.4/notices/static/notices/js/notices.js
+-rw-r--r--   0        0        0      909 2023-07-06 09:05:55.272797 django_one_time_notices-0.1.4/notices/templates/notices/notices.html
+-rw-r--r--   0        0        0       29 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/templates/notices/notices_clear.html
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.4/notices/templatetags/__init__.py
+-rw-r--r--   0        0        0     1678 2023-07-06 09:19:40.240769 django_one_time_notices-0.1.4/notices/templatetags/notices_tags.py
+-rw-r--r--   0        0        0     1550 2023-07-06 09:28:30.048712 django_one_time_notices-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3221 1970-01-01 00:00:00.000000 django_one_time_notices-0.1.4/PKG-INFO
```

### Comparing `django_one_time_notices-0.1.3/README.md` & `django_one_time_notices-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -72,14 +72,18 @@
 Note that only the notice with the latest version will be shown. If the latest version
 has not started yet, a previous version will not be shown, even if it hasn't expired. 
 
 Set the `timeout_seconds` to set a cookie timeout; this means the notice will be reshown.
 
 To show a new notice, add another Notice instance with an incremented version number.
 
+### configure settings
+`NOTICES_COLOUR`: Change the colour of the popup with any css colour
+`NOTICES_SAFE`: Mark notices content as safe - allow any arbitrary html. Default False.
+
 ### via django settings
 
 Override the Notice model by adding to your `settings.py`:
 `NOTICES_VERSION` # an integer
 `NOTICES_TITLE`  # optional, default = "New!"
 `NOTICES_CONTENT`  # optional, default = ""
 `NOTICES_TIMEOUT_SECONDS`  # optional, default = None
```

### Comparing `django_one_time_notices-0.1.3/notices/context_processors.py` & `django_one_time_notices-0.1.4/notices/context_processors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.conf import settings
+from django.utils.safestring import mark_safe
 
 from notices.models import Notice
 
 
 def notices(request):
     # first try to load Notice config from settings
     settings_config = Notice.from_settings()
@@ -13,14 +14,17 @@
     version = Notice.latest_version()
     if version == 0:
         title = content = colour = timeout_seconds = None
     else:
         latest_notice = Notice.latest_notice()
         title = latest_notice.title
         content = latest_notice.content
+        safe = getattr(settings, "NOTICES_SAFE", False)
+        if safe:
+            content = mark_safe(content)
         if hasattr(settings, "NOTICES_COLOUR"):
             colour_setting = "NOTICES_COLOUR"
         else:
             colour_setting = "NOTICES_COLOR"
         colour = getattr(settings, colour_setting, None)
         # cookie timeout; default to 10 years
         timeout_seconds = latest_notice.timeout_seconds
```

### Comparing `django_one_time_notices-0.1.3/notices/example_project/example_app/templates/example_app/home.html` & `django_one_time_notices-0.1.4/notices/example_project/example_app/templates/example_app/home.html`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/example_project/example_project/settings.py` & `django_one_time_notices-0.1.4/notices/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/example_project/example_project/urls.py` & `django_one_time_notices-0.1.4/notices/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/example_project/manage.py` & `django_one_time_notices-0.1.4/notices/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/migrations/0001_initial.py` & `django_one_time_notices-0.1.4/notices/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/models.py` & `django_one_time_notices-0.1.4/notices/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
                     "notices_version": version,
                     "notices_title": getattr(settings, "NOTICES_TITLE", "New!"),
                     "notices_content": getattr(settings, "NOTICES_CONTENT", ""),
                     "notices_colour": getattr(settings, colour_setting, None),
                     "notices_timeout_seconds": getattr(
                         settings, "NOTICES_TIMEOUT_SECONDS", None
                     ),
+                    "notices_safe": getattr(settings, "NOTICES_SAFE", False),
                 }
 
     def has_expired(self):
         if not self.expires_at:
             return False
         return self.expires_at < timezone.now()
```

### Comparing `django_one_time_notices-0.1.3/notices/static/notices/css/notices.css` & `django_one_time_notices-0.1.4/notices/static/notices/css/notices.css`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/static/notices/js/notices.js` & `django_one_time_notices-0.1.4/notices/static/notices/js/notices.js`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/templates/notices/notices.html` & `django_one_time_notices-0.1.4/notices/templates/notices/notices.html`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/notices/templatetags/notices_tags.py` & `django_one_time_notices-0.1.4/notices/templatetags/notices_tags.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.3/pyproject.toml` & `django_one_time_notices-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-one-time-notices"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Becky Smith <rebkwok@gmail.com>"]
 readme = "README.md"
 packages = [{include = "notices"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `django_one_time_notices-0.1.3/PKG-INFO` & `django_one_time_notices-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-one-time-notices
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: Becky Smith
 Author-email: rebkwok@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -90,14 +90,18 @@
 Note that only the notice with the latest version will be shown. If the latest version
 has not started yet, a previous version will not be shown, even if it hasn't expired. 
 
 Set the `timeout_seconds` to set a cookie timeout; this means the notice will be reshown.
 
 To show a new notice, add another Notice instance with an incremented version number.
 
+### configure settings
+`NOTICES_COLOUR`: Change the colour of the popup with any css colour
+`NOTICES_SAFE`: Mark notices content as safe - allow any arbitrary html. Default False.
+
 ### via django settings
 
 Override the Notice model by adding to your `settings.py`:
 `NOTICES_VERSION` # an integer
 `NOTICES_TITLE`  # optional, default = "New!"
 `NOTICES_CONTENT`  # optional, default = ""
 `NOTICES_TIMEOUT_SECONDS`  # optional, default = None
```

