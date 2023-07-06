# Comparing `tmp/bayesianbandits-0.4.3.tar.gz` & `tmp/bayesianbandits-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.4.3.tar", max compression
+gzip compressed data, was "bayesianbandits-0.4.4.tar", max compression
```

## Comparing `bayesianbandits-0.4.3.tar` & `bayesianbandits-0.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/LICENSE
--rw-r--r--   0        0        0     1093 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/README.md
--rw-r--r--   0        0        0     2919 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3538 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    22393 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    29847 2023-06-21 20:28:19.162026 bayesianbandits-0.4.3/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-06-21 20:28:19.166026 bayesianbandits-0.4.3/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5036 2023-06-21 20:28:19.166026 bayesianbandits-0.4.3/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2634 2023-06-21 20:28:19.166026 bayesianbandits-0.4.3/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      705 2023-06-21 20:28:19.170026 bayesianbandits-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1093 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/README.md
+-rw-r--r--   0        0        0     2991 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     3774 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    23085 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    29847 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5036 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2634 2023-07-06 00:14:50.505508 bayesianbandits-0.4.4/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      765 2023-07-06 00:14:50.509508 bayesianbandits-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 bayesianbandits-0.4.4/PKG-INFO
```

### Comparing `bayesianbandits-0.4.3/LICENSE` & `bayesianbandits-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.3/README.md` & `bayesianbandits-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.3/bayesianbandits/__init__.py` & `bayesianbandits-0.4.4/bayesianbandits/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,20 +84,27 @@
 
 These are custom exceptions raised by the bandit classes.
 
 .. autosummary::
     :toctree: _autosummary
 
     DelayedRewardException
+    DelayedRewardWarning
 
 """
 
 
 from ._arm import Arm
-from ._basebandit import Bandit, DelayedRewardException, contextual, restless
+from ._basebandit import (
+    Bandit,
+    DelayedRewardException,
+    DelayedRewardWarning,
+    contextual,
+    restless,
+)
 from ._estimators import (
     DirichletClassifier,
     GammaRegressor,
     NormalInverseGammaRegressor,
     NormalRegressor,
 )
 from ._policy_decorators import (
```

### Comparing `bayesianbandits-0.4.3/bayesianbandits/_arm.py` & `bayesianbandits-0.4.4/bayesianbandits/_arm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from __future__ import annotations
 from functools import wraps
-from typing import Callable, Optional, TypeVar, cast, Any
+from typing import Callable, Optional, TypeVar, Union, cast, Any
 from typing_extensions import ParamSpec, Concatenate
 import numpy as np
-from numpy.typing import ArrayLike, NDArray
+from numpy.typing import NDArray
 
 from ._typing import DecayingLearner, Learner, ActionToken
 
 P = ParamSpec("P")
 R = TypeVar("R", covariant=True)
+RewardFunction = Union[
+    Callable[..., np.float_],
+    Callable[..., NDArray[np.float_]],
+    Callable[..., Union[np.float_, NDArray[np.float_]]],
+]
 
 
 def requires_learner(
     func: Callable[Concatenate[Arm, P], R]
 ) -> Callable[Concatenate[Arm, P], R]:
     """Decorator to check if the arm has a learner set."""
 
@@ -29,17 +34,19 @@
     """Arm of a bandit.
 
     Parameters
     ----------
     action_token : Any
         Token to return when the arm is pulled. This should be something processed
         by the user's code to execute the action associated with the arm.
-    reward_function : Callable
+    reward_function : RewardFunction
         Function to call to compute the reward. Takes the output of the learner's
-        `sample` function as input and should return a scalar reward.
+        `sample` function as input and should return a scalar reward. Should take
+        a single scalar or array-like argument and return a scalar or
+        1D array.
     learner : Optional[Learner], default=None
         Learner to use for the arm. If None, the arm cannot be used.
 
     Examples
     --------
     >>> from bayesianbandits import Arm
     >>> import numpy as np
