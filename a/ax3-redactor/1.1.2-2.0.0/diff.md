# Comparing `tmp/ax3-redactor-1.1.2.tar.gz` & `tmp/ax3-redactor-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ax3-redactor-1.1.2.tar", last modified: Wed Jun  1 17:15:58 2022, max compression
+gzip compressed data, was "ax3-redactor-2.0.0.tar", last modified: Wed Jul  5 23:32:49 2023, max compression
```

## Comparing `ax3-redactor-1.1.2.tar` & `ax3-redactor-2.0.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-06-01 17:15:58.419121 ax3-redactor-1.1.2/
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      109 2022-03-23 00:51:32.000000 ax3-redactor-1.1.2/MANIFEST.in
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     2510 2022-06-01 17:15:58.419121 ax3-redactor-1.1.2/PKG-INFO
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     1181 2022-03-23 00:51:32.000000 ax3-redactor-1.1.2/README.md
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-06-01 17:15:58.415121 ax3-redactor-1.1.2/ax3_redactor.egg-info/
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     2510 2022-06-01 17:15:58.000000 ax3-redactor-1.1.2/ax3_redactor.egg-info/PKG-INFO
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      493 2022-06-01 17:15:58.000000 ax3-redactor-1.1.2/ax3_redactor.egg-info/SOURCES.txt
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)        1 2022-06-01 17:15:58.000000 ax3-redactor-1.1.2/ax3_redactor.egg-info/dependency_links.txt
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)        1 2022-03-23 00:53:40.000000 ax3-redactor-1.1.2/ax3_redactor.egg-info/not-zip-safe
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)       24 2022-06-01 17:15:58.000000 ax3-redactor-1.1.2/ax3_redactor.egg-info/requires.txt
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)        9 2022-06-01 17:15:58.000000 ax3-redactor-1.1.2/ax3_redactor.egg-info/top_level.txt
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-06-01 17:15:58.419121 ax3-redactor-1.1.2/redactor/
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)        0 2022-03-23 00:51:32.000000 ax3-redactor-1.1.2/redactor/__init__.py
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-06-01 17:15:58.419121 ax3-redactor-1.1.2/redactor/migrations/
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      822 2022-03-23 00:51:32.000000 ax3-redactor-1.1.2/redactor/migrations/0001_initial.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)        0 2022-03-23 00:51:32.000000 ax3-redactor-1.1.2/redactor/migrations/__init__.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      889 2022-04-07 14:08:23.000000 ax3-redactor-1.1.2/redactor/mixins.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      468 2022-04-07 13:54:41.000000 ax3-redactor-1.1.2/redactor/models.py
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-06-01 17:15:58.415121 ax3-redactor-1.1.2/redactor/static/
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-06-01 17:15:58.419121 ax3-redactor-1.1.2/redactor/static/redactor/
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      310 2022-03-23 00:51:32.000000 ax3-redactor-1.1.2/redactor/static/redactor/admin-redactor.css
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      576 2022-04-07 14:00:05.000000 ax3-redactor-1.1.2/redactor/static/redactor/admin-redactor.js
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      177 2022-03-23 00:51:32.000000 ax3-redactor-1.1.2/redactor/urls.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     2261 2022-06-01 17:13:47.000000 ax3-redactor-1.1.2/redactor/views.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)       38 2022-06-01 17:15:58.419121 ax3-redactor-1.1.2/setup.cfg
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     1255 2022-06-01 17:15:45.000000 ax3-redactor-1.1.2/setup.py
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:32:49.236620 ax3-redactor-2.0.0/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1064 2023-07-05 23:18:39.000000 ax3-redactor-2.0.0/LICENCE
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      109 2023-07-05 23:18:39.000000 ax3-redactor-2.0.0/MANIFEST.in
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     2400 2023-07-05 23:32:49.236497 ax3-redactor-2.0.0/PKG-INFO
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1513 2023-07-05 23:30:05.000000 ax3-redactor-2.0.0/README.md
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:32:49.234856 ax3-redactor-2.0.0/ax3_redactor.egg-info/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     2400 2023-07-05 23:32:49.000000 ax3-redactor-2.0.0/ax3_redactor.egg-info/PKG-INFO
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      516 2023-07-05 23:32:49.000000 ax3-redactor-2.0.0/ax3_redactor.egg-info/SOURCES.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)        1 2023-07-05 23:32:49.000000 ax3-redactor-2.0.0/ax3_redactor.egg-info/dependency_links.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)        1 2023-07-05 23:32:49.000000 ax3-redactor-2.0.0/ax3_redactor.egg-info/not-zip-safe
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)       24 2023-07-05 23:32:49.000000 ax3-redactor-2.0.0/ax3_redactor.egg-info/requires.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)        9 2023-07-05 23:32:49.000000 ax3-redactor-2.0.0/ax3_redactor.egg-info/top_level.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1773 2023-07-05 23:28:06.000000 ax3-redactor-2.0.0/pyproject.toml
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:32:49.235520 ax3-redactor-2.0.0/redactor/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:18:39.000000 ax3-redactor-2.0.0/redactor/__init__.py
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:32:49.235972 ax3-redactor-2.0.0/redactor/migrations/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      822 2023-07-05 23:18:39.000000 ax3-redactor-2.0.0/redactor/migrations/0001_initial.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:18:39.000000 ax3-redactor-2.0.0/redactor/migrations/__init__.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      889 2023-07-05 23:27:52.000000 ax3-redactor-2.0.0/redactor/mixins.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      467 2023-07-05 23:27:19.000000 ax3-redactor-2.0.0/redactor/models.py
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:32:49.233354 ax3-redactor-2.0.0/redactor/static/
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 23:32:49.236322 ax3-redactor-2.0.0/redactor/static/redactor/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      310 2023-07-05 23:18:39.000000 ax3-redactor-2.0.0/redactor/static/redactor/admin-redactor.css
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      576 2023-07-05 23:18:39.000000 ax3-redactor-2.0.0/redactor/static/redactor/admin-redactor.js
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      171 2023-07-05 23:24:41.000000 ax3-redactor-2.0.0/redactor/urls.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     2199 2023-07-05 23:24:41.000000 ax3-redactor-2.0.0/redactor/views.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)       38 2023-07-05 23:32:49.236669 ax3-redactor-2.0.0/setup.cfg
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1250 2023-07-05 23:32:00.000000 ax3-redactor-2.0.0/setup.py
```

### Comparing `ax3-redactor-1.1.2/PKG-INFO` & `ax3-redactor-2.0.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,92 @@
 Metadata-Version: 2.1
 Name: ax3-redactor
