# Comparing `tmp/robotcode_debugger-0.45.0.tar.gz` & `tmp/robotcode_debugger-0.46.0.tar.gz`

## Comparing `robotcode_debugger-0.45.0.tar` & `robotcode_debugger-0.46.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    49549 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     7540 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13753 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/README.md
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/pyproject.toml
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.45.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5813 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    24396 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    52858 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    10557 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12484 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15002 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13755 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/LICENSE.txt
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/README.md
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/pyproject.toml
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 robotcode_debugger-0.46.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/debugger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
+import asyncio
 import itertools
 import os
 import pathlib
 import re
 import threading
-import traceback
 import weakref
 from collections import deque
 from enum import Enum
 from pathlib import Path, PurePath
 from typing import (
     Any,
     Callable,
@@ -22,21 +22,24 @@
     NamedTuple,
     Optional,
     Set,
     Tuple,
     Union,
 )
 
+from robot.api.parsing import get_model
 from robot.errors import VariableError
-from robot.running import EXECUTION_CONTEXTS, Keyword
+from robot.output import LOGGER
+from robot.running import EXECUTION_CONTEXTS, Keyword, TestCase, TestSuite
 from robot.running.userkeyword import UserKeywordHandler
 from robot.utils import NormalizedDict
 from robot.variables import evaluate_expression
 from robotcode.core.event import event
 from robotcode.core.logging import LoggingDescriptor
+from robotcode.robot.utils import get_robot_version
 
 from .dap_types import (
     Breakpoint,
     ContinuedEvent,
     ContinuedEventBody,
     EvaluateArgumentContext,
     Event,
@@ -57,14 +60,24 @@
     StoppedReason,
     Thread,
     ValueFormat,
     Variable,
     VariablePresentationHint,
 )
 
+if get_robot_version() >= (6, 1):
+
+    def internal_evaluate_expression(expression: str, variable_store: Any) -> Any:
+        return evaluate_expression(expression, variable_store)
+
+else:
+
+    def internal_evaluate_expression(expression: str, variable_store: Any) -> Any:
+        return evaluate_expression(expression, variable_store.store)
+
 
 class Undefined:
     def __str__(self) -> str:
         return self.__repr__()
 
     def __repr__(self) -> str:
         return "<undefined>"
@@ -254,21 +267,23 @@
         self.last_fail_message: Optional[str] = None
         self.stop_on_entry = False
         self._debug = True
         self.terminated = False
         self.terminated_requested = False
         self.attached = False
         self.path_mappings: List[PathMapping] = []
+        self.server_loop: Optional[asyncio.AbstractEventLoop] = None
 
         self._keyword_to_evaluate: Optional[Callable[..., Any]] = None
         self._evaluated_keyword_result: Any = None
         self._evaluate_keyword_event = threading.Event()
         self._evaluate_keyword_event.set()
         self._after_evaluate_keyword_event = threading.Event()
         self._after_evaluate_keyword_event.set()
+        self.expression_mode = False
 
     @property
     def debug(self) -> bool:
         return self._debug
 
     @debug.setter
     def debug(self, value: bool) -> None:
@@ -335,14 +350,16 @@
             if send_event:
                 self.send_event(
                     self,
                     ContinuedEvent(
                         body=ContinuedEventBody(thread_id=self.main_thread.ident, all_threads_continued=True)
                     ),
                 )
+
+            self.requested_state = RequestedState.Nothing
             self.state = State.Running
             self.condition.notify_all()
 
     def pause_thread(self, thread_id: int) -> None:
         if self.main_thread is None or thread_id != self.main_thread.ident:
             raise InvalidThreadIdError(thread_id)
 
@@ -512,15 +529,15 @@
                 breakpoints = [v for v in self.breakpoints[source_path].breakpoints if v.line == line_no]
                 if len(breakpoints) > 0:
                     for point in breakpoints:
                         if point.condition is not None:
                             hit = False
                             try:
                                 vars = EXECUTION_CONTEXTS.current.variables.current
