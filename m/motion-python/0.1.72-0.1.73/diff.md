# Comparing `tmp/motion_python-0.1.72.tar.gz` & `tmp/motion_python-0.1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.72.tar", max compression
+gzip compressed data, was "motion_python-0.1.73.tar", max compression
```

## Comparing `motion_python-0.1.72.tar` & `motion_python-0.1.73.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3344 2023-07-06 18:38:18.732894 motion_python-0.1.72/README.md
--rw-r--r--   0        0        0      338 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/__init__.py
--rw-r--r--   0        0        0     3867 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/cli.py
--rw-r--r--   0        0        0    22752 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/component.py
--rw-r--r--   0        0        0    17241 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/execute.py
--rw-r--r--   0        0        0    13742 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/instance.py
--rw-r--r--   0        0        0     4889 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/migrate.py
--rw-r--r--   0        0        0    13660 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0     1125 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/route.py
--rw-r--r--   0        0        0     5890 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/server/fit_task.py
--rw-r--r--   0        0        0     9333 2023-07-06 18:38:18.736894 motion_python-0.1.72/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-07-06 18:38:38.128875 motion_python-0.1.72/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.72/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-07-06 19:19:41.586125 motion_python-0.1.73/README.md
+-rw-r--r--   0        0        0      344 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/__init__.py
+-rw-r--r--   0        0        0     3867 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/cli.py
+-rw-r--r--   0        0        0    22800 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/component.py
+-rw-r--r--   0        0        0    17433 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/execute.py
+-rw-r--r--   0        0        0    13869 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/instance.py
+-rw-r--r--   0        0        0     4889 2023-07-06 19:19:41.586125 motion_python-0.1.73/motion/migrate.py
+-rw-r--r--   0        0        0    13660 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0     1142 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/route.py
+-rw-r--r--   0        0        0     5908 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/server/update_task.py
+-rw-r--r--   0        0        0     9369 2023-07-06 19:19:41.590126 motion_python-0.1.73/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-07-06 19:20:05.642346 motion_python-0.1.73/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.73/PKG-INFO
```

### Comparing `motion_python-0.1.72/README.md` & `motion_python-0.1.73/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.72/motion/cli.py` & `motion_python-0.1.73/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.72/motion/component.py` & `motion_python-0.1.73/motion/component.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,103 +16,103 @@
 
         AdderComponent = Component("MyAdder")
 
         @AdderComponent.init_state
         def setUp():
             return {"value": 0}
 
-        @AdderComponent.infer("add")
+        @AdderComponent.serve("add")
         def plus(state, value):
             return state["value"] + value
 
-        @AdderComponent.fit("add")
-        def add(state, value, infer_result):
+        @AdderComponent.update("add")
+        def add(state, value, serve_result):
             return {"value": state["value"] + value}
 
         if __name__ == "__main__":
             c = AdderComponent() # Create instance of AdderComponent
-            c.run("add", kwargs={"value": 1}, flush_fit=True) # Blocks until fit
-            # is done. Resulting state is {"value": 1}
+            c.run("add", kwargs={"value": 1}, flush_update=True) # Blocks
+            # until update is done. Resulting state is {"value": 1}
             c.run("add", kwargs={"value": 2}) # Will return 3, not waiting
-            # for fit operation.
+            # for update operation.
             # Resulting state will eventually be {"value": 3}
         ```
 
     === "Multiple Dataflows"
         ```python
         from motion import Component
 
         Calculator = Component("MyCalculator")
 
         @Calculator.init_state
         def setUp():
             return {"value": 0}
 
-        @Calculator.infer("add")
+        @Calculator.serve("add")
         def plus(state, value):
             return state["value"] + value
 
-        @Calculator.fit("add")
-        def increment(state, infer_result, value):
+        @Calculator.update("add")
+        def increment(state, serve_result, value):
             return {"value": state["value"] + value}
 
-        @Calculator.infer("subtract")
+        @Calculator.serve("subtract")
         def minus(state, value):
             return state["value"] - value
 
-        @Calculator.fit("subtract")
-        def decrement(state, infer_result, value):
+        @Calculator.update("subtract")
+        def decrement(state, serve_result, value):
             return {"value": state["value"] - value}
 
         if __name__ == "__main__":
             c = Calculator()
-            c.run("add", kwargs={"value": 1}, flush_fit=True) # Will return 1,
-            # blocking until fit is done. Resulting state is {"value": 1}
-            c.run("subtract", kwargs={"value": 1}, flush_fit=True)
-            # Will return 0, blocking until fit is done. Resulting state is #
+            c.run("add", kwargs={"value": 1}, flush_update=True) # Will return 1,
+            # blocking until update is done. Resulting state is {"value": 1}
+            c.run("subtract", kwargs={"value": 1}, flush_update=True)
+            # Will return 0, blocking until update is done. Resulting state is #
             # {"value": 0}
         ```
 
-    === "Batching Fit Operations"
+    === "Batching update operations"
 
         ```python
         from motion import Component
         import numpy as np
 
         MLMonitor = Component("Monitoring_ML_Component")
 
         @MLMonitor.init_state
         def setUp():
             return {
                 "model": YOUR_MODEL_HERE,
                 "historical_values": [],
-                "historical_infer_results": []
+                "historical_serve_results": []
             }
 
-        @MLMonitor.infer("features")
+        @MLMonitor.serve("features")
         def predict(state, value):
             return state["model"].predict(value)
 
-        @MLMonitor.fit("features")
-        def monitor(state, value, infer_result):
+        @MLMonitor.update("features")
+        def monitor(state, value, serve_result):
 
             values = state["historical_values"] + [value]
-            infer_results = state["historical_infer_results"] + [infer_result]
+            serve_results = state["historical_serve_results"] + [serve_result]
 
             # Check drift every 10 values
             if len(values) == 10:
-                if YOUR_ANOMALY_ALGORITHM(values, infer_results):
+                if YOUR_ANOMALY_ALGORITHM(values, serve_results):
                     # Fire an alert
                     YOUR_ALERT_FUNCTION()
                 values = []
-                infer_results = []
+                serve_results = []
 
             return {
                 "historical_values": values,
-                "historical_infer_results": infer_results
+                "historical_serve_results": serve_results
             }
 
         if __name__ == "__main__":
             c = MLMonitor() # Create instance
             c.run(features=YOUR_FEATURES_HERE)
 
             for _ in range(100):
@@ -132,16 +132,16 @@
                     Usage: `C.params["param_name"]` if C is the Component you
                     have created.
         """
         self._name = name
         self._params = CustomDict(name, "params", "", params)
 
         # Set up routes
-        self._infer_routes: Dict[str, Route] = {}
-        self._fit_routes: Dict[str, List[Route]] = {}
+        self._serve_routes: Dict[str, Route] = {}
+        self._update_routes: Dict[str, List[Route]] = {}
         self._init_state_func: Optional[Callable] = None
         self._save_state_func: Optional[Callable] = None
         self._load_state_func: Optional[Callable] = None
 
     @property
     def name(self) -> str:
         """Name of the component.
