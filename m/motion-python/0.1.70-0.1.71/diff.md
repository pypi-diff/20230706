# Comparing `tmp/motion_python-0.1.70.tar.gz` & `tmp/motion_python-0.1.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.70.tar", max compression
+gzip compressed data, was "motion_python-0.1.71.tar", max compression
```

## Comparing `motion_python-0.1.70.tar` & `motion_python-0.1.71.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3344 2023-06-30 02:57:24.512919 motion_python-0.1.70/README.md
--rw-r--r--   0        0        0      338 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/cli.py
--rw-r--r--   0        0        0    24213 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/component.py
--rw-r--r--   0        0        0    17749 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/execute.py
--rw-r--r--   0        0        0    13924 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/instance.py
--rw-r--r--   0        0        0     4889 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/route.py
--rw-r--r--   0        0        0     5944 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/server/fit_task.py
--rw-r--r--   0        0        0     9481 2023-06-30 02:57:24.512919 motion_python-0.1.70/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-30 02:57:49.945693 motion_python-0.1.70/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.70/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-06 18:29:22.418477 motion_python-0.1.71/README.md
+-rw-r--r--   0        0        0      338 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/cli.py
+-rw-r--r--   0        0        0    22752 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/component.py
+-rw-r--r--   0        0        0    17241 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/execute.py
+-rw-r--r--   0        0        0    13742 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/instance.py
+-rw-r--r--   0        0        0     4889 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1125 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/route.py
+-rw-r--r--   0        0        0     5890 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/server/fit_task.py
+-rw-r--r--   0        0        0     9333 2023-07-06 18:29:22.418477 motion_python-0.1.71/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-06 18:29:45.570838 motion_python-0.1.71/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.71/PKG-INFO
```

### Comparing `motion_python-0.1.70/README.md` & `motion_python-0.1.71/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.70/motion/cli.py` & `motion_python-0.1.71/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.70/motion/component.py` & `motion_python-0.1.71/motion/component.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-import functools
 import inspect
-from typing import Any, Callable, Dict, List, Optional, Union, get_type_hints
-
-from pydantic import BaseModel
+from typing import Any, Callable, Dict, List, Optional, Union
 
 from motion.instance import ComponentInstance
 from motion.route import Route
 from motion.utils import CustomDict, random_passphrase, validate_args
 
 
 class Component:
@@ -24,22 +21,23 @@
             return {"value": 0}
 
         @AdderComponent.infer("add")
         def plus(state, value):
             return state["value"] + value
 
         @AdderComponent.fit("add")
-        def add(state, values, infer_results):
-            return {"value": state["value"] + sum(values)}
+        def add(state, value, infer_result):
+            return {"value": state["value"] + value}
 
         if __name__ == "__main__":
             c = AdderComponent() # Create instance of AdderComponent
-            c.run(add=1, flush_fit=True) # Will return 1, blocking until fit
+            c.run("add", kwargs={"value": 1}, flush_fit=True) # Blocks until fit
             # is done. Resulting state is {"value": 1}
-            c.run(add=2) # Will return 3, not waiting for fit operation.
+            c.run("add", kwargs={"value": 2}) # Will return 3, not waiting
+            # for fit operation.
             # Resulting state will eventually be {"value": 3}
         ```
 
     === "Multiple Dataflows"
         ```python
         from motion import Component
 
@@ -50,90 +48,81 @@
             return {"value": 0}
 
         @Calculator.infer("add")
         def plus(state, value):
             return state["value"] + value
 
         @Calculator.fit("add")
-        def increment(state, values, infer_results):
-            return {"value": state["value"] + sum(values)}
+        def increment(state, infer_result, value):
+            return {"value": state["value"] + value}
 
         @Calculator.infer("subtract")
         def minus(state, value):
             return state["value"] - value
 
         @Calculator.fit("subtract")
-        def decrement(state, values, infer_results):
-            return {"value": state["value"] - sum(values)}
+        def decrement(state, infer_result, value):
+            return {"value": state["value"] - value}
 
         if __name__ == "__main__":
             c = Calculator()
-            c.run(add=1, flush_fit=True) # Will return 1, blocking until fit
-            # is done. Resulting state is {"value": 1}
-            c.run(subtract=1, flush_fit=True) # Will return 0, blocking
-            # until fit is done. Resulting state is {"value": 0}
+            c.run("add", kwargs={"value": 1}, flush_fit=True) # Will return 1,
+            # blocking until fit is done. Resulting state is {"value": 1}
+            c.run("subtract", kwargs={"value": 1}, flush_fit=True)
+            # Will return 0, blocking until fit is done. Resulting state is #
+            # {"value": 0}
         ```
 
-    === "Batch Size > 1"
+    === "Batching Fit Operations"
 
         ```python
         from motion import Component
         import numpy as np
 
         MLMonitor = Component("Monitoring_ML_Component")
 
         @MLMonitor.init_state
         def setUp():
-            return {"model": YOUR_MODEL_HERE, "history": []}
+            return {
+                "model": YOUR_MODEL_HERE,
+                "historical_values": [],
+                "historical_infer_results": []
+            }
 
         @MLMonitor.infer("features")
         def predict(state, value):
             return state["model"].predict(value)
 
