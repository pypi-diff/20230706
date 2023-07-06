# Comparing `tmp/kolena_client-0.75.0.tar.gz` & `tmp/kolena_client-0.76.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena_client-0.75.0.tar", max compression
+gzip compressed data, was "kolena_client-0.76.0.tar", max compression
```

## Comparing `kolena_client-0.75.0.tar` & `kolena_client-0.76.0.tar`

### file list

```diff
@@ -1,111 +1,113 @@
--rw-r--r--   0        0        0    11346 2023-06-28 00:31:50.503242 kolena_client-0.75.0/LICENSE
--rw-r--r--   0        0        0      556 2023-06-28 00:31:50.503242 kolena_client-0.75.0/LICENSE_HEADER
--rw-r--r--   0        0        0     2293 2023-06-28 00:31:50.503242 kolena_client-0.75.0/README.md
--rw-r--r--   0        0        0     1356 2023-06-28 00:37:17.961604 kolena_client-0.75.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5111 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5597 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0     1052 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0    16345 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    13671 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     4297 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      579 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      783 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      783 2023-06-28 00:31:50.555243 kolena_client-0.75.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     5033 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0      852 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8851 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    13920 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13600 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20960 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10130 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14750 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16125 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3880 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/initialize.py
--rw-r--r--   0        0        0     2439 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13948 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13854 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0     1103 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     2977 2023-06-28 00:31:50.559243 kolena_client-0.75.0/kolena/workflow/metrics/_formula.py
--rw-r--r--   0        0        0    16014 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8265 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    10261 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18116 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22734 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    10564 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15251 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0     9419 2023-06-28 00:31:50.563243 kolena_client-0.75.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3042 2023-06-28 00:37:17.961604 kolena_client-0.75.0/pyproject.toml
--rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 kolena_client-0.75.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-06 00:28:24.524548 kolena_client-0.76.0/LICENSE
+-rw-r--r--   0        0        0      556 2023-07-06 00:28:24.524548 kolena_client-0.76.0/LICENSE_HEADER
+-rw-r--r--   0        0        0     2293 2023-07-06 00:28:24.524548 kolena_client-0.76.0/README.md
+-rw-r--r--   0        0        0     1356 2023-07-06 00:33:52.018326 kolena_client-0.76.0/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5111 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5597 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     5654 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    15446 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    10294 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    13260 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     5029 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      783 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      921 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     5033 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0     1164 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-07-06 00:28:24.580549 kolena_client-0.76.0/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8995 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    14122 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13804 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20960 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10274 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/model.py
+-rw-r--r--   0        0        0    14952 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16329 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/initialize.py
+-rw-r--r--   0        0        0     2439 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13948 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13854 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1103 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     2977 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    16014 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8459 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18319 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22734 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    10564 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15455 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0     9419 2023-07-06 00:28:24.584549 kolena_client-0.76.0/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3047 2023-07-06 00:33:52.018326 kolena_client-0.76.0/pyproject.toml
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 kolena_client-0.76.0/PKG-INFO
```

### Comparing `kolena_client-0.75.0/LICENSE` & `kolena_client-0.76.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/LICENSE_HEADER` & `kolena_client-0.76.0/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/README.md` & `kolena_client-0.76.0/README.md`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/__init__.py` & `kolena_client-0.76.0/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/__init__.py` & `kolena_client-0.76.0/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/__init__.py` & `kolena_client-0.76.0/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/batched_load.py` & `kolena_client-0.76.0/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/client_log.py` & `kolena_client-0.76.0/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/core.py` & `kolena_client-0.76.0/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/detection.py` & `kolena_client-0.76.0/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/fr.py` & `kolena_client-0.76.0/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/generic.py` & `kolena_client-0.76.0/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/repository.py` & `kolena_client-0.76.0/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/token.py` & `kolena_client-0.76.0/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_api/v1/workflow.py` & `kolena_client-0.76.0/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_experimental/__init__.py` & `kolena_client-0.76.0/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_experimental/object_detection/__init__.py` & `kolena_client-0.76.0/kolena/_experimental/object_detection/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 # noreorder
 from .workflow import TestSample
 from .workflow import GroundTruth
 from .workflow import Inference
 from .workflow import TestCase
 from .workflow import TestSuite
 from .workflow import Model
+from .workflow import ThresholdStrategy
 from .workflow import ThresholdConfiguration
 from .evaluator import ObjectDetectionEvaluator
 
 __all__ = [
     "TestSample",
     "GroundTruth",
     "Inference",
     "TestCase",
     "TestSuite",
     "Model",
+    "ThresholdStrategy",
     "ThresholdConfiguration",
     "ObjectDetectionEvaluator",
 ]
```

### Comparing `kolena_client-0.75.0/kolena/_experimental/object_detection/evaluator.py` & `kolena_client-0.76.0/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,19 +18,17 @@
 from typing import Set
 from typing import Tuple
 
 import numpy as np
 
 from kolena._experimental.object_detection.utils import compute_average_precision
 from kolena._experimental.object_detection.utils import compute_confusion_matrix_plot
-from kolena._experimental.object_detection.utils import compute_f1_plot
 from kolena._experimental.object_detection.utils import compute_f1_plot_multiclass
 from kolena._experimental.object_detection.utils import compute_optimal_f1_threshold_multiclass
 from kolena._experimental.object_detection.utils import compute_pr_curve
-from kolena._experimental.object_detection.utils import compute_pr_plot
 from kolena._experimental.object_detection.utils import compute_pr_plot_multiclass
 from kolena._experimental.object_detection.workflow import ClassMetricsPerTestCase
 from kolena._experimental.object_detection.workflow import GroundTruth
 from kolena._experimental.object_detection.workflow import Inference
 from kolena._experimental.object_detection.workflow import TestCase
 from kolena._experimental.object_detection.workflow import TestCaseMetrics
 from kolena._experimental.object_detection.workflow import TestSample
