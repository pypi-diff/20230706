# Comparing `tmp/z3_target_bigquery-0.6.6.tar.gz` & `tmp/z3_target_bigquery-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3_target_bigquery-0.6.6.tar", max compression
+gzip compressed data, was "z3_target_bigquery-0.6.7.tar", max compression
```

## Comparing `z3_target_bigquery-0.6.6.tar` & `z3_target_bigquery-0.6.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1078 2023-01-20 23:36:48.960193 z3_target_bigquery-0.6.6/LICENSE
--rw-r--r--   0        0        0    20800 2023-04-20 22:31:15.806538 z3_target_bigquery-0.6.6/README.md
--rw-r--r--   0        0        0     2099 2023-04-20 19:59:59.743672 z3_target_bigquery-0.6.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-20 18:27:41.011352 z3_target_bigquery-0.6.6/target_bigquery/__init__.py
--rw-r--r--   0        0        0     4965 2023-04-02 03:16:22.076367 z3_target_bigquery-0.6.6/target_bigquery/batch_job.py
--rw-r--r--   0        0        0     2575 2023-04-02 03:16:22.077092 z3_target_bigquery-0.6.6/target_bigquery/constants.py
--rw-r--r--   0        0        0    42167 2023-04-20 22:07:12.619047 z3_target_bigquery-0.6.6/target_bigquery/core.py
--rw-r--r--   0        0        0     9442 2023-04-02 03:16:22.078271 z3_target_bigquery-0.6.6/target_bigquery/gcs_stage.py
--rw-r--r--   0        0        0     4986 2023-04-02 03:16:22.079246 z3_target_bigquery-0.6.6/target_bigquery/proto_gen.py
--rw-r--r--   0        0        0    13091 2023-04-02 03:16:22.079767 z3_target_bigquery-0.6.6/target_bigquery/storage_write.py
--rw-r--r--   0        0        0     4468 2023-04-02 03:16:22.080448 z3_target_bigquery-0.6.6/target_bigquery/streaming_insert.py
--rw-r--r--   0        0        0    22149 2023-04-20 22:02:47.844135 z3_target_bigquery-0.6.6/target_bigquery/target.py
--rw-r--r--   0        0        0    22323 1970-01-01 00:00:00.000000 z3_target_bigquery-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-01-20 23:36:48.960193 z3_target_bigquery-0.6.7/LICENSE
+-rw-r--r--   0        0        0    20800 2023-04-20 22:31:15.806538 z3_target_bigquery-0.6.7/README.md
+-rw-r--r--   0        0        0     2099 2023-07-06 01:50:04.802064 z3_target_bigquery-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-20 18:27:41.011352 z3_target_bigquery-0.6.7/target_bigquery/__init__.py
+-rw-r--r--   0        0        0     4965 2023-04-02 03:16:22.076367 z3_target_bigquery-0.6.7/target_bigquery/batch_job.py
+-rw-r--r--   0        0        0     2575 2023-04-02 03:16:22.077092 z3_target_bigquery-0.6.7/target_bigquery/constants.py
+-rw-r--r--   0        0        0    42187 2023-07-06 01:48:30.817830 z3_target_bigquery-0.6.7/target_bigquery/core.py
+-rw-r--r--   0        0        0     9442 2023-04-02 03:16:22.078271 z3_target_bigquery-0.6.7/target_bigquery/gcs_stage.py
+-rw-r--r--   0        0        0     4986 2023-04-02 03:16:22.079246 z3_target_bigquery-0.6.7/target_bigquery/proto_gen.py
+-rw-r--r--   0        0        0    13961 2023-07-06 01:48:30.818548 z3_target_bigquery-0.6.7/target_bigquery/storage_write.py
+-rw-r--r--   0        0        0     4468 2023-04-02 03:16:22.080448 z3_target_bigquery-0.6.7/target_bigquery/streaming_insert.py
+-rw-r--r--   0        0        0    22598 2023-07-06 01:48:30.819534 z3_target_bigquery-0.6.7/target_bigquery/target.py
+-rw-r--r--   0        0        0    22323 1970-01-01 00:00:00.000000 z3_target_bigquery-0.6.7/PKG-INFO
```

### Comparing `z3_target_bigquery-0.6.6/LICENSE` & `z3_target_bigquery-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.6/README.md` & `z3_target_bigquery-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.6/pyproject.toml` & `z3_target_bigquery-0.6.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "z3-target-bigquery"
-version = "0.6.6"
+version = "0.6.7"
 description = "z3-target-bigquery is a Singer target for BigQuery. It supports storage write, GCS, streaming, and batch load methods. Built with the Meltano SDK."
 authors = ["Alex Butler <butler.alex2010@gmail.com>"]
 keywords = ["ELT", "BigQuery"]
 license = "MIT"
 include = ["target_bigquery/*.py", "README.md", "LICENSE"]
 homepage = "https://github.com/z3z1ma/target-bigquery"
 repository = "https://github.com/z3z1ma/target-bigquery"
