# Comparing `tmp/cumulus_library-0.3.3.tar.gz` & `tmp/cumulus_library-0.4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-0.4.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-0.3.3.tar` & `cumulus_library-0.4.0.dev1.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-lrwxr-xr-x   0        0        0        0 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      587 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/README.md
--rw-r--r--   0        0        0      963 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       45 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/__init__.py
--rw-r--r--   0        0        0      628 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/base_runner.py
--rwxr-xr-x   0        0        0    11182 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/cli.py
--rw-r--r--   0        0        0     5249 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0      272 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/errors.py
--rw-r--r--   0        0        0     1889 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/helper.py
--rw-r--r--   0        0        0      205 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2343 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0        0 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4848 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3346 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/counts.py
--rw-r--r--   0        0        0     3364 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     5876 2023-06-30 19:42:30.237433 cumulus_library-0.3.3/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0     2549 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/condition.sql
--rw-r--r--   0        0        0     2688 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/condition_codable_concept.sql
--rw-r--r--   0        0        0     4176 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/denormalizer.py
--rw-r--r--   0        0        0     2857 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/documentreference.sql
--rw-r--r--   0        0        0     3294 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/encounter.sql
--rw-r--r--   0        0        0     4126 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/fhir_define.sql
--rw-r--r--   0        0        0      661 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1231 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/medication_request.sql
--rw-r--r--   0        0        0     1208 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/observation.sql
--rw-r--r--   0        0        0     2874 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/observation_lab.sql
--rw-r--r--   0        0        0     1272 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/observation_vital_signs.sql
--rw-r--r--   0        0        0     1691 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/patient.sql
--rw-r--r--   0        0        0     6521 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/patient_extensions.sql
--rw-r--r--   0        0        0     1426 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     1472 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0      824 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     1562 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2023-06-30 19:42:30.241433 cumulus_library-0.3.3/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 10584966 2023-06-30 19:42:30.277433 cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2023-06-30 19:42:30.369432 cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      394 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      138 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     4643 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    16059 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/study_parser.py
--rw-r--r--   0        0        0     1430 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0      577 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      610 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0       61 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     1798 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      370 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0       52 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0       54 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0     7462 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/template_sql/templates.py
--rw-r--r--   0        0        0     2664 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/cumulus_library/upload.py
--rw-r--r--   0        0        0     1588 2023-06-30 19:42:30.377432 cumulus_library-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 cumulus_library-0.3.3/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      587 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/README.md
+-rw-r--r--   0        0        0      963 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       51 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/__init__.py
+-rw-r--r--   0        0        0      628 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/base_runner.py
+-rwxr-xr-x   0        0        0    11182 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/cli.py
+-rw-r--r--   0        0        0     5249 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0      272 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/errors.py
+-rw-r--r--   0        0        0     1889 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/helper.py
+-rw-r--r--   0        0        0      205 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2343 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4848 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3346 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/counts.py
+-rw-r--r--   0        0        0     3364 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     6030 2023-07-06 16:36:22.076354 cumulus_library-0.4.0.dev1/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0     2549 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition.sql
+-rw-r--r--   0        0        0     2688 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition_codable_concept.sql
+-rw-r--r--   0        0        0     3493 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.py
+-rw-r--r--   0        0        0     4550 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/count_core.sql
+-rw-r--r--   0        0        0     4176 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/denormalizer.py
+-rw-r--r--   0        0        0     2857 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/documentreference.sql
+-rw-r--r--   0        0        0     1505 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter.sql
+-rw-r--r--   0        0        0     2001 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/encounter_type.sql
+-rw-r--r--   0        0        0     4330 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/fhir_define.sql
+-rw-r--r--   0        0        0      782 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1231 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/medication_request.sql
+-rw-r--r--   0        0        0     1208 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation.sql
+-rw-r--r--   0        0        0     2874 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_lab.sql
+-rw-r--r--   0        0        0     1272 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_vital_signs.sql
+-rw-r--r--   0        0        0     1222 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient.sql
+-rw-r--r--   0        0        0     6521 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient_extensions.sql
+-rw-r--r--   0        0        0     1426 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     1472 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0      824 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     1562 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2023-07-06 16:36:22.080354 cumulus_library-0.4.0.dev1/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0 10584966 2023-07-06 16:36:22.124354 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2023-07-06 16:36:22.236356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      394 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      138 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0     4643 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    16059 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0     1430 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0      577 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      610 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0       61 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     1798 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      370 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0       52 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0       54 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0     7462 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/template_sql/templates.py
+-rw-r--r--   0        0        0     2664 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/cumulus_library/upload.py
+-rw-r--r--   0        0        0     1588 2023-07-06 16:36:22.248356 cumulus_library-0.4.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 cumulus_library-0.4.0.dev1/PKG-INFO
```

### Comparing `cumulus_library-0.3.3/README.md` & `cumulus_library-0.4.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/.sqlfluff` & `cumulus_library-0.4.0.dev1/cumulus_library/.sqlfluff`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/base_runner.py` & `cumulus_library-0.4.0.dev1/cumulus_library/base_runner.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/cli.py` & `cumulus_library-0.4.0.dev1/cumulus_library/cli.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/cli_parser.py` & `cumulus_library-0.4.0.dev1/cumulus_library/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/helper.py` & `cumulus_library-0.4.0.dev1/cumulus_library/helper.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-0.4.0.dev1/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/schema/columns.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/schema/counts.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/schema/typesystem.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/schema/valueset.py` & `cumulus_library-0.4.0.dev1/cumulus_library/schema/valueset.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 class ValueSet(Enum):
     Gender = "http://hl7.org/fhir/ValueSet/administrative-gender"
     Race = "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race"
     Ethnicity = "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity"
     DurationUnits = "http://hl7.org/fhir/valueset-duration-units.html"
     Units = "http://hl7.org/fhir/ValueSet/ucum-units"
-    EncounterCode = "http://hl7.org/fhir/v3/ActEncounterCode/vs.html"
+    PatientClass = "http://terminology.hl7.org/CodeSystem/v2-0004"
+    EncounterCode = "http://terminology.hl7.org/ValueSet/v3-ActEncounterCode"
+    EncounterPriority = "http://terminology.hl7.org/CodeSystem/v3-ActPriority"
     EncounterStatus = "http://hl7.org/fhir/ValueSet/encounter-status"
     EncounterType = "http://hl7.org/fhir/ValueSet/encounter-type"
     EncounterReason = "http://hl7.org/fhir/ValueSet/encounter-reason"
     EncounterLocationStatus = "http://hl7.org/fhir/ValueSet/encounter-location-status"
     ConditionCode = "http://hl7.org/fhir/ValueSet/condition-code"
     ConditionCategory = "http://hl7.org/fhir/ValueSet/condition-category"
     DocumentType = "http://hl7.org/fhir/ValueSet/c80-doc-typecodes"
```

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/condition.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/condition_codable_concept.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/condition_codable_concept.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/denormalizer.py` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/denormalizer.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/documentreference.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/documentreference.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/fhir_define.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/fhir_define.sql`

 * *Files 6% similar despite different names*

