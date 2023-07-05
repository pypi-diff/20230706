# Comparing `tmp/AX3 model extras-1.5.3.tar.gz` & `tmp/AX3 model extras-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AX3 model extras-1.5.3.tar", last modified: Tue May  3 22:14:06 2022, max compression
+gzip compressed data, was "AX3 model extras-2.0.0.tar", last modified: Wed Jul  5 22:06:59 2023, max compression
```

## Comparing `AX3 model extras-1.5.3.tar` & `AX3 model extras-2.0.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-05-03 22:14:06.246866 AX3 model extras-1.5.3/
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-05-03 22:14:06.242866 AX3 model extras-1.5.3/AX3_model_extras.egg-info/
--rwxrwxrwx   0 axiacore  (1001) axiacore  (1001)     4388 2022-05-03 22:14:06.000000 AX3 model extras-1.5.3/AX3_model_extras.egg-info/PKG-INFO
--rwxrwxrwx   0 axiacore  (1001) axiacore  (1001)      501 2022-05-03 22:14:06.000000 AX3 model extras-1.5.3/AX3_model_extras.egg-info/SOURCES.txt
--rwxrwxrwx   0 axiacore  (1001) axiacore  (1001)        1 2022-05-03 22:14:06.000000 AX3 model extras-1.5.3/AX3_model_extras.egg-info/dependency_links.txt
--rwxrwxrwx   0 axiacore  (1001) axiacore  (1001)       62 2022-05-03 22:14:06.000000 AX3 model extras-1.5.3/AX3_model_extras.egg-info/requires.txt
--rwxrwxrwx   0 axiacore  (1001) axiacore  (1001)       17 2022-05-03 22:14:06.000000 AX3 model extras-1.5.3/AX3_model_extras.egg-info/top_level.txt
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     1065 2020-12-22 21:19:57.000000 AX3 model extras-1.5.3/LICENSE
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)       68 2021-04-30 16:16:35.000000 AX3 model extras-1.5.3/MANIFEST.in
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     4388 2022-05-03 22:14:06.242866 AX3 model extras-1.5.3/PKG-INFO
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     2832 2021-04-30 17:00:22.000000 AX3 model extras-1.5.3/README.md
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-05-03 22:14:06.242866 AX3 model extras-1.5.3/ax3_model_extras/
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)        0 2020-12-22 21:19:57.000000 AX3 model extras-1.5.3/ax3_model_extras/__init__.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      143 2021-04-22 15:13:29.000000 AX3 model extras-1.5.3/ax3_model_extras/apps.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     4203 2021-04-22 15:13:29.000000 AX3 model extras-1.5.3/ax3_model_extras/fields.py
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-05-03 22:14:06.242866 AX3 model extras-1.5.3/ax3_model_extras/locale/
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-05-03 22:14:06.242866 AX3 model extras-1.5.3/ax3_model_extras/locale/es/
-drwxrwxr-x   0 axiacore  (1001) axiacore  (1001)        0 2022-05-03 22:14:06.242866 AX3 model extras-1.5.3/ax3_model_extras/locale/es/LC_MESSAGES/
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     1417 2022-04-25 22:47:37.000000 AX3 model extras-1.5.3/ax3_model_extras/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     1973 2022-04-25 22:47:37.000000 AX3 model extras-1.5.3/ax3_model_extras/locale/es/LC_MESSAGES/django.po
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      739 2020-12-22 21:19:57.000000 AX3 model extras-1.5.3/ax3_model_extras/storages.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     2764 2022-05-03 22:13:12.000000 AX3 model extras-1.5.3/ax3_model_extras/validators.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)     1103 2022-04-25 18:18:40.000000 AX3 model extras-1.5.3/ax3_model_extras/webp.py
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)       38 2022-05-03 22:14:06.246866 AX3 model extras-1.5.3/setup.cfg
--rw-rw-r--   0 axiacore  (1001) axiacore  (1001)      915 2022-05-03 22:13:45.000000 AX3 model extras-1.5.3/setup.py
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 22:06:59.500926 AX3 model extras-2.0.0/
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 22:06:59.498860 AX3 model extras-2.0.0/AX3_model_extras.egg-info/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     3477 2023-07-05 22:06:59.000000 AX3 model extras-2.0.0/AX3_model_extras.egg-info/PKG-INFO
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      476 2023-07-05 22:06:59.000000 AX3 model extras-2.0.0/AX3_model_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)        1 2023-07-05 22:06:59.000000 AX3 model extras-2.0.0/AX3_model_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)       45 2023-07-05 22:06:59.000000 AX3 model extras-2.0.0/AX3_model_extras.egg-info/requires.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)       17 2023-07-05 22:06:59.000000 AX3 model extras-2.0.0/AX3_model_extras.egg-info/top_level.txt
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1065 2023-07-05 21:47:19.000000 AX3 model extras-2.0.0/LICENSE
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)       68 2023-07-05 21:47:19.000000 AX3 model extras-2.0.0/MANIFEST.in
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     3477 2023-07-05 22:06:59.500763 AX3 model extras-2.0.0/PKG-INFO
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     3059 2023-07-05 21:58:50.000000 AX3 model extras-2.0.0/README.md
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 22:06:59.499823 AX3 model extras-2.0.0/ax3_model_extras/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 21:47:19.000000 AX3 model extras-2.0.0/ax3_model_extras/__init__.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      143 2023-07-05 21:47:19.000000 AX3 model extras-2.0.0/ax3_model_extras/apps.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     3917 2023-07-05 21:54:11.000000 AX3 model extras-2.0.0/ax3_model_extras/fields.py
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 22:06:59.497439 AX3 model extras-2.0.0/ax3_model_extras/locale/
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 22:06:59.497492 AX3 model extras-2.0.0/ax3_model_extras/locale/es/
+drwxr-xr-x   0 felipe3dfx   (501) staff       (20)        0 2023-07-05 22:06:59.500357 AX3 model extras-2.0.0/ax3_model_extras/locale/es/LC_MESSAGES/
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1417 2023-07-05 21:47:19.000000 AX3 model extras-2.0.0/ax3_model_extras/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1973 2023-07-05 21:47:19.000000 AX3 model extras-2.0.0/ax3_model_extras/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      739 2023-07-05 21:47:19.000000 AX3 model extras-2.0.0/ax3_model_extras/storages.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)     1707 2023-07-05 21:55:11.000000 AX3 model extras-2.0.0/ax3_model_extras/validators.py
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)       38 2023-07-05 22:06:59.500978 AX3 model extras-2.0.0/setup.cfg
+-rw-r--r--   0 felipe3dfx   (501) staff       (20)      882 2023-07-05 21:56:13.000000 AX3 model extras-2.0.0/setup.py
```

### Comparing `AX3 model extras-1.5.3/AX3_model_extras.egg-info/PKG-INFO` & `AX3 model extras-2.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,153 +1,155 @@
 Metadata-Version: 2.1
