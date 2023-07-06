# Comparing `tmp/hyfi-1.0.4.tar.gz` & `tmp/hyfi-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.0.4.tar", max compression
+gzip compressed data, was "hyfi-1.0.5.tar", max compression
```

## Comparing `hyfi-1.0.4.tar` & `hyfi-1.0.5.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     1071 2023-07-04 21:41:16.278685 hyfi-1.0.4/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-04 21:41:16.278685 hyfi-1.0.4/README.md
--rw-r--r--   0        0        0     4863 2023-07-04 21:41:42.590413 hyfi-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4267 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2550 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/__click__.py
--rw-r--r--   0        0        0      788 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/__global__/__init__.py
--rw-r--r--   0        0        0     9245 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/__global__/config.py
--rw-r--r--   0        0        0      733 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-04 21:41:42.514413 hyfi-1.0.4/src/hyfi/_version.py
--rw-r--r--   0        0        0     1890 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7229 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    32964 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     7331 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/composer/extended.py
--rw-r--r--   0        0        0        0 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-04 21:41:42.514413 hyfi-1.0.4/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      553 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      320 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      217 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      921 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      170 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      178 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      351 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      395 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0       99 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6548 2023-07-04 21:41:16.282685 hyfi-1.0.4/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0     5915 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4228 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    50188 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4915 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4183 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/path/base.py
--rw-r--r--   0        0        0      782 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      599 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1609 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8085 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2900 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5618 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/py.typed
--rw-r--r--   0        0        0     4268 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     6967 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30058 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     6568 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     3769 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20157 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-04 21:41:16.286685 hyfi-1.0.4/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-05 23:58:53.756217 hyfi-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-05 23:58:53.756217 hyfi-1.0.5/README.md
+-rw-r--r--   0        0        0     4863 2023-07-05 23:59:18.488518 hyfi-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4267 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2550 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      788 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__global__/__init__.py
+-rw-r--r--   0        0        0     9245 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__global__/config.py
+-rw-r--r--   0        0        0      733 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-05 23:59:18.412517 hyfi-1.0.5/src/hyfi/_version.py
+-rw-r--r--   0        0        0     1890 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7229 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    32964 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     7421 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/composer/extended.py
+-rw-r--r--   0        0        0        0 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-05 23:59:18.412517 hyfi-1.0.5/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      553 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      320 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      217 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      921 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       73 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      133 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      170 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      161 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      359 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      378 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0       99 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0       99 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6548 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0     5915 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4228 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-05 23:58:53.760217 hyfi-1.0.5/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    50188 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4915 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4183 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      782 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      599 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1609 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8085 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     2900 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5618 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4268 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7014 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30058 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     6568 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     3769 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20157 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-05 23:58:53.764217 hyfi-1.0.5/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 hyfi-1.0.5/PKG-INFO
```

### Comparing `hyfi-1.0.4/LICENSE` & `hyfi-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/README.md` & `hyfi-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/pyproject.toml` & `hyfi-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.0.4"
+version = "1.0.5"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -13,15 +13,15 @@
 hyfi = 'hyfi.__cli__:hydra_main'
 hyfi-run = 'hyfi.__click__:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
-pydantic = "^2.0.1"
+pydantic = "^2.0.2"
 chardet = "<=5.1.0"
 pandas = ">=1.5.3,<=2.0.2"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
 numpy = "<=1.24.4"
 python-dotenv = "^1.0.0"
 requests = "^2.27.1"
@@ -34,15 +34,15 @@
 huggingface-hub = ">=0.8.1,<=0.15.1"
 # google-cloud-storage = ">=1.32.0,<3.0"
 # boto3 = ">=1.0,<2.0"
 click = "<=8.1.3"
 pyarrow = "<=12.0.1"
 datasets = "<=2.13.1"
 joblib = "^1.3.1"
-pydantic-settings = "^2.0.0"
+pydantic-settings = "^2.0.1"
 
 [tool.poetry.group.ipython]
 optional = true
 
 [tool.poetry.group.ipython.dependencies]
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
```

### Comparing `hyfi-1.0.4/src/hyfi/__cli__.py` & `hyfi-1.0.5/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/__click__.py` & `hyfi-1.0.5/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/__global__/__init__.py` & `hyfi-1.0.5/src/hyfi/__global__/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/__global__/config.py` & `hyfi-1.0.5/src/hyfi/__global__/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/__init__.py` & `hyfi-1.0.5/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/about/__init__.py` & `hyfi-1.0.5/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/batch/__init__.py` & `hyfi-1.0.5/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/__init__.py` & `hyfi-1.0.5/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.0.5/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/cache_file.py` & `hyfi-1.0.5/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/common.py` & `hyfi-1.0.5/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/file_lock.py` & `hyfi-1.0.5/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/meta.py` & `hyfi-1.0.5/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/progress.py` & `hyfi-1.0.5/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.0.5/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.0.5/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.0.5/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.0.5/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.0.5/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/testing.py` & `hyfi-1.0.5/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/cached_path/util.py` & `hyfi-1.0.5/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/composer/__init__.py` & `hyfi-1.0.5/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/composer/extended.py` & `hyfi-1.0.5/src/hyfi/composer/extended.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 import random
 from typing import Any, Callable, Dict, Union
 
 import hydra
 from omegaconf import OmegaConf
 
 from hyfi.__global__ import __home_path__, __hyfi_path__
