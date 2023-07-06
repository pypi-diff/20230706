# Comparing `tmp/django_cloud_storages-1.1.7.tar.gz` & `tmp/django_cloud_storages-1.1.8.tar.gz`

## Comparing `django_cloud_storages-1.1.7.tar` & `django_cloud_storages-1.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/.readthedocs.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/__init__.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/backends/__init__.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/backends/appwrite.py
--rw-r--r--   0        0        0    10464 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/cloud_storages/backends/dropbox.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/LICENSE
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/README.md
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/.readthedocs.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/cloud_storages/__init__.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/cloud_storages/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/cloud_storages/backends/__init__.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/cloud_storages/backends/appwrite.py
+-rw-r--r--   0        0        0    10523 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/cloud_storages/backends/dropbox.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/LICENSE
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/README.md
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 django_cloud_storages-1.1.8/PKG-INFO
```

### Comparing `django_cloud_storages-1.1.7/.readthedocs.yaml` & `django_cloud_storages-1.1.8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.7/cloud_storages/utils.py` & `django_cloud_storages-1.1.8/cloud_storages/utils.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.7/cloud_storages/backends/appwrite.py` & `django_cloud_storages-1.1.8/cloud_storages/backends/appwrite.py`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.7/cloud_storages/backends/dropbox.py` & `django_cloud_storages-1.1.8/cloud_storages/backends/dropbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,16 @@
 
     def delete(self, name):
         """
         Delete the specified file from the storage system.
         """
         full_name = self._full_path(name)
         try:
-            self.dbx.files_delete_v2(full_name)
+            result = self.dbx.files_delete_v2(full_name)
+            return result
         except ApiError as e:
             throwDropboxException(e)
                 
     def exists(self, name):
         """
         Return True if a file referenced by the given name already exists in the
         storage system, or False if the name is available for a new file.
@@ -164,15 +165,16 @@
             return True
         except ApiError as e:
             err = e.error
             if err.is_path_lookup():
                 # lookUpError = err.get_path_lookup()
                 # error_msg = dropBoxErrorMsg(lookUpError._tag)
                 return False
-            raise e
+            else:
+                raise e
     
     def listdir(self, path):
         """
         List the contents of the specified path. Return a 2-tuple of lists:
         the first item being directories, the second item being files.
         """
         directories, files = [], []
```

### Comparing `django_cloud_storages-1.1.7/.gitignore` & `django_cloud_storages-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.7/LICENSE` & `django_cloud_storages-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.7/README.md` & `django_cloud_storages-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.7/pyproject.toml` & `django_cloud_storages-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_cloud_storages-1.1.7/PKG-INFO` & `django_cloud_storages-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloud-storages
-Version: 1.1.7
+Version: 1.1.8
 Summary: Cloud file storages for django.
 Project-URL: Homepage, https://pypi.org/project/django-cloud-storages
 Project-URL: Source code, https://github.com/Samiddha99/django-cloud-storages
 Project-URL: Documentation, https://django-cloud-storages.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/Samiddha99/django-cloud-storages/issues
 Author-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
 Maintainer-email: Samiddha Chakrabarti <samiddha99@protonmail.com>
```

