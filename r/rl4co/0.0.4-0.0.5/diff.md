# Comparing `tmp/rl4co-0.0.4.tar.gz` & `tmp/rl4co-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl4co-0.0.4.tar", last modified: Tue Jul  4 17:10:46 2023, max compression
+gzip compressed data, was "rl4co-0.0.5.tar", last modified: Thu Jul  6 13:47:23 2023, max compression
```

## Comparing `rl4co-0.0.4.tar` & `rl4co-0.0.5.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.976010 rl4co-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-04 17:10:36.000000 rl4co-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-04 17:10:46.976010 rl4co-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-04 17:10:36.000000 rl4co-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-04 17:10:36.000000 rl4co-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/envs/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/atsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/envs/common/
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/common/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/cvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/dpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/ffsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/mdpp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/mtsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/op.py
--rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/pctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/pdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/sdvrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/spctsp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/envs/tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/nn/
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/env_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/env_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/flash_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/nn/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/graph/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/graph/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/graph/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.960010 rl4co-0.0.4/rl4co/models/rl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/rl/ppo/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/ppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/ppo/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/rl/reinforce/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/reinforce/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/reinforce/baselines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/rl/reinforce/critic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.960010 rl4co-0.0.4/rl4co/models/zoo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/am/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/am/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/amppo/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/amppo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/amppo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/amppo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/ham/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ham/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/mdam/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/mdam/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.968011 rl4co-0.0.4/rl4co/models/zoo/pomo/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/pomo/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/models/zoo/ptrnet/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/ptrnet/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/models/zoo/symnco/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/models/zoo/symnco/policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/tasks/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/tasks/rl4co.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/callbacks/speed_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.972010 rl4co-0.0.4/rl4co/utils/download/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/download/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/instantiators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/param_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-04 17:10:36.000000 rl4co-0.0.4/rl4co/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.964010 rl4co-0.0.4/rl4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-04 17:10:46.000000 rl4co-0.0.4/rl4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 17:10:46.976010 rl4co-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 17:10:46.976010 rl4co-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-04 17:10:36.000000 rl4co-0.0.4/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-04 17:10:36.000000 rl4co-0.0.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-04 17:10:36.000000 rl4co-0.0.4/tests/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.122796 rl4co-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-06 13:47:13.000000 rl4co-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-06 13:47:23.122796 rl4co-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-07-06 13:47:13.000000 rl4co-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-06 13:47:13.000000 rl4co-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12329 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8078 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/atsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/envs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/cvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/dpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/ffsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/mdpp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/mtsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13562 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/pctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10231 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/pdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/sdvrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/spctsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/envs/tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/models/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/env_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/env_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/flash_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.110796 rl4co-0.0.5/rl4co/models/nn/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/graph/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/graph/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/graph/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co/models/rl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/rl/ppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/ppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/ppo/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/rl/reinforce/
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/reinforce/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/reinforce/baselines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/rl/reinforce/critic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co/models/zoo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/am/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/am/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/amppo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/amppo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/amppo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/amppo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/ham/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18979 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ham/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/mdam/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12120 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/mdam/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.114796 rl4co-0.0.5/rl4co/models/zoo/pomo/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/pomo/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/models/zoo/ptrnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/ptrnet/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/models/zoo/symnco/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/models/zoo/symnco/policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/tasks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8790 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/tasks/rl4co.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.118796 rl4co-0.0.5/rl4co/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/callbacks/speed_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.122796 rl4co-0.0.5/rl4co/utils/download/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/download/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/param_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-06 13:47:13.000000 rl4co-0.0.5/rl4co/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.106796 rl4co-0.0.5/rl4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21176 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 13:47:23.000000 rl4co-0.0.5/rl4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:47:23.122796 rl4co-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:47:23.122796 rl4co-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-06 13:47:13.000000 rl4co-0.0.5/tests/test_envs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-06 13:47:13.000000 rl4co-0.0.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-06 13:47:13.000000 rl4co-0.0.5/tests/test_ops.py
```

### Comparing `rl4co-0.0.4/LICENSE` & `rl4co-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/PKG-INFO` & `rl4co-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.4
+Version: 0.0.5
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rl4co-0.0.4/README.md` & `rl4co-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/pyproject.toml` & `rl4co-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/data/dataset.py` & `rl4co-0.0.5/rl4co/data/dataset.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/data/generate_data.py` & `rl4co-0.0.5/rl4co/data/generate_data.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/data/utils.py` & `rl4co-0.0.5/rl4co/data/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/atsp.py` & `rl4co-0.0.5/rl4co/envs/atsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/common/base.py` & `rl4co-0.0.5/rl4co/envs/common/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/common/utils.py` & `rl4co-0.0.5/rl4co/envs/common/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/cvrp.py` & `rl4co-0.0.5/rl4co/envs/cvrp.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,15 @@
                     "reward": reward,
                     "done": done,
                 }
             },
             td.shape,
         )
         td_step["next"].set("action_mask", self.get_action_mask(td_step["next"]))
