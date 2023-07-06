# Comparing `tmp/nhs_context_logging-0.2.4.tar.gz` & `tmp/nhs_context_logging-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_context_logging-0.2.4.tar", max compression
+gzip compressed data, was "nhs_context_logging-0.2.5.tar", max compression
```

## Comparing `nhs_context_logging-0.2.4.tar` & `nhs_context_logging-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1159 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/LICENSE.md
--rw-r--r--   0        0        0     7970 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/README.md
--rw-r--r--   0        0        0     1636 2023-06-25 21:14:44.034891 nhs_context_logging-0.2.4/nhs_context_logging/__init__.py
--rw-r--r--   0        0        0     1446 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/constants.py
--rw-r--r--   0        0        0     1076 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/fixtures.py
--rw-r--r--   0        0        0     5954 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/formatters.py
--rw-r--r--   0        0        0     1685 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/handlers.py
--rw-r--r--   0        0        0    34864 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/logger.py
--rw-r--r--   0        0        0        0 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/py.typed
--rw-r--r--   0        0        0     3830 2023-06-25 21:14:22.798491 nhs_context_logging-0.2.4/nhs_context_logging/utils.py
--rw-r--r--   0        0        0     2809 2023-06-25 21:14:44.030891 nhs_context_logging-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/__init__.py
--rw-r--r--   0        0        0      486 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0    36874 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/logger_tests.py
--rw-r--r--   0        0        0     4214 2023-06-25 21:14:22.802491 nhs_context_logging-0.2.4/tests/utils.py
--rw-r--r--   0        0        0     8392 1970-01-01 00:00:00.000000 nhs_context_logging-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1159 2023-07-06 19:26:13.111002 nhs_context_logging-0.2.5/LICENSE.md
+-rw-r--r--   0        0        0     7970 2023-07-06 19:26:13.111002 nhs_context_logging-0.2.5/README.md
+-rw-r--r--   0        0        0     1636 2023-07-06 19:26:34.556195 nhs_context_logging-0.2.5/nhs_context_logging/__init__.py
+-rw-r--r--   0        0        0     1453 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/constants.py
+-rw-r--r--   0        0        0     1076 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/fixtures.py
+-rw-r--r--   0        0        0     6063 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/formatters.py
+-rw-r--r--   0        0        0     1685 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/handlers.py
+-rw-r--r--   0        0        0    34935 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/logger.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/py.typed
+-rw-r--r--   0        0        0     3830 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/nhs_context_logging/utils.py
+-rw-r--r--   0        0        0     2808 2023-07-06 19:26:33.223993 nhs_context_logging-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/__init__.py
+-rw-r--r--   0        0        0      486 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0    38463 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/logger_tests.py
+-rw-r--r--   0        0        0     4214 2023-07-06 19:26:13.115002 nhs_context_logging-0.2.5/tests/utils.py
+-rw-r--r--   0        0        0     8392 1970-01-01 00:00:00.000000 nhs_context_logging-0.2.5/PKG-INFO
```

### Comparing `nhs_context_logging-0.2.4/LICENSE.md` & `nhs_context_logging-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.4/README.md` & `nhs_context_logging-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.4/nhs_context_logging/__init__.py` & `nhs_context_logging-0.2.5/nhs_context_logging/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from nhs_context_logging.logger import (
     LogActionContextManager,
     TemporaryGlobalFieldsContextManager,
 )
 from nhs_context_logging.logger import app_logger as _app_logger
 from nhs_context_logging.logger import logging_context
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 DEFAULT_LOG_LEVEL = Constants.DEFAULT_LOG_LEVEL
 LOG_AT_LEVEL = Constants.LOG_AT_LEVEL
 LOG_LEVEL = Constants.LOG_LEVEL
 
 CRITICAL = _app_logger.CRITICAL
 FATAL = _app_logger.FATAL
```

### Comparing `nhs_context_logging-0.2.4/nhs_context_logging/constants.py` & `nhs_context_logging-0.2.5/nhs_context_logging/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # The function executed successfully but an expected error was thrown (e.g. a validation exception)
     STATUS_ERROR = "error"
     # The function raised an unexpected exception
     STATUS_FAILED = "failed"
 
     LOG_REFERENCE_FIELD = "log_reference"
     LOG_REFERENCE_ON_ERR_FIELD = "log_reference_on_error"
