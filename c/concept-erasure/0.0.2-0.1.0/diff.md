# Comparing `tmp/concept-erasure-0.0.2.tar.gz` & `tmp/concept-erasure-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concept-erasure-0.0.2.tar", last modified: Thu Jun  8 01:29:11 2023, max compression
+gzip compressed data, was "concept-erasure-0.1.0.tar", last modified: Wed Jul  5 22:26:46 2023, max compression
```

## Comparing `concept-erasure-0.0.2.tar` & `concept-erasure-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.243680 concept-erasure-0.0.2/
--rw-rw-r--   0 nora      (1000) nora      (1000)     1067 2023-05-06 06:37:09.000000 concept-erasure-0.0.2/LICENSE
--rw-rw-r--   0 nora      (1000) nora      (1000)     3538 2023-06-08 01:29:11.243680 concept-erasure-0.0.2/PKG-INFO
--rw-rw-r--   0 nora      (1000) nora      (1000)     3221 2023-06-08 01:12:37.000000 concept-erasure-0.0.2/README.md
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.223680 concept-erasure-0.0.2/concept_erasure/
--rw-rw-r--   0 nora      (1000) nora      (1000)      316 2023-06-07 20:01:09.000000 concept-erasure-0.0.2/concept_erasure/__init__.py
--rw-rw-r--   0 nora      (1000) nora      (1000)    10680 2023-06-07 20:04:25.000000 concept-erasure-0.0.2/concept_erasure/concept_eraser.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     4019 2023-06-07 20:04:25.000000 concept-erasure-0.0.2/concept_erasure/concept_scrubber.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     5134 2023-05-15 22:58:42.000000 concept-erasure-0.0.2/concept_erasure/data.py
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.231680 concept-erasure-0.0.2/concept_erasure/scrubbing/
--rw-rw-r--   0 nora      (1000) nora      (1000)       83 2023-06-07 06:41:41.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/__init__.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     1665 2023-06-07 20:04:25.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/auto.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     7308 2023-06-07 19:40:03.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/llama.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     5191 2023-06-07 19:39:44.000000 concept-erasure-0.0.2/concept_erasure/scrubbing/neox.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     1746 2023-06-06 08:24:40.000000 concept-erasure-0.0.2/concept_erasure/utils.py
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.227680 concept-erasure-0.0.2/concept_erasure.egg-info/
--rw-rw-r--   0 nora      (1000) nora      (1000)     3538 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/PKG-INFO
--rw-rw-r--   0 nora      (1000) nora      (1000)      609 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/SOURCES.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)        1 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/dependency_links.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)       41 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/entry_points.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)       87 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/requires.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)       16 2023-06-08 01:29:11.000000 concept-erasure-0.0.2/concept_erasure.egg-info/top_level.txt
--rw-rw-r--   0 nora      (1000) nora      (1000)     1312 2023-06-07 19:52:23.000000 concept-erasure-0.0.2/pyproject.toml
--rw-rw-r--   0 nora      (1000) nora      (1000)       38 2023-06-08 01:29:11.243680 concept-erasure-0.0.2/setup.cfg
-drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-06-08 01:29:11.239680 concept-erasure-0.0.2/tests/
--rw-rw-r--   0 nora      (1000) nora      (1000)     5417 2023-06-07 19:38:40.000000 concept-erasure-0.0.2/tests/test_concept_eraser.py
--rw-rw-r--   0 nora      (1000) nora      (1000)     1748 2023-06-07 07:53:07.000000 concept-erasure-0.0.2/tests/test_scrubbing.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-05 22:26:46.084589 concept-erasure-0.1.0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1067 2023-05-06 06:37:09.000000 concept-erasure-0.1.0/LICENSE
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4131 2023-07-05 22:26:46.080589 concept-erasure-0.1.0/PKG-INFO
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3814 2023-07-05 20:18:56.000000 concept-erasure-0.1.0/README.md
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-05 22:26:46.076589 concept-erasure-0.1.0/concept_erasure/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      474 2023-07-05 21:17:30.000000 concept-erasure-0.1.0/concept_erasure/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1326 2023-07-05 21:49:04.000000 concept-erasure-0.1.0/concept_erasure/caching.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2287 2023-07-05 21:20:13.000000 concept-erasure-0.1.0/concept_erasure/concept_scrubber.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5134 2023-05-15 22:58:42.000000 concept-erasure-0.1.0/concept_erasure/data.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)    10046 2023-07-05 22:21:14.000000 concept-erasure-0.1.0/concept_erasure/leace.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1057 2023-07-05 22:21:14.000000 concept-erasure-0.1.0/concept_erasure/random_scrub.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-05 22:26:46.080589 concept-erasure-0.1.0/concept_erasure/scrubbing/
+-rw-rw-r--   0 nora      (1000) nora      (1000)       83 2023-06-07 06:41:41.000000 concept-erasure-0.1.0/concept_erasure/scrubbing/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1656 2023-07-05 21:50:21.000000 concept-erasure-0.1.0/concept_erasure/scrubbing/auto.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7535 2023-07-05 22:21:14.000000 concept-erasure-0.1.0/concept_erasure/scrubbing/llama.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5183 2023-07-05 22:21:14.000000 concept-erasure-0.1.0/concept_erasure/scrubbing/neox.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1605 2023-06-29 07:10:33.000000 concept-erasure-0.1.0/concept_erasure/shrinkage.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1746 2023-06-14 01:09:53.000000 concept-erasure-0.1.0/concept_erasure/utils.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-05 22:26:46.080589 concept-erasure-0.1.0/concept_erasure.egg-info/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4131 2023-07-05 22:26:46.000000 concept-erasure-0.1.0/concept_erasure.egg-info/PKG-INFO
+-rw-rw-r--   0 nora      (1000) nora      (1000)      703 2023-07-05 22:26:46.000000 concept-erasure-0.1.0/concept_erasure.egg-info/SOURCES.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)        1 2023-07-05 22:26:46.000000 concept-erasure-0.1.0/concept_erasure.egg-info/dependency_links.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)       41 2023-07-05 22:26:46.000000 concept-erasure-0.1.0/concept_erasure.egg-info/entry_points.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)       87 2023-07-05 22:26:46.000000 concept-erasure-0.1.0/concept_erasure.egg-info/requires.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)       16 2023-07-05 22:26:46.000000 concept-erasure-0.1.0/concept_erasure.egg-info/top_level.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1312 2023-07-05 21:52:42.000000 concept-erasure-0.1.0/pyproject.toml
+-rw-rw-r--   0 nora      (1000) nora      (1000)       38 2023-07-05 22:26:46.084589 concept-erasure-0.1.0/setup.cfg
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-05 22:26:46.080589 concept-erasure-0.1.0/tests/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6801 2023-07-05 22:21:14.000000 concept-erasure-0.1.0/tests/test_leace.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1748 2023-06-07 07:53:07.000000 concept-erasure-0.1.0/tests/test_scrubbing.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1233 2023-06-29 07:06:53.000000 concept-erasure-0.1.0/tests/test_shrinkage.py
```

### Comparing `concept-erasure-0.0.2/LICENSE` & `concept-erasure-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `concept-erasure-0.0.2/PKG-INFO` & `concept-erasure-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: concept-erasure
-Version: 0.0.2
+Version: 0.1.0
 Summary: Erasing concepts from neural representations with provable guarantees
 License: MIT License
 Keywords: fairness,interpretability,explainable-ai
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Least-Squares Concept Erasure (LEACE)
 Concept erasure aims to remove specified features from a representation. It can be used to improve fairness (e.g. preventing a classifier from using gender or race) and interpretability (e.g. removing a concept to observe changes in model behavior). This is the repo for **LEAst-squares Concept Erasure (LEACE)**, a closed-form method which provably prevents all linear classifiers from detecting a concept while inflicting the least possible damage to the representation. You can check out the paper [here](https://arxiv.org/abs/2306.03819).
 
 # Installation
 
+We require Python 3.10 or later. You can install the package from PyPI:
+
 ```bash
 pip install concept-erasure
 ```
 
 # Usage
 
-`ConceptEraser` is the central class in this repo. It keeps track of the covariance and cross-covariance statistics needed to erase a concept, and lazily computes the LEACE parameters when needed.
+The two main classes in this repo are `LeaceFitter` and `LeaceEraser`.
+
+- `LeaceFitter` keeps track of the covariance and cross-covariance statistics needed to compute the LEACE erasure function. These statistics can be updated in an incremental fashion with `LeaceFitter.update()`. The erasure function is lazily computed when the `.eraser` property is accessed. This class uses O(_d<sup>2</sup>_) memory, where _d_ is the dimensionality of the representation, so you may want to discard it after computing the erasure function.
+- `LeaceEraser` is a compact representation of the LEACE erasure function, using only O(_dk_) memory, where _k_ is the number of classes in the concept you're trying to erase (or equivalently, the _dimensionality_ of the concept if it's not categorical).
 
 ## Batch usage
 
-In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is using `ConceptEraser.fit()` followed by `ConceptEraser.forward()`:
+In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is by using the `LeaceEraser.fit()` convenience method:
 
 ```python
 import torch
 from sklearn.datasets import make_classification
 from sklearn.linear_model import LogisticRegression
 