```

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/batch_job.py` & `z3_target_bigquery-0.6.7/target_bigquery/batch_job.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/constants.py` & `z3_target_bigquery-0.6.7/target_bigquery/constants.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/core.py` & `z3_target_bigquery-0.6.7/target_bigquery/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -496,30 +496,30 @@
             # We must merge the temp table into the target table.
             target = self.merge_target.as_table()
             date_columns = ["_sdc_extracted_at", "_sdc_received_at"]
             tmp, ctas_tmp = None, "SELECT 1 AS _no_op"
             if self._is_dedupe_before_upsert_candidate():
                 # We can't use MERGE with a non-unique key, so we need to dedupe the temp table into
                 # a _SESSION scoped intermediate table.
-                tmp = f"{target.name}__tmp"
+                tmp = f"{self.merge_target.name}__tmp"
                 dedupe_query = (
-                    f"SELECT * FROM {self.table} "
+                    f"SELECT * FROM {self.table.get_escaped_name()} "
                     f"QUALIFY ROW_NUMBER() OVER (PARTITION BY {', '.join(self.key_properties)} "
                     f"ORDER BY COALESCE({', '.join(date_columns)}) DESC) = 1"
                 )
                 ctas_tmp = f"CREATE OR REPLACE TEMP TABLE `{tmp}` AS {dedupe_query}"
             merge_clause = (
                 f"MERGE `{self.merge_target}` AS target USING `{tmp or self.table}` AS source ON "
                 + " AND ".join(f"target.`{f}` = source.`{f}`" for f in self.key_properties)
             )
             update_clause = "UPDATE SET " + ", ".join(
                 f"target.`{f.name}` = source.`{f.name}`" for f in target.schema
             )
             insert_clause = (
-                f"INSERT ({', '.join(f.name for f in target.schema)}) "
+                f"INSERT ({', '.join(f'`{f.name}`' for f in target.schema)}) "
                 f"VALUES ({', '.join(f'source.`{f.name}`' for f in target.schema)})"
             )
             self.client.query(
                 f"{ctas_tmp}; {merge_clause} "
                 f"WHEN MATCHED THEN {update_clause} "
                 f"WHEN NOT MATCHED THEN {insert_clause}; "
                 f"DROP TABLE IF EXISTS {self.table.get_escaped_name()};"
@@ -527,18 +527,18 @@
             self.table = self.merge_target
             self.merge_target = None
         elif self.overwrite_target is not None:
             # We must overwrite the target table with the temp table.
             # Do it in a transaction to avoid partial writes.
             target = self.overwrite_target.as_table()
             self.client.query(
-                f"DROP TABLE IF EXISTS {self.overwrite_target.get_escaped_name()}; "
-                f"CREATE TABLE {self.overwrite_target} LIKE {self.table.get_escaped_name()} AS "
-                f"SELECT * FROM {self.table.get_escaped_name()};"
-                f"DROP TABLE IF EXISTS {self.table.get_escaped_name()};"
+                f"DROP TABLE IF EXISTS {self.overwrite_target.get_escaped_name()}; CREATE TABLE"
+                f" {self.overwrite_target.get_escaped_name()} AS SELECT * FROM"
+                f" {self.table.get_escaped_name()}; DROP TABLE IF EXISTS"
+                f" {self.table.get_escaped_name()};"
             ).result()
             self.table = self.merge_target
             self.merge_target = None
 
 
 class Denormalized:
     """This class provides common overrides for denormalized sinks and should be subclassed
```

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/gcs_stage.py` & `z3_target_bigquery-0.6.7/target_bigquery/gcs_stage.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/proto_gen.py` & `z3_target_bigquery-0.6.7/target_bigquery/proto_gen.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/storage_write.py` & `z3_target_bigquery-0.6.7/target_bigquery/storage_write.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # The above copyright notice and this permission notice shall be included in all copies or
 # substantial portions of the Software.
 """BigQuery Storage Write Sink.
 Throughput test: 11m 0s @ 1M rows / 150 keys / 1.5GB
 NOTE: This is naive and will vary drastically based on network speed, for example on a GCP VM.
 """
 import os