-        @MLMonitor.fit("features", batch_size=10)
-        def monitor(state, values, infer_results):
-            new_X = np.array(values)
-            new_y = np.array(infer_results)
-            concatenated = np.concatenate((state["history"], new_y))
-            if YOUR_ANOMALY_ALGORITHM(concatenated, history):
-                # Fire an alert
-                YOUR_ALERT_FUNCTION()
-            return {"history": history + [concatenated]}
+        @MLMonitor.fit("features")
+        def monitor(state, value, infer_result):
+
+            values = state["historical_values"] + [value]
+            infer_results = state["historical_infer_results"] + [infer_result]
+
+            # Check drift every 10 values
+            if len(values) == 10:
+                if YOUR_ANOMALY_ALGORITHM(values, infer_results):
+                    # Fire an alert
+                    YOUR_ALERT_FUNCTION()
+                values = []
+                infer_results = []
+
+            return {
+                "historical_values": values,
+                "historical_infer_results": infer_results
+            }
 
         if __name__ == "__main__":
             c = MLMonitor() # Create instance
-            c.run(features=YOUR_FEATURES_HERE) # Don't wait for fit to finish
-            # because batch size is 10
+            c.run(features=YOUR_FEATURES_HERE)
 
             for _ in range(100):
                 c.run(features=YOUR_FEATURES_HERE)
                 # Some alert may be fired in the background!
         ```
-
-    === "Type Validation"
-        ```python
-        from motion import Component
-        from pydantic import BaseModel
-
-        class MyModel(BaseModel):
-            value: int
-
-        MyComponent = Component("MyComponentWithValidation")
-
-        @MyComponent.infer("noop")
-        def noop(state, value: MyModel):
-            return value.value
-
-        if __name__ == "__main__":
-            c = MyComponent()
-            c.run(noop=MyModel(value=1)) # Will return 1
-            c.run(noop={"value": 1}) # Will return 1
-            c.run(noop=MyModel(value="1")) # Will raise an Error
-            c.run(noop=1) # Will raise an Error
-        ```
     """
 
     def __init__(self, name: str, params: Dict[str, Any] = {}):
         """Creates a new Motion component.
 
         Args:
             name (str):
@@ -294,31 +283,29 @@
         Returns:
             Callable: Decorated load_state function.
         """
         self._load_state_func = func
         return func
 
     def infer(self, keys: Union[str, List[str]]) -> Callable:
-        """Decorator for any infer dataflow through the component. Takes
-        in a string that represents the input keyword for the infer dataflow.
+        """Decorator for any infer operation for a dataflow through the
+        component. Takes in a string or list of strings that represents the
+        dataflow key. If the decorator is called with a list of strings, each
+        dataflow key will be mapped to the same infer function.
 
         2 arguments required for an infer operation:
             * `state`: The current state of the component, which is a
                 dictionary with string keys and any type values.
             * `value`: The value passed in through a `c.run` call with the
                 `key` argument.
 
-        Components can have multiple infer ops, but each infer op must have its
-        own unique `key` argument. Infer ops should not modify the state
-        object. If you want to modify the state object, use the `fit` decorator.
-
-        The `value` argument can be optionally type checked with Pydantic type
-        hints. If the type hint is a Pydantic model, the `value` argument will
-        be converted to that model if it is a dictionary and not already of the
-        model type.
+        Components can have multiple infer ops, but no dataflow key within
+        the component can have more than one infer op. Infer ops should not
+        modify the state object. If you want to modify the state object, use
+        the `fit` decorator.
 
         Example Usage:
         ```python
         from motion import Component
 
         MyComponent = Component("MyComponent")
 
@@ -331,16 +318,16 @@
             return state["value"] + value
 
         @MyComponent.infer("multiply")
         def multiply(state, value):
             return state["value"] * value
 
         c = MyComponent()
-        c.run(add=1, flush_fit=True) # Returns 1
-        c.run(multiply=2) # Returns 2
+        c.run("add", kwargs={"value": 1}, flush_fit=True) # Returns 1
+        c.run("multiply", kwargs={"value": 2}) # Returns 2
         ```
 
         Args:
             keys (Union[str, List[str]]): String or list of strings that
                 represent the input keyword(s) for the infer dataflow.
 
         Returns:
@@ -352,60 +339,39 @@
         for key in keys:
             if "::" in key:
                 raise ValueError(
                     f"Dataflow key {key} should not have a double colon (::)"
                 )
 
         def decorator(func: Callable) -> Any:
-            type_hint = get_type_hints(func).get("value", None)
+            # type_hint = get_type_hints(func).get("value", None)
             if not validate_args(inspect.signature(func).parameters, "infer"):
                 raise ValueError(
-                    f"Infer function {func.__name__} should have 2 arguments "
-                    + "`state` and `value`"
+                    f"Infer function {func.__name__} should have arguments " + "`state`"
                 )
 
-            @functools.wraps(func)
-            def wrapper(state: CustomDict, value: Any) -> Any:
-                if (
-                    type_hint
-                    and inspect.isclass(type_hint)
-                    and issubclass(type_hint, BaseModel)
-                    and not isinstance(value, type_hint)
-                ):
-                    try:
-                        value = type_hint(**value)
-                    except Exception:
-                        raise ValueError(
-                            f"value argument must be of type {type_hint.__name__}"
-                        )
-
-                return func(state, value)
-
-            wrapper._op = "infer"  # type: ignore
+            func._op = "infer"  # type: ignore
 
             for key in keys:
-                self.add_route(key, wrapper._op, wrapper)  # type: ignore
+                self.add_route(key, func._op, func)  # type: ignore
 
-            return wrapper
+            return func
 
         return decorator
 
-    def fit(self, keys: Union[str, List[str]], batch_size: int = 1) -> Any:
-        """Decorator for any fit dataflows through the component. Takes
-        in a string that represents the input keyword for the fit op.
-        Only executes the fit op (function) when the batch size is reached.
+    def fit(self, keys: Union[str, List[str]]) -> Any:
+        """Decorator for any fit operations for dataflows through the
+        component. Takes in a string or list of strings that represents the
+        dataflow key. If the decorator is called with a list of strings, each
+        dataflow key will be mapped to the same fit operation.
 
-        3 arguments required for a fit operation:
+        2 arguments required for a fit operation:
             - `state`: The current state of the component, represented as a
             dictionary.
-            - `values`: A list of values passed in through a `c.run` call with
-            the `key` argument. Of length `batch_size`.
-            - `infer_results`: A list of the results from the infer ops that
-            correspond to the values in the `values` argument. Of length
-            `batch_size`.
+            - `infer_result`: The result from the infer op that occurred before.
 
         Components can have multiple fit ops, and the same key can also have
         multiple fit ops. Fit functions should return a dictionary
         of state updates to be merged with the current state.
 
         Example Usage:
         ```python
