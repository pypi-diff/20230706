# Comparing `tmp/nlp-models-2.3.2.tar.gz` & `tmp/nlp-models-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-2.3.2.tar", last modified: Tue Jun 20 16:31:27 2023, max compression
+gzip compressed data, was "nlp-models-3.0.0.tar", last modified: Wed Jul  5 22:20:06 2023, max compression
```

## Comparing `nlp-models-2.3.2.tar` & `nlp-models-3.0.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.967660 nlp-models-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 16:31:12.000000 nlp-models-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-20 16:31:27.967660 nlp-models-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 16:31:12.000000 nlp-models-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 16:31:12.000000 nlp-models-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-20 16:31:27.971660 nlp-models-2.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 16:31:12.000000 nlp-models-2.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.959659 nlp-models-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.963659 nlp-models-2.3.2/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.967660 nlp-models-2.3.2/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9619 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-20 16:31:12.000000 nlp-models-2.3.2/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:31:27.967660 nlp-models-2.3.2/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 16:31:27.000000 nlp-models-2.3.2/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-05 22:19:56.000000 nlp-models-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-05 22:20:06.589419 nlp-models-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-05 22:19:56.000000 nlp-models-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-05 22:19:56.000000 nlp-models-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-05 22:20:06.589419 nlp-models-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-05 22:19:56.000000 nlp-models-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.585419 nlp-models-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-07-05 22:19:56.000000 nlp-models-3.0.0/src/nlp_models/multi_task_model/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:20:06.589419 nlp-models-3.0.0/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 22:20:06.000000 nlp-models-3.0.0/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-2.3.2/LICENSE` & `nlp-models-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.2/PKG-INFO` & `nlp-models-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.3.2
+Version: 3.0.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 2.3.2 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 3.0.0 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

### Comparing `nlp-models-2.3.2/README.md` & `nlp-models-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-2.3.2/setup.cfg` & `nlp-models-3.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 2.3.2
+version = 3.0.0
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-2.3.2/src/bert_classifier/bert.py` & `nlp-models-3.0.0/src/nlp_models/bert_classifier/bert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 bert inheritance class and functions
 '''
 import torch
-from .io import get_pretrained_model
+from ..base.io import get_pretrained_model
 
 
 class BertClass(torch.nn.Module):
     '''
     Custom class for bert classification model
     '''
     def __init__(self, num_label, base_model=None):
```

### Comparing `nlp-models-2.3.2/src/bert_classifier/data.py` & `nlp-models-3.0.0/src/nlp_models/base/data.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,22 @@
     '''
     def __init__(self,
                  dataframe,
                  data_field,
                  label_field,
                  tokenizer,
                  max_len,
-                 multi_label=False
+                 int_labels=False
                  ):
         self.max_len = max_len
         self.data = dataframe
         self.tokenizer = tokenizer
         self.content = self.data[data_field]
         self.label = self.data[label_field]
-        self.multi_label = multi_label
+        self.int_labels = int_labels
 
     def __len__(self):
         return len(self.content)
 
     def __getitem__(self, index):
         content = str(self.content[index])
         content = " ".join(content.split())
@@ -37,27 +37,27 @@
             padding='max_length',
             max_length=self.max_len,
             return_attention_mask=True,
             return_token_type_ids=True,
             return_tensors='pt'
         )
         features = encoded_content
-        if self.multi_label:
+        if not self.int_labels:
             labels = torch.tensor(self.label[index], dtype=torch.float)
         else:
             labels = torch.tensor(self.label[index], dtype=torch.long)
 
         return features, labels
 
 
 def create_label_dict(dataframe, label_col):
     labels = dataframe.groupby(label_col).size().sort_values(ascending=False).index.tolist()
     label_dict = dict([(d, i) for i, d in enumerate(labels)])
     return label_dict
 
 