+from time import sleep
 from multiprocessing import Process
 from multiprocessing.connection import Connection
 from multiprocessing.dummy import Process as _Thread
 from queue import Empty
 from typing import (
     TYPE_CHECKING,
     Any,
@@ -42,19 +43,20 @@
     from target_bigquery.target import TargetBigQuery
 
 import logging
 
 from target_bigquery.core import BaseBigQuerySink, BaseWorker, Denormalized, storage_client_factory
 from target_bigquery.proto_gen import proto_schema_factory_v2
 
+logger = logging.getLogger(__name__)
+
 # Stream specific constant
 MAX_IN_FLIGHT = 15
 """Maximum number of concurrent requests per worker be processed by grpc before awaiting."""
 
-
 Dispatcher = Callable[[types.AppendRowsRequest], writer.AppendRowsFuture]
 StreamComponents = Tuple[str, writer.AppendRowsStream, Dispatcher]
 
 
 def get_application_stream(client: BigQueryWriteClient, job: "Job") -> StreamComponents:
     """Get an application created stream for the parent. This stream must be finalized and committed."""
     write_stream = types.WriteStream()
@@ -118,60 +120,75 @@
     message.DESCRIPTOR.CopyToProto(proto_descriptor)
     proto_schema.proto_descriptor = proto_descriptor
     proto_data.writer_schema = proto_schema
     template.proto_rows = proto_data
     return template
 
 
-class Job(NamedTuple):
+class Job():
     parent: str
     template: types.AppendRowsRequest
     stream_notifier: Connection
     data: types.ProtoRows
-    offset: int = 0
     attempts: int = 1
-
+    
+    def __init__(self,
+        parent,
+        template,
+        stream_notifier,
+        data):
+        """Initialize the worker process."""
+        self.parent = parent
+        self.template = template
+        self.stream_notifier = stream_notifier
+        self.data = data
 
 class StorageWriteBatchWorker(BaseWorker):
     """Worker process for the storage write API."""
 
     def __init__(self, *args, **kwargs):
         """Initialize the worker process."""
         super().__init__(*args, **kwargs)
         self.get_stream_components = get_application_stream
         self.awaiting: List[writer.AppendRowsFuture] = []
         self.cache: Dict[str, StreamComponents] = {}
         self.max_errors_before_recycle = 5
+        self.offsets: Dict[str, int] = {}
+        self.logger=logger
 
     def run(self):
         """Run the worker process."""
         client: BigQueryWriteClient = storage_client_factory(self.credentials)
         if os.getenv("TARGET_BIGQUERY_DEBUG", "false").lower() == "true":
             bidi_logger = logging.getLogger("google.api_core.bidi")
             bidi_logger.setLevel(logging.DEBUG)
         while True:
             try:
                 job: Optional[Job] = self.queue.get(timeout=30.0)
             except Empty:
                 break
             if job is None:
                 break
-            if job.parent not in self.cache:
+            if job.parent not in self.cache or self.cache[job.parent][1]._closed:
                 self.cache[job.parent] = self.get_stream_components(client, job)
+                self.offsets[job.parent] = 0
             write_stream, _, dispatch = cast(StreamComponents, self.cache[job.parent])
+           
             try:
                 kwargs = {}
                 if write_stream.endswith("_default"):
                     kwargs["offset"] = None
                     kwargs["path"] = write_stream
                 else:
-                    kwargs["offset"] = job.offset
+                    kwargs["offset"] = self.offsets[job.parent]
                 self.awaiting.append(dispatch(generate_request(job.data, **kwargs)))
+                
             except Exception as exc:
                 job.attempts += 1
+                self.logger.info(f"job.attempts : {job.attempts}")
                 self.max_errors_before_recycle -= 1
                 if job.attempts > 3:
                     # TODO: add a metric for this + a DLQ & wrap exception type
                     self.error_notifier.send((exc, self.serialize_exception(exc)))
                 else:
                     self.queue.put(job)
                 # Track errors and recycle the stream if we hit a threshold
@@ -182,23 +199,26 @@
                 if self.max_errors_before_recycle == 0:
                     self.wait(drain=True)
                     self.close_cached_streams()
                     raise
             else:
                 self.log_notifier.send(
                     f"[{self.ext_id}] Sent {len(job.data.serialized_rows)} rows to {write_stream}"
-                    f" with offset {job.offset}."
+                    f" with offset {self.offsets[job.parent]}."
                 )
+                self.offsets[job.parent] += len(job.data.serialized_rows)
                 if len(self.awaiting) > MAX_IN_FLIGHT:
                     self.wait()
             finally:
                 self.queue.task_done()
         # Wait for all in-flight requests to complete after poison pill
+        self.logger.info(f"[{self.ext_id}] : {self.offsets}")
         self.wait(drain=True)
         self.close_cached_streams()
+        self.logger.info("Worker process exiting.")
         self.log_notifier.send("Worker process exiting.")
 
     def close_cached_streams(self) -> None:
         """Close all cached streams."""
         for _, stream, _ in self.cache.values():
             try:
                 stream.close()
@@ -236,14 +256,15 @@
 
 class StorageWriteProcessBatchWorker(StorageWriteBatchWorker, Process):
     pass
 
 
 class BigQueryStorageWriteSink(BaseBigQuerySink):
     MAX_WORKERS = os.cpu_count() * 2
+    MAX_JOBS_QUEUED = MAX_WORKERS * 2
     WORKER_CAPACITY_FACTOR = 10
     WORKER_CREATION_MIN_INTERVAL = 1.0
 
     @staticmethod
     def worker_cls_factory(
         worker_executor_cls: Type[Process], config: Dict[str, Any]
     ) -> Type[
@@ -272,15 +293,14 @@
         self.parent = BigQueryWriteClient.table_path(
             self.table.project,
             self.table.dataset,
             self.table.name,
         )
         self.stream_notification, self.stream_notifier = target.pipe_cls(False)
         self.template = generate_template(self.proto_schema)
-        self.offset = 0
 
     @property
     def proto_schema(self) -> Type[Message]:
         if not hasattr(self, "_proto_schema"):
             self._proto_schema = proto_schema_factory_v2(
                 self.table.get_resolved_schema(self.apply_transforms)
             )
@@ -296,25 +316,27 @@
 
     def process_record(self, record: Dict[str, Any], context: Dict[str, Any]) -> None:
         self.proto_rows.serialized_rows.append(
             json_format.ParseDict(record, self.proto_schema()).SerializeToString()
         )
 
     def process_batch(self, context: Dict[str, Any]) -> None:
+        while self.global_queue.qsize() >= self.MAX_JOBS_QUEUED:
+            self.logger.warn(f"Max jobs enqueued reached ({self.MAX_JOBS_QUEUED})")
+            sleep(1)
+        
         self.global_queue.put(
             Job(
                 parent=self.parent,
                 template=self.template,
                 data=self.proto_rows,
                 stream_notifier=self.stream_notifier,
-                offset=self.offset,
             )
         )
         self.increment_jobs_enqueued()
-        self.offset += len(self.proto_rows.serialized_rows)
 
     def commit_streams(self) -> None:
         while self.stream_notification.poll():
             stream_payload = self.stream_notification.recv()
             self.logger.debug("Stream enqueued %s", stream_payload)
             self.open_streams.add(stream_payload)
         if not self.open_streams:
```

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/streaming_insert.py` & `z3_target_bigquery-0.6.7/target_bigquery/streaming_insert.py`

 * *Files identical despite different names*

### Comparing `z3_target_bigquery-0.6.6/target_bigquery/target.py` & `z3_target_bigquery-0.6.7/target_bigquery/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # without restriction, including without limitation the rights to use, copy, modify, merge,
 # publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons
 # to whom the Software is furnished to do so, subject to the following conditions:
 #
 # The above copyright notice and this permission notice shall be included in all copies or
 # substantial portions of the Software.
 """BigQuery target class."""
+import os
 import copy
 import time
 import uuid
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple, Type, Union
 
 from singer_sdk import Sink
 from singer_sdk import typing as th
@@ -33,23 +34,26 @@
 if TYPE_CHECKING:
     from multiprocessing import Process, Queue
     from multiprocessing.connection import Connection
 
 # Defaults for target worker pool parameters
 MAX_WORKERS = 15
 """Maximum number of workers to spawn."""
+MAX_JOBS_QUEUED = 30
+"""Maximum number of jobs placed in the global queue to avoid memory overload."""
 WORKER_CAPACITY_FACTOR = 5
 """Jobs enqueued must exceed the number of active workers times this number."""
 WORKER_CREATION_MIN_INTERVAL = 5
 """Minimum time between worker creation attempts."""
 
-
 class TargetBigQuery(Target):
     """Target for BigQuery."""
 
+    _MAX_RECORD_AGE_IN_MINUTES = 5.0
+    
     name = "target-bigquery"
     config_jsonschema = th.PropertiesList(
         th.Property(
             "credentials_path",
             th.StringType,
             description="The path to a gcp credentials json file.",
         ),
@@ -480,14 +484,15 @@
         existing_sink = self._sinks_active.get(stream_name, None)
         if not existing_sink:
             return self.add_sink(stream_name, schema, key_properties)
         return existing_sink
 
     def drain_one(self, sink: Sink) -> None:  # type: ignore
         """Drain a sink. Includes a hook to manage the worker pool and notifications."""
+        #self.logger.info(f"Jobs queued : {self.queue.qsize()} | Max nb jobs queued : {os.cpu_count() * 4} | Nb workers : {len(self.workers)} | Max nb workers : {os.cpu_count() * 2}")
         self.resize_worker_pool()
         while self.job_notification.poll():
             ext_id = self.job_notification.recv()
             self.worker_pings[ext_id] = time.time()
             self._jobs_enqueued -= 1
         while self.log_notification.poll():
             msg = self.log_notification.recv()
@@ -515,16 +520,19 @@
         state = copy.deepcopy(self._latest_state)
         sink: BaseBigQuerySink
         self._drain_all(list(self._sinks_active.values()), self.max_parallelism)
         if is_endofpipe:
             for worker in self.workers:
                 if worker.is_alive():
                     self.queue.put(None)
-            for worker in self.workers:
+            while len(self.workers):
                 worker.join()
+                worker = self.workers.pop()
             for sink in self._sinks_active.values():
                 sink.clean_up()
         else:
+            for worker in self.workers:
+                worker.join()
             for sink in self._sinks_active.values():
                 sink.pre_state_hook()
         self._write_state_message(state)
         self._reset_max_record_age()
```

### Comparing `z3_target_bigquery-0.6.6/PKG-INFO` & `z3_target_bigquery-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3-target-bigquery
-Version: 0.6.6
+Version: 0.6.7
 Summary: z3-target-bigquery is a Singer target for BigQuery. It supports storage write, GCS, streaming, and batch load methods. Built with the Meltano SDK.
 Home-page: https://github.com/z3z1ma/target-bigquery
 License: MIT
 Keywords: ELT,BigQuery
 Author: Alex Butler
 Author-email: butler.alex2010@gmail.com
 Requires-Python: >=3.8,<3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: z3-target-bigquery Version: 0.6.6 Summary: z3-
+Metadata-Version: 2.1 Name: z3-target-bigquery Version: 0.6.7 Summary: z3-
 target-bigquery is a Singer target for BigQuery. It supports storage write,
 GCS, streaming, and batch load methods. Built with the Meltano SDK. Home-page:
 https://github.com/z3z1ma/target-bigquery License: MIT Keywords: ELT,BigQuery
 Author: Alex Butler Author-email: butler.alex2010@gmail.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 4 - Beta Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
```