-Version: 1.1.2
+Version: 2.0.0
 Summary: A Django app to add support for redactor
 Home-page: https://github.com/Axiacore/ax3-redactor
 Author: Axiacore
 Author-email: info@axiacore.com
-License: UNKNOWN
-Description: # AX3 Redactor
-        
-        This app is part of the AX3 technology developed by Axiacore.
-        
-        It will allow to use redactor inside the django admin interface.
-        
-        ## Quick start
-        
-        1. Add "redactor" to your INSTALLED_APPS setting like this:
-        ```
-            INSTALLED_APPS = [
-                ...
-                'redactor',
-            ]
-        ```
-        
-        2. Include the redactor URLconf in your project urls.py like this:
-        ```
-            path('', include('redactor.urls')),
-        ```
-        
-        3. Run `python manage.py migrate` to create the redactor models.
-        
-        4. Copy this redactor library files into a `static` folder in your proyect:
-        ```
-            vendor/redactor/redactor.min.css
-            vendor/redactor/redactor.min.js
-            vendor/redactor/plugins/imagemanager.min.js
-            vendor/redactor/plugins/video.min.js
-            vendor/redactor/plugins/widget.min.js
-        ```
-        
-        5. Add to the admin.py the redactor support for a given model:
-        ```
-            from django.contrib import admin
-        
-            from redactor.mixins import RedactorMixin
-        
-            from .models import Post
-        
-        
-            @admin.register(Post)
-            class PostAdmin(RedactorMixin, admin.ModelAdmin):
-                ...
-        
-                redactor_fields = ['content']
-        
-                ...
-        ```
-        
-        `content` is a `TextField` attribute at the `Post` model.
-        You can use multiple fields.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# AX3 Redactor
+
+This app is part of the AX3 technology developed by Axiacore.
+
+It will allow to use redactor inside the django admin interface.
+
+## Quick start
+
+1. Add "redactor" to your INSTALLED_APPS setting like this:
+
+```python
+    INSTALLED_APPS = [
+        ...
+        'redactor',
+    ]
+```
+
+2. Include the redactor URLconf in your project urls.py like this:
+
+```python
+    path('', include('redactor.urls')),
+```
+
+3. Run `python manage.py migrate` to create the redactor models.
+
+4. Copy this redactor library files into a `static` folder in your proyect:
+
+```python
+    vendor/redactor/redactor.min.css
+    vendor/redactor/redactor.min.js
+    vendor/redactor/plugins/imagemanager.min.js
+    vendor/redactor/plugins/video.min.js
+    vendor/redactor/plugins/widget.min.js
+```
+
+5. Add to the admin.py the redactor support for a given model:
+
+```python
+    from django.contrib import admin
+
+    from redactor.mixins import RedactorMixin
+
+    from .models import Post
+
+
+    @admin.register(Post)
+    class PostAdmin(RedactorMixin, admin.ModelAdmin):
+        ...
+
+        redactor_fields = ['content']
+
+        ...
+```
+
+`content` is a `TextField` attribute at the `Post` model.
+You can use multiple fields.
+
+## Releasing a new version
+
+Make sure you have an API Token for PyPI: https://pypi.org/help/#apitoken
+
+Make sure you increase the version number and create a git tag:
+
+```bash
+$ python3 -m pip install --user --upgrade setuptools wheel twine
+$ ./release.sh
+```
+
+Made by [Axiacore](https://axiacore.com).
```

### Comparing `ax3-redactor-1.1.2/README.md` & `ax3-redactor-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,39 +3,43 @@
 This app is part of the AX3 technology developed by Axiacore.
 
 It will allow to use redactor inside the django admin interface.
 
 ## Quick start
 
 1. Add "redactor" to your INSTALLED_APPS setting like this:
-```
+
+```python
     INSTALLED_APPS = [
         ...
         'redactor',
     ]
 ```
 
 2. Include the redactor URLconf in your project urls.py like this:
-```
+
+```python
     path('', include('redactor.urls')),
 ```
 
 3. Run `python manage.py migrate` to create the redactor models.
 
 4. Copy this redactor library files into a `static` folder in your proyect:
-```
+
+```python
     vendor/redactor/redactor.min.css
     vendor/redactor/redactor.min.js
     vendor/redactor/plugins/imagemanager.min.js
     vendor/redactor/plugins/video.min.js
     vendor/redactor/plugins/widget.min.js
 ```
 
 5. Add to the admin.py the redactor support for a given model:
-```
+
+```python
     from django.contrib import admin
 
     from redactor.mixins import RedactorMixin
 
     from .models import Post
 
 
@@ -46,7 +50,20 @@
         redactor_fields = ['content']
 
         ...
 ```
 
 `content` is a `TextField` attribute at the `Post` model.
 You can use multiple fields.
+
+## Releasing a new version
+
+Make sure you have an API Token for PyPI: https://pypi.org/help/#apitoken
+
+Make sure you increase the version number and create a git tag:
+
+```bash
+$ python3 -m pip install --user --upgrade setuptools wheel twine
+$ ./release.sh
+```
+
+Made by [Axiacore](https://axiacore.com).
```

### Comparing `ax3-redactor-1.1.2/ax3_redactor.egg-info/PKG-INFO` & `ax3-redactor-2.0.0/ax3_redactor.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,92 @@
 Metadata-Version: 2.1
 Name: ax3-redactor
-Version: 1.1.2
+Version: 2.0.0
 Summary: A Django app to add support for redactor
 Home-page: https://github.com/Axiacore/ax3-redactor
 Author: Axiacore
 Author-email: info@axiacore.com
-License: UNKNOWN
-Description: # AX3 Redactor
-        
-        This app is part of the AX3 technology developed by Axiacore.
-        
-        It will allow to use redactor inside the django admin interface.
-        
-        ## Quick start
-        
-        1. Add "redactor" to your INSTALLED_APPS setting like this:
-        ```
-            INSTALLED_APPS = [
-                ...
-                'redactor',
-            ]
-        ```
-        
-        2. Include the redactor URLconf in your project urls.py like this:
-        ```
-            path('', include('redactor.urls')),
-        ```
-        
-        3. Run `python manage.py migrate` to create the redactor models.
-        
-        4. Copy this redactor library files into a `static` folder in your proyect:
-        ```
-            vendor/redactor/redactor.min.css
-            vendor/redactor/redactor.min.js
-            vendor/redactor/plugins/imagemanager.min.js
-            vendor/redactor/plugins/video.min.js
-            vendor/redactor/plugins/widget.min.js
-        ```
-        
-        5. Add to the admin.py the redactor support for a given model:
-        ```
-            from django.contrib import admin
-        
-            from redactor.mixins import RedactorMixin
-        
-            from .models import Post
-        
-        
-            @admin.register(Post)
-            class PostAdmin(RedactorMixin, admin.ModelAdmin):
-                ...
-        
-                redactor_fields = ['content']
-        
-                ...
-        ```
-        
-        `content` is a `TextField` attribute at the `Post` model.
-        You can use multiple fields.
-        
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# AX3 Redactor
+
+This app is part of the AX3 technology developed by Axiacore.
+
+It will allow to use redactor inside the django admin interface.
+
+## Quick start
+
+1. Add "redactor" to your INSTALLED_APPS setting like this:
+
+```python
+    INSTALLED_APPS = [
+        ...
+        'redactor',
+    ]
+```
+
+2. Include the redactor URLconf in your project urls.py like this:
+
+```python
+    path('', include('redactor.urls')),
+```
+
+3. Run `python manage.py migrate` to create the redactor models.
+
+4. Copy this redactor library files into a `static` folder in your proyect:
+
+```python
+    vendor/redactor/redactor.min.css
+    vendor/redactor/redactor.min.js
+    vendor/redactor/plugins/imagemanager.min.js
+    vendor/redactor/plugins/video.min.js
+    vendor/redactor/plugins/widget.min.js
+```
+
+5. Add to the admin.py the redactor support for a given model:
+
+```python
+    from django.contrib import admin
+
+    from redactor.mixins import RedactorMixin
+
+    from .models import Post
+
+
+    @admin.register(Post)
+    class PostAdmin(RedactorMixin, admin.ModelAdmin):
+        ...
+
+        redactor_fields = ['content']
+
+        ...
+```
+
+`content` is a `TextField` attribute at the `Post` model.
+You can use multiple fields.
+
+## Releasing a new version
+
+Make sure you have an API Token for PyPI: https://pypi.org/help/#apitoken
+
+Make sure you increase the version number and create a git tag:
+
+```bash
+$ python3 -m pip install --user --upgrade setuptools wheel twine
+$ ./release.sh
+```
+
+Made by [Axiacore](https://axiacore.com).
```

### Comparing `ax3-redactor-1.1.2/redactor/migrations/0001_initial.py` & `ax3-redactor-2.0.0/redactor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ax3-redactor-1.1.2/redactor/mixins.py` & `ax3-redactor-2.0.0/redactor/mixins.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,19 +8,19 @@
         for field in getattr(self, 'basic_redactor_fields', []):
             form.base_fields[field].widget.attrs['enable-basic-redactor'] = True
 
         return form
 
     class Media:
         css = {
-            'all': (
+            'all': [
                 'vendor/redactor/redactor.min.css',
                 'redactor/admin-redactor.css',
-            )
+            ]
         }
-        js = (
+        js = [
             'vendor/redactor/redactor.min.js',
             'vendor/redactor/plugins/imagemanager.min.js',
             'vendor/redactor/plugins/video.min.js',
             'vendor/redactor/plugins/widget.min.js',
             'redactor/admin-redactor.js',
-        )
+        ]
```

### Comparing `ax3-redactor-1.1.2/redactor/static/redactor/admin-redactor.js` & `ax3-redactor-2.0.0/redactor/static/redactor/admin-redactor.js`

 * *Files identical despite different names*

### Comparing `ax3-redactor-1.1.2/redactor/views.py` & `ax3-redactor-2.0.0/redactor/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from io import BytesIO
 
-from ax3_model_extras.webp import generate_webp
 from django.conf import settings
 from django.contrib.auth.mixins import UserPassesTestMixin
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.http import JsonResponse
 from django.utils.decorators import method_decorator
 from django.views.decorators.csrf import csrf_exempt
 from django.views.generic import View
@@ -15,19 +14,22 @@
 
 @method_decorator(csrf_exempt, name='dispatch')
 class RedactorView(UserPassesTestMixin, View):
     def test_func(self):
         return self.request.user.is_authenticated and self.request.user.is_staff
 
     def get(self, request, *args, **kwargs):
-        return JsonResponse([
-            {
-                'thumb': obj.file.url, 'url': obj.file.url, 'id': obj.id, 'title': obj.name
-            } for obj in RedactorFile.objects.filter(is_image=True)[:20]
-        ], safe=False)
+        return JsonResponse(
+            [
+                {
+                    'thumb': obj.file.url, 'url': obj.file.url, 'id': obj.id, 'title': obj.name
+                } for obj in RedactorFile.objects.filter(is_image=True)[:20]
+            ],
+            safe=False
+        )
 
     def post(self, request, *args, **kwargs):
         count = 0
         images = {}
         for file in request.FILES.getlist('file[]'):
             if getattr(settings, 'AWS_ACCESS_KEY_ID', None):
                 obj = RedactorFile.objects.create(file=file, name=file.name, is_image=False)
@@ -43,15 +45,14 @@
                     output_image.save(bytes_io, format=img_format, optimize=True)
 
                     obj = RedactorFile.objects.create(
                         file=SimpleUploadedFile(file.name, bytes_io.getvalue()),
                         name=file.name,
                         is_image=True,
                     )
-                    generate_webp(image_field=obj.file)
                 except UnidentifiedImageError:
                     obj = RedactorFile.objects.create(file=file, name=file.name, is_image=False)
 
-            images['file-{}'.format(count)] = {'url': obj.file.url, 'name': obj.name, 'id': obj.id}
+            images[f'file-{count}'] = {'url': obj.file.url, 'name': obj.name, 'id': obj.id}
             count += 1
 
         return JsonResponse(images, safe=False)
```

### Comparing `ax3-redactor-1.1.2/setup.py` & `ax3-redactor-2.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
-__VERSION__ = '1.1.2'
+__VERSION__ = '2.0.0'
 
-with open('README.md', 'r') as fh:
+with open('README.md') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ax3-redactor',
     version=__VERSION__,
     author='Axiacore',
     author_email='info@axiacore.com',
     description='A Django app to add support for redactor',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Axiacore/ax3-redactor',
     packages=setuptools.find_packages(),
-    install_requires=['ax3-model-extras>=1.2.4'],
+    install_requires=['ax3-model-extras>=2.0.0'],
     include_package_data=True,
     zip_safe=False,  # because we're including static files
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