@@ -421,35 +387,30 @@
         def add(state, values):
             return {"value": state["value"] + sum(values)}
 
         @MyComponent.infer("multiply")
         def multiply(state, value):
             return state["value"] * value
 
-        @MyComponent.fit("multiply", batch_size=2) # Runs after 2 c.run calls
-        def multiply(state, values, infer_results):
-            product = 1
-            for value in values:
-                product *= value
-            return state["value"] * product
+        @MyComponent.fit("multiply")
+        def multiply(state, infer_result, value):
+            return state["value"] * value
 
         c = MyComponent()
-        c.run(add=1, flush_fit=True) # Returns 1
-        c.run(multiply=2) # Returns 2, fit not executed yet
-        c.run(multiply=3) # Returns 3, fit will execute; state["value"] = 6
+        c.run("add", kwargs={"value": 1}, flush_fit=True) # Returns 1
+        c.run("multiply", kwargs={"value": 2}) # Returns 2, fit not executed yet
+        c.run("multiply", kwargs={"value": 3}) # Returns 3, fit will execute
+        # to get state["value"] = 6
         # Some time later...
-        c.run(multiply=4) # Returns 24
+        c.run("multiply", kwargs={"value": 4}) # Returns 24
         ```
 
         Args:
             keys (Union[str, List[str]]): String or list of strings that
                 represent the input keyword(s) for the fit dataflow.
-            batch_size (int, optional):
-                Number of values to wait for before
-                calling the fit function. Defaults to 1.
 
         Returns:
             Callable: Decorated fit function.
         """
         frame = inspect.currentframe().f_back  # type: ignore
         fname = frame.f_code.co_name  # type: ignore
         if fname != "<module>":
@@ -459,20 +420,20 @@
             )
         if isinstance(keys, str):
             keys = [keys]
 
         def decorator(func: Callable) -> Any:
             if not validate_args(inspect.signature(func).parameters, "fit"):
                 raise ValueError(
-                    f"Fit method {func.__name__} should have 3 arguments: "
-                    + "`state`, `values`, and `infer_results`."
+                    f"Fit method {func.__name__} should have >= 2 arguments: "
+                    + "`state` and `infer_result`."
                 )
 
             # func._input_key = key  # type: ignore
-            func._batch_size = batch_size  # type: ignore
+            # func._batch_size = batch_size  # type: ignore
             func._op = "fit"  # type: ignore
 
             for key in keys:
                 self.add_route(key, func._op, func)  # type: ignore
 
             return func
 
@@ -501,17 +462,18 @@
         # Define infer and fit operations
         @MyComponent.infer("key1")
         def ...
 
         @MyComponent.fit("key1)
         def ...
 
-        c_instance = MyComponent(init_state_params={"starting_val": 3})
         # Creates instance of MyComponent
-        c_instance.run(..)
+        if __name__ == "__main__":
+            c_instance = MyComponent(init_state_params={"starting_val": 3})
+            c_instance.run(..)
         ```
 
         Args:
             name (str, optional):
                 Name of the component instance. Defaults to "".
             init_state_params (Dict[str, Any], optional):
                 Parameters to pass into the init_state function. Defaults to {}.
@@ -577,15 +539,15 @@
                 graph[key] = {}
             graph[key]["fit"] = []
             for route in routes:
                 graph[key]["fit"].append(
                     {
                         "name": route.udf.__name__,
                         "udf": inspect.getsource(route.udf),
-                        "batch_size": route.udf._batch_size,  # type: ignore
+                        # "batch_size": route.udf._batch_size,  # type: ignore
                     }
                 )
 
         nodes = []
         edges = []
         node_id = 1
         max_x_offset = 0
