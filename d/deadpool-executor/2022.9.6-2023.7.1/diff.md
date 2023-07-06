# Comparing `tmp/deadpool-executor-2022.9.6.tar.gz` & `tmp/deadpool_executor-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deadpool-executor-2022.9.6.tar", last modified: Fri Sep 23 10:56:10 2022, max compression
+gzip compressed data, was "deadpool_executor-2023.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deadpool-executor-2022.9.6.tar` & `deadpool_executor-2023.7.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0    34523 2022-09-17 05:35:45.842877 deadpool-executor-2022.9.6/LICENSE
--rw-r--r--   0        0        0    19275 2022-09-23 10:54:46.092568 deadpool-executor-2022.9.6/README.rst
--rw-r--r--   0        0        0    14577 2022-09-23 10:55:21.644818 deadpool-executor-2022.9.6/deadpool.py
--rw-r--r--   0        0        0      470 2022-09-23 04:37:29.294197 deadpool-executor-2022.9.6/examples/callbacks.py
--rw-r--r--   0        0        0      509 2022-09-23 04:37:29.294197 deadpool-executor-2022.9.6/examples/entrypoint.py
--rw-r--r--   0        0        0      730 2022-09-23 04:37:29.294197 deadpool-executor-2022.9.6/examples/priorities.py
--rw-r--r--   0        0        0     1289 2022-09-23 05:25:29.116451 deadpool-executor-2022.9.6/pyproject.toml
--rw-r--r--   0        0        0      168 2022-09-23 01:15:48.344108 deadpool-executor-2022.9.6/tests/conftest.py
--rw-r--r--   0        0        0     7929 2022-09-23 05:57:30.073581 deadpool-executor-2022.9.6/tests/test_deadpool.py
--rw-r--r--   0        0        0    20354 1970-01-01 00:00:00.000000 deadpool-executor-2022.9.6/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/.coveragerc
+-rw-r--r--   0        0        0    34523 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.1/LICENSE
+-rw-r--r--   0        0        0    20242 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/README.rst
+-rw-r--r--   0        0        0       86 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/covstart.pth
+-rw-r--r--   0        0        0    22051 2023-07-06 00:57:38.760330 deadpool_executor-2023.7.1/deadpool.py
+-rw-r--r--   0        0        0      477 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/examples/callbacks.py
+-rw-r--r--   0        0        0      516 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/examples/entrypoint.py
+-rw-r--r--   0        0        0      737 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/examples/priorities.py
+-rw-r--r--   0        0        0     1168 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/noxfile.py
+-rw-r--r--   0        0        0     1289 2022-10-24 05:21:18.405196 deadpool_executor-2023.7.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/tests/conftest.py
+-rw-r--r--   0        0        0    11381 2023-07-06 00:56:58.624632 deadpool_executor-2023.7.1/tests/test_deadpool.py
+-rw-r--r--   0        0        0    21321 1970-01-01 00:00:00.000000 deadpool_executor-2023.7.1/PKG-INFO
```

### Comparing `deadpool-executor-2022.9.6/LICENSE` & `deadpool_executor-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deadpool-executor-2022.9.6/README.rst` & `deadpool_executor-2023.7.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -486,13 +486,57 @@
 
    with deadpool.DeadPool(
            shutdown_wait=True,
            shutdown_cancel_futures=True
    ):
        fut = exe.submit(...)
 