-def label2id(dataframe, label_col, label_dict, multi_label=False):
-    if multi_label:
-        dataframe[label_col] = dataframe[label_col].apply(lambda c: [int(k in c) for k in label_dict.keys()])
-    else:
-        dataframe[label_col] = dataframe[label_col].apply(lambda c: label_dict[c])
-    return dataframe
+def label_to_id_list(label, labels):
+    return [int(k in label) for k in labels]
+
+
+def label_to_id_int(label, label_dict):
+    return label_dict[label]
```

### Comparing `nlp-models-2.3.2/src/bert_classifier/io.py` & `nlp-models-3.0.0/src/nlp_models/base/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     return torch.load(model_dir, map_location=torch.device(device))
 
 
 def load_model_safe(num_label):
     '''
     preferred and more flexible way to load model
     '''
-    from .bert import BertClass
+    from ..bert_classifier.bert import BertClass
     pretrained_model = get_pretrained_model(PRETRAINED_MODEL, MODEL_NAME)
     model = BertClass(pretrained_model, num_label)
     model.load_state_dict(torch.load(FINETUNED_MODEL_STATE))
     return model
 
 
 def save_label_dict(label_dict, dict_file=LABEL_DICT):
```

### Comparing `nlp-models-2.3.2/src/bert_classifier/predict.py` & `nlp-models-3.0.0/src/nlp_models/bert_classifier/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 Inference module
 '''
 import torch
 from .bert import bert_encoder
-from .io import get_pretrained_tokenizer
+from ..base.io import get_pretrained_tokenizer
 
 
 MAX_LEN = 512
 
 
 class Inference:
     '''
```

### Comparing `nlp-models-2.3.2/src/bert_classifier/train.py` & `nlp-models-3.0.0/src/nlp_models/bert_classifier/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 '''
 Custom training module
 '''
 import time
 import torch
 import numpy as np
 from tqdm import tqdm
-from .io import save_checkpoint
-from .metrics import accuracy_metrics
+from ..base.io import save_checkpoint
+from ..base.utils import batch_to_device
+from ..base.metrics import accuracy_metrics
 
 
 def loss_fn_multiple_labels(outputs, targets):
     '''
     binary cross entropy loss for multi-labels
     '''
     return torch.nn.BCEWithLogitsLoss()(outputs, targets)
@@ -38,22 +39,23 @@
     for epoch in range(epochs):
         model.train()
         print("")
         print(f'======== Epoch {epoch+1} / {epochs} ========')
         print(f'Total steps: {len(train_dataloader)} || Training in progress...')
         t0 = time.time()
         total_train_loss, total_train_accuracy = 0, 0
-        for _, batch in tqdm(enumerate(train_dataloader)):
+        for _, (features, label) in tqdm(enumerate(train_dataloader)):
             # import pdb; pdb.set_trace();
             model.zero_grad(set_to_none=True)
-            ids = batch['input_ids'].squeeze(1).to(device)
-            mask = batch['attention_mask'].squeeze(1).to(device)
-            type_ids = batch['token_type_ids'].squeeze(1).to(device)
-            label = batch['label'].to(device)
-            output = model(ids, mask, type_ids)
+            features = batch_to_device(features, device)
+            # ids = batch['input_ids'].squeeze(1).to(device)
+            # mask = batch['attention_mask'].squeeze(1).to(device)
+            # type_ids = batch['token_type_ids'].squeeze(1).to(device)
+            label = label.to(device)
+            output = model(**features)
 
             loss = loss_fn(output, label)
             total_train_loss += loss.item()
 
             total_train_accuracy += accuracy_metrics(output.detach().cpu().numpy(), label.detach().cpu().numpy())
 
             # if step % 5000 == 0:
@@ -84,17 +86,15 @@
 def validate(model, test_dataloader, device='cpu'):
     '''
     produce validation results
     '''
     model.eval()
     val_targets, val_outputs, val_loss = [], [], []
     with torch.no_grad():
