# Comparing `tmp/numalogic-0.4a1.tar.gz` & `tmp/numalogic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.4a1.tar", max compression
+gzip compressed data, was "numalogic-0.5.0.tar", max compression
```

## Comparing `numalogic-0.4a1.tar` & `numalogic-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,53 @@
--rw-r--r--   0        0        0    11357 2023-06-02 21:10:54.495132 numalogic-0.4a1/LICENSE
--rw-r--r--   0        0        0     5244 2023-06-02 21:10:54.495132 numalogic-0.4a1/README.md
--rw-r--r--   0        0        0      706 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/__init__.py
--rw-r--r--   0        0        0      729 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/_constants.py
--rw-r--r--   0        0        0     1681 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/base.py
--rw-r--r--   0        0        0     1048 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/config/__init__.py
--rw-r--r--   0        0        0     2473 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/config/_config.py
--rw-r--r--   0        0        0     4569 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/config/factory.py
--rw-r--r--   0        0        0        0 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/__init__.py
--rw-r--r--   0        0        0      683 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3772 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0     3108 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/trainer.py
--rw-r--r--   0        0        0      581 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11541 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8702 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      211 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     4043 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2463 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       78 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/numaflow/__init__.py
--rw-r--r--   0        0        0     1925 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/numaflow/_base.py
--rw-r--r--   0        0        0     1118 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      328 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     5312 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/registry/artifact.py
--rw-r--r--   0        0        0     1672 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13598 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    10708 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    11661 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4701 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/tools/__init__.py
--rw-r--r--   0        0        0     1870 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0     8172 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/tools/data.py
--rw-r--r--   0        0        0     1610 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     1525 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/tools/types.py
--rw-r--r--   0        0        0     1153 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     5090 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     1861 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     2600 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     1771 2023-06-02 21:10:54.563132 numalogic-0.4a1/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     2619 2023-06-02 21:10:54.567132 numalogic-0.4a1/pyproject.toml
--rw-r--r--   0        0        0     6548 1970-01-01 00:00:00.000000 numalogic-0.4a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-06 18:42:43.473405 numalogic-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5244 2023-07-06 18:42:43.473405 numalogic-0.5.0/README.md
+-rw-r--r--   0        0        0      676 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/_constants.py
+-rw-r--r--   0        0        0     1636 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3231 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1048 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     2473 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/config/_config.py
+-rw-r--r--   0        0        0     4680 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/config/factory.py
+-rw-r--r--   0        0        0        0 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      683 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3772 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0     3146 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/trainer.py
+-rw-r--r--   0        0        0      581 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11561 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8702 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      211 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     4043 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2463 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       78 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/numaflow/__init__.py
+-rw-r--r--   0        0        0     1925 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/numaflow/_base.py
+-rw-r--r--   0        0        0     1282 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      328 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     5777 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15562 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     2828 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13638 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    12507 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    11784 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0     1870 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0     8422 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/data.py
+-rw-r--r--   0        0        0     1740 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     1973 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1153 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     5090 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     1861 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     2600 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     1771 2023-07-06 18:42:43.533406 numalogic-0.5.0/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     2771 2023-07-06 18:42:43.537406 numalogic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6686 1970-01-01 00:00:00.000000 numalogic-0.5.0/PKG-INFO
```

### Comparing `numalogic-0.4a1/LICENSE` & `numalogic-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/README.md` & `numalogic-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/__init__.py` & `numalogic-0.5.0/numalogic/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,9 +10,8 @@
 # limitations under the License.
 
 
 import logging
 
 
 LOGGER = logging.getLogger(__name__)
-LOGGER.setLevel(logging.INFO)
 LOGGER.addHandler(logging.NullHandler())
```

### Comparing `numalogic-0.4a1/numalogic/_constants.py` & `numalogic-0.5.0/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/base.py` & `numalogic-0.5.0/numalogic/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 """Base classes for all models and transforms."""
 
 
 from abc import ABCMeta
 
 import numpy.typing as npt
 import pytorch_lightning as pl
-from sklearn.base import TransformerMixin, BaseEstimator, OutlierMixin
+from sklearn.base import TransformerMixin, OutlierMixin
 
 
-class BaseTransformer(TransformerMixin, BaseEstimator):
+class BaseTransformer(TransformerMixin):
     """Base class for all transformer classes."""
 
     pass
 
 
 class StatelessTransformer(BaseTransformer):
     """Base class for stateless transforms."""
@@ -43,11 +43,11 @@
 
 class TorchModel(pl.LightningModule, metaclass=ABCMeta):
     """Base class for all Pytorch based models."""
 
     pass
 
 