@@ -156,26 +156,26 @@
 
         Returns:
             str: Component name.
         """
         return self._name
 
     def add_route(self, key: str, op: str, udf: Callable) -> None:
-        if op == "infer":
-            if key in self._infer_routes.keys():
+        if op == "serve":
+            if key in self._serve_routes.keys():
                 raise ValueError(
-                    f"Cannot have more than one infer route for key `{key}`."
+                    f"Cannot have more than one serve route for key `{key}`."
                 )
 
-            self._infer_routes[key] = Route(key=key, op=op, udf=udf)
-        elif op == "fit":
-            if key not in self._fit_routes.keys():
-                self._fit_routes[key] = []
+            self._serve_routes[key] = Route(key=key, op=op, udf=udf)
+        elif op == "update":
+            if key not in self._update_routes.keys():
+                self._update_routes[key] = []
 
-            self._fit_routes[key].append(Route(key=key, op=op, udf=udf))
+            self._update_routes[key].append(Route(key=key, op=op, udf=udf))
 
         else:
             raise ValueError(f"Invalid op `{op}`.")
 
     @property
     def params(self) -> Dict[str, Any]:
         """Parameters to use in component functions.
@@ -189,15 +189,15 @@
             params={"param1": 1, "param2": 2}
         )
 
         @MyComponent.init_state
         def setUp():
             return {"value": 0}
 
-        @MyComponent.infer("add")
+        @MyComponent.serve("add")
         def plus(state, value):
             # Access params with MyComponent.params["param_name"]
             return state["value"] + value + MyComponent.params["param1"] +
             MyComponent.params["param2"]
         ```
 
         Returns:
@@ -282,159 +282,157 @@
 
         Returns:
             Callable: Decorated load_state function.
         """
         self._load_state_func = func
         return func
 
-    def infer(self, keys: Union[str, List[str]]) -> Callable:
-        """Decorator for any infer operation for a dataflow through the
+    def serve(self, keys: Union[str, List[str]]) -> Callable:
+        """Decorator for any serve operation for a dataflow through the
         component. Takes in a string or list of strings that represents the
         dataflow key. If the decorator is called with a list of strings, each
-        dataflow key will be mapped to the same infer function.
+        dataflow key will be mapped to the same serve function.
 
-        2 arguments required for an infer operation:
+        1 argument required for an serve operation:
             * `state`: The current state of the component, which is a
-                dictionary with string keys and any type values.
-            * `value`: The value passed in through a `c.run` call with the
-                `key` argument.
+                dictionary with string keys and any-type values.
 
-        Components can have multiple infer ops, but no dataflow key within
-        the component can have more than one infer op. Infer ops should not
+        Components can have multiple serve ops, but no dataflow key within
+        the component can have more than one serve op. serve ops should not
         modify the state object. If you want to modify the state object, use
-        the `fit` decorator.
+        the `update` decorator.
 
         Example Usage:
         ```python
         from motion import Component
 
         MyComponent = Component("MyComponent")
 
         @MyComponent.init_state
         def setUp():
             return {"value": 0}
 
-        @MyComponent.infer("add")
+        @MyComponent.serve("add")
         def add(state, value):
             return state["value"] + value
 
-        @MyComponent.infer("multiply")
+        @MyComponent.serve("multiply")
         def multiply(state, value):
             return state["value"] * value
 
         c = MyComponent()
-        c.run("add", kwargs={"value": 1}, flush_fit=True) # Returns 1
+        c.run("add", kwargs={"value": 1}, flush_update=True) # Returns 1
         c.run("multiply", kwargs={"value": 2}) # Returns 2
         ```
 
         Args:
             keys (Union[str, List[str]]): String or list of strings that
-                represent the input keyword(s) for the infer dataflow.
+                represent the input keyword(s) for the serve dataflow.
 
         Returns:
-            Callable: Decorated infer function.
+            Callable: Decorated serve function.
         """
         if isinstance(keys, str):
             keys = [keys]
 
         for key in keys:
             if "::" in key:
                 raise ValueError(
                     f"Dataflow key {key} should not have a double colon (::)"
                 )
 
         def decorator(func: Callable) -> Any:
             # type_hint = get_type_hints(func).get("value", None)
-            if not validate_args(inspect.signature(func).parameters, "infer"):
+            if not validate_args(inspect.signature(func).parameters, "serve"):
                 raise ValueError(
-                    f"Infer function {func.__name__} should have arguments " + "`state`"
+                    f"serve function {func.__name__} should have arguments " + "`state`"
                 )
 
-            func._op = "infer"  # type: ignore
+            func._op = "serve"  # type: ignore
 
             for key in keys:
                 self.add_route(key, func._op, func)  # type: ignore
 
             return func
 
         return decorator
 
-    def fit(self, keys: Union[str, List[str]]) -> Any:
-        """Decorator for any fit operations for dataflows through the
+    def update(self, keys: Union[str, List[str]]) -> Any:
+        """Decorator for any update operations for dataflows through the
         component. Takes in a string or list of strings that represents the
         dataflow key. If the decorator is called with a list of strings, each
-        dataflow key will be mapped to the same fit operation.
+        dataflow key will be mapped to the same update operation.
 
-        2 arguments required for a fit operation:
+        2 arguments required for a update operation:
             - `state`: The current state of the component, represented as a
             dictionary.
-            - `infer_result`: The result from the infer op that occurred before.
+            - `serve_result`: The result from the serve op that occurred before.
 
-        Components can have multiple fit ops, and the same key can also have
-        multiple fit ops. Fit functions should return a dictionary
+        Components can have multiple update ops, and the same key can also have
+        multiple update ops. Update functions should return a dictionary
         of state updates to be merged with the current state.
 
         Example Usage:
         ```python
         from motion import Component
 
         MyComponent = Component("MyComponent")
 
         @MyComponent.init_state
         def setUp():
             return {"value": 0}
 
-        @MyComponent.fit("add")
+        @MyComponent.update("add")
         def add(state, values):
             return {"value": state["value"] + sum(values)}
 
-        @MyComponent.infer("multiply")
+        @MyComponent.serve("multiply")
         def multiply(state, value):
             return state["value"] * value
 
-        @MyComponent.fit("multiply")
-        def multiply(state, infer_result, value):
+        @MyComponent.update("multiply")
+        def multiply(state, serve_result, value):
             return state["value"] * value
 
         c = MyComponent()
