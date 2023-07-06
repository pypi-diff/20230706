# Comparing `tmp/salesforce-codetf-1.0.2.1.tar.gz` & `tmp/salesforce-codetf-1.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salesforce-codetf-1.0.2.1.tar", last modified: Thu Jul  6 08:02:00 2023, max compression
+gzip compressed data, was "salesforce-codetf-1.0.2.2.tar", last modified: Thu Jul  6 08:16:33 2023, max compression
```

## Comparing `salesforce-codetf-1.0.2.1.tar` & `salesforce-codetf-1.0.2.2.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:02:00.491470 salesforce-codetf-1.0.2.1/
--rw-r--r--   0 root         (0) root         (0)    11411 2023-05-22 01:09:51.000000 salesforce-codetf-1.0.2.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    23459 2023-07-06 08:02:00.492470 salesforce-codetf-1.0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23054 2023-06-28 09:19:40.000000 salesforce-codetf-1.0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.413311 salesforce-codetf-1.0.2.1/codetf/
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.450314 salesforce-codetf-1.0.2.1/codetf/code_utility/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.469315 salesforce-codetf-1.0.2.1/codetf/code_utility/apex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/apex/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5146 2023-05-22 05:30:29.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/apex/apex_code_utility.py
--rw-r--r--   0 root         (0) root         (0)     5116 2023-05-22 10:01:52.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/ast_parser.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/base_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.487316 salesforce-codetf-1.0.2.1/codetf/code_utility/java/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/java/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/java/java_code_utility.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/language_specific_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.506318 salesforce-codetf-1.0.2.1/codetf/code_utility/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.1/codetf/code_utility/python/python_code_utility.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.534320 salesforce-codetf-1.0.2.1/codetf/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 07:54:40.000000 salesforce-codetf-1.0.2.1/codetf/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5677 2023-05-22 22:51:11.000000 salesforce-codetf-1.0.2.1/codetf/common/registry.py
--rw-r--r--   0 root         (0) root         (0)    14084 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/common/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.552321 salesforce-codetf-1.0.2.1/codetf/configs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.1/codetf/configs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.563322 salesforce-codetf-1.0.2.1/codetf/configs/dataset/
--rw-r--r--   0 root         (0) root         (0)      328 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.1/codetf/configs/dataset/dataset.yaml
--rw-r--r--   0 root         (0) root         (0)      131 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/configs/default.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.605325 salesforce-codetf-1.0.2.1/codetf/configs/inference/
--rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 09:11:25.000000 salesforce-codetf-1.0.2.1/codetf/configs/inference/bert.yaml
--rw-r--r--   0 root         (0) root         (0)     2852 2023-05-29 19:15:11.000000 salesforce-codetf-1.0.2.1/codetf/configs/inference/causal_lm.yaml
--rw-r--r--   0 root         (0) root         (0)     5094 2023-06-19 21:11:58.000000 salesforce-codetf-1.0.2.1/codetf/configs/inference/codet5.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.626327 salesforce-codetf-1.0.2.1/codetf/configs/training/
--rw-r--r--   0 root         (0) root         (0)      766 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.1/codetf/configs/training/causal_lm.yaml
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-19 20:22:57.000000 salesforce-codetf-1.0.2.1/codetf/configs/training/codet5.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.718334 salesforce-codetf-1.0.2.1/codetf/data_utility/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-06-19 18:30:44.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/apps_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-05-22 05:34:12.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/base_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-06-19 20:30:20.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/codexglue_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-06 08:10:48.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/human_eval_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1111 2023-06-19 18:30:44.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/mpp_dataset.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 07:39:56.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/stackexchange_instruction_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.1/codetf/data_utility/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.754337 salesforce-codetf-1.0.2.1/codetf/models/
--rw-r--r--   0 root         (0) root         (0)     3494 2023-05-29 19:06:10.000000 salesforce-codetf-1.0.2.1/codetf/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2311 2023-06-19 20:44:49.000000 salesforce-codetf-1.0.2.1/codetf/models/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.765338 salesforce-codetf-1.0.2.1/codetf/models/bert_models/
--rw-r--r--   0 root         (0) root         (0)     3681 2023-06-27 14:58:24.000000 salesforce-codetf-1.0.2.1/codetf/models/bert_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.776338 salesforce-codetf-1.0.2.1/codetf/models/causal_lm_models/
--rw-r--r--   0 root         (0) root         (0)     4098 2023-06-28 19:36:14.000000 salesforce-codetf-1.0.2.1/codetf/models/causal_lm_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.787339 salesforce-codetf-1.0.2.1/codetf/models/seq2seq_models/
--rw-r--r--   0 root         (0) root         (0)     5919 2023-06-27 14:58:07.000000 salesforce-codetf-1.0.2.1/codetf/models/seq2seq_models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.816341 salesforce-codetf-1.0.2.1/codetf/performance/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.1/codetf/performance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-06-14 10:17:09.000000 salesforce-codetf-1.0.2.1/codetf/performance/evaluation_metric.py
--rw-r--r--   0 root         (0) root         (0)     3440 2023-06-14 10:17:10.000000 salesforce-codetf-1.0.2.1/codetf/performance/model_evaluator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:58.309303 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:01:59.488393 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/
--rwxr-xr-x   0 root         (0) root         (0)   623752 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/apex.so
--rw-r--r--   0 root         (0) root         (0)   517568 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/bash.so
--rw-r--r--   0 root         (0) root         (0)   361144 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/c.so
--rw-r--r--   0 root         (0) root         (0)  3032464 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/c_sharp.so
--rw-r--r--   0 root         (0) root         (0)  1217512 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/cpp.so
--rw-r--r--   0 root         (0) root         (0)    99680 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/css.so
--rw-r--r--   0 root         (0) root         (0)   236232 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/elm.so
--rw-r--r--   0 root         (0) root         (0)   230128 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/go.so
--rw-r--r--   0 root         (0) root         (0)  8532424 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/haskell.so
--rw-r--r--   0 root         (0) root         (0)   149608 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/html.so
--rw-r--r--   0 root         (0) root         (0)   262848 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/java.so
--rw-r--r--   0 root         (0) root         (0)   280160 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/javascript.so
--rw-r--r--   0 root         (0) root         (0)  4604424 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/kotlin.so
--rw-r--r--   0 root         (0) root         (0)   198688 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/lua.so
--rw-r--r--   0 root         (0) root         (0)   432360 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/php.so
--rw-r--r--   0 root         (0) root         (0)   254160 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/python.so
--rw-r--r--   0 root         (0) root         (0)  1098880 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/ruby.so
--rw-r--r--   0 root         (0) root         (0)   804520 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/rust.so
--rw-r--r--   0 root         (0) root         (0)   263848 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/scala.so
--rw-r--r--   0 root         (0) root         (0)   590536 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/solidity.so
--rwxr-xr-x   0 root         (0) root         (0)   164488 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/soql.so
--rwxr-xr-x   0 root         (0) root         (0)   180872 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/sosl.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:02:00.246451 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/
--rwxr-xr-x   0 root         (0) root         (0)   533096 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/apex.so
--rw-r--r--   0 root         (0) root         (0)   160688 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/asm.so
--rw-r--r--   0 root         (0) root         (0)   704688 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/bash.so
--rw-r--r--   0 root         (0) root         (0)   442184 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/c.so
--rw-r--r--   0 root         (0) root         (0)  3112856 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/c_sharp.so
--rw-r--r--   0 root         (0) root         (0)  1512216 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/cpp.so
--rw-r--r--   0 root         (0) root         (0)   137144 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/css.so
--rw-r--r--   0 root         (0) root         (0)   442568 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/elm.so
--rw-r--r--   0 root         (0) root         (0)   301056 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/go.so
--rw-r--r--   0 root         (0) root         (0)  4731648 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/haskell.so
--rw-r--r--   0 root         (0) root         (0)   950536 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/html.so
--rw-r--r--   0 root         (0) root         (0)   315720 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/java.so
--rw-r--r--   0 root         (0) root         (0)   343560 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/javascript.so
--rw-r--r--   0 root         (0) root         (0)  4924440 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/kotlin.so
--rw-r--r--   0 root         (0) root         (0)   234240 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/lua.so
--rw-r--r--   0 root         (0) root         (0)   623208 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/php.so
--rw-r--r--   0 root         (0) root         (0)   352352 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/python.so
--rw-r--r--   0 root         (0) root         (0)  1364728 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/ruby.so
--rw-r--r--   0 root         (0) root         (0)   902504 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/rust.so
--rw-r--r--   0 root         (0) root         (0)   309752 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/scala.so
--rw-r--r--   0 root         (0) root         (0)   727704 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/solidity.so
--rwxr-xr-x   0 root         (0) root         (0)   127040 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/soql.so
--rwxr-xr-x   0 root         (0) root         (0)   139328 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/sosl.so
--rw-r--r--   0 root         (0) root         (0) 18164400 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/verilog.so
--rw-r--r--   0 root         (0) root         (0)   445224 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/yaml.so
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:02:00.321457 salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23459 2023-07-06 08:01:57.000000 salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4215 2023-07-06 08:01:58.000000 salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       96 2023-07-06 08:01:58.000000 salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 19:37:41.000000 salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      354 2023-07-06 08:01:58.000000 salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-06 08:01:58.000000 salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-06 08:02:00.500470 salesforce-codetf-1.0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1653 2023-07-06 07:55:58.000000 salesforce-codetf-1.0.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:02:00.388462 salesforce-codetf-1.0.2.1/test_code_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.1/test_code_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.1/test_code_utilities/test_extract_code_attributes.py
--rw-r--r--   0 root         (0) root         (0)      528 2023-05-22 10:09:06.000000 salesforce-codetf-1.0.2.1/test_code_utilities/test_parse_code.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-05-22 09:36:05.000000 salesforce-codetf-1.0.2.1/test_code_utilities/test_remove_comments.py
--rw-r--r--   0 root         (0) root         (0)     1109 2023-05-29 16:35:31.000000 salesforce-codetf-1.0.2.1/test_code_utilities/test_variable_renaming.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:02:00.482469 salesforce-codetf-1.0.2.1/test_inference/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:54.000000 salesforce-codetf-1.0.2.1/test_inference/__init__.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.1/test_inference/test_codebert_embedding.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-06-20 05:04:39.000000 salesforce-codetf-1.0.2.1/test_inference/test_codegen_nl2code.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.1/test_inference/test_codet5_multitask.py
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-28 19:36:25.000000 salesforce-codetf-1.0.2.1/test_inference/test_codet5plus_nl2code.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-05-29 17:43:59.000000 salesforce-codetf-1.0.2.1/test_inference/test_load_model_zoo.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-06-28 19:36:34.000000 salesforce-codetf-1.0.2.1/test_inference/test_starcoder_nl2code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:33.894352 salesforce-codetf-1.0.2.2/
+-rw-r--r--   0 root         (0) root         (0)    11411 2023-05-22 01:09:51.000000 salesforce-codetf-1.0.2.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    23459 2023-07-06 08:16:33.897352 salesforce-codetf-1.0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    23054 2023-06-28 09:19:40.000000 salesforce-codetf-1.0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.078213 salesforce-codetf-1.0.2.2/codetf/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.119216 salesforce-codetf-1.0.2.2/codetf/code_utility/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.138217 salesforce-codetf-1.0.2.2/codetf/code_utility/apex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/apex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5146 2023-05-22 05:30:29.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/apex/apex_code_utility.py
+-rw-r--r--   0 root         (0) root         (0)     5116 2023-05-22 10:01:52.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/ast_parser.py
+-rw-r--r--   0 root         (0) root         (0)      846 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/base_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.157219 salesforce-codetf-1.0.2.2/codetf/code_utility/java/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/java/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/java/java_code_utility.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/language_specific_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.176220 salesforce-codetf-1.0.2.2/codetf/code_utility/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.2/codetf/code_utility/python/python_code_utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.205222 salesforce-codetf-1.0.2.2/codetf/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 07:54:40.000000 salesforce-codetf-1.0.2.2/codetf/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5677 2023-05-22 22:51:11.000000 salesforce-codetf-1.0.2.2/codetf/common/registry.py
+-rw-r--r--   0 root         (0) root         (0)    14084 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/common/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.229224 salesforce-codetf-1.0.2.2/codetf/configs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.2/codetf/configs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.241225 salesforce-codetf-1.0.2.2/codetf/configs/dataset/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.2/codetf/configs/dataset/dataset.yaml
+-rw-r--r--   0 root         (0) root         (0)      131 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/configs/default.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.274228 salesforce-codetf-1.0.2.2/codetf/configs/inference/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-05-22 09:11:25.000000 salesforce-codetf-1.0.2.2/codetf/configs/inference/bert.yaml
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-05-29 19:15:11.000000 salesforce-codetf-1.0.2.2/codetf/configs/inference/causal_lm.yaml
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-06-19 21:11:58.000000 salesforce-codetf-1.0.2.2/codetf/configs/inference/codet5.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.296229 salesforce-codetf-1.0.2.2/codetf/configs/training/
+-rw-r--r--   0 root         (0) root         (0)      766 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.2/codetf/configs/training/causal_lm.yaml
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-19 20:22:57.000000 salesforce-codetf-1.0.2.2/codetf/configs/training/codet5.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.377236 salesforce-codetf-1.0.2.2/codetf/data_utility/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-06-19 18:30:44.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/apps_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-05-22 05:34:12.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/base_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-06-19 20:30:20.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/codexglue_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-06 08:10:48.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/human_eval_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2023-06-19 18:30:44.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/mpp_dataset.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-06 07:39:56.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/stackexchange_instruction_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.2/codetf/data_utility/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.397237 salesforce-codetf-1.0.2.2/codetf/models/
+-rw-r--r--   0 root         (0) root         (0)     3494 2023-05-29 19:06:10.000000 salesforce-codetf-1.0.2.2/codetf/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-06-19 20:44:49.000000 salesforce-codetf-1.0.2.2/codetf/models/base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.409238 salesforce-codetf-1.0.2.2/codetf/models/bert_models/
+-rw-r--r--   0 root         (0) root         (0)     3681 2023-06-27 14:58:24.000000 salesforce-codetf-1.0.2.2/codetf/models/bert_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.420239 salesforce-codetf-1.0.2.2/codetf/models/causal_lm_models/
+-rw-r--r--   0 root         (0) root         (0)     4098 2023-06-28 19:36:14.000000 salesforce-codetf-1.0.2.2/codetf/models/causal_lm_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.431240 salesforce-codetf-1.0.2.2/codetf/models/seq2seq_models/
+-rw-r--r--   0 root         (0) root         (0)     5919 2023-06-27 14:58:07.000000 salesforce-codetf-1.0.2.2/codetf/models/seq2seq_models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.461242 salesforce-codetf-1.0.2.2/codetf/performance/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 05:30:30.000000 salesforce-codetf-1.0.2.2/codetf/performance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-06-14 10:17:09.000000 salesforce-codetf-1.0.2.2/codetf/performance/evaluation_metric.py
+-rw-r--r--   0 root         (0) root         (0)     3439 2023-07-06 08:10:33.000000 salesforce-codetf-1.0.2.2/codetf/performance/model_evaluator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.003207 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:32.975281 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/
+-rwxr-xr-x   0 root         (0) root         (0)   623752 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/apex.so
+-rw-r--r--   0 root         (0) root         (0)   517568 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/bash.so
+-rw-r--r--   0 root         (0) root         (0)   361144 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/c.so
+-rw-r--r--   0 root         (0) root         (0)  3032464 2023-05-22 01:09:52.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/c_sharp.so
+-rw-r--r--   0 root         (0) root         (0)  1217512 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/cpp.so
+-rw-r--r--   0 root         (0) root         (0)    99680 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/css.so
+-rw-r--r--   0 root         (0) root         (0)   236232 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/elm.so
+-rw-r--r--   0 root         (0) root         (0)   230128 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/go.so
+-rw-r--r--   0 root         (0) root         (0)  8532424 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/haskell.so
+-rw-r--r--   0 root         (0) root         (0)   149608 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/html.so
+-rw-r--r--   0 root         (0) root         (0)   262848 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/java.so
+-rw-r--r--   0 root         (0) root         (0)   280160 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/javascript.so
+-rw-r--r--   0 root         (0) root         (0)  4604424 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/kotlin.so
+-rw-r--r--   0 root         (0) root         (0)   198688 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/lua.so
+-rw-r--r--   0 root         (0) root         (0)   432360 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/php.so
+-rw-r--r--   0 root         (0) root         (0)   254160 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/python.so
+-rw-r--r--   0 root         (0) root         (0)  1098880 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/ruby.so
+-rw-r--r--   0 root         (0) root         (0)   804520 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/rust.so
+-rw-r--r--   0 root         (0) root         (0)   263848 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/scala.so
+-rw-r--r--   0 root         (0) root         (0)   590536 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/solidity.so
+-rwxr-xr-x   0 root         (0) root         (0)   164488 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/soql.so
+-rwxr-xr-x   0 root         (0) root         (0)   180872 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/sosl.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:33.688336 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/
+-rwxr-xr-x   0 root         (0) root         (0)   533096 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/apex.so
+-rw-r--r--   0 root         (0) root         (0)   160688 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/asm.so
+-rw-r--r--   0 root         (0) root         (0)   704688 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/bash.so
+-rw-r--r--   0 root         (0) root         (0)   442184 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/c.so
+-rw-r--r--   0 root         (0) root         (0)  3112856 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/c_sharp.so
+-rw-r--r--   0 root         (0) root         (0)  1512216 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/cpp.so
+-rw-r--r--   0 root         (0) root         (0)   137144 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/css.so
+-rw-r--r--   0 root         (0) root         (0)   442568 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/elm.so
+-rw-r--r--   0 root         (0) root         (0)   301056 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/go.so
+-rw-r--r--   0 root         (0) root         (0)  4731648 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/haskell.so
+-rw-r--r--   0 root         (0) root         (0)   950536 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/html.so
+-rw-r--r--   0 root         (0) root         (0)   315720 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/java.so
+-rw-r--r--   0 root         (0) root         (0)   343560 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/javascript.so
+-rw-r--r--   0 root         (0) root         (0)  4924440 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/kotlin.so
+-rw-r--r--   0 root         (0) root         (0)   234240 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/lua.so
+-rw-r--r--   0 root         (0) root         (0)   623208 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/php.so
+-rw-r--r--   0 root         (0) root         (0)   352352 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/python.so
+-rw-r--r--   0 root         (0) root         (0)  1364728 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/ruby.so
+-rw-r--r--   0 root         (0) root         (0)   902504 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/rust.so
+-rw-r--r--   0 root         (0) root         (0)   309752 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/scala.so
+-rw-r--r--   0 root         (0) root         (0)   727704 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/solidity.so
+-rwxr-xr-x   0 root         (0) root         (0)   127040 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/soql.so
+-rwxr-xr-x   0 root         (0) root         (0)   139328 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/sosl.so
+-rw-r--r--   0 root         (0) root         (0) 18164400 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/verilog.so
+-rw-r--r--   0 root         (0) root         (0)   445224 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/yaml.so
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:33.763342 salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23459 2023-07-06 08:16:31.000000 salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-07-06 08:16:31.000000 salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2023-07-06 08:16:31.000000 salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 19:37:41.000000 salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      370 2023-07-06 08:16:31.000000 salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-06 08:16:31.000000 salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-06 08:16:33.906353 salesforce-codetf-1.0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-07-06 08:12:54.000000 salesforce-codetf-1.0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:33.812345 salesforce-codetf-1.0.2.2/test_code_utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:53.000000 salesforce-codetf-1.0.2.2/test_code_utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.2/test_code_utilities/test_extract_code_attributes.py
+-rw-r--r--   0 root         (0) root         (0)      528 2023-05-22 10:09:06.000000 salesforce-codetf-1.0.2.2/test_code_utilities/test_parse_code.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-05-22 09:36:05.000000 salesforce-codetf-1.0.2.2/test_code_utilities/test_remove_comments.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2023-05-29 16:35:31.000000 salesforce-codetf-1.0.2.2/test_code_utilities/test_variable_renaming.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:16:33.884351 salesforce-codetf-1.0.2.2/test_inference/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 01:09:54.000000 salesforce-codetf-1.0.2.2/test_inference/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.2/test_inference/test_codebert_embedding.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-20 05:04:39.000000 salesforce-codetf-1.0.2.2/test_inference/test_codegen_nl2code.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-06-06 03:11:09.000000 salesforce-codetf-1.0.2.2/test_inference/test_codet5_multitask.py
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-28 19:36:25.000000 salesforce-codetf-1.0.2.2/test_inference/test_codet5plus_nl2code.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-05-29 17:43:59.000000 salesforce-codetf-1.0.2.2/test_inference/test_load_model_zoo.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-06-28 19:36:34.000000 salesforce-codetf-1.0.2.2/test_inference/test_starcoder_nl2code.py
```

### Comparing `salesforce-codetf-1.0.2.1/LICENSE.txt` & `salesforce-codetf-1.0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/PKG-INFO` & `salesforce-codetf-1.0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 1.0.2.1
+Version: 1.0.2.2
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Keywords: AI4Code,Code Intelligence,Generative AI,Deep Learning,Library,PyTorch,HuggingFace
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.2.1 Summary: CodeTF:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.2.2 Summary: CodeTF:
 A Transformer-based Library for Code Intelligence Home-page: https://
 github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
 Keywords: AI4Code,Code Intelligence,Generative AI,Deep
 Learning,Library,PyTorch,HuggingFace Requires-Python: >=3.8.0 Description-
 Content-Type: text/markdown License-File: LICENSE.txt
 
                               [assets/logo.png]