-class BaseThresholdModel(OutlierMixin, BaseEstimator):
+class BaseThresholdModel(OutlierMixin):
     """Base class for all threshold models."""
 
     pass
```

### Comparing `numalogic-0.4a1/numalogic/config/__init__.py` & `numalogic-0.5.0/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/config/_config.py` & `numalogic-0.5.0/numalogic/config/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/config/factory.py` & `numalogic-0.5.0/numalogic/config/factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from typing import Union
+from typing import Union, ClassVar
 
 from numalogic.config._config import ModelInfo, RegistryInfo
 from numalogic.tools.exceptions import UnknownConfigArgsError
 
 
 class _ObjectFactory:
-    _CLS_MAP = {}
+    _CLS_MAP: ClassVar[dict] = {}
 
     def get_instance(self, object_info: Union[ModelInfo, RegistryInfo]):
         try:
             _cls = self._CLS_MAP[object_info.name]
         except KeyError as err:
             raise UnknownConfigArgsError(
                 f"Invalid model info instance provided: {object_info}"
@@ -37,15 +37,15 @@
 
 class PreprocessFactory(_ObjectFactory):
     """Factory class to create preprocess instances."""
 
     from sklearn.preprocessing import StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler
     from numalogic.transforms import LogTransformer, StaticPowerTransformer, TanhScaler
 
-    _CLS_MAP = {
+    _CLS_MAP: ClassVar[dict] = {
         "StandardScaler": StandardScaler,
         "MinMaxScaler": MinMaxScaler,
         "MaxAbsScaler": MaxAbsScaler,
         "RobustScaler": RobustScaler,
         "LogTransformer": LogTransformer,
         "StaticPowerTransformer": StaticPowerTransformer,
         "TanhScaler": TanhScaler,
@@ -53,23 +53,23 @@
 
 
 class PostprocessFactory(_ObjectFactory):
     """Factory class to create postprocess instances."""
 
     from numalogic.transforms import TanhNorm, ExpMovingAverage
 
-    _CLS_MAP = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage}
+    _CLS_MAP: ClassVar[dict] = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage}
 
 
 class ThresholdFactory(_ObjectFactory):
     """Factory class to create threshold instances."""
 
     from numalogic.models.threshold import StdDevThreshold, StaticThreshold, SigmoidThreshold
 
-    _CLS_MAP = {
+    _CLS_MAP: ClassVar[dict] = {
         "StdDevThreshold": StdDevThreshold,
         "StaticThreshold": StaticThreshold,
         "SigmoidThreshold": SigmoidThreshold,
     }
 
 
 class ModelFactory(_ObjectFactory):
@@ -82,30 +82,30 @@
         SparseConv1dAE,
         LSTMAE,
         SparseLSTMAE,
         TransformerAE,
         SparseTransformerAE,
     )
 
-    _CLS_MAP = {
+    _CLS_MAP: ClassVar[dict] = {
         "VanillaAE": VanillaAE,
         "SparseVanillaAE": SparseVanillaAE,
         "Conv1dAE": Conv1dAE,
         "SparseConv1dAE": SparseConv1dAE,
         "LSTMAE": LSTMAE,
         "SparseLSTMAE": SparseLSTMAE,
         "TransformerAE": TransformerAE,
         "SparseTransformerAE": SparseTransformerAE,
     }
 
 
 class RegistryFactory(_ObjectFactory):
     """Factory class to create registry instances."""
 
-    _CLS_SET = {"RedisRegistry", "MLflowRegistry"}
+    _CLS_SET: ClassVar[frozenset] = {"RedisRegistry", "MLflowRegistry"}
 
     def get_instance(self, object_info: Union[ModelInfo, RegistryInfo]):
         import numalogic.registry as reg
 
         try:
             _cls = getattr(reg, object_info.name)
         except AttributeError as err:
```

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/__init__.py` & `numalogic-0.5.0/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/base.py` & `numalogic-0.5.0/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/trainer.py` & `numalogic-0.5.0/numalogic/models/autoencoder/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import pytorch_lightning as pl
 import torch
 from pytorch_lightning import Trainer
 from torch import Tensor
 
 from numalogic.tools.callbacks import ProgressDetails
 from numalogic.tools.data import inverse_window
+from typing import Optional
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AutoencoderTrainer(Trainer):
     r"""A PyTorch Lightning Trainer for Autoencoder models.
 
@@ -64,15 +65,15 @@
             enable_checkpointing=enable_checkpointing,
             enable_progress_bar=enable_progress_bar,
             enable_model_summary=enable_model_summary,
             callbacks=callbacks,
             **trainer_kw
         )
 
-    def predict(self, model: pl.LightningModule = None, unbatch=True, **kwargs) -> Tensor:
+    def predict(self, model: Optional[pl.LightningModule] = None, unbatch=True, **kwargs) -> Tensor:
         r"""Predicts the output of the model.
 
         Args:
         ----
             model: The model to predict with. (default: None)
             unbatch: Whether to inverse window the output. (default: True)
             **kwargs: Additional keyword arguments to pass to the Lightning
```

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.5.0/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.5.0/numalogic/models/autoencoder/variants/conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
-from typing import Union
+from typing import Union, Optional
 from collections.abc import Sequence
 
 import torch
 from torch import nn, Tensor
 from torch.distributions import kl_divergence, Bernoulli
 from torch.nn.init import calculate_gain
 
@@ -208,15 +208,15 @@
     def __init__(
         self,
         seq_len: int,
         in_channels: int,
         enc_channels: Sequence[int] = (16, 8),
         enc_kernel_sizes: Union[int, Sequence[int]] = 3,
         pool_kernel_size: int = 2,
-        dec_activation: str = None,
+        dec_activation: Optional[str] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.seq_len = seq_len
         self.in_channels = in_channels
 
         if isinstance(enc_kernel_sizes, int):
```

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.5.0/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.5.0/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.5.0/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/forecast/variants/naive.py` & `numalogic-0.5.0/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/threshold/_static.py` & `numalogic-0.5.0/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/models/threshold/_std.py` & `numalogic-0.5.0/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/numaflow/_base.py` & `numalogic-0.5.0/numalogic/numaflow/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/registry/__init__.py` & `numalogic-0.5.0/numalogic/registry/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,7 +26,14 @@
 
 try:
     from numalogic.registry.redis_registry import RedisRegistry  # noqa: F401
 except ImportError:
     pass
 else:
     __all__.append("RedisRegistry")
+
+try:
+    from numalogic.registry.dynamodb_registry import DynamoDBRegistry  # noqa: F401
+except ImportError:
+    pass
+else:
+    __all__.append("DynamoDBRegistry")
```

### Comparing `numalogic-0.4a1/numalogic/registry/artifact.py` & `numalogic-0.5.0/numalogic/registry/artifact.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,60 +7,79 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from dataclasses import dataclass
-from typing import Any, Generic, TypeVar
+from typing import Any, Generic, TypeVar, Union, Optional
 
-from numalogic.tools.types import artifact_t, KEYS, META_T, META_VT, EXTRA_T
+from numalogic.tools.types import artifact_t, KEYS, META_T, META_VT, EXTRA_T, state_dict_t
 
 
 @dataclass
 class ArtifactData:
-    """Dataclass to hold the artifact, its metadata and other extra info."""
+    """
+    Dataclass to hold the artifact, its metadata and other extra info.
+
+    Args:
+    ----
+        artifact: artifact to be saved; can be a model instance, a state_dict.
+        metadata: additional metadata surrounding the artifact that needs to be saved.
+        extras: any other extra information that needs to be saved.
+
+    """
 
     __slots__ = ("artifact", "metadata", "extras")
 
-    artifact: artifact_t
+    artifact: Union[artifact_t, state_dict_t]
     metadata: META_T
     extras: EXTRA_T
 
 
 A_D = TypeVar("A_D", bound=ArtifactData, covariant=True)
 M_K = TypeVar("M_K", bound=str)
 
 
 class ArtifactManager(Generic[KEYS, A_D]):
     """Abstract base class for artifact save, load and delete.
 
-    :param uri: server/connection uri
+    Args:
+    ----
+        uri: server/connection uri
     """
 
+    _STORETYPE = "registry"
+
     __slots__ = ("uri",)
 
     def __init__(self, uri: str):
         self.uri = uri
 
     def load(
-        self, skeys: KEYS, dkeys: KEYS, latest: bool = True, version: str = None
+        self, skeys: KEYS, dkeys: KEYS, latest: bool = True, version: Optional[str] = None
     ) -> ArtifactData:
         """Loads the desired artifact from mlflow registry and returns it.
 
         Args:
         ----
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             latest: boolean field to determine if latest version is desired or not
             version: explicit artifact version.
         """
         raise NotImplementedError("Please implement this method!")
 
-    def save(self, skeys: KEYS, dkeys: KEYS, artifact: artifact_t, **metadata: META_VT) -> Any:
+    def save(
+        self,
+        skeys: KEYS,
+        dkeys: KEYS,
+        artifact: Union[artifact_t, state_dict_t],
+        **metadata: META_VT
+    ) -> Any:
         r"""Saves the artifact into mlflow registry and updates version.
 
         Args:
         ----
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             artifact: primary artifact to be saved
@@ -116,14 +135,16 @@
 
     Args:
     ----
         cachesize: size of the cache
         ttl: time to live for each item in the cache
     """
 
+    _STORETYPE = "cache"
+
     __slots__ = ("_cachesize", "_ttl")
 
     def __init__(self, cachesize: int, ttl: int):
         self._cachesize = cachesize
         self._ttl = ttl
 
     @property
```

### Comparing `numalogic-0.4a1/numalogic/registry/mlflow_registry.py` & `numalogic-0.5.0/numalogic/registry/mlflow_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,29 +73,29 @@
     _TRACKING_URI = None
 
     def __new__(
         cls,
         tracking_uri: Optional[str],
         models_to_retain: int = 5,
         model_stage: ModelStage = ModelStage.PRODUCTION,
-        cache_registry: ArtifactCache = None,
+        cache_registry: Optional[ArtifactCache] = None,
         *args,
         **kwargs,
     ):
         instance = super().__new__(cls, *args, **kwargs)
         if (not cls._TRACKING_URI) or (cls._TRACKING_URI != tracking_uri):
             cls._TRACKING_URI = tracking_uri
         return instance
 
     def __init__(
         self,
         tracking_uri: str,
         models_to_retain: int = 5,
         model_stage: str = ModelStage.PRODUCTION,
-        cache_registry: ArtifactCache = None,
+        cache_registry: Optional[ArtifactCache] = None,
     ):
         super().__init__(tracking_uri)
         mlflow.set_tracking_uri(tracking_uri)
         self.client = MlflowClient()
         self.models_to_retain = models_to_retain
         self.model_stage = model_stage
         self.cache_registry = cache_registry
@@ -134,15 +134,15 @@
         return None
 
     def load(
         self,
         skeys: KEYS,
         dkeys: KEYS,
         latest: bool = True,
-        version: str = None,
+        version: Optional[str] = None,
         artifact_type: str = "pytorch",
     ) -> Optional[ArtifactData]:
         """Load the artifact from the registry. The artifact is loaded from the cache if available.
 
         Args:
         ----
             skeys: Static keys
@@ -202,15 +202,15 @@
             )
 
     def save(
         self,
         skeys: KEYS,
         dkeys: KEYS,
         artifact: artifact_t,
-        run_id: str = None,
+        run_id: Optional[str] = None,
         **metadata: META_VT,
     ) -> Optional[ModelVersion]:
         """Saves the artifact into mlflow registry and updates version.
 
         Args:
         ----
             skeys: static key fields as list/tuple of strings
```

### Comparing `numalogic-0.4a1/numalogic/registry/redis_registry.py` & `numalogic-0.5.0/numalogic/registry/redis_registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,39 @@
+# Copyright 2022 The Numaproj Authors.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#     http://www.apache.org/licenses/LICENSE-2.0
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import logging
 import time
 from datetime import datetime, timedelta
 from typing import Optional
 
 from redis.exceptions import RedisError
 
 from numalogic.registry.artifact import ArtifactManager, ArtifactData, ArtifactCache
 from numalogic.registry._serialize import loads, dumps
 from numalogic.tools.exceptions import ModelKeyNotFound, RedisRegistryError
 from numalogic.tools.types import artifact_t, redis_client_t, KEYS, META_T, META_VT
 
-_LOGGER = logging.getLogger()
+_LOGGER = logging.getLogger(__name__)
 
 
 class RedisRegistry(ArtifactManager):
     """Model saving and loading using Redis Registry.
 
     Args:
     ----
-        client: Take in the reids client already established/created
+        client: Take in the redis client already established/created
         ttl: Total Time to Live (in seconds) for the key when saving in redis (dafault = 604800)
         cache_registry: Cache registry to use (default = None).
 
     Examples
     --------
     >>> import redis
     >>> from numalogic.models.autoencoder.variants import VanillaAE
@@ -38,15 +49,15 @@
 
     __slots__ = ("client", "ttl", "cache_registry")
 
     def __init__(
         self,
         client: redis_client_t,
         ttl: int = 604800,
-        cache_registry: ArtifactCache = None,
+        cache_registry: Optional[ArtifactCache] = None,
     ):
         super().__init__("")
         self.client = client
         self.ttl = ttl
         self.cache_registry = cache_registry
 
     @staticmethod
@@ -64,16 +75,16 @@
             key
         """
         _static_key = ":".join(skeys)
         _dynamic_key = ":".join(dkeys)
         return "::".join([_static_key, _dynamic_key])
 
     @staticmethod
-    def __construct_production_key(key: str):
-        return RedisRegistry.construct_key(skeys=[key], dkeys=["PROD"])
+    def __construct_latest_key(key: str):
+        return RedisRegistry.construct_key(skeys=[key], dkeys=["LATEST"])
 
     @staticmethod
     def __construct_version_key(key: str, version: str):
         return RedisRegistry.construct_key(skeys=[key], dkeys=[version])
 
     @staticmethod
     def get_version(key: str) -> str:
@@ -90,14 +101,15 @@
     def _load_from_cache(self, key: str) -> Optional[ArtifactData]:
         if not self.cache_registry:
             return None
         return self.cache_registry.load(key)
 
     def _save_in_cache(self, key: str, artifact_data: ArtifactData) -> None:
         if self.cache_registry:
+            _LOGGER.debug("Saving artifact in cache with key: %s", key)
             self.cache_registry.save(key, artifact_data)
 
     def _clear_cache(self, key: Optional[str] = None) -> Optional[ArtifactData]:
         if self.cache_registry:
             if key:
                 return self.cache_registry.delete(key)
             return self.cache_registry.clear()
@@ -119,48 +131,62 @@
             deserialized_metadata = loads(serialized_metadata)
         return ArtifactData(
             artifact=deserialized_artifact,
             metadata=deserialized_metadata,
             extras={
                 "timestamp": float(artifact_timestamp.decode()),
                 "version": artifact_version.decode(),
+                "source": self._STORETYPE,
             },
         )
 
-    def __load_latest_artifact(self, key: str) -> ArtifactData:
+    def __load_latest_artifact(self, key: str) -> tuple[ArtifactData, bool]:
+        """
+        Load the latest artifact from the registry.
+
+        Args:
+            key: full model key.
+
+        Returns
+        -------
+            ArtifactData and a boolean flag indicating if the artifact was loaded from cache.
+
+        Raises
+        ------
+            ModelKeyNotFound: If the model key is not found in the registry.
+        """
         cached_artifact = self._load_from_cache(key)
         if cached_artifact:
             _LOGGER.debug("Found cached artifact for key: %s", key)
-            return cached_artifact
-        production_key = self.__construct_production_key(key)
-        if not self.client.exists(production_key):
-            raise ModelKeyNotFound(
-                f"Production key: {production_key}, Not Found !!!\n Exiting....."
-            )
-        model_key = self.client.get(production_key)
-        _LOGGER.info("Production key, %s, is pointing to the key : %s", production_key, model_key)
-        return self.__load_version_artifact(version=self.get_version(model_key.decode()), key=key)
+            return cached_artifact, True
+        latest_key = self.__construct_latest_key(key)
+        if not self.client.exists(latest_key):
+            raise ModelKeyNotFound(f"latest key: {latest_key}, Not Found !!!")
+        model_key = self.client.get(latest_key)
+        _LOGGER.debug("latest key, %s, is pointing to the key : %s", latest_key, model_key)
+        return (
+            self.__load_version_artifact(version=self.get_version(model_key.decode()), key=key),
+            False,
+        )
 
     def __load_version_artifact(self, version: str, key: str) -> ArtifactData:
         model_key = self.__construct_version_key(key, version)
         if not self.client.exists(model_key):
             raise ModelKeyNotFound("Could not find model key with key: %s" % model_key)
         return self.__get_artifact_data(
             model_key=model_key,
         )
 
     def __save_artifact(
         self, pipe, artifact: artifact_t, metadata: META_T, key: KEYS, version: str
     ) -> str:
         new_version_key = self.__construct_version_key(key, version)
-        production_key = self.__construct_production_key(key)
-        pipe.set(name=production_key, value=new_version_key)
-        _LOGGER.info(
-            "Setting Production key : %s ,to this new key = %s", production_key, new_version_key
-        )
+        latest_key = self.__construct_latest_key(key)
+        pipe.set(name=latest_key, value=new_version_key)
+        _LOGGER.debug("Setting latest key : %s ,to this new key = %s", latest_key, new_version_key)
         serialized_metadata = ""
         if metadata:
             serialized_metadata = dumps(deserialized_object=metadata)
         serialized_artifact = dumps(deserialized_object=artifact)
         pipe.hset(
             name=new_version_key,
             mapping={
@@ -173,42 +199,51 @@
         return new_version_key
 
     def load(
         self,
         skeys: KEYS,
         dkeys: KEYS,
         latest: bool = True,
-        version: str = None,
+        version: Optional[str] = None,
     ) -> Optional[ArtifactData]:
         """Loads the artifact from redis registry. Either latest or version (one of the arguments)
          is needed to load the respective artifact.
 
+         If cache registry is provided, it will first check the cache registry for the artifact.
+
         Args:
         ----
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
-            latest: load the model in production stage
+            latest: load the model in latest stage
             version: version to load.
 
         Returns
         -------
             ArtifactData instance
+
+        Raises
+        ------
+            ValueError: If both latest and version are provided or none of them are provided.
+            RedisRegistryError: If any redis error occurs.
         """
         if (latest and version) or (not latest and not version):
             raise ValueError("Either One of 'latest' or 'version' needed in load method call")
         key = self.construct_key(skeys, dkeys)
+        is_cached = False
         try:
             if latest:
-                artifact_data = self.__load_latest_artifact(key)
-                self._save_in_cache(key, artifact_data)
+                artifact_data, is_cached = self.__load_latest_artifact(key)
             else:
                 artifact_data = self.__load_version_artifact(version, key)
         except RedisError as err:
             raise RedisRegistryError(f"{err.__class__.__name__} raised") from err
         else:
+            if (not is_cached) and latest:
+                self._save_in_cache(key, artifact_data)
             return artifact_data
 
     def save(
         self,
         skeys: KEYS,
         dkeys: KEYS,
         artifact: artifact_t,
@@ -221,69 +256,84 @@
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             artifact: primary artifact to be saved
             metadata: additional metadata surrounding the artifact that needs to be saved.
 
         Returns
         -------
-            model version
+            Model version (str)
+
+        Raises
+        ------
+            RedisRegistryError: If there is any RedisError while saving the artifact.
         """
         key = self.construct_key(skeys, dkeys)
-        production_key = self.__construct_production_key(key)
+        latest_key = self.__construct_latest_key(key)
         version = 0
         try:
-            if self.client.exists(production_key):
-                _LOGGER.debug("Production key exists for the model")
-                version_key = self.client.get(name=production_key)
+            if self.client.exists(latest_key):
+                _LOGGER.debug("Latest key: %s exists for the model", latest_key)
+                version_key = self.client.get(name=latest_key)
                 version = int(self.get_version(version_key.decode())) + 1
             with self.client.pipeline() as pipe:
                 new_version_key = self.__save_artifact(pipe, artifact, metadata, key, str(version))
                 pipe.expire(name=new_version_key, time=self.ttl)
-                _LOGGER.info("Model is successfully with the key = %s", new_version_key)
                 pipe.execute()
         except RedisError as err:
             raise RedisRegistryError(f"{err.__class__.__name__} raised") from err
         else:
+            _LOGGER.info("Model with the key = %s, saved successfully.", new_version_key)
             return str(version)
 
     def delete(self, skeys: KEYS, dkeys: KEYS, version: str) -> None:
         """Deletes the model version from registry.
 
         Args:
         ----
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             version: model version to delete.
+
+        Raises
+        ------
+            ModelKeyNotFound: If the model version is not found in registry.
+            RedisRegistryError: If there is any RedisError while deleting the artifact.
         """
         key = self.construct_key(skeys, dkeys)
         del_key = self.__construct_version_key(key, version)
         try:
             if self.client.exists(del_key):
                 self.client.delete(del_key)
-                _LOGGER.info("Model with the key = %s, deleted successfully", del_key)
             else:
-                _LOGGER.debug("Key to delete: %s, Not Found !!!\n Exiting.....", del_key)
                 raise ModelKeyNotFound(
-                    "Key to delete: %s, Not Found !!!\n Exiting....." % del_key,
+                    "Key to delete: %s, Not Found!" % del_key,
                 )
         except RedisError as err:
             raise RedisRegistryError(f"{err.__class__.__name__} raised") from err
         else:
+            _LOGGER.info("Model with the key = %s, deleted successfully", del_key)
             self._clear_cache(del_key)
 
     @staticmethod
     def is_artifact_stale(artifact_data: ArtifactData, freq_hr: int) -> bool:
         """Returns whether the given artifact is stale or not, i.e. if
         more time has elapsed since it was last retrained.
 
         Args:
         ----
             artifact_data: ArtifactData object to look into
             freq_hr: Frequency of retraining in hours.
 
+        Returns
+        -------
+            True if artifact is stale, False otherwise.
+
+        Raises
+        ------
+            RedisRegistryError: If there is any error while fetching timestamp information.
         """
         try:
             artifact_ts = float(artifact_data.extras["timestamp"])
         except (KeyError, TypeError) as err:
             raise RedisRegistryError("Error fetching timestamp information") from err
         stale_ts = (datetime.now() - timedelta(hours=freq_hr)).timestamp()
         return stale_ts > artifact_ts
```

### Comparing `numalogic-0.4a1/numalogic/synthetic/__init__.py` & `numalogic-0.5.0/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/synthetic/anomalies.py` & `numalogic-0.5.0/numalogic/synthetic/anomalies.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import StandardScaler
+from typing import Optional, ClassVar
 
 
 class AnomalyGenerator:
     """
     Class to inject synthetic anomaly to the input time series based on parameters.
 
     Args:
@@ -37,15 +38,20 @@
                 - "positive": higher outlier value injected compared to the current actual value
                 - "negative": lower outliers injected compared to the current actual value
         mu: Distributions mean of the Gaussian Noise injected
         sigma: Distributions std of the Gaussian Noise injected
         random_seed: seed for random number generator.
     """
 
-    __MIN_COLUMNS = {"global": 1, "contextual": 1, "causal": 2, "collective": 2}
+    __MIN_COLUMNS: ClassVar[dict[str, int]] = {
+        "global": 1,
+        "contextual": 1,
+        "causal": 2,
+        "collective": 2,
+    }
 
     def __init__(
         self,
         ref_df: pd.DataFrame,
         anomaly_type: str = "global",
         anomaly_ratio: float = 0.1,
         anomaly_sign: str = "positive",
@@ -76,15 +82,15 @@
         if self.anomaly_sign == "positive":
             return 1
         if self.anomaly_sign == "negative":
             return -1
         raise ValueError(f"Invalid anomaly sign provided: {self.anomaly_sign}")
 
     def inject_anomalies(
-        self, target_df: pd.DataFrame, cols: Sequence[str] = None, **kwargs
+        self, target_df: pd.DataFrame, cols: Optional[Sequence[str]] = None, **kwargs
     ) -> pd.DataFrame:
         """@param target_df: Target DataFrame where anomalies will be injected
         @param cols: Columns to inject anomalies
         @param kwargs: Optional kwargs for individual anomaly types.
         """
         if self.anomaly_type == "global":
             return self._inject_global_anomalies(target_df, cols, **kwargs)
@@ -93,15 +99,15 @@
         if self.anomaly_type == "collective":
             return self._inject_collective_anomalies(target_df, cols, **kwargs)
         if self.anomaly_type == "causal":
             return self._inject_causal_anomalies(target_df, cols, **kwargs)
         raise AttributeError(f"Invalid anomaly type provided: {self.anomaly_type}")
 
     def _inject_global_anomalies(
-        self, target_df: pd.DataFrame, cols: Sequence[str] = None, impact=3
+        self, target_df: pd.DataFrame, cols: Optional[Sequence[str]] = None, impact=3
     ) -> pd.DataFrame:
         target_df = self._init_target_df(target_df, cols)
         anomaly_df = pd.DataFrame(index=target_df.index)
         anomaly_df["is_anomaly"] = 0
 
         for col in self.__injected_cols:
             tseries = target_df[col]
```

### Comparing `numalogic-0.4a1/numalogic/synthetic/sparsity.py` & `numalogic-0.5.0/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/synthetic/timeseries.py` & `numalogic-0.5.0/numalogic/synthetic/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 
 import numpy as np
 import pandas as pd
 from datetime import date
 
 from numpy.typing import NDArray
+from typing import Optional
 
 
 class SyntheticTSGenerator:
     """
     Generates synthetic time series data.
 
     Args:
@@ -47,15 +48,15 @@
         secondary_period=10080,
         seasonal_ts_prob=0.7,
         baseline_range=(200.0, 350.0),
         slope_range=(-0.001, 0.01),
         amplitude_range=(10, 40),
         cosine_ratio_range=(0.5, 0.9),
         noise_range=(5, 15),
-        phase_shift_range: tuple[int, int] = None,
+        phase_shift_range: Optional[tuple[int, int]] = None,
         random_seed: int = 42,
     ):
         self.seq_len = seq_len
         self.num_series = num_series
         self.dt_index = pd.DatetimeIndex(
             pd.date_range(end=date.today(), periods=seq_len, freq=freq)
         )
```

### Comparing `numalogic-0.4a1/numalogic/tools/callbacks.py` & `numalogic-0.5.0/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/tools/data.py` & `numalogic-0.5.0/numalogic/tools/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -115,15 +115,19 @@
 
         self._seq_len = seq_len
         self._data = data.astype(np.float32)
 
     @property
     def data(self) -> npt.NDArray[float]:
         """Returns the reference data in the input shape."""
-        return self._data
+        return self._data.copy()
+
+    def as_array(self) -> npt.NDArray[float]:
+        """Returns the full data in a sequence of shape (batch, seq_len, num_features)."""
+        return self[:]
 
     def create_seq(self, input_: npt.NDArray[float]) -> Generator[npt.NDArray[float], None, None]:
         r"""Yields sequences of specified length from the input data.
 
         Args:
         ----
             input_: A numpy array containing the input data.
@@ -156,16 +160,17 @@
 
     def __getitem__(self, idx: Union[int, slice]) -> npt.NDArray[float]:
         r"""Retrieves a sequence from the input data at the specified index."""
         if isinstance(idx, slice):
             if idx.step is not None:
                 raise ValueError("Slice with step is not supported in StreamingDataset")
             output = []
+            raw_data_size = len(self._data)
             start = idx.start or 0
-            stop = idx.stop or len(self)
+            stop = min(idx.stop, raw_data_size) if idx.stop else raw_data_size
             for i in range(start, stop - self._seq_len + 1):
                 output.append(self._data[i : (i + self._seq_len)])
             return np.stack(output)
         if idx >= len(self):
             raise IndexError(f"{idx} out of bound!")
         return self._data[idx : idx + self._seq_len]
```

### Comparing `numalogic-0.4a1/numalogic/tools/exceptions.py` & `numalogic-0.5.0/numalogic/tools/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,11 +54,17 @@
 
 class RedisRegistryError(Exception):
     """Base class for all exceptions raised by the RedisRegistry class."""
 
     pass
 
 
+class DynamoDBRegistryError(Exception):
+    """Base class for all exceptions raised by the DynamoDBRegistry class."""
+
+    pass
+
+
 class ModelKeyNotFound(RedisRegistryError):
     """Raised when a model key is not found in the registry."""
 
     pass
```

### Comparing `numalogic-0.4a1/numalogic/transforms/__init__.py` & `numalogic-0.5.0/numalogic/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/transforms/_movavg.py` & `numalogic-0.5.0/numalogic/transforms/_movavg.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/transforms/_postprocess.py` & `numalogic-0.5.0/numalogic/transforms/_postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/transforms/_scaler.py` & `numalogic-0.5.0/numalogic/transforms/_scaler.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/numalogic/transforms/_stateless.py` & `numalogic-0.5.0/numalogic/transforms/_stateless.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.4a1/pyproject.toml` & `numalogic-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.4a1"
+version = "0.5.0"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
@@ -12,37 +12,40 @@
 ]
 classifiers = [
     "Topic :: Software Development :: Libraries",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
 ]
 repository = "https://github.com/numaproj/numalogic"
 documentation = "https://numalogic.numaproj.io/"
 homepage = "https://numalogic.numaproj.io/"
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.11"
+python = ">=3.9, <3.12"
 numpy = "^1.23"
 pandas = "^2.0"
 scikit-learn = "^1.2"
 omegaconf = "^2.3.0"
 cachetools = "^5.3.0"
 
 # extras
 mlflow-skinny = { version = ">2.0, <3.0", optional = true }
 redis = {extras = ["hiredis"], version = "^4.5.4", optional = true}
 pynumaflow = { version = "~0.4", optional = true }
+boto3 = { version = "^1.24.64", optional = true }
 
 [tool.poetry.extras]
 mlflow = ["mlflow-skinny"]
 redis = ["redis"]
 numaflow = ["pynumaflow"]
+dynamodb = ["boto3"]
 
 [tool.poetry.group.torch]
 optional = true
 
 [tool.poetry.group.torch.dependencies]
 pytorch-lightning = "^2.0"
 
@@ -51,18 +54,20 @@
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.4.2"
 black = "^23.0"
 pytest = "^7.1"
 pytest-cov = "^4.0"
 torchinfo = "^1.7.2"
-ruff = "^0.0.264"
+ruff = "~0.0.275"
 pre-commit = "^3.3.1"
 fakeredis = "^2.11.2"
 freezegun = "^1.2.2"
+pympler = "^1.0.1"
+moto = "^4.0.1"
 
 [tool.poetry.group.jupyter]
 optional = true
 
 [tool.poetry.group.jupyter.dependencies]
 jupyter = "^1.0.0"
 ipykernel = "^6.15.1"
```

### Comparing `numalogic-0.4a1/PKG-INFO` & `numalogic-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.4a1
+Version: 0.5.0
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
+Provides-Extra: dynamodb
 Provides-Extra: mlflow
 Provides-Extra: numaflow
 Provides-Extra: redis
+Requires-Dist: boto3 (>=1.24.64,<2.0.0) ; extra == "dynamodb"
 Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: mlflow-skinny (>2.0,<3.0) ; extra == "mlflow"
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: pynumaflow (>=0.4,<0.5) ; extra == "numaflow"
 Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0) ; extra == "redis"
```