+Developer Workflow
+------------------
+
+nox
+^^^
+This project uses ``nox``. Follow the instructions for installing
+nox at their page, and then come back here.
+
+While nox can be configured so that all the tools for each of
+the tasks can be installed automatically when run, this takes
+too much time and so I've decided that you should just have
+the following tools in your environment, ready to go. They
+do not need to be installed in the same venv or anything like
+that. I've found a convenient way to do this is with ``pipx``.
+For example, to install ``black`` using ``pipx`` you can do
+the following:
+
+.. code-block:: shell
+
+   $ pipx install black
+
+You must do the same for ``isort`` and ``ruff``. See the following
+sections for actually using ``nox`` to perform dev actions.
+
+tests
+^^^^^
+
+To run the tests:
+
+.. code-block:: shell
+
+   $ nox -s tests
+
+style
+^^^^^
+
+To apply style fixes, and check for any remaining lints,
+
+.. code-block:: shell
+
+   $ nox -t style
+
+
+
 
 .. _shutdown: https://docs.python.org/3/library/concurrent.futures.html?highlight=brokenprocesspool#concurrent.futures.Executor.shutdown
 .. _ProcessPoolExecutor: https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#processpoolexecutor
 .. _RuntimeError: https://github.com/noxdafox/pebble/issues/42#issuecomment-551245730
 .. _OOM killer: https://en.wikipedia.org/wiki/Out_of_memory#Out_of_memory_management
 .. _multiprocessing.Pool: https://docs.python.org/3.11/library/multiprocessing.html#multiprocessing.pool.Pool
```

### Comparing `deadpool-executor-2022.9.6/examples/priorities.py` & `deadpool_executor-2023.7.1/examples/priorities.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import random, time
+import random
+import time
+
 import deadpool
 
 
 def work(symbol):
     time.sleep(random.random() * 4.0)
     print(symbol, end="", flush=True)
     return 1
```

### Comparing `deadpool-executor-2022.9.6/pyproject.toml` & `deadpool_executor-2023.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deadpool-executor-2022.9.6/tests/test_deadpool.py` & `deadpool_executor-2023.7.1/tests/test_deadpool.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,87 @@
+import asyncio
+import logging
 import os
 import queue
 import signal
-from contextlib import contextmanager
+import sys
 import time
+import unittest
 from concurrent.futures import CancelledError, as_completed
-import logging
+from contextlib import contextmanager
+from functools import partial
 
 import pytest
 
 import deadpool
 
 
+@pytest.fixture()
+def logging_initializer():
+    return partial(logging.basicConfig, level=logging.DEBUG)
+
+
+async def test_func():
+    await asyncio.sleep(0.1)
+    return 42
+
+
+class TestDeadPool(unittest.TestCase):
+    async def test_acquire(self):
+        async with deadpool.DeadPool(size=2) as pool:
+            fut1 = pool.acquire()
+            fut2 = pool.acquire()
+            await asyncio.sleep(0.1)  # ensure both workers are running
+            self.assertEqual(pool.num_workers(), 2)
+            pool.release(await fut1)
+            pool.release(await fut2)
+        self.assertEqual(pool.num_workers(), 0)
+
+    async def test_concurrent_tasks(self):
+        async with deadpool.DeadPool(size=2) as pool:
+            results = await asyncio.gather(
+                pool.run_in_executor(test_func), pool.run_in_executor(test_func)
+            )
+            self.assertEqual(len(results), 2)
+            self.assertIn(42, results)
+
+    async def test_oversubscription(self):
+        async with deadpool.DeadPool(size=2) as pool:
+            fut1 = pool.acquire()
+            fut2 = pool.acquire()
+            fut3 = pool.acquire()
+            await asyncio.sleep(0.1)  # ensure all workers are running
+            self.assertEqual(pool.num_workers(), 2)
+            pool.release(await fut1)
+            pool.release(await fut2)
+            pool.release(await fut3)
+        self.assertEqual(pool.num_workers(), 0)
+
+    async def test_closed_pool(self):
+        pool = deadpool.DeadPool(size=2)
+        await pool.acquire()
+        await pool.acquire()
+        pool.close()
+        with self.assertRaises(RuntimeError):
+            await pool.acquire()
+
+    async def test_worker_exceptions(self):
+        async def failing_func():
+            await asyncio.sleep(0.1)
+            raise ValueError("failed")
+
+        async with deadpool.DeadPool(size=2) as pool:
+            results = await asyncio.gather(
+                pool.run_in_executor(failing_func), pool.run_in_executor(test_func)
+            )
+            self.assertEqual(len(results), 2)
+            self.assertIn(42, results)
+            self.assertIsInstance(results[0], ValueError)
+
+
 def f():
     return 123
 
 
 def t(duration=10.0):
     time.sleep(duration)
     return duration
@@ -35,63 +102,80 @@
 
     deadpool.cancel_all_futures_on_queue(q)
 
     for f in futs:
         assert f.cancelled()
 
 