-        for _, batch in enumerate(test_dataloader):
-            ids = batch['input_ids'].squeeze(1).to(device)
-            mask = batch['attention_mask'].squeeze(1).to(device)
-            type_ids = batch['token_type_ids'].squeeze(1).to(device)
-            label = batch['label'].to(device)
-            outputs = model(ids, mask, type_ids)
+        for _, (features, label) in enumerate(test_dataloader):
+            features = batch_to_device(features, device)
+            label = label.to(device)
+            outputs = model(**features)
             val_targets.extend(label.detach().cpu().numpy())
             val_outputs.extend(torch.sigmoid(outputs).detach().cpu().numpy())
             val_loss.extend([loss_fn(outputs, label).detach().cpu().numpy()])
     return val_outputs, val_targets, val_loss
```

### Comparing `nlp-models-2.3.2/src/multi_task_model/layers.py` & `nlp-models-3.0.0/src/nlp_models/base/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import json
-import torch
 from typing import Union
+import torch
 from .utils import fullname, import_from_string
 
 
 class Dropout(torch.nn.Module):
     '''
     Dropout layer
     Param dropout: Sets a dropout value for dense layer
@@ -36,18 +36,18 @@
     One-layer feedforward neural network
     '''
     def __init__(
         self,
         input_features: int,
         output_features: int,
         bias: bool = True,
-        activation_function = torch.nn.Sigmoid(),
+        activation_function=torch.nn.Sigmoid(),
         init_weights: Union[torch.Tensor, None] = None,
-        init_bias: Union[torch.Tensor, None] = None 
-        ) -> None:
+        init_bias: Union[torch.Tensor, None] = None
+    ) -> None:
         super().__init__()
         self.input_features = input_features
         self.output_features = output_features
         self.bias = bias
         self.activation_function = activation_function
         self.linear = torch.nn.Linear(input_features, output_features, bias)
```

### Comparing `nlp-models-2.3.2/src/multi_task_model/mtl.py` & `nlp-models-3.0.0/src/nlp_models/multi_task_model/mtl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import transformers
 import numpy as np
-from .layers import Dropout, Dense
-from .utils import get_embedding_group
+from ..base.layers import Dropout, Dense
+from ..base.utils import get_embedding_group
 
 
 class AutoModelForMTL(torch.nn.Module):
     '''
     Formation of MTL model, sharing a same base model
     '''
     def __init__(self, base_model_name, num_labels, no_normalize=False, *args, **kwargs) -> None:
@@ -29,22 +29,22 @@
     def mean_pooling(self, model_output, attention_mask):
         token_embeddings = model_output[0]
         input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
         return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
 
     def cls_pooling(self, model_output):
         return model_output[0][:, 0]
-    
+
     @staticmethod
-    def save_model(model, dir):
-        torch.save(model, dir)
+    def save_model(model, model_dir):
+        torch.save(model, model_dir)
 
     @staticmethod
-    def load_model(dir, device=torch.device('cpu')):
-        return torch.load(dir, device)
+    def load_model(model_dir, device=torch.device('cpu')):
+        return torch.load(model_dir, device)
 
 
 class MTLInference:
     '''
     class for MTL model infering
     '''
     def __init__(self, tokenizer_card, model_card, num_labels=None, pretrained_model=True, device=torch.device('cpu')) -> None:
@@ -62,14 +62,32 @@
         with torch.no_grad():
             encoded = self.encode(query)
             outputs = self.mtl_model(**encoded)
         pred_label = outputs[0]
         query_embedding = outputs[1]
         return pred_label, query_embedding
 
+    def pred_raw(self, query):
+        return self.predict(query)[0].squeeze().tolist()
+
+    @staticmethod
+    def pred_index(raw_pred):
+        pred = np.flatnonzero(np.array(raw_pred).__gt__(0.5)).tolist()
+        if isinstance(pred, int):
+            return [pred]
+        return pred
+
+    @staticmethod
+    def get_label(pred, label_dict):
+        return [label_dict[p] for p in pred]
+
+    def predict_label(self, query):
+        p_raw = self.pred_raw(query)
+        return self.pred_index(p_raw)
+
     def optimal_answer(self, query, cat_lookup, corpus, top_k=1):
         pred_label, query_embedding = self.predict(query)
         corpus_embeddings, question_corpus, answer_corpus = get_embedding_group(pred_label, cat_lookup, corpus)
         sim_scores = torch.mm(query_embedding, corpus_embeddings.transpose(0, 1).cpu().tolist())
         top_idx = np.argpartition(sim_scores, range(-top_k, 0))[-top_k:][::-1]
         score = list(sim_scores[top_idx])
         question_matched = [question_corpus[i] for i in top_idx]