@@ -45,39 +43,49 @@
 from kolena.workflow.metrics import f1_score as compute_f1_score
 from kolena.workflow.metrics import match_inferences_multiclass
 from kolena.workflow.metrics import MulticlassInferenceMatches
 from kolena.workflow.metrics import precision as compute_precision
 from kolena.workflow.metrics import recall as compute_recall
 
 
-class ObjectDetectionEvaluator(Evaluator):
+class MulticlassObjectDetectionEvaluator(Evaluator):
     """
-    This `ObjectDetectionEvaluator` transforms inferences into metrics for the object detection workflow for a single
-    class or multiple classes.
+    The `MulticlassObjectDetectionEvaluator` transforms inferences into metrics for the object detection workflow for
+    multiple classes.
 
     When a [`ThresholdConfiguration`][kolena._experimental.object_detection.workflow.ThresholdConfiguration] is
     configured to use an F1-Optimal threshold strategy, the evaluator requires that the first test case retrieved for
     a test suite contains the complete sample set.
 
     For additional functionality, see the associated [base class documentation][kolena.workflow.evaluator.Evaluator].
     """
 
-    # Assumes that the first test case retrieved for the test suite contains the complete sample set to be used for
-    # F1-Optimal threshold computation. Subsequent requests for a given threshold strategy (for other test cases) will
-    # hit this cache and use the previously computed population level confidence thresholds.
     threshold_cache: Dict[str, Dict[str, float]] = {}  # configuration -> label -> threshold
+    """
+    Assumes that the first test case retrieved for the test suite contains the complete sample set to be used for
+    F1-Optimal threshold computation. Subsequent requests for a given threshold strategy (for other test cases) will
+    hit this cache and use the previously computed population level confidence thresholds.
+    """
 
-    # Keeps track of test sample locators for each test case (used for total # of image count in aggregated metrics)
     locators_by_test_case: Dict[str, List[str]] = {}
+    """
+    Keeps track of test sample locators for each test case (used for total # of image count in aggregated metrics).
+    """
+
+    matchings_by_test_case: Dict[str, List[MulticlassInferenceMatches]] = defaultdict(list)
+    """
+    Caches matchings per test case for test case metrics and test case plots.
+    """
 
     def compute_image_metrics(
         self,
         ground_truth: GroundTruth,
         inference: Inference,
         configuration: ThresholdConfiguration,
+        test_case_name: str,
         labels: Set[str],  # the labels being tested in this test case
     ) -> TestSampleMetrics:
         assert configuration is not None, "must specify configuration"
         thresholds = self.get_confidence_thresholds(configuration)
         bbox_matches: MulticlassInferenceMatches = match_inferences_multiclass(
             ground_truth.bboxes,
             [
@@ -85,30 +93,26 @@
                 for inf in inference.bboxes
                 if inf.label in labels and inf.score >= configuration.min_confidence_score
             ],
             ignored_ground_truths=ground_truth.ignored_bboxes,
             mode="pascal",
             iou_threshold=configuration.iou_threshold,
         )
-        image_labels = {gt.label for gt in ground_truth.bboxes}
+        self.matchings_by_test_case[test_case_name].append(bbox_matches)
         tp = [inf for _, inf in bbox_matches.matched if inf.score >= thresholds[inf.label]]
-        fp = [
-            inf
-            for inf in bbox_matches.unmatched_inf
-            if inf.label in image_labels and inf.score >= thresholds[inf.label]
-        ]
+        fp = [inf for inf in bbox_matches.unmatched_inf if inf.score >= thresholds[inf.label]]
         fn = [gt for gt, _ in bbox_matches.unmatched_gt] + [
             gt for gt, inf in bbox_matches.matched if inf.score < thresholds[inf.label]
         ]
         confused = [
             inf for _, inf in bbox_matches.unmatched_gt if inf is not None and inf.score >= thresholds[inf.label]
         ]
         non_ignored_inferences = tp + fp
         scores = [inf.score for inf in non_ignored_inferences]
-
+        image_labels = {gt.label for gt in ground_truth.bboxes}
         fields = [
             ScoredClassificationLabel(label=label, score=thresholds[label])
             for label in thresholds.keys()
             if label in image_labels
         ]
         return TestSampleMetrics(
             TP=tp,
@@ -146,27 +150,33 @@
                 ignored_ground_truths=ground_truth.ignored_bboxes,
                 mode="pascal",
                 iou_threshold=configuration.iou_threshold,
             )
             for _, ground_truth, inference in inferences
         ]
         optimal_thresholds = compute_optimal_f1_threshold_multiclass(all_bbox_matches)