@@ -663,28 +625,28 @@
                     # Add fit node
                     fit_node = {
                         "id": str(node_id),
                         "position": {"x": fit_x_offset, "y": key_y_position},
                         "data": {
                             "label": fit["name"],
                             "udf": fit["udf"],
-                            "batch_size": fit["batch_size"],
+                            # "batch_size": fit["batch_size"],
                         },
                         "type": "fit",
                     }
                     nodes.append(fit_node)
 
                     edges.append(
                         {
                             "id": "e{}-{}".format(fit_node["id"], state_node["id"]),
                             "target": state_node["id"],
                             "source": fit_node["id"],
                             "sourceHandle": "top",
                             "animated": True,  # type: ignore
-                            "label": f"batch_size: {fit['batch_size']}",
+                            # "label": f"batch_size: {fit['batch_size']}",
                         }
                     )
 
                     if "infer" in value.keys():
                         edges.append(
                             {
                                 "id": "e{}-{}".format(infer_node["id"], fit_node["id"]),
```

### Comparing `motion_python-0.1.70/motion/execute.py` & `motion_python-0.1.71/motion/execute.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,15 +131,14 @@
         for rkey, routes in self._fit_routes.items():
             for udf_name, route in routes.items():
                 pname = f"{self._instance_name}::{rkey}::{udf_name}"
                 multiprocessing.Event()
                 self.worker_tasks[pname] = FitTask(
                     self._instance_name,
                     route,
-                    batch_size=route.udf._batch_size,  # type: ignore
                     save_state_func=self._save_state_func,
                     load_state_func=self._load_state_func,
                     queue_identifier=self._get_queue_identifier(rkey, udf_name),
                     channel_identifier=self._get_channel_identifier(rkey, udf_name),
                     redis_host=rp.host,
                     redis_port=rp.port,
                     redis_db=rp.db,
@@ -169,15 +168,14 @@
                     # Restart
                     rkey = pname.split("::")[1]
                     udf_name = pname.split("::")[2]
                     route = self._fit_routes[rkey][udf_name]
                     self.worker_tasks[pname] = FitTask(
                         self._instance_name,
                         route,
-                        batch_size=route.udf._batch_size,  # type: ignore
                         save_state_func=self._save_state_func,
                         load_state_func=self._load_state_func,
                         queue_identifier=self._get_queue_identifier(rkey, udf_name),
                         channel_identifier=self._get_channel_identifier(rkey, udf_name),
                         redis_host=rp.host,
                         redis_port=rp.port,
                         redis_db=rp.db,
@@ -256,25 +254,18 @@
             )
 
             self.version = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
 
             # Release lock
             lock.release()
 
-    def empty_batch(self) -> Dict[str, List[Any]]:
-        return {
-            "fit_events": [],
-            "values": [],
-            "infer_results": [],
-        }
-
     def _enqueue_and_trigger_fit(
         self,
         key: str,
-        value: Any,
+        kwargs: Dict[str, Any],
         infer_result: Any,
         flush_fit: bool,
         route_hit: bool,
     ) -> bool:
         # Run the fit routes
         # Enqueue results into fit queues
         if key in self._fit_routes.keys():
@@ -296,22 +287,19 @@
                     )
                     fit_events.add(fit_udf_name, fit_event)
 
                 # Add to fit queue
                 self._redis_con.rpush(
                     queue_identifier,
                     cloudpickle.dumps(
-                        (
-                            {
-                                "value": value,
-                                "infer_result": infer_result,
-                                "identifier": identifier,
-                            },
-                            flush_fit,
-                        )
+                        {
+                            "kwargs": kwargs,
+                            "infer_result": infer_result,
+                            "identifier": identifier,
+                        }
                     ),
                 )
 
             if flush_fit:
                 # Wait for fit result to finish
                 fit_events.wait()
                 # Update state
@@ -325,15 +313,15 @@
                 self.version = int(v)
 
         return route_hit
 
     def _try_cached_infer(
         self,
         key: str,
-        value: Any,
+        kwargs: Dict[str, Any],
         ignore_cache: bool,
         force_refresh: bool,
     ) -> Tuple[bool, Optional[Any], Optional[str]]:
         route_run = False
         infer_result = None
 
         if force_refresh:
@@ -344,15 +332,15 @@
                     f"Error loading state for {self._instance_name}."
                     + " No version found."
                 )
             self.version = int(v)
 
         # Try hashing the value
         try:
-            value_hash = hash_object(value)
+            value_hash = hash_object(kwargs)
         except TypeError:
             value_hash = None
 
         # Check if key is in cache if value can be hashed and
         # user doesn't want to force refresh state
         if value_hash and not force_refresh and not ignore_cache:
             cache_result_key = f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
@@ -361,36 +349,34 @@
                 route_run = True
 
         return route_run, infer_result, value_hash
 
     def run(
         self,
         key: str,
-        value: Any,
+        kwargs: Dict[str, Any],
         cache_ttl: int,
         ignore_cache: bool,
         force_refresh: bool,
         flush_fit: bool,
     ) -> Any:
         route_hit = False
         infer_result = None
 
         # Run the infer route
         if key in self._infer_routes.keys():
             route_hit = True
             route_run, infer_result, value_hash = self._try_cached_infer(
-                key, value, ignore_cache, force_refresh
+                key, kwargs, ignore_cache, force_refresh
             )
 
             # If not in cache or value can't be hashed or
             # user wants to force refresh state, run route
             if not route_run:
-                infer_result = self._infer_routes[key].run(
-                    state=self._state, value=value
-                )
+                infer_result = self._infer_routes[key].run(state=self._state, **kwargs)
 
                 # Check that infer_result is not an awaitable
                 if asyncio.iscoroutine(infer_result):
                     raise TypeError(
                         f"Route {key} returned an awaitable. "
                         + "Call `await instance.arun(...)` instead."
                     )
@@ -405,46 +391,46 @@
                         cloudpickle.dumps(infer_result),
                         ex=cache_ttl,
                     )
 
         # Run the fit routes
         # Enqueue results into fit queues
         route_hit = self._enqueue_and_trigger_fit(
-            key, value, infer_result, flush_fit, route_hit
+            key, kwargs, infer_result, flush_fit, route_hit
         )
 
         if not route_hit:
             raise KeyError(f"Key {key} not in routes.")
 
         return infer_result
 
     async def arun(
         self,
         key: str,
-        value: Any,
+        kwargs: Dict[str, Any],
         cache_ttl: int,
         ignore_cache: bool,
         force_refresh: bool,
         flush_fit: bool,
     ) -> Any:
         route_hit = False
         infer_result = None
 
         # Run the infer route
         if key in self._infer_routes.keys():
             route_hit = True
             route_run, infer_result, value_hash = self._try_cached_infer(
-                key, value, ignore_cache, force_refresh
+                key, kwargs, ignore_cache, force_refresh
             )
 
             # If not in cache or value can't be hashed or
             # user wants to force refresh state, run route
             if not route_run:
                 infer_result_awaitable = self._infer_routes[key].run(
-                    state=self._state, value=value
+                    state=self._state, **kwargs
                 )
                 if not asyncio.iscoroutine(infer_result_awaitable):
                     raise TypeError(
                         f"Route {key} returned a non-awaitable. "
                         + "Call `instance.run(...)` instead."
                     )
 
