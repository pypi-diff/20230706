# Comparing `tmp/django_one_time_notices-0.1.2.tar.gz` & `tmp/django_one_time_notices-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_one_time_notices-0.1.2.tar", max compression
+gzip compressed data, was "django_one_time_notices-0.1.3.tar", max compression
```

## Comparing `django_one_time_notices-0.1.2.tar` & `django_one_time_notices-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     2166 2023-07-05 09:12:05.416089 django_one_time_notices-0.1.2/README.md
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/__init__.py
--rw-r--r--   0        0        0      141 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/admin.py
--rw-r--r--   0        0        0      146 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/apps.py
--rw-r--r--   0        0        0     1078 2023-07-05 10:24:30.076861 django_one_time_notices-0.1.2/notices/context_processors.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/__init__.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/migrations/__init__.py
--rw-r--r--   0        0        0      553 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/templates/example_app/home.html
--rw-r--r--   0        0        0      123 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_app/views.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/__init__.py
--rw-r--r--   0        0        0      401 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/asgi.py
--rw-r--r--   0        0        0     2888 2022-10-17 17:43:23.021443 django_one_time_notices-0.1.2/notices/example_project/example_project/settings.py
--rw-r--r--   0        0        0      811 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/urls.py
--rw-r--r--   0        0        0      404 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/example_project/wsgi.py
--rwxr-xr-x   0        0        0      671 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/example_project/manage.py
--rw-r--r--   0        0        0      865 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/migrations/0001_initial.py
--rw-r--r--   0        0        0      397 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/migrations/0002_alter_notice_version.py
--rw-r--r--   0        0        0      414 2023-07-05 08:34:05.713146 django_one_time_notices-0.1.2/notices/migrations/0003_notice_timeout_seconds.py
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/migrations/__init__.py
--rw-r--r--   0        0        0     2080 2023-07-05 10:24:30.092861 django_one_time_notices-0.1.2/notices/models.py
--rw-r--r--   0        0        0      864 2022-10-17 17:34:52.769745 django_one_time_notices-0.1.2/notices/static/notices/css/notices.css
--rw-r--r--   0        0        0     1101 2023-07-05 08:24:49.738939 django_one_time_notices-0.1.2/notices/static/notices/js/notices.js
--rw-r--r--   0        0        0      909 2023-07-05 08:53:25.144794 django_one_time_notices-0.1.2/notices/templates/notices/notices.html
--rw-r--r--   0        0        0       29 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/templates/notices/notices_clear.html
--rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/templatetags/__init__.py
--rw-r--r--   0        0        0     1643 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.2/notices/templatetags/notices_tags.py
--rw-r--r--   0        0        0     1482 2023-07-05 09:13:02.068042 django_one_time_notices-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2765 1970-01-01 00:00:00.000000 django_one_time_notices-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2441 2023-07-06 07:39:23.982751 django_one_time_notices-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/__init__.py
+-rw-r--r--   0        0        0      141 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/admin.py
+-rw-r--r--   0        0        0      146 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/apps.py
+-rw-r--r--   0        0        0     1078 2023-07-05 10:24:30.076861 django_one_time_notices-0.1.3/notices/context_processors.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/migrations/__init__.py
+-rw-r--r--   0        0        0      553 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/templates/example_app/home.html
+-rw-r--r--   0        0        0      123 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_app/views.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/__init__.py
+-rw-r--r--   0        0        0      401 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/asgi.py
+-rw-r--r--   0        0        0     2888 2022-10-17 17:43:23.021443 django_one_time_notices-0.1.3/notices/example_project/example_project/settings.py
+-rw-r--r--   0        0        0      811 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/urls.py
+-rw-r--r--   0        0        0      404 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/example_project/wsgi.py
+-rwxr-xr-x   0        0        0      671 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/example_project/manage.py
+-rw-r--r--   0        0        0      865 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/migrations/0001_initial.py
+-rw-r--r--   0        0        0      397 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/migrations/0002_alter_notice_version.py
+-rw-r--r--   0        0        0      414 2023-07-05 08:34:05.713146 django_one_time_notices-0.1.3/notices/migrations/0003_notice_timeout_seconds.py
+-rw-r--r--   0        0        0      403 2023-07-06 07:11:27.361085 django_one_time_notices-0.1.3/notices/migrations/0004_notice_starts_at.py
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/migrations/__init__.py
+-rw-r--r--   0        0        0     2447 2023-07-06 07:45:06.517339 django_one_time_notices-0.1.3/notices/models.py
+-rw-r--r--   0        0        0      864 2022-10-17 17:34:52.769745 django_one_time_notices-0.1.3/notices/static/notices/css/notices.css
+-rw-r--r--   0        0        0     1101 2023-07-05 08:24:49.738939 django_one_time_notices-0.1.3/notices/static/notices/js/notices.js
+-rw-r--r--   0        0        0      909 2023-07-05 08:53:25.144794 django_one_time_notices-0.1.3/notices/templates/notices/notices.html
+-rw-r--r--   0        0        0       29 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/templates/notices/notices_clear.html
+-rw-r--r--   0        0        0        0 2022-10-17 16:55:57.370315 django_one_time_notices-0.1.3/notices/templatetags/__init__.py
+-rw-r--r--   0        0        0     1678 2023-07-06 07:56:14.270567 django_one_time_notices-0.1.3/notices/templatetags/notices_tags.py
+-rw-r--r--   0        0        0     1550 2023-07-06 07:58:53.929902 django_one_time_notices-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 django_one_time_notices-0.1.3/PKG-INFO
```

### Comparing `django_one_time_notices-0.1.2/README.md` & `django_one_time_notices-0.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -60,17 +60,21 @@
 The modal will be shown.  Once it has been dismissed it won't be shown again unless the notice version changes (see below), the `notice_seen` cookie is deleted, or the notice timeout is reached.
 
 ## Setting/updating the notice
 
 ### via models and django admin
 Add a `Notice` instance in the django admin. 
 