-def test_simple():
-    with deadpool.Deadpool() as exe:
+@pytest.mark.parametrize("malloc_threshold", [None, 0, 1_000_000])
+def test_simple(malloc_threshold):
+    with deadpool.Deadpool(
+        malloc_trim_rss_memory_threshold_bytes=malloc_threshold
+    ) as exe:
         fut = exe.submit(t, 0.5)
         result = fut.result()
 
     assert result == 0.5
 
     # Outside the context manager, no new tasks
     # can be submitted.
     with pytest.raises(deadpool.PoolClosed):
         exe.submit(f)
 
 
+def test_simple_batch(logging_initializer):
+    with deadpool.Deadpool(max_workers=1, initializer=logging_initializer) as exe:
+        futs = [exe.submit(t, 0.1) for _ in range(2)]
+        results = [fut.result() for fut in futs]
+
+    assert results == [0.1] * 2
+
+
 @pytest.mark.parametrize("wait", [True, False])
 @pytest.mark.parametrize("cancel_futures", [True, False])
-def test_shutdown(wait, cancel_futures):
+def test_shutdown(logging_initializer, wait, cancel_futures):
     with deadpool.Deadpool(
+        max_workers=1,
         shutdown_wait=wait,
         shutdown_cancel_futures=cancel_futures,
+        initializer=logging_initializer,
     ) as exe:
         fut = exe.submit(f)
         result = fut.result()
 
     assert result == 123
 
 
 @pytest.mark.parametrize("wait", [True, False])
 @pytest.mark.parametrize("cancel_futures", [True, False])
-def test_shutdown_manual(wait, cancel_futures):
+def test_shutdown_manual(logging_initializer, wait, cancel_futures):
     logging.info("Test start")
 
     def callback(*args):
         logging.info(f"fut callback: {args=}")
 
-    exe = deadpool.Deadpool(max_workers=2)
+    exe = deadpool.Deadpool(max_workers=2, initializer=logging_initializer)
     fut1 = exe.submit(t, 2)
     fut1.add_done_callback(callback)
     fut2 = exe.submit(t, 2)
     fut2.add_done_callback(callback)
     fut3 = exe.submit(t, 2)  # This one will not start executing
     fut3.add_done_callback(callback)
 
     # logging.info(f"{exe.submitted_jobs.qsize()=}")
     # logging.info(f"{exe.running_futs=}")
     time.sleep(0.5)
     logging.info(f"{exe.submitted_jobs.qsize()=}")
     logging.info(f"{exe.running_futs=}")
     exe.shutdown(wait=wait, cancel_futures=cancel_futures)
-    logging.info(f"shutdown has unblocked")
+    logging.info("shutdown has unblocked")
+
+    logging.debug(f"{fut1.pid=}")
+    logging.debug(f"{fut2.pid=}")
+    logging.debug(f"{fut3.pid=}")
 
     if wait is False:
         if cancel_futures is True:
             assert fut1.cancelled()
             assert fut2.cancelled()
             assert fut3.cancelled()
         else:
@@ -233,28 +317,28 @@
 
         f1.add_pid_callback(pid_callback)
 
     assert collector and isinstance(collector[0], int)
 
 
 def f_sub():
-    with deadpool.Deadpool() as exe:
+    with deadpool.Deadpool(daemon=False) as exe:
         fut = exe.submit(g_sub)
         return fut.result()
 
 
 def g_sub():
     with deadpool.Deadpool() as exe:
-        futs = exe.map(time.sleep, [55.0] * 10)
+        _futs = exe.map(time.sleep, [55.0] * 10)
 
     return 123
 
 
 def test_sub_sub_process():
-    with deadpool.Deadpool(max_workers=5) as exe:
+    with deadpool.Deadpool(max_workers=5, daemon=False, mp_context="spawn") as exe:
         f1 = exe.submit(f_sub)
         time.sleep(0.5)
         assert f1.pid
         # Note: this doesn't kill the children, only the subprocess
         # of the task itself. The children continue to run.
         os.kill(f1.pid, signal.SIGKILL)
         with pytest.raises(deadpool.ProcessError):
