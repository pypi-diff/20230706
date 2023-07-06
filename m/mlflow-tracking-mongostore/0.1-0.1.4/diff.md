# Comparing `tmp/mlflow_tracking_mongostore-0.1-py3-none-any.whl.zip` & `tmp/mlflow_tracking_mongostore-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17825 bytes, number of entries: 9
+Zip file size: 17943 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 09:59 mlflow_tracking_mongostore/__init__.py
--rw-r--r--  2.0 unx     7861 b- defN 23-Jul-01 14:09 mlflow_tracking_mongostore/models.py
+-rw-r--r--  2.0 unx     8249 b- defN 23-Jul-06 13:05 mlflow_tracking_mongostore/models.py
 -rw-r--r--  2.0 unx    43830 b- defN 23-Jun-30 11:53 mlflow_tracking_mongostore/mongo_store.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-03 15:34 mlflow_tracking_mongostore-0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1389 b- defN 23-Jul-03 15:34 mlflow_tracking_mongostore-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 15:34 mlflow_tracking_mongostore-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-03 15:34 mlflow_tracking_mongostore-0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-03 15:34 mlflow_tracking_mongostore-0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      869 b- defN 23-Jul-03 15:34 mlflow_tracking_mongostore-0.1.dist-info/RECORD
-9 files, 65574 bytes uncompressed, 16287 bytes compressed:  75.2%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1389 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      149 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      881 b- defN 23-Jul-06 13:10 mlflow_tracking_mongostore-0.1.4.dist-info/RECORD
+9 files, 65974 bytes uncompressed, 16381 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mlflow_tracking_mongostore/models.py
 Comment: 
 
 Filename: mlflow_tracking_mongostore/mongo_store.py
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.dist-info/LICENSE
+Filename: mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.dist-info/METADATA
+Filename: mlflow_tracking_mongostore-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.dist-info/WHEEL
+Filename: mlflow_tracking_mongostore-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.dist-info/entry_points.txt
+Filename: mlflow_tracking_mongostore-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.dist-info/top_level.txt
+Filename: mlflow_tracking_mongostore-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.dist-info/RECORD
+Filename: mlflow_tracking_mongostore-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_tracking_mongostore/models.py

```diff
@@ -104,14 +104,15 @@
 
     def to_mlflow_entity(self) -> ExperimentTag:
         return ExperimentTag(key=self.key, value=self.value)
 
 
 class MongoExperiment(Document):
     experiment_id = StringField(primary_key=True)
+    exp_id = StringField(max_length=32, db_field="id")
     name = StringField(required=True, max_length=200)
     artifact_location = StringField(max_length=256)
     lifecycle_stage = StringField(max_length=50, default=LifecycleStage.ACTIVE)
     tags = ListField(EmbeddedDocumentField(MongoExperimentTag))
     creation_time = LongField()
     last_update_time = LongField()
 
@@ -124,14 +125,18 @@
             artifact_location=self.artifact_location,
             lifecycle_stage=self.lifecycle_stage,
             tags=[t.to_mlflow_entity() for t in self.tags],
             creation_time=self.creation_time,
             last_update_time=self.last_update_time,
         )
 
+    def save(self, *args, **kwargs):
+        self.exp_id = self.experiment_id
+        return super(MongoExperiment, self).save(*args, **kwargs)
+
 
 class MongoTag(EmbeddedDocument):
     key = StringField(required=True)
     value = StringField(required=True)
 
     def to_mlflow_entity(self) -> RunTag:
         return RunTag(key=self.key, value=self.value)
@@ -180,14 +185,15 @@
             timestamp=self.timestamp,
             step=self.step,
         )
 
 
 class MongoRun(Document):
     run_uuid = StringField(primary_key=True, required=True, max_length=32)
+    run_id = StringField(max_length=32, db_field="id")
     run_name = StringField(max_length=250)
     source_type = StringField(
         max_length=20, default=SourceType.to_string(SourceType.LOCAL)
     )
     source_name = StringField(max_length=500)
     entry_point_name = StringField(max_length=50)
     user_id = StringField(max_length=256, default="")
@@ -248,7 +254,11 @@
 
     def get_param_by_key(self, key):
         params = list(filter(lambda param: param.key == key, self.params))
         return params[0] if params else None
 
     def get_tags_by_key(self, key):
         return list(filter(lambda param: param.key == key, self.tags))
+
+    def save(self, *args, **kwargs):
+        self.run_id = self.run_uuid
+        return super(MongoRun, self).save(*args, **kwargs)
```