-    INTERNAL_ID_FIELD = "internal_id"
+    LOG_CORRELATION_ID_FIELD = "internal_id"
     TIMESTAMP_FIELD = "timestamp"
     TRACEBACK_FIELD = "traceback"
     EXCEPTION_FIELD = "exception"
     LOG_INFO = "log_info"
     STACK_INFO = "stack_info"
 
     MESSAGE_TYPE_FIELD = "message_type"
```

### Comparing `nhs_context_logging-0.2.4/nhs_context_logging/fixtures.py` & `nhs_context_logging-0.2.5/nhs_context_logging/fixtures.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.4/nhs_context_logging/formatters.py` & `nhs_context_logging-0.2.5/nhs_context_logging/formatters.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def format(self, record: logging.LogRecord) -> dict:  # type: ignore[override]
 
         log: Dict[str, Any] = {}
 
         log.update(
             {
-                "timestamp": datetime.fromtimestamp(record.created).timestamp(),
+                Constants.TIMESTAMP_FIELD: datetime.fromtimestamp(record.created).timestamp(),
             }
         )
 
         log_args: Dict[str, Any] = {}
         if record.args:
 
             args = record.args
@@ -53,31 +53,31 @@
             if isinstance(args, list) and callable(args[0]):
                 args = args[0]()
             if not isinstance(args, dict):
                 args = dict(args=record.args)
 
             if args:
 
-                rec_ts = cast(float, args.get("timestamp"))
+                rec_ts = cast(float, args.get(Constants.TIMESTAMP_FIELD))
                 if rec_ts:
-                    args["timestamp"] = datetime.fromtimestamp(rec_ts).timestamp()
+                    args[Constants.TIMESTAMP_FIELD] = datetime.fromtimestamp(rec_ts).timestamp()
 
                 log_args.update(args)
 
-        if "expected_errors" in log_args:
-            del log_args["expected_errors"]
+        if Constants.EXPECTED_ERRORS in log_args:
+            del log_args[Constants.EXPECTED_ERRORS]
 
         include_traceback = log_args.get(Constants.INCLUDE_TRACEBACK, True)
         if Constants.INCLUDE_TRACEBACK in log_args:
             del log_args[Constants.INCLUDE_TRACEBACK]
 
-        if "redact_fields" in log_args:
-            del log_args["redact_fields"]
+        if Constants.REDACT_FIELDS in log_args:
+            del log_args[Constants.REDACT_FIELDS]
 
-        for priority_field in ("log_reference", "internal_id"):
+        for priority_field in (Constants.LOG_REFERENCE_FIELD, Constants.LOG_CORRELATION_ID_FIELD):
 
             field_value = log_args.pop(priority_field, None)
             if field_value:
                 log[priority_field] = field_value
 
         log.update(log_args)
```

### Comparing `nhs_context_logging-0.2.4/nhs_context_logging/handlers.py` & `nhs_context_logging-0.2.5/nhs_context_logging/handlers.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.4/nhs_context_logging/logger.py` & `nhs_context_logging-0.2.5/nhs_context_logging/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,15 +560,15 @@
 
     @property
     def log_level(self):
         return self.fields.get(Constants.LOG_LEVEL, Constants.DEFAULT_LOG_LEVEL)
 
     @property
     def internal_id(self) -> str:
-        return str(self.fields[Constants.INTERNAL_ID_FIELD])
+        return str(self.fields[Constants.LOG_CORRELATION_ID_FIELD])
 
     @property
     def log_reference(self):
         return self.fields.get(Constants.LOG_REFERENCE_FIELD)
 
     def add_fields(self, **fields):
         if not fields:
@@ -583,18 +583,18 @@
         requested_log_level = self.fields.get(Constants.LOG_AT_LEVEL)
         if requested_log_level is not None:
             del self.fields[Constants.LOG_AT_LEVEL]
             logging_context.force_log_at_level(requested_log_level)
 
         self.fields[Constants.LOG_LEVEL] = self.fields.get(Constants.LOG_LEVEL, Constants.DEFAULT_LOG_LEVEL)
 
-        if Constants.INTERNAL_ID_FIELD not in self.fields:
+        if Constants.LOG_CORRELATION_ID_FIELD not in self.fields:
             last_task = logging_context.current()
             internal_id = last_task.internal_id if last_task else LogActionContextManager.internal_id_factory()