@@ -58,15 +65,15 @@
     >>> arm.update(np.array([[1]]), np.array([1]))
 
     """
 
     def __init__(
         self,
         action_token: Any,
-        reward_function: Callable[[ArrayLike], ArrayLike],
+        reward_function: RewardFunction,
         learner: Optional[Learner] = None,
     ) -> None:
         self.action_token = ActionToken(action_token)
         self.reward_function = reward_function
         self.learner = learner
 
     @requires_learner
```

### Comparing `bayesianbandits-0.4.3/bayesianbandits/_basebandit.py` & `bayesianbandits-0.4.4/bayesianbandits/_basebandit.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,20 +318,31 @@
             # check if `unique_id` is a non-string iterable
             elif isinstance(unique_id, Collection) and not isinstance(unique_id, str):
                 return self._update_batch(
                     X_fit, y_fit, cast(Collection[Any], unique_id)
                 )
 
             try:
-                arm_to_update = self.arms[self.cache.pop(unique_id)]  # type: ignore
+                assert self.cache is not None  # this is here for the type checker
+                arm = self.cache.pop(unique_id)
             except KeyError:
                 raise DelayedRewardException(
                     f"The unique_id {unique_id} is not in the cache. "
                     "Please use a valid unique identifier."
                 )
+            try:
+                arm_to_update = self.arms[arm]
+            except KeyError:
+                warn(
+                    DelayedRewardWarning(
+                        f"The arm {arm} is not in the bandit. Skipping."
+                    ),
+                    stacklevel=2,
+                )
+                return
 
         else:
             arm_to_update = cast(ArmProtocol, self.last_arm_pulled)
 
         arm_to_update.update(X_fit, y_fit)
 
     def _update_batch(
@@ -370,15 +381,25 @@
         for X_part, y_part, arms in groupby_array(
             X[present_ids],
             y[present_ids],
             arm_names[present_ids],
             by=arm_names[present_ids],
         ):
             arm_name = arms[0]
-            self.arms[arm_name].update(X_part, y_part)
+            try:
+                arm_to_update = self.arms[arm_name]
+            except KeyError:
+                warn(
+                    DelayedRewardWarning(
+                        f"The arm {arm_name} is not in the bandit. Skipping."
+                    ),
+                    stacklevel=2,
+                )
+                continue
+            arm_to_update.update(X_part, y_part)
 
     @overload
     def sample(self, X: ArrayLike, /, *, size: int = 1) -> ArrayLike:
         ...
 
     @overload
     def sample(self, /, *, size: int = 1) -> ArrayLike:
@@ -683,15 +704,15 @@
         if self._contextual:  # type: ignore
             self.decay(X, decay_last_arm=False)
         else:
             self.decay(decay_last_arm=False)
 
     setattr(cls, "update", _restless_update)
 
-    return cast(Type[_B], cls)
+    return cls
 
 
 def check_is_bandit(cls: type):
     if not issubclass(cls, Bandit):
         raise ValueError("This decorator can only be used on a Bandit subclass.")
```

### Comparing `bayesianbandits-0.4.3/bayesianbandits/_estimators.py` & `bayesianbandits-0.4.4/bayesianbandits/_estimators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.3/bayesianbandits/_np_utils.py` & `bayesianbandits-0.4.4/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.3/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.4.4/bayesianbandits/_policy_decorators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.3/bayesianbandits/_typing.py` & `bayesianbandits-0.4.4/bayesianbandits/_typing.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.4.3/pyproject.toml` & `bayesianbandits-0.4.4/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.4.3"
-description = ""
+version = "0.4.4"
+description = "A Pythonic microframework for Multi-Armed Bandit algorithms."
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
 scikit-learn = "^1.2.1"
```

### Comparing `bayesianbandits-0.4.3/PKG-INFO` & `bayesianbandits-0.4.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.4.3
-Summary: 
+Version: 0.4.4
+Summary: A Pythonic microframework for Multi-Armed Bandit algorithms.
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

