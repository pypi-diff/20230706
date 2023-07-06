# Comparing `tmp/evofr-0.1.19.tar.gz` & `tmp/evofr-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evofr-0.1.19.tar", max compression
+gzip compressed data, was "evofr-0.1.20.tar", max compression
```

## Comparing `evofr-0.1.19.tar` & `evofr-0.1.20.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0    34523 2023-01-10 22:30:08.129997 evofr-0.1.19/LICENSE.txt
--rw-r--r--   0        0        0      888 2023-01-25 21:51:20.520616 evofr-0.1.19/evofr/__init__.py
--rw-r--r--   0        0        0      296 2022-06-23 22:50:02.937378 evofr-0.1.19/evofr/data/__init__.py
--rw-r--r--   0        0        0     1020 2022-09-14 16:20:57.633521 evofr-0.1.19/evofr/data/case_counts.py
--rw-r--r--   0        0        0     4419 2022-10-03 18:11:22.276420 evofr-0.1.19/evofr/data/case_frequencies.py
--rw-r--r--   0        0        0     5110 2022-10-03 18:22:14.382080 evofr-0.1.19/evofr/data/data_helpers.py
--rw-r--r--   0        0        0      471 2022-08-27 00:43:53.017698 evofr-0.1.19/evofr/data/data_spec.py
--rw-r--r--   0        0        0     1410 2022-08-27 00:43:53.018135 evofr-0.1.19/evofr/data/hier_cases.py
--rw-r--r--   0        0        0     2291 2022-10-03 18:10:38.950987 evofr-0.1.19/evofr/data/hier_frequencies.py
--rw-r--r--   0        0        0     3097 2023-02-01 20:10:34.869507 evofr-0.1.19/evofr/data/variant_frequencies.py
--rw-r--r--   0        0        0     1194 2023-01-06 07:10:08.312029 evofr-0.1.19/evofr/infer/BJBackendsScrap.py
--rw-r--r--   0        0        0     8451 2023-01-25 21:51:20.521303 evofr-0.1.19/evofr/infer/InferBlackJax.py
--rw-r--r--   0        0        0     2149 2022-09-15 21:51:48.846733 evofr-0.1.19/evofr/infer/InferMCMC.py
--rw-r--r--   0        0        0     3278 2023-01-25 21:51:20.522220 evofr-0.1.19/evofr/infer/InferSVI.py
--rw-r--r--   0        0        0     2478 2022-08-27 00:43:53.040621 evofr-0.1.19/evofr/infer/MCMC_handler.py
--rw-r--r--   0        0        0     2995 2022-08-27 00:43:53.019730 evofr-0.1.19/evofr/infer/SVI_handler.py
--rw-r--r--   0        0        0     1652 2023-01-25 21:51:20.522616 evofr-0.1.19/evofr/infer/SamplePrior.py
--rw-r--r--   0        0        0      302 2023-01-25 21:51:20.523080 evofr-0.1.19/evofr/infer/__init__.py
--rw-r--r--   0        0        0       78 2023-01-25 21:51:20.523543 evofr-0.1.19/evofr/infer/backends.py
--rw-r--r--   0        0        0      289 2022-12-21 20:12:56.042653 evofr-0.1.19/evofr/models/__init__.py
--rw-r--r--   0        0        0     5083 2023-06-05 20:35:41.520530 evofr-0.1.19/evofr/models/mlr_hierarchical.py
--rw-r--r--   0        0        0     9727 2023-02-01 20:10:34.871076 evofr-0.1.19/evofr/models/mlr_innovation.py
--rw-r--r--   0        0        0    11893 2022-11-08 19:03:50.750502 evofr-0.1.19/evofr/models/mlr_nowcast.py
--rw-r--r--   0        0        0     2886 2022-09-30 21:23:27.866766 evofr-0.1.19/evofr/models/mlr_spline.py
--rw-r--r--   0        0        0      700 2022-08-27 20:30:22.404715 evofr-0.1.19/evofr/models/model_spec.py
--rw-r--r--   0        0        0     4553 2023-04-05 18:05:00.919362 evofr-0.1.19/evofr/models/multinomial_logistic_regression.py
--rw-r--r--   0        0        0     5778 2023-04-20 23:41:11.598062 evofr-0.1.19/evofr/models/mutational_fitness_mlr.py
--rw-r--r--   0        0        0     3333 2022-09-26 17:53:00.939634 evofr-0.1.19/evofr/models/piantham_model.py
--rw-r--r--   0        0        0     2243 2022-08-27 01:00:23.614755 evofr-0.1.19/evofr/models/renewal_model/LAS.py
--rw-r--r--   0        0        0      257 2022-11-08 19:05:19.255557 evofr-0.1.19/evofr/models/renewal_model/__init__.py
--rw-r--r--   0        0        0      149 2022-07-13 00:53:30.188448 evofr-0.1.19/evofr/models/renewal_model/basis_functions/__init__.py
--rw-r--r--   0        0        0      198 2022-07-08 20:37:47.686469 evofr-0.1.19/evofr/models/renewal_model/basis_functions/basis_fns.py
--rw-r--r--   0        0        0     3391 2022-07-14 20:27:07.660069 evofr-0.1.19/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py
--rw-r--r--   0        0        0     4778 2022-09-30 21:38:46.300190 evofr-0.1.19/evofr/models/renewal_model/basis_functions/splines.py
--rw-r--r--   0        0        0     6540 2023-04-06 23:46:59.942673 evofr-0.1.19/evofr/models/renewal_model/model_factories.py
--rw-r--r--   0        0        0     2405 2023-01-10 22:30:08.131767 evofr-0.1.19/evofr/models/renewal_model/model_functions.py
--rw-r--r--   0        0        0     1366 2023-01-10 22:30:08.132058 evofr-0.1.19/evofr/models/renewal_model/model_helpers.py
--rw-r--r--   0        0        0    11983 2023-06-05 20:37:51.670043 evofr-0.1.19/evofr/models/renewal_model/model_options.py
--rw-r--r--   0        0        0     1655 2023-05-25 17:19:40.179597 evofr-0.1.19/evofr/models/renewal_model/renewal_model.py
--rw-r--r--   0        0        0     4392 2022-09-10 15:55:23.454857 evofr-0.1.19/evofr/models/renewal_model/renewal_regression.py
--rw-r--r--   0        0        0     4898 2023-06-05 20:32:08.169834 evofr-0.1.19/evofr/models/renewal_model/renewal_single_variant.py
--rw-r--r--   0        0        0      831 2022-07-08 20:51:40.490887 evofr-0.1.19/evofr/models/renewal_model/spline_incidence.py
--rw-r--r--   0        0        0       62 2023-01-12 23:49:44.920731 evofr-0.1.19/evofr/plotting/__init__.py
--rw-r--r--   0        0        0    11903 2023-01-12 23:49:44.921903 evofr-0.1.19/evofr/plotting/plot_functions.py
--rw-r--r--   0        0        0    11557 2023-01-25 21:51:20.525631 evofr-0.1.19/evofr/plotting/plotting_classes.py
--rw-r--r--   0        0        0       97 2022-12-22 03:54:22.139076 evofr-0.1.19/evofr/posterior/__init__.py
--rw-r--r--   0        0        0     2996 2022-12-22 03:54:22.139787 evofr-0.1.19/evofr/posterior/posterior_handler.py
--rw-r--r--   0        0        0    14113 2023-04-06 23:46:59.943078 evofr-0.1.19/evofr/posterior/posterior_helpers.py
--rw-r--r--   0        0        0      512 2023-06-05 20:39:48.949092 evofr-0.1.19/pyproject.toml
--rw-r--r--   0        0        0      922 1970-01-01 00:00:00.000000 evofr-0.1.19/setup.py
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 evofr-0.1.19/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-01-10 22:30:08.129997 evofr-0.1.20/LICENSE.txt
+-rw-r--r--   0        0        0      891 2023-07-06 19:50:47.255858 evofr-0.1.20/evofr/__init__.py
+-rw-r--r--   0        0        0      296 2022-06-23 22:50:02.937378 evofr-0.1.20/evofr/data/__init__.py
+-rw-r--r--   0        0        0     1020 2022-09-14 16:20:57.633521 evofr-0.1.20/evofr/data/case_counts.py
+-rw-r--r--   0        0        0     4419 2022-10-03 18:11:22.276420 evofr-0.1.20/evofr/data/case_frequencies.py
+-rw-r--r--   0        0        0     5110 2022-10-03 18:22:14.382080 evofr-0.1.20/evofr/data/data_helpers.py
+-rw-r--r--   0        0        0      471 2022-08-27 00:43:53.017698 evofr-0.1.20/evofr/data/data_spec.py
+-rw-r--r--   0        0        0     1410 2022-08-27 00:43:53.018135 evofr-0.1.20/evofr/data/hier_cases.py
+-rw-r--r--   0        0        0     2291 2022-10-03 18:10:38.950987 evofr-0.1.20/evofr/data/hier_frequencies.py
+-rw-r--r--   0        0        0     3097 2023-02-01 20:10:34.869507 evofr-0.1.20/evofr/data/variant_frequencies.py
+-rw-r--r--   0        0        0     1194 2023-01-06 07:10:08.312029 evofr-0.1.20/evofr/infer/BJBackendsScrap.py
+-rw-r--r--   0        0        0     8451 2023-07-06 19:50:05.910611 evofr-0.1.20/evofr/infer/InferBlackJax.py
+-rw-r--r--   0        0        0     2149 2022-09-15 21:51:48.846733 evofr-0.1.20/evofr/infer/InferMCMC.py
+-rw-r--r--   0        0        0     3278 2023-01-25 21:51:20.522220 evofr-0.1.20/evofr/infer/InferSVI.py
+-rw-r--r--   0        0        0     2478 2022-08-27 00:43:53.040621 evofr-0.1.20/evofr/infer/MCMC_handler.py
+-rw-r--r--   0        0        0     2995 2022-08-27 00:43:53.019730 evofr-0.1.20/evofr/infer/SVI_handler.py
+-rw-r--r--   0        0        0     1652 2023-06-23 00:13:54.221670 evofr-0.1.20/evofr/infer/SamplePrior.py
+-rw-r--r--   0        0        0      304 2023-07-06 19:49:35.981482 evofr-0.1.20/evofr/infer/__init__.py
+-rw-r--r--   0        0        0       78 2023-01-25 21:51:20.523543 evofr-0.1.20/evofr/infer/backends.py
+-rw-r--r--   0        0        0      289 2022-12-21 20:12:56.042653 evofr-0.1.20/evofr/models/__init__.py
+-rw-r--r--   0        0        0     6190 2023-06-29 21:35:19.093496 evofr-0.1.20/evofr/models/mlr_hierarchical.py
+-rw-r--r--   0        0        0    11404 2023-06-29 21:35:19.093715 evofr-0.1.20/evofr/models/mlr_innovation.py
+-rw-r--r--   0        0        0    11893 2022-11-08 19:03:50.750502 evofr-0.1.20/evofr/models/mlr_nowcast.py
+-rw-r--r--   0        0        0     2850 2023-06-29 21:35:19.093879 evofr-0.1.20/evofr/models/mlr_spline.py
+-rw-r--r--   0        0        0      700 2022-08-27 20:30:22.404715 evofr-0.1.20/evofr/models/model_spec.py
+-rw-r--r--   0        0        0     4553 2023-04-05 18:05:00.919362 evofr-0.1.20/evofr/models/multinomial_logistic_regression.py
+-rw-r--r--   0        0        0     5813 2023-06-29 21:28:06.249946 evofr-0.1.20/evofr/models/mutational_fitness_mlr.py
+-rw-r--r--   0        0        0     3333 2022-09-26 17:53:00.939634 evofr-0.1.20/evofr/models/piantham_model.py
+-rw-r--r--   0        0        0     2243 2022-08-27 01:00:23.614755 evofr-0.1.20/evofr/models/renewal_model/LAS.py
+-rw-r--r--   0        0        0      257 2022-11-08 19:05:19.255557 evofr-0.1.20/evofr/models/renewal_model/__init__.py
+-rw-r--r--   0        0        0      149 2022-07-13 00:53:30.188448 evofr-0.1.20/evofr/models/renewal_model/basis_functions/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-29 21:35:19.094052 evofr-0.1.20/evofr/models/renewal_model/basis_functions/basis_fns.py
+-rw-r--r--   0        0        0     3341 2023-06-29 21:35:19.094264 evofr-0.1.20/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py
+-rw-r--r--   0        0        0     4716 2023-06-29 21:35:19.094468 evofr-0.1.20/evofr/models/renewal_model/basis_functions/splines.py
+-rw-r--r--   0        0        0     6540 2023-07-06 19:38:05.942556 evofr-0.1.20/evofr/models/renewal_model/model_factories.py
+-rw-r--r--   0        0        0     2405 2023-01-10 22:30:08.131767 evofr-0.1.20/evofr/models/renewal_model/model_functions.py
+-rw-r--r--   0        0        0     1366 2023-01-10 22:30:08.132058 evofr-0.1.20/evofr/models/renewal_model/model_helpers.py
+-rw-r--r--   0        0        0    11983 2023-07-06 19:38:05.943763 evofr-0.1.20/evofr/models/renewal_model/model_options.py
+-rw-r--r--   0        0        0     1655 2023-05-25 17:19:40.179597 evofr-0.1.20/evofr/models/renewal_model/renewal_model.py
+-rw-r--r--   0        0        0     4392 2022-09-10 15:55:23.454857 evofr-0.1.20/evofr/models/renewal_model/renewal_regression.py
+-rw-r--r--   0        0        0     4898 2023-06-29 21:28:06.250450 evofr-0.1.20/evofr/models/renewal_model/renewal_single_variant.py
+-rw-r--r--   0        0        0      831 2022-07-08 20:51:40.490887 evofr-0.1.20/evofr/models/renewal_model/spline_incidence.py
+-rw-r--r--   0        0        0       62 2023-01-12 23:49:44.920731 evofr-0.1.20/evofr/plotting/__init__.py
+-rw-r--r--   0        0        0    11903 2023-01-12 23:49:44.921903 evofr-0.1.20/evofr/plotting/plot_functions.py
+-rw-r--r--   0        0        0    11557 2023-01-25 21:51:20.525631 evofr-0.1.20/evofr/plotting/plotting_classes.py
+-rw-r--r--   0        0        0       97 2022-12-22 03:54:22.139076 evofr-0.1.20/evofr/posterior/__init__.py
+-rw-r--r--   0        0        0     2996 2022-12-22 03:54:22.139787 evofr-0.1.20/evofr/posterior/posterior_handler.py
+-rw-r--r--   0        0        0    14113 2023-04-06 23:46:59.943078 evofr-0.1.20/evofr/posterior/posterior_helpers.py
+-rw-r--r--   0        0        0      511 2023-07-06 19:39:49.176831 evofr-0.1.20/pyproject.toml
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 evofr-0.1.20/PKG-INFO
```

### Comparing `evofr-0.1.19/LICENSE.txt` & `evofr-0.1.20/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/__init__.py` & `evofr-0.1.20/evofr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 from .models import ModelSpec
 from .models import MultinomialLogisticRegression, HierMLR
 from .models import PianthamModel
 from .models import InnovationMLR, InnovationSequenceCounts
 from .models.renewal_model import *
 
