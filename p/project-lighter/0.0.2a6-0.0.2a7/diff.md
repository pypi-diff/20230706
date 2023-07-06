# Comparing `tmp/project_lighter-0.0.2a6.tar.gz` & `tmp/project_lighter-0.0.2a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_lighter-0.0.2a6.tar", max compression
+gzip compressed data, was "project_lighter-0.0.2a7.tar", max compression
```

## Comparing `project_lighter-0.0.2a6.tar` & `project_lighter-0.0.2a7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1080 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/LICENSE
--rw-r--r--   0        0        0     2164 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/README.md
--rw-r--r--   0        0        0       67 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/__init__.py
--rw-r--r--   0        0        0      125 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/__init__.py
--rw-r--r--   0        0        0    14204 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/logger.py
--rw-r--r--   0        0        0     6508 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/utils.py
--rw-r--r--   0        0        0        0 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/writer/__init__.py
--rw-r--r--   0        0        0     7593 2023-06-23 16:45:53.177088 project_lighter-0.0.2a6/lighter/callbacks/writer/base.py
--rw-r--r--   0        0        0     2662 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/callbacks/writer/file.py
--rw-r--r--   0        0        0     2427 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/callbacks/writer/table.py
--rw-r--r--   0        0        0    19796 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/system.py
--rw-r--r--   0        0        0       36 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/__init__.py
--rw-r--r--   0        0        0      627 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/cli.py
--rw-r--r--   0        0        0     2566 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/collate.py
--rw-r--r--   0        0        0     1547 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/dynamic_imports.py
--rw-r--r--   0        0        0     3866 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/freezer.py
--rw-r--r--   0        0        0     2278 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/misc.py
--rw-r--r--   0        0        0     5881 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/model.py
--rw-r--r--   0        0        0     2483 2023-06-23 16:45:53.181088 project_lighter-0.0.2a6/lighter/utils/runner.py
--rw-r--r--   0        0        0       24 2023-06-23 16:46:22.909276 project_lighter-0.0.2a6/lighter/version.py
--rw-r--r--   0        0        0     4420 2023-06-23 16:46:22.837276 project_lighter-0.0.2a6/pyproject.toml
--rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 project_lighter-0.0.2a6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-06 19:04:42.686131 project_lighter-0.0.2a7/LICENSE
+-rw-r--r--   0        0        0     2164 2023-07-06 19:04:42.686131 project_lighter-0.0.2a7/README.md
+-rw-r--r--   0        0        0       67 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/__init__.py
+-rw-r--r--   0        0        0    17473 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/logger.py
+-rw-r--r--   0        0        0     6508 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/__init__.py
+-rw-r--r--   0        0        0     7593 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/base.py
+-rw-r--r--   0        0        0     2662 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/file.py
+-rw-r--r--   0        0        0     2427 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/callbacks/writer/table.py
+-rw-r--r--   0        0        0    19962 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/system.py
+-rw-r--r--   0        0        0       36 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/__init__.py
+-rw-r--r--   0        0        0      627 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/cli.py
+-rw-r--r--   0        0        0     2566 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/collate.py
+-rw-r--r--   0        0        0     1547 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/dynamic_imports.py
+-rw-r--r--   0        0        0     3866 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/freezer.py
+-rw-r--r--   0        0        0     2278 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/misc.py
+-rw-r--r--   0        0        0     6293 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/model.py
+-rw-r--r--   0        0        0     2483 2023-07-06 19:04:42.690131 project_lighter-0.0.2a7/lighter/utils/runner.py
+-rw-r--r--   0        0        0       24 2023-07-06 19:05:07.194157 project_lighter-0.0.2a7/lighter/version.py
+-rw-r--r--   0        0        0     4420 2023-07-06 19:05:07.142157 project_lighter-0.0.2a7/pyproject.toml
+-rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 project_lighter-0.0.2a7/PKG-INFO
```

### Comparing `project_lighter-0.0.2a6/LICENSE` & `project_lighter-0.0.2a7/LICENSE`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/README.md` & `project_lighter-0.0.2a7/README.md`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/callbacks/logger.py` & `project_lighter-0.0.2a7/lighter/callbacks/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import Any, Dict, Union
 
+import itertools
 import sys
 from datetime import datetime
 from pathlib import Path
 
 import torch
-import yaml
 from loguru import logger
-from monai.bundle.config_parser import ConfigParser
 from monai.utils.module import optional_import
 from pytorch_lightning import Callback, Trainer
+from pytorch_lightning.callbacks.lr_monitor import LearningRateMonitor
 
 from lighter import LighterSystem
 from lighter.callbacks.utils import get_lighter_mode, is_data_type_supported, parse_data, preprocess_image
 from lighter.utils.dynamic_imports import OPTIONAL_IMPORTS
 
 
 class LighterLogger(Callback):