-        return td_step     
+        return td_step
 
     def _reset(
         self,
         td: Optional[TensorDict] = None,
         batch_size: Optional[list] = None,
     ) -> TensorDict:
         if batch_size is None:
@@ -137,37 +137,45 @@
         self.device = td.device
 
         # Create reset TensorDict
         td_reset = TensorDict(
             {
                 "locs": torch.cat((td["depot"][:, None, :], td["locs"]), -2),
                 "demand": td["demand"],
-                "current_node": torch.zeros(*batch_size, 1, dtype=torch.long, device=self.device),
-                "used_capacity":  torch.zeros((*batch_size, 1), device=self.device),
-                "vehicle_capacity": torch.full((*batch_size, 1), self.vehicle_capacity, device=self.device),
-                "visited": torch.zeros((*batch_size, 1, td["locs"].shape[-2] + 1), dtype=torch.uint8, device=self.device),
+                "current_node": torch.zeros(
+                    *batch_size, 1, dtype=torch.long, device=self.device
+                ),
+                "used_capacity": torch.zeros((*batch_size, 1), device=self.device),
+                "vehicle_capacity": torch.full(
+                    (*batch_size, 1), self.vehicle_capacity, device=self.device
+                ),
+                "visited": torch.zeros(
+                    (*batch_size, 1, td["locs"].shape[-2] + 1),
+                    dtype=torch.uint8,
+                    device=self.device,
+                ),
             },
             batch_size=batch_size,
         )
         td_reset.set("action_mask", self.get_action_mask(td_reset))
         return td_reset
-    
+
     @staticmethod
     def get_action_mask(td: TensorDict) -> torch.Tensor:
         # For demand steps_dim is inserted by indexing with id, for used_capacity insert node dim for broadcasting
         exceeds_cap = td["demand"][:, None, :] + td["used_capacity"][..., None] > 1.0
 
         # Nodes that cannot be visited are already visited or too much demand to be served now
         mask_loc = td["visited"][..., 1:].to(exceeds_cap.dtype) | exceeds_cap
 
         # Cannot visit the depot if just visited and still unserved nodes
         mask_depot = (td["current_node"] == 0) & ((mask_loc == 0).int().sum(-1) > 0)
         return ~torch.cat((mask_depot[..., None], mask_loc), -1).squeeze(-2)
 
-    def get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:        
+    def get_reward(self, td: TensorDict, actions: TensorDict) -> TensorDict:
         # Check that the solution is valid
         if self.check_solution:
             self.check_solution_validity(td, actions)
 
         # Gather dataset in order of tour
         depot = td["locs"][..., 0:1, :]
         locs_ordered = torch.cat([depot, gather_by_index(td["locs"], actions)], dim=1)
@@ -307,15 +315,15 @@
 
         td = td.detach().cpu()
         # if batch_size greater than 0 , we need to select the first batch element
         if td.batch_size != torch.Size([]):
             td = td[0]
 
         locs = td["locs"]
-        scale = CAPACITIES.get(td['locs'].size(-2)-1, 1)
+        scale = CAPACITIES.get(td["locs"].size(-2) - 1, 1)
         demands = td["demand"] * scale
 
         if actions is None:
             actions = td.get("action", None)
 
         # add the depot at the first action and the end action
         actions = torch.cat([torch.tensor([0]), actions, torch.tensor([0])])