-from concept_erasure import ConceptEraser
+from concept_erasure import LeaceEraser
 
 n, d, k = 2048, 128, 2
 
 X, Y = make_classification(
     n_samples=n,
     n_features=d,
     n_classes=k,
@@ -45,50 +50,50 @@
 Y_t = torch.from_numpy(Y)
 
 # Logistic regression does learn something before concept erasure
 real_lr = LogisticRegression(max_iter=1000).fit(X, Y)
 beta = torch.from_numpy(real_lr.coef_)
 assert beta.norm(p=torch.inf) > 0.1
 
-eraser = ConceptEraser.fit(X_t, Y_t)
+eraser = LeaceEraser.fit(X_t, Y_t)
 X_ = eraser(X_t)
 
 # But learns nothing after
 null_lr = LogisticRegression(max_iter=1000, tol=0.0).fit(X_.numpy(), Y)
 beta = torch.from_numpy(null_lr.coef_)
 assert beta.norm(p=torch.inf) < 1e-4
 ```
 
 ## Streaming usage
-If you have a **stream** of data, you can use `ConceptEraser.update()` to update the statistics and `ConceptEraser.forward()` to erase the concept. This is useful if you have a large dataset and want to avoid storing it all in memory.
+If you have a **stream** of data, you can use `LeaceFitter.update()` to update the statistics. This is useful if you have a large dataset and want to avoid storing it all in memory.
 
 ```python
-from concept_erasure import ConceptEraser
+from concept_erasure import LeaceFitter
 from sklearn.datasets import make_classification
 import torch
 
 n, d, k = 2048, 128, 2
 
 X, Y = make_classification(
     n_samples=n,
     n_features=d,
     n_classes=k,
     random_state=42,
 )
 X_t = torch.from_numpy(X)
 Y_t = torch.from_numpy(Y)
 
-eraser = ConceptEraser(d, 1, dtype=X_t.dtype)
+fitter = LeaceFitter(d, 1, dtype=X_t.dtype)
 
 # Compute cross-covariance matrix using batched updates
 for x, y in zip(X_t.chunk(2), Y_t.chunk(2)):
-    eraser.update(x, y)
+    fitter.update(x, y)
 
 # Erase the concept from the data
-x_ = eraser(X_t[0])
+x_ = fitter.eraser(X_t[0])
 ```
 
 # Paper replication
 
 Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in [this repo](https://github.com/EleutherAI/tagged-pile). We plan to upload the tagged datasets to the HuggingFace Hub shortly.
 
 ## Concept scrubbing
```

### Comparing `concept-erasure-0.0.2/README.md` & `concept-erasure-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # Least-Squares Concept Erasure (LEACE)
 Concept erasure aims to remove specified features from a representation. It can be used to improve fairness (e.g. preventing a classifier from using gender or race) and interpretability (e.g. removing a concept to observe changes in model behavior). This is the repo for **LEAst-squares Concept Erasure (LEACE)**, a closed-form method which provably prevents all linear classifiers from detecting a concept while inflicting the least possible damage to the representation. You can check out the paper [here](https://arxiv.org/abs/2306.03819).
 
 # Installation
 
+We require Python 3.10 or later. You can install the package from PyPI:
+
 ```bash
 pip install concept-erasure
 ```
 
 # Usage
 
-`ConceptEraser` is the central class in this repo. It keeps track of the covariance and cross-covariance statistics needed to erase a concept, and lazily computes the LEACE parameters when needed.
+The two main classes in this repo are `LeaceFitter` and `LeaceEraser`.
+
+- `LeaceFitter` keeps track of the covariance and cross-covariance statistics needed to compute the LEACE erasure function. These statistics can be updated in an incremental fashion with `LeaceFitter.update()`. The erasure function is lazily computed when the `.eraser` property is accessed. This class uses O(_d<sup>2</sup>_) memory, where _d_ is the dimensionality of the representation, so you may want to discard it after computing the erasure function.
+- `LeaceEraser` is a compact representation of the LEACE erasure function, using only O(_dk_) memory, where _k_ is the number of classes in the concept you're trying to erase (or equivalently, the _dimensionality_ of the concept if it's not categorical).
 
 ## Batch usage
 
-In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is using `ConceptEraser.fit()` followed by `ConceptEraser.forward()`:
+In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is by using the `LeaceEraser.fit()` convenience method:
 
 ```python
 import torch
 from sklearn.datasets import make_classification
 from sklearn.linear_model import LogisticRegression
 
-from concept_erasure import ConceptEraser
+from concept_erasure import LeaceEraser
 
 n, d, k = 2048, 128, 2
 
 X, Y = make_classification(
     n_samples=n,
     n_features=d,
     n_classes=k,
@@ -34,50 +39,50 @@
 Y_t = torch.from_numpy(Y)
 
 # Logistic regression does learn something before concept erasure
 real_lr = LogisticRegression(max_iter=1000).fit(X, Y)
 beta = torch.from_numpy(real_lr.coef_)
 assert beta.norm(p=torch.inf) > 0.1
 
-eraser = ConceptEraser.fit(X_t, Y_t)
+eraser = LeaceEraser.fit(X_t, Y_t)
 X_ = eraser(X_t)
 
 # But learns nothing after
 null_lr = LogisticRegression(max_iter=1000, tol=0.0).fit(X_.numpy(), Y)
 beta = torch.from_numpy(null_lr.coef_)
 assert beta.norm(p=torch.inf) < 1e-4
 ```
 
 ## Streaming usage
-If you have a **stream** of data, you can use `ConceptEraser.update()` to update the statistics and `ConceptEraser.forward()` to erase the concept. This is useful if you have a large dataset and want to avoid storing it all in memory.
+If you have a **stream** of data, you can use `LeaceFitter.update()` to update the statistics. This is useful if you have a large dataset and want to avoid storing it all in memory.
 
 ```python
-from concept_erasure import ConceptEraser
+from concept_erasure import LeaceFitter
 from sklearn.datasets import make_classification
 import torch
 
 n, d, k = 2048, 128, 2
 
 X, Y = make_classification(
     n_samples=n,
     n_features=d,
     n_classes=k,
     random_state=42,
 )
 X_t = torch.from_numpy(X)
 Y_t = torch.from_numpy(Y)
 
-eraser = ConceptEraser(d, 1, dtype=X_t.dtype)
+fitter = LeaceFitter(d, 1, dtype=X_t.dtype)
 
 # Compute cross-covariance matrix using batched updates
 for x, y in zip(X_t.chunk(2), Y_t.chunk(2)):
-    eraser.update(x, y)
+    fitter.update(x, y)
 
 # Erase the concept from the data
-x_ = eraser(X_t[0])
+x_ = fitter.eraser(X_t[0])
 ```
 
 # Paper replication
 
 Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in [this repo](https://github.com/EleutherAI/tagged-pile). We plan to upload the tagged datasets to the HuggingFace Hub shortly.
 
 ## Concept scrubbing
```

### Comparing `concept-erasure-0.0.2/concept_erasure/concept_eraser.py` & `concept-erasure-0.1.0/concept_erasure/leace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,289 +1,272 @@
+from dataclasses import dataclass
 from typing import Literal
 
 import torch
-from torch import Tensor, nn
+from torch import Tensor
 
-ErasureMethod = Literal["leace", "orth", "relaxed"]
+from .caching import cached_property, invalidates_cache
+from .shrinkage import optimal_linear_shrinkage
 
+ErasureMethod = Literal["leace", "orth"]
 
-class ConceptEraser(nn.Module):
-    """Minimally edit features to make specified concepts linearly undetectable.
 
-    There are three erasure methods currently supported:
-    - `"leace"`: Least-squares Concept Erasure from https://arxiv.org/abs/2306.03819.
-    - `"orth"`: Orthogonal projection onto colsp(Sigma_xz)^perp.
-    - `"relaxed"`: Applies a PSD map with spectral norm <= 1 that ensures the resulting
-    cross-covariance matrix Cov(PX, Z) has spectral norm no greater than `svd_tol`.
-    Importantly, this method **does not** ensure linear guardedness, but may be useful
-    for concept scrubbing purposes. It has the benefit of being less sensitive to noise
-    and the choice of `svd_tol` than other methods.
+@dataclass(frozen=True)
+class LeaceEraser:
+    """Compact LEACE eraser that surgically erases a concept from a representation."""
+
+    proj_left: Tensor
+    proj_right: Tensor
+    bias: Tensor | None
+
+    @classmethod
+    def fit(cls, x: Tensor, z: Tensor, **kwargs) -> "LeaceEraser":
+        """Convenience method to fit a LeaceEraser on data and return it."""
+        return LeaceFitter.fit(x, z, **kwargs).eraser
+
+    @property
+    def P(self) -> Tensor:
+        """The projection matrix."""
+        eye = torch.eye(
+            self.proj_left.shape[0],
+            device=self.proj_left.device,
+            dtype=self.proj_left.dtype,
+        )
+        return eye - self.proj_left @ self.proj_right
+
+    def __call__(self, x: Tensor) -> Tensor:
+        """Apply the projection to the input tensor."""
+        delta = x - self.bias if self.bias is not None else x
+
+        # Ensure we do the matmul in the most efficient order.
+        x_ = x - (delta @ self.proj_right.T) @ self.proj_left.T
+        return x_.type_as(x)
+
+
+class LeaceFitter:
+    """Fits a LEACE eraser that surgically erases a concept from a representation.
+
+    This class implements Least-squares Concept Erasure (LEACE) from
+    https://arxiv.org/abs/2306.03819. You can also use a slightly simpler orthogonal
+    projection-based method by setting `method="orth"`.
+
+    This class stores the covariance statistics needed to compute the LEACE eraser.
+    This allows the statistics to be updated incrementally.
+
+    Since the LEACE projection matrix is guaranteed to be a rank k - 1 perturbation of
+    the identity, we store it implicitly in the d x k matrices `proj_left` and
+    `proj_right`. The full matrix is given by `torch.eye(d) - proj_left @ proj_right`.
     """
 
     mean_x: Tensor
     """Running mean of X."""
 
     mean_z: Tensor
     """Running mean of Z."""
 
-    sigma_xz_M2: Tensor
+    sigma_xz_: Tensor
     """Unnormalized cross-covariance matrix X^T Z."""
 
-    x_M2: Tensor | None
+    sigma_xx_: Tensor | None
     """Unnormalized covariance matrix X^T X."""
 
-    n_x: Tensor
+    n: Tensor
     """Number of X samples seen so far."""
 
-    n_z: Tensor
-    """Number of Z samples seen so far."""
-
-    _P: Tensor | None
-
     @classmethod
-    def fit(cls, x: Tensor, z: Tensor, **kwargs) -> "ConceptEraser":
-        """Convenience method to fit a ConceptEraser on data and return it."""
+    def fit(cls, x: Tensor, z: Tensor, **kwargs) -> "LeaceFitter":
+        """Convenience method to fit a LeaceFitter on data and return it."""
         n, d = x.shape
         _, k = z.reshape(n, -1).shape
 
-        return cls(d, k, device=x.device, dtype=x.dtype, **kwargs).update(x, z)
+        fitter = LeaceFitter(d, k, device=x.device, dtype=x.dtype, **kwargs)
+        return fitter.update(x, z)
 
     def __init__(
         self,
         x_dim: int,
         z_dim: int,
         method: ErasureMethod = "leace",
         *,
         affine: bool = True,
         constrain_cov_trace: bool = True,
         device: str | torch.device | None = None,
         dtype: torch.dtype | None = None,
+        shrinkage: bool = True,
         svd_tol: float = 0.01,
     ):
-        """Initialize a ConceptEraser.
+        """Initialize a `LeaceFitter`.
 
         Args:
-            x_dim: Dimensionality of the input.
-            z_dim: Dimensionality of the labels.
+            x_dim: Dimensionality of the representation.
+            z_dim: Dimensionality of the concept.
             method: Type of projection matrix to use.
             affine: Whether to use a bias term to ensure the unconditional mean of the
                 features remains the same after erasure.
             constrain_cov_trace: Whether to constrain the trace of the covariance of X
                 after erasure to be no greater than before erasure. This is especially
                 useful when injecting the scrubbed features back into a model. Without
                 this constraint, the norm of the model's hidden states may diverge in
                 some cases.
             device: Device to put the statistics on.
             dtype: Data type to use for the statistics.
+            shrinkage: Whether to use shrinkage to estimate the covariance matrix of X.
             svd_tol: Singular values under this threshold are truncated, both during
                 the phase where we do SVD on the cross-covariance matrix, and at the
                 phase where we compute the pseudoinverse of the projected covariance
                 matrix. Higher values are more numerically stable and result in less
                 damage to the representation, but may leave trace correlations intact.
         """
         super().__init__()
 
-        self.z_dim = z_dim
         self.x_dim = x_dim
+        self.z_dim = z_dim
 
         self.affine = affine
         self.constrain_cov_trace = constrain_cov_trace
-        self.proj_rank = z_dim
         self.method = method
-        self.z_dim = z_dim
+        self.shrinkage = shrinkage
 
         assert svd_tol > 0.0, "`svd_tol` must be positive for numerical stability."
         self.svd_tol = svd_tol
 
-        self.register_buffer("mean_x", torch.zeros(x_dim, device=device, dtype=dtype))
-        self.register_buffer("mean_z", self.mean_x.new_zeros(z_dim))
-        self.register_buffer(
-            "sigma_xz_M2",
-            self.mean_x.new_zeros(x_dim, z_dim),
-        )
-        self.register_buffer("n_x", torch.tensor(0, device=device, dtype=dtype))
-        self.register_buffer("n_z", torch.tensor(0, device=device, dtype=dtype))
-        self.register_buffer("_P", None)
+        self.mean_x = torch.zeros(x_dim, device=device, dtype=dtype)
+        self.mean_z = torch.zeros(z_dim, device=device, dtype=dtype)
+
+        self.n = torch.tensor(0, device=device, dtype=dtype)
+        self.sigma_xz_ = torch.zeros(x_dim, z_dim, device=device, dtype=dtype)
+        # self.sigma_zz_ = torch.zeros(z_dim, z_dim, device=device, dtype=dtype)
 
         if self.method == "leace":
-            M2 = self.mean_x.new_zeros(x_dim, x_dim)
-        elif self.method in ("orth", "relaxed"):
-            M2 = None
+            self.sigma_xx_ = torch.zeros(x_dim, x_dim, device=device, dtype=dtype)
+        elif self.method == "orth":
+            self.sigma_xx_ = None
         else:
             raise ValueError(f"Unknown projection type {self.method}")
 
-        self.register_buffer("x_M2", M2)
-
-    def forward(self, x: Tensor) -> Tensor:
-        """Minimally edit `x` to remove correlations with the target concepts.
-
-        Args:
-            x: Representations of shape (..., x_dim).
-
-        Returns:
-            The edited representations of shape (..., x_dim).
-        """
-        d, _ = self.sigma_xz_M2.shape
-        assert self.n_x > 0, "Call update() before forward()"
-        assert x.shape[-1] == d
-
-        if self.affine:
-            x_ = (x - self.mean_x) @ self.P.T + self.mean_x
-            return x_.type_as(x)
-        else:
-            return (x.type_as(self.P) @ self.P.T).type_as(x)
-
     @torch.no_grad()
-    def update(self, x: Tensor, z: Tensor | None = None) -> "ConceptEraser":
-        """Update the running statistics with a new batch of data.
-
-        It's possible to call this method without `z` if you only want to update the
-        statistics of X. This is useful if you don't have labels but want to adjust the
-        mean and covariance of X to match a new dataset.
-        """
-        d, c = self.sigma_xz_M2.shape
+    @invalidates_cache("eraser")
+    def update(self, x: Tensor, z: Tensor) -> "LeaceFitter":
+        """Update the running statistics with a new batch of data."""
+        d, c = self.sigma_xz_.shape
         x = x.reshape(-1, d).type_as(self.mean_x)
-
-        if not x.isfinite().all():
-            raise RuntimeError("Non-finite values in input")
-
         n, d2 = x.shape
-        assert d == d2, f"Unexpected number of features {d2}"
 
-        # We always have an X, we might not have a Z
-        self.n_x += n
+        assert d == d2, f"Unexpected number of features {d2}"
+        self.n += n
 
         # Welford's online algorithm
         delta_x = x - self.mean_x
-        self.mean_x += delta_x.sum(dim=0) / self.n_x
+        self.mean_x += delta_x.sum(dim=0) / self.n
         delta_x2 = x - self.mean_x
 
         # Update the covariance matrix of X if needed (for LEACE)
         if self.method == "leace":
-            assert self.x_M2 is not None
-            self.x_M2.addmm_(delta_x.mT, delta_x2)
+            assert self.sigma_xx_ is not None
+            self.sigma_xx_.addmm_(delta_x.mT, delta_x2)
 
-        # Invalidate the cached projection matrix
-        self._P = None
+        z = z.reshape(n, -1).type_as(x)
+        assert z.shape[-1] == c, f"Unexpected number of classes {z.shape[-1]}"
 
-        # We do have labels, so we can update the Z statistics
-        if z is not None:
-            # y might start out 1D, but we want to treat it as 2D
-            z = z.reshape(n, -1).type_as(x)
-            assert z.shape[-1] == c, f"Unexpected number of classes {z.shape[-1]}"
-
-            self.n_z += n
-
-            delta_z = z - self.mean_z
-            self.mean_z += delta_z.sum(dim=0) / self.n_x
-            delta_z2 = z - self.mean_z
+        delta_z = z - self.mean_z
+        self.mean_z += delta_z.sum(dim=0) / self.n
+        delta_z2 = z - self.mean_z
 
-            # Update the cross-covariance matrix
-            self.sigma_xz_M2.addmm_(delta_x.mT, delta_z2)
+        # Update the cross-covariance matrix
+        self.sigma_xz_.addmm_(delta_x.mT, delta_z2)
 
         return self
 
-    @property
-    def P(self) -> Tensor:
-        """Projection matrix for removing the subspace."""
-        if self._P is not None:
-            return self._P
-
+    @cached_property
+    def eraser(self) -> LeaceEraser:
+        """Erasure function lazily computed given the current statistics."""
         eye = torch.eye(self.x_dim, device=self.mean_x.device, dtype=self.mean_x.dtype)
-        u, s, _ = torch.linalg.svd(self.sigma_xz, full_matrices=False)
 
-        if self.method == "relaxed":
-            # Treat `svd_tol` as a constraint on the spectral norm of sigma_xz after
-            # erasure. In this case Q is not actually a projection matrix, it's a
-            # PSD non-expansive map (spectral norm <= 1).
-            Q = eye - u * torch.clamp(1 - self.svd_tol / s, 0, 1) @ u.T
+        # Compute the whitening and unwhitening matrices
+        if self.method == "leace":
+            sigma = self.sigma_xx
+            L, V = torch.linalg.eigh(sigma)
+
+            # Threshold used by torch.linalg.pinv
+            mask = L > (L[-1] * sigma.shape[-1] * torch.finfo(L.dtype).eps)
+
+            # Assuming PSD; account for numerical error
+            L.clamp_min_(0.0)
+
+            W = V * L.rsqrt().where(mask, 0.0) @ V.mT
+            W_inv = V * L.sqrt().where(mask, 0.0) @ V.mT
         else:
-            # Throw away singular values that are too small
-            mask = s > self.svd_tol
-            if not mask.any():
-                return eye
-
-            u = u[:, mask]
-            Q = eye - u @ u.T if mask.any() else eye
-
-            # Save this for debugging
-            self.proj_rank = mask.sum().item()
-
-        if self.method != "leace":
-            self._P = Q
-            return self._P
+            W, W_inv = eye, eye
 
-        self._P = self.proj_for_subspace(u)
-        return self._P
+        u, s, _ = torch.linalg.svd(W @ self.sigma_xz, full_matrices=False)
 
-    def proj_for_subspace(self, u: Tensor) -> Tensor:
-        """Projection matrix for removing the subspace."""
-        eye = torch.eye(self.x_dim, device=self.mean_x.device, dtype=self.mean_x.dtype)
-        Q = eye - u @ u.T
+        # Throw away singular values that are too small
+        u *= s > self.svd_tol
 
-        # LEACE and orthogonal projection matrix computation
-        # Adjust Q to account for the covariance of X
-        sigma = self.cov_x
-        A = Q @ sigma @ Q
-        try:
-            L, V = torch.linalg.eigh(A)
-        except torch.linalg.LinAlgError as e:
-            # Better error messages in the common case where A is non-finite
-            if not A.isfinite().all():
-                raise RuntimeError("Non-finite values in covariance matrix") from e
-            else:
-                raise e
-
-        # Manual pseudoinverse
-        L = L.reciprocal().where(L > self.svd_tol, 0.0)
-        P = sigma @ V @ torch.diag_embed(L) @ V.mT
-
-        # Prevent the covariance trace from increasing
-        old_trace = torch.trace(sigma)
-        new_trace = torch.trace(P @ sigma @ P.mT)
-
-        # If applying the projection matrix increases the variance, this might
-        # cause instability, especially when erasure is applied multiple times.
-        # We regularize toward the orthogonal projection matrix to avoid this.
-        if self.constrain_cov_trace and new_trace > old_trace:
-            # Set up the variables for the quadratic equation
-            x = new_trace
-            y = 2 * torch.trace(P @ sigma @ Q.mT)
-            z = torch.trace(Q @ sigma @ Q.mT)
-            w = old_trace
-
-            # Solve for the mixture of P and Q that makes the trace equal to the
-            # trace of the original covariance matrix
-            discr = torch.sqrt(4 * w * x - 4 * w * y + 4 * w * z - 4 * x * z + y**2)
-            alpha1 = (-y / 2 + z - discr / 2) / (x - y + z)
-            alpha2 = (-y / 2 + z + discr / 2) / (x - y + z)
-
-            # Choose the positive root
-            alpha = torch.where(alpha1 > 0, alpha1, alpha2).clamp(0, 1)
-            P = alpha * P + (1 - alpha) * Q
+        proj_left = W_inv @ u
+        proj_right = u.T @ W
+
+        if self.constrain_cov_trace and self.method == "leace":
+            P = eye - proj_left @ proj_right
+
+            # Prevent the covariance trace from increasing
+            sigma = self.sigma_xx
+            old_trace = torch.trace(sigma)
+            new_trace = torch.trace(P @ sigma @ P.mT)
+
+            # If applying the projection matrix increases the variance, this might
+            # cause instability, especially when erasure is applied multiple times.
+            # We regularize toward the orthogonal projection matrix to avoid this.
+            if new_trace > old_trace:
+                Q = eye - u @ u.T
+
+                # Set up the variables for the quadratic equation
+                x = new_trace
+                y = 2 * torch.trace(P @ sigma @ Q.mT)
+                z = torch.trace(Q @ sigma @ Q.mT)
+                w = old_trace
+
+                # Solve for the mixture of P and Q that makes the trace equal to the
+                # trace of the original covariance matrix
+                discr = torch.sqrt(
+                    4 * w * x - 4 * w * y + 4 * w * z - 4 * x * z + y**2
+                )
+                alpha1 = (-y / 2 + z - discr / 2) / (x - y + z)
+                alpha2 = (-y / 2 + z + discr / 2) / (x - y + z)
+
+                # Choose the positive root
+                alpha = torch.where(alpha1 > 0, alpha1, alpha2).clamp(0, 1)
+                P = alpha * P + (1 - alpha) * Q
+
+                # TODO: Avoid using SVD here
+                u, s, vh = torch.linalg.svd(eye - P)
+                proj_left = u * s.sqrt()
+                proj_right = vh * s.sqrt()
 
-        return P
+        return LeaceEraser(
+            proj_left, proj_right, bias=self.mean_x if self.affine else None
+        )
 
     @property
-    def cov_x(self) -> Tensor:
+    def sigma_xx(self) -> Tensor:
         """The covariance matrix of X."""
-        assert self.n_x > 1, "Call update() before accessing cov_x"
+        assert self.n > 1, "Call update() before accessing sigma_xx"
         assert (
-            self.x_M2 is not None
+            self.sigma_xx_ is not None
         ), "Covariance statistics are not being tracked for X"
 
-        cov = self.x_M2 / (self.n_x - 1)
-
         # Accumulated numerical error may cause this to be slightly non-symmetric
-        return (cov + cov.mT) / 2
+        S_hat = (self.sigma_xx_ + self.sigma_xx_.mT) / 2
+
+        # Apply Random Matrix Theory-based shrinkage
+        if self.shrinkage:
+            return optimal_linear_shrinkage(S_hat / self.n, self.n)
+
+        # Just apply Bessel's correction
+        else:
+            return S_hat / (self.n - 1)
 
     @property
     def sigma_xz(self) -> Tensor:
         """The cross-covariance matrix."""
-        assert self.n_z > 1, "Call update() with labels before accessing sigma_xz"
-        return self.sigma_xz_M2 / (self.n_z - 1)
-
-    def finalize(self) -> "ConceptEraser":
-        """Compute the projection matrix and drop covariance matrices."""
-        self.P
-        self.x_M2 = None
-        return self
+        assert self.n > 1, "Call update() with labels before accessing sigma_xz"
+        return self.sigma_xz_ / (self.n - 1)
```

### Comparing `concept-erasure-0.0.2/concept_erasure/data.py` & `concept-erasure-0.1.0/concept_erasure/data.py`

 * *Files identical despite different names*

### Comparing `concept-erasure-0.0.2/concept_erasure/scrubbing/auto.py` & `concept-erasure-0.1.0/concept_erasure/scrubbing/auto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from warnings import warn
 
 import torch.nn.functional as F
 from datasets import Dataset
 from transformers import GPTNeoXForCausalLM, LlamaForCausalLM, PreTrainedModel
 
-from ..concept_eraser import ErasureMethod
 from ..concept_scrubber import ConceptScrubber
+from ..leace import ErasureMethod
 from .llama import patch_attention_llama_, scrub_llama
 from .neox import patch_attention_neox_, scrub_neox
 
 
 def patch_attention_(model: PreTrainedModel):
     """Patch the attention layers of a model to use fast attention kernels."""
     ty = model.config.model_type
```

### Comparing `concept-erasure-0.0.2/concept_erasure/scrubbing/llama.py` & `concept-erasure-0.1.0/concept_erasure/scrubbing/llama.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from transformers.models.llama.modeling_llama import (
     LlamaAttention,
     LlamaDecoderLayer,
     apply_rotary_pos_emb,
 )
 
-from concept_erasure import ConceptEraser, ConceptScrubber, ErasureMethod
+from concept_erasure import ConceptScrubber, ErasureMethod, LeaceFitter
 from concept_erasure.utils import assert_type
 
 
 def _fast_attn(
     self,
     hidden_states: torch.Tensor,
     attention_mask: torch.Tensor | None = None,
@@ -118,35 +118,38 @@
 
     # Enumerate the layers
     for j, layer in enumerate(tqdm(base.layers, unit="layer")):
         assert isinstance(layer, LlamaDecoderLayer)
 
         attn_eraser = None
         if scrubber is not None:
-            attn_eraser = ConceptEraser(
+            attn_fitter = LeaceFitter(
                 d, k, affine=affine, device=model.device, method=method
             )
-            scrubber.erasers[f"layers-{j}-input_layernorm"] = attn_eraser
 
             # Fit the next eraser on the previous hidden states
             for x, z in tqdm(zip(xs, zs), desc="Fitting (attn)", total=N):
                 assert scrubber is not None
 
                 # Discard post-LN output and recompute during application to save RAM
                 x = layer.input_layernorm(x.to(model.device))
-                attn_eraser.update(x, z)
+                attn_fitter.update(x, z)
+
+            attn_eraser = attn_fitter.eraser
+            scrubber.erasers[f"layers-{j}-input_layernorm"] = attn_eraser
+            del attn_fitter  # Save VRAM
 
         # Run attention & MLP with the erasers we just fit
         for i, x in tqdm(enumerate(xs), desc="Applying (attn)", total=N):
             # Bring back to the accelerator
             x = x.to(model.device)
             h = layer.input_layernorm(x)  # Recomputing from above
 
             # Apply the eraser
-            if scrubber is not None:
+            if attn_eraser is not None and scrubber is not None:
                 h = attn_eraser(h).type_as(h)
 
             pos_ids = torch.arange(0, h.shape[-2], device=h.device, dtype=torch.long)
             pos_ids = pos_ids.unsqueeze(0).view(-1, h.shape[-2])
 
             h, _, __ = layer.self_attn(h, position_ids=pos_ids)
             h = x = x + h  # Post-attention residual connection
@@ -161,35 +164,38 @@
 
         # Skip the part where we scrub the MLP if we're not doing that
         if not sublayers:
             continue
 
         mlp_eraser = None
         if scrubber is not None:
-            mlp_eraser = ConceptEraser(
+            mlp_fitter = LeaceFitter(
                 d, k, affine=affine, device=model.device, method=method
             )
-            scrubber.erasers[f"layers-{j}-post_attention_layernorm"] = mlp_eraser
 
             # Fit the next eraser on the previous hidden states
             for x, z in tqdm(zip(xs, zs), desc="Fitting (MLP)", total=N):
                 assert scrubber is not None
 
                 # Discard post-LN output and recompute during application to save RAM
                 x = layer.post_attention_layernorm(x.to(model.device))
-                mlp_eraser.update(x, z)
+                mlp_fitter.update(x, z)
+
+            mlp_eraser = mlp_fitter.eraser
+            scrubber.erasers[f"layers-{j}-post_attention_layernorm"] = mlp_eraser
+            del mlp_fitter  # Save VRAM
 
         for i, x in tqdm(enumerate(xs), desc="Applying (MLP)", total=N):
             # Bring back to the accelerator
             x = x.to(model.device)
             h = layer.post_attention_layernorm(x)  # Recomputing from above
 
             # Apply the eraser
-            if scrubber is not None:
-                h = mlp_eraser(h).type_as(h)
+            if mlp_eraser is not None and scrubber is not None:
+                h = mlp_eraser.eraser(h).type_as(h)
 
             h = layer.mlp(h)
             h = x + h  # Post-MLP residual connection
             xs[i] = h.to("cpu", non_blocking=True)
 
     for batch, x in tqdm(zip(train.iter(batch_size), xs), total=N):
         assert isinstance(batch, dict)
```

### Comparing `concept-erasure-0.0.2/concept_erasure/scrubbing/neox.py` & `concept-erasure-0.1.0/concept_erasure/scrubbing/neox.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from transformers import (
     GPTNeoXForCausalLM,
     GPTNeoXLayer,
     GPTNeoXModel,
 )
 from transformers.models.gpt_neox.modeling_gpt_neox import GPTNeoXAttention
 
-from concept_erasure import ConceptEraser, ConceptScrubber, ErasureMethod
+from concept_erasure import ConceptScrubber, ErasureMethod, LeaceFitter
 from concept_erasure.utils import assert_type
 
 
 def patch_attention_neox_(model: torch.nn.Module):
     """Patch the attention layers of a GPTNeoX model to use fast attention kernels."""
 
     def fast_attn(self, q, k, v, attention_mask=None, head_mask=None):
@@ -76,38 +76,37 @@
     # Enumerate the layers
     for j, layer in enumerate(tqdm(base.layers, unit="layer")):
         assert isinstance(layer, GPTNeoXLayer)
         assert layer.use_parallel_residual, "Only parallel residual is supported"
 
         attn_eraser, mlp_eraser = None, None
         if scrubber is not None:
-            attn_eraser = ConceptEraser(
+            attn_fitter = LeaceFitter(
                 d, k, affine=affine, device=model.device, method=method
             )
-            scrubber.erasers[f"layers-{j}-input_layernorm"] = attn_eraser
+            scrubber.erasers[f"layers-{j}-input_layernorm"] = attn_fitter
 
-            mlp_eraser = ConceptEraser(
+            mlp_fitter = LeaceFitter(
                 d, k, affine=affine, device=model.device, method=method
             )
-            scrubber.erasers[f"layers-{j}-post_attention_layernorm"] = mlp_eraser
+            scrubber.erasers[f"layers-{j}-post_attention_layernorm"] = mlp_fitter
 
             # Fit the next eraser on the previous hidden states
             for i, (x, z) in tqdm(enumerate(zip(xs, zs)), desc="Fitting", total=N):
                 x = x.to(model.device)
 
                 # Discard post-LN output and recompute during application to save RAM
                 attn_norm_out = layer.input_layernorm(x)
-                attn_eraser.update(attn_norm_out, z)
+                attn_fitter.update(attn_norm_out, z)
 
                 mlp_norm_out = layer.post_attention_layernorm(attn_norm_out)
-                mlp_eraser.update(mlp_norm_out, z)
+                mlp_fitter.update(mlp_norm_out, z)
 
-            # Save VRAM by discarding the covariance matrices
-            attn_eraser.finalize()
-            mlp_eraser.finalize()
+            attn_eraser, mlp_eraser = attn_fitter.eraser, mlp_fitter.eraser
+            del attn_fitter, mlp_fitter  # Save VRAM
 
         # Run attention & MLP with the erasers we just fit
         for i, x in tqdm(enumerate(xs), desc="Applying", total=N):
             x = x.to(model.device)
             h = layer.input_layernorm(x)  # Recomputing from above
 
             if attn_eraser is not None:
```

### Comparing `concept-erasure-0.0.2/concept_erasure/utils.py` & `concept-erasure-0.1.0/concept_erasure/utils.py`

 * *Files identical despite different names*

### Comparing `concept-erasure-0.0.2/concept_erasure.egg-info/PKG-INFO` & `concept-erasure-0.1.0/concept_erasure.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 Metadata-Version: 2.1
 Name: concept-erasure
-Version: 0.0.2
+Version: 0.1.0
 Summary: Erasing concepts from neural representations with provable guarantees
 License: MIT License
 Keywords: fairness,interpretability,explainable-ai
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Least-Squares Concept Erasure (LEACE)
 Concept erasure aims to remove specified features from a representation. It can be used to improve fairness (e.g. preventing a classifier from using gender or race) and interpretability (e.g. removing a concept to observe changes in model behavior). This is the repo for **LEAst-squares Concept Erasure (LEACE)**, a closed-form method which provably prevents all linear classifiers from detecting a concept while inflicting the least possible damage to the representation. You can check out the paper [here](https://arxiv.org/abs/2306.03819).
 
 # Installation
 
+We require Python 3.10 or later. You can install the package from PyPI:
+
 ```bash
 pip install concept-erasure
 ```
 
 # Usage
 
-`ConceptEraser` is the central class in this repo. It keeps track of the covariance and cross-covariance statistics needed to erase a concept, and lazily computes the LEACE parameters when needed.
+The two main classes in this repo are `LeaceFitter` and `LeaceEraser`.
+
+- `LeaceFitter` keeps track of the covariance and cross-covariance statistics needed to compute the LEACE erasure function. These statistics can be updated in an incremental fashion with `LeaceFitter.update()`. The erasure function is lazily computed when the `.eraser` property is accessed. This class uses O(_d<sup>2</sup>_) memory, where _d_ is the dimensionality of the representation, so you may want to discard it after computing the erasure function.
+- `LeaceEraser` is a compact representation of the LEACE erasure function, using only O(_dk_) memory, where _k_ is the number of classes in the concept you're trying to erase (or equivalently, the _dimensionality_ of the concept if it's not categorical).
 
 ## Batch usage
 
-In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is using `ConceptEraser.fit()` followed by `ConceptEraser.forward()`:
+In most cases, you probably have a batch of feature vectors `X` and concept labels `Z` and want to erase the concept from `X`. The easiest way to do this is by using the `LeaceEraser.fit()` convenience method:
 
 ```python
 import torch
 from sklearn.datasets import make_classification
 from sklearn.linear_model import LogisticRegression
 
-from concept_erasure import ConceptEraser
+from concept_erasure import LeaceEraser
 
 n, d, k = 2048, 128, 2
 
 X, Y = make_classification(
     n_samples=n,
     n_features=d,
     n_classes=k,
@@ -45,50 +50,50 @@
 Y_t = torch.from_numpy(Y)
 
 # Logistic regression does learn something before concept erasure
 real_lr = LogisticRegression(max_iter=1000).fit(X, Y)
 beta = torch.from_numpy(real_lr.coef_)
 assert beta.norm(p=torch.inf) > 0.1
 
-eraser = ConceptEraser.fit(X_t, Y_t)
+eraser = LeaceEraser.fit(X_t, Y_t)
 X_ = eraser(X_t)
 
 # But learns nothing after
 null_lr = LogisticRegression(max_iter=1000, tol=0.0).fit(X_.numpy(), Y)
 beta = torch.from_numpy(null_lr.coef_)
 assert beta.norm(p=torch.inf) < 1e-4
 ```
 
 ## Streaming usage
-If you have a **stream** of data, you can use `ConceptEraser.update()` to update the statistics and `ConceptEraser.forward()` to erase the concept. This is useful if you have a large dataset and want to avoid storing it all in memory.
+If you have a **stream** of data, you can use `LeaceFitter.update()` to update the statistics. This is useful if you have a large dataset and want to avoid storing it all in memory.
 
 ```python
-from concept_erasure import ConceptEraser
+from concept_erasure import LeaceFitter
 from sklearn.datasets import make_classification
 import torch
 
 n, d, k = 2048, 128, 2
 
 X, Y = make_classification(
     n_samples=n,
     n_features=d,
     n_classes=k,
     random_state=42,
 )
 X_t = torch.from_numpy(X)
 Y_t = torch.from_numpy(Y)
 
-eraser = ConceptEraser(d, 1, dtype=X_t.dtype)
+fitter = LeaceFitter(d, 1, dtype=X_t.dtype)
 
 # Compute cross-covariance matrix using batched updates
 for x, y in zip(X_t.chunk(2), Y_t.chunk(2)):
-    eraser.update(x, y)
+    fitter.update(x, y)
 
 # Erase the concept from the data
-x_ = eraser(X_t[0])
+x_ = fitter.eraser(X_t[0])
 ```
 
 # Paper replication
 
 Scripts used to generate the part-of-speech tags for the concept scrubbing experiments can be found in [this repo](https://github.com/EleutherAI/tagged-pile). We plan to upload the tagged datasets to the HuggingFace Hub shortly.
 
 ## Concept scrubbing
```

### Comparing `concept-erasure-0.0.2/concept_erasure.egg-info/SOURCES.txt` & `concept-erasure-0.1.0/concept_erasure.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 LICENSE
 README.md
 pyproject.toml
 concept_erasure/__init__.py
-concept_erasure/concept_eraser.py
+concept_erasure/caching.py
 concept_erasure/concept_scrubber.py
 concept_erasure/data.py
+concept_erasure/leace.py
+concept_erasure/random_scrub.py
+concept_erasure/shrinkage.py
 concept_erasure/utils.py
 concept_erasure.egg-info/PKG-INFO
 concept_erasure.egg-info/SOURCES.txt
 concept_erasure.egg-info/dependency_links.txt
 concept_erasure.egg-info/entry_points.txt
 concept_erasure.egg-info/requires.txt
 concept_erasure.egg-info/top_level.txt
 concept_erasure/scrubbing/__init__.py
 concept_erasure/scrubbing/auto.py
 concept_erasure/scrubbing/llama.py
 concept_erasure/scrubbing/neox.py
-tests/test_concept_eraser.py
-tests/test_scrubbing.py
+tests/test_leace.py
+tests/test_scrubbing.py
+tests/test_shrinkage.py
```

### Comparing `concept-erasure-0.0.2/pyproject.toml` & `concept-erasure-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = {text = "MIT License"}
 dependencies = [
     "datasets",
     "torch",
     # 4.0 introduced the breaking change of using return_dict=True by default
     "transformers>=4.0.0",
 ]
-version = "0.0.2"
+version = "0.1.0"
 
 [project.optional-dependencies]
 dev = [
     "numpy",
     "pre-commit",
     "pytest",
     "pyright",
```

### Comparing `concept-erasure-0.0.2/tests/test_concept_eraser.py` & `concept-erasure-0.1.0/tests/test_leace.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,74 @@
-from itertools import product
+from itertools import pairwise, product
 
-import numpy as np
 import pytest
 import torch
+import torch.nn.functional as F
 from sklearn.datasets import make_classification
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import LinearSVC
 
-from concept_erasure import ConceptEraser
+from concept_erasure import ErasureMethod, LeaceFitter, optimal_linear_shrinkage
 
 
-def test_stats():
-    num_features = 3
-    num_classes = 2
+@pytest.mark.parametrize("shrinkage", [False, True])
+def test_stats(shrinkage: bool):
     batch_size = 10
     num_batches = 5
+    num_classes = 2
+    num_features = 3
+    N = batch_size * num_batches
 
-    eraser = ConceptEraser(num_features, num_classes)
+    fitter = LeaceFitter(num_features, num_classes, shrinkage=shrinkage)
 
     # Generate random data
     torch.manual_seed(42)
     x_data = [torch.randn(batch_size, num_features) for _ in range(num_batches)]
     y_data = [
         torch.randint(0, num_classes, (batch_size, num_classes))
         for _ in range(num_batches)
     ]
+    projections = []
 
     # Compute cross-covariance matrix using batched updates
     for x, y in zip(x_data, y_data):
-        eraser.update(x, y)
+        fitter.update(x, y)
+        projections.append(fitter.eraser.P)
+
+    # Make sure the cached eraser is getting invalidated on update() correctly
+    for p1, p2 in pairwise(projections):
+        assert not torch.allclose(p1, p2)
 
     # Compute the expected cross-covariance matrix using the whole dataset
     x_all = torch.cat(x_data)
     y_all = torch.cat(y_data)
     mean_x = x_all.mean(dim=0)
     mean_y = y_all.type_as(x_all).mean(dim=0)
     x_centered = x_all - mean_x
     y_centered = y_all - mean_y
 
     expected_cov = torch.einsum("b...m,b...n->...mn", x_centered, x_centered)
-    expected_cov /= batch_size * num_batches - 1
+    if shrinkage:
+        expected_cov = optimal_linear_shrinkage(
+            expected_cov / N, batch_size * num_batches
+        )
+    else:
+        expected_cov /= N - 1
 
     expected_sigma_xz = torch.einsum("b...m,b...n->...mn", x_centered, y_centered)
-    expected_sigma_xz /= batch_size * num_batches - 1
+    expected_sigma_xz /= N - 1
 
-    # Compare the computed cross-covariance matrix with the expected one
-    torch.testing.assert_close(eraser.cov_x, expected_cov)
-    torch.testing.assert_close(eraser.sigma_xz, expected_sigma_xz)
+    torch.testing.assert_close(fitter.sigma_xx, expected_cov)
+    torch.testing.assert_close(fitter.sigma_xz, expected_sigma_xz)
 
 
 # Both `1` and `2` are binary classification problems, but `1` means the labels are
 # encoded in a 1D one-hot vector, while `2` means the labels are encoded in an
 # n x 2 one-hot matrix.
 @pytest.mark.parametrize("num_classes", [1, 2, 3, 5, 10, 20])
-@torch.no_grad()
 def test_projection(num_classes: int):
     n, d = 2048, 128
     num_distinct = max(num_classes, 2)
 
     X, Y = make_classification(
         n_samples=n,
         n_features=d,
@@ -68,32 +79,60 @@
     X_t = torch.from_numpy(X)
     Y_t = torch.from_numpy(Y)
     if num_classes > 1:
         Y_1h = torch.nn.functional.one_hot(Y_t, num_classes)
     else:
         Y_1h = Y_t
 
+    bools = [False, True]
+    methods: list[ErasureMethod] = ["leace", "orth"]
     eps = 2e-9
-    mse_dict: dict[tuple[bool, str], float] = {}
+    for affine, method, shrink in product(bools, methods, bools):
+        # Shrinkage not applicable to orthogonal projection
+        if method == "orth" and shrink:
+            continue
+
+        fitter = LeaceFitter(
+            d,
+            num_classes,
+            affine=affine,
+            dtype=X_t.dtype,
+            method=method,
+            shrinkage=shrink,
+        ).update(X_t, Y_1h)
 
-    for affine, method in product([False, True], ["leace", "orth"]):
-        eraser = ConceptEraser.fit(X_t, Y_1h, affine=affine, method=method)
+        eraser = fitter.eraser
         X_ = eraser(X_t)
 
+        # Check first-order optimality condition. To account for the nullspace
+        # constraint, we use the canonical form for oblique projection matrices,
+        # fixing the nullspace and only optimizing over the range space.
+        A, s, B_t = torch.linalg.svd(eraser.P)
+        A, B = A[:, s > 0.5].requires_grad_(True), B_t[s > 0.5].T
+
+        # See "A matrix representation formula for a nonzero projection operator" in
+        # https://en.wikipedia.org/wiki/Projection_(linear_algebra)
+        P = A @ torch.inverse(B.T @ A) @ B.T
+        x_ = (X_t - fitter.mean_x) @ P.T + fitter.mean_x if affine else X_t @ P.T
+
+        # Define a random positive definite inner product
+        L = torch.randn(d, d, dtype=X_t.dtype) / d**0.5
+        loss = F.mse_loss(x_ @ L, X_t @ L)
+        loss.backward()
+
+        # Should be optimal iff we're using LEACE with the bias term and no shrinkage
+        assert (A.grad.norm() < eps) == (affine and method == "leace" and not shrink)
+
         # Check idempotence
         torch.testing.assert_close(eraser(X_), X_)
 
         # Check that the rank of the update <= num_classes
         rank = torch.linalg.svdvals(X_t - X_).gt(eps).sum()
         assert rank <= num_classes
 
-        # Record the mean squared error for comparison
-        X_np = X_.numpy()
-        mse_dict[(affine, method)] = np.square(X_np - X).mean()
-
         # Check that the unconditional mean is unchanged
         if affine:
             torch.testing.assert_close(X_t.mean(dim=0), X_.mean(dim=0))
 
         # Compute class means and check that they are equal after the projection
         class_means_ = torch.stack(
             [X_[Y_t == c].mean(dim=0) for c in range(num_distinct)]
@@ -130,17 +169,13 @@
             # The dual formulation injects random noise into the solution
             dual=False,
             # Unfortunately the intercept is subject to L2 regularization; setting this
             # to a large value largely cancels out the effect. Regularizing the
             # intercept can cause the coefficients to get larger than they should be.
             intercept_scaling=1e6,
             tol=eps,
-        ).fit(X_np, Y)
+        ).fit(X_.numpy(), Y)
         assert abs(null_svm.coef_).max() < eps
 
         # But it should learn something before the projection
         real_svm = LinearSVC(dual=False, intercept_scaling=1e6, tol=eps).fit(X, Y)
         assert abs(real_svm.coef_).max() > 0.1
-
-    # Check that using method="leace" strictly better than "orth"
-    assert mse_dict[(True, "leace")] < mse_dict[(True, "orth")]
-    assert mse_dict[(False, "leace")] < mse_dict[(False, "orth")]
```

### Comparing `concept-erasure-0.0.2/tests/test_scrubbing.py` & `concept-erasure-0.1.0/tests/test_scrubbing.py`

 * *Files identical despite different names*

