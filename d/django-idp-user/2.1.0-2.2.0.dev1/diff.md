# Comparing `tmp/django_idp_user-2.1.0.tar.gz` & `tmp/django_idp_user-2.2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_idp_user-2.1.0.tar", last modified: Mon Jun  5 14:51:04 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django_idp_user-2.1.0.tar` & `django_idp_user-2.2.0.dev1.tar`

### file list

```diff
@@ -1,52 +1,42 @@
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/LICENSE
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       73 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/MANIFEST.in
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3604 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2507 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/README.rst
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/django_idp_user.egg-info/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3604 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/PKG-INFO
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1172 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/SOURCES.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/dependency_links.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       55 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/requires.txt
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        9 2023-06-05 14:51:04.000000 django_idp_user-2.1.0/django_idp_user.egg-info/top_level.txt
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       95 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1972 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/agents.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1024 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/apps.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/auth/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       66 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/auth/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3921 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/auth/authentication.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2345 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/checks.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/management/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/management/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.536938 django_idp_user-2.1.0/idp_user/management/commands/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/management/commands/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      823 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/management/commands/put_app_entities_records_to_kafka.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/migrations/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     4340 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0001_initial.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      378 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0002_auto_20220120_1617.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      390 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0003_auto_20220513_1025.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      579 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0004_auto_20220817_1526.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      446 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/0005_alter_userrole_id.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/migrations/__init__.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/models/
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       55 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/models/__init__.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       89 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/models/user.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)      713 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/models/user_role.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      959 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/producer.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      800 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/schema_extensions.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/services/
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       30 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/services/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17047 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/services/user.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      771 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/settings.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      132 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/signals.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2868 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/typing.py
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)       16 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/urls.py
-drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/idp_user/utils/
--rwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/__init__.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      600 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/choices.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      311 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/classes.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      435 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/idp_user/utils/exceptions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2312 2023-06-05 14:49:38.000000 django_idp_user-2.1.0/idp_user/utils/functions.py
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1141 2023-06-05 14:51:04.540938 django_idp_user-2.1.0/setup.cfg
--rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       69 2023-04-19 07:49:11.000000 django_idp_user-2.1.0/setup.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/requirements.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/__init__.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/agents.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/apps.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/checks.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/producer.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/schema_extensions.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/settings.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/signals.py
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/urls.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/auth/__init__.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/auth/admin_authentication.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/auth/async_authentication.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/auth/authentication.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/management/commands/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/management/commands/put_app_entities_records_to_kafka.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/migrations/0001_initial_squashed_0005_alter_userrole_id.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/migrations/0002_auto_20220120_1617.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/migrations/0003_auto_20220513_1025.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/migrations/0004_auto_20220817_1526.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/migrations/0005_alter_userrole_id.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/migrations/__init__.py
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/models/__init__.py
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/models/user.py
+-rwxr-xr-x   0        0        0      727 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/models/user_role.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/services/__init__.py
+-rw-r--r--   0        0        0    12964 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/services/async_user.py
+-rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/services/base_user.py
+-rw-r--r--   0        0        0    15390 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/services/user.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/utils/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/utils/choices.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/utils/classes.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/utils/exceptions.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/utils/functions.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/idp_user/utils/typing.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/.gitignore
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/LICENSE
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/README.md
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     7439 2020-02-02 00:00:00.000000 django_idp_user-2.2.0.dev1/PKG-INFO
```

### Comparing `django_idp_user-2.1.0/LICENSE` & `django_idp_user-2.2.0.dev1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2021 CardoAI
+Copyright 2023 CardoAI
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django_idp_user-2.1.0/PKG-INFO` & `django_idp_user-2.2.0.dev1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-Metadata-Version: 2.1
-Name: django_idp_user
-Version: 2.1.0
-Summary: A Django app that handles the communication between the IDP and the products for the authorization of users.
-Home-page: https://github.com/CardoAI/django-idp-user
-Author: Mahmoud Al-Rawy, Euron Metaliaj, Klajdi Çaushi, Aleksandër Nasto, Andi Çuku, Klement Omeri
-Author-email: hello@cardoai.com
-License: MIT (X11)
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.9
-License-File: LICENSE
-
-===============
-Django IDP User
-===============
+# Django IDP User
 
-Quick start
------------
+[![pypi-badge]][pypi]
+[![build-status-image]][build-status]
+[![package-status]][repo]
+[![github-last-commit]][repo]
 
-1. Add "idp_user" to your INSTALLED_APPS setting like this::
+---
 
+## Installation
+
+1. Install the package:
+    ```
+    pip install django-idp-user
+    ```
+
+    If you want to use the async version of the package, you can install it with the `async` extra:
+    ```
+    pip install django-idp-user[async]
+    ```
+
+2. Add `idp_user` to your `INSTALLED_APPS`:
+    ```python
     INSTALLED_APPS = [
-        ...
+        # ...
         'idp_user',
     ]
+    ```
 