@@ -460,15 +446,15 @@
                         cloudpickle.dumps(infer_result),
                         ex=cache_ttl,
                     )
 
         # Run the fit routes
         # Enqueue results into fit queues
         route_hit = self._enqueue_and_trigger_fit(
-            key, value, infer_result, flush_fit, route_hit
+            key, kwargs, infer_result, flush_fit, route_hit
         )
 
         if not route_hit:
             raise KeyError(f"Key {key} not in routes.")
 
         return infer_result
 
@@ -493,22 +479,19 @@
             fit_event = FitEvent(self._redis_con, channel_identifier, identifier)
             fit_events.add(fit_udf_name, fit_event)
 
             # Add to fit queue
             self._redis_con.rpush(
                 queue_identifier,
                 cloudpickle.dumps(
-                    (
-                        {
-                            "value": None,
-                            "infer_result": None,
-                            "identifier": identifier,
-                        },
-                        True,
-                    )
+                    {
+                        "value": None,
+                        "infer_result": None,
+                        "identifier": identifier,
+                    }
                 ),
             )
 
         # Wait for fit result to finish
         fit_events.wait()
         # Update state
         self._state = self._loadState()
```

### Comparing `motion_python-0.1.70/motion/instance.py` & `motion_python-0.1.71/motion/instance.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,16 +65,18 @@
             fit_routes=fit_routes,
             disabled=self.disabled,
         )
         self.running = True
 
     @property
     def instance_name(self) -> str:
-        """Component name with a random phrase or user-defined ID to represent
-        the name of this instance."""
+        """Component name with a random phrase to represent
+        the name of this instance.
+        In the form of componentname__randomphrase.
+        """
         return self._instance_name
 
     @property
     def instance_id(self) -> str:
         """Latter part of the instance name, which is a random phrase
         or a user-defined ID."""
         return self._instance_name.split("__")[-1]
@@ -91,18 +93,19 @@
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
         # Define infer and fit operations
 
-        c_instance = C()
-        c_instance.run(...)
-        c_instance.run(...)
-        c_instance.shutdown()
+        if __name__ == "__main__":
+            c_instance = C()
+            c_instance.run(...)
+            c_instance.run(...)
+            c_instance.shutdown()
         ```
         """
         if self.disabled:
             return
 
         if not self.running:
             return
@@ -129,16 +132,17 @@
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
         # Define infer and fit operations
 
-        c_instance = C()
-        c_instance.get_version() # Returns 1 (first version)
+        if __name__ == "__main__":
+            c_instance = C()
+            c_instance.get_version() # Returns 1 (first version)
         ```
         """
         return self._executor.version  # type: ignore
 
     def update_state(self, state_update: Dict[str, Any]) -> None:
         """Writes the state update to the component instance's state.
         If a fit op is currently running, the state update will be
@@ -206,45 +210,43 @@
 
     def flush_fit(self, dataflow_key: str) -> None:
         """Flushes the fit queue corresponding to the dataflow
         key, if it exists, and updates the instance state.
         Warning: this is a blocking operation and could take
         a while if your fit op takes a long time!
 
-        The fit queue will be flushed even if there aren't
-        the predefined batch_size number of elements.
-
         Example Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
         @C.infer("add")
         def add(state, value):
             return state["value"] + value
 
-        @C.fit("add", batch_size=2)
-        def add(state, values, infer_results):
-            return {"value": state["value"] + sum(values)}
+        @C.fit("add")
+        def add(state, value, infer_result):
+            return {"value": state["value"] + value}
 
         @C.infer("multiply")
         def multiply(state, value):
             return state["value"] * value
 
-        c = C() # Create instance of C
-        c.run(add=1)
-        c.flush_fit("add") # (1)!
-        c.run(add=2) # This will use the updated state
+        if __name__ == "__main__":
+            c = C() # Create instance of C
+            c.run("add", kwargs={"value": 1})
+            c.flush_fit("add") # (1)!
+            c.run("add", kwargs={"value": 2}) # This will use the updated state
 
-        # 1. Runs the fit op even though only one element is in the batch
+        # 1. Waits for the fit op to finish, then updates the state
         ```
 
         Args:
             dataflow_key (str): Key of the dataflow.
 
         Raises:
             RuntimeError: If the component instance was initialized to
@@ -253,25 +255,25 @@
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
         self._executor.flush_fit(dataflow_key)
 
     def run(
         self,
-        *,
+        # *,
+        dataflow_key: str,
+        kwargs: Dict[str, Any] = {},
         cache_ttl: int = DEFAULT_KEY_TTL,
         ignore_cache: bool = False,
         force_refresh: bool = False,
         flush_fit: bool = False,
-        **kwargs: Any,
     ) -> Any:
         """Runs the dataflow (infer and fit ops) for the keyword argument
         passed in. If the key is not found to have any ops, an error
-        is raised. Only one keyword argument should be passed in.
-        Fit ops are only executed when the batch size is reached.
+        is raised. Only one dataflow key should be passed in.
 
         Example Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