@@ -355,15 +363,15 @@
 
         # plot demand bars
         for node_idx in range(1, len(locs)):
             ax.add_patch(
                 plt.Rectangle(
                     (locs[node_idx, 0] - 0.005, locs[node_idx, 1] + 0.015),
                     0.01,
-                    demands[node_idx - 1]/(scale * 10),
+                    demands[node_idx - 1] / (scale * 10),
                     edgecolor=cm.Set2(0),
                     facecolor=cm.Set2(0),
                     fill=True,
                 )
             )
 
         # text demand
@@ -407,20 +415,11 @@
                 xy=(to_loc[0], to_loc[1]),
                 xytext=(from_loc[0], from_loc[1]),
                 arrowprops=dict(arrowstyle="-|>", color=out(color_idx)),
                 size=15,
                 annotation_clip=False,
             )
 
-        # setup
+        # Setup limits and show
         ax.set_xlim(-0.05, 1.05)
         ax.set_ylim(-0.05, 1.05)
-
-        # Set plot title and axis labels
-        title_font = {"fontsize": 14}
-        label_font = {"fontsize": 12}
-        ax.set_title("CVRP Solution", fontdict=title_font)
-        ax.set_xlabel("X Coordinate", fontdict=label_font)
-        ax.set_ylabel("Y Coordinate", fontdict=label_font)
-
-        # plt.tight_layout()
         plt.show()
```

### Comparing `rl4co-0.0.4/rl4co/envs/dpp.py` & `rl4co-0.0.5/rl4co/envs/dpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/ffsp.py` & `rl4co-0.0.5/rl4co/envs/ffsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/mdpp.py` & `rl4co-0.0.5/rl4co/envs/mdpp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/mtsp.py` & `rl4co-0.0.5/rl4co/envs/mtsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/op.py` & `rl4co-0.0.5/rl4co/envs/op.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/pctsp.py` & `rl4co-0.0.5/rl4co/envs/pctsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/pdp.py` & `rl4co-0.0.5/rl4co/envs/pdp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/sdvrp.py` & `rl4co-0.0.5/rl4co/envs/sdvrp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/spctsp.py` & `rl4co-0.0.5/rl4co/envs/spctsp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/envs/tsp.py` & `rl4co-0.0.5/rl4co/envs/tsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,12 +203,11 @@
 
         # Add arrows between visited nodes as a quiver plot
         dx, dy = np.diff(x), np.diff(y)
         ax.quiver(
             x[:-1], y[:-1], dx, dy, scale_units="xy", angles="xy", scale=1, color="k"
         )
 
-        # Set plot title and axis labels
-        ax.set_title("TSP Solution")
-        ax.set_xlabel("x-coordinate")
-        ax.set_ylabel("y-coordinate")
+        # Setup limits and show
+        ax.set_xlim(-0.05, 1.05)
+        ax.set_ylim(-0.05, 1.05)
         plt.show()
```

### Comparing `rl4co-0.0.4/rl4co/models/nn/attention.py` & `rl4co-0.0.5/rl4co/models/nn/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/env_context.py` & `rl4co-0.0.5/rl4co/models/nn/env_context.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/env_embedding.py` & `rl4co-0.0.5/rl4co/models/nn/env_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
 class SDVRPDynamicEmbedding(nn.Module):
     def __init__(self, embedding_dim):
         super(SDVRPDynamicEmbedding, self).__init__()
         self.projection = nn.Linear(1, 3 * embedding_dim, bias=False)
 
     def forward(self, td):
-        demands_with_depot = td["demand"][..., None].clone()
+        demands_with_depot = td["demand_with_depot"][..., None].clone()
         demands_with_depot[..., 0, :] = 0
         glimpse_key_dynamic, glimpse_val_dynamic, logit_key_dynamic = self.projection(
             demands_with_depot
         ).chunk(3, dim=-1)
         return glimpse_key_dynamic, glimpse_val_dynamic, logit_key_dynamic
