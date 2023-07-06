# Comparing `tmp/autotm-0.1.0.tar.gz` & `tmp/autotm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotm-0.1.0.tar", max compression
+gzip compressed data, was "autotm-0.2.0.tar", max compression
```

## Comparing `autotm-0.1.0.tar` & `autotm-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0    35149 2023-06-29 08:39:40.067544 autotm-0.1.0/LICENSE
--rw-r--r--   0        0        0     2676 2023-06-29 08:39:40.067544 autotm-0.1.0/README.md
--rw-r--r--   0        0        0     1126 2023-06-29 08:50:04.426083 autotm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 08:39:40.151545 autotm-0.1.0/src/autotm/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:39:40.151545 autotm-0.1.0/src/autotm/algorithms_for_tuning/__init__.py
--rw-r--r--   0        0        0     4988 2023-06-29 08:39:40.151545 autotm-0.1.0/src/autotm/algorithms_for_tuning/bayesian_optimization/bayes_opt.py
--rw-r--r--   0        0        0        0 2023-06-29 08:39:40.151545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/__init__.py
--rw-r--r--   0        0        0       84 2023-06-29 08:39:40.151545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/config.yaml
--rw-r--r--   0        0        0     2370 2023-06-29 08:39:40.151545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/crossover.py
--rw-r--r--   0        0        0    44465 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/ga.py
--rwxr-xr-x   0        0        0     4579 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/genetic_algorithm.py
--rw-r--r--   0        0        0     4736 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/mutation.py
--rw-r--r--   0        0        0     3287 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/selection.py
--rw-r--r--   0        0        0     5255 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/strategy.py
--rw-r--r--   0        0        0     4121 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/algorithms_for_tuning/individuals.py
--rw-r--r--   0        0        0     3621 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/algorithms_for_tuning/nelder_mead_optimization/nelder_mead.py
--rw-r--r--   0        0        0     1506 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/batch_vect_utils.py
--rw-r--r--   0        0        0     1388 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/data_generator/synthetic_data_generation.ipynb
--rw-r--r--   0        0        0        0 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/fitness/__init__.py
--rw-r--r--   0        0        0     7367 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/fitness/base_score.py
--rw-r--r--   0        0        0     1720 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/fitness/external_scores.py
--rw-r--r--   0        0        0    25659 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/fitness/intratext_coherence_score.py
--rw-r--r--   0        0        0      116 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/fitness/scores.py
--rw-r--r--   0        0        0     2966 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/fitness/tasks.py
--rw-r--r--   0        0        0    32248 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/fitness/tm.py
--rw-r--r--   0        0        0     6387 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/infer.py
--rwxr-xr-x   0        0        0     1353 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/make-recovery-file.py
--rw-r--r--   0        0        0     6874 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/params_logging_utils.py
--rw-r--r--   0        0        0        0 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/preprocessing/__init__.py
--rw-r--r--   0        0        0    12770 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/preprocessing/dictionaries_preparation.py
--rw-r--r--   0        0        0     4752 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/preprocessing/text_preprocessing.py
--rw-r--r--   0        0        0     2618 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/schemas.py
--rw-r--r--   0        0        0     4710 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/utils.py
--rw-r--r--   0        0        0        0 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/visualization/__init__.py
--rw-r--r--   0        0        0     9692 2023-06-29 08:39:40.155545 autotm-0.1.0/src/autotm/visualization/dynamic_tracker.py
--rw-r--r--   0        0        0     4011 1970-01-01 00:00:00.000000 autotm-0.1.0/setup.py
--rw-r--r--   0        0        0     3825 1970-01-01 00:00:00.000000 autotm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-05 13:01:19.927029 autotm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3257 2023-07-06 15:27:22.555559 autotm-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.927029 autotm-0.2.0/autotm/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.927029 autotm-0.2.0/autotm/algorithms_for_tuning/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.927029 autotm-0.2.0/autotm/algorithms_for_tuning/bayesian_optimization/__init__.py
+-rw-r--r--   0        0        0     4952 2023-07-05 13:01:19.927029 autotm-0.2.0/autotm/algorithms_for_tuning/bayesian_optimization/bayes_opt.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.927029 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-05 13:01:19.927029 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/config.yaml
+-rw-r--r--   0        0        0     4054 2023-07-06 15:27:22.555559 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/crossover.py
+-rw-r--r--   0        0        0    44098 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/ga.py
+-rwxr-xr-x   0        0        0     4809 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/genetic_algorithm.py
+-rw-r--r--   0        0        0     4896 2023-07-06 14:53:03.523296 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/mutation.py
+-rw-r--r--   0        0        0     3287 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/selection.py
+-rw-r--r--   0        0        0     5203 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/strategy.py
+-rw-r--r--   0        0        0     4161 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/algorithms_for_tuning/individuals.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/algorithms_for_tuning/nelder_mead_optimization/__init__.py
+-rw-r--r--   0        0        0     3597 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/algorithms_for_tuning/nelder_mead_optimization/nelder_mead.py
+-rw-r--r--   0        0        0    11432 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/base.py
+-rw-r--r--   0        0        0     1506 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/batch_vect_utils.py
+-rw-r--r--   0        0        0     1322 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/data_generator/synthetic_data_generation.ipynb
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/fitness/__init__.py
+-rw-r--r--   0        0        0     7373 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/fitness/base_score.py
+-rw-r--r--   0        0        0     1720 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/fitness/external_scores.py
+-rw-r--r--   0        0        0     2924 2023-07-05 13:01:19.931029 autotm-0.2.0/autotm/fitness/tasks.py
+-rw-r--r--   0        0        0    32442 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/fitness/tm.py
+-rw-r--r--   0        0        0     6237 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/infer.py
+-rw-r--r--   0        0        0     5299 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/main.py
+-rwxr-xr-x   0        0        0     1351 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/make-recovery-file.py
+-rw-r--r--   0        0        0     6857 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/params_logging_utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/preprocessing/__init__.py
+-rw-r--r--   0        0        0    13168 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/preprocessing/dictionaries_preparation.py
+-rw-r--r--   0        0        0     5034 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/preprocessing/text_preprocessing.py
+-rw-r--r--   0        0        0     2618 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/schemas.py
+-rw-r--r--   0        0        0     4892 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/utils.py
+-rw-r--r--   0        0        0        0 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/visualization/__init__.py
+-rw-r--r--   0        0        0     9985 2023-07-05 13:01:19.935029 autotm-0.2.0/autotm/visualization/dynamic_tracker.py
+-rw-r--r--   0        0        0     1054 2023-07-06 15:30:44.794646 autotm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 autotm-0.2.0/PKG-INFO
```

### Comparing `autotm-0.1.0/LICENSE` & `autotm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autotm-0.1.0/README.md` & `autotm-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+
+<img align="left" src="docs/img/MyLogo.png" alt="Library scheme" height="200"/>
+
 # AutoTM
 