-from hyfi.__global__.config import __global_config__, __search_package_path__
+from hyfi.__global__.config import (
+    __global_config__,
+    __search_package_path__,
+    __version__,
+)
 from hyfi.cached_path import cached_path
 from hyfi.composer import Composer, SpecialKeys
 from hyfi.utils.envs import ENVs
 from hyfi.utils.funcs import FUNCs
 from hyfi.utils.iolibs import IOLIBs
 from hyfi.utils.logging import LOGGING
 from hyfi.utils.packages import PKGs
@@ -142,14 +146,15 @@
             obj: The object to print the source code of.
 
         """
         print(XC.getsource(obj))
 
 
 OmegaConf.register_new_resolver("__hyfi_path__", __hyfi_path__)
+OmegaConf.register_new_resolver("__version__", __version__)
 OmegaConf.register_new_resolver("__search_package_path__", __search_package_path__)
 OmegaConf.register_new_resolver("__home_path__", __home_path__)
 OmegaConf.register_new_resolver("today", FUNCs.today)
 OmegaConf.register_new_resolver("to_datetime", FUNCs.strptime)
 OmegaConf.register_new_resolver("iif", lambda cond, t, f: t if cond else f)
 OmegaConf.register_new_resolver("alt", lambda val, alt: val or alt)
 OmegaConf.register_new_resolver("randint", random.randint, use_cache=True)
```

### Comparing `hyfi-1.0.4/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.0.5/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.0.5/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.0.5/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.0.5/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.0.5/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.0.5/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.0.5/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/copier/__init__.py` & `hyfi-1.0.5/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/dotenv/__init__.py` & `hyfi-1.0.5/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/graphics/collage.py` & `hyfi-1.0.5/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/graphics/motion.py` & `hyfi-1.0.5/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/graphics/utils.py` & `hyfi-1.0.5/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/joblib/__init__.py` & `hyfi-1.0.5/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/joblib/batch/apply.py` & `hyfi-1.0.5/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.0.5/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.0.5/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/main/__init__.py` & `hyfi-1.0.5/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/path/__init__.py` & `hyfi-1.0.5/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/path/base.py` & `hyfi-1.0.5/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/path/batch.py` & `hyfi-1.0.5/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/path/dirnames.py` & `hyfi-1.0.5/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/path/task.py` & `hyfi-1.0.5/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/pipe/__init__.py` & `hyfi-1.0.5/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/pipe/test.py` & `hyfi-1.0.5/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/pipeline/__init__.py` & `hyfi-1.0.5/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/pipeline/configs.py` & `hyfi-1.0.5/src/hyfi/pipeline/configs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/project/__init__.py` & `hyfi-1.0.5/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/task/__init__.py` & `hyfi-1.0.5/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/task/batch.py` & `hyfi-1.0.5/src/hyfi/task/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     batch_name: str = "demo"
     batch: Optional[BatchConfig] = None
 
     _property_set_methods_ = {
         "task_name": "set_task_name",
         "task_root": "set_task_root",
         "batch_name": "set_batch_name",
-        "batch_num": "set_batch_num",
     }
     _subconfigs_ = {"batch": BatchConfig}
 
     def set_batch_name(self, val):
         if not self.batch_name or self.batch_name != val:
             if self.path:
                 self.path.batch_name = val
@@ -72,14 +71,18 @@
             self.batch_dir,
         )
 
     @property
     def batch_num(self):
         return self.batch.batch_num if self.batch else None
 
+    @batch_num.setter
+    def batch_num(self, val):
+        self.set_batch_num(val)
+
     @property
     def seed(self):
         return self.batch.seed if self.batch else None
 
     @property
     def batch_dir(self):
         return self.batch.batch_dir if self.batch else None
```

### Comparing `hyfi-1.0.4/src/hyfi/utils/contexts.py` & `hyfi-1.0.5/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/datasets.py` & `hyfi-1.0.5/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/envs.py` & `hyfi-1.0.5/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/funcs.py` & `hyfi-1.0.5/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/gpumon.py` & `hyfi-1.0.5/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/iolibs.py` & `hyfi-1.0.5/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/logging.py` & `hyfi-1.0.5/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/notebooks.py` & `hyfi-1.0.5/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/utils/packages.py` & `hyfi-1.0.5/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/src/hyfi/workflow/__init__.py` & `hyfi-1.0.5/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.0.4/PKG-INFO` & `hyfi-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.0.4
+Version: 1.0.5
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -24,16 +24,16 @@
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: joblib (>=1.3.1,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (<=1.24.4)
 Requires-Dist: pandas (>=1.5.3,<=2.0.2)
 Requires-Dist: pathspec (>=0.9.0)
 Requires-Dist: pyarrow (<=12.0.1)
-Requires-Dist: pydantic (>=2.0.1,<3.0.0)
-Requires-Dist: pydantic-settings (>=2.0.0,<3.0.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic-settings (>=2.0.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12.1,<14.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi
 Description-Content-Type: text/markdown
```