-        self.threshold_cache[configuration.display_name()] = optimal_thresholds
+        self.threshold_cache[configuration.display_name()] = defaultdict(
+            lambda: configuration.min_confidence_score,
+            optimal_thresholds,
+        )
 
     def compute_test_sample_metrics(
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> List[Tuple[TestSample, TestSampleMetrics]]:
         assert configuration is not None, "must specify configuration"
         # compute thresholds to cache values for subsequent steps
         self.compute_and_cache_f1_optimal_thresholds(configuration, inferences)
         labels = {gt.label for _, gts, _ in inferences for gt in gts.bboxes}
-        return [(ts, self.compute_image_metrics(gt, inf, configuration, labels)) for ts, gt, inf in inferences]
+        return [
+            (ts, self.compute_image_metrics(gt, inf, configuration, test_case.name, labels))
+            for ts, gt, inf in inferences
+        ]
 
     def compute_aggregate_label_metrics(
         self,
         matchings: List[MulticlassInferenceMatches],
         label: str,
         thresholds: Dict[str, float],
     ) -> ClassMetricsPerTestCase:
@@ -242,32 +252,19 @@
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[TestSampleMetrics],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> TestCaseMetrics:
         assert configuration is not None, "must specify configuration"
         thresholds = self.get_confidence_thresholds(configuration)
         labels = {gt.label for _, gts, _ in inferences for gt in gts.bboxes}
-        all_bbox_matches = [
-            match_inferences_multiclass(
-                ground_truth.bboxes,
-                [
-                    inf
-                    for inf in inference.bboxes
-                    if inf.label in labels and inf.score >= configuration.min_confidence_score
-                ],
-                ignored_ground_truths=ground_truth.ignored_bboxes,
-                mode="pascal",
-                iou_threshold=configuration.iou_threshold,
-            )
-            for _, ground_truth, inference in inferences
-        ]
+        all_bbox_matches = self.matchings_by_test_case[test_case.name]
 
         # compute nested metrics per class
         per_class_metrics: List[ClassMetricsPerTestCase] = []
-        for label in labels:
+        for label in sorted(labels):
             metrics_per_class = self.compute_aggregate_label_metrics(all_bbox_matches, label, thresholds)
             per_class_metrics.append(metrics_per_class)
 
         self.locators_by_test_case[test_case.name] = [ts.locator for ts, _, _ in inferences]
         tp_count = sum(im.count_TP for im in metrics)
         fp_count = sum(im.count_FP for im in metrics)
         fn_count = sum(im.count_FN for im in metrics)
@@ -289,30 +286,16 @@
         self,
         test_case: TestCase,
         inferences: List[Tuple[TestSample, GroundTruth, Inference]],
         metrics: List[TestSampleMetrics],
         configuration: Optional[ThresholdConfiguration] = None,
     ) -> Optional[List[Plot]]:
         assert configuration is not None, "must specify configuration"
-        labels = {gt.label for _, gts, _ in inferences for gt in gts.bboxes}
         thresholds = self.get_confidence_thresholds(configuration)
-        all_bbox_matches = [
-            match_inferences_multiclass(
-                ground_truth.bboxes,
-                [
-                    inf
-                    for inf in inference.bboxes
-                    if inf.label in labels and inf.score >= configuration.min_confidence_score
-                ],
-                ignored_ground_truths=ground_truth.ignored_bboxes,
-                mode="pascal",
-                iou_threshold=configuration.iou_threshold,
-            )
-            for _, ground_truth, inference in inferences
-        ]
+        all_bbox_matches = self.matchings_by_test_case[test_case.name]
 
         # clean matching for confusion matrix
         match_matched = [
             (gt, inf) for match in all_bbox_matches for gt, inf in match.matched if inf.score >= thresholds[inf.label]
         ]
         match_unmatched_gt = [
             (gt, inf)
@@ -329,16 +312,14 @@
         ]
 
         plots: Optional[List[Plot]] = []
         plots.extend(
             filter(
                 None,
                 [
-                    compute_pr_plot(all_bbox_matches),
-                    compute_f1_plot(all_bbox_matches),
                     compute_f1_plot_multiclass(all_bbox_matches),
                     compute_pr_plot_multiclass(all_bbox_matches),
                     compute_confusion_matrix_plot(confusion_matrix_matchings),
                 ],
             ),
         )
```

### Comparing `kolena_client-0.75.0/kolena/_experimental/object_detection/utils.py` & `kolena_client-0.76.0/kolena/_experimental/object_detection/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,22 @@
 
 def _compute_threshold_curve(
     y_true: np.ndarray,
     y_score: np.ndarray,
     curve_type: Literal["pr", "f1"],
     curve_label: Optional[str] = None,
 ) -> Optional[Curve]:
-    if len(y_score) >= 501:
-        thresholds = list(np.linspace(min(abs(y_score)), max(y_score), 501))
-    elif len(y_score) > 1:
-        thresholds = np.unique(y_score[y_score >= 0.0]).tolist()  # sorts
-    else:
+    if len(y_score) < 1:
         return None
 
+    thresholds = np.unique(y_score[y_score >= 0.0]).tolist()  # sorts
+
+    if len(thresholds) >= 501:
+        thresholds = list(np.linspace(min(thresholds), max(thresholds), 501))
+
     precisions: List[float] = []
     recalls: List[float] = []
     f1s: List[float] = []
     for threshold in thresholds:
         y_pred = [1 if score >= threshold else 0 for score in y_score]
         precision, recall, f1, _ = sklearn_metrics.precision_recall_fscore_support(
             y_true,
@@ -91,23 +92,17 @@
     else:
         return Curve(x=recalls, y=precisions, label=curve_label)
 
 
 def _compute_multiclass_curves(
     all_matches: List[MulticlassInferenceMatches],
     curve_type: Literal["pr", "f1"],
-    curve_label: Optional[str] = None,
 ) -> Optional[List[Curve]]:
     curves: List[Curve] = []
-    y_true, y_score = _compute_sklearn_arrays(all_matches)
     y_true_score_by_label = _compute_sklearn_arrays_by_class(all_matches)
-    curve = _compute_threshold_curve(y_true, y_score, curve_type, curve_label)
-    if curve is None:
-        return None
-    curves.append(curve)
 
     for label, (y_true, y_score) in sorted(y_true_score_by_label.items(), key=lambda x: x[0]):
         curve = _compute_threshold_curve(y_true, y_score, curve_type, label)
         if curve is not None:
             curves.append(curve)
     return curves if curves else None
 
@@ -150,25 +145,23 @@
         if curve
         else None
     )
 
 
 def compute_pr_plot_multiclass(
     all_matches: List[MulticlassInferenceMatches],
-    curve_label: Optional[str] = None,
 ) -> Optional[CurvePlot]:
     """
     Creates a PR (precision-recall) curve for the multiclass object detection workflow.
     For `n` labels, each plot has `n+1` curves. One for the test case, and one per label.
 
     :param all_matches: a list of multiclass matching results.
-    :param curve_label: the label of the main curve.
     :return: :class:`CurvePlot` for the PR curves of the test case and each label.
     """