@@ -303,35 +387,54 @@
 
 
 @pytest.mark.parametrize(
     "raises,exc_type,match",
     [
         (MyBadException, MyBadException, "(1, 2, 3)"),
         (MyBadExceptionSetState, ValueError, "failed to unpickle"),
-        (MyBadExceptionReduce, deadpool.ProcessError, "completed unexpectedly"),
-        (MyBadExceptionReduceRaise, deadpool.ProcessError, "completed unexpectedly"),
+        pytest.param(
+            MyBadExceptionReduce,
+            deadpool.ProcessError,
+            "pickling it failed",
+            marks=pytest.mark.skipif(
+                sys.version_info < (3, 10), reason="different message"
+            ),
+        ),
+        pytest.param(
+            MyBadExceptionReduceRaise,
+            deadpool.ProcessError,
+            "pickling it failed",
+            marks=pytest.mark.skipif(
+                sys.version_info < (3, 10), reason="different message"
+            ),
+        ),
     ],
 )
-def test_bad_exception(raises, exc_type, match):
-    with deadpool.Deadpool() as exe:
+def test_bad_exception(logging_initializer, raises, exc_type, match):
+    with deadpool.Deadpool(max_workers=1, initializer=logging_initializer) as exe:
         fut = exe.submit(raise_custom_exception, raises)
 
         with pytest.raises(exc_type, match=match):
-            result = fut.result()
+            _result = fut.result()
 
 
 def test_cancel_and_kill():
     with deadpool.Deadpool() as exe:
         fut = exe.submit(t, 10)
         time.sleep(0.5)
         fut.cancel_and_kill_if_running()
         with pytest.raises(deadpool.CancelledError):
             fut.result()
 
 
+def test_trim_memory():
+    """Just testing it doesn't fail."""
+    deadpool.trim_memory()
+
+
 @contextmanager
 def elapsed():
     t0 = time.perf_counter()
     try:
         yield
     finally:
         t1 = time.perf_counter()
```

### Comparing `deadpool-executor-2022.9.6/PKG-INFO` & `deadpool_executor-2023.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deadpool-executor
-Version: 2022.9.6
+Version: 2023.7.1
 Summary: Deadpool
 Author-email: Caleb Hattingh <caleb.hattingh@gmail.com>
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
@@ -511,14 +511,58 @@
 
    with deadpool.DeadPool(
            shutdown_wait=True,
            shutdown_cancel_futures=True
    ):
        fut = exe.submit(...)
 
+Developer Workflow
+------------------
+
+nox
+^^^
+This project uses ``nox``. Follow the instructions for installing
+nox at their page, and then come back here.
+
+While nox can be configured so that all the tools for each of
+the tasks can be installed automatically when run, this takes
+too much time and so I've decided that you should just have
+the following tools in your environment, ready to go. They
+do not need to be installed in the same venv or anything like
+that. I've found a convenient way to do this is with ``pipx``.
+For example, to install ``black`` using ``pipx`` you can do
+the following:
+
+.. code-block:: shell
+
+   $ pipx install black
+
+You must do the same for ``isort`` and ``ruff``. See the following
+sections for actually using ``nox`` to perform dev actions.
+
+tests
+^^^^^
+
+To run the tests:
+
+.. code-block:: shell
+
+   $ nox -s tests
+
+style
+^^^^^
+
+To apply style fixes, and check for any remaining lints,
+
+.. code-block:: shell
+
+   $ nox -t style
+
+
+
 
 .. _shutdown: https://docs.python.org/3/library/concurrent.futures.html?highlight=brokenprocesspool#concurrent.futures.Executor.shutdown
 .. _ProcessPoolExecutor: https://docs.python.org/3/library/concurrent.futures.html?highlight=broken%20process%20pool#processpoolexecutor
 .. _RuntimeError: https://github.com/noxdafox/pebble/issues/42#issuecomment-551245730
 .. _OOM killer: https://en.wikipedia.org/wiki/Out_of_memory#Out_of_memory_management
 .. _multiprocessing.Pool: https://docs.python.org/3.11/library/multiprocessing.html#multiprocessing.pool.Pool
```