@@ -279,39 +281,40 @@
         def setUp():
             return {"value": 0}
 
         @C.infer("add")
         def add(state, value):
             return state["value"] + value
 
-        @C.fit("add", batch_size=2)
-        def add(state, values, infer_results):
-            return {"value": state["value"] + sum(values)}
-
-        @C.infer("multiply")
-        def multiply(state, value):
-            return state["value"] * value
+        @C.fit("add")
+        def add(state, value, infer_result):
+            return {"value": state["value"] + value}
 
-        c = C() # Create instance of C
-        c.run(add=1, flush_fit=True) # (1)!
-        c.run(add=1) # Returns 1
-        c.run(add=2, flush_fit=True) # Returns 2, result state["value"] = 4
-        # Previous line called fit function and flushed fit queue
-        c.run(add=3) # No fit op runs since batch size = 1
-        c.run(multiply=2) # Returns 8 since state["value"] = 4
-        c.run(multiply=3, flush_fit=True) # (2)!
-
-        # 1. This forces the fit op to run even though the batch size
-        #   isn't reached, and waits for the fit op to finish running
-        # 2. This doesn't force or wait for any fit ops, since there are
-        #   no fit ops defined for `multiply`
+        if __name__ == "__main__":
+            c = C() # Create instance of C
+            c.run("add", kwargs={"value": 1}, flush_fit=True) # (1)!
+            c.run("add", kwargs={"value": 1}) # Returns 1
+            c.run("add", kwargs={"value": 2}, flush_fit=True) # (2)!
+
+            c.run("add", kwargs={"value": 3})
+            time.sleep(3) # Wait for the previous fit op to finish
+
+            c.run("add", kwargs={"value": 3}, force_refresh=True) # (3)!
+
+        # 1. Waits for the fit op to finish, then updates the state
+        # 2. Returns 2, result state["value"] = 4
+        # 3. Force refreshes the state before running the dataflow, and
+        #    reruns the infer op even though the result might be cached.
         ```
 
 
         Args:
+            dataflow_key (str): Key of the dataflow to run.
+            kwargs (Dict[str, Any]): Keyword arguments to pass into the
+                dataflow ops, in addition to the state.
             cache_ttl (int, optional):
                 How long the inference result should live in a cache (in
                 seconds). Defaults to 1 day (60 * 60 * 24).
             ignore_cache (bool, optional):
                 If True, ignores the cache and runs the infer op. Does not
                 force refresh the state. Defaults to False.
             force_refresh (bool, optional): Read the latest value of the
@@ -319,58 +322,46 @@
                 version of the state or a cached result may be used.
                 Defaults to False.
             flush_fit (bool, optional):
                 If True, waits for the fit op to finish executing before
                 returning. If the fit queue hasn't reached batch_size
                 yet, the fit op runs anyways. Force refreshes the
                 state after the fit op completes. Defaults to False.
-            **kwargs:
-                Keyword arguments for the infer and fit ops. You can only
-                pass in one pair.
-
-        Raises:
-            ValueError: If more than one dataflow key-value pair is passed.
-            RuntimeError: If the component instance was initialized to
-            be disabled.
 
         Returns:
             Any: Result of the inference call. Might take a long time
             to run if `flush_fit = True` and the fit operation is
             computationally expensive.
         """
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
-        if len(kwargs) != 1:
-            raise ValueError("Only one key-value pair is allowed in kwargs.")
-
-        key, value = next(iter(kwargs.items()))
-
         infer_result = self._executor.run(
-            key=key,
-            value=value,
+            key=dataflow_key,
+            kwargs=kwargs,
             cache_ttl=cache_ttl,
             ignore_cache=ignore_cache,
             force_refresh=force_refresh,
             flush_fit=flush_fit,
         )
 
         return infer_result
 
     async def arun(
         self,
-        *,
+        # *,
+        dataflow_key: str,
+        kwargs: Dict[str, Any] = {},
         cache_ttl: int = DEFAULT_KEY_TTL,
         ignore_cache: bool = False,
         force_refresh: bool = False,
         flush_fit: bool = False,
-        **kwargs: Any,
     ) -> Awaitable[Any]:
-        """Async version of run. Runs the dataflow (infer and fit ops) for the .
-        keyword argument.
+        """Async version of run. Runs the dataflow (infer and fit ops) for the
+        specified key.
 
         Example Usage:
         ```python
         from motion import Component
         import asyncio
 
         C = Component("MyComponent")
@@ -378,21 +369,24 @@
         @C.infer("sleep")
         async def sleep(state, value):
             await asyncio.sleep(value)
             return "Slept!"
 
         async def main():
             c = C()
-            await c.arun(sleep=1)
+            await c.arun("sleep", kwargs={"value": 1})
 
         if __name__ == "__main__":
             asyncio.run(main())
         ```
 
         Args:
+            dataflow_key (str): Key of the dataflow to run.
+            kwargs (Dict[str, Any]): Keyword arguments to pass into the
+                dataflow ops, in addition to the state.
             cache_ttl (int, optional):
                 How long the inference result should live in a cache (in
                 seconds). Defaults to 1 day (60 * 60 * 24).
             ignore_cache (bool, optional):
                 If True, ignores the cache and runs the infer op. Does not
                 force refresh the state. Defaults to False.
             force_refresh (bool, optional): Read the latest value of the
@@ -415,22 +409,18 @@
 
         Returns:
             Awaitable[Any]: Awaitable Result of the inference call.
         """
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
-        if len(kwargs) != 1:
-            raise ValueError("Only one key-value pair is allowed in kwargs.")
-
-        key, value = next(iter(kwargs.items()))
-
         infer_result = await self._executor.arun(
-            key=key,
-            value=value,
+            key=dataflow_key,
+            kwargs=kwargs,
+            # value=value,
             cache_ttl=cache_ttl,
             ignore_cache=ignore_cache,
             force_refresh=force_refresh,
             flush_fit=flush_fit,
         )  # type: ignore
 
         return infer_result  # type: ignore
```