-    pr_curves: Optional[List[Curve]] = _compute_multiclass_curves(all_matches, "pr", curve_label)
+    pr_curves: Optional[List[Curve]] = _compute_multiclass_curves(all_matches, "pr")
 
     return (
         CurvePlot(
             title="Precision vs. Recall Per Class",
             x_label="Recall",
             y_label="Precision",
             curves=pr_curves,
@@ -202,25 +195,24 @@
         if curve
         else None
     )
 
 
 def compute_f1_plot_multiclass(
     all_matches: List[MulticlassInferenceMatches],
-    curve_label: Optional[str] = None,
 ) -> Optional[CurvePlot]:
     """
     Creates a F1-threshold (confidence threshold) curve for the multiclass object detection workflow.
     For `n` labels, each plot has `n+1` curves. One for the test case, and one per label.
 
     :param all_matches: a list of multiclass matching results.
     :param curve_label: the label of the main curve.
     :return: :class:`CurvePlot` for the F1-threshold curves of the test case and each label.
     """
-    f1_curves: Optional[List[Curve]] = _compute_multiclass_curves(all_matches, "f1", curve_label)
+    f1_curves: Optional[List[Curve]] = _compute_multiclass_curves(all_matches, "f1")
 
     return (
         CurvePlot(
             title="F1-Score vs. Confidence Threshold Per Class",
             x_label="Confidence Threshold",
             y_label="F1-Score",
             curves=f1_curves,
```

### Comparing `kolena_client-0.75.0/kolena/_experimental/object_detection/workflow.py` & `kolena_client-0.76.0/kolena/_experimental/object_detection/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,46 @@
     TestSample,
     GroundTruth,
     Inference,
 )
 
 
 @dataclass(frozen=True)
+class TestSampleMetricsSingleClass(MetricsTestSample):
+    TP: List[ScoredLabeledBoundingBox]
+    FP: List[ScoredLabeledBoundingBox]
+    FN: List[LabeledBoundingBox]
+
+    count_TP: int
+    count_FP: int
+    count_FN: int
+
+    has_TP: bool
+    has_FP: bool
+    has_FN: bool
+
+    max_confidence_above_t: Optional[float]
+    min_confidence_above_t: Optional[float]
+    thresholds: float
+
+
+@dataclass(frozen=True)
+class TestCaseMetricsSingleClass(MetricsTestCase):
+    Objects: int
+    Inferences: int
+    TP: int
+    FN: int
+    FP: int
+    Precision: float
+    Recall: float
+    F1: float
+    AP: float
+
+
+@dataclass(frozen=True)
 class TestSampleMetrics(MetricsTestSample):
     TP: List[ScoredLabeledBoundingBox]
     FP: List[ScoredLabeledBoundingBox]
     FN: List[LabeledBoundingBox]
     Confused: List[ScoredLabeledBoundingBox]
 
     count_TP: int
@@ -139,13 +171,15 @@
 
 
 @dataclass(frozen=True)
 class ThresholdConfiguration(EvaluatorConfiguration):
     threshold_strategy: ThresholdStrategy
     iou_threshold: float
     min_confidence_score: float
+    with_class_level_metrics: bool
 
     def display_name(self) -> str:
         return (
-            f"Threshold: {self.threshold_strategy.display_name()}, "
+            f"Threshold: {self.threshold_strategy.display_name()}"
+            f"{' by class' if self.with_class_level_metrics else ''}, "
             f"IoU: {self.iou_threshold}, confidence ≥ {self.min_confidence_score}"
         )
```

### Comparing `kolena_client-0.75.0/kolena/_extras/__init__.py` & `kolena_client-0.76.0/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_extras/metrics/__init__.py` & `kolena_client-0.76.0/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_extras/metrics/sklearn.py` & `kolena_client-0.76.0/kolena/_extras/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/__init__.py` & `kolena_client-0.76.0/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/asset_path_mapper.py` & `kolena_client-0.76.0/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/batched_load.py` & `kolena_client-0.76.0/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/cli.py` & `kolena_client-0.76.0/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/consts.py` & `kolena_client-0.76.0/kolena/_utils/consts.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,7 +17,13 @@
 class BatchSize(int, Enum):
     UPLOAD_CHIPS = 1_000
     UPLOAD_RECORDS = 10_000_000
     UPLOAD_RESULTS = 1_000_000
 
     LOAD_RECORDS = UPLOAD_RECORDS
     LOAD_SAMPLES = 1_000_000
+
+
+class FieldName(str, Enum):
+    TEST_CASE_NAME = "Test Case name"
+    TEST_SUITE_NAME = "Test Suite name"
+    MODEL_NAME = "Model name"
```

### Comparing `kolena_client-0.75.0/kolena/_utils/dataframes/__init__.py` & `kolena_client-0.76.0/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/dataframes/validators.py` & `kolena_client-0.76.0/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/datatypes.py` & `kolena_client-0.76.0/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/endpoints.py` & `kolena_client-0.76.0/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/frozen.py` & `kolena_client-0.76.0/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/geometry.py` & `kolena_client-0.76.0/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/inference_validators.py` & `kolena_client-0.76.0/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/instrumentation.py` & `kolena_client-0.76.0/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/krequests.py` & `kolena_client-0.76.0/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/log.py` & `kolena_client-0.76.0/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/repository.py` & `kolena_client-0.76.0/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/serde.py` & `kolena_client-0.76.0/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/serializable.py` & `kolena_client-0.76.0/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/state.py` & `kolena_client-0.76.0/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/uninstantiable.py` & `kolena_client-0.76.0/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/_utils/validators.py` & `kolena_client-0.76.0/kolena/detection/_internal/ground_truth.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from pydantic import Extra
+from enum import Enum
 
 
-class ValidatorConfig:
-    """Pydantic configuration for dataclasses and @validate_arguments decorators."""
-
-    arbitrary_types_allowed = True
-    smart_union = True
-    extra = Extra.allow  # do not fail when unrecognized values are provided
+class GroundTruthType(str, Enum):
+    CLASSIFICATION_LABEL = "CLASSIFICATION_LABEL"
+    BOUNDING_BOX = "BOUNDING_BOX"
+    SEGMENTATION_MASK = "SEGMENTATION_MASK"
```

### Comparing `kolena_client-0.75.0/kolena/classification/__init__.py` & `kolena_client-0.76.0/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/metadata.py` & `kolena_client-0.76.0/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/model.py` & `kolena_client-0.76.0/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/multiclass/__init__.py` & `kolena_client-0.76.0/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/multiclass/_utils.py` & `kolena_client-0.76.0/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/multiclass/evaluator.py` & `kolena_client-0.76.0/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/multiclass/test_run.py` & `kolena_client-0.76.0/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/multiclass/workflow.py` & `kolena_client-0.76.0/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/test_case.py` & `kolena_client-0.76.0/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/test_config.py` & `kolena_client-0.76.0/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/test_image.py` & `kolena_client-0.76.0/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/test_run.py` & `kolena_client-0.76.0/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/classification/test_suite.py` & `kolena_client-0.76.0/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/__init__.py` & `kolena_client-0.76.0/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_datatypes.py` & `kolena_client-0.76.0/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/__init__.py` & `kolena_client-0.76.0/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/datatypes.py` & `kolena_client-0.76.0/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/inference.py` & `kolena_client-0.76.0/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/metadata.py` & `kolena_client-0.76.0/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/model.py` & `kolena_client-0.76.0/kolena/detection/_internal/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 from kolena._api.v1.detection import Model as API
 from kolena._api.v1.workflow import WorkflowType
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import DFType
 from kolena._utils.consts import BatchSize
+from kolena._utils.consts import FieldName
 from kolena._utils.endpoints import get_model_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseTestCase
 from kolena.detection._internal import BaseTestImage
 from kolena.detection._internal import BaseTestSuite
 from kolena.detection._internal.test_image import TestImageType
 from kolena.errors import InputValidationError
 from kolena.errors import NotFoundError
@@ -75,14 +77,15 @@
     _TestCaseClass: Type[BaseTestCase] = BaseTestCase
     _TestSuiteClass: Type[BaseTestSuite] = BaseTestSuite
     _InferenceClass: Type[InferenceType] = InferenceType
     _LoadInferencesDataFrameClass: Type[DFType] = DFType
 
     @validate_arguments(config=ValidatorConfig)
     def __init__(self, name: str, workflow: WorkflowType, metadata: Optional[Dict[str, Any]] = None):
+        validate_name(name, FieldName.MODEL_NAME)
         try:
             loaded = self._load_by_name(name)
             if len(loaded.metadata) > 0 and loaded.metadata != metadata:
                 log.warn(f"mismatch in model metadata, using loaded metadata (loaded: {loaded.metadata})")
         except NotFoundError:
             loaded = self._create(workflow, name, metadata or {})
```

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/test_case.py` & `kolena_client-0.76.0/kolena/detection/_internal/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,20 @@
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import DFType
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
 from kolena._utils.consts import BatchSize
+from kolena._utils.consts import FieldName
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseTestImage
 from kolena.errors import NotFoundError
 from kolena.workflow._validators import assert_workflows_match
 
 
 class BaseTestCase(ABC, Frozen, WithTelemetry):
@@ -83,14 +85,15 @@
         name: str,
         workflow: WorkflowType,
         version: Optional[int] = None,
         description: Optional[str] = None,
         images: Optional[List[_TestImageClass]] = None,
         reset: bool = False,
     ):
+        validate_name(name, FieldName.TEST_CASE_NAME)
         try:
             self._populate_from_other(self.load(name, version))
             if description is not None and self.description != description and not reset:
                 log.warn("test case already exists, not updating description when reset=False")
             if images is not None:
                 if self.version > 0 and not reset:
                     log.warn("not updating images for test case that has already been edited when reset=False")
@@ -126,14 +129,15 @@
         cls,
         workflow: WorkflowType,
         name: str,
         description: Optional[str] = None,
         images: Optional[List[_TestImageClass]] = None,
     ) -> "BaseTestCase":
         """Create a new test case with the provided name."""
+        validate_name(name, FieldName.TEST_CASE_NAME)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=workflow.value)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test case '{name}' (v{obj.version})")
         if images is not None:
```

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/test_config.py` & `kolena_client-0.76.0/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/test_image.py` & `kolena_client-0.76.0/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/test_run.py` & `kolena_client-0.76.0/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/_internal/test_suite.py` & `kolena_client-0.76.0/kolena/detection/_internal/test_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 from pydantic import validate_arguments
 
 import kolena._api.v1.core as CoreAPI
 from kolena._api.v1.detection import TestSuite as API
 from kolena._api.v1.workflow import WorkflowType
 from kolena._utils import krequests
 from kolena._utils import log
+from kolena._utils.consts import FieldName
 from kolena._utils.endpoints import get_test_suite_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.detection._internal import BaseTestCase
 from kolena.errors import NotFoundError
 from kolena.workflow._validators import assert_workflows_match
 
 
 class BaseTestSuite(ABC, Frozen, WithTelemetry):
@@ -67,14 +69,15 @@
         name: str,
         workflow: WorkflowType,
         version: Optional[int] = None,
         description: Optional[str] = None,
         test_cases: Optional[List[BaseTestCase]] = None,
         reset: bool = False,
     ):
+        validate_name(name, FieldName.TEST_SUITE_NAME)
         self._validate_test_cases(test_cases)
 
         try:
             self._populate_from_other(self.load(name, version))
             if description is not None and self.description != description and not reset:
                 log.warn("test suite already exists, not updating description when reset=False")
             if test_cases is not None:
@@ -107,14 +110,15 @@
         cls,
         workflow: WorkflowType,
         name: str,
         description: Optional[str] = None,
         test_cases: Optional[List[BaseTestCase]] = None,
     ) -> "BaseTestSuite":
         """Create a new test suite with the provided name."""
