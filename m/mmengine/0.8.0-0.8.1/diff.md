# Comparing `tmp/mmengine-0.8.0.tar.gz` & `tmp/mmengine-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmengine-0.8.0.tar", last modified: Mon Jul  3 12:32:28 2023, max compression
+gzip compressed data, was "dist/mmengine-0.8.1.tar", last modified: Thu Jul  6 02:23:14 2023, max compression
```

## Comparing `mmengine-0.8.0.tar` & `mmengine-0.8.1.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-03 12:30:58.000000 mmengine-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-07-03 12:32:28.000000 mmengine-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17518 2023-07-03 12:30:58.000000 mmengine-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/_strategy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/complexity_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/jit_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/jit_handles.py
--rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/analysis/print_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/config/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70813 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/device/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/dist/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/dist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/evaluator/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/evaluator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/fileio/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/http_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/lmdb_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/local_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/memcached_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/petrel_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/backends/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/file_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/fileio/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/pickle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/handlers/yaml_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/fileio/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/early_stopping_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/ema_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/empty_cache_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/iter_timer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/logger_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/naive_visualization_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/param_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/profiler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/runtime_info_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/sampler_seed_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/sync_buffer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hooks/test_time_aug_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/deprecated.json
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/mmcls.json
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/openmmlab.json
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/hub/torchvision_0.12.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/infer/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/history_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/logging/message_hub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/averaged_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/model/base_model/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_model/data_preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/base_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/test_time_aug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/model/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    21334 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/fully_sharded_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/seperate_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/model/wrappers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/optim/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/amp_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/apex_optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/default_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/optimizer/zero_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/optim/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/momentum_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/optim/scheduler/param_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/build_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/default_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/registry/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/runner/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/_flexible_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/base_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/log_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/loops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)   101587 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/base_data_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/instance_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/label_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/structures/pixel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/testing/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/_internal/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/testing/runner_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/utils/dl_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/parrots_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/setup_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/torch_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/dl_utils/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/vis_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-07-03 12:30:59.000000 mmengine-0.8.0/mmengine/visualization/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-03 12:32:28.000000 mmengine-0.8.0/mmengine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 12:32:27.000000 mmengine-0.8.0/mmengine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-03 12:32:28.000000 mmengine-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-03 12:30:59.000000 mmengine-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-06 02:21:50.000000 mmengine-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-06 02:23:14.000000 mmengine-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-07-06 02:21:50.000000 mmengine-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39482 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26640 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/_strategy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/complexity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26249 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/jit_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/jit_handles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31115 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/analysis/print_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71175 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33863 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20024 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43256 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20768 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/dist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/evaluator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/fileio/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/http_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/lmdb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18135 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/local_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/memcached_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27918 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/petrel_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/backends/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/file_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/fileio/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/pickle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/handlers/yaml_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/fileio/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29409 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/early_stopping_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/ema_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/empty_cache_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16661 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/iter_timer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/logger_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/naive_visualization_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/param_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14669 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/profiler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/runtime_info_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/sampler_seed_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/sync_buffer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hooks/test_time_aug_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/deprecated.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/mmcls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/openmmlab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/hub/torchvision_0.12.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27712 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/infer/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/history_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18541 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/logging/message_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/averaged_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/model/base_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_model/data_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/test_time_aug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26125 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/model/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/fully_sharded_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/seperate_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/model/wrappers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/optim/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/amp_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/apex_optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6728 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14591 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/default_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7677 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/optimizer/zero_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/optim/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18104 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/momentum_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64430 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/optim/scheduler/param_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13415 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/build_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/default_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26948 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/registry/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66277 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/_flexible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/base_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30359 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/log_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17179 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/loops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101587 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24573 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/base_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13483 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/instance_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/label_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/structures/pixel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/testing/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/_internal/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/testing/runner_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/utils/dl_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/parrots_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/setup_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/torch_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/dl_utils/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17512 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36637 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/vis_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53917 2023-07-06 02:21:50.000000 mmengine-0.8.1/mmengine/visualization/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-06 02:23:14.000000 mmengine-0.8.1/mmengine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-06 02:23:14.000000 mmengine-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-07-06 02:21:50.000000 mmengine-0.8.1/setup.py
```

### Comparing `mmengine-0.8.0/PKG-INFO` & `mmengine-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -66,15 +66,15 @@
         
         ## What's New
         
         v0.8.0 was released on 2023-06-30.
         
         Highlights:
         