```diff
@@ -61,21 +61,26 @@
             'http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity'
         ),
         (
             'PostalCode',
             'http://hl7.org/fhir/datatypes-definitions.html#Address.postalCode'
         ),
         (
+            'PatientClass',
+            'http://terminology.hl7.org/CodeSystem/v2-0004'
+        ),
+        (
             'Encounter',
             'http://hl7.org/fhir/us/core/StructureDefinition/us-core-encounter'
         ),
         ('EncounterStatus', 'http://hl7.org/fhir/ValueSet/encounter-status'),
         ('EncounterType', 'http://hl7.org/fhir/ValueSet/encounter-type'),
         ('EncounterReason', 'http://hl7.org/fhir/ValueSet/encounter-reason'),
-        ('EncounterCode', 'http://hl7.org/fhir/v3/ActEncounterCode/vs.html'),
+        ('EncounterCode', 'http://terminology.hl7.org/ValueSet/v3-ActEncounterCode'),
+        ('EncounterPriority', 'http://terminology.hl7.org/CodeSystem/v3-ActPriority'),
         (
             'EncounterLocationStatus',
             'http://hl7.org/fhir/ValueSet/encounter-location-status'
         ),
         ('Period', 'http://hl7.org/fhir/datatypes.html#Period'),
         ('Coding', 'http://hl7.org/fhir/datatypes.html#Coding'),
         (
```

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/manifest.toml` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/manifest.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,26 +7,30 @@
 
 [sql_config]
 file_names = [
     "setup.sql",
     "fhir_define.sql",
     "patient.sql",
     "encounter.sql",
+    "encounter_type.sql",
     "documentreference.sql",
     "condition.sql",
     "observation.sql",
     "observation_lab.sql",
     "observation_vital_signs.sql",
     "medication_request.sql",
     "study_period.sql",
+    "count_core.sql"
 ]
 
 [export_config]
 export_list = [
     "core__count_patient",
     "core__count_encounter_month",
+    "core__count_encounter_type",
+    "core__count_encounter_type_month",
     "core__count_documentreference_month",
     "core__count_observation_lab_month",
     "core__count_condition_month",
     "core__count_medicationrequest_month",
     "core__meta_date",
 ]
```

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/medication_request.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/medication_request.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/observation.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/observation_lab.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_lab.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/observation_vital_signs.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/observation_vital_signs.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/patient.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient.sql`

 * *Files 15% similar despite different names*

```diff
@@ -35,30 +35,7 @@
 FROM
     temp_patient AS tp,
     unnest(tp.address) AS t_address (addr_row) --noqa: AL05
 
 WHERE
     tp.birthdate IS NOT NULL
     AND tp.gender IS NOT NULL;
-
-
-CREATE TABLE core__count_patient AS
-WITH powerset AS (
-    SELECT
-        count(DISTINCT cp.subject_ref) AS cnt_subject,
-        cp.gender,
-        cp.age,
-        cp.race_display,
-        cp.ethnicity_display
-    FROM core__patient AS cp
-    GROUP BY cube(cp.gender, cp.age, cp.race_display, cp.ethnicity_display)
-)
-
-SELECT
-    cnt_subject AS cnt,
-    gender,
-    age,
-    race_display,
-    ethnicity_display
-FROM powerset
-WHERE cnt_subject >= 10
-ORDER BY cnt DESC;
```

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/patient_extensions.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/patient_extensions.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/setup.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/core/study_period.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/template/counts.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/template/manifest.toml` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/template/setup.sql` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-0.4.0.dev1/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/study_parser.py` & `cumulus_library-0.4.0.dev1/cumulus_library/study_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/template_sql/templates.py` & `cumulus_library-0.4.0.dev1/cumulus_library/template_sql/templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/cumulus_library/upload.py` & `cumulus_library-0.4.0.dev1/cumulus_library/upload.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/pyproject.toml` & `cumulus_library-0.4.0.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-0.3.3/PKG-INFO` & `cumulus_library-0.4.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 0.3.3
+Version: 0.4.0.dev1
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.9, <3.12
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