+        validate_name(name, FieldName.TEST_SUITE_NAME)
         request = CoreAPI.TestSuite.CreateRequest(name=name, description=description or "", workflow=workflow.value)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.TestSuite.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         if test_cases is not None:
```

### Comparing `kolena_client-0.75.0/kolena/detection/ground_truth.py` & `kolena_client-0.76.0/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/inference.py` & `kolena_client-0.76.0/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/metadata.py` & `kolena_client-0.76.0/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/model.py` & `kolena_client-0.76.0/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/test_case.py` & `kolena_client-0.76.0/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/test_config.py` & `kolena_client-0.76.0/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/test_image.py` & `kolena_client-0.76.0/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/test_run.py` & `kolena_client-0.76.0/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/detection/test_suite.py` & `kolena_client-0.76.0/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/errors.py` & `kolena_client-0.76.0/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/fr/__init__.py` & `kolena_client-0.76.0/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/fr/_utils.py` & `kolena_client-0.76.0/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/fr/datatypes.py` & `kolena_client-0.76.0/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/fr/model.py` & `kolena_client-0.76.0/kolena/fr/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 import numpy as np
 from pydantic.dataclasses import dataclass
 
 from kolena._api.v1.fr import Model as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
+from kolena._utils.consts import FieldName
 from kolena._utils.endpoints import get_model_url
 from kolena._utils.serde import from_dict
 from kolena._utils.uninstantiable import Uninstantiable
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.fr import TestCase
 from kolena.fr import TestSuite
 from kolena.fr.datatypes import LoadedPairResultDataFrame
 
 
 class Model(Uninstantiable["Model.Data"]):