@@ -34,14 +34,15 @@
 
         self.log_types = {"input": input_type, "target": target_type, "pred": pred_type}
         # Max number of samples from the batch to log.
         self.max_samples = max_samples
 
         self.tensorboard = tensorboard
         self.wandb = wandb
+        self.lr_monitor = LighterLearningRateMonitor()
 
         # Running loss. Resets at each epoch. Loss is not calculated for `test` mode.
         self.loss = {"train": 0, "val": 0}
         # Epoch steps. Resets at each epoch. No `test` mode step counter as loss is not calculated for it.
         self.epoch_step_counter = {"train": 0, "val": 0}
         # Global steps. Replaces `Trainer.global_step` because it counts optimizer steps
         # instead of batch steps, which can be problematic when using gradient accumulation.
@@ -89,14 +90,18 @@
             if not wandb_available:
                 logger.error("Weights & Biases not installed. To install it, run `pip install wandb`. Exiting.")
                 sys.exit()
             wandb_dir = self.log_dir / "wandb"
             wandb_dir.mkdir()
             self.wandb = OPTIONAL_IMPORTS["wandb"].init(project=self.project, dir=wandb_dir, config=self.config)
 
+    def on_train_start(self, trainer: Trainer, pl_module: LighterSystem):
+        # Setup the learning rate monitor.
+        self.lr_monitor.on_train_start(trainer=trainer)
+
     def teardown(self, trainer: Trainer, pl_module: LighterSystem, stage: str) -> None:
         if not trainer.is_global_zero:
             return
         if self.tensorboard:
             self.tensorboard.close()
 
     def _log_by_type(self, name: str, data: Any, log_type: str, global_step: int) -> None:
@@ -217,14 +222,20 @@
                             f"`{name}` has to be a Tensor, List[Tensor], Tuple[Tensor],  Dict[str, Tensor], "
                             f"Dict[str, List[Tensor]], or Dict[str, Tuple[Tensor]]. `{type(outputs[name])}` is not supported."
                         )
                     for identifier, item in parse_data(outputs[name]).items():
                         item_name = f"{mode}/data/{name}" if identifier is None else f"{mode}/data/{name}_{identifier}"
                         self._log_by_type(item_name, item, self.log_types[name], global_step)
 
+                # Log learning rate stats. Logs at step if a scheduler's interval is step-based.
+                if mode == "train":
+                    lr_stats = self.lr_monitor.get_stats(trainer, "step")
+                    for name, value in lr_stats.items():
+                        self._log_scalar(f"{mode}/optimizer/{name}/step", value, global_step)
+
             # Increment the step counters.
             self.global_step_counter[mode] += 1
             if mode in ["train", "val"]:
                 self.epoch_step_counter[mode] += 1
 
     def _on_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
         """Performs logging at the end of an epoch. Logs the epoch number, the loss, and the metrics.
@@ -269,14 +280,20 @@
                     self._log_scalar(f"{mode}/loss/epoch", loss, global_step)
 
                 # Log metrics.
                 if metrics is not None:
                     for name, metric in metrics.items():
                         self._log_scalar(f"{mode}/metrics/{name}/epoch", metric, global_step)
 
+                # Log learning rate stats. Logs at epoch if a scheduler's interval is epoch-based, or if no scheduler is used.
+                if mode == "train":
+                    lr_stats = self.lr_monitor.get_stats(trainer, "epoch")
+                    for name, value in lr_stats.items():
+                        self._log_scalar(f"{mode}/optimizer/{name}/epoch", value, global_step)
+
     def _get_global_step(self, trainer: Trainer) -> int:
         """Return the global step for the current mode. Note that when Trainer
         is running Trainer.fit() and is in `val` mode, this method will return
         the global step of the `train` mode in order to correctly log the validation
         steps against training steps.
 
         Args:
@@ -319,7 +336,55 @@
         self._on_epoch_end(trainer, pl_module)
 
     def on_validation_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
         self._on_epoch_end(trainer, pl_module)
 
     def on_test_epoch_end(self, trainer: Trainer, pl_module: LighterSystem) -> None:
         self._on_epoch_end(trainer, pl_module)