-[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 ![build](https://github.com/ngc436/AutoTM/actions/workflows/build.yaml/badge.svg)
-[![GitHub Repo stars](https://img.shields.io/github/stars/ngc436/AutoTM?style=social)](https://github.com/ngc436/AutoTM/stargazers)
-
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version](https://badge.fury.io/py/autotm.svg)](https://badge.fury.io/py/autotm)
+[![Documentation Status](https://readthedocs.org/projects/autotm/badge/?version=latest)](https://autotm.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://static.pepy.tech/personalized-badge/autotm?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/autotm)
 Automatic parameters selection for topic models (ARTM approach) using evolutionary algorithms. 
 AutoTM provides necessary tools to preprocess english and russian text datasets and tune topic models.
 
 ## What is AutoTM?
 Topic modeling is one of the basic methods for EDA of unlabelled text data. While ARTM (additive regularization 
 for topic models) approach provides the significant flexibility and quality comparative or better that neural 
 approaches it is hard to tune such models due to amount of hyperparameters and their combinations.
@@ -23,29 +28,39 @@
 <img src="docs/img/img_library_eng.png" alt="Library scheme" height=""/>
 
 
 ## Installation
 
 ! Note: The functionality of topic models training is available only for linux distributions.
 
+Via pip:
+
+```pip install autotm```
+
+From source:
+
 ```pip install -r requirements.txt```  
 
 ```python -m spacy download en_core_web_sm```
 
 ```export PYTHONPATH="${PYTHONPATH}:/path/to/src"```
 
 [//]: # (## Dataset and )
 
 ## Quickstart
 
 The notebook with an example is available in ```examples``` folder.
 
-## Distributed version
+## Running from the command line
+
+To fit a model:
+```autotmctl --verbose fit --config conf/config.yaml --in data/sample_corpora/sample_dataset_lenta.csv```
 
-Distributed version to run experiments on kubernetes is available in ```autotm-distributed``` brunch. Still this version is in development stage and will be transfered to separate repository.
+To predict with a fitted model:
+```autotmctl predict --in data/sample_corpora/sample_dataset_lenta.csv --model model.artm```
 
 ## Backlog:
 - [ ] Add tests
 - [ ] Add new multi-stage 
  
 ## Citation
```

### Comparing `autotm-0.1.0/pyproject.toml` & `autotm-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 [tool.poetry]
 name = "autotm"
-version = "0.1.0"
+version = "0.2.0"
 description = "Automatic hyperparameters tuning for topic models (ARTM approach) using evolutionary algorithms"
 authors = [
     "Khodorchenko Maria <mariyaxod@yandex.ru>",
     "Nikolay Butakov alipoov.nb@gmail.com"
 ]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://autotm.readthedocs.io/en/latest/"
 repository = "https://github.com/ngc436/AutoTM"
 packages = [
-    {include = "src/autotm"}
+    {include = "autotm"}
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.10"
 bigartm = "0.9.2"
+protobuf = "<=3.20.0"
 tqdm = "*"
 numpy = "*"
 PyYAML = "*"
-#Jinja2 = "3.1.2"
 dataclasses-json = "*"
 mlflow = "*"
 click = "*"
-#pymysql = "0.9.3"
-#psycopg2-binary = "2.8.5"
 pymongo = "*"
 scikit-learn = "*"
 scipy = "*"
 hyperopt = "*"
-#navec = "0.10.0"
-#seaborn = "0.11.0"
 pymystem3 = "*"
 nltk = "*"
 plotly = "*"
-spacy = "*"
+spacy = ">=3.5"
 spacy-langdetect = "*"
 gensim = "*"
 pandas = "*"
 billiard = "*"
 pydantic = "*"
-#protobuf = "3.20.*"
 dill = "*"
 pytest = "*"
-#SALib = "~=1.4.7"
-#deap = "~=1.3.3"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 sphinx = "*"
+flake8 = "*"
+
+[tool.poetry.scripts]
+autotmctl = 'autotm.main:cli'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/bayesian_optimization/bayes_opt.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/bayesian_optimization/bayes_opt.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 import copy
 import logging
 import os
 import random
 import sys
 import uuid
 import warnings
-from logging import config
 from multiprocessing.pool import AsyncResult
 from typing import List, Optional, Union
 
 import click
 import yaml
-import tqdm
 from hyperopt import STATUS_OK, fmin, hp, tpe
-from kube_fitness.tasks import IndividualDTO, TqdmToLogger
+from tqdm import tqdm
 from yaml import Loader
 
-from algorithms_for_tuning.utils import make_log_config_dict
+from autotm.algorithms_for_tuning.individuals import IndividualDTO
+from autotm.utils import TqdmToLogger, make_log_config_dict
 
 ALG_ID = "bo"
 
 SPACE = {
     "decor": hp.quniform("decor", 0, 1e5, 0.05),
     "n1": hp.quniform("n1", 0, 8, 1),
     "spb": hp.quniform("spb", 1e-3, 1e2, 0.05),
@@ -37,44 +36,51 @@
     "decor_2": hp.quniform("decor_2", 0, 1e5, 0.05),
 }
 
 warnings.filterwarnings("ignore")
 
 logger = logging.getLogger("BO")
 
+# TODO: refactor this part
 # getting config vars
 if "FITNESS_CONFIG_PATH" in os.environ:
     filepath = os.environ["FITNESS_CONFIG_PATH"]
+    with open(filepath, "r") as file:
+        config = yaml.load(file, Loader=Loader)
 else:
-    filepath = "../../algorithms_for_tuning/bo_algorithm/config.yaml"
-
-with open(filepath, "r") as file:
-    config = yaml.load(file, Loader=Loader)
-
-    def estimate_fitness(
-        population: List[IndividualDTO], _: bool = False, __: int = 2
-    ) -> List[IndividualDTO]:
-        results = []
-
-        tqdm_out = TqdmToLogger(logger, level=logging.INFO)
-        for p in tqdm(population, file=tqdm_out):
-            individual = copy.deepcopy(p)
-            individual.fitness_value = random.random()
-            results.append(individual)
-
-        return results
-
-    def log_best_solution(
-        individual: IndividualDTO,
-        wait_for_result_timeout: Optional[float] = None,
-        alg_args: Optional[str] = None,
-    ) -> Union[IndividualDTO, AsyncResult]:
-        ind = copy.deepcopy(individual)
-        ind.fitness_value = random.random()
-        return ind
+    config = {
+        "testMode": False,
+        "boAlgoParams": {
+            "numEvals": 100
+        }
+    }
+
+
+def estimate_fitness(
+    population: List[IndividualDTO], _: bool = False, __: int = 2
+) -> List[IndividualDTO]:
+    results = []
+
+    tqdm_out = TqdmToLogger(logger, level=logging.INFO)
+    for p in tqdm(population, file=tqdm_out):
+        individual = copy.deepcopy(p)
+        individual.fitness_value = random.random()
+        results.append(individual)
+
+    return results
+
+
+def log_best_solution(
+    individual: IndividualDTO,
+    wait_for_result_timeout: Optional[float] = None,
+    alg_args: Optional[str] = None,
+) -> Union[IndividualDTO, AsyncResult]:
+    ind = copy.deepcopy(individual)
+    ind.fitness_value = random.random()
+    return ind
 
 
 NUM_FITNESS_EVALUATIONS = config["boAlgoParams"]["numEvals"]
 
 
 class BigartmFitness:
     def __init__(self, dataset: str, exp_id: Optional[int] = None):
@@ -133,15 +139,14 @@
 )
 @click.option("--exp-id", required=True, type=int, help="mlflow experiment id")
 def run_algorithm(dataset, log_file, exp_id):
     run_uid = uuid.uuid4() if not config["testMode"] else None
     logging_config = make_log_config_dict(filename=log_file, uid=run_uid)
     logging.config.dictConfig(logging_config)
 
-    prepare_fitness_estimator()
     fitness = BigartmFitness(dataset, exp_id)
     best_params = fmin(
         fitness, SPACE, algo=tpe.suggest, max_evals=NUM_FITNESS_EVALUATIONS
     )
     best_solution = fitness.make_individ(**best_params)
     best_solution = log_best_solution(
         best_solution, wait_for_result_timeout=-1, alg_args=" ".join(sys.argv)
```

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/ga.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,63 +4,58 @@
 import math
 import operator
 import random
 import sys
 import time
 import uuid
 import warnings
-from os.path import abspath, exists
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
-import random
+from typing import Optional
 
 import numpy as np
-from sklearn.svm import SVR
 from sklearn.ensemble import BaggingRegressor
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import (
     RBF,
     Matern,
     WhiteKernel,
     ConstantKernel,
     ExpSineSquared,
     RationalQuadratic,
 )
 from sklearn.metrics import mean_squared_error
 from sklearn.neural_network import MLPRegressor
+from sklearn.svm import SVR
 from sklearn.tree import DecisionTreeRegressor
 
-from autotm.algorithms_for_tuning.genetic_algorithm.mutation import mutation
 from autotm.algorithms_for_tuning.genetic_algorithm.crossover import crossover
+from autotm.algorithms_for_tuning.genetic_algorithm.mutation import mutation
 from autotm.algorithms_for_tuning.genetic_algorithm.selection import selection
-from autotm.algorithms_for_tuning.individuals import make_individual, IndividualDTO
+from autotm.algorithms_for_tuning.individuals import make_individual, IndividualDTO, Individual
 from autotm.algorithms_for_tuning.nelder_mead_optimization.nelder_mead import (
     NelderMeadOptimization,
 )
-
+from autotm.fitness.tasks import estimate_fitness, log_best_solution
 from autotm.utils import AVG_COHERENCE_SCORE
-from scipy.optimize import minimize
 from autotm.visualization.dynamic_tracker import MetricsCollector
 
-from autotm.fitness.tasks import estimate_fitness, log_best_solution
-
 ALG_ID = "ga"
 SPEEDUP = True
 
 warnings.filterwarnings("ignore")
 logger = logging.getLogger("GA_algo")
 
 
 # TODO: Add fitness type
 def set_surrogate_fitness(value, fitness_type="avg_coherence_score"):
     npmis = {
-        f"npmi_50": None,
-        f"npmi_15": None,
-        f"npmi_25": None,
-        f"npmi_50_list": None,
+        "npmi_50": None,
+        "npmi_15": None,
+        "npmi_25": None,
+        "npmi_50_list": None,
     }
     scores_dict = {
         fitness_type: value,
         "perplexityScore": None,
         "backgroundTokensRatioScore": None,
         "contrast": None,
         "purity": None,
@@ -182,39 +177,39 @@
     def model_search(self, model):
         raise NotImplementedError
         # for model.components
 
 
 class GA:
     def __init__(
-            self,
-            dataset,
-            data_path,
-            num_individuals,
-            num_iterations,
-            mutation_type="mutation_one_param",
-            crossover_type="blend_crossover",
-            selection_type="fitness_prop",
-            elem_cross_prob=0.2,
-            num_fitness_evaluations: Optional[int] = 500,
-            early_stopping_iterations: Optional[int] = 500,
-            best_proc=0.3,
-            alpha=None,
-            exp_id: Optional[int] = None,
-            surrogate_name=None,
-            calc_scheme="type2",
-            topic_count: Optional[int] = None,
-            fitness_obj_type="single_objective",
-            tag: Optional[str] = None,
-            use_nelder_mead: bool = False,
-            use_nelder_mead_in_mutation: bool = False,
-            use_nelder_mead_in_crossover: bool = False,
-            use_nelder_mead_in_selector: bool = False,
-            train_option: str = "offline",
-            **kwargs,
+        self,
+        dataset,
+        data_path,
+        num_individuals,
+        num_iterations,
+        mutation_type="mutation_one_param",
+        crossover_type="blend_crossover",
+        selection_type="fitness_prop",
+        elem_cross_prob=0.2,
+        num_fitness_evaluations: Optional[int] = 500,
+        early_stopping_iterations: Optional[int] = 500,
+        best_proc=0.3,
+        alpha=None,
+        exp_id: Optional[int] = None,
+        surrogate_name=None,
+        calc_scheme="type2",
+        topic_count: Optional[int] = None,
+        fitness_obj_type="single_objective",
+        tag: Optional[str] = None,
+        use_nelder_mead: bool = False,
+        use_nelder_mead_in_mutation: bool = False,
+        use_nelder_mead_in_crossover: bool = False,
+        use_nelder_mead_in_selector: bool = False,
+        train_option: str = "offline",
+        **kwargs,
     ):
         """
 
         :param dataset: dataset name
         :param data_path: path to data
         :param num_individuals: number of individuals
         :param num_iterations: number of iterations
@@ -281,29 +276,29 @@
             dataset=self.dataset, n_specific_topics=topic_count
         )
         self.crossover_changes_dict = (
             {}
         )  # generation, parent_1_params, parent_2_params, ...
 
     def set_regularizer_limits(
-            self,
-            low_decor=0,
-            high_decor=1e5,
-            low_n=0,
-            high_n=30,
-            low_back=0,
-            high_back=5,
-            low_spb=0,
-            high_spb=1e2,
-            low_spm=-1e-3,
-            high_spm=1e2,
-            low_sp_phi=-1e3,
-            high_sp_phi=1e3,
-            low_prob=0,
-            high_prob=1,
+        self,
+        low_decor=0,
+        high_decor=1e5,
+        low_n=0,
+        high_n=30,
+        low_back=0,
+        high_back=5,
+        low_spb=0,
+        high_spb=1e2,
+        low_spm=-1e-3,
+        high_spm=1e2,
+        low_sp_phi=-1e3,
+        high_sp_phi=1e3,
+        low_prob=0,
+        high_prob=1,
     ):
         self.high_decor = high_decor
         self.low_decor = low_decor
         self.low_n = low_n
         self.high_n = high_n
         self.low_back = low_back
         self.high_back = high_back
@@ -682,15 +677,15 @@
         for point in starting_points_set:
             st_point = point[:12] + [point[15]]
             res = nelder_opt.run_algorithm(
                 num_iterations=num_iterations, ini_point=st_point
             )
             solution = list(res["x"])
             solution = (
-                    solution[:-1] + point[12:15] + [solution[-1]]
+                solution[:-1] + point[12:15] + [solution[-1]]
             )  # TODO: check mutation ids
             fitness = -res.fun
             solution_dto = IndividualDTO(
                 id=str(uuid.uuid4()),
                 data_path=self.data_path,
                 dataset=self.dataset,
                 params=solution,
@@ -702,15 +697,15 @@
                 fitness_value={AVG_COHERENCE_SCORE: fitness},
                 train_option=self.train_option,
             )
 
             new_population.append(make_individual(dto=solution_dto))
         return new_population
 
-    def run(self, verbose=False):
+    def run(self, verbose=False, visualize_results=False) -> Individual:
         self.evaluations_counter = 0
         ftime = str(int(time.time()))
 
         # os.makedirs(LOG_FILE_PATH, exist_ok=True)
 
         logger.info(f"Starting experiment: {ftime}")
 
@@ -753,15 +748,15 @@
             population.sort(key=operator.attrgetter("fitness_value"), reverse=True)
             pairs_generator = self.selection(
                 population=population,
                 best_proc=self.best_proc,
                 children_num=self.crossover_children,
             )
 
-            logger.info(f"PAIRS ARE CREATED")
+            logger.info("PAIRS ARE CREATED")
 
             # Crossover
             new_generation, crossover_changes = self.run_crossover(
                 pairs_generator, surrogate_iteration, iteration_num=ii
             )
 
             new_generation.sort(key=operator.attrgetter("fitness_value"), reverse=True)
@@ -769,18 +764,15 @@
 
             logger.info("CROSSOVER IS OVER")
 
             if self.use_nelder_mead_in_crossover:
                 # TODO: implement Nelder-Mead here
                 pass
 
-            if (
-                    self.num_fitness_evaluations
-                    and self.evaluations_counter >= self.num_fitness_evaluations
-            ):
+            if self.num_fitness_evaluations and self.evaluations_counter >= self.num_fitness_evaluations:
                 bparams = "".join([str(i) for i in population[0].params])
                 self.metric_collector.save_fitness(
                     generation=ii,
                     params=[i.params for i in population],
                     fitness=[i.fitness_value for i in population],
                 )
                 logger.info(
@@ -805,23 +797,22 @@
                 individ
                 for individ in new_generation
                 if individ.params != the_best_guy_params
             ]
 
             new_generation_n = min(
                 (
-                        self.num_individuals
-                        - int(np.ceil(self.num_individuals * self.best_proc))
+                    self.num_individuals - int(np.ceil(self.num_individuals * self.best_proc))
                 ),
                 len(new_generation),
             )
             old_generation_n = self.num_individuals - new_generation_n
 
             population = (
-                    population[:old_generation_n] + new_generation[:new_generation_n]
+                population[:old_generation_n] + new_generation[:new_generation_n]
             )
 
             try:
                 del new_generation
             except:
                 pass
 
@@ -941,18 +932,15 @@
                 for i, elem in enumerate(nm_population):
                     if population[i].fitness_value < elem.fitness_value:
                         print(
                             f"NM found better solution! {elem.fitness_value} vs {population[i].fitness_value}"
                         )
                         population[i] = elem
 
-            if (
-                    self.num_fitness_evaluations
-                    and self.evaluations_counter >= self.num_fitness_evaluations
-            ):
+            if self.num_fitness_evaluations and self.evaluations_counter >= self.num_fitness_evaluations:
                 self.metric_collector.save_fitness(
                     generation=ii,
                     params=[i.params for i in population],
                     fitness=[i.fitness_value for i in population],
                 )
                 bparams = "".join([str(i) for i in population[0].params])
                 logger.info(
@@ -1019,24 +1007,27 @@
                 f"DATASET {self.dataset}."
                 f"TOPICS NUM {self.topic_count}."
                 f"RUN ID {run_id}."
             )
             best_solution = population[0]
             log_best_solution(best_solution, alg_args=" ".join(sys.argv), is_tmp=True)
 
-        self.metric_collector.save_and_visualise_trace()
+        if visualize_results:
+            self.metric_collector.save_and_visualise_trace()
+        else:
+            self.metric_collector.save_trace()
 
         logger.info(f"Y: {y}")
         best_individual = population[0]
         ind = log_best_solution(best_individual, alg_args=" ".join(sys.argv))
         logger.info(
             f"Logged the best solution. Obtained fitness is {ind.fitness_value}"
         )
 
-        return ind.fitness_value
+        return ind
 
 
 # multistage bag of regularizers approach
 # TODO: add penalty for the solution length
 
 
 class GAmultistage(GA):
@@ -1055,27 +1046,27 @@
         self.initial_element_stage_probability = 0.5
         self.positioning_matrix = np.full(
             (len(self.bag_of_regularizers), self.max_stages - 1), 0.5
         )
         self.set_regularizer_limits()
 
     def set_regularizer_limits(
-            self,
-            low_decor=0,
-            high_decor=1e5,
-            low_n=1,
-            high_n=30,  # minimal value changed to 1
-            low_back=0,
-            high_back=5,
-            low_spb=0,
-            high_spb=1e2,
-            low_spm=-1e-3,
-            high_spm=1e2,
-            low_sp_phi=-1e3,
-            high_sp_phi=1e3,
+        self,
+        low_decor=0,
+        high_decor=1e5,
+        low_n=1,
+        high_n=30,  # minimal value changed to 1
+        low_back=0,
+        high_back=5,
+        low_spb=0,
+        high_spb=1e2,
+        low_spm=-1e-3,
+        high_spm=1e2,
+        low_sp_phi=-1e3,
+        high_sp_phi=1e3,
     ):
         self.high_decor = high_decor
         self.low_decor = low_decor
         self.low_n = low_n
         self.high_n = high_n
         self.low_back = low_back
         self.high_back = high_back
```

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/genetic_algorithm.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/genetic_algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #!/usr/bin/env python3
 import logging
 import sys
-from logging import config
+import uuid
 import warnings
-import yaml
-from yaml import Loader
 from typing import Union
 
-import uuid
-
 from autotm.algorithms_for_tuning.genetic_algorithm.ga import GA
+from autotm.fitness.tm import fit_tm, TopicModel
 from autotm.utils import make_log_config_dict
 
 warnings.filterwarnings("ignore")
 
-logger = logging.getLogger("GA")
+logger = logging.getLogger(__name__)
 
 NUM_FITNESS_EVALUATIONS = 150
 
 
 def run_algorithm(
     dataset: str,
     data_path: str,
@@ -39,15 +36,15 @@
     gpr_kernel: str = None,
     gpr_alpha: float = None,
     gpr_normalize_y: float = None,
     use_nelder_mead_in_mutation: bool = False,
     use_nelder_mead_in_crossover: bool = False,
     use_nelder_mead_in_selector: bool = False,
     train_option: str = "offline",
-):
+) -> TopicModel:
     """
 
     :param dataset: Dataset name that is being processed. The name will be used to store results
     :param data_path: Path to all the artifacts obtained after
     :param exp_id: Mlflow experiment id
     :param topic_count: desired count of SPECIFIC topics (in optimization process BACK topics are also produced, thus the total amount of topics can be more than topic_count)
     :param num_individuals: Number of individuals in generation
@@ -117,13 +114,18 @@
         gpr_alpha=gpr_alpha,
         normalize_y=gpr_normalize_y,
         use_nelder_mead_in_mutation=use_nelder_mead_in_mutation,
         use_nelder_mead_in_crossover=use_nelder_mead_in_crossover,
         use_nelder_mead_in_selector=use_nelder_mead_in_selector,
         train_option=train_option,
     )
-    best_value = g.run(verbose=True)
-    print(best_value * (-1))
+    best_individual = g.run(verbose=True)
+    logger.info(f"Best individual fitness_value: {best_individual.fitness_value * (-1)}")
 
+    best_topic_model = fit_tm(
+        preproc_data_path=data_path,
+        topic_count=topic_count,
+        params=best_individual.params,
+        train_option=train_option
+    )
 
-if __name__ == "__main__":
-    run_algorithm()
+    return best_topic_model
```

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/mutation.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/mutation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import random
 import numpy as np
+from typing import List
 
 
 def mutation_one_param(
-    individ,
-    low_spb,
-    high_spb,
-    low_spm,
-    high_spm,
-    low_n,
-    high_n,
-    low_back,
-    high_back,
-    low_decor,
-    high_decor,
-    elem_mutation_prob=0.1,
+        individ: List[float],
+        low_spb: float,
+        high_spb: float,
+        low_spm: float,
+        high_spm: float,
+        low_n: int,
+        high_n: int,
+        low_back: float,
+        high_back: float,
+        low_decor: float,
+        high_decor: float,
+        elem_mutation_prob: float = 0.1,
 ):
     for i in range(len(individ)):
         if random.random() <= elem_mutation_prob:
             if i in [2, 3]:
                 individ[i] = np.random.uniform(low=low_spb, high=high_spb, size=1)[0]
             for i in [5, 6, 8, 9]:
                 individ[i] = np.random.uniform(low=low_spm, high=high_spm, size=1)[0]
```

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/selection.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/selection.py`

 * *Files identical despite different names*

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/genetic_algorithm/strategy.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/genetic_algorithm/strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # strategies of automatic EA configuration
 
 # CMA-ES (Covariance Matrix Adaptation Evolution Strategy)
 
+from math import sqrt, log
+
 # code source: https://github.com/DEAP/deap/blob/master/deap/cma.py
 import numpy
-from math import sqrt, log, exp
 
 
 class Strategy(object):
     def __init__(self, centroid, sigma, **kwargs):
         self.params = kwargs
 
         # Create a centroid as a numpy array
@@ -52,15 +53,15 @@
         *population*.
         :param population: A list of individuals from which to update the
                            parameters.
         """
         population.sort(key=lambda ind: ind.fitness, reverse=True)
 
         old_centroid = self.centroid
-        self.centroid = numpy.dot(self.weights, population[0 : self.mu])
+        self.centroid = numpy.dot(self.weights, population[0: self.mu])
 
         c_diff = self.centroid - old_centroid
 
         # Cumulation : update evolution path
         self.ps = (1 - self.cs) * self.ps + sqrt(
             self.cs * (2 - self.cs) * self.mueff
         ) / self.sigma * numpy.dot(
@@ -79,15 +80,15 @@
         self.update_count += 1
 
         self.pc = (1 - self.cc) * self.pc + hsig * sqrt(
             self.cc * (2 - self.cc) * self.mueff
         ) / self.sigma * c_diff
 
         # Update covariance matrix
-        artmp = population[0 : self.mu] - old_centroid
+        artmp = population[0: self.mu] - old_centroid
         self.C = (
             (
                 1
                 - self.ccov1
                 - self.ccovmu
                 + (1 - hsig) * self.ccov1 * self.cc * (2 - self.cc)
             )
@@ -129,18 +130,14 @@
         self.mueff = 1.0 / sum(self.weights**2)
 
         self.cc = params.get("ccum", 4.0 / (self.dim + 4.0))
         self.cs = params.get("cs", (self.mueff + 2.0) / (self.dim + self.mueff + 3.0))
         self.ccov1 = params.get("ccov1", 2.0 / ((self.dim + 1.3) ** 2 + self.mueff))
         self.ccovmu = params.get(
             "ccovmu",
-            2.0
-            * (self.mueff - 2.0 + 1.0 / self.mueff)
-            / ((self.dim + 2.0) ** 2 + self.mueff),
+            2.0 * (self.mueff - 2.0 + 1.0 / self.mueff) / ((self.dim + 2.0) ** 2 + self.mueff),
         )
         self.ccovmu = min(1 - self.ccov1, self.ccovmu)
         self.damps = (
-            1.0
-            + 2.0 * max(0, sqrt((self.mueff - 1.0) / (self.dim + 1.0)) - 1.0)
-            + self.cs
+            1.0 + 2.0 * max(0.0, sqrt((self.mueff - 1.0) / (self.dim + 1.0)) - 1.0) + self.cs
         )
         self.damps = params.get("damps", self.damps)
```

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/individuals.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/individuals.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,18 @@
         y = np.array(y)
         return np.mean(y, axis=0)
 
 
 class LearnedScorerFitnessIndividual(BaseIndividual):
     @property
     def fitness_value(self) -> float:
-        dataset_name = self.dto.dataset  # TODO: check namings
-        m = LearnedModel(save_path=PATH_TO_LEARNED_SCORING, dataset_name=dataset_name)
+        # dataset_name = self.dto.dataset  # TODO: check namings
+        # m = LearnedModel(save_path=PATH_TO_LEARNED_SCORING, dataset_name=dataset_name)
         # TODO: predict from metrics df
+        raise NotImplementedError()
 
 
 class SparsityScalerBasedFitnessIndividual(BaseIndividual):
     @property
     def fitness_value(self) -> float:
         # it is a handling of the situation when a fitness-worker wasn't able to correctly calculate this indvidual
         # due to some error in the proceess
```

### Comparing `autotm-0.1.0/src/autotm/algorithms_for_tuning/nelder_mead_optimization/nelder_mead.py` & `autotm-0.2.0/autotm/algorithms_for_tuning/nelder_mead_optimization/nelder_mead.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import numpy as np
 from scipy.optimize import minimize
-from typing import Union
+
 from autotm.fitness.tm import FitnessCalculatorWrapper
-import numpy as np
 
 
 class NelderMeadOptimization:
     def __init__(
         self,
         dataset,
         data_path,
```

### Comparing `autotm-0.1.0/src/autotm/batch_vect_utils.py` & `autotm-0.2.0/autotm/batch_vect_utils.py`

 * *Files identical despite different names*

### Comparing `autotm-0.1.0/src/autotm/data_generator/synthetic_data_generation.ipynb` & `autotm-0.2.0/autotm/data_generator/synthetic_data_generation.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964583333333333%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'def data_generator(\\n'), (1, '    "*

 * *            "vocab_size=10000,\\n'), (2, '    num_documents=5000,\\n'), (3, '    "*

 * *            "mean_text_len=15,\\n'), (4, '    std_text_len=5,\\n'), (5, '    topics_num=10,\\n'), "*

 * *            '(6, \'    distribution="dirichlet",\\n\'), (7, \'):\\n\'), (11, \'        doc_len = '*

 * *            "int(np.random.normal(loc=mean_text_len, scale=std_text_len))')], delete: [10, 9, 5, "*

 * *            '4, 3, 2, 1, 0]}}}'}*

```diff
@@ -15,25 +15,26 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
             },
             "outputs": [],
             "source": [
-                "def data_generator(vocab_size=10000,\n",
-                "                   num_documents=5000,\n",
-                "                   mean_text_len=15,\n",
-                "                   std_text_len=5,\n",
-                "                   topics_num=10,\n",
-                "                   distribution='dirichlet'):\n",
+                "def data_generator(\n",
+                "    vocab_size=10000,\n",
+                "    num_documents=5000,\n",
+                "    mean_text_len=15,\n",
+                "    std_text_len=5,\n",
+                "    topics_num=10,\n",
+                "    distribution=\"dirichlet\",\n",
+                "):\n",
                 "    vocabulary = [i for i in range(vocab_size)]\n",
                 "\n",
                 "    for doc in num_documents:\n",
-                "        doc_len = int(np.random.normal(loc=mean_text_len, scale=std_text_len))\n",
-                "        "
+                "        doc_len = int(np.random.normal(loc=mean_text_len, scale=std_text_len))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false
```

### Comparing `autotm-0.1.0/src/autotm/fitness/base_score.py` & `autotm-0.2.0/autotm/fitness/base_score.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import (
     Any,
     Callable,
     Dict,
 )
 
-from autotm.fitness import scores as tn_scores
+# from autotm.fitness import scores as tn_scores
 
 
 class BaseScore:
     """
     Base Class to construct custom score functions.
     """
 
@@ -79,16 +79,16 @@
             )
         else:
             pass
 
         self._should_compute = should_compute
         self.value = []
 
-        if not hasattr(tn_scores, self.__class__.__name__):
-            setattr(tn_scores, self.__class__.__name__, self.__class__)
+        # if not hasattr(tn_scores, self.__class__.__name__):
+        #     setattr(tn_scores, self.__class__.__name__, self.__class__)
 
     @staticmethod
     def compute_always(fit_iteration: int) -> bool:
         return True
 
     @staticmethod
     def compute_on_last(fit_iteration: int) -> bool:
```

### Comparing `autotm-0.1.0/src/autotm/fitness/external_scores.py` & `autotm-0.2.0/autotm/fitness/external_scores.py`

 * *Files identical despite different names*

### Comparing `autotm-0.1.0/src/autotm/fitness/tasks.py` & `autotm-0.2.0/autotm/fitness/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from autotm.schemas import IndividualDTO, fitness_to_json, fitness_from_json
 from autotm.algorithms_for_tuning.individuals import make_individual
 
 logger = logging.getLogger("root")
 
 
 def do_fitness_calculating(
-        individual: str,
-        log_artifact_and_parameters: bool = False,
-        log_run_stats: bool = False,
-        alg_args: Optional[str] = None,
-        is_tmp: bool = False,
+    individual: str,
+    log_artifact_and_parameters: bool = False,
+    log_run_stats: bool = False,
+    alg_args: Optional[str] = None,
+    is_tmp: bool = False,
 ) -> str:
     individual: IndividualDTO = IndividualDTO.parse_raw(individual)
 
     with fit_tm_of_individual(
-            dataset=individual.dataset,
-            data_path=individual.data_path,
-            params=individual.params,
-            fitness_name=individual.fitness_name,
-            topic_count=individual.topic_count,
-            force_dataset_settings_checkout=individual.force_dataset_settings_checkout,
-            train_option=individual.train_option,
+        dataset=individual.dataset,
+        data_path=individual.data_path,
+        params=individual.params,
+        fitness_name=individual.fitness_name,
+        topic_count=individual.topic_count,
+        force_dataset_settings_checkout=individual.force_dataset_settings_checkout,
+        train_option=individual.train_option,
     ) as (time_metrics, metrics, tm):
         individual.fitness_value = metrics
 
         with model_files(tm) as tm_files:
             if log_artifact_and_parameters:
                 log_params_and_artifacts(
                     tm, tm_files, individual, time_metrics, alg_args, is_tmp=is_tmp
@@ -38,27 +38,27 @@
             if log_run_stats:
                 log_stats(tm, tm_files, individual, time_metrics, alg_args)
 
     return individual.json()
 
 
 def calculate_fitness(
-        individual: str,
-        log_artifact_and_parameters: bool = False,
-        log_run_stats: bool = False,
-        alg_args: Optional[str] = None,
-        is_tmp: bool = False
+    individual: str,
+    log_artifact_and_parameters: bool = False,
+    log_run_stats: bool = False,
+    alg_args: Optional[str] = None,
+    is_tmp: bool = False,
 ) -> str:
     try:
         return do_fitness_calculating(
-            individual, log_artifact_and_parameters, log_run_stats, is_tmp
+            individual, log_artifact_and_parameters, log_run_stats, alg_args, is_tmp
         )
     except Exception as e:
         print(str(e))
-        raise Exception(f"Some exception")
+        raise Exception("Some exception")
 
 
 def estimate_fitness(population: List[IndividualDTO]) -> List[IndividualDTO]:
     logger.info("Calculating fitness...")
     population_with_fitness = []
     for individual in population:
         json_individ = fitness_to_json(individual.dto)
@@ -67,23 +67,25 @@
             make_individual(fitness_from_json(individ_with_fitness))
         )
     logger.info("The fitness results have been obtained")
     return population_with_fitness
 
 
 def log_best_solution(
-        individual: IndividualDTO,
-        wait_for_result_timeout: Optional[float] = None,
-        alg_args: Optional[str] = None,
-        is_tmp: bool = False,
+    individual: IndividualDTO,
+    wait_for_result_timeout: Optional[float] = None,
+    alg_args: Optional[str] = None,
+    is_tmp: bool = False,
 ):
-    logger.info(f"Sending a best individual to be logged")
+    logger.info("Sending a best individual to be logged")
     res = make_individual(
         fitness_from_json(
             calculate_fitness(
-                fitness_to_json(individual.dto), log_artifact_and_parameters=True, is_tmp=is_tmp
+                fitness_to_json(individual.dto),
+                log_artifact_and_parameters=True,
+                is_tmp=is_tmp,
             )
         )
     )
 
     # TODO: write logging
     return res
```

### Comparing `autotm-0.1.0/src/autotm/fitness/tm.py` & `autotm-0.2.0/autotm/fitness/tm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,57 @@
 import logging
+import multiprocessing
+import multiprocessing as mp
 import os
 import pickle
 import time
 import uuid
 from collections import OrderedDict
 from contextlib import contextmanager
 from typing import Dict, Optional, Tuple, ContextManager, List
-import multiprocessing as mp
 
 import artm
 import gensim.corpora as corpora
 import numpy as np
 import pandas as pd
 from billiard.exceptions import SoftTimeLimitExceeded
-from gensim.models.coherencemodel import CoherenceModel
 from tqdm import tqdm
 
+from autotm.batch_vect_utils import SampleBatchVectorizer
 from autotm.fitness.external_scores import ts_bground, ts_uniform, ts_vacuous, switchp
 from autotm.utils import (
     MetricsScores,
     AVG_COHERENCE_SCORE,
     TimeMeasurements,
     log_exec_timer,
 )
-from autotm.batch_vect_utils import SampleBatchVectorizer
 
 logger = logging.getLogger()
 logging.basicConfig(level="INFO")
 
 
+def extract_topics(model: artm.ARTM):
+    if "TopTokensScore" not in model.score_tracker:
+        logger.warning(
+            "Key 'TopTokensScore' is not presented in the model's score_tracker. "
+            "Returning empty dict of topics."
+        )
+        return dict()
+    res = model.score_tracker["TopTokensScore"].last_tokens
+    topics = {topic: tokens[:50] for topic, tokens in res.items()}
+    return topics
+
+
+def print_topics(model: artm.ARTM):
+    for i, (topic, top_tokens) in enumerate(extract_topics(model).items()):
+        print(topic)
+        print(top_tokens)
+        print()
+
+
 class Dataset:
     _batches_path: str = "batches"
     _wv_path: str = "test_set_data_voc.txt"
     _cooc_dict_path: str = "cooc_dictionary.txt"
     _dictionary_path: str = "dictionary.txt"
     _vocab_path: str = "vocab.txt"
     _cooc_file_df_path: str = "cooc_df.txt"
@@ -231,15 +250,14 @@
         if self.fitness_name == "default":
             logging.info(
                 f"Using TM model: {TopicModel} according "
                 f"to fitness name: {self.fitness_name}, topics count: {self.topic_count}"
             )
             self.tm = TopicModel(
                 uid,
-                self.experiments_path,
                 self.topic_count,
                 self.num_processors,
                 dataset,
                 self.params,
                 train_option=self.train_option,
             )
         else:
@@ -356,41 +374,34 @@
     return fitness
 
 
 class TopicModel:
     def __init__(
         self,
         uid: uuid.UUID,
-        experiments_path: str,
         topic_count: int,
         num_processors: int,
         dataset: Dataset,
         params: list,
         decor_test=False,
         train_option: str = "offline",
     ):
         self.uid = uid
-        self.experiments_path: str = experiments_path
         self.topic_count: int = topic_count
         self.num_processors: int = num_processors
         self.dataset = dataset
         self.train_option = train_option
 
         self.model = None
         self.S = self.topic_count
         self.specific = ["main{}".format(i) for i in range(self.S)]
-
-        self.save_path = os.path.join(self.experiments_path, "best_model")
         self.decor_test = decor_test
 
-        if not os.path.exists(self.save_path):
-            os.makedirs(self.save_path)
-
         self.__set_params(params)
-        self.back = ["back{}".format(i) for i in range(self.B)]
+        self.back = ["back{}".format(i) for i in range(int(self.B))]
 
     def init_model(self):
         self.model = artm.ARTM(
             num_topics=self.S + self.B,
             class_ids=["@default_class"],
             dictionary=self.dataset.dictionary,
             show_progress_bars=False,
@@ -544,36 +555,22 @@
 
         self.model.regularizers.add(
             artm.DecorrelatorPhiRegularizer(
                 name="decorr", topic_names=self.specific, tau=self.decor
             )
         )
 
-    def dump_model(self, ii):
-        self.model.dump_artm_model(os.path.join(self.save_path, "model_{}".format(ii)))
-
     def save_model(self, path):
         self.model.dump_artm_model(path)
 
     def print_topics(self):
-        for i, (topic, top_tokens) in enumerate(self.get_topics().items()):
-            print(topic)
-            print(top_tokens)
-            print()
+        print_topics(self.model)
 
     def get_topics(self):
-        if "TopTokensScore" not in self.model.score_tracker:
-            logger.warning(
-                f"Key 'TopTokensScore' is not presented in the model's (uid={self.uid}) score_tracker. "
-                f"Returning empty dict of topics."
-            )
-            return dict()
-        res = self.model.score_tracker["TopTokensScore"].last_tokens
-        topics = {topic: tokens[:50] for topic, tokens in res.items()}
-        return topics
+        return extract_topics(self.model)
 
     def _get_avg_coherence_score(self, for_individ_fitness=False):
         coherences_main, coherences_back = self.__return_all_tokens_coherence(
             self.model, s=self.S, b=self.B
         )
         if for_individ_fitness:
             # print('COMPONENTS: ', np.mean(list(coherences_main.values())), np.min(list(coherences_main.values())))
@@ -685,15 +682,15 @@
             )
         )
 
     def __calculate_topic_coherence(self, tokens, top=50):
         tokens = tokens[:top]
         total_sum = 0
         for ix, token_1 in enumerate(tokens[:-1]):
-            for ij, token_2 in enumerate(tokens[(ix + 1) :]):
+            for ij, token_2 in enumerate(tokens[(ix + 1):]):
                 try:
                     total_sum += self.dataset.mutual_info_dict[
                         "{}_{}".format(token_1, token_2)
                     ]
                 except KeyError:
                     total_sum += 0
 
@@ -780,16 +777,15 @@
         if for_individ_fitness:
             print(
                 "COMPONENTS: ",
                 np.mean(list(coherences_main.values())),
                 np.min(list(coherences_main.values())),
             )
             avg_coherence_score = (
-                np.mean(list(coherences_main.values()))
-                + np.min(list(coherences_main.values())) * coeff
+                np.mean(list(coherences_main.values())) + np.min(list(coherences_main.values())) * coeff
             )
         else:
             avg_coherence_score = np.mean(list(coherences_main.values())) * coeff
 
         return {AVG_COHERENCE_SCORE: avg_coherence_score}
 
     # TODO: fix
@@ -865,18 +861,18 @@
                     (f"npmi_{num_tokens}", np.mean(npmi_list) if npmi_list else None),
                     (f"npmi_{num_tokens}_list", npmi_list),
                 ]
             }
 
         else:
             npmis = {
-                f"npmi_50": None,
-                f"npmi_15": None,
-                f"npmi_25": None,
-                f"npmi_50_list": None,
+                "npmi_50": None,
+                "npmi_15": None,
+                "npmi_25": None,
+                "npmi_50_list": None,
             }
 
         if calculate_switchp:
             logger.info("Calculating switchp")
 
             if texts:
                 switchp_scores = switchp(self.model.get_phi(), texts)
@@ -931,7 +927,29 @@
             "switchP": np.nanmean(switchp_scores),
             "all_topics": all_topics_flag,
             **coherence_scores,
             **npmis,
         }
 
         return scores_dict
+
+
+def fit_tm(preproc_data_path: str, topic_count: int, params: list, train_option: str) -> TopicModel:
+    with log_exec_timer("Loading dataset: "):
+        dataset = Dataset(base_path=preproc_data_path, topic_count=topic_count)
+        dataset.load_dataset()
+
+    tm = TopicModel(
+        uuid.uuid4(),
+        topic_count,
+        num_processors=multiprocessing.cpu_count(),
+        dataset=dataset,
+        params=type_check(params),
+        train_option=train_option,
+    )
+
+    tm.init_model()
+
+    with log_exec_timer("TM Training"):
+        tm.train()
+
+    return tm
```

### Comparing `autotm-0.1.0/src/autotm/infer.py` & `autotm-0.2.0/autotm/infer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+import logging
 import os
+from typing import Union
+
 import yaml
 import json
 
 import pandas as pd
 import artm
 from autotm.preprocessing.dictionaries_preparation import prepare_batch_vectorizer
 
 PATH_TO_RUN_NAME = "tags/mlflow.runName"
 PATH_TO_EXPERIMENT_ID = ""
 
 PROCESSED_TEXT_COL = "processed_text"
 TOP_TOPICS_COL = "SER_top_topics"
 
+logger = logging.getLogger(__name__)
+
 
 def get_experiment_path(
-        exp_id: int, run_name: str, mlflow_path: str = "./mlruns/"
+    exp_id: int, run_name: str, mlflow_path: str = "./mlruns/"
 ) -> str:
     """
 
     :param mlflow_path: path where mlflow stores the results default is
     :param exp_id: id of the experiment, which artifacts is needed
     :param run_name: name of the mlflow run
     :return: path to the experiment artifacts
@@ -29,17 +34,17 @@
             if len(subfolders) > 1:
                 with open(os.path.join(mlflow_path, folder, "meta.yaml"), "r") as f:
                     data = yaml.load(f, Loader=yaml.Loader)
                 if data["name"] == f"experiment_{exp_id}":
                     for subfolder in subfolders:
                         if subfolder != "meta.yaml":
                             with open(
-                                    os.path.join(
-                                        mlflow_path, folder, subfolder, PATH_TO_RUN_NAME
-                                    )
+                                os.path.join(
+                                    mlflow_path, folder, subfolder, PATH_TO_RUN_NAME
+                                )
                             ) as f:
                                 f_run_name = f.read()
                                 if f_run_name.strip() == run_name:
                                     return os.path.join(
                                         mlflow_path, folder, subfolder, "artifacts"
                                     )
     return None
@@ -65,27 +70,27 @@
     if "Unnamed: 0" in list(df):
         df = df.set_index("Unnamed: 0")
         df = df.T
     return df
 
 
 def get_most_probable_topics_from_theta(
-        df: pd.DataFrame, theta_df: pd.DataFrame, top_n: int = 2
+    df: pd.DataFrame, theta_df: pd.DataFrame, top_n: int = 2
 ) -> pd.DataFrame:
     """
 
     :param df: processed dataset which is produced by prepare_all function
     :param theta_df: theta matrix of trained model
     :param top_n: amount of top topics to consider
     :return: pd.Dataframe with 'top_topics' column
     """
     theta_df = _transform_matrix(theta_df)
     print(theta_df)
     assert (
-            df.shape[0] == theta_df.shape[0]
+        df.shape[0] == theta_df.shape[0]
     ), "Shapes of f and theta matrix are different"
     print(theta_df.apply(lambda x: ", ".join(x.nlargest(top_n).index.tolist()), axis=1))
     df[TOP_TOPICS_COL] = theta_df.apply(
         lambda x: ", ".join(x.nlargest(top_n).index.tolist()), axis=1
     ).tolist()
     return df
 
@@ -100,87 +105,79 @@
         top_topics_names = [i.strip() for i in row[TOP_TOPICS_COL].split(",")]
         for topic in top_topics_names:
             words = set(row[PROCESSED_TEXT_COL].split()).intersection(
                 set(topics[topic])
             )
             if len(words) > 1:
                 topic_tokens[topic] = [word for word in topics[topic] if word in words][
-                                      :top_w
-                                      ]
+                    :top_w
+                ]
         all_dicts.append(topic_tokens)
     df["SER_words_of_topic"] = all_dicts
     return df
 
 
 def get_most_probable_words_from_phi(df, phi_df):
     raise NotImplementedError
 
 
 class TopicsExtractor:
-    def __init__(self, model_path):
-        self.__tm_model_path = model_path
-        self.model = self.__load_model()
+    def __init__(self, model: Union[str, artm.ARTM]):
+        if isinstance(model, str):
+            self.__tm_model_path = model
+            self.model = self.__load_model()
+        else:
+            self.__tm_model_path = None
+            self.model = model
         self.__tmp_batches_path = "./tmp/tmp_batches/"
         self.__tmp_dict_path = "./tmp/tmp_dict/"
         self.topics_dict = self.model.score_tracker["TopTokensScore"].last_tokens
 
     def info(self):
         pass
 
     def return_topics(self):
         pass
 
     def __load_model(self):
         return artm.load_artm_model(self.__tm_model_path)
 
     def get_prob_mixture(
-            self,
-            data_path,
-            TMP_BATCHES_PATH="./tmp/tmp_batches/",
-            TMP_DICT_PATH="./tmp/tmp_dict/",
-            OUTPUT_DIR="./out",
-            text_column_name="processed_text",
-            input_format="csv",
-            top_n=2,
-    ):
-        try:
-            os.makedirs(TMP_BATCHES_PATH)
-            os.makedirs(TMP_DICT_PATH)
-        except:
-            print("folders already exist")
-
-        for tmp_batch in os.listdir(TMP_BATCHES_PATH):
-            os.remove(os.path.join(TMP_BATCHES_PATH, tmp_batch))
-
-        if input_format == "csv":
-            posts = pd.read_csv(data_path)
-        else:
-            posts = pd.read_parquet(data_path)
-
-        posts = posts[~posts[text_column_name].isna()]
-        posts = posts.reset_index(drop=True)
-
-        texts = posts[text_column_name].tolist()
+        self,
+        dataset: pd.DataFrame,
+        working_dir: str,
+        text_column_name="processed_text",
+        top_n=2,
+    ) -> pd.DataFrame:
+        tmp_batch_dir = os.path.join(working_dir, "tmp_batch_dir")
+        tmp_vw_path = os.path.join(working_dir, "tmp_wv.txt")
+
+        assert not os.path.exists(tmp_batch_dir), "Tmp batch should not exist beforehand"
+        assert not os.path.exists(tmp_vw_path), "Tmp vw filw should not exist beforehand"
+
+        os.makedirs(tmp_batch_dir)
+
+        dataset = dataset[~dataset[text_column_name].isna()]
+        dataset = dataset.reset_index(drop=True)
+        texts = dataset[text_column_name].tolist()
 
-        print("LEN {}".format(len(texts)))
+        logger.info("LEN {}".format(len(texts)))
 
         batch_vectorizer_test = prepare_batch_vectorizer(
-            batches_dir=TMP_DICT_PATH,
-            vw_path="./tmp/tmp_wv.txt",
-            data_path=data_path,
+            batches_dir=tmp_batch_dir,
+            vw_path=tmp_vw_path,
+            dataset=dataset,
             column_name=text_column_name,
         )
 
         theta_test = self.model.transform(batch_vectorizer=batch_vectorizer_test)
+
         theta_test_trans = theta_test.T
-        main_topics = [i for i in list(theta_test_trans) if i.startswith("main")]
-        theta_test_trans["top_topics"] = (
-            theta_test_trans[main_topics]
-            .apply(lambda x: ", ".join(x.nlargest(top_n).index.tolist()), axis=1)
-            .tolist()
-        )
-        theta_test_trans = theta_test_trans.join(posts[[text_column_name]])
-        theta_test_trans.to_csv(
-            os.path.join(OUTPUT_DIR, "data_with_theta.csv"), index=None
-        )
+        # main_topics = [i for i in list(theta_test_trans) if i.startswith("main")]
+        # theta_test_trans["top_topics"] = (
+        #     theta_test_trans[main_topics]
+        #     .apply(lambda x: ", ".join(x.nlargest(top_n).index.tolist()), axis=1)
+        #     .tolist()
+        # )
+        # theta_test_trans = theta_test_trans.join(dataset[[text_column_name]])
 
-        print("All is saved to {} !".format(OUTPUT_DIR))
+        return theta_test_trans
```

### Comparing `autotm-0.1.0/src/autotm/make-recovery-file.py` & `autotm-0.2.0/autotm/make-recovery-file.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 logger = logging.getLogger()
 
 
 # example: irace-log-2021-07-19T21:48:00-2b5faba3-99a8-47ba-a5cd-2c99e6877160.Rdata
 def fpath_to_datetime(fpath: str) -> datetime:
     fname = os.path.basename(fpath)
-    dt_str = fname[len("irace-log-") : len("irace-log-") + len("YYYY-mm-ddTHH:MM:ss")]
+    dt_str = fname[len("irace-log-"): len("irace-log-") + len("YYYY-mm-ddTHH:MM:ss")]
     dt = datetime.datetime.strptime(dt_str, "%Y-%m-%dT%H:%M:%S")
     return dt
 
 
 if __name__ == "__main__":
     save_dir = sys.argv[1]
     logger.info(f"Looking for data files in {save_dir}")
@@ -36,8 +36,8 @@
     last_data_filepath, _ = max(data_files, key=lambda x: x[1])
     recovery_filepath = os.path.join(save_dir, "recovery_rdata.checkpoint")
 
     logger.info(
         f"Copying last generated data file ({last_data_filepath}) as recovery file ({recovery_filepath})"
     )
     shutil.copy(last_data_filepath, recovery_filepath)
-    logger.info(f"Copying done")
+    logger.info("Copying done")
```

### Comparing `autotm-0.1.0/src/autotm/params_logging_utils.py` & `autotm-0.2.0/autotm/params_logging_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from typing import Optional, Tuple, List, cast, ContextManager, Dict
 
 import artm
 import gridfs
 import mlflow
 from pymongo import MongoClient
 
-from autotm.utils import TimeMeasurements
-from autotm.schemas import IndividualDTO, fitness_to_json
 from autotm.fitness.tm import TopicModel
-
+from autotm.schemas import IndividualDTO
+from autotm.utils import TimeMeasurements
 
 logger = logging.getLogger()
 
 
 @dataclass
 class TopicModelFiles:
     model_dir: str
@@ -71,17 +70,17 @@
 
 def make_readable_topics(tm: TopicModel) -> str:
     topics = tm.get_topics()
 
     def topic_seq_num(pair: Tuple[str, List[str]]) -> int:
         tname, _ = pair
         if tname.startswith("main"):
-            return int(tname[len("main") :])
+            return int(tname[len("main"):])
         if tname.startswith("back"):
-            return tm.topic_count + int(tname[len("back") :])
+            return tm.topic_count + int(tname[len("back"):])
         return -1
 
     ordered_topics = sorted(topics.items(), key=topic_seq_num)
     topics_reprs = [
         f"{topic}:{os.linesep}{os.linesep.join(' '.join(words[i:i + 10]) for i in range(0, len(words), 10))}"
         for topic, words in ordered_topics
     ]
@@ -91,21 +90,21 @@
 
 def log_params_and_artifacts(
     tm: TopicModel,
     tm_files: TopicModelFiles,
     individual: IndividualDTO,
     time_metrics: TimeMeasurements,
     alg_args: Optional[str],
-    is_tmp: bool = False
+    is_tmp: bool = False,
 ):
     logger.info("Logging params and artifacts to mlflow")
     logger.info(f"Created experiment_{individual.exp_id}")
     run_name = f"fitness-{individual.dataset}-{uuid.uuid4()}"
     if is_tmp:
-        run_name+=f'_tmp_{individual.iteration_id}'
+        run_name += f"_tmp_{individual.iteration_id}"
 
     try:
         experiment_id = mlflow.create_experiment(f"experiment_{individual.exp_id}")
     except:
         experiment = mlflow.get_experiment_by_name(f"experiment_{individual.exp_id}")
         experiment_id = experiment.experiment_id
         logger.info("Experiment exists, omitting creation")
```

### Comparing `autotm-0.1.0/src/autotm/preprocessing/dictionaries_preparation.py` & `autotm-0.2.0/autotm/preprocessing/dictionaries_preparation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import logging
 import os
-from typing import List
+from typing import List, Union
 
 import artm
 import math
 import pickle
 import pandas as pd
 import re
 from autotm.utils import parallelize_dataframe
 import itertools
 from collections import Counter
 
 RESERVED_TUPLE = ("_SERVICE_", "total_pairs_count")
 
+logger = logging.getLogger(__name__)
 
 # TODO: add inter-text coherence metrics (SemantiC, TopLen and FoCon)
 
 
 def get_words_dict(text, stop_list):
     all_words = text
     words = sorted(set(all_words) - stop_list)
@@ -49,15 +51,15 @@
     cooc_df_dict = {}  # format dict{(tuple): cooc}
     term_freq_dict = {}
     existing_vocab = set(vocab)
     for text in data:
         document_cooc_df_dict = {}
         splitted = [word for word in text.split() if word in existing_vocab]
         for i in range(0, len(splitted) - window):
-            for comb in itertools.combinations(splitted[i : i + window], 2):  # speed up
+            for comb in itertools.combinations(splitted[i: i + window], 2):  # speed up
                 comb = tuple(sorted(comb))  # adding comb sorting
                 if comb in document_cooc_df_dict:
                     continue
                 else:
                     document_cooc_df_dict[comb] = 1
                     term_freq_dict = _add_word_to_dict(comb[0], term_freq_dict)
                     term_freq_dict = _add_word_to_dict(comb[1], term_freq_dict)
@@ -69,28 +71,27 @@
     term_freq_dict = {}
     cooc_tf_dict = {RESERVED_TUPLE: 0}  # format dict{(tuple): cooc}
     existing_vocab = set(vocab)
     for text in data:
         document_cooc_tf_dict = {}
         splitted = [word for word in text.split() if word in existing_vocab]
         for i in range(0, len(splitted) - window):
-            for comb in itertools.combinations(splitted[i : i + window], 2):
+            for comb in itertools.combinations(splitted[i: i + window], 2):
                 if comb in document_cooc_tf_dict:
                     document_cooc_tf_dict[comb] += 1
                 else:
                     document_cooc_tf_dict[comb] = 1
 
                 term_freq_dict = _add_word_to_dict(comb[0], term_freq_dict)
                 term_freq_dict = _add_word_to_dict(comb[1], term_freq_dict)
                 cooc_tf_dict[RESERVED_TUPLE] += 2
         # cooc_tf_dict = dict(Counter(document_cooc_tf_dict) + Counter(cooc_tf_dict))
         counter = Counter(document_cooc_tf_dict)
         counter.update(cooc_tf_dict)
         cooc_tf_dict = dict(counter)
-        k = 0
     return cooc_tf_dict, term_freq_dict
     # local_num_of_pairs += 2
     # pass
 
 
 def calculate_ppmi(cooc_dict_path, n, term_freq_dict):
     print("Calculating pPMI...")
@@ -113,18 +114,28 @@
     :param df: dataframe with 'processed_text'  column
     :param window: The size of window to collect cooccurrences in
     :param n_cores: available cores for parallel processing. Default: -1 (all)
     :return: cooc_df and cooc_tf dictionaries
     """
     data = df["processed_text"].tolist()
     cooc_df_dict = parallelize_dataframe(
-        data, _calculate_cooc_df_dict, n_cores, return_type="dict", vocab=vocab, window=window
+        data,
+        _calculate_cooc_df_dict,
+        n_cores,
+        return_type="dict",
+        vocab=vocab,
+        window=window,
     )
     cooc_tf_dict = parallelize_dataframe(
-        data, _calculate_cooc_tf_dict, n_cores, return_type="dict", vocab=vocab, window=window
+        data,
+        _calculate_cooc_tf_dict,
+        n_cores,
+        return_type="dict",
+        vocab=vocab,
+        window=window,
     )
     return cooc_df_dict, cooc_tf_dict
 
 
 def write_vw_dict(res_dict, vocab_words, fpath):
     with open(fpath, "w") as fopen:
         for word in vocab_words:
@@ -141,19 +152,19 @@
         t_cooc_dict = cooc_dict[0]
     else:
         t_cooc_dict = cooc_dict
     data_dict = {}
     for item in sorted(t_cooc_dict.items(), key=lambda key: key[0]):
         if item == RESERVED_TUPLE:
             continue
-        word_1 = item[0][0]  # TODO: check this
-        word_2 = item[0][1]
-        if vocab_words.index(item[0][0]) > vocab_words.index(item[0][1]):
-            word_2 = item[0][0]
-            word_1 = item[0][1]
+        # word_1 = item[0][0]  # TODO: check this
+        # word_2 = item[0][1]
+        # if vocab_words.index(item[0][0]) > vocab_words.index(item[0][1]):
+        #     word_2 = item[0][0]
+        #     word_1 = item[0][1]
         if item[0][0] in data_dict:
             data_dict[item[0][0]].append(f"{item[0][1]}:{item[1]}")
         else:
             data_dict[item[0][0]] = [f"{item[0][1]}:{item[1]}"]
     write_vw_dict(data_dict, vocab_words, vw_path)
 
 
@@ -195,15 +206,17 @@
             if len(splitted_line) > 2:
                 raise Exception("There are more than 2 modalities!")
             vocab_words.append(splitted_line[0].strip())
 
     data = pd.read_csv(path_to_dataset)
     docs_count = data.shape[0]
 
-    df_dicts, tf_dicts = calculate_cooc_dicts(vocab_words, data, n_cores=n_cores, window=cooc_window)
+    df_dicts, tf_dicts = calculate_cooc_dicts(
+        vocab_words, data, n_cores=n_cores, window=cooc_window
+    )
 
     cooc_df_dict, cooc_df_term_dict = df_dicts[0], df_dicts[1]
     cooc_tf_dict, cooc_tf_term_dict = tf_dicts[0], tf_dicts[1]
 
     pairs_count = cooc_tf_dict[RESERVED_TUPLE]
 
     # print(docs_count, pairs_count)
@@ -241,55 +254,59 @@
         " |"
         + name_type
         + " "
         + " ".join(["{}:{}".format(k, v) for k, v in tokens_dict.items()])
     )
 
 
-def prepare_voc(batches_dir, vw_path, data_path, column_name="processed_text.txt"):
+def prepare_voc(batches_dir, vw_path, dataset: Union[pd.DataFrame, str], column_name="processed_text.txt"):
     print("Starting...")
     with open(vw_path, "w", encoding="utf8") as ofile:
-        num_parts = 0
-        try:
-            for file in os.listdir(data_path):
-                if file.startswith("part"):
-                    print("part_{}".format(num_parts), end="\r")
-                    if file.split(".")[-1] == "csv":
-                        part = pd.read_csv(os.path.join(data_path, file))
-                    else:
-                        part = pd.read_parquet(os.path.join(data_path, file))
-                    part_processed = part[column_name].tolist()
-                    for text in part_processed:
-                        result = return_string_part("@default_class", text)
-                        ofile.write(result + "\n")
-                    num_parts += 1
-
-        except NotADirectoryError:
-            print("part 1/1")
-            part = pd.read_csv(data_path)
-            part_processed = part[column_name].tolist()
+        if isinstance(dataset, str):
+            num_parts = 0
+            try:
+                for file in os.listdir(dataset):
+                    if file.startswith("part"):
+                        print("part_{}".format(num_parts), end="\r")
+                        if file.split(".")[-1] == "csv":
+                            part = pd.read_csv(os.path.join(dataset, file))
+                        else:
+                            part = pd.read_parquet(os.path.join(dataset, file))
+                        part_processed = part[column_name].tolist()
+                        for text in part_processed:
+                            result = return_string_part("@default_class", text)
+                            ofile.write(result + "\n")
+                        num_parts += 1
+
+            except NotADirectoryError:
+                print("part 1/1")
+                part = pd.read_csv(dataset)
+                part_processed = part[column_name].tolist()
+                for text in part_processed:
+                    result = return_string_part("@default_class", text)
+                    ofile.write(result + "\n")
+        else:
+            part_processed = dataset[column_name].tolist()
             for text in part_processed:
                 result = return_string_part("@default_class", text)
                 ofile.write(result + "\n")
 
-    print(" batches {} \n vocabulary {} \n are ready".format(batches_dir, vw_path))
+    logger.info(" batches {} \n vocabulary {} \n are ready".format(batches_dir, vw_path))
 
 
 def prepare_batch_vectorizer(
-    batches_dir: str, vw_path: str, data_path: str, column_name: str = "processed_text"
+    batches_dir: str, vw_path: str, dataset: Union[pd.DataFrame, str], column_name: str = "processed_text"
 ):
-    prepare_voc(batches_dir, vw_path, data_path, column_name=column_name)
+    prepare_voc(batches_dir, vw_path, dataset, column_name=column_name)
     batch_vectorizer = artm.BatchVectorizer(
         data_path=vw_path,
         data_format="vowpal_wabbit",
         target_folder=batches_dir,
         batch_size=100,
     )
-    #     else:
-    #         batch_vectorizer = artm.BatchVectorizer(data_path=batches_dir, data_format='batches')
 
     return batch_vectorizer
 
 
 def mutual_info_dict_preparation(fname):
     tokens_dict = {}
 
@@ -315,15 +332,15 @@
     cooc_file_path_tf = os.path.join(save_path, "cooc_tf.txt")
     ppmi_dict_df = os.path.join(save_path, "ppmi_df.txt")
     ppmi_dict_tf = os.path.join(save_path, "ppmi_tf.txt")
     MUTUAL_INFO_DICT_PATH = os.path.join(save_path, "mutual_info_dict.pkl")
     DOCUMENTS_TO_BATCH_PATH = os.path.join(save_path, "ppp.csv")
 
     # TODO: check why batch vectorizer is returned (unused further)
-    batch_vectorizer = prepare_batch_vectorizer(
+    prepare_batch_vectorizer(
         BATCHES_DIR, WV_PATH, DOCUMENTS_TO_BATCH_PATH
     )
 
     my_dictionary = artm.Dictionary()
     my_dictionary.gather(data_path=BATCHES_DIR, vocab_file_path=WV_PATH)
     my_dictionary.filter(min_df=3, class_id="text")
     my_dictionary.save_text(DICTIONARY_PATH)
```

### Comparing `autotm-0.1.0/src/autotm/preprocessing/text_preprocessing.py` & `autotm-0.2.0/autotm/preprocessing/text_preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import os
+from typing import Union, cast
+
 import pandas as pd
 import pymystem3
 from nltk.corpus import stopwords, wordnet
 from autotm.utils import parallelize_dataframe
 import nltk
-
-nltk.download("stopwords")
 import re
 from sklearn.feature_extraction.text import CountVectorizer
 
 import spacy
 from spacy.language import Language
 from spacy_langdetect import LanguageDetector
 from nltk.stem import WordNetLemmatizer
 
+
+# TODO: make transformer class and prep function to download all files
+
+nltk.download("stopwords")
+nltk.download("wordnet")
+
 stop = stopwords.words("russian") + [" "] + stopwords.words("english")
 
 r_html = re.compile(r"(\<[^>]*\>)")
 r_punct = re.compile(r'[."\[\]/,()!?;:*#|\\%^$&{}~_`=-@]')
 r_vk_ids = re.compile(r"(id{1}[0-9]*)")
 r_num = re.compile(r"([0-9]+)")
 r_white_space = re.compile(r"\s{2,}")
@@ -38,57 +44,56 @@
     return LanguageDetector()
 
 
 nlp_model = spacy.load("en_core_web_sm")
 nlp_model.add_pipe("language_detector", last=True)
 
 
-def new_html(text: str) -> str:
-    """ This is my perfect function"""
+def remove_html(text: str) -> str:
+    """html removal function"""
     text = r_html.sub("", text)
     return text
 
 
 def process_punkt(text: str) -> str:
     text = r_punct.sub(" ", text)
     text = r_vk_ids.sub(" ", text)
     text = r_num.sub(" ", text)
     text = r_white_space.sub(" ", text)
     return text.strip()
 
 
 def get_lemma(word: str) -> str:
-    lemma = wordnet.morphy(word)
-    if lemma is None:
+    """function to extract lemma from english words"""
+    synsets = wordnet.synsets(word)
+    if synsets is None or len(synsets) == 0:
         return word
     else:
-        return lemma
+        return synsets[0].lemmas()[0].name()
 
 
 def tokens_num(text):
     return len(text.split(" "))
 
 
-def lemmatize_text_ru(text: str) -> str:
+def lemmatize_text_ru(text: str, leave_service_info=False) -> str:
     try:
-        text = new_html(text)
+        text = remove_html(text)
     except:
         return ""
     text = text.lower()
     text = process_punkt(text)
-    #         text = re.findall(r_rus, text)
-    #         text = ' '.join(text)
     try:
         tokens = r_words.split(text)
     except:
         return ""
     tokens = (x for x in tokens if len(x) >= 3 and not x.isdigit())
     text = " ".join(tokens)
     tokens = m.lemmatize(text)
-    tokens = (x for x in tokens if len(x) > 3)
+    tokens = (x for x in tokens if len(x) >= 3)
     tokens = (x for x in tokens if x not in stop)
     tokens = (x for x in tokens if x.isalpha())
     text = " ".join(tokens)
     return text
 
 
 def get_wordnet_pos(word):
@@ -137,34 +142,34 @@
     else:
         print(f"The language {lang} is not known")
         raise NameError
     return df
 
 
 def process_dataset(
-    fname: str,
-    col_to_process: str,
-    save_path: str,
-    lang: str = "ru",
-    min_tokens_count: int = 3,
-    n_cores: int = -1,
+        fname: Union[pd.DataFrame, str],
+        col_to_process: str,
+        save_path: str,
+        lang: str = "ru",
+        min_tokens_count: int = 3,
+        n_cores: int = -1,
 ):
     """
 
     :param fname: Path to the dataset to process.
     :param col_to_process: The name of text column to be processed.
     :param save_path: Path where to store all the artifacts.
     :param lang: Language of the data (ru/en).
     :param min_tokens_count: Minimal amount of tokens to consider the further processing and topic modeling (3 by default).
     :param n_cores: Amount of cores for parallelization.
     :return:
     """
     os.makedirs(save_path, exist_ok=True)
     save_path = os.path.join(save_path, "ppp.csv")
-    data = pd.read_csv(fname)
+    data = pd.read_csv(fname) if isinstance(fname, str) else cast(pd.DataFrame, fname)
     data = parallelize_dataframe(
         data, lemmatize_text, n_cores, lang=lang, col_to_process=col_to_process
     )
     data["tokens_len"] = data["processed_text"].apply(tokens_num)
     data = data[data["tokens_len"] > min_tokens_count]
     data.to_csv(save_path, index=None)
     print("Saved to {}".format(save_path))
```

### Comparing `autotm-0.1.0/src/autotm/schemas.py` & `autotm-0.2.0/autotm/schemas.py`

 * *Files identical despite different names*

### Comparing `autotm-0.1.0/src/autotm/utils.py` & `autotm-0.2.0/autotm/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,20 +103,35 @@
     pool.join()
     return res
 
 
 def make_log_config_dict(
     filename: str = "/var/log/tm-alg.txt", uid: Optional[str] = None
 ) -> Dict[str, Any]:
-    if uid:
-        dirname = os.path.dirname(filename)
-        file, ext = os.path.splitext(os.path.basename(filename))
-        log_filename = os.path.join(dirname, f"{file}-{uid}.{ext}")
+    if filename is not None:
+        if uid:
+            dirname = os.path.dirname(filename)
+            file, ext = os.path.splitext(os.path.basename(filename))
+            log_filename = os.path.join(dirname, f"{file}-{uid}.{ext}")
+        else:
+            log_filename = filename
+
+        logfile_handler = {
+            "logfile": {
+                "level": "DEBUG",
+                "formatter": "standard",
+                "class": "logging.FileHandler",
+                "filename": log_filename,
+            }
+        }
+        handlers = ["default", "logfile"]
     else:
-        log_filename = filename
+        logfile_handler = dict()
+        handlers = ["default"]
+
     return {
         "version": 1,
         "disable_existing_loggers": True,
         "formatters": {
             "standard": {
                 "format": "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
             },
@@ -124,37 +139,32 @@
         "handlers": {
             "default": {
                 "level": "DEBUG",
                 "formatter": "standard",
                 "class": "logging.StreamHandler",
                 "stream": "ext://sys.stderr",
             },
-            "logfile": {
-                "level": "DEBUG",
-                "formatter": "standard",
-                "class": "logging.FileHandler",
-                "filename": log_filename,
-            },
+            **logfile_handler
         },
         "loggers": {
             "root": {
-                "handlers": ["default", "logfile"],
+                "handlers": handlers,
                 "level": "DEBUG",
                 "propagate": False,
             },
             "GA": {
-                "handlers": ["default", "logfile"],
+                "handlers": handlers,
                 "level": "DEBUG",
                 "propagate": False,
             },
             "GA_algo": {
-                "handlers": ["default", "logfile"],
+                "handlers": handlers,
                 "level": "DEBUG",
                 "propagate": False,
             },
             "GA_surrogate": {
-                "handlers": ["default", "logfile"],
+                "handlers": handlers,
                 "level": "DEBUG",
                 "propagate": False,
             },
         },
     }
```

### Comparing `autotm-0.1.0/src/autotm/visualization/dynamic_tracker.py` & `autotm-0.2.0/autotm/visualization/dynamic_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import time
+import warnings
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 from scipy.spatial import distance
 
 GENERATION_COL = "generation"
@@ -185,15 +186,19 @@
                     FITNESS_DIFF_COL: self.mutation_changes[gen]["fitness_diff"],
                     "original_params": self.mutation_changes[gen]["original_params"],
                     "mutated_params": self.mutation_changes[gen]["mutated_params"],
                 }
                 cur_df = pd.DataFrame(cur_df_dict)
                 cur_df[GENERATION_COL] = gen
                 dfs.append(cur_df)
-            self.mutation_df = pd.concat(dfs)
+            if len(dfs) > 0:
+                self.mutation_df = pd.concat(dfs)
+            else:
+                warnings.warn("No mutations changes have been found to save", RuntimeWarning)
+                self.mutation_df = pd.DataFrame([])
         if self.crossover_df is not None:
             print("Crossover df already exists")
         else:
             dfs = []
             for gen in self.crossover_changes:
                 cur_df_dict = {
                     "parent_1_params": self.crossover_changes[gen]["parent_1_params"],
@@ -223,35 +228,35 @@
         )
         self.crossover_df.to_csv(
             os.path.join(
                 self.save_path, f"{self.save_fname}_crossover_{int(time.time())}.csv"
             )
         )
 
-    def save_and_visualise_trace(self):
+    def save_trace(self):
         self.get_metric_df()
-        # save params
         self.write_metrics_to_file()
 
+    def save_and_visualise_trace(self, plot_mutation_effectiveness=False):
+        self.save_trace()
+
         # traces vis
         graph_template = "plotly_white"
 
         fig = px.line(
             self.metric_df,
             x=GENERATION_COL,
             y=FITNESS_COL,
             title="Score changes with generations",
             template=graph_template,
         )
         fig.show()
 
-        # mutation diff vis
-        fig = px.scatter(
-            self.mutation_df,
-            x=PARAMS_DIST_COL,
-            y=FITNESS_DIFF_COL,
-            title="Effectiveness of mutation operation",
-            template=graph_template,
-        )
-        fig.show()
-
-        # crossover diff vis
+        if plot_mutation_effectiveness:
+            fig = px.scatter(
+                self.mutation_df,
+                x=PARAMS_DIST_COL,
+                y=FITNESS_DIFF_COL,
+                title="Effectiveness of mutation operation",
+                template=graph_template,
+            )
+            fig.show()
```

### Comparing `autotm-0.1.0/PKG-INFO` & `autotm-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotm
-Version: 0.1.0
+Version: 0.2.0
 Summary: Automatic hyperparameters tuning for topic models (ARTM approach) using evolutionary algorithms
 Home-page: https://autotm.readthedocs.io/en/latest/
 License: Apache-2.0
 Author: Khodorchenko Maria
 Author-email: mariyaxod@yandex.ru
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -20,32 +20,38 @@
 Requires-Dist: gensim
 Requires-Dist: hyperopt
 Requires-Dist: mlflow
 Requires-Dist: nltk
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: plotly
+Requires-Dist: protobuf (<=3.20.0)
 Requires-Dist: pydantic
 Requires-Dist: pymongo
 Requires-Dist: pymystem3
 Requires-Dist: pytest
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
-Requires-Dist: spacy
+Requires-Dist: spacy (>=3.5)
 Requires-Dist: spacy-langdetect
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/ngc436/AutoTM
 Description-Content-Type: text/markdown
 
+
+<img align="left" src="docs/img/MyLogo.png" alt="Library scheme" height="200"/>
+
 # AutoTM
 
-[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 ![build](https://github.com/ngc436/AutoTM/actions/workflows/build.yaml/badge.svg)
-[![GitHub Repo stars](https://img.shields.io/github/stars/ngc436/AutoTM?style=social)](https://github.com/ngc436/AutoTM/stargazers)
-
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![PyPI version](https://badge.fury.io/py/autotm.svg)](https://badge.fury.io/py/autotm)
+[![Documentation Status](https://readthedocs.org/projects/autotm/badge/?version=latest)](https://autotm.readthedocs.io/en/latest/?badge=latest)
+[![Downloads](https://static.pepy.tech/personalized-badge/autotm?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/autotm)
 Automatic parameters selection for topic models (ARTM approach) using evolutionary algorithms. 
 AutoTM provides necessary tools to preprocess english and russian text datasets and tune topic models.
 
 ## What is AutoTM?
 Topic modeling is one of the basic methods for EDA of unlabelled text data. While ARTM (additive regularization 
 for topic models) approach provides the significant flexibility and quality comparative or better that neural 
 approaches it is hard to tune such models due to amount of hyperparameters and their combinations.
@@ -61,29 +67,39 @@
 <img src="docs/img/img_library_eng.png" alt="Library scheme" height=""/>
 
 
 ## Installation
 
 ! Note: The functionality of topic models training is available only for linux distributions.
 
+Via pip:
+
+```pip install autotm```
+
+From source:
+
 ```pip install -r requirements.txt```  
 
 ```python -m spacy download en_core_web_sm```
 
 ```export PYTHONPATH="${PYTHONPATH}:/path/to/src"```
 
 [//]: # (## Dataset and )
 
 ## Quickstart
 
 The notebook with an example is available in ```examples``` folder.
 
-## Distributed version
+## Running from the command line
+
+To fit a model:
+```autotmctl --verbose fit --config conf/config.yaml --in data/sample_corpora/sample_dataset_lenta.csv```
 
-Distributed version to run experiments on kubernetes is available in ```autotm-distributed``` brunch. Still this version is in development stage and will be transfered to separate repository.
+To predict with a fitted model:
+```autotmctl predict --in data/sample_corpora/sample_dataset_lenta.csv --model model.artm```
 
 ## Backlog:
 - [ ] Add tests
 - [ ] Add new multi-stage 
  
 ## Citation
```