@@ -51,14 +53,15 @@
         Create a new model with the provided name and metadata.
 
         :param name: Unique name of the new model to create.
         :param metadata: Unstructured metadata to associate with the model.
         :return: The newly created model.
         :raises ValueError: A model by the provided name already exists.
         """
+        validate_name(name, FieldName.MODEL_NAME)
         request = API.CreateRequest(name=name, metadata=metadata)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = Model.__factory__(from_dict(data_class=Model.Data, data=res.json()))
         log.info(f"created model '{name}' ({get_model_url(obj.data.id)})")
         return obj
```

### Comparing `kolena_client-0.75.0/kolena/fr/test_case.py` & `kolena_client-0.76.0/kolena/fr/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 from kolena._api.v1.fr import TestCase as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
 from kolena._utils.consts import BatchSize
+from kolena._utils.consts import FieldName
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
 from kolena.fr.datatypes import TEST_CASE_COLUMNS
 from kolena.fr.datatypes import TestCaseDataFrame
 from kolena.fr.datatypes import TestCaseDataFrameSchema
 from kolena.fr.datatypes import TestCaseRecord
 
@@ -84,14 +86,15 @@
         self,
         name: str,
         version: Optional[int] = None,
         description: Optional[str] = None,
         test_samples: Optional[List[TestCaseRecord]] = None,
         reset: bool = False,
     ):
+        validate_name(name, FieldName.TEST_CASE_NAME)
         try:
             self._populate_from_other(self.load(name, version))
             if description is not None and self.description != description and not reset:
                 log.warn("test case already exists, not updating description when reset=False")
             if test_samples is not None:
                 if self.version > 0 and not reset:
                     log.warn("not updating test samples for test case that has already been edited when reset=False")
@@ -130,14 +133,15 @@
         Create a new test case with the provided name.
 
         :param name: The name of the new test case to create.
         :param description: Optional free-form description of the test case to create.
         :param test_samples: Optionally specify a set of test samples to populate the test case.
         :return: The newly created test case.
         """
+        validate_name(name, FieldName.TEST_CASE_NAME)
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test case '{name}' (v{obj.version})")
         if test_samples is not None:
```

### Comparing `kolena_client-0.75.0/kolena/fr/test_images.py` & `kolena_client-0.76.0/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/fr/test_run.py` & `kolena_client-0.76.0/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/fr/test_suite.py` & `kolena_client-0.76.0/kolena/fr/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 
 from deprecation import deprecated
 from pydantic import validate_arguments
 
 from kolena._api.v1.fr import TestSuite as API
 from kolena._utils import krequests
 from kolena._utils import log
+from kolena._utils.consts import FieldName
 from kolena._utils.endpoints import get_test_suite_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
 from kolena.fr.test_case import TestCase
 
 
 class TestSuite(ABC, Frozen, WithTelemetry):
     """
@@ -82,14 +84,15 @@
         name: str,
         version: Optional[int] = None,
         description: Optional[str] = None,
         baseline_test_cases: Optional[List[TestCase]] = None,
         non_baseline_test_cases: Optional[List[TestCase]] = None,
         reset: bool = False,
     ):
+        validate_name(name, FieldName.TEST_SUITE_NAME)
         try:
             self._populate_from_other(self.load(name, version))
             if description is not None and self.description != description and not reset:
                 log.warn("test suite already exists, not updating description when reset=False")
             if baseline_test_cases is not None or non_baseline_test_cases is not None:
                 if self.version > 0 and not reset:
                     log.warn("test suite already exists, not updating test cases when reset=False")
@@ -130,14 +133,15 @@
 
         :param name: The name of the new test suite to create.
         :param description: Optional free-form description of the test suite to create.
         :param baseline_test_cases: Optionally specify a list of test cases to use as baseline for the test suite.
         :param non_baseline_test_cases: Optionally specify a list of test cases to populate the test suite.
         :return: The newly created test suite.
         """
