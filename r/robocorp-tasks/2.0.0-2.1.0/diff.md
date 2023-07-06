# Comparing `tmp/robocorp_tasks-2.0.0.tar.gz` & `tmp/robocorp_tasks-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-2.0.0.tar", max compression
+gzip compressed data, was "robocorp_tasks-2.1.0.tar", max compression
```

## Comparing `robocorp_tasks-2.0.0.tar` & `robocorp_tasks-2.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     5432 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/README.md
--rw-r--r--   0        0        0     1234 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3502 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     4495 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1457 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5121 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0    10199 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0     2245 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_config.py
--rw-r--r--   0        0        0      182 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0     1122 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     1367 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_lifecycle.py
--rw-r--r--   0        0        0     5080 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0      461 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     3943 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0     5489 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     2436 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/_toml_settings.py
--rw-r--r--   0        0        0      869 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0        0 2023-06-28 12:52:46.820026 robocorp_tasks-2.0.0/src/robocorp/tasks/py.typed
--rw-r--r--   0        0        0     6209 1970-01-01 00:00:00.000000 robocorp_tasks-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5432 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/README.md
+-rw-r--r--   0        0        0     1234 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3502 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4495 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1467 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5121 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0    10273 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0     2245 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_config.py
+-rw-r--r--   0        0        0      182 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0     1122 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     1367 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_lifecycle.py
+-rw-r--r--   0        0        0     5080 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2160 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     3943 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5489 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0     2436 2023-07-06 17:52:11.430171 robocorp_tasks-2.1.0/src/robocorp/tasks/_toml_settings.py
+-rw-r--r--   0        0        0      869 2023-07-06 17:52:11.434171 robocorp_tasks-2.1.0/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0        0 2023-07-06 17:52:11.434171 robocorp_tasks-2.1.0/src/robocorp/tasks/py.typed
+-rw-r--r--   0        0        0     6209 1970-01-01 00:00:00.000000 robocorp_tasks-2.1.0/PKG-INFO
```

### Comparing `robocorp_tasks-2.0.0/README.md` & `robocorp_tasks-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/pyproject.toml` & `robocorp_tasks-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "2.0.0"
+version = "2.1.0"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
 license = "Apache-2.0"
```

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/__init__.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 automatically logged is not imported prior the the `cli.main` call.
 """
 from pathlib import Path
 from typing import Optional
 
 from ._protocols import ITask
 
-__version__ = "2.0.0"
+__version__ = "2.1.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 def task(func):
     """
     Decorator for tasks (entry points) which can be executed by `robocorp.tasks`.
```

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_argdispatch.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_callback.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         if self._reversed:
             iter_in = reversed(self._callbacks)
         else:
             iter_in = self._callbacks
         for c in iter_in:
             try:
                 c(*args, **kwargs)
-            except:
+            except Exception:
                 logger.exception(f"Error calling: {c}.")
                 if self.raise_exceptions:
                     raise
```

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_commands.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     from ._hooks import (
         after_all_tasks_run,
         after_task_run,
         before_all_tasks_run,
         before_task_run,
     )
     from ._log_auto_setup import read_robocorp_log_config, setup_cli_auto_logging
-    from ._log_output_setup import setup_log_output
+    from ._log_output_setup import setup_log_output, setup_log_output_to_port
     from ._protocols import ITask, Status
     from ._task import Context, set_current_task
 
     console.set_mode(console_colors)
 
     # Don't show internal machinery on tracebacks:
     # setting __tracebackhide__ will make it so that robocorp-log
@@ -170,15 +170,15 @@
         # Note: we can't customize what's a "project" file or a "library" file, right now
         # the customizations are all based on module names.
         config
     ), redirect.setup_stdout_logging(log_output_to_stdout), setup_log_output(
         output_dir=Path(output_dir),
         max_files=max_log_files,
         max_file_size=max_log_file_size,
-    ), context.register_lifecycle_prints():
+    ), setup_log_output_to_port(), context.register_lifecycle_prints():
         run_status = "PASS"
         setup_message = ""
 
         run_name = os.path.basename(p)
         if task_name:
             run_name += f" - {task_name}"
 
@@ -250,15 +250,15 @@
             # After the run is finished, start a timer which will print the
             # current threads if the process doesn't exit after a given timeout.
             from threading import Timer
 
             var_name = "RC_DUMP_THREADS_AFTER_RUN_TIMEOUT"
             try:
                 timeout = float(os.environ.get(var_name, "40"))
-            except:
+            except Exception:
                 sys.stderr.write(
                     f"Invalid value for: {var_name} environment value. Cannot convert to float."
                 )
                 timeout = 40
 
             def on_timeout():
                 _dump_threads(
@@ -274,15 +274,15 @@
     if stream is None:
         stream = sys.stderr
 
     thread_id_to_name = {}
     try:
         for t in threading.enumerate():
             thread_id_to_name[t.ident] = "%s  (daemon: %s)" % (t.name, t.daemon)
-    except:
+    except Exception:
         pass
 
     stack_trace = [
         "===============================================================================",
         message,
         "================================= Thread Dump =================================",
     ]
```

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_config.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_lifecycle.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_task.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/_toml_settings.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/_toml_settings.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/src/robocorp/tasks/cli.py` & `robocorp_tasks-2.1.0/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-2.0.0/PKG-INFO` & `robocorp_tasks-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 2.0.0
+Version: 2.1.0
 Summary: The automation framework for Python
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