-Notices have `title`, `content`, `version` and optional `timeout_seconds` and `expires_at` fields.
+Notices have `title`, `content`, `version` and optional `timeout_seconds`, `starts_at` and `expires_at` fields.
 
-Version can be any positive number; it defaults to incrementing the last version number.  Set the `expires_at` datetime to avoid showing this notice after the specified date, even if the user has never seen/dismissed it.
+Version can be any positive number; it defaults to incrementing the last version number.  Set the `expires_at` datetime to avoid showing this notice after the specified date, even if the user has never seen/dismissed it. Set the `starts_at` datetime to avoid showing the notice until a
+particular date/time.
+
+Note that only the notice with the latest version will be shown. If the latest version
+has not started yet, a previous version will not be shown, even if it hasn't expired. 
 
 Set the `timeout_seconds` to set a cookie timeout; this means the notice will be reshown.
 
 To show a new notice, add another Notice instance with an incremented version number.
 
 ### via django settings
```

### Comparing `django_one_time_notices-0.1.2/notices/context_processors.py` & `django_one_time_notices-0.1.3/notices/context_processors.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/example_project/example_app/templates/example_app/home.html` & `django_one_time_notices-0.1.3/notices/example_project/example_app/templates/example_app/home.html`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/example_project/example_project/settings.py` & `django_one_time_notices-0.1.3/notices/example_project/example_project/settings.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/example_project/example_project/urls.py` & `django_one_time_notices-0.1.3/notices/example_project/example_project/urls.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/example_project/manage.py` & `django_one_time_notices-0.1.3/notices/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/migrations/0001_initial.py` & `django_one_time_notices-0.1.3/notices/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/models.py` & `django_one_time_notices-0.1.3/notices/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,24 @@
 
 
 class Notice(models.Model):
 
     title = models.CharField(max_length=255, default="New!")
     content = models.TextField()
     version = models.PositiveIntegerField(blank=True, unique=True)
+    starts_at = models.DateTimeField(null=True, blank=True)
     expires_at = models.DateTimeField(null=True, blank=True)
     timeout_seconds = models.PositiveIntegerField(blank=True, null=True)
 
     def __str__(self):
+        starts_str = ""
+        if self.starts_at and not self.has_started():
+            starts_str = f"starts: {self.starts_at.strftime('%d-%b-%Y %H:%M UTC')} - "
         return (
-            f"v{self.version} - "
+            f"v{self.version} - {starts_str}"
             f"expires: {self.expires_at.strftime('%d-%b-%Y %H:%M UTC') if self.expires_at else 'never'}"
         )
 
     @classmethod
     def latest_notice(cls):
         return cls.objects.order_by("-version").first()
 
@@ -51,11 +55,16 @@
                 }
 
     def has_expired(self):
         if not self.expires_at:
             return False
         return self.expires_at < timezone.now()
 
+    def has_started(self):
+        if not self.starts_at:
+            return True
+        return self.starts_at < timezone.now()
+
     def save(self, *args, **kwargs):
         if not self.id and not self.version:
             self.version = Notice.latest_version() + 1
         super().save(*args, **kwargs)
```

