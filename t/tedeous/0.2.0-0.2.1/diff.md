# Comparing `tmp/tedeous-0.2.0.tar.gz` & `tmp/tedeous-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tedeous-0.2.0.tar", last modified: Tue Jun 13 14:33:23 2023, max compression
+gzip compressed data, was "tedeous-0.2.1.tar", last modified: Thu Jul  6 13:22:11 2023, max compression
```

## Comparing `tedeous-0.2.0.tar` & `tedeous-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:33:23.857148 tedeous-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-13 14:33:17.000000 tedeous-0.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 14:33:23.857148 tedeous-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-13 14:33:17.000000 tedeous-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:33:23.857148 tedeous-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-13 14:33:17.000000 tedeous-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:33:23.857148 tedeous-0.2.0/tedeous/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15995 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/derivative.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/finite_diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/input_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/points_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-06-13 14:33:17.000000 tedeous-0.2.0/tedeous/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:33:23.857148 tedeous-0.2.0/tedeous.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 14:33:23.000000 tedeous-0.2.0/tedeous.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:11.774417 tedeous-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 13:22:06.000000 tedeous-0.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 13:22:11.774417 tedeous-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-06 13:22:06.000000 tedeous-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:22:11.774417 tedeous-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-06 13:22:06.000000 tedeous-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:11.770417 tedeous-0.2.1/tedeous/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16374 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11410 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/derivative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/finite_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/input_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/points_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16472 2023-07-06 13:22:06.000000 tedeous-0.2.1/tedeous/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:22:11.770417 tedeous-0.2.1/tedeous.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:22:11.000000 tedeous-0.2.1/tedeous.egg-info/top_level.txt
```

### Comparing `tedeous-0.2.0/LICENCE` & `tedeous-0.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/PKG-INFO` & `tedeous-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.2.0
+Version: 0.2.1
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tedeous-0.2.0/README.rst` & `tedeous-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/setup.py` & `tedeous-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def get_requirements():
     requirements = extract_requirements('requirements.txt')
     return requirements
 
 setup(
     name = 'tedeous',
-    version= '0.2.0' ,
+    version= '0.2.1' ,
     description = 'TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library',
     long_description = 'Combine power of pytorch, numerical methods and math overall to conquer and solve ALL {O,P}DEs. There are some examples to provide a little insight to an operator form',
     author = 'Alexander Hvatov',
     author_email = 'itmo.nss.team@gmail.com', # add email
     classifiers = [      
               'Development Status :: 3 - Alpha',
               'Programming Language :: Python :: 3',
```

### Comparing `tedeous-0.2.0/tedeous/cache.py` & `tedeous-0.2.1/tedeous/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 from typing import Union, Tuple, Any
 
 from tedeous.metrics import Solution
 from tedeous.input_preprocessing import Equation, EquationMixin
 from tedeous.device import device_type
 
 
+def count_output(model):
+    modules, output_layer = list(model.modules()), None
+    for layer in reversed(modules):
+        if hasattr(layer, 'out_features'):
+            output_layer = layer.out_features
+            break
+    return output_layer
+
+
 def create_random_fn(eps):
     def randomize_params(m):
         if type(m) == torch.nn.Linear or type(m) == torch.nn.Conv2d:
             m.weight.data = m.weight.data + \
                             (2 * torch.randn(m.weight.size()) - 1) * eps
             m.bias.data = m.bias.data + (2 * torch.randn(m.bias.size()) - 1) * eps
 
@@ -86,29 +95,30 @@
             * **init_model** -- [nn.Sequential or nn.ModuleList] \n
             * **model** -- [nn.Sequential or nn.ModuleList].
         """
         try:
             model[0]
         except:
             model = model.model
-        
+
         try:
             init_model[0]
         except:
             init_model = init_model.model
         
         return init_model, model
         
 
     def cache_lookup(self, lambda_bound: float = 0.001, weak_form: None = None, cache_dir: str = '../cache/',
-                nmodels: Union[int, None] = None, cache_verbose: bool = False) -> Tuple[dict, torch.Tensor]:
+                nmodels: Union[int, None] = None, save_graph: bool = False, cache_verbose: bool = False) -> Tuple[dict, torch.Tensor]:
         """
         Looking for a saved cache.
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
+            save_graph: boolean constant, responsible for saving the computational graph.
             cache_dir: directory where saved cache in.
             nmodels: maximal number of models that are looked before optimization
             cache_verbose: more detailed info about models in cache.
         Returns:
             * **best_checkpoint** -- best model with optimizator state.\n
             * **min_loss** -- minimum error in pre-trained error.
         """
@@ -133,29 +143,29 @@
             # this one for the input shape fix if needed
             
             solver_model, cache_model = self.model_reform(self.model, model)
 
             if cache_model[0].in_features != solver_model[0].in_features:
                 continue
             try:
-                if cache_model[-1].out_features != solver_model[-1].out_features:
+                if count_output(model) != count_output(self.model):
                     continue
             except Exception:
                 continue
             model = model.to(device)
-            l = Solution(self.grid, self.equal_cls, model, self.mode). \
-                loss_evaluation(lambda_bound=lambda_bound, weak_form=weak_form)
-            if l < min_loss:
-                min_loss = l
+            loss = Solution(self.grid, self.equal_cls, model, self.mode). \
+                loss_evaluation(lambda_bound=lambda_bound, weak_form=weak_form, save_graph=save_graph)
+            if loss < min_loss:
+                min_loss = loss
                 best_checkpoint['model'] = model
                 best_checkpoint['model_state_dict'] = model.state_dict()
                 best_checkpoint['optimizer_state_dict'] = \
                     checkpoint['optimizer_state_dict']
                 if cache_verbose:
-                    print('best_model_num={} , loss={}'.format(i, l))
+                    print('best_model_num={} , loss={}'.format(i, loss))
         if best_checkpoint == {}:
             best_checkpoint = None
             min_loss = np.inf
         return best_checkpoint, min_loss
 
     def save_model(self, prep_model: Any, state: dict, optimizer_state: dict,
                    cache_dir='../cache/', name: Union[str, None] = None):
```

### Comparing `tedeous-0.2.0/tedeous/config.py` & `tedeous-0.2.1/tedeous/config.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous/derivative.py` & `tedeous-0.2.1/tedeous/derivative.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous/device.py` & `tedeous-0.2.1/tedeous/device.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous/finite_diffs.py` & `tedeous-0.2.1/tedeous/finite_diffs.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous/input_preprocessing.py` & `tedeous-0.2.1/tedeous/input_preprocessing.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous/metrics.py` & `tedeous-0.2.1/tedeous/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,35 +302,43 @@
         self.model = model.to(device_type())
         self.mode = mode
         self.operator = DE_operator(self.grid, self.prepared_operator, self.model,
                                    self.mode)
         self.bconds = Bounds(self.grid, self.prepared_bconds, self.model,
                                    self.mode)
 
-    def default_loss(self, lambda_bound:  Union[int, float] = 10):
+    def default_loss(self, lambda_bound:  Union[int, float] = 10, save_graph: bool = True):
         """
         Computes l2 loss.
         Args:
+            save_graph: boolean constant, responsible for saving the computational graph.
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
         Returns:
             model loss.
         """
         op = self.operator.pde_compute()
 
         if self.prepared_bconds == None:
-            return torch.sum(torch.mean((op) ** 2, 0))
+            return torch.sum(torch.mean(op ** 2, 0))
 
         b_val, true_b_val = self.bconds.apply_bconds_operator()
 
         if self.mode == 'mat':
-            loss = torch.mean((op) ** 2) + \
+            loss = torch.mean(op ** 2) + \
                    lambda_bound * torch.mean((b_val - true_b_val) ** 2)
         else:
-            loss = torch.sum(torch.mean((op) ** 2, 0)) + \
+            loss = torch.sum(torch.mean(op ** 2, 0)) + \
                    lambda_bound * torch.sum(torch.mean((b_val - true_b_val) ** 2, 0))
+
+        if not save_graph:
+            temp_loss = loss.detach()
+            del loss
+            torch.cuda.empty_cache()
+            loss = temp_loss
+
         return loss
 
     def casual_loss(self, lambda_bound:  Union[int, float] = 10, tol: float = 0) -> torch.Tensor:
         """
         Computes casual loss, which is caclulated with weights matrix:
         W = exp(-tol*(Loss_i)) where Loss_i is sum of the L2 loss from 0
         to t_i moment of time. This loss function should be used when one
@@ -380,28 +388,29 @@
         b_val, true_b_val = self.bconds.apply_bconds_operator()
 
         loss = torch.sum(op) + \
                lambda_bound * torch.sum(torch.mean((b_val - true_b_val) ** 2, 0))
 
         return loss
 
-    def loss_evaluation(self, lambda_bound: Union[int, float] = 10, weak_form: Union[None, list] = None, tol=0) -> Union[default_loss, weak_loss, casual_loss]:
+    def loss_evaluation(self, lambda_bound: Union[int, float] = 10, weak_form: Union[None, list] = None, save_graph: bool = True, tol=0) -> Union[default_loss, weak_loss, casual_loss]:
         """
         Setting the required loss calculation method.
         Args:
             lambda_bound: an arbitrary chosen constant, influence only convergence speed.
             weak_form: list of basis functions.
+            save_graph: boolean constant, responsible for saving the computational graph.
             tol: float constant, influences on error penalty. 
         Returns:
             A given calculation method.
         """
         if self.mode == 'mat' or self.mode == 'autograd':
             if self.prepared_bconds == None:
                 print('No bconds is not possible, returning infinite loss')
                 return np.inf
 
         if weak_form != None and weak_form != []:
             return self.weak_loss(weak_form, lambda_bound=lambda_bound)
         elif tol != 0:
             return self.casual_loss(lambda_bound=lambda_bound, tol=tol)
         else:
-            return self.default_loss(lambda_bound=lambda_bound)
+            return self.default_loss(lambda_bound=lambda_bound, save_graph=save_graph)
```

### Comparing `tedeous-0.2.0/tedeous/models.py` & `tedeous-0.2.1/tedeous/models.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous/points_type.py` & `tedeous-0.2.1/tedeous/points_type.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous/solver.py` & `tedeous-0.2.1/tedeous/solver.py`

 * *Files identical despite different names*

### Comparing `tedeous-0.2.0/tedeous.egg-info/PKG-INFO` & `tedeous-0.2.1/tedeous.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tedeous
-Version: 0.2.0
+Version: 0.2.1
 Summary: TEDEouS - Torch Exhaustive Differential Equations Solver. Differential equation solver, based on pytorch library
 Author: Alexander Hvatov
 Author-email: itmo.nss.team@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