+        validate_name(name, FieldName.TEST_SUITE_NAME)
         request = API.CreateRequest(name=name, description=description or "")
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=API.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         obj._hydrate(baseline_test_cases, non_baseline_test_cases)
```

### Comparing `kolena_client-0.75.0/kolena/initialize.py` & `kolena_client-0.76.0/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/__init__.py` & `kolena_client-0.76.0/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/_datatypes.py` & `kolena_client-0.76.0/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/_validators.py` & `kolena_client-0.76.0/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/annotation.py` & `kolena_client-0.76.0/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/asset.py` & `kolena_client-0.76.0/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/define_workflow.py` & `kolena_client-0.76.0/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/evaluator.py` & `kolena_client-0.76.0/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/evaluator_function.py` & `kolena_client-0.76.0/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/ground_truth.py` & `kolena_client-0.76.0/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/inference.py` & `kolena_client-0.76.0/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/metrics/__init__.py` & `kolena_client-0.76.0/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/metrics/_formula.py` & `kolena_client-0.76.0/kolena/workflow/metrics/_formula.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/metrics/_geometry.py` & `kolena_client-0.76.0/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/model.py` & `kolena_client-0.76.0/kolena/workflow/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,21 @@
 
 from kolena._api.v1.core import Model as CoreAPI
 from kolena._api.v1.generic import Model as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.consts import BatchSize
+from kolena._utils.consts import FieldName
 from kolena._utils.endpoints import get_model_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import NotFoundError
 from kolena.workflow import GroundTruth
 from kolena.workflow import Inference
 from kolena.workflow import TestCase
 from kolena.workflow import TestSample as BaseTestSample
 from kolena.workflow._datatypes import TestSampleDataFrame
@@ -91,14 +93,15 @@
         self,
         name: str,
         infer: Optional[Callable[[TestSample], Inference]] = None,
         metadata: Optional[Dict[str, Any]] = None,
     ):
         if type(self) == Model:
             raise Exception("<Model> must be subclassed.")
+        validate_name(name, FieldName.MODEL_NAME)
         try:
             loaded = self.load(name, infer)
             if len(loaded.metadata.keys()) > 0 and loaded.metadata != metadata:
                 log.warn(f"mismatch in model metadata, using loaded metadata (loaded: {loaded.metadata})")
         except NotFoundError:
             loaded = self.create(name, infer, metadata)
 
@@ -115,14 +118,15 @@
         Create a new model.
 
         :param name: The unique name of the new model to create.
         :param infer: Optional inference function for this model.
         :param metadata: Optional unstructured metadata to store with this model.
         :return: The newly created model.
         """
+        validate_name(name, FieldName.MODEL_NAME)
         metadata = metadata or {}
         request = CoreAPI.CreateRequest(name=name, metadata=metadata, workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         obj = cls._from_data_with_infer(from_dict(data_class=CoreAPI.EntityData, data=res.json()), infer)
         log.info(f"created model '{name}' ({get_model_url(obj._id)})")
         return obj
```

### Comparing `kolena_client-0.75.0/kolena/workflow/plot.py` & `kolena_client-0.76.0/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/test_case.py` & `kolena_client-0.76.0/kolena/workflow/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,21 @@
 from kolena._api.v1.generic import TestCase as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.batched_load import init_upload
 from kolena._utils.batched_load import upload_data_frame
 from kolena._utils.consts import BatchSize
+from kolena._utils.consts import FieldName
 from kolena._utils.dataframes.validators import validate_df_schema
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import IncorrectUsageError
 from kolena.errors import NotFoundError
 from kolena.workflow import GroundTruth
 from kolena.workflow import TestSample
 from kolena.workflow._datatypes import TestCaseEditorDataFrame
 from kolena.workflow._datatypes import TestSampleDataFrame
@@ -120,14 +122,16 @@
         version: Optional[int] = None,
         description: Optional[str] = None,
         test_samples: Optional[List[Tuple[TestSample, GroundTruth]]] = None,
         reset: bool = False,
     ):
         if type(self) == TestCase:
             raise Exception("<TestCase> must be subclassed.")
+
+        validate_name(name, FieldName.TEST_CASE_NAME)
         self._validate_test_samples(test_samples)
 
         try:
             self._populate_from_other(self.load(name, version))
             if description is not None and self.description != description and not reset:
                 log.warn("test case already exists, not updating description when reset=False")
             if test_samples is not None:
@@ -194,14 +198,15 @@
 
         :param name: The name of the new test case to create.
         :param description: Optional free-form description of the test case to create.
         :param test_samples: Optionally specify a set of test samples and ground truths to populate the test case.
         :return: The newly created test case.
         """
         cls._validate_test_samples(test_samples)
+        validate_name(name, FieldName.TEST_CASE_NAME)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name)
         res = krequests.post(endpoint_path=API.Path.CREATE.value, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test case '{name}' (v{obj.version})")
         if test_samples is not None:
```

### Comparing `kolena_client-0.75.0/kolena/workflow/test_run.py` & `kolena_client-0.76.0/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/test_sample.py` & `kolena_client-0.76.0/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/kolena/workflow/test_suite.py` & `kolena_client-0.76.0/kolena/workflow/test_suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,19 +28,21 @@
 
 from kolena._api.v1.core import TestSuite as CoreAPI
 from kolena._api.v1.generic import TestSuite as API
 from kolena._utils import krequests
 from kolena._utils import log
 from kolena._utils.batched_load import _BatchedLoader
 from kolena._utils.consts import BatchSize
+from kolena._utils.consts import FieldName
 from kolena._utils.endpoints import get_test_suite_url
 from kolena._utils.frozen import Frozen
 from kolena._utils.instrumentation import telemetry
 from kolena._utils.instrumentation import WithTelemetry
 from kolena._utils.serde import from_dict
+from kolena._utils.validators import validate_name
 from kolena._utils.validators import ValidatorConfig
 from kolena.errors import IncorrectUsageError
 from kolena.errors import NotFoundError
 from kolena.workflow import TestSample
 from kolena.workflow._datatypes import TestSuiteTestSamplesDataFrame
 from kolena.workflow._validators import assert_workflows_match
 from kolena.workflow.test_case import TestCase
@@ -100,14 +102,15 @@
         name: str,
         version: Optional[int] = None,
         description: Optional[str] = None,
         test_cases: Optional[List[TestCase]] = None,
         reset: bool = False,
         tags: Optional[Set[str]] = None,
     ):