-Name: AX3-model-extras
-Version: 1.5.3
+Name: AX3 model extras
+Version: 2.0.0
 Summary: Django app extras for AX3 models
-Home-page: https://github.com/Axiacore/ax3-model-extras
+Home-page: https://github.com/axiacore/ax3-model-extras
 Author: Axiacore
 Author-email: info@axiacore.com
-License: UNKNOWN
-Description: # AX3 Model Extras
-        
-        ## Installation
-        AX3 Model Extras is easy to install from the PyPI package:
-        
-        ```bash
-        $ pip install ax3-model-extras
-        ```
-        
-        To enable ax3_model_extras in your project you need to add it to INSTALLED_APPS in your projects settings.py file:
-        
-        ```python
-        INSTALLED_APPS = (
-            ...
-            'ax3_model_extras',
-            ...
-        )
-        ```
-        
-        ## Validate image size
-        
-        If you want to validate the dimension and file size for images:
-        
-        ```python
-        from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = models.ImageField(
-                validators=[ImageDimensionValidator([1920, 800]), FileSizeValidator(350)],
-                help_text='JPG. 1920x800px. 350kb max.',
-            )
-        ```
-        
-        If you want to validate one dimension, you have to send the other dimension with 0
-        
-        ```python
-        from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = models.ImageField(
-                validators=[ImageDimensionValidator([1920, 0]), FileSizeValidator(350)],
-                help_text='JPG. width=1920px. 350kb max.',
-            )
-        ```
-        
-        
-        
-        ## Improve file storage
-        
-        If you want to improve the local file storage or use S3 upload:
-        
-        ```python
-        from ax3_model_extras.storages import get_storage, get_upload_path
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = models.ImageField(
-                upload_to=get_upload_path,
-                storage=get_storage(),
-            )
-        ```
-        
-        
-        ## Optimize images before upload them.
-        
-        Use as:
-        
-        ```python
-        from ax3_model_extras.fields import OptimizedImageField
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = OptimizedImageField()
-        
-        ```
-        
-        
-        If want to set the size of the image using the 'cover' method do:
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-        )
-        ```
-        
-        
-        If want to set the size of the image using the 'thumbnail' method do:
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-            optimized_image_resize_method='thumbnail',
-        )
-        ```
-        
-        
-        If want to restrict the file format do (If not set it supports JPEG, PNG and GIF):
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-            optimized_image_resize_method='thumbnail',
-            optimized_file_formats=['PNG'],
-        )
-        ```
-        
-        
-        If want to specific quality of the image (If not set it default =  75):
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-            optimized_image_resize_method='thumbnail',
-            optimized_file_formats=['PNG'],
-            optimized_image_quality=85.5,
-        )
-        ```
-        
-        Resize is done using https://pypi.org/project/python-resize-image/
-        
-        Made by Axiacore.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AX3 Model Extras
+
+## Installation
+
+AX3 Model Extras is easy to install from the PyPI package:
+
+```bash
+$ pip install ax3-model-extras
+```
+
+To enable ax3_model_extras in your project you need to add it to INSTALLED_APPS in your projects settings.py file:
+
+```python
+INSTALLED_APPS = (
+    ...
+    'ax3_model_extras',
+    ...
+)
+```
+
+## Validate image size
+
+If you want to validate the dimension and file size for images:
+
+```python
+from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = models.ImageField(
+        validators=[ImageDimensionValidator([1920, 800]), FileSizeValidator(350)],
+        help_text='JPG. 1920x800px. 350kb max.',
+    )
+```
+
+If you want to validate one dimension, you have to send the other dimension with 0
+
+```python
+from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = models.ImageField(
+        validators=[ImageDimensionValidator([1920, 0]), FileSizeValidator(350)],
+        help_text='JPG. width=1920px. 350kb max.',
+    )
+```
+
+## Improve file storage
+
+If you want to improve the local file storage or use S3 upload:
+
+```python
+from ax3_model_extras.storages import get_storage, get_upload_path
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = models.ImageField(
+        upload_to=get_upload_path,
+        storage=get_storage(),
+    )
+```
+
+## Optimize images before upload them.
+
+Use as:
+
+```python
+from ax3_model_extras.fields import OptimizedImageField
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = OptimizedImageField()
+
+```
+
+If want to set the size of the image using the 'cover' method do:
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+)
+```
+
+If want to set the size of the image using the 'thumbnail' method do:
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+    optimized_image_resize_method='thumbnail',
+)
+```
+
+If want to restrict the file format do (If not set it supports JPEG, PNG and GIF):
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+    optimized_image_resize_method='thumbnail',
+    optimized_file_formats=['PNG'],
+)
+```
+
+If want to specific quality of the image (If not set it default =  75):
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+    optimized_image_resize_method='thumbnail',
+    optimized_file_formats=['PNG'],
+    optimized_image_quality=85.5,
+)
+```
+
+Resize is done using [python-resize-image](https://pypi.org/project/python-resize-image/)
+
+## Releasing a new version
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

### Comparing `AX3 model extras-1.5.3/LICENSE` & `AX3 model extras-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AX3 model extras-1.5.3/PKG-INFO` & `AX3 model extras-2.0.0/AX3_model_extras.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,153 +1,155 @@
 Metadata-Version: 2.1
-Name: AX3 model extras
-Version: 1.5.3
+Name: AX3-model-extras
+Version: 2.0.0
 Summary: Django app extras for AX3 models
-Home-page: https://github.com/Axiacore/ax3-model-extras
+Home-page: https://github.com/axiacore/ax3-model-extras
 Author: Axiacore
 Author-email: info@axiacore.com
-License: UNKNOWN
-Description: # AX3 Model Extras
-        
-        ## Installation
-        AX3 Model Extras is easy to install from the PyPI package:
-        
-        ```bash
-        $ pip install ax3-model-extras
-        ```
-        
-        To enable ax3_model_extras in your project you need to add it to INSTALLED_APPS in your projects settings.py file:
-        
-        ```python
-        INSTALLED_APPS = (
-            ...
-            'ax3_model_extras',
-            ...
-        )
-        ```
-        
-        ## Validate image size
-        
-        If you want to validate the dimension and file size for images:
-        
-        ```python
-        from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = models.ImageField(
-                validators=[ImageDimensionValidator([1920, 800]), FileSizeValidator(350)],
-                help_text='JPG. 1920x800px. 350kb max.',
-            )
-        ```
-        
-        If you want to validate one dimension, you have to send the other dimension with 0
-        
-        ```python
-        from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = models.ImageField(
-                validators=[ImageDimensionValidator([1920, 0]), FileSizeValidator(350)],
-                help_text='JPG. width=1920px. 350kb max.',
-            )
-        ```
-        
-        
-        
-        ## Improve file storage
-        
-        If you want to improve the local file storage or use S3 upload:
-        
-        ```python
-        from ax3_model_extras.storages import get_storage, get_upload_path
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = models.ImageField(
-                upload_to=get_upload_path,
-                storage=get_storage(),
-            )
-        ```
-        
-        
-        ## Optimize images before upload them.
-        
-        Use as:
-        
-        ```python
-        from ax3_model_extras.fields import OptimizedImageField
-        
-        
-        class Post(models.Model):
-            title = models.CharField()
-        
-            slug = models.SlugField()
-        
-            image = OptimizedImageField()
-        
-        ```
-        
-        
-        If want to set the size of the image using the 'cover' method do:
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-        )
-        ```
-        
-        
-        If want to set the size of the image using the 'thumbnail' method do:
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-            optimized_image_resize_method='thumbnail',
-        )
-        ```
-        
-        
-        If want to restrict the file format do (If not set it supports JPEG, PNG and GIF):
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-            optimized_image_resize_method='thumbnail',
-            optimized_file_formats=['PNG'],
-        )
-        ```
-        
-        
-        If want to specific quality of the image (If not set it default =  75):
-        
-        ```python
-        image = OptimizedImageField(
-            optimized_image_output_size=(1920, 800),
-            optimized_image_resize_method='thumbnail',
-            optimized_file_formats=['PNG'],
-            optimized_image_quality=85.5,
-        )
-        ```
-        
-        Resize is done using https://pypi.org/project/python-resize-image/
-        
-        Made by Axiacore.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AX3 Model Extras
+
+## Installation
+
+AX3 Model Extras is easy to install from the PyPI package:
+
+```bash
+$ pip install ax3-model-extras
+```
+
+To enable ax3_model_extras in your project you need to add it to INSTALLED_APPS in your projects settings.py file:
+
+```python
+INSTALLED_APPS = (
+    ...
+    'ax3_model_extras',
+    ...
+)
+```
+
+## Validate image size
+
+If you want to validate the dimension and file size for images:
+
+```python
+from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = models.ImageField(
+        validators=[ImageDimensionValidator([1920, 800]), FileSizeValidator(350)],
+        help_text='JPG. 1920x800px. 350kb max.',
+    )
+```
+
+If you want to validate one dimension, you have to send the other dimension with 0
+
+```python
+from ax3_model_extras.validators import FileSizeValidator, ImageDimensionValidator
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = models.ImageField(
+        validators=[ImageDimensionValidator([1920, 0]), FileSizeValidator(350)],
+        help_text='JPG. width=1920px. 350kb max.',
+    )
+```
+
+## Improve file storage
+
+If you want to improve the local file storage or use S3 upload:
+
+```python
+from ax3_model_extras.storages import get_storage, get_upload_path
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = models.ImageField(
+        upload_to=get_upload_path,
+        storage=get_storage(),
+    )
+```
+
+## Optimize images before upload them.
+
+Use as:
+
+```python
+from ax3_model_extras.fields import OptimizedImageField
+
+
+class Post(models.Model):
+    title = models.CharField()
+
+    slug = models.SlugField()
+
+    image = OptimizedImageField()
+
+```
+
+If want to set the size of the image using the 'cover' method do:
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+)
+```
+
+If want to set the size of the image using the 'thumbnail' method do:
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+    optimized_image_resize_method='thumbnail',
+)
+```
+
+If want to restrict the file format do (If not set it supports JPEG, PNG and GIF):
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+    optimized_image_resize_method='thumbnail',
+    optimized_file_formats=['PNG'],
+)
+```
+
+If want to specific quality of the image (If not set it default =  75):
+
+```python
+image = OptimizedImageField(
+    optimized_image_output_size=(1920, 800),
+    optimized_image_resize_method='thumbnail',
+    optimized_file_formats=['PNG'],
+    optimized_image_quality=85.5,
+)
+```
+
+Resize is done using [python-resize-image](https://pypi.org/project/python-resize-image/)
+
+## Releasing a new version
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

### Comparing `AX3 model extras-1.5.3/README.md` & `AX3 model extras-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # AX3 Model Extras
 
 ## Installation
+
 AX3 Model Extras is easy to install from the PyPI package:
 
 ```bash
 $ pip install ax3-model-extras
 ```
 
 To enable ax3_model_extras in your project you need to add it to INSTALLED_APPS in your projects settings.py file:
@@ -49,16 +50,14 @@
 
     image = models.ImageField(
         validators=[ImageDimensionValidator([1920, 0]), FileSizeValidator(350)],
         help_text='JPG. width=1920px. 350kb max.',
     )
 ```
 
-
-
 ## Improve file storage
 
 If you want to improve the local file storage or use S3 upload:
 
 ```python
 from ax3_model_extras.storages import get_storage, get_upload_path
 
@@ -70,15 +69,14 @@
 
     image = models.ImageField(
         upload_to=get_upload_path,
         storage=get_storage(),
     )
 ```
 
-
 ## Optimize images before upload them.
 
 Use as:
 
 ```python
 from ax3_model_extras.fields import OptimizedImageField
 
@@ -88,52 +86,57 @@
 
     slug = models.SlugField()
 
     image = OptimizedImageField()
 
 ```
 
-
 If want to set the size of the image using the 'cover' method do:
 
 ```python
 image = OptimizedImageField(
     optimized_image_output_size=(1920, 800),
 )
 ```
 
-
 If want to set the size of the image using the 'thumbnail' method do:
 
 ```python
 image = OptimizedImageField(
     optimized_image_output_size=(1920, 800),
     optimized_image_resize_method='thumbnail',
 )
 ```
 
-
 If want to restrict the file format do (If not set it supports JPEG, PNG and GIF):
 
 ```python
 image = OptimizedImageField(
     optimized_image_output_size=(1920, 800),
     optimized_image_resize_method='thumbnail',
     optimized_file_formats=['PNG'],
 )
 ```
 
-
 If want to specific quality of the image (If not set it default =  75):
 
 ```python
 image = OptimizedImageField(
     optimized_image_output_size=(1920, 800),
     optimized_image_resize_method='thumbnail',
     optimized_file_formats=['PNG'],
     optimized_image_quality=85.5,
 )
 ```
 
-Resize is done using https://pypi.org/project/python-resize-image/
+Resize is done using [python-resize-image](https://pypi.org/project/python-resize-image/)
+
+## Releasing a new version
+
+Make sure you increase the version number and create a git tag:
+
+```bash
+$ python3 -m pip install --user --upgrade setuptools wheel twine
+$ ./release.sh
+```
 
-Made by Axiacore.
+Made by [Axiacore](https://axiacore.com).
```

### Comparing `AX3 model extras-1.5.3/ax3_model_extras/fields.py` & `AX3 model extras-2.0.0/ax3_model_extras/fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from django.core.exceptions import ValidationError
 from django.db.models import ImageField
 from django.utils.translation import gettext_lazy as _
 from PIL import Image
 from resizeimage import resizeimage
 from resizeimage.imageexceptions import ImageSizeError
 
-from .webp import generate_webp
-
 
 class OptimizedImageField(ImageField):
     def __init__(self, *args, **kwargs):
         """
         `optimized_image_output_size` must be a tuple and `optimized_image_resize_method` can be
         'crop', 'cover', 'contain', 'width', 'height' or 'thumbnail'.
         """
@@ -30,22 +28,14 @@
         kwargs.pop('optimized_image_output_size', None)
         kwargs.pop('optimized_image_resize_method', None)
         kwargs.pop('optimized_file_formats', None)
         kwargs.pop('optimized_image_quality', None)
 
         return name, path, args, kwargs
 
-    def pre_save(self, model_instance, add):
-        image_field = super().pre_save(model_instance, add)
-
-        if image_field:
-            generate_webp(image_field=image_field, quality=str(self.optimized_image_quality))
-
-        return image_field
-
     def save_form_data(self, instance, data):
         updating_image = data and getattr(instance, self.name) != data
         if updating_image:
 
             if self.optimized_image_quality < 0 or self.optimized_image_quality > 100:
                 raise ValidationError({self.name: [_('The allowed quality is from 0 to 100')]})
```

### Comparing `AX3 model extras-1.5.3/ax3_model_extras/locale/es/LC_MESSAGES/django.mo` & `AX3 model extras-2.0.0/ax3_model_extras/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `AX3 model extras-1.5.3/ax3_model_extras/locale/es/LC_MESSAGES/django.po` & `AX3 model extras-2.0.0/ax3_model_extras/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `AX3 model extras-1.5.3/ax3_model_extras/storages.py` & `AX3 model extras-2.0.0/ax3_model_extras/storages.py`

 * *Files identical despite different names*

### Comparing `AX3 model extras-1.5.3/setup.py` & `AX3 model extras-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import os
 
 import setuptools
 
-__VERSION__ = '1.5.3'
+__VERSION__ = '2.0.0'
 
-with open('README.md', 'r') as fh:
+with open('README.md') as fh:
     long_description = fh.read()
 
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setuptools.setup(
     name='AX3 model extras',
     version=__VERSION__,
     author='Axiacore',
     author_email='info@axiacore.com',
     description='Django app extras for AX3 models',
     include_package_data=True,
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/Axiacore/ax3-model-extras',
+    url='https://github.com/axiacore/ax3-model-extras',
     packages=setuptools.find_packages(),
     install_requires=[
         'django >= 3.2',
         'python-resize-image',
         'python_magic',
-        'phonenumberslite',
     ],
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