```

### Comparing `salesforce-codetf-1.0.2.1/README.md` & `salesforce-codetf-1.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/__init__.py` & `salesforce-codetf-1.0.2.2/codetf/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/code_utility/apex/apex_code_utility.py` & `salesforce-codetf-1.0.2.2/codetf/code_utility/apex/apex_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/code_utility/ast_parser.py` & `salesforce-codetf-1.0.2.2/codetf/code_utility/ast_parser.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/code_utility/base_utility.py` & `salesforce-codetf-1.0.2.2/codetf/code_utility/base_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/code_utility/java/java_code_utility.py` & `salesforce-codetf-1.0.2.2/codetf/code_utility/java/java_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/code_utility/python/python_code_utility.py` & `salesforce-codetf-1.0.2.2/codetf/code_utility/python/python_code_utility.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/common/registry.py` & `salesforce-codetf-1.0.2.2/codetf/common/registry.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/common/utils.py` & `salesforce-codetf-1.0.2.2/codetf/common/utils.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/configs/inference/causal_lm.yaml` & `salesforce-codetf-1.0.2.2/codetf/configs/inference/causal_lm.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/configs/inference/codet5.yaml` & `salesforce-codetf-1.0.2.2/codetf/configs/inference/codet5.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/configs/training/causal_lm.yaml` & `salesforce-codetf-1.0.2.2/codetf/configs/training/causal_lm.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/configs/training/codet5.yaml` & `salesforce-codetf-1.0.2.2/codetf/configs/training/codet5.yaml`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/data_utility/apps_dataset.py` & `salesforce-codetf-1.0.2.2/codetf/data_utility/apps_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/data_utility/base_dataset.py` & `salesforce-codetf-1.0.2.2/codetf/data_utility/base_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/data_utility/codexglue_dataset.py` & `salesforce-codetf-1.0.2.2/codetf/data_utility/codexglue_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/data_utility/human_eval_dataset.py` & `salesforce-codetf-1.0.2.2/codetf/data_utility/human_eval_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/data_utility/mpp_dataset.py` & `salesforce-codetf-1.0.2.2/codetf/data_utility/mpp_dataset.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/data_utility/util.py` & `salesforce-codetf-1.0.2.2/codetf/data_utility/util.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/models/__init__.py` & `salesforce-codetf-1.0.2.2/codetf/models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/models/base_model.py` & `salesforce-codetf-1.0.2.2/codetf/models/base_model.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/models/bert_models/__init__.py` & `salesforce-codetf-1.0.2.2/codetf/models/bert_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/models/causal_lm_models/__init__.py` & `salesforce-codetf-1.0.2.2/codetf/models/causal_lm_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/models/seq2seq_models/__init__.py` & `salesforce-codetf-1.0.2.2/codetf/models/seq2seq_models/__init__.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/performance/evaluation_metric.py` & `salesforce-codetf-1.0.2.2/codetf/performance/evaluation_metric.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/performance/model_evaluator.py` & `salesforce-codetf-1.0.2.2/codetf/performance/model_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.accelerator = Accelerator()
 
    
     def evaluate_pass_k(self, problems, unit_tests, batch_size=1, max_length=600, 
                         top_p=0.95, k=[1,10,100], 
                         num_return_sequences=200, sequences_per_chunk=10, num_workers=1):
         # Load dataset
-        data_loader = Dat aLoader(problems, batch_size=batch_size)
+        data_loader = DataLoader(problems, batch_size=batch_size)
         data_loader = self.accelerator.prepare(data_loader)
         
         # Initialize stopping criteria
         gen_kwargs = {
             "do_sample": True,
             "top_p": top_p,
             "stopping_criteria": StoppingCriteriaList([EndOfFunctionCriteria(0, EOF_STRINGS, self.model_class.get_tokenizer())]),
```

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/apex.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/apex.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/bash.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/bash.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/c.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/c.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/c_sharp.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/c_sharp.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/cpp.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/cpp.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/css.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/css.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/elm.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/elm.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/go.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/go.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/haskell.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/haskell.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/html.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/html.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/java.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/java.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/javascript.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/javascript.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/kotlin.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/kotlin.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/lua.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/lua.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/php.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/php.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/python.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/python.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/ruby.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/ruby.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/rust.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/rust.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/scala.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/scala.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/solidity.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/solidity.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/soql.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/soql.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Darwin/sosl.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Darwin/sosl.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/apex.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/apex.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/asm.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/asm.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/bash.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/bash.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/c.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/c.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/c_sharp.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/c_sharp.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/cpp.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/cpp.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/css.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/css.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/elm.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/elm.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/go.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/go.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/haskell.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/haskell.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/html.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/html.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/java.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/java.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/javascript.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/javascript.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/kotlin.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/kotlin.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/lua.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/lua.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/php.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/php.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/python.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/python.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/ruby.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/ruby.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/rust.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/rust.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/scala.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/scala.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/solidity.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/solidity.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/soql.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/soql.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/sosl.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/sosl.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/verilog.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/verilog.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/codetf/tree-sitter-prebuilts/Linux/yaml.so` & `salesforce-codetf-1.0.2.2/codetf/tree-sitter-prebuilts/Linux/yaml.so`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/PKG-INFO` & `salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salesforce-codetf
-Version: 1.0.2.1
+Version: 1.0.2.2
 Summary: CodeTF: A Transformer-based Library for Code Intelligence
 Home-page: https://github.com/Salesforce/CodeTF
 Author: Nghi D. Q. Bui
 License: Apache 2.0
 Keywords: AI4Code,Code Intelligence,Generative AI,Deep Learning,Library,PyTorch,HuggingFace
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.2.1 Summary: CodeTF:
+Metadata-Version: 2.1 Name: salesforce-codetf Version: 1.0.2.2 Summary: CodeTF:
 A Transformer-based Library for Code Intelligence Home-page: https://
 github.com/Salesforce/CodeTF Author: Nghi D. Q. Bui License: Apache 2.0
 Keywords: AI4Code,Code Intelligence,Generative AI,Deep
 Learning,Library,PyTorch,HuggingFace Requires-Python: >=3.8.0 Description-
 Content-Type: text/markdown License-File: LICENSE.txt
 
                               [assets/logo.png]
```

