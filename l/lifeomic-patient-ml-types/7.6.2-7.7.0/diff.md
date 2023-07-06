# Comparing `tmp/lifeomic_patient_ml_types-7.6.2.tar.gz` & `tmp/lifeomic_patient_ml_types-7.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-7.6.2.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-7.7.0.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-7.6.2.tar` & `lifeomic_patient_ml_types-7.7.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    15045 2023-06-05 19:27:08.715935 lifeomic_patient_ml_types-7.6.2/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      664 2023-06-05 19:28:26.884631 lifeomic_patient_ml_types-7.6.2/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.2/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.6.2/PKG-INFO
+-rw-r--r--   0        0        0    15565 2023-07-06 18:45:29.982074 lifeomic_patient_ml_types-7.7.0/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      664 2023-07-06 18:47:16.558804 lifeomic_patient_ml_types-7.7.0/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.7.0/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-7.7.0/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-7.6.2/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-7.7.0/lifeomic_patient_ml_types/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -471,14 +471,37 @@
     class Config:
         extra = Extra.forbid
 
     name: str
     value: str
 
 
+class LogEvent(BaseModel):
+    """
+    An event logged by some component of a model run, as well as metadata about the log event.
+    """
+
+    class Config:
+        extra = Extra.forbid
+
+    type: Literal["logEntry"]
+    timestamp: float
+    """
+    The time when the log event occurred, expressed as milliseconds since the unix epoch.
+    """
+    payload: str
+    """
+    The actual body of the logged event.
+    """
+    stage: str
+    """
+    The model run's stage or component that produced this log event.
+    """
+
+
 class ImageSegmentationProblemBase(BaseModel):
     class Config:
         extra = Extra.allow
 
     problemType: Literal["imgSeg"]
     trainingDataFilter: FhirCodesFilter
     """
```

### Comparing `lifeomic_patient_ml_types-7.6.2/pyproject.toml` & `lifeomic_patient_ml_types-7.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "7.6.2"
+version = "7.7.0"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