```

### Comparing `rl4co-0.0.4/rl4co/models/nn/flash_attention.py` & `rl4co-0.0.5/rl4co/models/nn/flash_attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/graph/gat.py` & `rl4co-0.0.5/rl4co/models/nn/graph/gat.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/graph/gcn.py` & `rl4co-0.0.5/rl4co/models/nn/graph/gcn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/graph/mpnn.py` & `rl4co-0.0.5/rl4co/models/nn/graph/mpnn.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/mlp.py` & `rl4co-0.0.5/rl4co/models/nn/mlp.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/ops.py` & `rl4co-0.0.5/rl4co/models/nn/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/nn/utils.py` & `rl4co-0.0.5/rl4co/models/nn/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,7 +49,19 @@
 
 
 def random_policy(td):
     """Helper function to select a random action from available actions"""
     action = torch.multinomial(td["action_mask"].float(), 1).squeeze(-1)
     td.set("action", action)
     return td
+
+
+def rollout(env, td, policy):
+    """Helper function to rollout a policy. Currently, TorchRL does not allow to step
+    over envs when done with `env.rollout()`. We need this because for environements that complete at different steps.
+    """
+    actions = []
+    while not td["done"].all():
+        td = policy(td)
+        actions.append(td["action"])
+        td = env.step(td)["next"]
+    return env.get_reward(td, torch.stack(actions, dim=1))
```

### Comparing `rl4co-0.0.4/rl4co/models/rl/ppo/model.py` & `rl4co-0.0.5/rl4co/models/rl/ppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/rl/ppo/task.py` & `rl4co-0.0.5/rl4co/models/rl/ppo/task.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/rl/reinforce/base.py` & `rl4co-0.0.5/rl4co/models/rl/reinforce/base.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/rl/reinforce/baselines.py` & `rl4co-0.0.5/rl4co/models/rl/reinforce/baselines.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/rl/reinforce/critic.py` & `rl4co-0.0.5/rl4co/models/rl/reinforce/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/am/decoder.py` & `rl4co-0.0.5/rl4co/models/zoo/am/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/am/model.py` & `rl4co-0.0.5/rl4co/models/zoo/am/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/am/policy.py` & `rl4co-0.0.5/rl4co/models/zoo/am/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/amppo/decoder.py` & `rl4co-0.0.5/rl4co/models/zoo/amppo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/amppo/model.py` & `rl4co-0.0.5/rl4co/models/zoo/amppo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/amppo/policy.py` & `rl4co-0.0.5/rl4co/models/zoo/amppo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ham/attention.py` & `rl4co-0.0.5/rl4co/models/zoo/ham/attention.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ham/encoder.py` & `rl4co-0.0.5/rl4co/models/zoo/ham/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ham/model.py` & `rl4co-0.0.5/rl4co/models/zoo/ham/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ham/policy.py` & `rl4co-0.0.5/rl4co/models/zoo/ham/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/mdam/decoder.py` & `rl4co-0.0.5/rl4co/models/zoo/mdam/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/mdam/encoder.py` & `rl4co-0.0.5/rl4co/models/zoo/mdam/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/mdam/model.py` & `rl4co-0.0.5/rl4co/models/zoo/mdam/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/mdam/policy.py` & `rl4co-0.0.5/rl4co/models/zoo/mdam/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/pomo/augmentations.py` & `rl4co-0.0.5/rl4co/models/zoo/pomo/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/pomo/decoder.py` & `rl4co-0.0.5/rl4co/models/zoo/pomo/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/pomo/model.py` & `rl4co-0.0.5/rl4co/models/zoo/pomo/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/pomo/policy.py` & `rl4co-0.0.5/rl4co/models/zoo/pomo/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ptrnet/critic.py` & `rl4co-0.0.5/rl4co/models/zoo/ptrnet/critic.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ptrnet/decoder.py` & `rl4co-0.0.5/rl4co/models/zoo/ptrnet/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ptrnet/encoder.py` & `rl4co-0.0.5/rl4co/models/zoo/ptrnet/encoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ptrnet/model.py` & `rl4co-0.0.5/rl4co/models/zoo/ptrnet/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/ptrnet/policy.py` & `rl4co-0.0.5/rl4co/models/zoo/ptrnet/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/symnco/augmentations.py` & `rl4co-0.0.5/rl4co/models/zoo/symnco/augmentations.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/symnco/decoder.py` & `rl4co-0.0.5/rl4co/models/zoo/symnco/decoder.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/symnco/losses.py` & `rl4co-0.0.5/rl4co/models/zoo/symnco/losses.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/symnco/model.py` & `rl4co-0.0.5/rl4co/models/zoo/symnco/model.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/models/zoo/symnco/policy.py` & `rl4co-0.0.5/rl4co/models/zoo/symnco/policy.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/tasks/eval.py` & `rl4co-0.0.5/rl4co/tasks/eval.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/tasks/rl4co.py` & `rl4co-0.0.5/rl4co/tasks/rl4co.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/callbacks/speed_monitor.py` & `rl4co-0.0.5/rl4co/utils/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/download/downloader.py` & `rl4co-0.0.5/rl4co/utils/download/downloader.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/download/gdrive.py` & `rl4co-0.0.5/rl4co/utils/download/gdrive.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/download/s3.py` & `rl4co-0.0.5/rl4co/utils/download/s3.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/helpers.py` & `rl4co-0.0.5/rl4co/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/instantiators.py` & `rl4co-0.0.5/rl4co/utils/instantiators.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/lightning.py` & `rl4co-0.0.5/rl4co/utils/lightning.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/logging_utils.py` & `rl4co-0.0.5/rl4co/utils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/ops.py` & `rl4co-0.0.5/rl4co/utils/ops.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/param_grouping.py` & `rl4co-0.0.5/rl4co/utils/param_grouping.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/pylogger.py` & `rl4co-0.0.5/rl4co/utils/pylogger.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/rich_utils.py` & `rl4co-0.0.5/rl4co/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/test_utils.py` & `rl4co-0.0.5/rl4co/utils/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,45 @@
 from torch.utils.data import DataLoader
 
 from rl4co.data.dataset import tensordict_collate_fn