+        validate_name(name, FieldName.TEST_SUITE_NAME)
         self._validate_workflow()
         self._validate_test_cases(test_cases)
 
         try:
             other = self.load(name, version)
         except NotFoundError:
             other = self.create(name, description, test_cases, tags)
@@ -191,14 +194,15 @@
         :param description: Optional free-form description of the test suite to create.
         :param test_cases: Optionally specify a list of test cases to populate the test suite.
         :param tags: Optionally specify a set of tags to attach to the test suite.
         :return: The newly created test suite.
         """
         cls._validate_workflow()
         cls._validate_test_cases(test_cases)
+        validate_name(name, FieldName.TEST_SUITE_NAME)
         request = CoreAPI.CreateRequest(name=name, description=description or "", workflow=cls.workflow.name, tags=tags)
         res = krequests.post(endpoint_path=API.Path.CREATE, data=json.dumps(dataclasses.asdict(request)))
         krequests.raise_for_status(res)
         data = from_dict(data_class=CoreAPI.EntityData, data=res.json())
         obj = cls._create_from_data(data)
         log.info(f"created test suite '{name}' (v{obj.version}) ({get_test_suite_url(obj._id)})")
         if test_cases is not None:
```

### Comparing `kolena_client-0.75.0/kolena/workflow/workflow.py` & `kolena_client-0.76.0/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena_client-0.75.0/pyproject.toml` & `kolena_client-0.76.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena-client"
-version = "0.75.0"  # version is automatically set to latest git tag during release process
+version = "0.76.0"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning (ML) testing and debugging platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
@@ -31,15 +31,15 @@
     { version = ">=1.23", python = ">=3.11" },
 ]
 pandas = [
     { version = ">=1.1,<1.6", python = ">=3.7,<3.11" },
     { version = ">=1.5,<1.6", python = ">=3.11" },
 ]
 pandera = ">=0.9.0"
-pydantic = ">=1.8"
+pydantic = ">=1.8,<2.0"
 dacite = ">=1.6"
 requests = ">=2.20,<2.30" # TODO: revert upper bound when urllib3 situation sorts out: https://github.com/psf/requests/issues/6432
 requests-toolbelt = "*"
 importlib-metadata = { version = "<5.0", python = "<3.8" }
 tqdm = ">=4,<5"
 Pillow = "^9.1.1"
 retrying = "^1.3.3"
```

### Comparing `kolena_client-0.75.0/PKG-INFO` & `kolena_client-0.76.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena-client
-Version: 0.75.0
+Version: 0.76.0
 Summary: Client for Kolena's machine learning (ML) testing and debugging platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
@@ -33,15 +33,15 @@
 Requires-Dist: importlib-metadata (<5.0) ; python_version < "3.8"
 Requires-Dist: numpy (>=1.19) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: numpy (>=1.23) ; python_version >= "3.11"
 Requires-Dist: pandas (>=1.1,<1.6) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: pandas (>=1.5,<1.6) ; python_version >= "3.11"
 Requires-Dist: pandera (>=0.9.0)
 Requires-Dist: pyarrow (>=8)
-Requires-Dist: pydantic (>=1.8)
+Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: requests (>=2.20,<2.30)
 Requires-Dist: requests-toolbelt
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0,<1.0.3) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "metrics")
 Requires-Dist: scikit-learn (>=1.2) ; (python_version >= "3.8") and (extra == "metrics")
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: tqdm (>=4,<5)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena-client Version: 0.75.0 Summary: Client for
+Metadata-Version: 2.1 Name: kolena-client Version: 0.76.0 Summary: Client for
 Kolena's machine learning (ML) testing and debugging platform. Home-page:
 https://kolena.io License: Apache-2.0 Keywords: Kolena,ML,testing Author:
 Kolena Engineering Author-email: eng@kolena.io Requires-Python: >=3.7.1,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3 Classifier:
@@ -18,16 +18,16 @@
 (>=8.1.3,<9.0.0) Requires-Dist: dacite (>=1.6) Requires-Dist: deprecation
 (>=2.1.0,<3.0.0) Requires-Dist: importlib-metadata (<5.0) ; python_version <
 "3.8" Requires-Dist: numpy (>=1.19) ; python_version >= "3.7" and
 python_version < "3.11" Requires-Dist: numpy (>=1.23) ; python_version >=
 "3.11" Requires-Dist: pandas (>=1.1,<1.6) ; python_version >= "3.7" and
 python_version < "3.11" Requires-Dist: pandas (>=1.5,<1.6) ; python_version >=
 "3.11" Requires-Dist: pandera (>=0.9.0) Requires-Dist: pyarrow (>=8) Requires-
-Dist: pydantic (>=1.8) Requires-Dist: requests (>=2.20,<2.30) Requires-Dist:
-requests-toolbelt Requires-Dist: retrying (>=1.3.3,<2.0.0) Requires-Dist:
+Dist: pydantic (>=1.8,<2.0) Requires-Dist: requests (>=2.20,<2.30) Requires-
+Dist: requests-toolbelt Requires-Dist: retrying (>=1.3.3,<2.0.0) Requires-Dist:
 scikit-learn (>=1.0,<1.0.3) ; (python_full_version >= "3.7.1" and
 python_version < "3.8") and (extra == "metrics") Requires-Dist: scikit-learn
 (>=1.2) ; (python_version >= "3.8") and (extra == "metrics") Requires-Dist:
 termcolor (>=1.1.0,<2.0.0) Requires-Dist: tqdm (>=4,<5) Requires-Dist: typing-
 extensions (>=4.5.0,<5.0.0) ; python_version < "3.8" Project-URL:
 Documentation, https://docs.kolena.io Description-Content-Type: text/markdown
                                    [Kolena]
```