-2. Add the settings of the app in settings.py like this::
-
-    APP_ENV = "development"/"staging"/"production"
+3. Add the settings of the app in `settings.py` like this:
+    ```python
+    APP_ENV = "development" or "staging" or "production"
 
     AUTH_USER_MODEL = 'idp_user.User'
 
     IDP_USER_APP = {
         "APP_IDENTIFIER": "str",
         "ROLES": "path.to.roles_choices",
         "FAUST_APP_PATH": "backend.kafka_consumer.app",
@@ -52,19 +42,19 @@
         "APP_ENTITIES": {
             "<entity_type>": {
                 "model": "<path.to.entity_type.model>",
                 "identifier_attr": "<field_name>",
                 "label_attr": "<field_name>",
             }
         },
-        "CONSUMER_APP_ENV": (Optional) "development"/"staging"/"production",
+        "CONSUMER_APP_ENV": "development" or "staging" or "production", # Optional
     }
 
     REST_FRAMEWORK = {
-        'DEFAULT_SCHEMA_CLASS': 'drf_spectacular.openapi.AutoSchema' / 'idp_user.schema_extensions.AutoSchemaWithRole',
+        'DEFAULT_SCHEMA_CLASS': 'drf_spectacular.openapi.AutoSchema' or 'idp_user.schema_extensions.AutoSchemaWithRole',
         'DEFAULT_AUTHENTICATION_CLASSES': (
             'idp_user.auth.AuthenticationBackend',
         ),
     }
 
     SPECTACULAR_SETTINGS = {
         'DEFAULT_AUTHENTICATION_CLASSES': (
@@ -74,44 +64,94 @@
     }
 
     # Kafka Related
     KAFKA_ARN = "<aws_kafka_arn>"  # Encoded in base64
     KAFKA_AWS_ACCESS_KEY_ID = "<access_key_id>"
     KAFKA_AWS_SECRET_ACCESS_KEY = "<secret_access_key_id>"  # Encoded in base64
     AWS_S3_REGION_NAME = "<region_name>"
+   ```
+
+4. Create the database tables for the app by running the following command:
+    ```
+    python manage.py migrate
+    ```
+
 
-3. Run ``python manage.py migrate`` to create the models.
+## Async Support
 
-Settings Reference
-------------------
+Django version 4.1.1 is required for async support.
+
+To use the async version of the package, you need to add the `async` extra when installing the package:
+```
+pip install django-idp-user[async]
+```
+
+If you are using Channels for websockets, you can use the `IDPChannelsAuthenticationMiddleware` like so:
+```python
+from channels.routing import ProtocolTypeRouter, URLRouter
+from idp_user.auth import IDPChannelsAuthenticationMiddleware
+
+application = ProtocolTypeRouter({
+    "websocket": IDPChannelsAuthenticationMiddleware(
+        AuthMiddlewareStack(
+            URLRouter(
+                # ...
+            )
+        )
+    ),
+})
+```
+
+
+## Settings Reference
 
 * ``APP_IDENTIFIER``
 
   * The app identifier, as defined in the IDP.
 
+
 * ``ROLES``
 
+
   * The path to the roles choices.
 
+
 * ``FAUST_APP_PATH``
 
+
   * The path to the Faust app.
 
+
 * ``IDP_URL``
 
+
   * The URL of the IDP, used for local development, or when using the IDP as an Authentication Backend.
 
+
 * ``USE_REDIS_CACHE``
 
+
   * If True, the cache will be used
   * When developing locally, you can leave this as ``False``.
 
+
 * ``APP_ENTITIES``
 
+
   * This dict links the AppEntityTypes declared on the IDP for this app to their actual models,
     so that they can be used for authorization purposes. In the value dicts, the attributes that will be
     used as the identifier and label are declared as well.
 
+
 * ``CONSUMER_APP_ENV``
 
   * The environment of the Faust Kafka Consumer app.
   * If not set, the value of ``APP_ENV`` will be used.
+
+
+[repo]: https://github.com/CardoAI/django-idp-user
+[package-status]: https://img.shields.io/badge/package--status-production-green
+[pypi]: https://pypi.org/project/django-idp-user/
+[pypi-badge]: https://img.shields.io/badge/version-2.2.0.dev1-blue
+[github-last-commit]: https://img.shields.io/github/last-commit/CardoAI/django-idp-user
+[build-status-image]: https://github.com/CardoAI/django-idp-user/actions/workflows/workflow.yml/badge.svg
+[build-status]: https://github.com/CardoAI/django-idp-user/actions/workflows/workflow.yml
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `django_idp_user-2.1.0/idp_user/agents.py` & `django_idp_user-2.2.0.dev1/idp_user/agents.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import faust
 from asgiref.sync import sync_to_async
 from django.conf import settings
 from django.utils.module_loading import import_string
 from faust import StreamT
 
-from .services import UserService
-from .settings import CONSUMER_APP_ENV
+from idp_user.services import UserService
+from idp_user.settings import CONSUMER_APP_ENV
 
-app = import_string(settings.IDP_USER_APP['FAUST_APP_PATH'])
+app = import_string(settings.IDP_USER_APP["FAUST_APP_PATH"])
 
 """
 {
     "username": "",
     "first_name": "",
     "last_name": "",
     "email": "",
@@ -44,27 +44,29 @@
 
 
 USER_UPDATES_TOPIC_NAME = f"{CONSUMER_APP_ENV}_user_updates"
 
 user_updates = app.topic(USER_UPDATES_TOPIC_NAME, value_type=UserRecord)
 
 
-@sync_to_async
-def update_user(user_record: UserRecord):
-    UserService.process_user(user_record.asdict())
+async def update_user(user_record: UserRecord):
+    await sync_to_async(UserService.process_user)(user_record.asdict())
 
 
-@sync_to_async
-def verify_if_user_exists_and_delete_roles(user_record: UserRecord):
-    UserService.verify_if_user_exists_and_delete_roles(user_record.asdict())
+async def verify_if_user_exists_and_delete_roles(user_record: UserRecord):
+    await sync_to_async(UserService.verify_if_user_exists_and_delete_roles)(
+        user_record.asdict()
+    )
 
 
 @app.agent(user_updates)
 async def update_user_stream_processor(user_records: StreamT[UserRecord]):
     async for user_record in user_records:
-        if user_record.app_specific_configs.get(settings.IDP_USER_APP['APP_IDENTIFIER']):
+        if user_record.app_specific_configs.get(
+            settings.IDP_USER_APP["APP_IDENTIFIER"]
+        ):
             await update_user(user_record)
         else:
             # Having arrived here means that the user does not have access in the current app
             # Verify however if the user already exists in the database of any tenant
             # If this is the case, delete his/her roles
             await verify_if_user_exists_and_delete_roles(user_record)
```

