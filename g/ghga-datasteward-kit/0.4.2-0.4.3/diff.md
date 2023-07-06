# Comparing `tmp/ghga_datasteward_kit-0.4.2.tar.gz` & `tmp/ghga_datasteward_kit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_datasteward_kit-0.4.2.tar", last modified: Tue Jul  4 08:54:47 2023, max compression
+gzip compressed data, was "ghga_datasteward_kit-0.4.3.tar", last modified: Thu Jul  6 11:59:00 2023, max compression
```

## Comparing `ghga_datasteward_kit-0.4.2.tar` & `ghga_datasteward_kit-0.4.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:54:47.870286 ghga_datasteward_kit-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-04 08:54:47.870286 ghga_datasteward_kit-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:54:47.866286 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/batch_s3_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/catalog_accession_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:54:47.866286 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20809 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:54:47.866286 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-04 08:54:47.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-04 08:54:47.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:54:47.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 08:54:47.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 08:54:47.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-04 08:54:47.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-04 08:54:47.000000 ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-04 08:54:47.870286 ghga_datasteward_kit-0.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:54:47.866286 ghga_datasteward_kit-0.4.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 08:54:47.870286 ghga_datasteward_kit-0.4.2/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/fixtures/ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/fixtures/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/test_file_ingest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/test_s3_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-04 08:54:38.000000 ghga_datasteward_kit-0.4.2/tests/test_size_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.508344 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6589 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/batch_s3_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3327 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/catalog_accession_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20809 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.508344 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 11:59:00.000000 ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:59:00.512344 ghga_datasteward_kit-0.4.3/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_file_ingest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_s3_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-06 11:58:48.000000 ghga_datasteward_kit-0.4.3/tests/test_size_adjustment.py
```

### Comparing `ghga_datasteward_kit-0.4.2/LICENSE` & `ghga_datasteward_kit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/PKG-INFO` & `ghga_datasteward_kit-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_datasteward_kit
-Version: 0.4.2
+Version: 0.4.3
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.2/README.md` & `ghga_datasteward_kit-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/__init__.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A utils package for GHGA data stewards."""
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
```

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/__main__.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/batch_s3_upload.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/batch_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/catalog_accession_generator.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/catalog_accession_generator.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/__init__.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/file.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/file.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/main.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/cli/metadata.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/config.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/file_ingest.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/file_ingest.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,29 +37,38 @@
         ..., description="Public key used for encryption of the payload."
     )
     input_dir: Path = Field(
         ...,
         description="Path to directory containing output files from the "
         + "upload/batch_upload command.",
     )
+    map_files_fields: list[str] = Field(
+        ["study_files"],
+        description="Names of the accession map fields for looking up the"
+        + " alias->accession mapping.",
+    )
 
 
-def alias_to_accession(alias: str, submission_store: SubmissionStore) -> str:
+def alias_to_accession(
+    alias: str, map_fields: list[str], submission_store: SubmissionStore
+) -> str:
     """Get all submissions to retrieve valid accessions from corresponding file aliases"""
 
     submission_ids = submission_store.get_all_submission_ids()
 
     all_submission_map = {}
 
     for submission_id in submission_ids:
-        all_submission_map.update(
-            submission_store.get_by_id(submission_id=submission_id).accession_map[
-                "files"
-            ]
-        )
+        submission = submission_store.get_by_id(submission_id=submission_id)
+        for field in map_fields:
+            if field not in submission.accession_map:
+                raise ValueError(
+                    f"Configured field {field} not found in accession map."
+                )
+            all_submission_map.update(submission.accession_map[field])
 
     accession = all_submission_map.get(alias)
 
     if accession is None:
         raise ValueError(f"No accession exists for file alias {alias}")
 
     return accession
@@ -87,25 +96,27 @@
     return errors
 
 
 def file_ingest(
     in_path: Path,
     token: str,
     config: IngestConfig,
-    alias_to_id: Callable[[str, SubmissionStore], str] = alias_to_accession,
+    alias_to_id: Callable[[str, list[str], SubmissionStore], str] = alias_to_accession,
 ):
     """
     Transform from s3 upload output representation to what the file ingest service expects.
     Then call the ingest endpoint
     """
 
     submission_store = SubmissionStore(config=config)
 
     output_metadata = models.OutputMetadata.load(input_path=in_path)
-    file_id = alias_to_id(output_metadata.alias, submission_store)
+    file_id = alias_to_id(
+        output_metadata.alias, config.map_files_fields, submission_store
+    )
     upload_metadata = output_metadata.to_upload_metadata(file_id=file_id)
     encrypted = upload_metadata.encrypt_metadata(pubkey=config.file_ingest_pubkey)
 
     headers = {"Authorization": f"Bearer {token}"}
 
     with httpx.Client() as client:
         response = client.post(
```

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/loading.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/loading.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/main.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/main.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/metadata.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/models.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/models.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/s3_upload.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit/utils.py` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/PKG-INFO` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga-datasteward-kit
-Version: 0.4.2
+Version: 0.4.3
 Summary: GHGA Data Steward Kit - A utils package for GHGA data stewards.
 Home-page: https://github.com/ghga-de/ghga-datasteward-kit
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ghga_datasteward_kit-0.4.2/ghga_datasteward_kit.egg-info/SOURCES.txt` & `ghga_datasteward_kit-0.4.3/ghga_datasteward_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/setup.cfg` & `ghga_datasteward_kit-0.4.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/setup.py` & `ghga_datasteward_kit-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/tests/fixtures/__init__.py` & `ghga_datasteward_kit-0.4.3/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/tests/fixtures/config.py` & `ghga_datasteward_kit-0.4.3/tests/fixtures/config.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/tests/fixtures/ingest.py` & `ghga_datasteward_kit-0.4.3/tests/fixtures/ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from ghga_datasteward_kit.file_ingest import IngestConfig
 from ghga_datasteward_kit.models import OutputMetadata
 
 EXAMPLE_SUBMISSION = Submission(
     title="test",
     description="test",
     content={"test_class": [{"alias": "test_alias"}]},
-    accession_map={"files": {"test_alias": "test_accession"}},
+    accession_map={"study_files": {"test_alias": "test_accession"}},
     id="testsubmission001",
     status_history=(
         StatusChange(
             timestamp=now_as_utc(),
             new_status=SubmissionStatus.COMPLETED,
         ),
     ),
@@ -86,14 +86,15 @@
 
             metadata.serialize(file_path)
 
             config = IngestConfig(
                 file_ingest_url="https://not-a-valid-url",
                 file_ingest_pubkey=encode_key(keypair.public),
                 input_dir=Path(input_dir),
+                map_files_fields=["study_files"],
                 submission_store_dir=Path(submission_store_dir),
             )
 
             submission_store = SubmissionStore(config=config)
             submission_store.insert_new(submission=EXAMPLE_SUBMISSION)
 
             yield IngestFixture(
```

### Comparing `ghga_datasteward_kit-0.4.2/tests/fixtures/metadata.py` & `ghga_datasteward_kit-0.4.3/tests/fixtures/metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/tests/fixtures/utils.py` & `ghga_datasteward_kit-0.4.3/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/tests/test_file_ingest.py` & `ghga_datasteward_kit-0.4.3/tests/test_file_ingest.py`

 * *Files 17% similar despite different names*

```diff
@@ -32,20 +32,39 @@
 @pytest.mark.asyncio
 async def test_alias_to_accession(ingest_fixture: IngestFixture):  # noqa: F811
     """Test alias->accession mapping"""
 
     submission_store = SubmissionStore(config=ingest_fixture.config)
     metadata = models.OutputMetadata.load(input_path=ingest_fixture.file_path)
 
-    accession = alias_to_accession(metadata.alias, submission_store=submission_store)
-    example_accession = list(EXAMPLE_SUBMISSION.accession_map["files"].values())[0]
+    accession = alias_to_accession(
+        alias=metadata.alias,
+        map_fields=ingest_fixture.config.map_files_fields,
+        submission_store=submission_store,
+    )
+    example_accession = list(
+        EXAMPLE_SUBMISSION.accession_map[
+            ingest_fixture.config.map_files_fields[0]
+        ].values()
+    )[0]
     assert accession == example_accession
 
     with pytest.raises(ValueError):
-        alias_to_accession("invalid_alias", submission_store=submission_store)
+        alias_to_accession(
+            alias="invalid_alias",
+            map_fields=ingest_fixture.config.map_files_fields,
+            submission_store=submission_store,
+        )
+
+    with pytest.raises(ValueError):
+        alias_to_accession(
+            alias=metadata.alias,
+            map_fields=["study_files", "sample_files"],
+            submission_store=submission_store,
+        )
 
 
 @pytest.mark.asyncio
 async def test_ingest_directly(
     ingest_fixture: IngestFixture, httpx_mock: HTTPXMock  # noqa: F811
 ):
     """Test file_ingest function directly"""
```

### Comparing `ghga_datasteward_kit-0.4.2/tests/test_metadata.py` & `ghga_datasteward_kit-0.4.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/tests/test_s3_upload.py` & `ghga_datasteward_kit-0.4.3/tests/test_s3_upload.py`

 * *Files identical despite different names*

### Comparing `ghga_datasteward_kit-0.4.2/tests/test_size_adjustment.py` & `ghga_datasteward_kit-0.4.3/tests/test_size_adjustment.py`

 * *Files identical despite different names*