-from rl4co.envs import CVRPEnv, DPPEnv, MTSPEnv, OPEnv, PCTSPEnv, PDPEnv, SDVRPEnv, TSPEnv
+from rl4co.envs import (
+    CVRPEnv,
+    DPPEnv,
+    MDPPEnv,
+    MTSPEnv,
+    OPEnv,
+    PCTSPEnv,
+    PDPEnv,
+    SDVRPEnv,
+    SPCTSPEnv,
+    TSPEnv,
+)
 
 
 def get_env(name, size):
     if name == "tsp":
         env = TSPEnv(num_loc=size)
     elif name == "cvrp":
         env = CVRPEnv(num_loc=size)
     elif name == "sdvrp":
         env = SDVRPEnv(num_loc=size)
-    elif name == "dpp":
-        env = DPPEnv()
     elif name == "pdp":
         env = PDPEnv(num_loc=size)
     elif name == "op":
         env = OPEnv(num_loc=size)
     elif name == "mtsp":
         env = MTSPEnv(num_loc=size)
     elif name == "pctsp":
         env = PCTSPEnv(num_loc=size)
+    elif name == "spctsp":
+        env = SPCTSPEnv(num_loc=size)
+    elif name == "dpp":
+        env = DPPEnv()
+    elif name == "mdpp":
+        env = MDPPEnv()
     else:
         raise ValueError(f"Unknown env_name: {name}")
 
     return env.transform()
 
 
 def generate_env_data(env, size, batch_size):
```

### Comparing `rl4co-0.0.4/rl4co/utils/transfer.py` & `rl4co-0.0.5/rl4co/utils/transfer.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co/utils/utils.py` & `rl4co-0.0.5/rl4co/utils/utils.py`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/rl4co.egg-info/PKG-INFO` & `rl4co-0.0.5/rl4co.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl4co
-Version: 0.0.4
+Version: 0.0.5
 Summary: RL4CO: an Extensive Reinforcement Learning for Combinatorial Optimization Benchmark
 Author-email: Federico Berto <berto.federico2@gmail.com>, Chuanbo Hua <cbhua@kaist.ac.kr>, Junyoung Park <junyoungpark.ml@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `rl4co-0.0.4/rl4co.egg-info/SOURCES.txt` & `rl4co-0.0.5/rl4co.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rl4co-0.0.4/tests/test_envs.py` & `rl4co-0.0.5/tests/test_envs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,53 @@
 import pytest