-        c.run("add", kwargs={"value": 1}, flush_fit=True) # Returns 1
-        c.run("multiply", kwargs={"value": 2}) # Returns 2, fit not executed yet
-        c.run("multiply", kwargs={"value": 3}) # Returns 3, fit will execute
+        c.run("add", kwargs={"value": 1}, flush_update=True) # Returns 1
+        c.run("multiply", kwargs={"value": 2}) # Returns 2, update not executed yet
+        c.run("multiply", kwargs={"value": 3}) # Returns 3, update will execute
         # to get state["value"] = 6
         # Some time later...
         c.run("multiply", kwargs={"value": 4}) # Returns 24
         ```
 
         Args:
             keys (Union[str, List[str]]): String or list of strings that
-                represent the input keyword(s) for the fit dataflow.
+                represent the input keyword(s) for the update dataflow.
 
         Returns:
-            Callable: Decorated fit function.
+            Callable: Decorated update function.
         """
         frame = inspect.currentframe().f_back  # type: ignore
         fname = frame.f_code.co_name  # type: ignore
         if fname != "<module>":
             raise ValueError(
-                f"Component {self.name} fit method must be defined in a module "
+                f"Component {self.name} update method must be defined in a module "
                 + f"context. It's currently initialized from function {fname}."
             )
         if isinstance(keys, str):
             keys = [keys]
 
         def decorator(func: Callable) -> Any:
-            if not validate_args(inspect.signature(func).parameters, "fit"):
+            if not validate_args(inspect.signature(func).parameters, "update"):
                 raise ValueError(
                     f"Fit method {func.__name__} should have >= 2 arguments: "
-                    + "`state` and `infer_result`."
+                    + "`state` and `serve_result`."
                 )
 
             # func._input_key = key  # type: ignore
             # func._batch_size = batch_size  # type: ignore
-            func._op = "fit"  # type: ignore
+            func._op = "update"  # type: ignore
 
             for key in keys:
                 self.add_route(key, func._op, func)  # type: ignore
 
             return func
 
         return decorator
@@ -455,19 +453,19 @@
 
         MyComponent = Component("MyComponent")
 
         @MyComponent.init_state
         def setUp(starting_val):
             return {"value": starting_val}
 
-        # Define infer and fit operations
-        @MyComponent.infer("key1")
+        # Define serve and update operations
+        @MyComponent.serve("key1")
         def ...
 
-        @MyComponent.fit("key1)
+        @MyComponent.update("key1)
         def ...
 
         # Creates instance of MyComponent
         if __name__ == "__main__":
             c_instance = MyComponent(init_state_params={"starting_val": 3})
             c_instance.run(..)
         ```
@@ -502,48 +500,48 @@
             ci = ComponentInstance(
                 component_name=self.name,
                 instance_name=instance_name,
                 init_state_func=self._init_state_func,
                 init_state_params=init_state_params,
                 save_state_func=self._save_state_func,
                 load_state_func=self._load_state_func,
-                infer_routes=self._infer_routes,
-                fit_routes=self._fit_routes,
+                serve_routes=self._serve_routes,
+                update_routes=self._update_routes,
                 logging_level=logging_level,
                 disabled=disabled,
             )
         except RuntimeError:
             raise RuntimeError(
                 "Error creating component instance. Make sure the entry point "
                 + "of your program is protected, using `if __name__ == '__main__':`"
             )
 
         return ci
 
     def get_graph(self, x_offset_step: int = 600) -> Dict[str, Any]:
         """
-        Gets the graph of infer and fit ops for this component.
+        Gets the graph of serve and update ops for this component.
         """
 
         graph: Dict[str, Dict[str, Any]] = {}
 