### Comparing `django_idp_user-2.1.0/idp_user/apps.py` & `django_idp_user-2.2.0.dev1/idp_user/apps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from django.apps import AppConfig
 from django.conf import settings
-from django.db.models.signals import post_save, post_delete
+
+
+from django.db.models.signals import post_delete, post_save
 
 
 class IDPUserConfig(AppConfig):
     name = "idp_user"
 
     def ready(self):
         # If Kafka is not configured, do not register signals
-        is_kafka_configured = getattr(settings, "KAFKA_ARN", None) or getattr(settings, "KAFKA_BROKER", None)
+        is_kafka_configured = getattr(settings, "KAFKA_ARN", None) or getattr(
+            settings, "KAFKA_BROKER", None
+        )
         if not is_kafka_configured:
             return
 
-        from idp_user.services import UserService
+        from idp_user.services.base_user import BaseUserService
         from idp_user.settings import APP_ENTITIES
-        from idp_user.typing import AppEntityTypeConfig
 
-        for app_entity_type, config in APP_ENTITIES.items():  # type: str, AppEntityTypeConfig
-            model = config['model']
+        for (
+            _app_entity_type,
+            config,
+        ) in APP_ENTITIES.items():
+            model = config["model"]
             post_save.connect(
-                receiver=UserService.process_app_entity_record_post_save,
+                receiver=BaseUserService.process_app_entity_record_post_save,
                 sender=model,
             )
             post_delete.connect(
-                receiver=UserService.process_app_entity_record_post_delete,
+                receiver=BaseUserService.process_app_entity_record_post_delete,
                 sender=model,
             )
```

### Comparing `django_idp_user-2.1.0/idp_user/checks.py` & `django_idp_user-2.2.0.dev1/idp_user/checks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 from django.conf import settings
-from django.core.checks import Warning, Error, register
+from django.core.checks import Error, Warning, register
 
 
 @register()
 def check_idp_user_settings(*args, **kwargs):
     def verify_idp_user_app_attr_exists(_attr, error=False):
         if _attr not in idp_user_settings:
             issue_kwargs = {
-                'msg': f'Missing {_attr} in IDP_USER_APP.',
-                'hint': f'You must declare the attribute {_attr} in the dict IDP_USER_APP in settings.py.',
-                'obj': settings,
-                'id': f'idp_user.{_attr}',
+                "msg": f"Missing {_attr} in IDP_USER_APP.",
+                "hint": f"You must declare the attribute {_attr} in the dict IDP_USER_APP in settings.py.",
+                "obj": settings,
+                "id": f"idp_user.{_attr}",
             }
             if error:
                 issues.append(Error(**issue_kwargs))
             else:
                 issues.append(Warning(**issue_kwargs))
 
     issues = []
 
     try:
-        settings.APP_ENV
+        if hasattr(settings, "APP_ENV") and settings.APP_ENV not in [
+            "development",
+            "staging",
+            "production",
+        ]:
+            issues.append(
+                Error(
+                    "Wrong APP_ENV.",
+                    hint="You must declare the APP_ENV (development/staging/production) variable in settings.py.",
+                    obj=settings,
+                    id="idp_user.E000",
+                )
+            )
     except AttributeError:
         issues.append(
             Error(
-                'Missing APP_ENV.',
-                hint='You must declare the APP_ENV (development/staging/production) variable in settings.py.',
+                "Missing APP_ENV.",
+                hint="You must declare the APP_ENV (development/staging/production) variable in settings.py.",
                 obj=settings,
-                id='idp_user.E001',
+                id="idp_user.E001",
             )
         )
 
     try:
         auth_user_model = settings.AUTH_USER_MODEL
-        if auth_user_model != 'idp_user.User':
+        if auth_user_model != "idp_user.User":
             issues.append(
                 Warning(
-                    'Wrong AUTH_USER_MODEL.',
+                    "Wrong AUTH_USER_MODEL.",
                     hint="You must set AUTH_USER_MODEL = 'idp_user.User' in settings.py.",
                     obj=settings,
-                    id='idp_user.E002',
+                    id="idp_user.E002",
                 )
             )
 
     except AttributeError:
         issues.append(
             Warning(
-                'Missing AUTH_USER_MODEL',
+                "Missing AUTH_USER_MODEL",
                 hint="You must set AUTH_USER_MODEL = 'idp_user.user' in settings.py.",
                 obj=settings,
-                id='idp_user.E003',
+                id="idp_user.E003",
             )
         )
 
     try:
         idp_user_settings = settings.IDP_USER_APP
 
         for attr in ["APP_IDENTIFIER", "FAUST_APP_PATH"]:
@@ -61,15 +73,15 @@
 
         for attr in ["ROLES"]:
             verify_idp_user_app_attr_exists(attr, error=False)
 
     except AttributeError:
         issues.append(
             Error(
-                'Missing IDP_USER_APP.',
-                hint='You must declare the idp_user settings in the variable IDP_USER_APP in settings.py.',
+                "Missing IDP_USER_APP.",
+                hint="You must declare the idp_user settings in the variable IDP_USER_APP in settings.py.",
                 obj=settings,
-                id='idp_user.E004',
+                id="idp_user.E004",
             )
         )
 
     return issues
```

### Comparing `django_idp_user-2.1.0/idp_user/migrations/0001_initial.py` & `django_idp_user-2.2.0.dev1/idp_user/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.1.0/idp_user/migrations/0004_auto_20220817_1526.py` & `django_idp_user-2.2.0.dev1/idp_user/migrations/0004_auto_20220817_1526.py`

 * *Files identical despite different names*

### Comparing `django_idp_user-2.1.0/idp_user/models/user_role.py` & `django_idp_user-2.2.0.dev1/idp_user/models/user_role.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from django.db import models
 
 
 class UserRole(models.Model):
-    user = models.ForeignKey(to="idp_user.User", related_name="user_roles", on_delete=models.CASCADE)
+    user = models.ForeignKey(
+        to="idp_user.User", related_name="user_roles", on_delete=models.CASCADE
+    )
     role = models.CharField(max_length=140)
     # This dictionary contains explicit restrictions about the app entities that the user can access, in the form:
     # {<entity_type>: [1, 2]}
     app_entities_restrictions = models.JSONField(null=True)
     # This dictionary contains explicit restrictions regarding app permissions, in the form:
     # {"perform_operation_1": {<entity_type>: [1, 2]}, "perform_operation_2": false}
     permission_restrictions = models.JSONField(default=dict)
 
     class Meta:
-        unique_together = [('user', 'role')]
+        unique_together = [("user", "role")]
```

### Comparing `django_idp_user-2.1.0/idp_user/schema_extensions.py` & `django_idp_user-2.2.0.dev1/idp_user/schema_extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from drf_spectacular.utils import OpenApiParameter
 
 from idp_user.auth.authentication import AuthenticationBackend
 
 
 class BearerTokenScheme(OpenApiAuthenticationExtension):
     target_class = AuthenticationBackend  # full import path OR class ref
-    name = 'IDPAuthentication'  # name used in the schema
+    name = "IDPAuthentication"  # name used in the schema
 
     def get_security_definition(self, auto_schema):
         return {
             "type": "http",
             "scheme": "bearer",
             "bearerFormat": "JWT",
         }
 
 
 class AutoSchemaWithRole(AutoSchema):
     def get_override_parameters(self):
         return [
-            OpenApiParameter("role", type=str, location=OpenApiParameter.QUERY, required=True),
+            OpenApiParameter(
+                "role", type=str, location=OpenApiParameter.QUERY, required=True
+            ),
         ]
```

### Comparing `django_idp_user-2.1.0/idp_user/services/user.py` & `django_idp_user-2.2.0.dev1/idp_user/services/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 import logging
 from collections import defaultdict
 from copy import deepcopy
-from datetime import datetime
-from typing import Any, Optional, Union, Type
+from typing import Any, Optional, Union
 
 from django.conf import settings
 from django.core.cache import cache
-from django.db import transaction, models
+from django.db import models, transaction
 from django.db.models import Q, QuerySet
 from rest_framework.exceptions import PermissionDenied
 from rest_framework.request import Request
 