### Comparing `django_one_time_notices-0.1.2/notices/static/notices/css/notices.css` & `django_one_time_notices-0.1.3/notices/static/notices/css/notices.css`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/static/notices/js/notices.js` & `django_one_time_notices-0.1.3/notices/static/notices/js/notices.js`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/templates/notices/notices.html` & `django_one_time_notices-0.1.3/notices/templates/notices/notices.html`

 * *Files identical despite different names*

### Comparing `django_one_time_notices-0.1.2/notices/templatetags/notices_tags.py` & `django_one_time_notices-0.1.3/notices/templatetags/notices_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             version = settings_config["notices_version"]
         else:
             version = Notice.latest_version()
             if version == 0:
                 return ""
 
             latest_notice = Notice.latest_notice()
-            if latest_notice.has_expired():
+            if latest_notice.has_expired() or not latest_notice.has_started():
                 return ""
 
         if version == 0:  # version 0 --> clear the cookie
             return render_to_string(
                 "notices/notices_clear.html", {}, getattr(context, "request", None)
             )
```

### Comparing `django_one_time_notices-0.1.2/pyproject.toml` & `django_one_time_notices-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-one-time-notices"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Becky Smith <rebkwok@gmail.com>"]
 readme = "README.md"
 packages = [{include = "notices"}]
 license = "MIT"
 
 [tool.poetry.dependencies]
@@ -18,14 +18,18 @@
 black = "^22.10.0"
 flake8 = "^5.0.4"
 isort = "^5.10.1"
 pytest-cov = "^4.0.0"
 flake8-pyproject = "^1.1.0.post0"
 pytest-env = "^0.6.2"
 
+
+[tool.poetry.group.test.dependencies]
+pytest-freezegun = "^0.4.2"
+
 [tool.flake8]
 extend-exclude = [".venv", "venv"]
 extend-select = "W504"  # match black&PEP8 putting binary operators after new lines
 ignore = [
     "E203",  # whitespace before : (black disagrees)
     "E501", # line too long (black fixes long lines, except for long strings which may benefit from being long (eg URLs))
     "W503",   # line break before binary operator (black disagrees)
```

### Comparing `django_one_time_notices-0.1.2/PKG-INFO` & `django_one_time_notices-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-one-time-notices
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Becky Smith
 Author-email: rebkwok@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -78,17 +78,21 @@
 The modal will be shown.  Once it has been dismissed it won't be shown again unless the notice version changes (see below), the `notice_seen` cookie is deleted, or the notice timeout is reached.
 
 ## Setting/updating the notice
 
 ### via models and django admin
 Add a `Notice` instance in the django admin. 
 
-Notices have `title`, `content`, `version` and optional `timeout_seconds` and `expires_at` fields.
+Notices have `title`, `content`, `version` and optional `timeout_seconds`, `starts_at` and `expires_at` fields.
 
-Version can be any positive number; it defaults to incrementing the last version number.  Set the `expires_at` datetime to avoid showing this notice after the specified date, even if the user has never seen/dismissed it.
+Version can be any positive number; it defaults to incrementing the last version number.  Set the `expires_at` datetime to avoid showing this notice after the specified date, even if the user has never seen/dismissed it. Set the `starts_at` datetime to avoid showing the notice until a
+particular date/time.
+
+Note that only the notice with the latest version will be shown. If the latest version
+has not started yet, a previous version will not be shown, even if it hasn't expired. 
 
 Set the `timeout_seconds` to set a cookie timeout; this means the notice will be reshown.
 
 To show a new notice, add another Notice instance with an incremented version number.
 
 ### via django settings
```

