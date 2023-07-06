# Comparing `tmp/mlflow_registry_mongostore-0.1.3-py3-none-any.whl.zip` & `tmp/mlflow_registry_mongostore-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 20178 bytes, number of entries: 10
+Zip file size: 20248 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 09:59 mlflow_registry_mongostore/__init__.py
 -rw-r--r--  2.0 unx    18488 b- defN 23-Jun-29 10:01 mlflow_registry_mongostore/_version.py
--rw-r--r--  2.0 unx     4996 b- defN 23-Jun-30 11:21 mlflow_registry_mongostore/models.py
+-rw-r--r--  2.0 unx     5214 b- defN 23-Jul-06 13:06 mlflow_registry_mongostore/models.py
 -rw-r--r--  2.0 unx    40867 b- defN 23-Jun-30 11:20 mlflow_registry_mongostore/mongo_store.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 05:36 mlflow_registry_mongostore-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1372 b- defN 23-Jul-06 05:36 mlflow_registry_mongostore-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 05:36 mlflow_registry_mongostore-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      155 b- defN 23-Jul-06 05:36 mlflow_registry_mongostore-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-06 05:36 mlflow_registry_mongostore-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      977 b- defN 23-Jul-06 05:36 mlflow_registry_mongostore-0.1.3.dist-info/RECORD
-10 files, 78331 bytes uncompressed, 18464 bytes compressed:  76.4%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1388 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      155 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      977 b- defN 23-Jul-06 13:11 mlflow_registry_mongostore-0.1.4.dist-info/RECORD
+10 files, 78565 bytes uncompressed, 18534 bytes compressed:  76.4%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: mlflow_registry_mongostore/models.py
 Comment: 
 
 Filename: mlflow_registry_mongostore/mongo_store.py
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.3.dist-info/LICENSE
+Filename: mlflow_registry_mongostore-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.3.dist-info/METADATA
+Filename: mlflow_registry_mongostore-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.3.dist-info/WHEEL
+Filename: mlflow_registry_mongostore-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.3.dist-info/entry_points.txt
+Filename: mlflow_registry_mongostore-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.3.dist-info/top_level.txt
+Filename: mlflow_registry_mongostore-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.3.dist-info/RECORD
+Filename: mlflow_registry_mongostore-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_registry_mongostore/models.py

```diff
@@ -81,14 +81,15 @@
             key=self.key,
             value=self.value,
         )
 
 
 class MongoRegisteredModel(Document):
     name = StringField(primary_key=True)
+    registed_model_id = StringField(max_length=32, db_field="id")
     creation_timestamp = LongField(default=get_current_time_millis)
     last_updated_timestamp = LongField()
     description = StringField(max_length=256)
     tags = ListField(EmbeddedDocumentField(MongoRegisteredModelTag))
 
     meta = {"collection": REGISTERED_MODEL_COLLECTION_NAME}
 
@@ -100,14 +101,18 @@
             description=self.description,
             tags=[t.to_mlflow_entity() for t in self.tags],
         )
 
     def get_tags_by_key(self, key):
         return list(filter(lambda param: param.key == key, self.tags))
 
+    def save(self, *args, **kwargs):
+        self.registed_model_id = self.name
+        return super(MongoRegisteredModel, self).save(*args, **kwargs)
+
 
 class MongoModelVersion(Document):
     # name = StringField(primary_key=True)
     registered_model_id = ReferenceField(
         "MongoRegisteredModel", reverse_delete_rule=CASCADE
     )
     version = IntField(required=True)
```

## Comparing `mlflow_registry_mongostore-0.1.3.dist-info/LICENSE` & `mlflow_registry_mongostore-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlflow_registry_mongostore-0.1.3.dist-info/METADATA` & `mlflow_registry_mongostore-0.1.4.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-registry-mongostore
-Version: 0.1.3
+Version: 0.1.4
 Summary: Mlflow plugin to use MongoDB as backend for MLflow Model Registry service
 Home-page: UNKNOWN
 Author: Rachid Belmeskine
 Maintainer-email: rachid.belmeskine@gmail.com
 License: UNKNOWN
 Keywords: mlflow
 Platform: UNKNOWN
@@ -23,17 +23,21 @@
 Requires-Dist: mlflow (==2.2.1)
 
 # mlflow-tracking-mongostore
 Mlflow plugin to use MongoDB as a backend for the MLflow tracking service. To use this plugin, you need a running instance of MongoDB.
 
 Run 'pip install mlflow-tracking-mongostore' to register the plugin as an entrypoint with MongoDB backend.
 
-
 # Installation
+```
 pip install mlflow-tracking-mongostore
-
+```
 
 # Usage
-$ mlflow server --backend-store-uri mongodb://USER:PASSWORD@MONGO_HOST:DB_NAME 
-OR 
-$ mlflow server --backend-store-uri mongodb+srv://USER:PASSWORD@$MONGO_HOST:DB_NAME
+```
+mlflow server --backend-store-uri mongodb://USER:PASSWORD@MONGO_HOST:DB_NAME
+```
+OR
+```
+mlflow server --backend-store-uri mongodb+srv://USER:PASSWORD@$MONGO_HOST:DB_NAME
+```
```

## Comparing `mlflow_registry_mongostore-0.1.3.dist-info/RECORD` & `mlflow_registry_mongostore-0.1.4.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mlflow_registry_mongostore/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_registry_mongostore/_version.py,sha256=nTDwWbHLCXMqdi1bkEkchAiz_JAzkXcmH3bKG0jf6fg,18488
-mlflow_registry_mongostore/models.py,sha256=UdebZ8LkSbKBk4a5KT74riIjqOgxXD5ti8lb0uR_gjY,4996
+mlflow_registry_mongostore/models.py,sha256=GtrxUR_y0t9QoWf3JmiVNR4zlnmCw4TOJryUb_IT4Dg,5214
 mlflow_registry_mongostore/mongo_store.py,sha256=5lxamQ_HlvoRbcZt3wD7NTz3toIk6JfG68bNePWyNzY,40867
-mlflow_registry_mongostore-0.1.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mlflow_registry_mongostore-0.1.3.dist-info/METADATA,sha256=h_lGR2tAvzo19p_3QXkbALHkd5KDGWjVvlkwT_JuedY,1372
-mlflow_registry_mongostore-0.1.3.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-mlflow_registry_mongostore-0.1.3.dist-info/entry_points.txt,sha256=tfl_ffj0PkSrXY4rvesmyyvPXDS-j5egPU_XNXoVKm4,155
-mlflow_registry_mongostore-0.1.3.dist-info/top_level.txt,sha256=6DHvL6p3UTy_bC25io6QqOIFVHNwvfFY0Nj_664suUE,27
-mlflow_registry_mongostore-0.1.3.dist-info/RECORD,,
+mlflow_registry_mongostore-0.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mlflow_registry_mongostore-0.1.4.dist-info/METADATA,sha256=tC2MAzmWXDVc8YuotCGi0mIzYDjBinycSi8QxbPJhoo,1388
+mlflow_registry_mongostore-0.1.4.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+mlflow_registry_mongostore-0.1.4.dist-info/entry_points.txt,sha256=tfl_ffj0PkSrXY4rvesmyyvPXDS-j5egPU_XNXoVKm4,155
+mlflow_registry_mongostore-0.1.4.dist-info/top_level.txt,sha256=6DHvL6p3UTy_bC25io6QqOIFVHNwvfFY0Nj_664suUE,27
+mlflow_registry_mongostore-0.1.4.dist-info/RECORD,,
```