-            self.fields[Constants.INTERNAL_ID_FIELD] = internal_id
+            self.fields[Constants.LOG_CORRELATION_ID_FIELD] = internal_id
 
         self.start_time = time()
 
         logging_context.push(self)
 
     def _end_action(self, exc_type, exc_val, exc_tb):
 
@@ -608,15 +608,15 @@
         self.end_time = time()
 
         if self.end_time is not None and self.start_time is not None:
             message[Constants.ACTION_DURATION] = message.get(
                 Constants.ACTION_DURATION, float(f"{(self.end_time - self.start_time):0.7f}")
             )
 
-        if exc_val:
+        if exc_val and not isinstance(exc_val, GeneratorExit):
             self._add_error_fields(message, exc_type, exc_val, exc_tb)
         else:
             message[Constants.ACTION_STATUS] = Constants.STATUS_SUCCEEDED
         message.pop(Constants.LOG_REFERENCE_ON_ERR_FIELD, None)
         logging_context.emit_message(message)
 
         return False
@@ -927,15 +927,15 @@
     def get_context_fields(self):
 
         fields = {}
         fields.update(self.current_global_fields)
         current_context = self.current()
         if not current_context:
             return fields
-        fields[Constants.INTERNAL_ID_FIELD] = current_context.internal_id
+        fields[Constants.LOG_CORRELATION_ID_FIELD] = current_context.internal_id
         return fields
 
     @staticmethod
     def add_app_globals(**kwargs):
         if kwargs:
             _app_globals.update(kwargs)
```

### Comparing `nhs_context_logging-0.2.4/nhs_context_logging/utils.py` & `nhs_context_logging-0.2.5/nhs_context_logging/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.4/pyproject.toml` & `nhs_context_logging-0.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nhs_context_logging"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["spinecore"]
 license = "GPLv3"
 packages = [
     { include = "nhs_context_logging" },
     { include = "tests", format = "sdist" },
 ]
@@ -138,15 +138,15 @@
     which python
     which pytest
     pytest
 """
 
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 metadata = false
 vcs = "git"
 style = "pep440"
 format-jinja = """
     {%- if distance == 0 -%}
         {{ serialize_pep440(base, stage, revision) }}
     {%- else -%}
```

### Comparing `nhs_context_logging-0.2.4/tests/logger_tests.py` & `nhs_context_logging-0.2.5/tests/logger_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import json
 import logging
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from functools import wraps
-from typing import Any, Callable, Generator, Optional, TypeVar, cast
+from typing import Any, Callable, Generator, List, Optional, Tuple, TypeVar, cast
 from uuid import uuid4
 
 import pytest
 
 from nhs_context_logging import (
     INFO,
     TemporaryGlobalFieldsContextManager,
@@ -26,15 +26,15 @@
     JSONFormatter,
     KeyValueFormatter,
     StructuredFormatter,
 )
 from tests.utils import concurrent_tasks, create_task, run_in_executor
 
 
-def assert_single_internal_id(log_capture: tuple):
+def assert_single_internal_id(log_capture: Tuple[List[dict], List[dict]]):
     internal_ids = {line["internal_id"] for line in (log_capture[0] + log_capture[1])}
     assert len(internal_ids) == 1, internal_ids
 
 
 @dataclass
 class MyModel:
     name: str
@@ -110,25 +110,25 @@
 
     std_out, _ = log_capture
     assert len(std_out) == 1
     assert std_out[0]["action"] == do_a_thing.__name__
     assert std_out[0]["internal_id"] != "bob"
 
 