-from ..models import User
-from ..models.user_role import UserRole
-from ..producer import Producer
-from ..settings import ROLES, APP_ENTITIES, IN_DEV, APP_IDENTIFIER, APP_ENTITY_RECORD_EVENT_TOPIC, TENANTS
-from ..signals import pre_update_idp_user, post_update_idp_user, post_create_idp_user
-from ..typing import UserTenantData, UserRecordDict, ALL, AppEntityTypeConfig, AppEntityRecordEventDict
-from ..utils.exceptions import UnsupportedAppEntityType
-from ..utils.functions import get_or_none, keep_keys, update_record, cache_user_service_results
+from idp_user.models import UserRole
+from idp_user.models.user import User
+from idp_user.services.base_user import BaseUserService
+from idp_user.settings import APP_ENTITIES, APP_IDENTIFIER, IN_DEV, ROLES, TENANTS
+from idp_user.signals import (
+    post_create_idp_user,
+    post_update_idp_user,
+    pre_update_idp_user,
+)
+from idp_user.utils.functions import (
+    cache_user_service_results,
+    get_or_none,
+    keep_keys,
+    update_record,
+)
+from idp_user.utils.typing import (
+    ALL,
+    AppEntityTypeConfig,
+    UserRecordDict,
+    UserTenantData,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class UserService:
-
+class UserService(BaseUserService):
     # Service Methods Used by Django Application
     @staticmethod
     def get_role(request: Request):
-        return request.query_params.get('role')
+        return request.query_params.get("role")
 
     @staticmethod
     def authorize_and_get_records_or_get_all_allowed(
-            user: User,
-            role: ROLES,
-            app_entity_type: str,
-            app_entity_records_identifiers: Optional[list[Any]],
-            permission: str = None
+        user: User,
+        role: ROLES,
+        app_entity_type: str,
+        app_entity_records_identifiers: Optional[list[Any]],
+        permission: str = None,
     ) -> models.QuerySet:
         """
         Make sure that the user can access the entity records being requested and return them.
         If no identifiers are being provided, return all allowed entity records.
 
         Args:
             user:                           The user performing the request
@@ -51,41 +62,40 @@
                                                 through IDP. The value is the name of the permission
 
 
         Raises:
             PermissionDenied: In case the requested records are not allowed
         """
 
-        if app_entity_records_identifiers:
-            UserService.authorize_app_entity_records(
-                user=user,
-                role=role,
-                app_entity_type=app_entity_type,
-                app_entity_records_identifiers=app_entity_records_identifiers,
-                permission=permission
-            )
-            return UserService._get_records(
-                app_entity_type=app_entity_type,
-                records_identifiers=app_entity_records_identifiers
-            )
-        else:
+        if not app_entity_records_identifiers:
             return UserService.get_allowed_app_entity_records(
                 user=user,
                 role=role,
                 app_entity_type=app_entity_type,
-                permission=permission
+                permission=permission,
             )
+        UserService.authorize_app_entity_records(
+            user=user,
+            role=role,
+            app_entity_type=app_entity_type,
+            app_entity_records_identifiers=app_entity_records_identifiers,
+            permission=permission,
+        )
+        return UserService._get_records(
+            app_entity_type=app_entity_type,
+            records_identifiers=app_entity_records_identifiers,
+        )
 
     @staticmethod
     def authorize_app_entity_records(
-            user: User,
-            role: ROLES,
-            app_entity_type: str,
-            app_entity_records_identifiers: list[Any],
-            permission: str = None,
+        user: User,
+        role: ROLES,
+        app_entity_type: str,
+        app_entity_records_identifiers: list[Any],
+        permission: str = None,
     ):
         """
         Verify if the user has access to the requested entity records.
         If a permission is specified and it has restrictable=True, the access is verified based on it.
 
         Args:
             user:                           The user performing the request
@@ -95,35 +105,40 @@
             permission:                     In case of specific permissions we can have permission restrictions
                                                 through IDP. The value is the name of the permission
 
         Raises:
             PermissionDenied: In case the requested records are not allowed
         """
 
-        assert app_entity_type in APP_ENTITIES.keys(), f"Unknown app entity: {app_entity_type}!"
+        assert (
+            app_entity_type in APP_ENTITIES.keys()
+        ), f"Unknown app entity: {app_entity_type}!"
 
-        allowed_app_entity_records_identifiers = UserService._get_allowed_app_entity_records_identifiers(
-            user=user,
-            role=role,
-            app_entity_type=app_entity_type,
-            permission=permission
+        allowed_app_entity_records_identifiers = (
+            UserService._get_allowed_app_entity_records_identifiers(
+                user=user,
+                role=role,
+                app_entity_type=app_entity_type,
+                permission=permission,
+            )
         )
 
         if allowed_app_entity_records_identifiers == ALL:
             return
 
-        if not set(app_entity_records_identifiers).issubset(set(allowed_app_entity_records_identifiers)):
-            raise PermissionDenied('You are not allowed to access the records in the requested entity!')
+        if not set(app_entity_records_identifiers).issubset(
+            set(allowed_app_entity_records_identifiers)
+        ):
+            raise PermissionDenied(
+                "You are not allowed to access the records in the requested entity!"
+            )
 
     @staticmethod
     def get_allowed_app_entity_records(
-            user: User,
-            role: ROLES,
-            app_entity_type: str,
-            permission: str = None
+        user: User, role: ROLES, app_entity_type: str, permission: str = None
     ) -> models.QuerySet:
         """
         Gets the app entity records that the user can access.
 
         Args:
             user:               The user performing the request
             role:               The role that the user is acting as.
@@ -131,59 +146,63 @@
             permission:         In case of specific permissions we can have permission restrictions
                                     through IDP. The value is the name of the permission
 
         Returns:
             QuerySet of App Entity Records that the user can access
         """
 
-        assert app_entity_type in APP_ENTITIES.keys(), f"Unknown app entity: {app_entity_type}!"
+        assert (
+            app_entity_type in APP_ENTITIES.keys()
+        ), f"Unknown app entity: {app_entity_type}!"
 
-        allowed_app_entity_records_identifiers = UserService._get_allowed_app_entity_records_identifiers(
-            user=user,
-            role=role,
-            app_entity_type=app_entity_type,
-            permission=permission
+        allowed_app_entity_records_identifiers = (
+            UserService._get_allowed_app_entity_records_identifiers(
+                user=user,
+                role=role,
+                app_entity_type=app_entity_type,
+                permission=permission,
+            )
         )
 
         return UserService._get_records(
             app_entity_type=app_entity_type,
-            records_identifiers=allowed_app_entity_records_identifiers
+            records_identifiers=allowed_app_entity_records_identifiers,
         )
 
     @staticmethod
     def _get_app_entity_type_configs(app_entity_type: str) -> AppEntityTypeConfig:
         try:
             return APP_ENTITIES[app_entity_type]
         except KeyError:
             raise KeyError(
                 f"No config declared for app_entity_type={app_entity_type} "
                 f"in IDP_USER_APP['APP_ENTITIES']!"
-            )
+            ) from None
 
     @staticmethod
     def _get_records(
-            app_entity_type: str,
-            records_identifiers: Union[list[Any], ALL]
+        app_entity_type: str, records_identifiers: Union[list[Any], ALL]
     ) -> models.QuerySet:
-        app_entity_type_configs = UserService._get_app_entity_type_configs(app_entity_type)
-        model = app_entity_type_configs['model']
+        app_entity_type_configs = UserService._get_app_entity_type_configs(
+            app_entity_type
+        )
+        model = app_entity_type_configs["model"]
 
         if records_identifiers == ALL:
             return model.objects.all()
         else:
-            model_identifier_attr = app_entity_type_configs['identifier_attr']
-            return model.objects.filter(**{f"{model_identifier_attr}__in": records_identifiers})
+            model_identifier_attr = app_entity_type_configs["identifier_attr"]
+            return model.objects.filter(
+                **{f"{model_identifier_attr}__in": records_identifiers}
+            )
 
     @staticmethod
     @cache_user_service_results
     def _get_allowed_app_entity_records_identifiers(
-            user: User,
-            role: ROLES,
-            app_entity_type: str,
-            permission: str = None
+        user: User, role: ROLES, app_entity_type: str, permission: str = None
     ) -> Union[list[Any], ALL]:
         """
         Gets the identifiers of the app entity records that the user can access.
         If no restriction both on role and permission level, return '__all__'
 
         Args:
             user:               The user performing the request
@@ -203,39 +222,44 @@
             return []
 
         # Permission restriction get precedence, if existing, for the given app_entity
         if permission:
             permission_restrictions = user_role.permission_restrictions
             if permission_restrictions and permission in permission_restrictions.keys():
                 permission_restriction = permission_restrictions.get(permission)
-                if permission_app_entity_restriction := permission_restriction.get(app_entity_type):
+                if permission_app_entity_restriction := permission_restriction.get(
+                    app_entity_type
+                ):
                     return permission_app_entity_restriction
 
         # Verify if there is any restriction on the entity for the user
         app_entities_restrictions = user_role.app_entities_restrictions
         if app_entities_restrictions and (
-                app_entity_restriction := app_entities_restrictions.get(app_entity_type)
+            app_entity_restriction := app_entities_restrictions.get(app_entity_type)
         ):
             return app_entity_restriction
 
         return ALL
 
     @staticmethod
     def _create_or_update_user(data: UserTenantData) -> User:
         user = get_or_none(User.objects, username=data.get("username"))
-        user_data = keep_keys(data, [
-            "username",
-            "email",
-            "first_name",
-            "last_name",
-            "is_active",
-            "is_staff",
-            "is_superuser",
-            "date_joined",
-        ])
+        user_data = keep_keys(
+            data,
+            [
+                "username",
+                "email",
+                "first_name",
+                "last_name",
+                "is_active",
+                "is_staff",
+                "is_superuser",
+                "date_joined",
+            ],
+        )
         if user:
             update_record(user, **user_data)
             UserService._invalidate_user_cache_entries(user=user)
             return user
         else:
             user = User.objects.create(**user_data)
             post_create_idp_user.send(sender=UserService, user=user)
@@ -244,15 +268,15 @@
 
     @staticmethod
     def _invalidate_user_cache_entries(user: User):
         """
         Invalidate all the entries in the cache for the given user.
         To do this, find all the entries that start with the app identifier and username of the user.
         """
-        if settings.IDP_USER_APP.get('USE_REDIS_CACHE', False) and not IN_DEV:
+        if settings.IDP_USER_APP.get("USE_REDIS_CACHE", False) and not IN_DEV:
             cache.delete_pattern(f"{APP_IDENTIFIER}-{user.username}*")
 
     @classmethod
     def process_user(cls, data: UserRecordDict):
         """
         Extract tenants from the user record and call _update_user for each tenant.
         Remove tenant information from the payload of _update_user since it is not needed
@@ -274,15 +298,17 @@
                 continue
 
             logger.info(f"Updating user {data['username']} for tenant {tenant}")
             pre_update_idp_user.send(sender=cls.__class__, tenant=tenant)
 
             # Extract specific tenant information
             user_record_for_tenant = deepcopy(data)
-            user_record_for_tenant['app_specific_configs'] = reported_user_app_configs[tenant]
+            user_record_for_tenant["app_specific_configs"] = reported_user_app_configs[
+                tenant
+            ]
 
             try:
                 with transaction.atomic(using=tenant):
                     UserService._update_user(user_record_for_tenant)  # type: ignore
             finally:
                 post_update_idp_user.send(sender=cls.__class__, tenant=tenant)
 
@@ -290,16 +316,18 @@
     def verify_if_user_exists_and_delete_roles(cls, data: UserRecordDict):
         """
         Verify if the user exists in any of the tenants and delete all the roles associated with it.
         """
         for tenant in TENANTS:
             pre_update_idp_user.send(sender=cls.__class__, tenant=tenant)
 
-            if user := get_or_none(User.objects, username=data['username']):
-                logger.info(f"Deleting roles for user {data['username']} in tenant {tenant}")
+            if user := get_or_none(User.objects, username=data["username"]):
+                logger.info(
+                    f"Deleting roles for user {data['username']} in tenant {tenant}"
+                )
                 UserRole.objects.filter(user=user).delete()  # type: ignore
 
             post_update_idp_user.send(sender=cls.__class__, tenant=tenant)
 
     @staticmethod
     def _update_user(data: UserTenantData):
         """
@@ -312,114 +340,67 @@
 
         user = UserService._create_or_update_user(data)
 
         current_user_roles = defaultdict()
         for user_role in user.user_roles.all():
             current_user_roles[user_role.role] = user_role
 
-        roles_data = data.get('app_specific_configs')
+        roles_data = data.get("app_specific_configs")
 
         for role, role_data in roles_data.items():
             if existing_user_role := current_user_roles.get(role):
                 update_record(
                     existing_user_role,
-                    permission_restrictions=role_data.get('permission_restrictions'),
-                    app_entities_restrictions=role_data.get("app_entities_restrictions")
+                    permission_restrictions=role_data.get("permission_restrictions"),
+                    app_entities_restrictions=role_data.get(
+                        "app_entities_restrictions"
+                    ),
                 )
             else:
                 UserRole.objects.create(
                     user=user,
                     role=role,
-                    permission_restrictions=role_data.get('permission_restrictions'),
-                    app_entities_restrictions=role_data.get("app_entities_restrictions")
+                    permission_restrictions=role_data.get("permission_restrictions"),
+                    app_entities_restrictions=role_data.get(
+                        "app_entities_restrictions"
+                    ),
                 )
 
         # Verify if any of the previous user roles is not being reported anymore
         # Delete it if this is the case
         for role, user_role in current_user_roles.items():  # type: str, UserRole
             if roles_data.get(role) is None:
                 user_role.delete()
 
     @staticmethod
     def _get_reported_user_app_configs(data):
-        return data.get('app_specific_configs', {}).get(APP_IDENTIFIER, {})
-
-    @staticmethod
-    def send_app_entity_record_event_to_kafka(app_entity_type: str, app_entity_record: Any, deleted=False):
-        app_entity_type_config = APP_ENTITIES[app_entity_type]
-
-        event: AppEntityRecordEventDict = {
-            'app_identifier': APP_IDENTIFIER,
-            'app_entity_type': app_entity_type,
-            'record_identifier': getattr(app_entity_record, app_entity_type_config['identifier_attr']),
-            'label': getattr(app_entity_record, app_entity_type_config['label_attr']),
-            'deleted': deleted
-        }
-
-        logger.info(f"Sending update {event}...")
-
-        Producer().send_message(
-            topic=APP_ENTITY_RECORD_EVENT_TOPIC,
-            key=str(datetime.now()),
-            data=event
-        )
-
-    @staticmethod
-    def _get_app_entity_type_from_model(model: Type[models.Model]):
-        for app_entity_type, config in APP_ENTITIES.items():  # type: str, AppEntityTypeConfig
-            if config['model'] == model:
-                return app_entity_type
-
-        raise UnsupportedAppEntityType(model)
-
-    @staticmethod
-    def process_app_entity_record_post_save(sender: Type[models.Model], instance, **kwargs):
-        """
-        Whenever an app entity record is saved (created/updated),
-        send a message to Kafka to notify the IDP.
-
-        kwargs are required for signal receivers.
-        """
-
-        UserService.send_app_entity_record_event_to_kafka(
-            app_entity_type=UserService._get_app_entity_type_from_model(sender),
-            app_entity_record=instance
-        )
-
-    @staticmethod
-    def process_app_entity_record_post_delete(sender: Type[models.Model], instance, **kwargs):
-        """
-        Whenever an app entity record is deleted,
-        send a message to Kafka to notify the IDP.
-
-        kwargs are required for signal receivers.
-        """
-
-        UserService.send_app_entity_record_event_to_kafka(
-            app_entity_type=UserService._get_app_entity_type_from_model(sender),
-            app_entity_record=instance,
-            deleted=True
-        )
+        return data.get("app_specific_configs", {}).get(APP_IDENTIFIER, {})
 
     @staticmethod
     def get_users_with_access_to_app_entity_record(
-            app_entity_type: str,
-            record_identifier: Any,
-            roles: list[str]
+        app_entity_type: str, record_identifier: Any, roles: list[str]
     ) -> QuerySet:
         """
         Get users that have access to the required app entity record in the given roles.
         """
 
-        assert app_entity_type in APP_ENTITIES.keys(), f"Unknown app entity: {app_entity_type}!"
+        assert (
+            app_entity_type in APP_ENTITIES.keys()
+        ), f"Unknown app entity: {app_entity_type}!"
 
         roles = UserRole.objects.filter(
-            Q(user__is_active=True) &
-            Q(role__in=roles) &
-            (
-                    Q(app_entities_restrictions__isnull=True) |
-                    Q(**{f"app_entities_restrictions__{app_entity_type}__isnull": True}) |
-                    Q(**{f"app_entities_restrictions__{app_entity_type}__contains": record_identifier})
+            Q(user__is_active=True)
+            & Q(role__in=roles)
+            & (
+                Q(app_entities_restrictions__isnull=True)
+                | Q(**{f"app_entities_restrictions__{app_entity_type}__isnull": True})
+                | Q(
+                    **{
+                        f"app_entities_restrictions__{app_entity_type}__contains": record_identifier
+                    }
+                )
             )
         )
 
-        return User.objects.filter(pk__in=list(roles.values_list('user__pk', flat=True)))
+        return User.objects.filter(
+            pk__in=list(roles.values_list("user__pk", flat=True))
+        )
```

### Comparing `django_idp_user-2.1.0/idp_user/settings.py` & `django_idp_user-2.2.0.dev1/idp_user/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from django.conf import settings
 from django.utils.module_loading import import_string
 
-CONSUMER_APP_ENV = settings.IDP_USER_APP.get('CONSUMER_APP_ENV') or settings.APP_ENV
-APP_IDENTIFIER = settings.IDP_USER_APP['APP_IDENTIFIER']
+ASYNC_MODE = settings.IDP_USER_APP.get("ASYNC_MODE", False)
+APP_IDENTIFIER = settings.IDP_USER_APP["APP_IDENTIFIER"]
 IN_DEV = settings.APP_ENV == "development"
-ROLES = import_string(settings.IDP_USER_APP.get('ROLES'))
-APP_ENTITIES = settings.IDP_USER_APP.get('APP_ENTITIES') or {}
+ROLES = import_string(settings.IDP_USER_APP.get("ROLES"))
+APP_ENTITIES = settings.IDP_USER_APP.get("APP_ENTITIES") or {}
 TENANTS = settings.IDP_USER_APP.get("TENANTS") or list(settings.DATABASES.keys())
+CONSUMER_APP_ENV = settings.IDP_USER_APP.get("CONSUMER_APP_ENV") or settings.APP_ENV
 
 if APP_ENTITIES:
-    for app_entity_type, config_dict in APP_ENTITIES.items():
-        config_dict['model'] = import_string(config_dict['model'])
+    for _, config_dict in APP_ENTITIES.items():
+        config_dict["model"] = import_string(config_dict["model"])
 
 
-APP_ENTITY_RECORD_EVENT_TOPIC = f"app_entity_record_events"
+APP_ENTITY_RECORD_EVENT_TOPIC = f"{CONSUMER_APP_ENV}_app_entity_record_events"
 
-AWS_S3_REGION_NAME = getattr(settings, 'AWS_S3_REGION_NAME', None) or 'eu-central-1'
+AWS_S3_REGION_NAME = getattr(settings, "AWS_S3_REGION_NAME", None) or "eu-central-1"
```

### Comparing `django_idp_user-2.1.0/idp_user/typing.py` & `django_idp_user-2.2.0.dev1/idp_user/utils/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import TypedDict, Union, List, Any, Optional, Type
+from typing import Any, List, Optional, Type, TypedDict, Union
 
 from django.db import models
 
-ALL = 'all'
+ALL = "all"
 
 
 class JwtData(TypedDict):
     iat: int
     nbf: int
     jti: str
     exp: str
@@ -70,15 +70,17 @@
 ]
 """
 
 # ===
 AppIdentifier = str
 TenantIdentifier = str
 
-UserRecordAppSpecificConfigs = dict[AppIdentifier, dict[TenantIdentifier, AppSpecificConfigs]]
+UserRecordAppSpecificConfigs = dict[
+    AppIdentifier, dict[TenantIdentifier, AppSpecificConfigs]
+]
 
 
 class UserRecordDict(TypedDict):
     first_name: str
     last_name: str
     username: str
     email: str
```

### Comparing `django_idp_user-2.1.0/idp_user/utils/functions.py` & `django_idp_user-2.2.0.dev1/idp_user/utils/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import base64
 import json
+from urllib.parse import parse_qs
 
 import boto3
 from django.conf import settings
 from django.core.cache import cache
 from django.core.exceptions import ObjectDoesNotExist
 
-from idp_user.settings import APP_IDENTIFIER, IN_DEV, AWS_S3_REGION_NAME
+from idp_user.settings import APP_IDENTIFIER, AWS_S3_REGION_NAME, IN_DEV
 
 
 def keep_keys(dictionary, keys):
     return {k: v for k, v in dictionary.items() if k in keys}
 
 
 def get_or_none(records, *args, **kwargs):
@@ -36,39 +37,59 @@
             cache_key += f",{arg}"
         for key, value in kwargs.items():
             cache_key += f",{key}={value}"
 
         result = cache.get(cache_key)
         if result:
             return json.loads(result)
-        else:
-            result = function(user=user, *args, **kwargs)
-            cache.set(cache_key, json.dumps(result))
-            return result
+        result = function(user=user, *args, **kwargs)  # noqa
+        cache.set(cache_key, json.dumps(result))
+        return result
 
-    if IN_DEV or not settings.IDP_USER_APP.get('USE_REDIS_CACHE', False):
+    if IN_DEV or not settings.IDP_USER_APP.get("USE_REDIS_CACHE", False):
         return function
 
     return wrapper
 
 
 def get_kafka_bootstrap_servers(include_uri_scheme=True):
     """
     If ARN is available, it means we can connect to the production servers.
     We have to find the bootstrap servers and create the connection using them.
     """
     if kafka_arn := settings.KAFKA_ARN:
-        resource = boto3.client("kafka", region_name=AWS_S3_REGION_NAME)
+        session = boto3.Session(
+            aws_access_key_id=settings.KAFKA_AWS_ACCESS_KEY_ID,
+            aws_secret_access_key=base64.b64decode(
+                settings.KAFKA_AWS_SECRET_ACCESS_KEY
+            ).decode("utf-8"),
+        )
+        resource = session.client("kafka", region_name=AWS_S3_REGION_NAME)
         response = resource.get_bootstrap_brokers(
             ClusterArn=base64.b64decode(kafka_arn).decode("utf-8")
         )
         assert (
-                "BootstrapBrokerString" in response.keys()
+            "BootstrapBrokerString" in response.keys()
         ), "Something went wrong while receiving kafka servers!"
 
         bootstrap_servers = response.get("BootstrapBrokerString").split(",")
-        if not include_uri_scheme:
-            return bootstrap_servers
-        return [f"kafka://{host}" for host in bootstrap_servers]
+        return (
+            [f"kafka://{host}" for host in bootstrap_servers]
+            if include_uri_scheme
+            else bootstrap_servers
+        )
     else:
         kafka_url = settings.KAFKA_BROKER
         return f"kafka://{kafka_url}" if include_uri_scheme else kafka_url
+
+
+def parse_query_params_from_scope(scope):
+    """
+    Parse query params from scope
+
+    Parameters:
+        scope (dict): scope from consumer
+
+    Returns:
+        dict: query params
+    """
+    return parse_qs(scope["query_string"].decode("utf-8"))
```