-                                hit = bool(evaluate_expression(vars.replace_string(point.condition), vars.store))
+                                hit = bool(internal_evaluate_expression(vars.replace_string(point.condition), vars))
                             except (SystemExit, KeyboardInterrupt):
                                 raise
                             except BaseException:
                                 hit = False
 
                             if not hit:
                                 return
@@ -555,14 +572,15 @@
                                         source=Source(path=str(source_path)),
                                         line=line_no,
                                     )
                                 ),
                             )
                             return
 
+                        self.requested_state = RequestedState.Nothing
                         self.state = State.Paused
                         self.send_event(
                             self,
                             StoppedEvent(
                                 body=StoppedEventBody(
                                     reason=StoppedReason.BREAKPOINT,
                                     thread_id=threading.current_thread().ident,
@@ -577,29 +595,29 @@
             and status == "FAIL"
             and any(
                 v
                 for v in self.exception_breakpoints
                 if v.filter_options and any(o for o in v.filter_options if o.filter_id in filter_id)
             )
         ):
+            self.requested_state = RequestedState.Nothing
             self.state = State.Paused
 
             self.send_event(
                 self,
                 StoppedEvent(
                     body=StoppedEventBody(
                         description=description,
                         reason=StoppedReason.EXCEPTION,
                         thread_id=threading.current_thread().ident,
                         all_threads_stopped=True,
                         text=text,
                     )
                 ),
             )
-            self.wait_for_running()
 
     def wait_for_running(self) -> None:
         if self.attached:
             while True:
                 with self.condition:
                     self.condition.wait_for(lambda: self.state in [State.Running, State.Stopped, State.CallKeyword])
 
@@ -611,17 +629,18 @@
                             self._keyword_to_evaluate = None
                     except (SystemExit, KeyboardInterrupt):
                         raise
                     except BaseException as e:
                         self._evaluated_keyword_result = e
                     finally:
                         self._evaluate_keyword_event.set()
-                        self._after_evaluate_keyword_event.wait(60)
+                        self._after_evaluate_keyword_event.wait(120)
 
                     continue
+
                 break
 
     def start_output_group(self, name: str, attributes: Dict[str, Any], type: Optional[str] = None) -> None:
         if self.group_output:
             source = attributes.get("source", None)
             line_no = attributes.get("lineno", None)
 
@@ -768,20 +787,23 @@
                 self.wait_for_running()
 
     def end_suite(self, name: str, attributes: Dict[str, Any]) -> None:
         if self.debug:
             status = attributes.get("status", "")
 
             if status == "FAIL":
-                self.process_end_state(
-                    status,
-                    {"failed_suite"},
-                    "Suite failed.",
-                    f"Suite failed{f': {v}' if (v:=attributes.get('message', None)) else ''}",
-                )
+                if self.server_loop:
+                    self.process_end_state(
+                        status,
+                        {"failed_suite"},
+                        "Suite failed.",
+                        f"Suite failed{f': {v}' if (v:=attributes.get('message', None)) else ''}",
+                    )
+
+                self.wait_for_running()
 
         source = attributes.get("source", None)
         line_no = attributes.get("lineno", 1)
         type = "SUITE"
 
         self.remove_stackframe_entry(name, type, source, line_no)
 
@@ -808,14 +830,16 @@
                 self.process_end_state(
                     status,
                     {"failed_test"},
                     "Test failed.",
                     f"Test failed{f': {v}' if (v:=attributes.get('message', None)) else ''}",
                 )
 
+                self.wait_for_running()
+
         source = attributes.get("source", None)
         line_no = attributes.get("lineno", 1)
         longname = attributes.get("longname", "")
         type = "TEST"
 
         self.remove_stackframe_entry(longname, type, source, line_no)
 
@@ -876,14 +900,16 @@
                 self.process_end_state(
                     status,
                     {"failed_keyword", *({"uncaught_failed_keyword"} if self.in_caughted_keyword() else {})},
                     "Keyword failed.",
                     f"Keyword failed: {self.last_fail_message}" if self.last_fail_message else "Keyword failed.",
                 )
 
+                self.wait_for_running()
+
         source = attributes.get("source", None)
         line_no = attributes.get("lineno", None)
         type = attributes.get("type", "KEYWORD")
         kwname = attributes.get("kwname", None)
 
         handler: Any = None
         if type in ["KEYWORD", "SETUP", "TEARDOWN"]:
@@ -934,52 +960,52 @@
                 if self.is_windows_path(mapping.local_root):
                     return pathlib.PureWindowsPath(mapping.local_root, relative_path)
 
                 return pathlib.PurePath(mapping.local_root, relative_path)
 
         return path
 
+    def source_from_entry(self, entry: StackFrameEntry) -> Optional[Source]:
+        if entry.source is not None and entry.is_file:
+            return Source(path=str(self.map_path_to_client(entry.source)), presentation_hint="normal")
+
+        return None
+
     def get_stack_trace(
         self,
         thread_id: int,
         start_frame: Optional[int] = None,
         levels: Optional[int] = None,
         format: Optional[StackFrameFormat] = None,
     ) -> StackTraceResult:
         if self.main_thread is None or thread_id != self.main_thread.ident:
             raise InvalidThreadIdError(thread_id)
 
         start_frame = start_frame or 0
         levels = start_frame + (levels or len(self.stack_frames))
 
-        def source_from_entry(entry: StackFrameEntry) -> Optional[Source]:
-            if entry.source is not None and entry.is_file:
-                return Source(path=str(self.map_path_to_client(entry.source)))
-
-            return None
-
         def yield_stack() -> Iterator[StackFrame]:
             for i, v in enumerate(itertools.islice(self.stack_frames, start_frame, levels)):
                 if v.stack_frames:
                     yield StackFrame(
                         id=v.id,
                         name=v.longname or v.kwname or v.name or v.type,
                         line=v.stack_frames[0].line if v.stack_frames[0].line is not None else 0,
                         column=v.stack_frames[0].column if v.stack_frames[0].column is not None else 1,
-                        source=source_from_entry(v.stack_frames[0]),
+                        source=self.source_from_entry(v.stack_frames[0]),
                         presentation_hint="normal" if v.stack_frames[0].is_file else "subtle",
                         module_id=v.libname,
                     )
                 if not v.top_hidden:
                     yield StackFrame(
                         id=v.id,
                         name=v.longname or v.kwname or v.name or v.type,
                         line=v.line if v.line is not None else 1,
                         column=v.column if v.column is not None else 1,
-                        source=source_from_entry(v),
+                        source=self.source_from_entry(v),
                         presentation_hint="normal" if v.is_file else "subtle",
                         module_id=v.libname,
                     )
 
         frames = list(yield_stack())
 
         return StackTraceResult(frames, len(self.stack_frames))
@@ -1210,91 +1236,143 @@
                     return EvaluateResult(repr(expression), repr(type(expression)))
 
             vars = (
                 (stack_frame.get_first_or_self().variables() or evaluate_context.variables.current)
                 if stack_frame is not None
                 else evaluate_context.variables._global
             )
+            if (
+                isinstance(context, EvaluateArgumentContext)
+                and context != EvaluateArgumentContext.REPL
+                or context != EvaluateArgumentContext.REPL.value
+                or self.expression_mode
+            ):
+                if expression.startswith("! "):
+                    splitted = self.SPLIT_LINE.split(expression[2:].strip())
 
-            if expression.startswith("! "):
-                splitted = self.SPLIT_LINE.split(expression[2:].strip())
+                    if splitted:
+                        variables: List[str] = []
+                        while len(splitted) > 1 and self.IS_VARIABLE_ASSIGNMENT_RE.match(splitted[0].strip()):
+                            var = splitted[0]
+                            splitted = splitted[1:]
+                            if var.endswith("="):
+                                var = var[:-1]
+                            variables.append(var)
+
+                        if splitted:
+
+                            def run_kw() -> Any:
+                                kw = Keyword(name=splitted[0], args=tuple(splitted[1:]), assign=tuple(variables))
+                                return kw.run(evaluate_context)
 
-                if splitted:
-                    variables: List[str] = []
-                    while len(splitted) > 1 and self.IS_VARIABLE_ASSIGNMENT_RE.match(splitted[0].strip()):
-                        var = splitted[0]
-                        splitted = splitted[1:]
-                        if var.endswith("="):
-                            var = var[:-1]
-                        variables.append(var)
+                            result = self.run_in_robot_thread(run_kw)
 
-                    if splitted:
+                elif self.IS_VARIABLE_RE.match(expression.strip()):
+                    try:
+                        result = vars.replace_scalar(expression)
+                    except VariableError:
+                        if context is not None and (
+                            isinstance(context, EvaluateArgumentContext)
+                            and (
+                                context
+                                in [
+                                    EvaluateArgumentContext.HOVER,
+                                    EvaluateArgumentContext.WATCH,
+                                ]
+                            )
+                            or context
+                            in [
+                                EvaluateArgumentContext.HOVER.value,
+                                EvaluateArgumentContext.WATCH.value,
+                            ]
+                        ):
+                            result = UNDEFINED
+                        else:
+                            raise
+                else:
+                    result = internal_evaluate_expression(vars.replace_string(expression), vars)
+            else:
+
+                def get_test_body_from_string(command: str) -> TestCase:
+                    suite_str = (
+                        "*** Test Cases ***\nDummyTestCase423141592653589793\n  "
+                        + ("\n  ".join(command.split("\n")) if "\n" in command else command)
+                    ) + "\n"
+
+                    model = get_model(suite_str)
+                    suite: TestSuite = TestSuite.from_model(model)
+                    return suite.tests[0]
+
+                def run_kw() -> Any:
+                    test = get_test_body_from_string(expression)
+                    result = None
+
+                    if len(test.body):
+                        for kw in test.body:
+                            with LOGGER.delayed_logging:
+                                try:
+                                    result = kw.run(evaluate_context)
+                                    if kw.assign:
+                                        result = None
+                                except (SystemExit, KeyboardInterrupt):
+                                    raise
+                                except BaseException:
+                                    result = None
+                                    break
+                                finally:
+                                    messages = LOGGER._log_message_cache or []
+                                    for msg in messages or ():
+                                        # hack to get and evaluate log level
+                                        listener: Any = next(iter(LOGGER), None)
+                                        if listener is None or listener._is_logged(msg.level):
+                                            self.log_message(
+                                                {"level": msg.level, "message": msg.message, "timestamp": msg.timestamp}
+                                            )
+                    return result
 
-                        def run_kw() -> Any:
-                            kw = Keyword(name=splitted[0], args=tuple(splitted[1:]), assign=tuple(variables))
-                            return kw.run(evaluate_context)
+                result = self.run_in_robot_thread(run_kw)
 
-                        with self.condition:
-                            self._keyword_to_evaluate = run_kw
-                            self._evaluated_keyword_result = None
+                if isinstance(result, BaseException):
+                    raise result
 
-                            self._evaluate_keyword_event.clear()
-                            self._after_evaluate_keyword_event.clear()
+        except (SystemExit, KeyboardInterrupt):
+            raise
+        except BaseException as e:
+            self._logger.exception(e)
+            raise
 
-                            old_state = self.state
-                            self.state = State.CallKeyword
-                            self.condition.notify_all()
+        return EvaluateResult(repr(result) if result is not None else "", repr(type(result)))
 
-                        try:
-                            self._evaluate_keyword_event.wait(60)
-                        finally:
-                            result = self._evaluated_keyword_result
+    def run_in_robot_thread(self, kw: Callable[[], Any]) -> Any:
+        with self.condition:
+            self._keyword_to_evaluate = kw
+            self._evaluated_keyword_result = None
 
-                            with self.condition:
-                                self._keyword_to_evaluate = None
-                                self._evaluated_keyword_result = None
+            self._evaluate_keyword_event.clear()
+            self._after_evaluate_keyword_event.clear()
 
-                                self.state = old_state
-                                self.condition.notify_all()
+            old_state = self.state
+            self.state = State.CallKeyword
+            self.condition.notify_all()
 
-                                self._after_evaluate_keyword_event.set()
+        try:
+            self._evaluate_keyword_event.wait(60)
+        finally:
+            result = self._evaluated_keyword_result
+
+            with self.condition:
+                self._keyword_to_evaluate = None
+                self._evaluated_keyword_result = None
 
-            elif self.IS_VARIABLE_RE.match(expression.strip()):
-                try:
-                    result = vars.replace_scalar(expression)
-                except VariableError:
-                    if context is not None and (
-                        isinstance(context, EvaluateArgumentContext)
-                        and (
-                            context
-                            in [
-                                EvaluateArgumentContext.HOVER,
-                                EvaluateArgumentContext.WATCH,
-                            ]
-                        )
-                        or context
-                        in [
-                            EvaluateArgumentContext.HOVER.value,
-                            EvaluateArgumentContext.WATCH.value,
-                        ]
-                    ):
-                        result = UNDEFINED
-                    else:
-                        raise
-            else:
-                result = evaluate_expression(vars.replace_string(expression), vars.store)
+                self.state = old_state
+                self.condition.notify_all()
 
-        except (SystemExit, KeyboardInterrupt):
-            raise
-        except BaseException as e:
-            self._logger.exception(e)
-            result = traceback.format_exc()
-            # result = e
+                self._after_evaluate_keyword_event.set()
 
-        return EvaluateResult(repr(result), repr(type(result)))
+            return result
 
     def set_variable(
         self, variables_reference: int, name: str, value: str, format: Optional[ValueFormat] = None
     ) -> SetVariableResult:
         entry = next(
             (
                 v
@@ -1308,15 +1386,15 @@
             context = entry.context()
             if context is not None:
                 variables = context.variables.current
 
                 if (name[2:-1] if self.IS_VARIABLE_RE.match(name) else name) not in variables:
                     raise NameError(f"Variable '{name}' not found.")
 
-                evaluated_value = evaluate_expression(variables.replace_string(value), variables.store)
+                evaluated_value = internal_evaluate_expression(variables.replace_string(value), variables)
                 variables[name] = evaluated_value
 
                 return SetVariableResult(repr(evaluated_value), repr(type(value)))
 
         raise ReferenceError("Invalid variable reference.")
 
     def set_exception_breakpoints(
```

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
         self._initialized = False
 
     @_logger.call
     def send_message(self, message: ProtocolMessage) -> None:
         body = as_json(message, compact=True).encode(self.CHARSET)
 
         header = (f"Content-Length: {len(body)}\r\n\r\n").encode("ascii")
-
         if self.write_transport is not None:
             msg = header + body
 
             if self._loop:
                 self.write_transport.write(msg)
 
     def send_error(
@@ -267,15 +266,15 @@
             except BaseException as e:
                 self._logger.exception(e)
                 self.send_error(
                     str(type(e).__name__),
                     message.seq,
                     message.command,
                     False,
-                    error_message=Message(format=f"{type(e).__name__}: {e}", show_user=True),
+                    error_message=Message(format=f"{type(e).__name__}: {e}"),
                 )
             finally:
                 with self._received_request_lock:
                     self._received_request.pop(message.seq, None)
 
         result.add_done_callback(done)
```

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/run.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,14 +187,15 @@
         Debugger.instance().stop_on_entry = stop_on_entry
         Debugger.instance().output_messages = output_messages
         Debugger.instance().output_log = output_log
         Debugger.instance().group_output = group_output
         Debugger.instance().output_timestamps = output_timestamps
         Debugger.instance().debug = debug
         Debugger.instance().set_main_thread(threading.current_thread())
+        Debugger.instance().server_loop = server.loop
         Debugger.instance().start()
 
         exit_code = 0
         try:
             from robotcode.runner.cli.robot import robot
 
             try:
```

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.46.0/src/robotcode/debugger/launcher/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,30 +133,30 @@
             supports_exception_filter_options=True,
         )
 
     @rpc_method(name="launch", param_type=LaunchRequestArguments)
     async def _launch(
         self,
         request: str,
-        python: str,
+        python: Optional[str] = None,
         cwd: str = ".",
         profiles: Optional[List[str]] = None,
         target: Optional[str] = None,
         paths: Optional[List[str]] = None,
         args: Optional[List[str]] = None,
         env: Optional[Dict[str, Optional[Any]]] = None,
         console: Optional[Literal["internalConsole", "integratedTerminal", "externalTerminal"]] = "integratedTerminal",
         name: Optional[str] = None,
         no_debug: Optional[bool] = None,
         robotPythonPath: Optional[List[str]] = None,  # noqa: N803
         launcherArgs: Optional[List[str]] = None,  # noqa: N803
         launcherTimeout: Optional[int] = None,  # noqa: N803
         debuggerArgs: Optional[List[str]] = None,  # noqa: N803
         debuggerTimeout: Optional[int] = None,  # noqa: N803
-        attachPython: Optional[bool] = False,  # noqa: N803
+        attachPython: Optional[bool] = True,  # noqa: N803
         attachPythonPort: Optional[int] = None,  # noqa: N803
         variables: Optional[Dict[str, Any]] = None,
         outputDir: Optional[str] = None,  # noqa: N803
         outputMessages: Optional[bool] = False,  # noqa: N803
         outputLog: Optional[bool] = False,  # noqa: N803
         outputTimestamps: Optional[bool] = False,  # noqa: N803
         groupOutput: Optional[bool] = False,  # noqa: N803
@@ -174,21 +174,19 @@
     ) -> None:
         from robotcode.core.utils.net import find_free_port
 
         connect_timeout = launcherTimeout or 10
 
         port = find_free_port(DEBUGGER_DEFAULT_PORT)
 
-        debugger_script = (
-            Path(Path(__file__).parent.parent) if self.debugger_script is None else Path(self.debugger_script)
-        )
+        debugger_script = ["-m", "robotcode.cli"] if self.debugger_script is None else [str(Path(self.debugger_script))]
 
         robotcode_run_args = [
-            python,
-            str(debugger_script),
+            python or sys.executable,
+            *debugger_script,
             *itertools.chain.from_iterable(["--profile", p] for p in profiles or []),
             *itertools.chain.from_iterable(["--default-path", p] for p in paths or []),
             *(robotCodeArgs or []),
             "debug",
         ]
 
         if no_debug:
```

### Comparing `robotcode_debugger-0.45.0/.gitignore` & `robotcode_debugger-0.46.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/LICENSE.txt` & `robotcode_debugger-0.46.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/README.md` & `robotcode_debugger-0.46.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.45.0/pyproject.toml` & `robotcode_debugger-0.46.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.45.0",
-  "robotcode-runner==0.45.0",
+  "robotcode-jsonrpc2==0.46.0",
+  "robotcode-runner==0.46.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
```

### Comparing `robotcode_debugger-0.45.0/PKG-INFO` & `robotcode_debugger-0.46.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-debugger
-Version: 0.45.0
+Version: 0.46.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.45.0
-Requires-Dist: robotcode-runner==0.45.0
+Requires-Dist: robotcode-jsonrpc2==0.46.0
+Requires-Dist: robotcode-runner==0.46.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
```