-        - Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [example](https://github.com/open-mmlab/mmengine/blob/main/examples/distributed_training_with_flexible_runner.py) for more detailed usages.
+        - Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for more detailed usages.
         
         - Introduce the pure Python style configuration file:
         
           - Support navigating to base configuration file in IDE
           - Support navigating to base variable in IDE
           - Support navigating to source code of class in IDE
           - Support inheriting two configuration files containing the same field
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.0 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.1 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
@@ -20,16 +20,16 @@
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
 ## What's New v0.8.0 was released on 2023-06-30. Highlights: - Support training
 with [FSDP](https://pytorch.org/tutorials/intermediate/
 FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://
-www.deepspeed.ai/). Refer to the [example](https://github.com/open-mmlab/
-mmengine/blob/main/examples/distributed_training_with_flexible_runner.py) for
+www.deepspeed.ai/). Refer to the [Training Large Models](https://
+mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for
 more detailed usages. - Introduce the pure Python style configuration file: -
 Support navigating to base configuration file in IDE - Support navigating to
 base variable in IDE - Support navigating to source code of class in IDE -
 Support inheriting two configuration files containing the same field - Load the
 configuration file without other third-party requirements Refer to the
 [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/
 config.html#a-pure-python-style-configuration-file-beta) for more detailed
```

### Comparing `mmengine-0.8.0/README.md` & `mmengine-0.8.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 ## What's New
 
 v0.8.0 was released on 2023-06-30.
 
 Highlights:
 
-- Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [example](https://github.com/open-mmlab/mmengine/blob/main/examples/distributed_training_with_flexible_runner.py) for more detailed usages.
+- Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for more detailed usages.
 
 - Introduce the pure Python style configuration file:
 
   - Support navigating to base configuration file in IDE
   - Support navigating to base variable in IDE
   - Support navigating to source code of class in IDE
   - Support inheriting two configuration files containing the same field
```

### Comparing `mmengine-0.8.0/mmengine/_strategy/__init__.py` & `mmengine-0.8.1/mmengine/_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/_strategy/base.py` & `mmengine-0.8.1/mmengine/_strategy/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/_strategy/deepspeed.py` & `mmengine-0.8.1/mmengine/_strategy/deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/_strategy/distributed.py` & `mmengine-0.8.1/mmengine/_strategy/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/_strategy/fsdp.py` & `mmengine-0.8.1/mmengine/_strategy/fsdp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/_strategy/single_device.py` & `mmengine-0.8.1/mmengine/_strategy/single_device.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/_strategy/utils.py` & `mmengine-0.8.1/mmengine/_strategy/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/analysis/complexity_analysis.py` & `mmengine-0.8.1/mmengine/analysis/complexity_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/analysis/jit_analysis.py` & `mmengine-0.8.1/mmengine/analysis/jit_analysis.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/analysis/jit_handles.py` & `mmengine-0.8.1/mmengine/analysis/jit_handles.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/analysis/print_helper.py` & `mmengine-0.8.1/mmengine/analysis/print_helper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/config/config.py` & `mmengine-0.8.1/mmengine/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,26 @@
 
 if platform.system() == 'Windows':
     import regex as re
 else:
     import re  # type: ignore
 
 
+def _lazy2string(cfg_dict, dict_type=None):
+    if isinstance(cfg_dict, dict):
+        dict_type = dict_type or type(cfg_dict)
+        return dict_type({k: _lazy2string(v) for k, v in dict.items(cfg_dict)})
+    elif isinstance(cfg_dict, (tuple, list)):
+        return type(cfg_dict)(_lazy2string(v) for v in cfg_dict)
+    elif isinstance(cfg_dict, (LazyAttr, LazyObject)):
+        return f'{cfg_dict.module}.{str(cfg_dict)}'
+    else:
+        return cfg_dict
+
+
 class ConfigDict(Dict):
     """A dictionary for config which has the same interface as python's built-
     in dictionary and can be used as a normal dictionary.
 
     The Config class would transform the nested fields (dictionary-like fields)
     in config file into ``ConfigDict``.
 
@@ -245,15 +257,15 @@
                 return a if a is not default else b
 
         merged = _merge_a_into_b(copy.deepcopy(other), copy.deepcopy(self))
         self.clear()
         for key, value in merged.items():
             self[key] = value
 
-    def to_dict(self):
+    def _to_lazy_dict(self):
         """Convert the ConfigDict to a normal dictionary recursively, and keep
         the ``LazyObject`` or ``LazyAttr`` object not built."""
 
         def _to_dict(data):
             if isinstance(data, ConfigDict):
                 return {
                     key: _to_dict(value)
@@ -264,14 +276,19 @@
             elif isinstance(data, (list, tuple)):
                 return type(data)(_to_dict(item) for item in data)
             else:
                 return data
 
         return _to_dict(self)
 
+    def to_dict(self):
+        """Convert the ConfigDict to a normal dictionary recursively, and keep
+        the ``LazyObject`` or ``LazyAttr`` object not built."""
+        return _lazy2string(self, dict_type=dict)
+
 
 def add_args(parser: ArgumentParser,
              cfg: dict,
              prefix: str = '') -> ArgumentParser:
     """Add config fields into argument parser.
 
     Args:
@@ -314,14 +331,16 @@
     values as attributes.
 
     Args:
         cfg_dict (dict, optional): A config dictionary. Defaults to None.
         cfg_text (str, optional): Text of config. Defaults to None.
         filename (str or Path, optional): Name of config file.
             Defaults to None.
+        format_python_code (bool): Whether to format Python code by yapf.
+            Defaults to True.
 
     Here is a simple example:
 
     Examples:
         >>> cfg = Config(dict(a=1, b=dict(b1=[0, 1])))
         >>> cfg.a
         1
@@ -344,29 +363,31 @@
     .. _config tutorial: https://mmengine.readthedocs.io/en/latest/advanced_tutorials/config.html
     """  # noqa: E501
 
     def __init__(self,
                  cfg_dict: dict = None,
                  cfg_text: Optional[str] = None,
                  filename: Optional[Union[str, Path]] = None,
-                 env_variables: Optional[dict] = None):
+                 env_variables: Optional[dict] = None,
+                 format_python_code: bool = True):
         filename = str(filename) if isinstance(filename, Path) else filename
         if cfg_dict is None:
             cfg_dict = dict()
         elif not isinstance(cfg_dict, dict):
             raise TypeError('cfg_dict must be a dict, but '
                             f'got {type(cfg_dict)}')
         for key in cfg_dict:
             if key in RESERVED_KEYS:
                 raise KeyError(f'{key} is reserved for config file')
 
         if not isinstance(cfg_dict, ConfigDict):
             cfg_dict = ConfigDict(cfg_dict)
         super().__setattr__('_cfg_dict', cfg_dict)
         super().__setattr__('_filename', filename)
+        super().__setattr__('_format_python_code', format_python_code)
         if cfg_text:
             text = cfg_text
         elif filename:
             with open(filename, encoding='utf-8') as f:
                 text = f.read()
         else:
             text = ''
@@ -376,26 +397,29 @@
         super().__setattr__('_env_variables', env_variables)
 
     @staticmethod
     def fromfile(filename: Union[str, Path],
                  use_predefined_variables: bool = True,
                  import_custom_modules: bool = True,
                  use_environment_variables: bool = True,
-                 lazy_import: Optional[bool] = None) -> 'Config':
+                 lazy_import: Optional[bool] = None,
+                 format_python_code: bool = True) -> 'Config':
         """Build a Config instance from config file.
 
         Args:
             filename (str or Path): Name of config file.
             use_predefined_variables (bool, optional): Whether to use
                 predefined variables. Defaults to True.
             import_custom_modules (bool, optional): Whether to support
                 importing custom modules in config. Defaults to None.
             lazy_import (bool): Whether to load config in `lazy_import` mode.
                 If it is `None`, it will be deduced by the content of the
                 config file. Defaults to None.
+            format_python_code (bool): Whether to format Python code by yapf.
+                Defaults to True.
 
         Returns:
             Config: Config instance built from config file.
         """
         filename = str(filename) if isinstance(filename, Path) else filename
         if lazy_import is None:
             lazy_import = Config._is_lazy_import(filename)
@@ -430,21 +454,26 @@
             ConfigDict.lazy = True
             try:
                 cfg_dict, imported_names = Config._parse_lazy_import(filename)
             except Exception as e:
                 raise e
             finally:
                 ConfigDict.lazy = False
-            for key, value in list(cfg_dict.to_dict().items()):
+
+            # delete builtin imported objects
+            for key, value in list(cfg_dict._to_lazy_dict().items()):
                 if isinstance(value, (types.FunctionType, types.ModuleType)):
                     cfg_dict.pop(key)
 
             # disable lazy import to get the real type. See more details about
             # lazy in the docstring of ConfigDict
-            cfg = Config(cfg_dict, filename=filename)
+            cfg = Config(
+                cfg_dict,
+                filename=filename,
+                format_python_code=format_python_code)
             object.__setattr__(cfg, '_imported_names', imported_names)
             return cfg
 
     @staticmethod
     def fromstring(cfg_str: str, file_format: str) -> 'Config':
         """Build a Config instance from config text.
 
@@ -1317,16 +1346,14 @@
             s = '\n'.join(s)
             s = first + '\n' + s
             return s
 
         def _format_basic_types(k, v, use_mapping=False):
             if isinstance(v, str):
                 v_str = repr(v)
-            elif isinstance(v, (LazyObject, LazyAttr)):
-                v_str = f"'{v.module}.{str(v)}'"
             else:
                 v_str = str(v)
 
             if use_mapping:
                 k_str = f"'{k}'" if isinstance(k, str) else str(k)
                 attr_str = f'{k_str}: {v_str}'
             else:
@@ -1350,16 +1377,14 @@
                     v_str += f'dict({_indent(_format_dict(item), indent)}),\n'
                 elif isinstance(item, tuple):
                     v_str += f'{_indent(_format_list_tuple(None, item), indent)},\n'  # noqa: 501
                 elif isinstance(item, list):
                     v_str += f'{_indent(_format_list_tuple(None, item), indent)},\n'  # noqa: 501
                 elif isinstance(item, str):
                     v_str += f'{_indent(repr(item), indent)},\n'
-                elif isinstance(item, (LazyObject, LazyAttr)):
-                    v_str += f"'{str(item)}',\n"
                 else:
                     v_str += str(item) + ',\n'
             if k is None:
                 return _indent(v_str, indent) + right
             if use_mapping:
                 k_str = f"'{k}'" if isinstance(k, str) else str(k)
                 attr_str = f'{k_str}: {v_str}'
@@ -1381,17 +1406,15 @@
 
             use_mapping = _contain_invalid_identifier(input_dict)
             if use_mapping:
                 r += '{'
             for idx, (k, v) in enumerate(input_dict.items()):
                 is_last = idx >= len(input_dict) - 1
                 end = '' if outest_level or is_last else ','
-                if isinstance(v, (LazyObject, LazyAttr)):
-                    attr_str = _format_basic_types(k, v, use_mapping) + end
-                elif isinstance(v, dict):
+                if isinstance(v, dict):
                     v_str = '\n' + _format_dict(v)
                     if use_mapping:
                         k_str = f"'{k}'" if isinstance(k, str) else str(k)
                         attr_str = f'{k_str}: dict({v_str}'
                     else:
                         attr_str = f'{str(k)}=dict({v_str}'
                     attr_str = _indent(attr_str, indent) + ')' + end
@@ -1402,27 +1425,28 @@
 
                 s.append(attr_str)
             r += '\n'.join(s)
             if use_mapping:
                 r += '}'
             return r
 
-        cfg_dict = self._to_lazy_dict()
+        cfg_dict = self.to_dict()
         text = _format_dict(cfg_dict, outest_level=True)
-        # copied from setup.cfg
-        yapf_style = dict(
-            based_on_style='pep8',
-            blank_line_before_nested_class_or_def=True,
-            split_before_expression_after_opening_paren=True)
-        try:
-            text, _ = FormatCode(text, style_config=yapf_style, verify=True)
-        except:  # noqa: E722
-            raise SyntaxError('Failed to format the config file, please '
-                              f'check the syntax of: \n{text}')
-
+        if self._format_python_code:
+            # copied from setup.cfg
+            yapf_style = dict(
+                based_on_style='pep8',
+                blank_line_before_nested_class_or_def=True,
+                split_before_expression_after_opening_paren=True)
+            try:
+                text, _ = FormatCode(
+                    text, style_config=yapf_style, verify=True)
+            except:  # noqa: E722
+                raise SyntaxError('Failed to format the config file, please '
+                                  f'check the syntax of: \n{text}')
         return text
 
     def __repr__(self):
         return f'Config (path: {self.filename}): {self._cfg_dict.__repr__()}'
 
     def __len__(self):
         return len(self._cfg_dict)
@@ -1486,15 +1510,15 @@
             is dumped to a str, otherwise to a file specified by the filename.
             Defaults to None.
 
         Returns:
             str or None: Config text.
         """
         file = str(file) if isinstance(file, Path) else file
-        cfg_dict = super().__getattribute__('_cfg_dict').to_dict()
+        cfg_dict = self.to_dict()
         if file is None:
             if self.filename is None or self.filename.endswith('.py'):
                 return self.pretty_text
             else:
                 file_format = self.filename.split('.')[-1]
                 return dump(cfg_dict, file_format=file_format)
         elif file.endswith('.py'):
@@ -1590,15 +1614,15 @@
                     if not _is_builtin_module(alias_node.name):
                         return True
         return False
 
     def _to_lazy_dict(self, keep_imported: bool = False) -> dict:
         """Convert config object to dictionary and filter the imported
         object."""
-        res = self._cfg_dict.to_dict()
+        res = self._cfg_dict._to_lazy_dict()
         if hasattr(self, '_imported_names') and not keep_imported:
             res = {
                 key: value
                 for key, value in res.items()
                 if key not in self._imported_names
             }
         return res
@@ -1609,29 +1633,15 @@
         Args:
             keep_imported (bool): Whether to keep the imported field.
                 Defaults to False
 
         If you import third-party objects in the config file, all imported
         objects will be converted to a string like ``torch.optim.SGD``
         """
-        _cfg_dict = self._to_lazy_dict(keep_imported)
-
-        def lazy2string(cfg_dict):
-            if isinstance(cfg_dict, dict):
-                return type(cfg_dict)(
-                    {k: lazy2string(v)
-                     for k, v in cfg_dict.items()})
-            elif isinstance(cfg_dict, (tuple, list)):
-                return type(cfg_dict)(lazy2string(v) for v in cfg_dict)
-            elif isinstance(cfg_dict, (LazyAttr, LazyObject)):
-                return f'{cfg_dict.module}.{str(cfg_dict)}'
-            else:
-                return cfg_dict
-
-        return lazy2string(_cfg_dict)
+        return self._cfg_dict.to_dict()
 
 
 class DictAction(Action):
     """
     argparse action to split an argument into KEY=VALUE form
     on the first = and append to a dictionary. List options can
     be passed as comma separated values, i.e 'KEY=V1,V2,V3', or with explicit
```

### Comparing `mmengine-0.8.0/mmengine/config/lazy.py` & `mmengine-0.8.1/mmengine/config/lazy.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/config/utils.py` & `mmengine-0.8.1/mmengine/config/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dataset/__init__.py` & `mmengine-0.8.1/mmengine/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dataset/base_dataset.py` & `mmengine-0.8.1/mmengine/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dataset/dataset_wrapper.py` & `mmengine-0.8.1/mmengine/dataset/dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dataset/sampler.py` & `mmengine-0.8.1/mmengine/dataset/sampler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dataset/utils.py` & `mmengine-0.8.1/mmengine/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/device/utils.py` & `mmengine-0.8.1/mmengine/device/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dist/__init__.py` & `mmengine-0.8.1/mmengine/dist/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dist/dist.py` & `mmengine-0.8.1/mmengine/dist/dist.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/dist/utils.py` & `mmengine-0.8.1/mmengine/dist/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/evaluator/evaluator.py` & `mmengine-0.8.1/mmengine/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/evaluator/metric.py` & `mmengine-0.8.1/mmengine/evaluator/metric.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/evaluator/utils.py` & `mmengine-0.8.1/mmengine/evaluator/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/__init__.py` & `mmengine-0.8.1/mmengine/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/__init__.py` & `mmengine-0.8.1/mmengine/fileio/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/base.py` & `mmengine-0.8.1/mmengine/fileio/backends/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/http_backend.py` & `mmengine-0.8.1/mmengine/fileio/backends/http_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/lmdb_backend.py` & `mmengine-0.8.1/mmengine/fileio/backends/lmdb_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/local_backend.py` & `mmengine-0.8.1/mmengine/fileio/backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/memcached_backend.py` & `mmengine-0.8.1/mmengine/fileio/backends/memcached_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/petrel_backend.py` & `mmengine-0.8.1/mmengine/fileio/backends/petrel_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/backends/registry_utils.py` & `mmengine-0.8.1/mmengine/fileio/backends/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/file_client.py` & `mmengine-0.8.1/mmengine/fileio/file_client.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/handlers/base.py` & `mmengine-0.8.1/mmengine/fileio/handlers/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/handlers/json_handler.py` & `mmengine-0.8.1/mmengine/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/handlers/pickle_handler.py` & `mmengine-0.8.1/mmengine/fileio/handlers/pickle_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/handlers/registry_utils.py` & `mmengine-0.8.1/mmengine/fileio/handlers/registry_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/handlers/yaml_handler.py` & `mmengine-0.8.1/mmengine/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/io.py` & `mmengine-0.8.1/mmengine/fileio/io.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/fileio/parse.py` & `mmengine-0.8.1/mmengine/fileio/parse.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/__init__.py` & `mmengine-0.8.1/mmengine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/checkpoint_hook.py` & `mmengine-0.8.1/mmengine/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/early_stopping_hook.py` & `mmengine-0.8.1/mmengine/hooks/early_stopping_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/ema_hook.py` & `mmengine-0.8.1/mmengine/hooks/ema_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/empty_cache_hook.py` & `mmengine-0.8.1/mmengine/hooks/empty_cache_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/hook.py` & `mmengine-0.8.1/mmengine/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/iter_timer_hook.py` & `mmengine-0.8.1/mmengine/hooks/iter_timer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/logger_hook.py` & `mmengine-0.8.1/mmengine/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/naive_visualization_hook.py` & `mmengine-0.8.1/mmengine/hooks/naive_visualization_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/param_scheduler_hook.py` & `mmengine-0.8.1/mmengine/hooks/param_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/profiler_hook.py` & `mmengine-0.8.1/mmengine/hooks/profiler_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/runtime_info_hook.py` & `mmengine-0.8.1/mmengine/hooks/runtime_info_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/sampler_seed_hook.py` & `mmengine-0.8.1/mmengine/hooks/sampler_seed_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/sync_buffer_hook.py` & `mmengine-0.8.1/mmengine/hooks/sync_buffer_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hooks/test_time_aug_hook.py` & `mmengine-0.8.1/mmengine/hooks/test_time_aug_hook.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hub/hub.py` & `mmengine-0.8.1/mmengine/hub/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hub/mmcls.json` & `mmengine-0.8.1/mmengine/hub/mmcls.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hub/openmmlab.json` & `mmengine-0.8.1/mmengine/hub/openmmlab.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/hub/torchvision_0.12.json` & `mmengine-0.8.1/mmengine/hub/torchvision_0.12.json`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/infer/infer.py` & `mmengine-0.8.1/mmengine/infer/infer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/logging/history_buffer.py` & `mmengine-0.8.1/mmengine/logging/history_buffer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/logging/logger.py` & `mmengine-0.8.1/mmengine/logging/logger.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/logging/message_hub.py` & `mmengine-0.8.1/mmengine/logging/message_hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/__init__.py` & `mmengine-0.8.1/mmengine/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/averaged_model.py` & `mmengine-0.8.1/mmengine/model/averaged_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/base_model/base_model.py` & `mmengine-0.8.1/mmengine/model/base_model/base_model.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/base_model/data_preprocessor.py` & `mmengine-0.8.1/mmengine/model/base_model/data_preprocessor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/base_module.py` & `mmengine-0.8.1/mmengine/model/base_module.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/test_time_aug.py` & `mmengine-0.8.1/mmengine/model/test_time_aug.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/utils.py` & `mmengine-0.8.1/mmengine/model/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/weight_init.py` & `mmengine-0.8.1/mmengine/model/weight_init.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/wrappers/__init__.py` & `mmengine-0.8.1/mmengine/model/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/wrappers/_deepspeed.py` & `mmengine-0.8.1/mmengine/model/wrappers/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/wrappers/distributed.py` & `mmengine-0.8.1/mmengine/model/wrappers/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/wrappers/fully_sharded_distributed.py` & `mmengine-0.8.1/mmengine/model/wrappers/fully_sharded_distributed.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         # Therefore we hide them in **kwargs.
         # TODO: Update when PyTorch 2.1.0 released
         if 'ignored_parameters' in kwargs:
             kwargs['ignored_parameters'] = self._get_ignored_params(
                 module, kwargs['ignored_parameters'])
 
         if 'ignored_modules' in kwargs:
-            kwargs['ignored_modules'] = self.ignored_modules(
+            kwargs['ignored_modules'] = self._get_ignored_modules(
                 module, kwargs['ignored_modules'])
 
         super().__init__(
             module=module,
             process_group=process_group,
             sharding_strategy=sharding_strategy,
             auto_wrap_policy=auto_wrap_policy,
```

### Comparing `mmengine-0.8.0/mmengine/model/wrappers/seperate_distributed.py` & `mmengine-0.8.1/mmengine/model/wrappers/seperate_distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/model/wrappers/utils.py` & `mmengine-0.8.1/mmengine/model/wrappers/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/__init__.py` & `mmengine-0.8.1/mmengine/optim/scheduler/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 # Copyright (c) OpenMMLab. All rights reserved.
-from .optimizer import (OPTIM_WRAPPER_CONSTRUCTORS, OPTIMIZERS,
-                        AmpOptimWrapper, ApexOptimWrapper, BaseOptimWrapper,
-                        DefaultOptimWrapperConstructor, OptimWrapper,
-                        OptimWrapperDict, ZeroRedundancyOptimizer,
-                        build_optim_wrapper)
 # yapf: disable
-from .scheduler import (ConstantLR, ConstantMomentum, ConstantParamScheduler,
-                        CosineAnnealingLR, CosineAnnealingMomentum,
-                        CosineAnnealingParamScheduler, ExponentialLR,
-                        ExponentialMomentum, ExponentialParamScheduler,
-                        LinearLR, LinearMomentum, LinearParamScheduler,
-                        MultiStepLR, MultiStepMomentum,
-                        MultiStepParamScheduler, OneCycleLR,
-                        OneCycleParamScheduler, PolyLR, PolyMomentum,
-                        PolyParamScheduler, ReduceOnPlateauLR,
-                        ReduceOnPlateauMomentum, ReduceOnPlateauParamScheduler,
-                        StepLR, StepMomentum, StepParamScheduler,
-                        _ParamScheduler)
+from .lr_scheduler import (ConstantLR, CosineAnnealingLR, CosineRestartLR,
+                           ExponentialLR, LinearLR, MultiStepLR, OneCycleLR,
+                           PolyLR, ReduceOnPlateauLR, StepLR)
+from .momentum_scheduler import (ConstantMomentum, CosineAnnealingMomentum,
+                                 CosineRestartMomentum, ExponentialMomentum,
+                                 LinearMomentum, MultiStepMomentum,
+                                 PolyMomentum, ReduceOnPlateauMomentum,
+                                 StepMomentum)
+from .param_scheduler import (ConstantParamScheduler,
+                              CosineAnnealingParamScheduler,
+                              CosineRestartParamScheduler,
+                              ExponentialParamScheduler, LinearParamScheduler,
+                              MultiStepParamScheduler, OneCycleParamScheduler,
+                              PolyParamScheduler,
+                              ReduceOnPlateauParamScheduler,
+                              StepParamScheduler, _ParamScheduler)
 
 # yapf: enable
 __all__ = [
-    'OPTIM_WRAPPER_CONSTRUCTORS', 'OPTIMIZERS', 'build_optim_wrapper',
-    'DefaultOptimWrapperConstructor', 'ConstantLR', 'CosineAnnealingLR',
-    'ExponentialLR', 'LinearLR', 'MultiStepLR', 'StepLR', 'ConstantMomentum',
-    'CosineAnnealingMomentum', 'ExponentialMomentum', 'LinearMomentum',
-    'MultiStepMomentum', 'StepMomentum', 'ConstantParamScheduler',
-    'CosineAnnealingParamScheduler', 'ExponentialParamScheduler',
-    'LinearParamScheduler', 'MultiStepParamScheduler', 'StepParamScheduler',
-    '_ParamScheduler', 'OptimWrapper', 'AmpOptimWrapper', 'ApexOptimWrapper',
-    'OptimWrapperDict', 'OneCycleParamScheduler', 'OneCycleLR', 'PolyLR',
-    'PolyMomentum', 'PolyParamScheduler', 'ReduceOnPlateauLR',
-    'ReduceOnPlateauMomentum', 'ReduceOnPlateauParamScheduler',
-    'ZeroRedundancyOptimizer', 'BaseOptimWrapper'
+    'ConstantLR', 'CosineAnnealingLR', 'ExponentialLR', 'LinearLR',
+    'MultiStepLR', 'StepLR', 'ConstantMomentum', 'CosineAnnealingMomentum',
+    'ExponentialMomentum', 'LinearMomentum', 'MultiStepMomentum',
+    'StepMomentum', 'ConstantParamScheduler', 'CosineAnnealingParamScheduler',
+    'ExponentialParamScheduler', 'LinearParamScheduler',
+    'MultiStepParamScheduler', 'StepParamScheduler', '_ParamScheduler',
+    'PolyParamScheduler', 'PolyLR', 'PolyMomentum', 'OneCycleParamScheduler',
+    'OneCycleLR', 'CosineRestartParamScheduler', 'CosineRestartLR',
+    'CosineRestartMomentum', 'ReduceOnPlateauParamScheduler',
+    'ReduceOnPlateauLR', 'ReduceOnPlateauMomentum'
 ]
```

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/__init__.py` & `mmengine-0.8.1/mmengine/optim/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/_deepspeed.py` & `mmengine-0.8.1/mmengine/optim/optimizer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/amp_optimizer_wrapper.py` & `mmengine-0.8.1/mmengine/optim/optimizer/amp_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/apex_optimizer_wrapper.py` & `mmengine-0.8.1/mmengine/optim/optimizer/apex_optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/base.py` & `mmengine-0.8.1/mmengine/optim/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/builder.py` & `mmengine-0.8.1/mmengine/optim/optimizer/builder.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/default_constructor.py` & `mmengine-0.8.1/mmengine/optim/optimizer/default_constructor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper.py` & `mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/optimizer_wrapper_dict.py` & `mmengine-0.8.1/mmengine/optim/optimizer/optimizer_wrapper_dict.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/optimizer/zero_optimizer.py` & `mmengine-0.8.1/mmengine/optim/optimizer/zero_optimizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/scheduler/lr_scheduler.py` & `mmengine-0.8.1/mmengine/optim/scheduler/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/scheduler/momentum_scheduler.py` & `mmengine-0.8.1/mmengine/optim/scheduler/momentum_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/optim/scheduler/param_scheduler.py` & `mmengine-0.8.1/mmengine/optim/scheduler/param_scheduler.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/registry/__init__.py` & `mmengine-0.8.1/mmengine/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/registry/build_functions.py` & `mmengine-0.8.1/mmengine/registry/build_functions.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/registry/default_scope.py` & `mmengine-0.8.1/mmengine/registry/default_scope.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/registry/registry.py` & `mmengine-0.8.1/mmengine/registry/registry.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/registry/root.py` & `mmengine-0.8.1/mmengine/registry/root.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/registry/utils.py` & `mmengine-0.8.1/mmengine/registry/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/__init__.py` & `mmengine-0.8.1/mmengine/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/_flexible_runner.py` & `mmengine-0.8.1/mmengine/runner/_flexible_runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/amp.py` & `mmengine-0.8.1/mmengine/runner/amp.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/base_loop.py` & `mmengine-0.8.1/mmengine/runner/base_loop.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/checkpoint.py` & `mmengine-0.8.1/mmengine/runner/checkpoint.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/log_processor.py` & `mmengine-0.8.1/mmengine/runner/log_processor.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/loops.py` & `mmengine-0.8.1/mmengine/runner/loops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/priority.py` & `mmengine-0.8.1/mmengine/runner/priority.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/runner.py` & `mmengine-0.8.1/mmengine/runner/runner.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/runner/utils.py` & `mmengine-0.8.1/mmengine/runner/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/structures/base_data_element.py` & `mmengine-0.8.1/mmengine/structures/base_data_element.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/structures/instance_data.py` & `mmengine-0.8.1/mmengine/structures/instance_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/structures/label_data.py` & `mmengine-0.8.1/mmengine/structures/label_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/structures/pixel_data.py` & `mmengine-0.8.1/mmengine/structures/pixel_data.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/testing/__init__.py` & `mmengine-0.8.1/mmengine/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/testing/_internal/distributed.py` & `mmengine-0.8.1/mmengine/testing/_internal/distributed.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/testing/compare.py` & `mmengine-0.8.1/mmengine/testing/compare.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/testing/runner_test_case.py` & `mmengine-0.8.1/mmengine/testing/runner_test_case.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/__init__.py` & `mmengine-0.8.1/mmengine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/__init__.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/collect_env.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/hub.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/hub.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/misc.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/parrots_wrapper.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/parrots_wrapper.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/setup_env.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/setup_env.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/time_counter.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/time_counter.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/torch_ops.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/torch_ops.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/trace.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/trace.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/dl_utils/visualize.py` & `mmengine-0.8.1/mmengine/utils/dl_utils/visualize.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/manager.py` & `mmengine-0.8.1/mmengine/utils/manager.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/misc.py` & `mmengine-0.8.1/mmengine/utils/misc.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/package_utils.py` & `mmengine-0.8.1/mmengine/utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/path.py` & `mmengine-0.8.1/mmengine/utils/path.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/progressbar.py` & `mmengine-0.8.1/mmengine/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/timer.py` & `mmengine-0.8.1/mmengine/utils/timer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/utils/version_utils.py` & `mmengine-0.8.1/mmengine/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/version.py` & `mmengine-0.8.1/mmengine/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) OpenMMLab. All rights reserved.
 
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 
 def parse_version_info(version_str):
     """Parse the version information.
 
     Args:
         version_str (str): version string like '0.1.0'.
```

### Comparing `mmengine-0.8.0/mmengine/visualization/utils.py` & `mmengine-0.8.1/mmengine/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/visualization/vis_backend.py` & `mmengine-0.8.1/mmengine/visualization/vis_backend.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine/visualization/visualizer.py` & `mmengine-0.8.1/mmengine/visualization/visualizer.py`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/mmengine.egg-info/PKG-INFO` & `mmengine-0.8.1/mmengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmengine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Engine of OpenMMLab projects
 Home-page: https://github.com/open-mmlab/mmengine
 Author: MMEngine Authors
 Author-email: openmmlab@gmail.com
 License: UNKNOWN
 Description: <div align="center">
           <img src="https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-429b-9354-c6fac64b7ef8.jpg" width="600"/>
@@ -66,15 +66,15 @@
         
         ## What's New
         
         v0.8.0 was released on 2023-06-30.
         
         Highlights:
         
-        - Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [example](https://github.com/open-mmlab/mmengine/blob/main/examples/distributed_training_with_flexible_runner.py) for more detailed usages.
+        - Support training with [FSDP](https://pytorch.org/tutorials/intermediate/FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://www.deepspeed.ai/). Refer to the [Training Large Models](https://mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for more detailed usages.
         
         - Introduce the pure Python style configuration file:
         
           - Support navigating to base configuration file in IDE
           - Support navigating to base variable in IDE
           - Support navigating to source code of class in IDE
           - Support inheriting two configuration files containing the same field
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mmengine Version: 0.8.0 Summary: Engine of
+Metadata-Version: 2.1 Name: mmengine Version: 0.8.1 Summary: Engine of
 OpenMMLab projects Home-page: https://github.com/open-mmlab/mmengine Author:
 MMEngine Authors Author-email: openmmlab@gmail.com License: UNKNOWN
 Description:
  [https://user-images.githubusercontent.com/58739961/187154444-fce76639-ac8d-
                           429b-9354-c6fac64b7ef8.jpg]
                                         
            OpenMMLab website HOT      OpenMMLab platform TRY_IT_OUT
@@ -20,16 +20,16 @@
   get_started/installation.html) | [ð¤Reporting Issues](https://github.com/
                     open-mmlab/mmengine/issues/new/choose)
                    English | [ç®ä½ä¸­æ](README_zh-CN.md)
 
 ## What's New v0.8.0 was released on 2023-06-30. Highlights: - Support training
 with [FSDP](https://pytorch.org/tutorials/intermediate/
 FSDP_adavnced_tutorial.html?highlight=fsdp) and [DeepSpeed](https://
-www.deepspeed.ai/). Refer to the [example](https://github.com/open-mmlab/
-mmengine/blob/main/examples/distributed_training_with_flexible_runner.py) for
+www.deepspeed.ai/). Refer to the [Training Large Models](https://
+mmengine.readthedocs.io/en/latest/common_usage/large_model_training.html) for
 more detailed usages. - Introduce the pure Python style configuration file: -
 Support navigating to base configuration file in IDE - Support navigating to
 base variable in IDE - Support navigating to source code of class in IDE -
 Support inheriting two configuration files containing the same field - Load the
 configuration file without other third-party requirements Refer to the
 [tutorial](https://mmengine.readthedocs.io/en/latest/advanced_tutorials/
 config.html#a-pure-python-style-configuration-file-beta) for more detailed
```

### Comparing `mmengine-0.8.0/mmengine.egg-info/SOURCES.txt` & `mmengine-0.8.1/mmengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmengine-0.8.0/setup.py` & `mmengine-0.8.1/setup.py`

 * *Files identical despite different names*