-from .infer import SVIHandler, MCMCHandler, BlackJaxHandler
+from .infer import SVIHandler, MCMCHandler #, BlackJaxHandler
 from .infer import (
     InferSVI,
     InferMCMC,
     InferFullRank,
     InferMAP,
     InferNUTS,
-    InferBlackJax,
+    #InferBlackJax,
     init_to_MAP,
 )
 
 from .posterior import PosteriorHandler, MultiPosterior
 from .posterior import get_median, get_quantile, get_quantiles
 from .posterior import (
     get_site_by_variant,
```

### Comparing `evofr-0.1.19/evofr/data/case_counts.py` & `evofr-0.1.20/evofr/data/case_counts.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/data/case_frequencies.py` & `evofr-0.1.20/evofr/data/case_frequencies.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/data/data_helpers.py` & `evofr-0.1.20/evofr/data/data_helpers.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/data/hier_cases.py` & `evofr-0.1.20/evofr/data/hier_cases.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/data/hier_frequencies.py` & `evofr-0.1.20/evofr/data/hier_frequencies.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/data/variant_frequencies.py` & `evofr-0.1.20/evofr/data/variant_frequencies.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/infer/BJBackendsScrap.py` & `evofr-0.1.20/evofr/infer/BJBackendsScrap.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/infer/InferBlackJax.py` & `evofr-0.1.20/evofr/infer/InferBlackJax.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/infer/InferMCMC.py` & `evofr-0.1.20/evofr/infer/InferMCMC.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/infer/InferSVI.py` & `evofr-0.1.20/evofr/infer/InferSVI.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/infer/MCMC_handler.py` & `evofr-0.1.20/evofr/infer/MCMC_handler.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/infer/SVI_handler.py` & `evofr-0.1.20/evofr/infer/SVI_handler.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/infer/SamplePrior.py` & `evofr-0.1.20/evofr/infer/SamplePrior.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/mlr_hierarchical.py` & `evofr-0.1.20/evofr/models/multinomial_logistic_regression.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,159 +1,153 @@
 from functools import partial
 from typing import Optional
 import numpy as np
-from jax import vmap
 import jax.numpy as jnp
+from jax import vmap
 from jax.nn import softmax
 
 import numpyro
 import numpyro.distributions as dist
 
+from .renewal_model.model_options import DirMultinomialSeq
 from .model_spec import ModelSpec
-from .multinomial_logistic_regression import (
-    MultinomialLogisticRegression,
-    simulate_MLR,
-)
-
-
-def simulate_hier_mlr(growth_advantages, freq0, tau, Ns):
-    # Assume all are in list of size groups
-    assert len(growth_advantages) == len(freq0)
-    assert len(growth_advantages) == len(Ns)
-    groups = len(growth_advantages)
-    seq_counts = []
-    for group in range(groups):
-        _, sc_group = simulate_MLR(
-            growth_advantages[group], freq0[group], tau, Ns[group]
-        )
-        seq_counts.append(sc_group)
-    return seq_counts
 
 
-def hier_MLR_numpyro(
-    seq_counts, N, X, tau=None, pool_scale=None, pred=False, var_names=None
+def simulate_MLR_freq(growth_advantage, freq0, tau, max_time):
+    times = np.arange(max_time)
+    delta = np.log(growth_advantage) / tau  # to relative fitness
+    ufreq = freq0 * np.exp(delta * times[..., None])
+    return ufreq / ufreq.sum(axis=-1)[..., None]
+
+
+def simulate_MLR(growth_advantage, freq0, tau, Ns):
+    max_time = len(Ns)
+    freq = simulate_MLR_freq(growth_advantage, freq0, tau, max_time)
+    seq_counts = [
+        np.random.multinomial(Ns[t], freq[t, :]) for t in range(max_time)
+    ]
+    return freq, np.stack(seq_counts)
+
+
+def MLR_numpyro(
+    seq_counts,
+    N,
+    X,
+    tau=None,
+    pred=False,
+    var_names=None,
+    dir_multinomial=False,
+    xi_prior=None,
 ):
-    _, N_variants, N_groups = seq_counts.shape
-    _, N_features, _ = X.shape
-
-    pool_scale = 4.0 if pool_scale is None else pool_scale
+    _, N_variants = seq_counts.shape
+    _, N_features = X.shape
 
     # Sampling parameters
-    with numpyro.plate("features", N_features, dim=-3):
-        with numpyro.plate("variants", N_variants - 1, dim=-2):
-            # Define loc and scale for beta for predictor and variant group
-            beta_loc = numpyro.sample("beta_loc", dist.Normal(0.0, 5.0))
-            beta_scale = numpyro.sample(
-                "beta_scale", dist.HalfNormal(pool_scale)
-            )
-
-            # Use location and scale parameter to draw within group
-            with numpyro.plate("group", N_groups, dim=-1):
-                raw_beta = numpyro.sample(
-                    "raw_beta", dist.Normal(beta_loc, beta_scale)
-                )
+    raw_beta = numpyro.sample(
+        "raw_beta",
+        dist.Normal(0.0, 3.0),
+        sample_shape=(N_features, N_variants - 1),
+    )
 
-    # All parameters are relative to last column / variant
     beta = numpyro.deterministic(
         "beta",
-        jnp.concatenate(
-            (raw_beta, jnp.zeros((N_features, 1, N_groups))), axis=1
-        ),
+        jnp.column_stack(
+            (raw_beta, jnp.zeros(N_features))
+        ),  # All parameters are relative to last column / variant
     )
 
-    # (T, F, G) times (F, V, G) -> (T, V, G)
-    dot_by_group = vmap(jnp.dot, in_axes=(-1, -1), out_axes=-1)
-    logits = dot_by_group(X, beta)  # Logit frequencies by variant
-
-    # Evaluate likelihood
-    obs = None if pred else np.swapaxes(np.nan_to_num(seq_counts), 1, 2)
-
-    _seq_counts = numpyro.sample(
-        "_seq_counts",
-        dist.MultinomialLogits(
-            logits=jnp.swapaxes(logits, 1, 2), total_count=np.nan_to_num(N)
-        ),
-        obs=obs,
-    )
+    logits = jnp.dot(X, beta)  # Logit frequencies by variant
+    freq = numpyro.deterministic("freq", softmax(logits, axis=-1))
 
-    # Re-ordering so groups are last
-    seq_counts = numpyro.deterministic(
-        "seq_counts", jnp.swapaxes(_seq_counts, 2, 1)
-    )
-
-    # Compute frequency
-    numpyro.deterministic("freq", softmax(logits, axis=1))
+    # Evaluate likelihood using either Multinomial or Dirichlet-multinomial
+    if dir_multinomial:
+        seq_likelihood = DirMultinomialSeq(xi_prior=xi_prior)
+        seq_likelihood.model(seq_counts, N, freq, pred=pred)
+    else:
+        obs = None if pred else np.nan_to_num(seq_counts)
+        numpyro.sample(
+            "seq_counts",
+            dist.MultinomialLogits(
+                logits=logits, total_count=np.nan_to_num(N)
+            ),
+            obs=obs,
+        )
 
     # Compute growth advantage from model
     if tau is not None:
         numpyro.deterministic(
-            "ga", jnp.exp(beta[-1, :-1, :] * tau)
+            "ga", jnp.exp(beta[-1, :-1] * tau)
         )  # Last row corresponds to linear predictor / growth advantage
-        numpyro.deterministic("ga_loc", jnp.exp(beta_loc[-1, :, 0] * tau))
 
 
-class HierMLR(ModelSpec):
-    def __init__(self, tau: float, pool_scale: Optional[float] = None) -> None:
-        """Construct ModelSpec for Hierarchial multinomial logistic regression.
+class MultinomialLogisticRegression(ModelSpec):
+    def __init__(
+        self,
+        tau: float,
+        dir_multinomial=False,
+        xi_prior: Optional[float] = None,
+    ) -> None:
+        """Construct ModelSpec for Multinomial logistic regression
 
         Parameters
         ----------
         tau:
             Assumed generation time for conversion to relative R.
-
-        pool_scale:
-            Prior standard deviation for pooling of growth advantages.
+        dir_multinomial:
+            Whether to use a Dirichlet-Multinomial likelihood for sequence counts.
+            Default is False.
+        xi_prior:
+            Prior on seq_counts overdispersion magnitude only used when dir_multinomial == True.
 
         Returns
         -------
-        HierMLR
+        MultinomialLogisticRegression
         """
         self.tau = tau  # Fixed generation time
-        self.pool_scale = pool_scale  # Prior std for coefficients
-        self.model_fn = partial(hier_MLR_numpyro, pool_scale=self.pool_scale)
+        self.dir_multinomial = dir_multinomial
+        self.xi_prior = xi_prior
+        self.model_fn = partial(
+            MLR_numpyro, dir_multinomial=self.dir_multinomial, xi_prior=self.xi_prior
+        )
 
     @staticmethod
-    def make_ols_feature(start, stop, n_groups):
+    def make_ols_feature(start, stop):
         """
-        Construct simple OLS features (1, x) for HierMLR as nd.array.
+        Construct simple OLS features (1, x) for MultinomialLogisticRegression.
 
         Parameters
         ----------
         start:
             Start value for OLS feature.
         stop:
             Stop value for OLS feature.
-
-        n_groups:
-            number of groups in the hierarchical model.
         """
-        X_flat = MultinomialLogisticRegression.make_ols_feature(start, stop)
-        return np.stack([X_flat] * n_groups, axis=-1)
+        t = jnp.arange(start=start, stop=stop)
+        return jnp.column_stack((jnp.ones_like(t), t))
 
     def augment_data(self, data: dict) -> None:
-        T, G = data["N"].shape
+        T = len(data["N"])
         data["tau"] = self.tau
-        data["X"] = self.make_ols_feature(0, T, G)
+        data["X"] = self.make_ols_feature(
+            0, T
+        )  # Use intercept and time as predictors
 
     @staticmethod
     def forecast_frequencies(samples, forecast_L):
         """
-        Use posterior beta to forecast posterior frequencies.
+        Use posterior beta to forecast posterior frequenicies.
         """
 
         # Making feature matrix for forecasting
         last_T = samples["freq"].shape[1]
-        n_groups = samples["freq"].shape[-1]
-
-        X = HierMLR.make_ols_feature(
-            start=last_T, stop=last_T + forecast_L, n_groups=n_groups
+        X = MultinomialLogisticRegression.make_ols_feature(
+            start=last_T, stop=last_T + forecast_L
         )
 
-        # (T, F, G) times (F, V, G) -> (T, V, G)
-        dot_by_group = vmap(jnp.dot, in_axes=(-1, -1), out_axes=-1)
-        dbg_by_sample = vmap(dot_by_group, in_axes=(None, 0), out_axes=0)
-
-        # Creating frequencies from posterior beta
+        # Posterior beta
         beta = jnp.array(samples["beta"])
-        logits = dbg_by_sample(X, beta)
-        samples["freq_forecast"] = softmax(logits, axis=-2)  # (S, T, V, G)
+
+        # Matrix multiplication by sample
+        dot_by_sample = vmap(jnp.dot, in_axes=(None, 0), out_axes=0)
+        logits = dot_by_sample(X, beta)  # Logit frequencies by variant
+        samples["freq_forecast"] = softmax(logits, axis=-1)
         return samples
```

### Comparing `evofr-0.1.19/evofr/models/mlr_innovation.py` & `evofr-0.1.20/evofr/models/mlr_innovation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import List, Optional
 from jax._src.nn.functions import softmax
+from jax import vmap
 import numpy as np
 import pandas as pd
 
 from evofr.data.data_spec import DataSpec
 from evofr.data.data_helpers import prep_dates, prep_sequence_counts
 from evofr.models.renewal_model.model_options import MultinomialSeq
 from .multinomial_logistic_regression import MultinomialLogisticRegression
@@ -85,37 +86,81 @@
         delta_loc_missing = numpyro.sample(
             "delta_loc_missing",
             dist.Normal(0.0, 3.0),
             sample_shape=(self.n_missing,),
         )
 
         # Combine delta_loc for missing and present predictors
-        delta_loc = jnp.empty(N_variants-1)
+        delta_loc = jnp.empty(N_variants - 1)
         delta_loc = delta_loc.at[~self.is_missing].set(delta_loc_present)
         delta_loc = delta_loc.at[self.is_missing].set(delta_loc_missing)
         numpyro.deterministic("delta_loc", delta_loc)
 
         delta_scale = numpyro.sample("delta_scale", dist.HalfNormal(0.1))
 
         raw_delta = numpyro.sample(
-            "raw_delta",
-            dist.Normal(delta_loc, delta_scale)
+            "raw_delta", dist.Normal(delta_loc, delta_scale)
         )
         return raw_delta
 
     def predict(self, features, samples):
         theta = samples["theta"]
         delta_scale = samples["delta_scale"]
 
         # Compute mean of delta
         delta_loc = jnp.einsum("vf, sf -> sv", features, theta)
         prior_delta = np.random.normal(delta_loc, delta_scale)
         return delta_loc, prior_delta
 
 
+def MLR_innovation_model_time_varying(
+    seq_counts, N, innovation_matrix, delta_prior, tau=None, pred=False
+):
+    T, N_variants = seq_counts.shape
+    _, N_features = X.shape
+
+    # Sampling parameters for growth advantages
+    # Sampling intercepts
+    raw_alpha = numpyro.sample(
+        "raw_alpha",
+        dist.Normal(0.0, 3.0),
+        sample_shape=(N_variants - 1,),
+    )
+    alpha = numpyro.deterministic("alpha", jnp.append(raw_alpha, jnp.zeros(1)))
+
+    # Now we need to get the time varying growth advantages
+    # Sampling time-varying innovations from prior model
+    raw_delta = delta_prior.model(N_variants) # (T, V)
+    pivot_delta = jnp.dot(raw_delta,  innovation_matrix[-1,:-1])
+    delta = numpyro.deterministic("delta", jnp.append(raw_delta, -pivot_delta))
+
+    # Innovations to beta for growth advantages
+    # (V, V) * (T, V) -> (T, V) # Gotta make sure shape right?
+    mapped_dot = vmap(jnp.dot, in_axes=(None, 0), out_axes=0)
+    beta = numpyro.deterministic("beta",  mapped_dot(innovation_matrix, delta))
+
+    logits = alpha[:, None] + jnp.cumsum(beta, axis=0)
+    numpyro.deterministic("freq", softmax(logits, axis=-1))
+
+    # Evaluate likelihood of sequence counts given delays
+    # SeqLik.model(seq_counts, N, freq, pred)  # Evaluate likelihood
+
+    obs = None if pred else np.nan_to_num(seq_counts)
+    numpyro.sample(
+        "seq_counts",
+        dist.Multinomial(total_count=np.nan_to_num(N), logits=logits),
+        obs=obs,
+    )
+
+    # Compute growth advantage from model
+    if tau is not None:
+        numpyro.deterministic("ga", jnp.exp(beta * tau)[:-1])
+        numpyro.deterministic("ga_delta", jnp.exp(delta * tau))
+
+
 def MLR_innovation_model(
     seq_counts,
     N,
     X,
     innovation_matrix,
     delta_prior,
     tau=None,
```

### Comparing `evofr-0.1.19/evofr/models/mlr_nowcast.py` & `evofr-0.1.20/evofr/models/mlr_nowcast.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/mlr_spline.py` & `evofr-0.1.20/evofr/models/mlr_spline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional
-from jax._src.device_array import DeviceArray
+from jax import Array
 import numpy as np
 import jax.numpy as jnp
 from jax.nn import softmax
 
 import numpyro
 import numpyro.distributions as dist
 
@@ -57,26 +57,26 @@
         )  # Last row corresponds to linear predictor / growth advantage
 
 
 class MLRSpline(ModelSpec):
     def __init__(
         self,
         tau: float,
-        s: Optional[DeviceArray] = None,
+        s: Optional[Array] = None,
         k: Optional[int] = None,
         order: Optional[int] = None,
     ) -> None:
         """Construct ModelSpec for MLR with a spline basis.
 
         Parameters
         ----------
         tau:
             Assumed generation time for conversion to relative R.
         s:
-            DeviceArray of knot locations for spline.
+            Array of knot locations for spline.
             Mutually exclusive argument with k.
         k:
             Number of basis elements.
             Mutually exclusive argument with s.
         order:
             Order of the spline to be used. Defaults to 4.
         Returns
```

### Comparing `evofr-0.1.19/evofr/models/model_spec.py` & `evofr-0.1.20/evofr/models/model_spec.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/mutational_fitness_mlr.py` & `evofr-0.1.20/evofr/models/mutational_fitness_mlr.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     # Sampling mutation innovations
     raw_delta = numpyro.sample(
         "raw_delta", dist.Normal(0.0, 1.0), sample_shape=(N_mutations,)
     )
     # Innovations to beta
     raw_beta = jnp.dot(mutation_presence, raw_delta)
-    raw_beta = raw_beta - raw_beta[-1]
+    raw_beta = numpyro.deterministic("raw_beta", raw_beta - raw_beta[-1])
 
     # How do we ensure identifiablity?
     # We need to make sure everything is relative to pivot
     # But we won't be able to estimate mutational fitness of things which ...
     # We can have effect by lineage for re-occuring mutations :-D.
 
     beta = numpyro.deterministic(
```

### Comparing `evofr-0.1.19/evofr/models/piantham_model.py` & `evofr-0.1.20/evofr/models/piantham_model.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/LAS.py` & `evofr-0.1.20/evofr/models/renewal_model/LAS.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py` & `evofr-0.1.20/evofr/models/renewal_model/basis_functions/hilbert_space_gaussian_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Optional
-from jax import vmap
-from jax.interpreters.xla import DeviceArray
+from jax import vmap, Array
 import jax.numpy as jnp
 from jax.scipy.special import gammaln
 from .basis_fns import BasisFunction
 
 
 class HSGaussianProcess(BasisFunction):
     """
@@ -50,15 +49,15 @@
         return (
             alpha
             * jnp.sqrt(2 * jnp.pi)
             * rho
             * jnp.exp(-0.5 * jnp.square(rho) * jnp.square(w))
         )
 
-    def make_features(self, data: dict) -> DeviceArray:
+    def make_features(self, data: dict) -> Array:
         T = data["N"].shape[0]
 
         # Make time period
         ts = jnp.arange(T)
 
         # Make eigenvalues
         ms = jnp.arange(1, self.m + 1)
@@ -101,15 +100,15 @@
             * jnp.power(2 * nu, nu)
             / (gammanu * jnp.power(rho, 2 * nu))
         )
         base = 2 * nu * jnp.power(rho, -2) + 4 * jnp.square(jnp.pi * w)
         expon = -nu - 0.5
         return coef * jnp.power(base, expon)
 
-    def make_features(self, data: dict) -> DeviceArray:
+    def make_features(self, data: dict) -> Array:
         T = data["N"].shape[0]
 
         # Make time period
         ts = jnp.arange(T)
 
         # Make eigenvalues
         ms = jnp.arange(1, self.m + 1)
```

### Comparing `evofr-0.1.19/evofr/models/renewal_model/basis_functions/splines.py` & `evofr-0.1.20/evofr/models/renewal_model/basis_functions/splines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from typing import Optional
-from jax import vmap
-from jax.interpreters.xla import DeviceArray
+from jax import vmap, Array
 import jax.numpy as jnp
 from .basis_fns import BasisFunction
 
 
 class Spline(BasisFunction):
     def __init__(
         self,
-        s: Optional[DeviceArray] = None,
+        s: Optional[Array] = None,
         order: Optional[int] = None,
         k: Optional[int] = None,
     ):
         """Construct Spline class.
 
         Parameters
         ----------
@@ -67,30 +66,30 @@
         X = vmap(lambda i: Spline._basis(t, _s, order, i))(
             jnp.arange(0, len(s) + order - 2)
         )  # Make spline basis
         return X.T
 
     def make_features(
         self, data: Optional[dict] = None, T: Optional[float] = None
-    ) -> DeviceArray:
+    ) -> Array:
         # Check for maximum time
         if T is None and data is not None:
             T = data["N"].shape[0]
 
         # If pivots not defined, make self.k equally spaced splines
         if self.s is None and self.k:
             self.s = jnp.linspace(0, T, self.k)
 
         return self.matrix(jnp.arange(T), self.s, self.order)
 
 
 class SplineDeriv:
     def __init__(
         self,
-        s: Optional[DeviceArray] = None,
+        s: Optional[Array] = None,
         order: Optional[int] = None,
         k: Optional[int] = None,
     ):
         """Construct SplineDeriv class. Represents the derivative of the Spline class.
 
         Parameters
         ----------
@@ -147,15 +146,15 @@
         X = vmap(lambda i: SplineDeriv._basis(t, _s, order, i))(
             jnp.arange(0, len(s) + order - 2)
         )  # Make spline basis
         return X.T
 
     def make_features(
         self, data: Optional[dict] = None, T: Optional[float] = None
-    ) -> DeviceArray:
+    ) -> Array:
         # Check for maximum time
         if T is None and data is not None:
             T = data["N"].shape[0]
 
         # If pivots not defined, make self.k equally spaced splines
         if self.s is None and self.k:
             self.s = jnp.linspace(0, T, self.k)
```

### Comparing `evofr-0.1.19/evofr/models/renewal_model/model_factories.py` & `evofr-0.1.20/evofr/models/renewal_model/model_factories.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/model_functions.py` & `evofr-0.1.20/evofr/models/renewal_model/model_functions.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/model_helpers.py` & `evofr-0.1.20/evofr/models/renewal_model/model_helpers.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/model_options.py` & `evofr-0.1.20/evofr/models/renewal_model/model_options.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/renewal_model.py` & `evofr-0.1.20/evofr/models/renewal_model/renewal_model.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/renewal_regression.py` & `evofr-0.1.20/evofr/models/renewal_model/renewal_regression.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/renewal_single_variant.py` & `evofr-0.1.20/evofr/models/renewal_model/renewal_single_variant.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/models/renewal_model/spline_incidence.py` & `evofr-0.1.20/evofr/models/renewal_model/spline_incidence.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/plotting/plot_functions.py` & `evofr-0.1.20/evofr/plotting/plot_functions.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/plotting/plotting_classes.py` & `evofr-0.1.20/evofr/plotting/plotting_classes.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/posterior/posterior_handler.py` & `evofr-0.1.20/evofr/posterior/posterior_handler.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/evofr/posterior/posterior_helpers.py` & `evofr-0.1.20/evofr/posterior/posterior_helpers.py`

 * *Files identical despite different names*

### Comparing `evofr-0.1.19/PKG-INFO` & `evofr-0.1.20/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: evofr
-Version: 0.1.19
+Version: 0.1.20
 Summary: Tools for evolutionary forecasting.
 License: AGPL-3.0
 Author: marlinfiggins
 Author-email: marlinfiggins@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: blackjax (>=0.9.6,<0.10.0)
-Requires-Dist: jax (>=0.3.13,<0.4.0)
-Requires-Dist: jaxlib (>=0.3.10,<0.4.0)
+Requires-Dist: jax (>=0.4.1,<0.5.0)
+Requires-Dist: jaxlib (>=0.4.1,<0.5.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
-Requires-Dist: numpyro (>=0.9.2,<0.10.0)
+Requires-Dist: numpyro (>=0.12.0,<0.13.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
```