-        for key, route in self._infer_routes.items():
+        for key, route in self._serve_routes.items():
             graph[key] = {
-                "infer": {
+                "serve": {
                     "name": route.udf.__name__,
                     "udf": inspect.getsource(route.udf),
                 },
             }
 
-        for key, routes in self._fit_routes.items():
+        for key, routes in self._update_routes.items():
             if key not in graph:
                 graph[key] = {}
-            graph[key]["fit"] = []
+            graph[key]["update"] = []
             for route in routes:
-                graph[key]["fit"].append(
+                graph[key]["update"].append(
                     {
                         "name": route.udf.__name__,
                         "udf": inspect.getsource(route.udf),
                         # "batch_size": route.udf._batch_size,  # type: ignore
                     }
                 )
 
@@ -579,82 +577,82 @@
                 "position": {"x": 0, "y": key_y_position},
                 "data": {"label": key},
                 "type": "key",
             }
             nodes.append(key_node)
             node_id += 1
 
-            # Assign x position for infer nodes
-            infer_x_offset = x_offset
+            # Assign x position for serve nodes
+            serve_x_offset = x_offset
 
-            if "infer" in value.keys():
-                # Add infer node
-                infer_node = {
+            if "serve" in value.keys():
+                # Add serve node
+                serve_node = {
                     "id": str(node_id),
-                    "position": {"x": infer_x_offset, "y": key_y_position},
+                    "position": {"x": serve_x_offset, "y": key_y_position},
                     "data": {
-                        "label": value["infer"]["name"],
-                        "udf": value["infer"]["udf"],
+                        "label": value["serve"]["name"],
+                        "udf": value["serve"]["udf"],
                     },
-                    "type": "infer",
+                    "type": "serve",
                 }
-                nodes.append(infer_node)
+                nodes.append(serve_node)
                 edges.append(
                     {
-                        "id": "e{}-{}".format(key_node["id"], infer_node["id"]),
+                        "id": "e{}-{}".format(key_node["id"], serve_node["id"]),
                         "source": key_node["id"],
-                        "target": infer_node["id"],
+                        "target": serve_node["id"],
                         "targetHandle": "left",
                     }
                 )
                 edges.append(
                     {
-                        "id": "e{}-{}".format(state_node["id"], infer_node["id"]),
+                        "id": "e{}-{}".format(state_node["id"], serve_node["id"]),
                         "source": state_node["id"],
-                        "target": infer_node["id"],
+                        "target": serve_node["id"],
                         "targetHandle": "top",
                     }
                 )
                 node_id += 1
 
-            # Assign x position for fit nodes
-            infer_x_offset += x_offset_step
-            fit_x_offset = infer_x_offset
-
-            if "fit" in value.keys():
-                for fit in value["fit"]:
-                    # Add fit node
+            # Assign x position for update nodes
+            serve_x_offset += x_offset_step
+            fit_x_offset = serve_x_offset
+
+            if "update" in value.keys():
+                for update in value["update"]:
+                    # Add update node
                     fit_node = {
                         "id": str(node_id),
                         "position": {"x": fit_x_offset, "y": key_y_position},
                         "data": {
-                            "label": fit["name"],
-                            "udf": fit["udf"],
+                            "label": update["name"],
+                            "udf": update["udf"],
                             # "batch_size": fit["batch_size"],
                         },
-                        "type": "fit",
+                        "type": "update",
                     }
                     nodes.append(fit_node)
 
                     edges.append(
                         {
                             "id": "e{}-{}".format(fit_node["id"], state_node["id"]),
                             "target": state_node["id"],
                             "source": fit_node["id"],
                             "sourceHandle": "top",
                             "animated": True,  # type: ignore
                             # "label": f"batch_size: {fit['batch_size']}",
                         }
                     )
 
-                    if "infer" in value.keys():
+                    if "serve" in value.keys():
                         edges.append(
                             {
-                                "id": "e{}-{}".format(infer_node["id"], fit_node["id"]),
-                                "source": infer_node["id"],
+                                "id": "e{}-{}".format(serve_node["id"], fit_node["id"]),
+                                "source": serve_node["id"],
                                 "sourceHandle": "right",
                                 "target": fit_node["id"],
                                 "targetHandle": "left",
                                 "animated": True,  # type: ignore
                             }
                         )
                     else:
```

### Comparing `motion_python-0.1.72/motion/execute.py` & `motion_python-0.1.73/motion/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 import cloudpickle
 import psutil
 import redis
 from redis.lock import Lock
 
 from motion.route import Route
-from motion.server.fit_task import FitTask
+from motion.server.update_task import UpdateTask
 from motion.utils import (
     CustomDict,
-    FitEvent,
-    FitEventGroup,
     RedisParams,
+    UpdateEvent,
+    UpdateEventGroup,
     hash_object,
     loadState,
     logger,
     saveState,
 )
 
 
@@ -27,16 +27,16 @@
     def __init__(
         self,
         instance_name: str,
         init_state_func: Optional[Callable],
         init_state_params: Dict[str, Any],
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
-        infer_routes: Dict[str, Route],
-        fit_routes: Dict[str, List[Route]],
+        serve_routes: Dict[str, Route],
+        update_routes: Dict[str, List[Route]],
         disabled: bool = False,
     ):
         self._instance_name = instance_name
 
         self._init_state_func = init_state_func
         self._init_state_params = init_state_params
         self._load_state_func = load_state_func
@@ -78,24 +78,24 @@
             # Load state
             self._state = self._loadState()
             self.version = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
 
         self.version = int(self.version)
 
         # Set up routes
-        self._infer_routes: Dict[str, Route] = infer_routes
-        self._fit_routes: Dict[str, Dict[str, Route]] = {
+        self._serve_routes: Dict[str, Route] = serve_routes
+        self._update_routes: Dict[str, Dict[str, Route]] = {
             rkey: {route.udf.__name__: route for route in routes}
-            for rkey, routes in fit_routes.items()
+            for rkey, routes in update_routes.items()
         }
 
         # Set up shutdown event
         # self._shutdown_event = threading.Event()
 
-        # Set up fit queues, batch sizes, and threads
+        # Set up update queues, batch sizes, and threads
         self.disabled = disabled
         if not disabled:
             self._build_fit_jobs()
 
     def _connectToRedis(self) -> redis.Redis:
         rp = RedisParams()
         r = redis.Redis(
@@ -116,27 +116,27 @@
             if not isinstance(initial_state, dict):
                 raise TypeError(f"{self._instance_name} init should return a dict.")
             return initial_state
 
         return {}
 
     def _build_fit_jobs(self) -> None:
-        """Builds fit jobs."""
+        """Builds update jobs."""
         # Set up worker loops
         self.worker_tasks = {}
         # self.worker_stop_events = {}
 
         rp = RedisParams()
         # self.worker_states = {}
 
-        for rkey, routes in self._fit_routes.items():
+        for rkey, routes in self._update_routes.items():
             for udf_name, route in routes.items():
                 pname = f"{self._instance_name}::{rkey}::{udf_name}"
                 multiprocessing.Event()
-                self.worker_tasks[pname] = FitTask(
+                self.worker_tasks[pname] = UpdateTask(
                     self._instance_name,
                     route,
                     save_state_func=self._save_state_func,
                     load_state_func=self._load_state_func,
                     queue_identifier=self._get_queue_identifier(rkey, udf_name),
                     channel_identifier=self._get_channel_identifier(rkey, udf_name),
                     redis_host=rp.host,
@@ -158,22 +158,22 @@
     def _monitor_processes(self) -> None:
         rp = RedisParams()
         while not self.stop_event.is_set():
             # Loop through processes to see if they are alive
             for pname, process in self.worker_tasks.items():
                 if not process.is_alive():
                     logger.debug(
-                        f"Failed to detect heartbeat for fit task {pname}."
+                        f"Failed to detect heartbeat for update task {pname}."
                         + " Restarting the task in the background."
                     )
                     # Restart
                     rkey = pname.split("::")[1]
                     udf_name = pname.split("::")[2]
-                    route = self._fit_routes[rkey][udf_name]
-                    self.worker_tasks[pname] = FitTask(
+                    route = self._update_routes[rkey][udf_name]
+                    self.worker_tasks[pname] = UpdateTask(
                         self._instance_name,
                         route,
                         save_state_func=self._save_state_func,
                         load_state_func=self._load_state_func,
                         queue_identifier=self._get_queue_identifier(rkey, udf_name),
                         channel_identifier=self._get_channel_identifier(rkey, udf_name),
                         redis_host=rp.host,
@@ -202,15 +202,15 @@
         if self.disabled:
             return
 
         if not self.running.value:
             return
 
         if is_open:
-            logger.info("Running fit operations on remaining data...")
+            logger.info("Running update operations on remaining data...")
 
         # Set shutdown event
         self.stop_event.set()
         self.running.value = False
 
         processes_to_wait_for = []
         for process in self.worker_tasks.values():
@@ -218,15 +218,15 @@
                 # os.kill(process.pid, signal.SIGUSR1)  # type:ignore
                 # Set stop event
                 # self.worker_stop_events[pname].set()
                 processes_to_wait_for.append(process)
 
         self._redis_con.close()
 
-        # Join fit processes
+        # Join update processes
         for process in processes_to_wait_for:
             process.join()
 
         self.monitor_thread.join()
 
     def _updateState(self, new_state: Dict[str, Any]) -> None:
         if not new_state:
@@ -254,79 +254,79 @@
             )
 
             self.version = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
 
             # Release lock
             lock.release()
 
-    def _enqueue_and_trigger_fit(
+    def _enqueue_and_trigger_update(
         self,
         key: str,
         kwargs: Dict[str, Any],
-        infer_result: Any,
-        flush_fit: bool,
+        serve_result: Any,
+        flush_update: bool,
         route_hit: bool,
     ) -> bool:
-        # Run the fit routes
-        # Enqueue results into fit queues
-        if key in self._fit_routes.keys():
+        # Run the update routes
+        # Enqueue results into update queues
+        if key in self._update_routes.keys():
             route_hit = True
 
-            fit_events = FitEventGroup(key)
-            for fit_udf_name in self._fit_routes[key].keys():
-                queue_identifier: str = self._get_queue_identifier(key, fit_udf_name)
+            update_events = UpdateEventGroup(key)
+            for update_udf_name in self._update_routes[key].keys():
+                queue_identifier: str = self._get_queue_identifier(key, update_udf_name)
                 channel_identifier: str = self._get_channel_identifier(
-                    key, fit_udf_name
+                    key, update_udf_name
                 )
 
                 identifier = str(uuid4())
 
-                if flush_fit:
+                if flush_update:
                     # Add pubsub channel to listen to
-                    fit_event = FitEvent(
+                    update_event = UpdateEvent(
                         self._redis_con, channel_identifier, identifier
                     )
-                    fit_events.add(fit_udf_name, fit_event)
+                    update_events.add(update_udf_name, update_event)
 
-                # Add to fit queue
+                # Add to update queue
                 self._redis_con.rpush(
                     queue_identifier,
                     cloudpickle.dumps(
                         {
                             "kwargs": kwargs,
-                            "infer_result": infer_result,
+                            "serve_result": serve_result,
                             "identifier": identifier,
                         }
                     ),
                 )
 
-            if flush_fit:
-                # Wait for fit result to finish
-                fit_events.wait()
+            if flush_update:
+                # Wait for update result to finish
+                update_events.wait()
                 # Update state
                 self._state = self._loadState()
                 v = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
                 if not v:
                     raise ValueError(
                         f"Error loading state for {self._instance_name}."
                         + " No version found."
                     )
                 self.version = int(v)
 
         return route_hit
 
-    def _try_cached_infer(
+    def _try_cached_serve(
         self,
         key: str,
         kwargs: Dict[str, Any],
         ignore_cache: bool,
         force_refresh: bool,
     ) -> Tuple[bool, Optional[Any], Optional[str]]:
         route_run = False
-        infer_result = None
+        serve_result = None
 
         if force_refresh:
             self._state = self._loadState()
             v = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
             if not v:
                 raise ValueError(
                     f"Error loading state for {self._instance_name}."
@@ -341,162 +341,162 @@
             value_hash = None
 
         # Check if key is in cache if value can be hashed and
         # user doesn't want to force refresh state
         if value_hash and not force_refresh and not ignore_cache:
             cache_result_key = f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
             if self._redis_con.exists(cache_result_key):
-                infer_result = cloudpickle.loads(self._redis_con.get(cache_result_key))
+                serve_result = cloudpickle.loads(self._redis_con.get(cache_result_key))
                 route_run = True
 
-        return route_run, infer_result, value_hash
+        return route_run, serve_result, value_hash
 
     def run(
         self,
         key: str,
         kwargs: Dict[str, Any],
         cache_ttl: int,
         ignore_cache: bool,
         force_refresh: bool,
-        flush_fit: bool,
+        flush_update: bool,
     ) -> Any:
         route_hit = False
-        infer_result = None
+        serve_result = None
 
-        # Run the infer route
-        if key in self._infer_routes.keys():
+        # Run the serve route
+        if key in self._serve_routes.keys():
             route_hit = True
-            route_run, infer_result, value_hash = self._try_cached_infer(
+            route_run, serve_result, value_hash = self._try_cached_serve(
                 key, kwargs, ignore_cache, force_refresh
             )
 
             # If not in cache or value can't be hashed or
             # user wants to force refresh state, run route
             if not route_run:
-                infer_result = self._infer_routes[key].run(state=self._state, **kwargs)
+                serve_result = self._serve_routes[key].run(state=self._state, **kwargs)
 
-                # Check that infer_result is not an awaitable
-                if asyncio.iscoroutine(infer_result):
+                # Check that serve_result is not an awaitable
+                if asyncio.iscoroutine(serve_result):
                     raise TypeError(
                         f"Route {key} returned an awaitable. "
                         + "Call `await instance.arun(...)` instead."
                     )
 
                 # Cache result
                 if value_hash:
                     cache_result_key = (
                         f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
                     )
                     self._redis_con.set(
                         cache_result_key,
-                        cloudpickle.dumps(infer_result),
+                        cloudpickle.dumps(serve_result),
                         ex=cache_ttl,
                     )
 
-        # Run the fit routes
-        # Enqueue results into fit queues
-        route_hit = self._enqueue_and_trigger_fit(
-            key, kwargs, infer_result, flush_fit, route_hit
+        # Run the update routes
+        # Enqueue results into update queues
+        route_hit = self._enqueue_and_trigger_update(
+            key, kwargs, serve_result, flush_update, route_hit
         )
 
         if not route_hit:
             raise KeyError(f"Key {key} not in routes.")
 
-        return infer_result
+        return serve_result
 
     async def arun(
         self,
         key: str,
         kwargs: Dict[str, Any],
         cache_ttl: int,
         ignore_cache: bool,
         force_refresh: bool,
-        flush_fit: bool,
+        flush_update: bool,
     ) -> Any:
         route_hit = False
-        infer_result = None
+        serve_result = None
 
-        # Run the infer route
-        if key in self._infer_routes.keys():
+        # Run the serve route
+        if key in self._serve_routes.keys():
             route_hit = True
-            route_run, infer_result, value_hash = self._try_cached_infer(
+            route_run, serve_result, value_hash = self._try_cached_serve(
                 key, kwargs, ignore_cache, force_refresh
             )
 
             # If not in cache or value can't be hashed or
             # user wants to force refresh state, run route
             if not route_run:
-                infer_result_awaitable = self._infer_routes[key].run(
+                serve_result_awaitable = self._serve_routes[key].run(
                     state=self._state, **kwargs
                 )
-                if not asyncio.iscoroutine(infer_result_awaitable):
+                if not asyncio.iscoroutine(serve_result_awaitable):
                     raise TypeError(
                         f"Route {key} returned a non-awaitable. "
                         + "Call `instance.run(...)` instead."
                     )
 
-                infer_result = await infer_result_awaitable
+                serve_result = await serve_result_awaitable
 
                 # Cache result
                 if value_hash:
                     cache_result_key = (
                         f"MOTION_RESULT:{self._instance_name}/{key}/{value_hash}"
                     )
                     self._redis_con.set(
                         cache_result_key,
-                        cloudpickle.dumps(infer_result),
+                        cloudpickle.dumps(serve_result),
                         ex=cache_ttl,
                     )
 
-        # Run the fit routes
-        # Enqueue results into fit queues
-        route_hit = self._enqueue_and_trigger_fit(
-            key, kwargs, infer_result, flush_fit, route_hit
+        # Run the update routes
+        # Enqueue results into update queues
+        route_hit = self._enqueue_and_trigger_update(
+            key, kwargs, serve_result, flush_update, route_hit
         )
 
         if not route_hit:
             raise KeyError(f"Key {key} not in routes.")
 
-        return infer_result
+        return serve_result
 
-    def flush_fit(self, dataflow_key: str) -> None:
-        # Check if key has fit ops
-        if dataflow_key not in self._fit_routes.keys():
+    def flush_update(self, dataflow_key: str) -> None:
+        # Check if key has update ops
+        if dataflow_key not in self._update_routes.keys():
             return
 
         # Push a noop into the relevant queues
-        fit_events = FitEventGroup(dataflow_key)
-        for fit_udf_name in self._fit_routes[dataflow_key].keys():
+        update_events = UpdateEventGroup(dataflow_key)
+        for update_udf_name in self._update_routes[dataflow_key].keys():
             queue_identifier: str = self._get_queue_identifier(
-                dataflow_key, fit_udf_name
+                dataflow_key, update_udf_name
             )
             channel_identifier: str = self._get_channel_identifier(
-                dataflow_key, fit_udf_name
+                dataflow_key, update_udf_name
             )
 
             identifier = "NOOP_" + str(uuid4())
 
             # Add pubsub channel to listen to
-            fit_event = FitEvent(self._redis_con, channel_identifier, identifier)
-            fit_events.add(fit_udf_name, fit_event)
+            update_event = UpdateEvent(self._redis_con, channel_identifier, identifier)
+            update_events.add(update_udf_name, update_event)
 
-            # Add to fit queue
+            # Add to update queue
             self._redis_con.rpush(
                 queue_identifier,
                 cloudpickle.dumps(
                     {
                         "value": None,
-                        "infer_result": None,
+                        "serve_result": None,
                         "identifier": identifier,
                     }
                 ),
             )
 
-        # Wait for fit result to finish
-        fit_events.wait()
+        # Wait for update result to finish
+        update_events.wait()
         # Update state
         self._state = self._loadState()
         v = self._redis_con.get(f"MOTION_VERSION:{self._instance_name}")
         if not v:
             raise ValueError(
                 f"Error loading state for {self._instance_name}." + " No version found."
             )
```

### Comparing `motion_python-0.1.72/motion/instance.py` & `motion_python-0.1.73/motion/instance.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         self,
         component_name: str,
         instance_name: str,
         init_state_func: Optional[Callable],
         init_state_params: Optional[Dict[str, Any]],
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
-        infer_routes: Dict[str, Route],
-        fit_routes: Dict[str, List[Route]],
+        serve_routes: Dict[str, Route],
+        update_routes: Dict[str, List[Route]],
         logging_level: str = "WARNING",
         disabled: bool = False,
     ):
         """Creates a new instance of a Motion component.
 
         Args:
             name (str):
@@ -57,16 +57,16 @@
         self.disabled = disabled
         self._executor = Executor(
             self._instance_name,
             init_state_func=init_state_func,
             init_state_params=init_state_params if init_state_params else {},
             save_state_func=save_state_func,
             load_state_func=load_state_func,
-            infer_routes=infer_routes,
-            fit_routes=fit_routes,
+            serve_routes=serve_routes,
+            update_routes=update_routes,
             disabled=self.disabled,
         )
         self.running = True
 
     @property
     def instance_name(self) -> str:
         """Component name with a random phrase to represent
@@ -91,15 +91,15 @@
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
-        # Define infer and fit operations
+        # Define serve and update operations
 
         if __name__ == "__main__":
             c_instance = C()
             c_instance.run(...)
             c_instance.run(...)
             c_instance.shutdown()
         ```
@@ -118,58 +118,58 @@
         self._executor.shutdown(is_open=is_open)
 
         self.running = False
 
     def get_version(self) -> int:
         """
         Gets the state version (might be outdated) currently being
-        used for infer ops.
+        used for serve ops.
 
         Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
-        # Define infer and fit operations
+        # Define serve and update operations
 
         if __name__ == "__main__":
             c_instance = C()
             c_instance.get_version() # Returns 1 (first version)
         ```
         """
         return self._executor.version  # type: ignore
 
-    def update_state(self, state_update: Dict[str, Any]) -> None:
+    def write_state(self, state_update: Dict[str, Any]) -> None:
         """Writes the state update to the component instance's state.
-        If a fit op is currently running, the state update will be
-        applied after the fit op is finished. Warning: this could
-        take a while if your fit op takes a long time!
+        If a update op is currently running, the state update will be
+        applied after the update op is finished. Warning: this could
+        take a while if your update ops take a long time!
 
         Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
-        # Define infer and fit operations
+        # Define serve and update operations
         ...
 
         if __name__ == "__main__":
             c_instance = C()
             c_instance.read_state("value") # Returns 0
-            c_instance.update_state({"value": 1, "value2": 2})
+            c_instance.write_state({"value": 1, "value2": 2})
             c_instance.read_state("value") # Returns 1
             c_instance.read_state("value2") # Returns 2
         ```
 
         Args:
             state_update (Dict[str, Any]): Dictionary of key-value pairs
                 to update the state with.
@@ -185,15 +185,15 @@
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
-        # Define infer and fit operations
+        # Define serve and update operations
         ...
 
         if __name__ == "__main__":
             c_instance = C()
             c_instance.read_state("value") # Returns 0
             c_instance.run(...)
             c_instance.read_state("value") # This will return the current value
@@ -204,173 +204,173 @@
             key (str): Key in the state to get the value for.
 
         Returns:
             Any: Current value for the key.
         """
         return self._executor._loadState()[key]
 
-    def flush_fit(self, dataflow_key: str) -> None:
-        """Flushes the fit queue corresponding to the dataflow
+    def flush_update(self, dataflow_key: str) -> None:
+        """Flushes the update queue corresponding to the dataflow
         key, if it exists, and updates the instance state.
         Warning: this is a blocking operation and could take
-        a while if your fit op takes a long time!
+        a while if your update op takes a long time!
 
         Example Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
-        @C.infer("add")
+        @C.serve("add")
         def add(state, value):
             return state["value"] + value
 
-        @C.fit("add")
-        def add(state, value, infer_result):
+        @C.update("add")
+        def add(state, value, serve_result):
             return {"value": state["value"] + value}
 
-        @C.infer("multiply")
+        @C.serve("multiply")
         def multiply(state, value):
             return state["value"] * value
 
         if __name__ == "__main__":
             c = C() # Create instance of C
             c.run("add", kwargs={"value": 1})
-            c.flush_fit("add") # (1)!
+            c.flush_update("add") # (1)!
             c.run("add", kwargs={"value": 2}) # This will use the updated state
 
-        # 1. Waits for the fit op to finish, then updates the state
+        # 1. Waits for the update op to finish, then updates the state
         ```
 
         Args:
             dataflow_key (str): Key of the dataflow.
 
         Raises:
             RuntimeError: If the component instance was initialized to
             be disabled.
         """
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
-        self._executor.flush_fit(dataflow_key)
+        self._executor.flush_update(dataflow_key)
 
     def run(
         self,
         # *,
         dataflow_key: str,
         kwargs: Dict[str, Any] = {},
         cache_ttl: int = DEFAULT_KEY_TTL,
         ignore_cache: bool = False,
         force_refresh: bool = False,
-        flush_fit: bool = False,
+        flush_update: bool = False,
     ) -> Any:
-        """Runs the dataflow (infer and fit ops) for the keyword argument
+        """Runs the dataflow (serve and update ops) for the keyword argument
         passed in. If the key is not found to have any ops, an error
         is raised. Only one dataflow key should be passed in.
 
         Example Usage:
         ```python
         from motion import Component
 
         C = Component("MyComponent")
 
         @C.init_state
         def setUp():
             return {"value": 0}
 
-        @C.infer("add")
+        @C.serve("add")
         def add(state, value):
             return state["value"] + value
 
-        @C.fit("add")
-        def add(state, value, infer_result):
+        @C.update("add")
+        def add(state, value, serve_result):
             return {"value": state["value"] + value}
 
         if __name__ == "__main__":
             c = C() # Create instance of C
-            c.run("add", kwargs={"value": 1}, flush_fit=True) # (1)!
+            c.run("add", kwargs={"value": 1}, flush_update=True) # (1)!
             c.run("add", kwargs={"value": 1}) # Returns 1
-            c.run("add", kwargs={"value": 2}, flush_fit=True) # (2)!
+            c.run("add", kwargs={"value": 2}, flush_update=True) # (2)!
 
             c.run("add", kwargs={"value": 3})
-            time.sleep(3) # Wait for the previous fit op to finish
+            time.sleep(3) # Wait for the previous update op to finish
 
             c.run("add", kwargs={"value": 3}, force_refresh=True) # (3)!
 
-        # 1. Waits for the fit op to finish, then updates the state
+        # 1. Waits for the update op to finish, then updates the state
         # 2. Returns 2, result state["value"] = 4
         # 3. Force refreshes the state before running the dataflow, and
-        #    reruns the infer op even though the result might be cached.
+        #    reruns the serve op even though the result might be cached.
         ```
 
 
         Args:
             dataflow_key (str): Key of the dataflow to run.
             kwargs (Dict[str, Any]): Keyword arguments to pass into the
                 dataflow ops, in addition to the state.
             cache_ttl (int, optional):
-                How long the inference result should live in a cache (in
+                How long the serveence result should live in a cache (in
                 seconds). Defaults to 1 day (60 * 60 * 24).
             ignore_cache (bool, optional):
-                If True, ignores the cache and runs the infer op. Does not
+                If True, ignores the cache and runs the serve op. Does not
                 force refresh the state. Defaults to False.
             force_refresh (bool, optional): Read the latest value of the
-                state before running an inference call, otherwise a stale
+                state before running an serveence call, otherwise a stale
                 version of the state or a cached result may be used.
                 Defaults to False.
-            flush_fit (bool, optional):
-                If True, waits for the fit op to finish executing before
-                returning. If the fit queue hasn't reached batch_size
-                yet, the fit op runs anyways. Force refreshes the
-                state after the fit op completes. Defaults to False.
+            flush_update (bool, optional):
+                If True, waits for the update op to finish executing before
+                returning. If the update queue hasn't reached batch_size
+                yet, the update op runs anyways. Force refreshes the
+                state after the update op completes. Defaults to False.
 
         Returns:
-            Any: Result of the inference call. Might take a long time
-            to run if `flush_fit = True` and the fit operation is
+            Any: Result of the serveence call. Might take a long time
+            to run if `flush_update = True` and the update operation is
             computationally expensive.
         """
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
-        infer_result = self._executor.run(
+        serve_result = self._executor.run(
             key=dataflow_key,
             kwargs=kwargs,
             cache_ttl=cache_ttl,
             ignore_cache=ignore_cache,
             force_refresh=force_refresh,
-            flush_fit=flush_fit,
+            flush_update=flush_update,
         )
 
-        return infer_result
+        return serve_result
 
     async def arun(
         self,
         # *,
         dataflow_key: str,
         kwargs: Dict[str, Any] = {},
         cache_ttl: int = DEFAULT_KEY_TTL,
         ignore_cache: bool = False,
         force_refresh: bool = False,
-        flush_fit: bool = False,
+        flush_update: bool = False,
     ) -> Awaitable[Any]:
-        """Async version of run. Runs the dataflow (infer and fit ops) for the
+        """Async version of run. Runs the dataflow (serve and update ops) for the
         specified key.
 
         Example Usage:
         ```python
         from motion import Component
         import asyncio
 
         C = Component("MyComponent")
 
-        @C.infer("sleep")
+        @C.serve("sleep")
         async def sleep(state, value):
             await asyncio.sleep(value)
             return "Slept!"
 
         async def main():
             c = C()
             await c.arun("sleep", kwargs={"value": 1})
@@ -380,47 +380,47 @@
         ```
 
         Args:
             dataflow_key (str): Key of the dataflow to run.
             kwargs (Dict[str, Any]): Keyword arguments to pass into the
                 dataflow ops, in addition to the state.
             cache_ttl (int, optional):
-                How long the inference result should live in a cache (in
+                How long the serveence result should live in a cache (in
                 seconds). Defaults to 1 day (60 * 60 * 24).
             ignore_cache (bool, optional):
-                If True, ignores the cache and runs the infer op. Does not
+                If True, ignores the cache and runs the serve op. Does not
                 force refresh the state. Defaults to False.
             force_refresh (bool, optional): Read the latest value of the
-                state before running an inference call, otherwise a stale
+                state before running an serveence call, otherwise a stale
                 version of the state or a cached result may be used.
                 Defaults to False.
-            flush_fit (bool, optional):
-                If True, waits for the fit op to finish executing before
-                returning. If the fit queue hasn't reached batch_size
-                yet, the fit op runs anyways. Force refreshes the
-                state after the fit op completes. Defaults to False.
+            flush_update (bool, optional):
+                If True, waits for the update op to finish executing before
+                returning. If the update queue hasn't reached batch_size
+                yet, the update op runs anyways. Force refreshes the
+                state after the update op completes. Defaults to False.
             **kwargs:
-                Keyword arguments for the infer and fit ops. You can only
+                Keyword arguments for the serve and update ops. You can only
                 pass in one pair.
 
         Raises:
             ValueError: If more than one dataflow key-value pair is passed.
             RuntimeError: If the component instance was initialized to
             be disabled.
 
         Returns:
-            Awaitable[Any]: Awaitable Result of the inference call.
+            Awaitable[Any]: Awaitable Result of the serveence call.
         """
         if self.disabled:
             raise RuntimeError("Cannot run a disabled component instance.")
 
-        infer_result = await self._executor.arun(
+        serve_result = await self._executor.arun(
             key=dataflow_key,
             kwargs=kwargs,
             # value=value,
             cache_ttl=cache_ttl,
             ignore_cache=ignore_cache,
             force_refresh=force_refresh,
-            flush_fit=flush_fit,
+            flush_update=flush_update,
         )  # type: ignore
 
-        return infer_result  # type: ignore
+        return serve_result  # type: ignore
```

### Comparing `motion_python-0.1.72/motion/migrate.py` & `motion_python-0.1.73/motion/migrate.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.72/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.73/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.72/motion/route.py` & `motion_python-0.1.73/motion/route.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from pydantic import BaseModel, Field, PrivateAttr
 
 from motion.utils import logger
 
 
 class Route(BaseModel):
     key: str = Field(..., description="The keyword to which this route applies.")
-    op: str = Field(..., description="The operation to perform.", regex="^(infer|fit)$")
+    op: str = Field(
+        ..., description="The operation to perform.", regex="^(serve|update)$"
+    )
     udf: Callable = Field(
         ...,
         description="The udf to call for the op. The udf should have at least "
         + "a `state` argument.",
     )
     _udf_params: Dict[str, Any] = PrivateAttr()
```

### Comparing `motion_python-0.1.72/motion/server/fit_task.py` & `motion_python-0.1.73/motion/server/update_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import redis
 from redis.lock import Lock
 
 from motion.route import Route
 from motion.utils import loadState, logger, saveState
 
 
-class FitTask(multiprocessing.Process):
+class UpdateTask(multiprocessing.Process):
     def __init__(
         self,
         instance_name: str,
         route: Route,
         # batch_size: int,
         save_state_func: Optional[Callable],
         load_state_func: Optional[Callable],
@@ -24,15 +24,15 @@
         redis_host: str,
         redis_port: int,
         redis_db: int,
         redis_password: str,
         running: Any,
     ):
         super().__init__()
-        self.name = f"FitTask-{instance_name}-{route.key}-{route.udf.__name__}"
+        self.name = f"UpdateTask-{instance_name}-{route.key}-{route.udf.__name__}"
         self.instance_name = instance_name
         self.save_state_func = save_state_func
         self.load_state_func = load_state_func
         self.redis_host = redis_host
         self.redis_port = redis_port
         self.redis_db = redis_db
         self.redis_password = redis_password
@@ -75,15 +75,15 @@
                     if not self.running.value:
                         break  # no more items in the list
                     else:
                         continue
 
                 item = cloudpickle.loads(full_item[1])
                 # self.batch.append(item)
-                # if flush_fit:
+                # if flush_update:
                 #     break
             except redis.exceptions.ConnectionError:
                 logger.error("Connection to redis lost.")
                 break
 
             # Check if we should stop
             if not self.running.value and not item:
@@ -103,33 +103,33 @@
                             "identifier": item["identifier"],
                             "exception": exception_str,
                         }
                     ),
                 )
                 continue
 
-            # Run fit op
+            # Run update op
             acquired_lock = lock.acquire(blocking=True)
             if acquired_lock:
                 try:
                     old_state = loadState(
                         redis_con, self.instance_name, self.load_state_func
                     )
                     state_update = self.route.run(
                         state=old_state,
-                        infer_result=item["infer_result"],
+                        serve_result=item["serve_result"],
                         **item["kwargs"],
                     )
                     # Await if state_update is a coroutine
                     if asyncio.iscoroutine(state_update):
                         state_update = asyncio.run(state_update)
 
                     if not isinstance(state_update, dict):
                         logger.error(
-                            "fit methods should return a dict of state updates."
+                            "Update methods should return a dict of state updates."
                         )
                     else:
                         old_state.update(state_update)
                         saveState(
                             old_state,
                             redis_con,
                             self.instance_name,
@@ -165,14 +165,14 @@
 
     #     # Add outstanding batch back to queue
     #     for item in self.batch:
     #         # Pickle item object
     #         pickled_item = cloudpickle.dumps(
     #             (
     #                 item,
-    #                 False,  # flush_fit should be False
+    #                 False,  # flush_update should be False
     #             )
     #         )
 
     #         redis_con.lpush(self.queue_identifier, pickled_item)
 
     #     self.batch = []
```

### Comparing `motion_python-0.1.72/motion/utils.py` & `motion_python-0.1.73/motion/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             )
 
 
 def validate_args(parameters: Any, op: str) -> bool:
     if "state" not in parameters.keys():
         return False
 
-    if op == "fit" and "infer_result" not in parameters.keys():
+    if op == "update" and "serve_result" not in parameters.keys():
         return False
 
     return True
 
 
 def configureLogging(level: str) -> None:
     handler = logging.StreamHandler()
@@ -220,16 +220,16 @@
 
     state_pickled = cloudpickle.dumps(state_to_save)
 
     redis_con.set(f"MOTION_STATE:{instance_name}", state_pickled)
     redis_con.incr(f"MOTION_VERSION:{instance_name}")
 
 
-class FitEvent:
-    """Waits for a fit operation to finish."""
+class UpdateEvent:
+    """Waits for a update operation to finish."""
 
     def __init__(self, redis_con: redis.Redis, channel: str, identifier: str) -> None:
         self.channel = channel
         self.pubsub = redis_con.pubsub()
         self.identifier = identifier
         self.pubsub.subscribe(channel)
 
@@ -253,58 +253,58 @@
                 break
 
             else:
                 if message_data_str == self.identifier:
                     break
 
 
-class FitEventGroup:
-    """Stores the events for fit operations on a given key."""
+class UpdateEventGroup:
+    """Stores the events for update operations on a given key."""
 
     def __init__(self, key: str) -> None:
         self.key = key
-        self.events: Dict[str, FitEvent] = {}
+        self.events: Dict[str, UpdateEvent] = {}
 
-    def add(self, udf_name: str, event: FitEvent) -> None:
+    def add(self, udf_name: str, event: UpdateEvent) -> None:
         self.events[udf_name] = event
 
     def wait(self) -> None:
-        """Waits for all fit operations for this dataflow key
+        """Waits for all update operations for this dataflow key
         to finish. Be careful not to trigger an infinite wait if the batch_size
         has not been hit yet!
 
         Example usage:
         ```python
         from motion import Component
 
         c = Component("MyComponent")
 
         @c.init_state
         def setUp():
             return {"state_val": 0, "state_val2": 0}
 
-        @c.fit("my_key")
-        def fit1(state, values, infer_results):
+        @c.update("my_key")
+        def fit1(state, values, serve_results):
             return {"state_val": state["state_val"] + sum(values)}
 
-        @c.fit("my_key")
-        def fit2(state, values, infer_results):
+        @c.update("my_key")
+        def fit2(state, values, serve_results):
             return {"state_val2": state["state_val2"] + sum(values)}
 
         result, fit_tasks = c.run(my_key=1)
-        print(result) # None because no infer op was hit
-        fit_tasks.wait() # Wait for all fit tasks to finish
+        print(result) # None because no serve op was hit
+        fit_tasks.wait() # Wait for all update tasks to finish
         # Now `state["state_val"] = 1` and `state["state_val2"] = 1`
         ```
         """
         for event in self.events.values():
             event.wait()
 
     def __str__(self) -> str:
-        return f"FitEventGroup(key={self.key}, events={self.events})"
+        return f"UpdateEventGroup(key={self.key}, events={self.events})"
 
     def __repr__(self) -> str:
         return self.__str__()
 
 
 def random_passphrase(num_words: int = 3) -> str:
     """Generate random passphrase from eff wordlist."""
```

### Comparing `motion_python-0.1.72/pyproject.toml` & `motion_python-0.1.73/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.72"
+version = "0.1.73"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.72/PKG-INFO` & `motion_python-0.1.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.72
+Version: 0.1.73
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