+
+
+class LighterLearningRateMonitor(LearningRateMonitor):
+    def __init__(self) -> None:
+        # Instantiate LearningRateMonitor with default values.
+        super().__init__()
+
+    def on_train_start(self, trainer: Trainer) -> None:
+        # Set the `self.log_momentum` flag based on the optimizers instead of manually through __init__().
+        for key in ["momentum", "betas"]:
+            if trainer.lr_scheduler_configs:
+                self.log_momentum = any(key not in conf.scheduler.optimizer.defaults for conf in trainer.lr_scheduler_configs)
+            else:
+                self.log_momentum = any(key not in optimizer.defaults for optimizer in trainer.optimizers)
+            if self.log_momentum:
+                break
+
+        # Find names for schedulers
+        names = []
+        result = self._find_names_from_schedulers(trainer.lr_scheduler_configs)
+        sched_hparam_keys = result[0]
+        optimizers_with_scheduler = result[1]
+        optimizers_with_scheduler_types = result[2]
+        names.extend(sched_hparam_keys)
+
+        # Find names for leftover optimizers
+        optimizer_hparam_keys, _ = self._find_names_from_optimizers(
+            trainer.optimizers,
+            seen_optimizers=optimizers_with_scheduler,
+            seen_optimizer_types=optimizers_with_scheduler_types,
+        )
+        names.extend(optimizer_hparam_keys)
+
+        # Initialize for storing values
+        names_flatten = list(itertools.chain.from_iterable(names))
+        self.lrs = {name: [] for name in names_flatten}
+        self.last_momentum_values = {f"{name}-momentum": None for name in names_flatten}
+
+    def get_stats(self, trainer: Trainer, interval: str) -> Dict[str, float]:
+        # If a scheduler is not defined, log the learning rate over epochs.
+        if not trainer.lr_scheduler_configs and interval == "step":
+            return {}
+        lr_stats = self._extract_stats(trainer, interval)
+        # Remove 'lr-' prefix from keys and replace '-' with '/'.
+        lr_stats = {k[3:].replace("-", "/"): v for k, v in lr_stats.items()}
+        # Add '/lr' to the end of the keys that don't end with 'momentum'.
+        lr_stats = {k if k.endswith("momentum") else f"{k}/lr": v for k, v in lr_stats.items()}
+        return lr_stats
```

### Comparing `project_lighter-0.0.2a6/lighter/callbacks/utils.py` & `project_lighter-0.0.2a7/lighter/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/callbacks/writer/base.py` & `project_lighter-0.0.2a7/lighter/callbacks/writer/base.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/callbacks/writer/file.py` & `project_lighter-0.0.2a7/lighter/callbacks/writer/file.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/callbacks/writer/table.py` & `project_lighter-0.0.2a7/lighter/callbacks/writer/table.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/system.py` & `project_lighter-0.0.2a7/lighter/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,30 +226,32 @@
 
         pred = reshape_pred_if_single_value_prediction(pred, target)
 
         # Calculate the loss.
         loss = None
         if mode in ["train", "val"]:
             loss = self._calculate_loss(pred, target)
+            loss_name = "loss" if mode == "train" else f"{mode}_loss"
+            # Log the loss and for monitoring purposes.
+            self.log(loss_name, loss, on_step=True, on_epoch=True, sync_dist=False, logger=False, batch_size=self.batch_size)
 
         # Apply the post-criterion activation. Necessary for measuring the metrics
         # correctly in cases when using a criterion such as `BCELossWithLogits`` which
         # requires the model to output logits, i.e. non-activated outputs.
         if self._post_criterion_activation is not None:
             pred = self._post_criterion_activation(pred)
 
         if mode == "predict":
             # In predict mode, skip the metrics and return the predicted value only.
             return pred
         else:
             # Calculate the metrics for the step.
             metrics = getattr(self, f"{mode}_metrics")(pred, target)
-            # Log the loss and metrics for monitoring purposes only.
-            self.log("loss" if mode == "train" else f"{mode}_loss", loss, on_step=True, on_epoch=True, logger=False)
-            self.log_dict(metrics, on_step=True, on_epoch=True, logger=False)
+            # Log the metrics for monitoring purposes.
+            self.log_dict(metrics, on_step=True, on_epoch=True, sync_dist=False, logger=False, batch_size=self.batch_size)
             # Return the loss, metrics, input, target, and pred.
             return {"loss": loss, "metrics": metrics, "input": input, "target": target, "pred": pred}
 
     def _calculate_loss(
         self, pred: Union[torch.Tensor, List, Tuple, Dict], target: Union[torch.Tensor, List, Tuple, Dict, None]
     ) -> torch.Tensor:
         """_summary_
```

### Comparing `project_lighter-0.0.2a6/lighter/utils/cli.py` & `project_lighter-0.0.2a7/lighter/utils/cli.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/utils/collate.py` & `project_lighter-0.0.2a7/lighter/utils/collate.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/utils/dynamic_imports.py` & `project_lighter-0.0.2a7/lighter/utils/dynamic_imports.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/utils/freezer.py` & `project_lighter-0.0.2a7/lighter/utils/freezer.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/utils/misc.py` & `project_lighter-0.0.2a7/lighter/utils/misc.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/lighter/utils/model.py` & `project_lighter-0.0.2a7/lighter/utils/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict
+from typing import Dict, List
 
 import torch
 from loguru import logger
 from torch.nn import Identity, Module, Sequential
 
 from lighter.utils.misc import setattr_dot_notation
 
@@ -66,28 +66,31 @@
 
     Returns:
         Sequential: PyTorch Sequential model with the last layer removed.
     """
     return Sequential(*list(model.children())[:-num_layers])
 
 