### Comparing `motion_python-0.1.70/motion/migrate.py` & `motion_python-0.1.71/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.70/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.71/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.70/motion/server/fit_task.py` & `motion_python-0.1.71/motion/server/fit_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 import asyncio
 import multiprocessing
 import traceback
-from typing import Any, Callable, List, Optional
+from typing import Any, Callable, Dict, Optional
 
 import cloudpickle
 import redis
 from redis.lock import Lock
 
 from motion.route import Route
 from motion.utils import loadState, logger, saveState
 
 
 class FitTask(multiprocessing.Process):
     def __init__(
         self,
         instance_name: str,
         route: Route,
-        batch_size: int,
+        # batch_size: int,
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
         queue_identifier: str,
         channel_identifier: str,
         redis_host: str,
         redis_port: int,
         redis_db: int,
         redis_password: str,
         running: Any,
     ):
         super().__init__()
+        self.name = f"FitTask-{instance_name}-{route.key}-{route.udf.__name__}"
         self.instance_name = instance_name
         self.save_state_func = save_state_func
         self.load_state_func = load_state_func
         self.redis_host = redis_host
         self.redis_port = redis_port
         self.redis_db = redis_db
         self.redis_password = redis_password
 
         self.route = route
-        self.batch_size = batch_size
+        # self.batch_size = batch_size
         self.queue_identifier = queue_identifier
         self.channel_identifier = channel_identifier
 
         # Keep track of batch
-        self.batch: List[Any] = []
+        # self.batch: List[Any] = []
 
         # Register the stop event
         # self.running = True
         # self.stop_event = stop_event
         self.running = running
         self.daemon = True
 
@@ -62,113 +63,116 @@
             db=self.redis_db,
         )
         # Acquire a lock
         lock_timeout = 300  # Lock timeout in seconds
         lock = Lock(redis_con, self.instance_name, lock_timeout)
 
         while self.running.value:
+            item: Dict[str, Any] = {}
             try:
-                for _ in range(self.batch_size):
-                    item = redis_con.blpop(self.queue_identifier, timeout=1)
-                    if item is None:
-                        if not self.running.value:
-                            break  # no more items in the list
-                        else:
-                            continue
-
-                    item, flush_fit = cloudpickle.loads(item[1])
-                    self.batch.append(item)
-                    if flush_fit:
-                        break
+                # for _ in range(self.batch_size):
+                full_item = redis_con.blpop(self.queue_identifier, timeout=0.5)
+                if full_item is None:
+                    if not self.running.value:
+                        break  # no more items in the list
+                    else:
+                        continue
+
+                item = cloudpickle.loads(full_item[1])
+                # self.batch.append(item)
+                # if flush_fit:
+                #     break
             except redis.exceptions.ConnectionError:
                 logger.error("Connection to redis lost.")
                 break
 
             # Check if we should stop
-            if not self.running.value:
-                self.cleanup()
+            if not self.running.value and not item:
+                # self.cleanup()
                 break
 
-            if not self.batch:
-                continue
-
-            # Remove from batch if it was a noop
-            values = []
-            infer_results = []
-            identifiers = []
-            for job in self.batch:
-                if not job["identifier"].startswith("NOOP_"):
-                    values.append(job["value"])
-                    infer_results.append(job["infer_result"])
-                identifiers.append(job["identifier"])
+            # if not self.batch:
+            #     continue
 
-            # Check that there are elements in values and infer_results
-            # Acquire lock and run op
             exception_str = ""
-            if len(values) >= 1:
-                acquired_lock = lock.acquire(blocking=True)
-                if acquired_lock:
-                    try:
-                        old_state = loadState(
-                            redis_con, self.instance_name, self.load_state_func
-                        )
-                        state_update = self.route.run(
-                            state=old_state,
-                            values=values,
-                            infer_results=infer_results,
-                        )
-                        # Await if state_update is a coroutine
-                        if asyncio.iscoroutine(state_update):
-                            state_update = asyncio.run(state_update)
-
-                        if not isinstance(state_update, dict):
-                            logger.error(
-                                "fit methods should return a dict of state updates."
-                            )
-                        else:
-                            old_state.update(state_update)
-                            saveState(
-                                old_state,
-                                redis_con,
-                                self.instance_name,
-                                self.save_state_func,
-                            )
-                    except Exception as e:
-                        # logger.error(f"Error in {self.queue_identifier} fit: {e}")
-                        logger.error(traceback.format_exc())
-                        exception_str = str(e)
-                    finally:
-                        logger.info("Releasing lock.")
-                        lock.release()
-                else:
-                    logger.error("Lock not acquired; batch lost.")
-
-            for identifier in identifiers:
+            # Check if it was a no op
+            if item["identifier"].startswith("NOOP_"):
                 redis_con.publish(
                     self.channel_identifier,
-                    str({"identifier": identifier, "exception": exception_str}),
+                    str(
+                        {
+                            "identifier": item["identifier"],
+                            "exception": exception_str,
+                        }
+                    ),
                 )
+                continue
 