## Comparing `mlflow_tracking_mongostore-0.1.dist-info/LICENSE` & `mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlflow_tracking_mongostore-0.1.dist-info/METADATA` & `mlflow_tracking_mongostore-0.1.4.dist-info/METADATA`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-tracking-mongostore
-Version: 0.1
+Version: 0.1.4
 Summary: Mlflow plugin to use MongoDB as backend for MLflow tracking service
 Home-page: UNKNOWN
 Author: Rachid Belmeskine
 Maintainer-email: rachid.belmeskine@gmail.com
 License: UNKNOWN
 Keywords: mlflow
 Platform: UNKNOWN
@@ -14,26 +14,30 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Requires-Dist: mongoengine (==0.27.0)
 Requires-Dist: mlflow (==2.2.1)
 
 # mlflow-tracking-mongostore
 Mlflow plugin to use MongoDB as a backend for the MLflow models registry service. To use this plugin, you need a running instance of MongoDB.
 
 Run 'pip install mlflow-registry-mongostore' to register the plugin as an entrypoint with MongoDB backend.
 
-
 # Installation
-    pip install mlflow-registry-mongostore
-
+```
+pip install mlflow-registry-mongostore
+```
 
 # Usage
-    $ mlflow server --backend-store-uri mongodb://$USER:$PASSWORD@$MONGO_HOST:$DB_NAME
-    OR
-    $ mlflow server --backend-store-uri mongodb+srv://$USER:$PASSWORD@$MONGO_HOST:$DB_NAME
+```
+mlflow server --backend-store-uri mongodb://USER:PASSWORD@MONGO_HOST:DB_NAME
+```
+OR
+```
+mlflow server --backend-store-uri mongodb+srv://USER:PASSWORD@$MONGO_HOST:DB_NAME
+```
```

## Comparing `mlflow_tracking_mongostore-0.1.dist-info/RECORD` & `mlflow_tracking_mongostore-0.1.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlflow_tracking_mongostore/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mlflow_tracking_mongostore/models.py,sha256=TR90ls_TTyeWNAfHai8HlPKmL6LCZGyKNiWUsfW-pcI,7861
+mlflow_tracking_mongostore/models.py,sha256=6HsTzJDkLzIjZl0vLa_xZNYKtSkhpIO470yfFum756A,8249
 mlflow_tracking_mongostore/mongo_store.py,sha256=O8A07-rNkeuJG6saX6KUok_DNZV36QsDpWAuZqqWT0Q,43830
-mlflow_tracking_mongostore-0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mlflow_tracking_mongostore-0.1.dist-info/METADATA,sha256=vxiyjWMPSjUF07dtigHjeuiQVYqy7x2b9txzBMiHtjk,1389
-mlflow_tracking_mongostore-0.1.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-mlflow_tracking_mongostore-0.1.dist-info/entry_points.txt,sha256=1DhRgG-R9Qmgl1i-WxNc8x5JtKenuAkyVNYfAmZQOBo,149
-mlflow_tracking_mongostore-0.1.dist-info/top_level.txt,sha256=OWuYjvOHTC4KzmrdfxF9HUBd_TMuvjKoihXmytBaCKM,27
-mlflow_tracking_mongostore-0.1.dist-info/RECORD,,
+mlflow_tracking_mongostore-0.1.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mlflow_tracking_mongostore-0.1.4.dist-info/METADATA,sha256=yZQUhf1rFv4m4D8layQ6GKit6BFocBZ_E6RZb0By_p8,1389
+mlflow_tracking_mongostore-0.1.4.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+mlflow_tracking_mongostore-0.1.4.dist-info/entry_points.txt,sha256=1DhRgG-R9Qmgl1i-WxNc8x5JtKenuAkyVNYfAmZQOBo,149
+mlflow_tracking_mongostore-0.1.4.dist-info/top_level.txt,sha256=OWuYjvOHTC4KzmrdfxF9HUBd_TMuvjKoihXmytBaCKM,27
+mlflow_tracking_mongostore-0.1.4.dist-info/RECORD,,
```