```

### Comparing `nlp-models-2.3.2/src/multi_task_model/trainer.py` & `nlp-models-3.0.0/src/nlp_models/multi_task_model/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import gc
-import torch
-import transformers
 from pathlib import Path
 from tqdm.notebook import tqdm
 from typing import Optional, Dict
 from dataclasses import dataclass, field
+import torch
+import transformers
 from torch.utils.data import DataLoader
-from .metrics import accuracy
-from .utils import batch_to_device
-from .loss import cross_entropy_loss_fn
+from ..base.metrics import accuracy
+from ..base.utils import batch_to_device
+from ..base.loss import cross_entropy_loss_fn
 
 
 @dataclass
 class Configs:
     epochs: int = 1
     optimizer_class = torch.optim.AdamW
     optimizer_params: Dict[str, float] = field(default_factory=lambda: ({"lr": 2e-5}))
     weight_decay: float = 0.01
     scheduler: str = 'WarmupLinear'
     warmup_steps: int = 10000
-    multi_label: bool = False
     num_labels: Optional[int] = None
     tune_base_model: bool = True
 
 
 class Trainer:
     def __init__(self,
                  model: torch.nn.Module,
@@ -68,23 +67,23 @@
     def train(self):
         epochs = tqdm(range(1, self.configs.epochs + 1), leave=True, desc="Training...")
         for epoch in epochs:
             self.model.train()
             epochs.set_description(f"EPOCH {epoch} / {self.configs.epochs} | training...")
             self.train_one_epoch(epoch)
             self.clear()
-            
+
             self.model.eval()
             epochs.set_description(f"EPOCH {epoch} / {self.configs.epochs} | validating...")
             self.validate_one_epoch(epoch)
             self.clear()
-                
+
             self.print_per_epoch(epoch)
             self.save_checkpoint(epoch)
-            
+
     def continue_training(self, chkpt_file):
         '''
         continue training from checkpoint
         '''
         self.model, self.optimizer, _ = self.load_checkpoint(chkpt_file, self.model, self.optimizer)
         self.schedule_cold_start()
         self.train()
@@ -92,36 +91,35 @@
     def train_one_epoch(self, epoch):
         batches = tqdm(self.train_dataloader, total=len(self.train_dataloader))
         total_train_loss = total_train_acc = 0
         for features, labels in batches:
             labels = labels.to(self.device)
             features = batch_to_device(features, self.device)
             outputs = self.model(**features)
-            loss = cross_entropy_loss_fn(outputs[0], labels, self.configs.multi_label)
+            loss = cross_entropy_loss_fn(outputs[0], labels)
 
             loss.backward()
             torch.nn.utils.clip_grad_norm_(self.model.parameters(), 1.0)
             self.optimizer.step()
             self.scheduler.step()
 
             total_train_loss += loss.item()
             total_train_acc += self.metrics(
                 outputs[0],
                 labels,
                 self.configs.num_labels,
-                self.configs.multi_label,
                 self.device
             ).item()
             
             batches.set_description(f"Train Loss Step: {loss.item():.2f}")
         
         self.logger(
-            epoch, 
-            total_train_acc/len(self.train_dataloader), 
-            total_train_loss/len(self.train_dataloader),
+            epoch,
+            total_train_acc / len(self.train_dataloader),
+            total_train_loss / len(self.train_dataloader),
             'train')
 
     @torch.no_grad()
     def validate_one_epoch(self, epoch):
         '''
         Validate module
         '''
@@ -133,32 +131,31 @@
         batches = tqdm(self.test_dataloader, total=len(self.test_dataloader))
         for features, labels in batches:
             labels = labels.to(self.device)
             features = batch_to_device(features, self.device)
             outputs = self.model(**features)
             val_outputs = torch.cat((val_outputs, outputs[0]), 0)
             val_targets = torch.cat((val_targets, labels), 0)
-            loss = cross_entropy_loss_fn(outputs[0], labels, self.configs.multi_label).reshape(1)
+            loss = cross_entropy_loss_fn(outputs[0], labels).reshape(1)
             val_loss = torch.cat((val_loss, loss), 0)
             batches.set_description(f"Validation Loss Step: {loss.item():.2f}")
         
         avg_val_loss = val_loss.mean().item()
         avg_val_acc = self.metrics(
             val_outputs,
             val_targets,
             self.configs.num_labels,
-            self.configs.multi_label,
             self.device
         ).item()
         
         self.logger(epoch, avg_val_acc, avg_val_loss, 'test')
 
     @staticmethod
     def get_optimizer(param_optimizer,
-                      optimizer_class = torch.optim.AdamW,
+                      optimizer_class=torch.optim.AdamW,
                       optimizer_params: dict = {'lr': 2e-5},
                       weight_decay: float = 0.01
                       ):
         no_decay = ['bias', 'LayerNorm.bias', 'LayerNorm.weight']
         optimizer_grouped_params = [
             {'params': [p for n, p in param_optimizer if not any(nd in n for nd in no_decay)], 'weight_decay': weight_decay},
             {'params': [p for n, p in param_optimizer if any(nd in n for nd in no_decay)], 'weight_decay': 0.0}
@@ -187,16 +184,16 @@
         elif scheduler == 'warmupcosinewithhardrestarts':
             return transformers.get_cosine_with_hard_restarts_schedule_with_warmup(
                 optimizer, num_warmup_steps=warmup_steps, num_training_steps=t_total)
         else:
             raise ValueError(f'Unkown scheduler {scheduler}')
 
     @staticmethod
-    def load_checkpoint(chkpt_dir, model, optimizer: Optional=None):
-        chkpt = torch.load(chkpt_dir)
+    def load_checkpoint(chkpt_dir, model, optimizer=None, device=torch.device('cpu')):
+        chkpt = torch.load(chkpt_dir, device)
         model.load_state_dict(chkpt['model_state_dict'])
         if optimizer:
             optimizer.load_state_dict(chkpt['optimizer_state_dict'])
         return model, optimizer, chkpt
     
     def save_checkpoint(self, epoch):
         if not self.chkpt_dir.exists():
```

### Comparing `nlp-models-2.3.2/src/multi_task_model/utils.py` & `nlp-models-3.0.0/src/nlp_models/base/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,38 +9,38 @@
     Used to load the correct classes from JSON files
     '''
     module = o.__class__.__module__
     if module is None or module == str.__class__.__module__:
         return o.__class__.__name__
     else:
         return module + '.' + o.__class__.__name__
-    
+
 
 def import_from_string(dotted_path):
     '''
     Import a dotted module path and return the attribute/class designed by
     the last name in the path. Raise ImportError if the import failed.
     '''
     try:
         module_path, class_name = dotted_path.rsplit('.', 1)
     except ValueError:
         msg = f'{dotted_path} doesn\'t look like a module path'
         raise ImportError(msg)
-    
+
     try:
         module = importlib.import_module(dotted_path)
     except Exception:
         module = importlib.import_module(module_path)
 
     try:
         return getattr(module, class_name)
     except AttributeError:
         msg = f'Module {module_path} does not define a {class_name} attribute/class'
         raise ImportError(msg)
-    
+
 
 def batch_to_device(batch, target_device: device):
     '''
     Send a pytorch batch to a device (CPU/GPU)
     '''
     for key in batch:
         if isinstance(batch[key], Tensor):
```

### Comparing `nlp-models-2.3.2/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-3.0.0/src/nlp_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.3.2
+Version: 3.0.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlp-models Version: 2.3.2 Summary: Transformers
+Metadata-Version: 2.1 Name: nlp-models Version: 3.0.0 Summary: Transformers
 based NLP models Home-page: https://github.com/minggnim/nlp-models Author: Ming
 Gao Author-email: ming_gao@outlook.com Classifier: Development Status :: 4 -
 Beta Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: License :: OSI
```