-def test_logging_simple(log_capture: tuple):
+def test_logging_simple(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     app_logger.info(lambda: dict(test=123))
 
     assert len(std_out) == 1
     assert len(std_err) == 0
     assert std_out[0]["test"] == 123
 
 
-def test_logging_simple_is_lazy(log_capture: tuple):
+def test_logging_simple_is_lazy(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     prev_level = app_logger.log_at_level
 
     try:
         app_logger.log_at_level = logging.WARN
 
@@ -143,25 +143,25 @@
         assert len(std_out) == 0
         assert len(std_err) == 0
         assert len(calls) == 0
     finally:
         app_logger.log_at_level = prev_level
 
 
-def test_logging_default_logger(log_capture: tuple):
+def test_logging_default_logger(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
     level = logging.root.level
     logging.root.setLevel(INFO)
     logging.info("test")
     logging.root.setLevel(level)
     assert len(std_err) == 0
     assert std_out[0]["message"] == "test"
 
 
-def test_log_exception(log_capture: tuple):
+def test_log_exception(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     try:
         raise ValueError("testing")
     except ValueError:
         app_logger.exception(lambda: dict(things=123))
 
@@ -175,15 +175,15 @@
     assert err["error_info"]["fq_type"] == "builtins.ValueError"
     assert isinstance(err["error_info"]["line_no"], int)
     assert err["error_info"]["line_no"] > 0
     assert "traceback" in err["error_info"]
     assert 'raise ValueError("testing")' in err["error_info"]["traceback"]
 
 
-def test_with_action_logging(log_capture: tuple):
+def test_with_action_logging(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     with log_action(field=123):
         num = 1 + 1
 
         add_fields(num=num)
 
@@ -194,15 +194,15 @@
 
     assert log["num"] == 2
     assert log["field"] == 123
 
     assert "internal_id" in log
 
 
-def test_with_action_logging_exploded_model(log_capture: tuple):
+def test_with_action_logging_exploded_model(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     with log_action(field=MyModel(name="vic")):
         num = 1 + 1
 
         add_fields(num=num)
 
@@ -215,15 +215,15 @@
 
     assert isinstance(log["field"], dict), "Model was not exploded to primitive form!"
     assert log["field"]["name"] == "vic"
 
     assert "internal_id" in log
 
 
-def test_with_action_logging_exploded_model_added_after(log_capture: tuple):
+def test_with_action_logging_exploded_model_added_after(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     with log_action(field=123):
         add_fields(obj=MyModel(name="vic"))
 
     assert len(std_err) == 0
     assert len(std_out) == 1
@@ -234,15 +234,15 @@
 
     assert isinstance(log["obj"], dict), "Model was not exploded to primitive form!"
     assert log["obj"]["name"] == "vic"
 
     assert "internal_id" in log
 
 
-def test_with_action_logging_exception(log_capture: tuple):
+def test_with_action_logging_exception(log_capture: Tuple[List[dict], List[dict]]):
     _, std_err = log_capture
 
     try:
 
         with log_action(field=123):
 
             num = 1 + 1
@@ -260,15 +260,15 @@
 
     assert log["num"] == 2
     assert log["field"] == 123
 
     assert "internal_id" in log
 
 
-def test_log_action(log_capture: tuple):
+def test_log_action(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action()
     @some_logging_decorator()
     def test_function():
         add_fields(field=123)
 
@@ -280,15 +280,15 @@
 
     assert log["field"] == 123
 
     assert log["action"] == "test_function"
     assert log["action_status"] == "succeeded"
 
 
-def test_log_action_with_args(log_capture: tuple):
+def test_log_action_with_args(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(log_args=["_bob"])
     @some_logging_decorator(some_arg=2)
     def test_function(_bob):
         add_fields(field=123)
 
@@ -302,15 +302,15 @@
 
     assert log["action"] == "test_function"
     assert log["action_status"] == "succeeded"
 
     assert log["_bob"] == "vic"
 
 
-def test_log_action_with_model_exploded(log_capture: tuple):
+def test_log_action_with_model_exploded(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(log_args=["_bob"])
     def test_function(_bob):
         add_fields(field=123)
 
     test_function(MyModel(name="vic"))
@@ -324,15 +324,15 @@
     assert log["action"] == "test_function"
     assert log["action_status"] == "succeeded"
 
     assert isinstance(log["_bob"], dict), "Model was not exploded to primitive form!"
     assert log["_bob"]["name"] == "vic"
 
 
-def test_log_action_with_named_action(log_capture: tuple):
+def test_log_action_with_named_action(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(action="test", log_args=["_bob"])
     def test_function(_bob):
         add_fields(field=123)
 
     test_function("vic")
@@ -345,15 +345,15 @@
 
     assert log["action"] == "test"
     assert log["action_status"] == "succeeded"
 
     assert log["_bob"] == "vic"
 
 
-def test_log_action_exception(log_capture: tuple):
+def test_log_action_exception(log_capture: Tuple[List[dict], List[dict]]):
     _, std_err = log_capture
 
     @log_action()
     def test_function():
         add_fields(field=123)
         raise ValueError("eek")
 
@@ -368,15 +368,15 @@
 
     assert log["field"] == 123
 
     assert log["action"] == "test_function"
     assert log["action_status"] == "failed"
 
 
-async def test_async_logging_context_concurrent(log_capture: tuple):
+async def test_async_logging_context_concurrent(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action()
     async def my_coro2(task_id: str):
         res = await asyncio.gather(
             *[
                 my_coro(f"{task_id}-task1", 1),
@@ -400,15 +400,15 @@
 
     assert len(std_err) == 0
     assert len(std_out) > 1
 
     assert_single_internal_id(log_capture)
 
 
-async def test_async_logging_context_linear(log_capture: tuple):
+async def test_async_logging_context_linear(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action()
     async def my_coro2(task_id: str):
         print(f"starting task {task_id}")
         res = await my_coro("task3", 0.25)
         print(f"ending task {task_id}")
@@ -427,15 +427,15 @@
 
     assert len(std_err) == 0
     assert len(std_out) == 2
 
     assert_single_internal_id(log_capture)
 
 
-async def test_async_logging_context_concurrent_tasks(log_capture: tuple):
+async def test_async_logging_context_concurrent_tasks(log_capture: Tuple[List[dict], List[dict]]):
     @log_action()
     async def my_coro2(task_id: str):
         print(f"starting task {task_id}")
         res = await asyncio.gather(
             *[
                 await create_task(my_coro, "task1", 1),
                 await create_task(my_coro, "task2", 0.5),
@@ -463,15 +463,15 @@
             await create_task(my_coro2, "2task4"),
         ]
     )
 
     assert_single_internal_id(log_capture)
 
 
-def test_concurrent_logging_context(log_capture: tuple):
+def test_concurrent_logging_context(log_capture: Tuple[List[dict], List[dict]]):
     global_id = uuid4().hex
 
     @log_action()
     def my_task(task_id: str, wait: float):
         print(f"starting task {task_id}")
         time.sleep(wait)
         print(f"ending task {task_id}")
@@ -495,15 +495,15 @@
     assert_single_internal_id(log_capture)
 
     my_io_global_id = {line["global_id"] for line in std_out if line["action"] == "my_task"}
     assert len(my_io_global_id) == 1
     assert my_io_global_id == {global_id}
 
 
-def test_generator(log_capture: tuple):
+def test_generator(log_capture: Tuple[List[dict], List[dict]]):
     @log_action()
     def inner_action() -> str:
         action = logging_context.current()
         return action.internal_id
 
     @log_action()
     def generator_action(count: int) -> Generator[str, None, None]:
@@ -517,15 +517,30 @@
         return action.internal_id, res
 
     outer_action()
 
     assert_single_internal_id(log_capture)
 
 
-async def test_async_logging_context_run_in_executor(log_capture: tuple):
+async def test_generator_exit(log_capture: Tuple[List[dict], List[dict]], tmp_path):
+    @log_action()
+    async def outer_action():
+        raise GeneratorExit()
+
+    with pytest.raises(GeneratorExit):
+        await outer_action()
+
+    assert_single_internal_id(log_capture)
+    std_out, std_err = log_capture
+    assert len(std_err) == 0
+    assert len(std_out) == 1
+    assert std_out[0]["log_info"]["level"] == "INFO"
+
+
+async def test_async_logging_context_run_in_executor(log_capture: Tuple[List[dict], List[dict]]):
     logging_context.setup_async()
     global_id = uuid4().hex
 
     std_out, std_err = log_capture
 
     @log_action()
     async def my_coro2(task_id: str):
@@ -612,30 +627,30 @@
     assert "log_info_path" in formatted
     assert " internal_id=testid " in formatted
     assert " list_type=1,2,3 " in formatted
     assert " nested_list=4,5,6 " in formatted
     assert " nested_key=secret" in formatted
 
 
-def test_sync_context(log_capture: tuple):
+def test_sync_context(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(log_reference="bob")
     def s_function(aaa):
         app_logger.info("smiddle")
         return aaa
 
     res = s_function(1)
     assert res == 1
 
     assert std_out[0]["message"] == "smiddle"
     assert std_out[-1]["log_reference"] == "bob"
 
 
-def test_default_redaction(log_capture: tuple):
+def test_default_redaction(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(log_reference="bob", nhs_number="yes", password="yes")
     def s_function(aaa):
         app_logger.info("smiddle")
         return aaa
 
@@ -644,15 +659,15 @@
 
     assert std_out[0]["message"] == "smiddle"
     assert std_out[-1]["log_reference"] == "bob"
     assert std_out[-1]["nhs_number"] == "--REDACTED--"
     assert std_out[-1]["password"] == "--REDACTED--"
 
 
-def test_default_redaction_exclusion(log_capture: tuple):
+def test_default_redaction_exclusion(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(log_reference="bob", nhs_number="yes", password="yes", dont_redact={"nhs_number"})
     def s_function(aaa):
         app_logger.info("smiddle")
         return aaa
 
@@ -661,15 +676,15 @@
 
     assert std_out[0]["message"] == "smiddle"
     assert std_out[-1]["log_reference"] == "bob"
     assert std_out[-1]["nhs_number"] == "yes"
     assert std_out[-1]["password"] == "--REDACTED--"
 
 
-def test_sync_generator(log_capture: tuple):
+def test_sync_generator(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(log_reference="test")
     def sgen_function(count):
         for i in range(count):
             app_logger.info(f"{i}middle")
             yield i
@@ -678,15 +693,15 @@
     assert len(res) == 3
 
     messages = [log["message"] for log in std_out if "message" in log]
     assert messages == ["0middle", "1middle", "2middle"]
     assert std_out[-1]["log_info"]["func"] == "test_sync_generator"
 
 
-async def test_async_context(log_capture: tuple):
+async def test_async_context(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action()
     async def a_function(aaa):
         app_logger.info("amiddle")
         return aaa
 
@@ -694,15 +709,15 @@
     assert res == 1
 
     messages = [log["message"] for log in std_out if "message" in log]
     assert messages == ["amiddle"]
     assert std_out[-1]["log_info"]["func"] == "test_async_context"
 
 
-async def test_async_generator(log_capture: tuple):
+async def test_async_generator(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action()
     async def asg_function(count):
         total = 0
         for i in range(count):
             app_logger.info(f"{i}middle")
@@ -715,15 +730,15 @@
 
     messages = [log["message"] for log in std_out if "message" in log]
     assert messages == ["0middle", "1middle", "2middle"]
     assert std_out[-1]["total"] == 3
     assert std_out[-1]["log_info"]["func"] == "test_async_generator"
 
 
-def test_sync_generator_context_manager(log_capture: tuple):
+def test_sync_generator_context_manager(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     def sg_function(count):
         total = 0
         for i in range(count):
             app_logger.info(f"{i}middle")
             total += 1
@@ -746,29 +761,29 @@
     refs = [log["internal_id"] for log in std_out[:-1]]
     assert set(refs) == {std_out[-2]["internal_id"]}
 
     messages = [log["message"] for log in std_out if "message" in log]
     assert messages == ["0middle", "1middle", "2middle", "fin"]
 
 
-async def test_add_fields_can_change_log_level(log_capture: tuple):
+async def test_add_fields_can_change_log_level(log_capture: Tuple[List[dict], List[dict]]):
     std_out, _ = log_capture
 
     @log_action(log_level=logging.NOTSET)
     async def a_function():
         add_fields(log_level=logging.INFO)
 
     await a_function()
 
     assert len(std_out) == 1
     assert std_out[0]["log_info"]["level"] == "INFO"
 
 
 @pytest.mark.skip
-async def test_async_generator_resolved_later(log_capture: tuple):
+async def test_async_generator_resolved_later(log_capture: Tuple[List[dict], List[dict]]):
     _, _ = log_capture
 
     async def asg_function(count):
         total = 0
         for i in range(count):
             app_logger.info(f"{i}middle")
             total += 1
@@ -780,72 +795,72 @@
         async with temporary_global_fields(test_global=123):
             return asg_function(3)
 
     gen = await outer_func()
     _ = [num async for num in gen]
 
 
-def test_logger_kwargs(log_capture: tuple):
+def test_logger_kwargs(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     app_logger.info(log_reference="MESH1234", another="test")
 
     assert len(std_err) == 0
     assert len(std_out) == 1
 
     log = std_out[0]
 
     assert log["log_reference"] == "MESH1234"
     assert log["another"] == "test"
 
 
-def test_logger_args_and_kwargs(log_capture: tuple):
+def test_logger_args_and_kwargs(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     app_logger.info(dict(test=1234), log_reference="MESH1234", test=0)
 
     assert len(std_err) == 0
     assert len(std_out) == 1
 
     log = std_out[0]
 
     assert log["log_reference"] == "MESH1234"
     assert log["test"] == 1234
 
 
-def test_logger_message_and_kwargs(log_capture: tuple):
+def test_logger_message_and_kwargs(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     app_logger.info("test", log_reference="MESH1234", test=0, message="test2")
 
     assert len(std_err) == 0
     assert len(std_out) == 1
 
     log = std_out[0]
 
     assert log["log_reference"] == "MESH1234"
     assert log["test"] == 0
     assert log["message"] == "test"
 
 
-def test_logger_list_args_and_kwargs(log_capture: tuple):
+def test_logger_list_args_and_kwargs(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     app_logger.info(123, log_reference="MESH1234", message="test2")
 
     assert len(std_err) == 0
     assert len(std_out) == 1
 
     log = std_out[0]
 
     assert "log_reference" not in log
     assert "message" not in log
 
 
-def test_logger_callable_args_and_kwargs(log_capture: tuple):
+def test_logger_callable_args_and_kwargs(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     def get_args():
         return dict(message=1234, thing="bob")
 
     app_logger.info(get_args, log_reference="MESH1234")
 
@@ -855,15 +870,15 @@
     log = std_out[0]
 
     assert log["thing"] == "bob"
     assert log["message"] == 1234
     assert "log_reference" in log
 
 
-def test_expected_errors(log_capture: tuple):
+def test_expected_errors(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action(action="ex_test", expected_errors=(ValueError,))
     def error_function(raise_value_error):
         if raise_value_error:
             raise ValueError("test")
 
@@ -889,15 +904,15 @@
     assert len(std_out) == 1
     log = std_out[0]
     assert log["action"] == "ex_test"
     assert log["log_info"]["level"] == "INFO"
     assert log["action_status"] == "error"
 
 
-def test_expected_errors_subclass(log_capture: tuple):
+def test_expected_errors_subclass(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     class SubValueError(ValueError):
         pass
 
     @log_action(action="ex_test", expected_errors=(ValueError,))
     def error_function(raise_value_error):
@@ -926,15 +941,15 @@
     assert len(std_out) == 1
     log = std_out[0]
     assert log["action"] == "ex_test"
     assert log["log_info"]["level"] == "INFO"
     assert log["action_status"] == "error"
 
 
-def test_expected_errors_raise_log_level_to_info(log_capture: tuple):
+def test_expected_errors_raise_log_level_to_info(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action(action="ex_test", log_level=logging.DEBUG, expected_errors=(ValueError,))
     def error_function():
         raise ValueError("test")
 
     with pytest.raises(ValueError):
@@ -944,15 +959,15 @@
     assert len(std_out) == 1
     log = std_out[0]
     assert log["action"] == "ex_test"
     assert log["log_info"]["level"] == "INFO"
     assert log["action_status"] == "error"
 
 
-def test_expected_errors_specific_levels(log_capture: tuple):
+def test_expected_errors_specific_levels(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action(
         action="ex_test",
         log_level=logging.DEBUG,
         expected_errors=(ValueError,),
         error_levels=((ValueError, logging.DEBUG),),
@@ -967,15 +982,15 @@
     assert len(std_out) == 1
     log = std_out[0]
     assert log["action"] == "ex_test"
     assert log["log_info"]["level"] == "DEBUG"
     assert log["action_status"] == "error"
 
 
-def test_expected_errors_raise_doesnt_lower_log_level(log_capture: tuple):
+def test_expected_errors_raise_doesnt_lower_log_level(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action(action="ex_test", log_level=logging.WARN, expected_errors=(ValueError,))
     def error_function():
         raise ValueError("test")
 
     with pytest.raises(ValueError):
@@ -985,15 +1000,15 @@
     assert len(std_out) == 1
     log = std_out[0]
     assert log["action"] == "ex_test"
     assert log["log_info"]["level"] == "WARNING"
     assert log["action_status"] == "error"
 
 
-def test_expected_errors_global_fields(log_capture: tuple):
+def test_expected_errors_global_fields(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action(action="ex_test")
     def error_function(raise_value_error):
         if raise_value_error:
             raise ValueError("test")
 
@@ -1013,15 +1028,15 @@
     assert log["log_info"]["level"] == "INFO"
     assert log["action_status"] == "error"
     assert log["error_info"]["type"] == "ValueError"
     assert log["error_info"]["fq_type"] == "builtins.ValueError"
     assert log["error_info"]["args"] == ("test",)
 
 
-def test_expected_errors_in_both(log_capture: tuple):
+def test_expected_errors_in_both(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action(action="ex_test", expected_errors=(NotImplementedError,))
     def error_function(raise_value_error):
         if raise_value_error:
             raise ValueError("test")
 
@@ -1059,15 +1074,15 @@
     assert log["action"] == "ex_test"
     assert log["log_info"]["level"] == "INFO"
     assert log["action_status"] == "error"
     assert log["error_info"]["type"] == "NotImplementedError"
     assert log["error_info"]["fq_type"] == "builtins.NotImplementedError"
 
 
-async def test_expected_errors_run_in_executor(log_capture: tuple):
+async def test_expected_errors_run_in_executor(log_capture: Tuple[List[dict], List[dict]]):
     logging_context.setup_async()
 
     std_out, std_err = log_capture
 
     @log_action(
         action="ex_test",
     )
@@ -1127,15 +1142,15 @@
 class _HTTPException(Exception):
     def __init__(self, status_code: int, detail: Optional[str] = None) -> None:
         super().__init__()
         self.status_code = status_code
         self.detail = detail
 
 
-def test_expected_errors_complex_exception(log_capture: tuple):
+def test_expected_errors_complex_exception(log_capture: Tuple[List[dict], List[dict]]):
     std_out, std_err = log_capture
 
     @log_action(expected_errors=(_HTTPException,))
     def error_function():
         raise _HTTPException(status_code=123, detail=dict(test=1234))
 
     with pytest.raises(_HTTPException) as ex:
@@ -1180,15 +1195,15 @@
     assert result == list(range(10))
 
     func = tgfcm(coro)
     result = await func("vic")
     assert result == "vic"
 
 
-async def test_async_sync_concurrent_tasks_transfer(log_capture: tuple):
+async def test_async_sync_concurrent_tasks_transfer(log_capture: Tuple[List[dict], List[dict]]):
     logging_context.setup_async()
 
     @log_action()
     def my_task():
         return "from task"
 
     @log_action()
@@ -1214,15 +1229,15 @@
 
     for line in std_out:
         print(line)
 
     assert_single_internal_id(log_capture)
 
 
-async def test_async_to_run_in_executor_sync(log_capture: tuple):
+async def test_async_to_run_in_executor_sync(log_capture: Tuple[List[dict], List[dict]]):
     logging_context.setup_async()
 
     global_id = uuid4().hex
 
     std_out, std_err = log_capture
 
     @log_action()
@@ -1262,15 +1277,15 @@
 
     fn2_ids = {line["fn2_id"] for line in std_out if line["action"].startswith("sync_fn2")}
     assert len(fn2_ids) == 3
 
     assert_single_internal_id(log_capture)
 
 
-def test_log_action_exception_with_log_ref_override(log_capture: tuple):
+def test_log_action_exception_with_log_ref_override(log_capture: Tuple[List[dict], List[dict]]):
     _, std_err = log_capture
 
     @log_action(log_reference="BANANA", log_reference_on_error="PLUM")
     def test_function():
         add_fields(field=123)
         raise ValueError("eek")
 
@@ -1287,15 +1302,15 @@
 
     assert log["action"] == "test_function"
     assert log["action_status"] == "failed"
     assert log["log_reference"] == "PLUM"
     assert "log_reference_on_error" not in log
 
 
-def test_log_action_exception_with_log_ref_unset(log_capture: tuple):
+def test_log_action_exception_with_log_ref_unset(log_capture: Tuple[List[dict], List[dict]]):
     _, std_err = log_capture
 
     @log_action(log_reference="BANANA", log_reference_on_error=None)
     def test_function():
         add_fields(field=123)
         raise ValueError("eek")
 
@@ -1312,15 +1327,15 @@
 
     assert log["action"] == "test_function"
     assert log["action_status"] == "failed"
     assert "log_reference" not in log
     assert "log_reference_on_error" not in log
 
 
-def test_log_action_exception_with_log_ref_unset_on_log_ref(log_capture: tuple):
+def test_log_action_exception_with_log_ref_unset_on_log_ref(log_capture: Tuple[List[dict], List[dict]]):
     _, std_err = log_capture
 
     @log_action(log_reference_on_error="BANANA")
     def test_function():
         add_fields(field=123)
         raise ValueError("eek")
```

### Comparing `nhs_context_logging-0.2.4/tests/utils.py` & `nhs_context_logging-0.2.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_context_logging-0.2.4/PKG-INFO` & `nhs_context_logging-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhs-context-logging
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 License: GPLv3
 Author: spinecore
 Requires-Python: >=3.8.1
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