-            # Clear batch
-            self.batch = []
-
-    def cleanup(self) -> None:
-        redis_con = redis.Redis(
-            host=self.redis_host,
-            port=self.redis_port,
-            password=self.redis_password,
-            db=self.redis_db,
-        )
-
-        # Add outstanding batch back to queue
-        for item in self.batch:
-            # Pickle item object
-            pickled_item = cloudpickle.dumps(
-                (
-                    item,
-                    False,  # flush_fit should be False
-                )
+            # Run fit op
+            acquired_lock = lock.acquire(blocking=True)
+            if acquired_lock:
+                try:
+                    old_state = loadState(
+                        redis_con, self.instance_name, self.load_state_func
+                    )
+                    state_update = self.route.run(
+                        state=old_state,
+                        infer_result=item["infer_result"],
+                        **item["kwargs"],
+                    )
+                    # Await if state_update is a coroutine
+                    if asyncio.iscoroutine(state_update):
+                        state_update = asyncio.run(state_update)
+
+                    if not isinstance(state_update, dict):
+                        logger.error(
+                            "fit methods should return a dict of state updates."
+                        )
+                    else:
+                        old_state.update(state_update)
+                        saveState(
+                            old_state,
+                            redis_con,
+                            self.instance_name,
+                            self.save_state_func,
+                        )
+                except Exception as e:
+                    # logger.error(f"Error in {self.queue_identifier} fit: {e}")
+                    logger.error(traceback.format_exc())
+                    exception_str = str(e)
+                finally:
+                    logger.info("Releasing lock.")
+                    lock.release()
+            else:
+                logger.error("Lock not acquired; item lost.")
+
+            redis_con.publish(
+                self.channel_identifier,
+                str(
+                    {
+                        "identifier": item["identifier"],
+                        "exception": exception_str,
+                    }
+                ),
             )
 
-            redis_con.lpush(self.queue_identifier, pickled_item)
+    # def cleanup(self) -> None:
+    #     redis_con = redis.Redis(
+    #         host=self.redis_host,
+    #         port=self.redis_port,
+    #         password=self.redis_password,
+    #         db=self.redis_db,
+    #     )
+
+    #     # Add outstanding batch back to queue
+    #     for item in self.batch:
+    #         # Pickle item object
+    #         pickled_item = cloudpickle.dumps(
+    #             (
+    #                 item,
+    #                 False,  # flush_fit should be False
+    #             )
+    #         )
+
+    #         redis_con.lpush(self.queue_identifier, pickled_item)
 
-        self.batch = []
+    #     self.batch = []
```

### Comparing `motion_python-0.1.70/motion/utils.py` & `motion_python-0.1.71/motion/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,27 +50,27 @@
     ```python
     from motion import clear_instance
 
     clear_instance("Counter__default")
     ```
 
     Args:
-        instance (str): Instance name of the component to clear.
-            In the form `componentname__instancename`.
+        instance_name (str): Instance name of the component to clear.
+            In the form `componentname__instanceid`.
 
     Raises:
         ValueError:
             If the instance name is not in the form
-            `componentname__instancename`.
+            `componentname__instanceid`.
 
     Returns:
         bool: True if the instance existed, False otherwise.
     """
     if "__" not in instance_name:
-        raise ValueError("Instance must be in the form `componentname__instancename`.")
+        raise ValueError("Instance must be in the form `componentname__instanceid`.")
 
     rp = RedisParams()
     redis_con = redis.Redis(host=rp.host, port=rp.port, password=rp.password, db=rp.db)
 
     # Check if the instance exists
     if not redis_con.exists(f"MOTION_VERSION:{instance_name}"):
         return False
@@ -99,27 +99,27 @@
     ```python
     from motion import inspect_state
 
     inspect_state("Counter__default")
     ```
 
     Args:
-        instance (str): Instance name of the component to inspect.
-            In the form `componentname__instancename`.
+        instance_name (str): Instance name of the component to inspect.
+            In the form `componentname__instanceid`.
 
     Raises:
         ValueError:
             If the instance name is not in the form
-            `componentname__instancename` or if the instance does not exist.
+            `componentname__instanceid` or if the instance does not exist.
 
     Returns:
         Dict[str, Any]: The state of the component instance.
     """
     if "__" not in instance_name:
-        raise ValueError("Instance must be in the form `componentname__instancename`.")
+        raise ValueError("Instance must be in the form `componentname__instanceid`.")
 
     rp = RedisParams()
     redis_con = redis.Redis(host=rp.host, port=rp.port, password=rp.password, db=rp.db)
 
     # Check if the instance exists
     if not redis_con.exists(f"MOTION_VERSION:{instance_name}"):
         raise ValueError(f"Instance {instance_name} does not exist.")
@@ -150,23 +150,19 @@
             raise KeyError(
                 f"Key `{key}` not found in {self.dict_type} for "
                 + f"instance {self.component_name}__{self.instance_id}."
             )
 
 
 def validate_args(parameters: Any, op: str) -> bool:
-    expected_args = (
-        ["state", "values", "infer_results"] if op == "fit" else ["state", "value"]
-    )
-    if len(parameters) != len(expected_args):
+    if "state" not in parameters.keys():
         return False
 
-    for param_name, _ in parameters.items():
-        if param_name not in expected_args:
-            return False
+    if op == "fit" and "infer_result" not in parameters.keys():
+        return False
 
     return True
 
 
 def configureLogging(level: str) -> None:
     handler = logging.StreamHandler()
```

### Comparing `motion_python-0.1.70/pyproject.toml` & `motion_python-0.1.71/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.70"
+version = "0.1.71"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.70/PKG-INFO` & `motion_python-0.1.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.70
+Version: 0.1.71
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