-def adjust_prefix_and_load_state_dict(model: Module, ckpt_path: str, ckpt_to_model_prefix: Dict[str, str] = None) -> Module:
+def adjust_prefix_and_load_state_dict(
+    model: Module, ckpt_path: str, ckpt_to_model_prefix: Dict[str, str] = None, layers_to_ignore: List[str] = None
+) -> Module:
     """Load state_dict from a checkpoint into a model using `torch.load(strict=False`).
     `ckpt_to_model_prefix` mapping allows to rename the prefix of the checkpoint's state_dict keys
     so that they match those of the model's state_dict. This is often needed when a model was trained
     as a backbone of another model, so its state_dict keys won't be the same to those of a standalone
     version of that model. Prior to defining the `ckpt_to_model_prefix`, it is advised to manually check
     for mismatch between the names and specify them accordingly.
 
     Args:
         model (Module): The PyTorch model instance to load the state_dict into.
         ckpt_path (str): Path to the checkpoint.
         ckpt_to_model_prefix (Dict[str, str], optional): A dictionary that maps keys in the checkpoint's
             state_dict to keys in the model's state_dict. If None, no key mapping is performed. Defaults to None.
-
+        layers_to_ignore (List[str], optional): A list of layer names that won't be loaded into the model.
+            Specify the names as they are after `ckpt_to_model_prefix` is applied. Defaults to None.
     Returns:
         Module: The model instance with the state_dict loaded.
 
     Raises:
         ValueError: If there is no overlap between checkpoint's and model's state_dict.
     """
 
@@ -107,21 +110,27 @@
             model_prefix = model_prefix if model_prefix == "" or model_prefix.endswith(".") else f"{model_prefix}."
             if ckpt_prefix != "":
                 # Replace ckpt_prefix with model_prefix in the checkpoint state_dict
                 ckpt = {key.replace(ckpt_prefix, model_prefix): value for key, value in ckpt.items() if ckpt_prefix in key}
             else:
                 # Add the model_prefix before the current key name if there's no specific ckpt_prefix
                 ckpt = {f"{model_prefix}{key}": value for key, value in ckpt.items() if ckpt_prefix in key}
+
     # Check if there is no overlap between the checkpoint's and model's state_dict.
     if not set(ckpt.keys()) & set(model.state_dict().keys()):
         raise ValueError(
             "There is no overlap between checkpoint's and model's state_dict. Check their "
             "`state_dict` keys and adjust accordingly using `ckpt_prefix` and `model_prefix`."
         )
 
+    # Remove the layers that are not to be loaded.
+    if layers_to_ignore is not None:
+        for layer in layers_to_ignore:
+            ckpt.pop(layer)
+
     # Load the adjusted state_dict into the model instance.
     incompatible_keys = model.load_state_dict(ckpt, strict=False)
 
     # Log the incompatible keys during checkpoint loading.
     if len(incompatible_keys.missing_keys) > 0 or len(incompatible_keys.unexpected_keys) > 0:
         logger.info(f"Encountered incompatible keys during checkpoint loading. If intended, ignore.\n{incompatible_keys}")
```

### Comparing `project_lighter-0.0.2a6/lighter/utils/runner.py` & `project_lighter-0.0.2a7/lighter/utils/runner.py`

 * *Files identical despite different names*

### Comparing `project_lighter-0.0.2a6/pyproject.toml` & `project_lighter-0.0.2a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 lighter = "lighter.utils.cli:interface"
 
 [tool.poetry]
 name = "project-lighter"
-version = "0.0.2a6"
+version = "0.0.2a7"
 description = "YAML-based automated rapid prototyping framework for deep learning experiments"
 readme = "README.md"
 authors = ["Ibrahim Hadzic <ibrahimhadzic45@gmail.com>" ,
             "Suraj Pai <b.pai@maastrichtuniversity.nl>", 
             "Keno Bressem <kbressem@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/lighter/lighter"
```

### Comparing `project_lighter-0.0.2a6/PKG-INFO` & `project_lighter-0.0.2a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: project-lighter
-Version: 0.0.2a6
+Version: 0.0.2a7
 Summary: YAML-based automated rapid prototyping framework for deep learning experiments
 Home-page: https://github.com/lighter/lighter
 License: MIT
 Author: Ibrahim Hadzic
 Author-email: ibrahimhadzic45@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