-import torch
 
 from rl4co.envs import ATSPEnv, CVRPEnv, DPPEnv, MTSPEnv, PDPEnv, SDVRPEnv, TSPEnv
-
-
-def policy(td):
-    """Helper function to select a random action from available actions"""
-    action = torch.multinomial(td["action_mask"].float(), 1).squeeze(-1)
-    td.set("action", action)
-    return td
-
-
-def rollout(env, td, policy):
-    """Helper function to rollout a policy"""
-    actions = []
-    while not td["done"].all():
-        td = policy(td)
-        actions.append(td["action"])
-        td = env.step(td)["next"]
-    return env.get_reward(td, torch.stack(actions, dim=1))
+from rl4co.models.nn.utils import random_policy, rollout
 
 
 @pytest.mark.parametrize("size, batch_size", [(20, 2)])
 def test_tsp(size, batch_size):
     env = TSPEnv(num_loc=size)
-    reward = rollout(env, env.reset(batch_size=[batch_size]), policy)
+    reward = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("size, batch_size", [(20, 2)])
 def test_atsp(size, batch_size):
     env = ATSPEnv(num_loc=size)
-    reward = rollout(env, env.reset(batch_size=[batch_size]), policy)
+    reward = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("size, batch_size", [(20, 2)])
 def test_dpp(size, batch_size):
     env = DPPEnv()
-    reward = rollout(env, env.reset(batch_size=[batch_size]), policy)
+    reward = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("size, batch_size", [(20, 2)])
 def test_cvrp(size, batch_size):
     env = CVRPEnv()
-    reward = rollout(env, env.reset(batch_size=[batch_size]), policy)
+    reward = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("size, batch_size", [(20, 2)])
 def test_sdvrp(size, batch_size):
     env = SDVRPEnv()
-    reward = rollout(env, env.reset(batch_size=[batch_size]), policy)
+    reward = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("size, batch_size", [(20, 2)])
 def test_pdp(size, batch_size):
     env = PDPEnv(num_loc=size)
-    reward = rollout(env, env.reset(batch_size=[batch_size]), policy)
+    reward = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
     assert reward.shape == (batch_size,)
 
 
 @pytest.mark.parametrize("size, batch_size", [(20, 2)])
 def test_mtsp(size, batch_size):
     env = MTSPEnv(num_loc=size)
-    reward = rollout(env, env.reset(batch_size=[batch_size]), policy)
+    reward = rollout(env, env.reset(batch_size=[batch_size]), random_policy)
     assert reward.shape == (batch_size,)
```

### Comparing `rl4co-0.0.4/tests/test_models.py` & `rl4co-0.0.5/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import sys
-
-sys.path.append(".")
 import pytest
 
 from rl4co.models import (
     POMO,
     AttentionModel,
     HeterogeneousAttentionModel,
     MDAMPolicy,
@@ -13,15 +10,15 @@
     SymNCOPolicy,
 )
 from rl4co.utils.test_utils import generate_env_data
 
 
 @pytest.mark.parametrize("size", [20])
 @pytest.mark.parametrize(
-    "env_name", ["tsp", "cvrp", "mtsp", "op", "dpp", "pctsp"]
+    "env_name", ["tsp", "cvrp", "sdvrp", "mtsp", "op", "pctsp", "spctsp", "dpp", "mdpp"]
 )  # todo: sdvrp
 def test_am(size, env_name, batch_size=2):
     env, x = generate_env_data(env_name, size, batch_size)
     td = env.reset(x)
     model = AttentionModel(env)
     out = model(td, decode_type="sampling")
     assert out["reward"].shape == (batch_size,)
```

### Comparing `rl4co-0.0.4/tests/test_ops.py` & `rl4co-0.0.5/tests/test_ops.py`

 * *Files identical despite different names*