### Comparing `salesforce-codetf-1.0.2.1/salesforce_codetf.egg-info/SOURCES.txt` & `salesforce-codetf-1.0.2.2/salesforce_codetf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/setup.py` & `salesforce-codetf-1.0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,26 +18,27 @@
   "sacrebleu==2.3.1",
   "scikit-learn==1.2.2",
   "torch==2.0.1",
   "torchvision==0.15.2",
   "tqdm==4.63.0",
   "transformers==4.30.2",
   "tree-sitter==0.20.1",
-  "bitsandbytes==0.39.1"
+  "bitsandbytes==0.39.1",
+  "evaluate==0.4.0"
 ]
 
 DEPENDENCY_LINKS = []
 if platform.system() == "Windows":
     DEPENDENCY_LINKS.append("https://download.pytorch.org/whl/torch_stable.html")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/transformers.git")
 DEPENDENCY_LINKS.append("git+https://github.com/huggingface/peft.git")
     
 setup(
   name = 'salesforce-codetf',
-  version = "1.0.2.1",
+  version = "1.0.2.2",
   py_modules = ['codetf'],
   description = 'CodeTF: A Transformer-based Library for Code Intelligence',
   author = 'Nghi D. Q. Bui',
   package_dir={"codeff": "codetf"},
   long_description=open("README.md", "r", encoding="utf-8").read(),
   long_description_content_type="text/markdown",
   keywords="AI4Code, Code Intelligence, Generative AI, Deep Learning, Library, PyTorch, HuggingFace",
```

### Comparing `salesforce-codetf-1.0.2.1/test_code_utilities/test_extract_code_attributes.py` & `salesforce-codetf-1.0.2.2/test_code_utilities/test_extract_code_attributes.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/test_code_utilities/test_parse_code.py` & `salesforce-codetf-1.0.2.2/test_code_utilities/test_parse_code.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/test_code_utilities/test_remove_comments.py` & `salesforce-codetf-1.0.2.2/test_code_utilities/test_remove_comments.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/test_code_utilities/test_variable_renaming.py` & `salesforce-codetf-1.0.2.2/test_code_utilities/test_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `salesforce-codetf-1.0.2.1/test_inference/test_codet5_multitask.py` & `salesforce-codetf-1.0.2.2/test_inference/test_codet5_multitask.py`

 * *Files identical despite different names*

