# Comparing `tmp/bike-0.3.2.tar.gz` & `tmp/bike-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bike-0.3.2.tar", max compression
+gzip compressed data, was "bike-0.3.3.tar", max compression
```

## Comparing `bike-0.3.2.tar` & `bike-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.2/LICENSE
--rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.2/README.md
--rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.2/bike/__init__.py
--rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.2/bike/controllers.py
--rw-r--r--   0        0        0     2995 2023-06-02 10:56:24.512070 bike-0.3.2/bike/fields.py
--rw-r--r--   0        0        0     8299 2023-05-21 10:46:27.744577 bike-0.3.2/bike/models.py
--rw-r--r--   0        0        0      495 2023-06-02 11:01:56.163636 bike-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.3/README.md
+-rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.3/bike/__init__.py
+-rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.3/bike/controllers.py
+-rw-r--r--   0        0        0     3013 2023-07-06 11:21:30.500729 bike-0.3.3/bike/fields.py
+-rw-r--r--   0        0        0     8564 2023-07-06 11:13:29.712411 bike-0.3.3/bike/models.py
+-rw-r--r--   0        0        0      495 2023-07-06 11:36:19.500581 bike-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.3/PKG-INFO
```

### Comparing `bike-0.3.2/LICENSE` & `bike-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bike-0.3.2/README.md` & `bike-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `bike-0.3.2/bike/controllers.py` & `bike-0.3.3/bike/controllers.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.2/bike/fields.py` & `bike-0.3.3/bike/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         if (value is None or str(value) == '') and self.required:
             if self.default is not None:
                 return self.default
             else:
                 raise Exception(f'Field {self.name} required.')
         for validator in self.validators_pre:
             value = validator(self.model, value)
-        if not value:
+        if value is None:
             value = self.default or None
         if self.list:
             value = [
                 self.list_type(**item) if isinstance(item, dict) else self.list_type(item) for item in value
             ]
         elif self.object:
             value = self.list_type(**value) if isinstance(value, dict) else value
@@ -72,15 +72,15 @@
                     value = datetime.datetime.strptime(value, '%Y-%m-%d').date()
                 elif self.type == float:
                     value = float(value)
                 elif self.type == bool:
                     value = True if value == 'true' else False
                 elif self.type == str:
                     value = str(value)
-                else:
+                elif self.required:
                     value = self.type(value)
             except Exception as e:
                 raise Exception(f'Field[{self.name}] - {e}')
         for validator in self.validators_pos:
             value = validator(instance, value)
         return value
```

### Comparing `bike-0.3.2/bike/models.py` & `bike-0.3.3/bike/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,36 @@
 
 
 __validators__ = {}
 types_default = {
     'str': '""',
     'int': '0',
     'float': '0.0',
-    'bool': 'False'
+    'bool': 'False',
 }
 
 
 def create_init_function(fields):
     params_required_txt = ''
     params_optional_txt = ''
     body_fn = ''
     for k, field in fields.items():
         name = field.alias if field.alias and field.alias_load else k
         if field.prefix and field.alias_load:
             name = f'{field.prefix}_{name}'
         if field.object:
-            param = f'{name}: dict | Any'
+            if issubclass(field.type, bike.Model):
+                param = f'{name}: "{field.type.__name__}"'
+            else:
+                param = f'{name}: dict | Any'
         else:
-            param = f'{name}: {field.type.__name__}'
+            if issubclass(field.type, bike.Model):
+                param = f'{name}: "{field.type.__name__}"'
+            else:
+                param = f'{name}: {field.type.__name__}'
         if field.required:
             if field.default:
                 param = f"{param} = '{field.default}'"
                 params_optional_txt = f'{params_optional_txt}, {param}' if params_optional_txt else param
             else:
                 params_required_txt = f'{params_required_txt}, {param}' if params_required_txt else param
         else:
```

### Comparing `bike-0.3.2/PKG-INFO` & `bike-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bike
-Version: 0.3.2
+Version: 0.3.3
 Summary: A lightweight model validator for modern projects.
 Home-page: https://github.com/manasseslima/bike
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

