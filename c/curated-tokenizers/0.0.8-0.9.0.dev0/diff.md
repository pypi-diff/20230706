# Comparing `tmp/curated-tokenizers-0.0.8.tar.gz` & `tmp/curated-tokenizers-0.9.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-tokenizers-0.0.8.tar", last modified: Thu Jul  6 15:18:28 2023, max compression
+gzip compressed data, was "curated-tokenizers-0.9.0.dev0.tar", last modified: Thu Jul  6 13:19:20 2023, max compression
```

## Comparing `curated-tokenizers-0.0.8.tar` & `curated-tokenizers-0.9.0.dev0.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.201086 curated-tokenizers-0.0.8/
--rw-r--r--   0 vsts      (1001) docker     (122)     2642 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)     1880 2023-07-06 15:18:28.205086 curated-tokenizers-0.0.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      939 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.169086 curated-tokenizers-0.0.8/curated_tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/_bbpe.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     6178 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/_bbpe.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)     2149 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/_spp.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     7562 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/_spp.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      654 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/_wordpiece.pxd
--rw-r--r--   0 vsts      (1001) docker     (122)     4633 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/_wordpiece.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/config.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/merges.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1190 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/merges.hh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.173086 curated-tokenizers-0.0.8/curated_tokenizers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/incorrect-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     6291 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/robbert-merges-1000.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    16815 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/robbert-vocab-1000.json
--rw-r--r--   0 vsts      (1001) docker     (122)     1865 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/test_bbpe_processor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4420 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/test_sp.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2009 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/test_word_piece_processor.py
--rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/toy-word-pieces.txt
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/tests/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/util.hh
--rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/wordpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/curated_tokenizers/wordpiece.hh
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.173086 curated-tokenizers-0.0.8/curated_tokenizers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1880 2023-07-06 15:18:28.000000 curated-tokenizers-0.0.8/curated_tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    10412 2023-07-06 15:18:28.000000 curated-tokenizers-0.0.8/curated_tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 15:18:28.000000 curated-tokenizers-0.0.8/curated_tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-07-06 15:18:28.000000 curated-tokenizers-0.0.8/curated_tokenizers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-06 15:18:28.000000 curated-tokenizers-0.0.8/curated_tokenizers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 15:18:27.000000 curated-tokenizers-0.0.8/curated_tokenizers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.165087 curated-tokenizers-0.0.8/sentencepiece/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.173086 curated-tokenizers-0.0.8/sentencepiece/python/
--rw-r--r--   0 vsts      (1001) docker     (122)     5858 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/python/once.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.189086 curated-tokenizers-0.0.8/sentencepiece/src/
--rw-r--r--   0 vsts      (1001) docker     (122)     6648 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/bpe_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/bpe_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     9294 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10322 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4416 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    18401 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/builder.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5102 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/builder.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/builder_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.189086 curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/
--rw-r--r--   0 vsts      (1001) docker     (122)    35154 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    40648 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece.pb.h
--rw-r--r--   0 vsts      (1001) docker     (122)   130839 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
--rw-r--r--   0 vsts      (1001) docker     (122)   189303 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/char_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1061 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/char_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/char_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1782 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/char_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/char_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/char_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6007 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/common.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5713 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/compile_charsmap_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4167 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/error.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3563 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/filesystem.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1852 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/filesystem.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1577 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/filesystem_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2345 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/freelist.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1221 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/freelist_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1341 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/init.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5359 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/init_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/model_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/model_factory.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1743 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/model_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6609 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/model_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9527 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/model_interface.h
--rw-r--r--   0 vsts      (1001) docker     (122)    15932 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/model_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)  7198605 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/normalization_rule.h
--rw-r--r--   0 vsts      (1001) docker     (122)    11633 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/normalizer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5835 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/normalizer.h
--rw-r--r--   0 vsts      (1001) docker     (122)    16156 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/normalizer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2024 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/pretokenizer_for_training.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/pretokenizer_for_training.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2654 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/pretokenizer_for_training_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30990 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_processor.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    19673 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_processor.h
--rw-r--r--   0 vsts      (1001) docker     (122)    47605 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_processor_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6527 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)    13402 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10493 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/spec_parser.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3986 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/spm_decode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6557 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/spm_encode_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2035 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/spm_export_vocab_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4163 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/spm_normalize_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    12142 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/spm_train_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1026 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/test_main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/testharness.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     8718 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/testharness.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2103 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/trainer_factory.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/trainer_factory.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1656 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/trainer_factory_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    25917 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/trainer_interface.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/trainer_interface.h
--rw-r--r--   0 vsts      (1001) docker     (122)    19808 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/trainer_interface_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unicode_script.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2807 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unicode_script.h
--rw-r--r--   0 vsts      (1001) docker     (122)   106446 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unicode_script_map.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1525 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unicode_script_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    31219 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unigram_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6912 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unigram_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)    32258 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unigram_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    18625 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unigram_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3879 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unigram_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3321 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/unigram_model_trainer_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     7746 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/util.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    11414 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12866 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/util_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/word_model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1045 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/word_model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/word_model_test.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2101 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/word_model_trainer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/word_model_trainer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2464 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/src/word_model_trainer_test.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.165087 curated-tokenizers-0.0.8/sentencepiece/third_party/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.165087 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.189086 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/container/
--rw-r--r--   0 vsts      (1001) docker     (122)     1001 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/container/flat_hash_map.h
--rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/container/flat_hash_set.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.189086 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/flags/
--rw-r--r--   0 vsts      (1001) docker     (122)     5614 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/flags/flag.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1673 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/flags/flag.h
--rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/flags/parse.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.193086 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/memory/
--rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/memory/memory.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.193086 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/
--rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/ascii.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/match.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1012 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/numbers.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1447 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_cat.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_format.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2413 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_join.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_replace.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_split.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7856 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/string_view.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20934 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/string_view.h
--rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/strip.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.193086 curated-tokenizers-0.0.8/sentencepiece/third_party/darts_clone/
--rw-r--r--   0 vsts      (1001) docker     (122)    51750 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/darts_clone/darts.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.197086 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/
--rw-r--r--   0 vsts      (1001) docker     (122)    15726 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/arena.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     8985 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/arenastring.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/bytestream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30847 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/coded_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10999 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/common.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    82338 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/extension_set.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3573 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4441 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    30000 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.169086 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.201086 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/
--rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
--rw-r--r--   0 vsts      (1001) docker     (122)    29756 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
--rw-r--r--   0 vsts      (1001) docker     (122)    18092 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
--rw-r--r--   0 vsts      (1001) docker     (122)    15918 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
--rw-r--r--   0 vsts      (1001) docker     (122)    96637 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
--rw-r--r--   0 vsts      (1001) docker     (122)    78585 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12437 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3993 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3266 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12532 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31313 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    10023 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3542 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7024 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.201086 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
--rw-r--r--   0 vsts      (1001) docker     (122)    69376 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5384 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
--rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12750 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
--rw-r--r--   0 vsts      (1001) docker     (122)    16950 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    48107 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
--rw-r--r--   0 vsts      (1001) docker     (122)    24921 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7104 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31973 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
--rw-r--r--   0 vsts      (1001) docker     (122)    27172 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8270 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)    32754 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
--rw-r--r--   0 vsts      (1001) docker     (122)    20834 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
--rw-r--r--   0 vsts      (1001) docker     (122)     4209 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
--rw-r--r--   0 vsts      (1001) docker     (122)   101600 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 15:18:28.201086 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
--rw-r--r--   0 vsts      (1001) docker     (122)    11769 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
--rw-r--r--   0 vsts      (1001) docker     (122)    17098 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5733 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
--rw-r--r--   0 vsts      (1001) docker     (122)     7283 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3911 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
--rw-r--r--   0 vsts      (1001) docker     (122)    11971 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8915 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4903 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
--rw-r--r--   0 vsts      (1001) docker     (122)    31213 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6157 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2184 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
--rw-r--r--   0 vsts      (1001) docker     (122)     5108 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12765 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3949 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
--rw-r--r--   0 vsts      (1001) docker     (122)     8558 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3293 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
--rw-r--r--   0 vsts      (1001) docker     (122)    17861 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3615 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
--rw-r--r--   0 vsts      (1001) docker     (122)    39629 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3356 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
--rw-r--r--   0 vsts      (1001) docker     (122)    14401 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
--rw-r--r--   0 vsts      (1001) docker     (122)    83648 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2756 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6587 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/int128.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    13526 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/io_win32.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20751 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/message_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    20703 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/parse_context.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     5500 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/repeated_field.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4197 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/status.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/statusor.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     9193 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/stringpiece.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     6283 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/stringprintf.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    26415 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    88575 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/strutil.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    10168 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/time.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    27892 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2392 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    11345 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
--rw-r--r--   0 vsts      (1001) docker     (122)    13255 2023-07-06 15:18:15.000000 curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1196 2023-07-06 15:18:28.205086 curated-tokenizers-0.0.8/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     6023 2023-07-06 15:18:12.000000 curated-tokenizers-0.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2642 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     1885 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      939 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/curated_tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_bbpe.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     5992 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_bbpe.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)     2149 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      654 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pxd
+-rw-r--r--   0 vsts      (1001) docker     (122)     4803 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      156 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/config.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2126 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1190 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.855949 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/incorrect-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     6291 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-merges-1000.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    16815 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-vocab-1000.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     2252 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_bbpe_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4233 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_sp.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2220 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_word_piece_processor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/toy-word-pieces.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)      333 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/util.hh
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1011 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.hh
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1885 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    10431 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 13:19:20.000000 curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.847950 curated-tokenizers-0.9.0.dev0/sentencepiece/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6596 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1748 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9294 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11226 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4521 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4850 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    18686 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5203 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7354 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/
+-rw-r--r--   0 vsts      (1001) docker     (122)    35154 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    40648 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   136631 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)   200094 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1304 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1061 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3525 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1782 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1265 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5168 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5936 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/compile_charsmap_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4103 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/error.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3563 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1852 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1577 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2605 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1280 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1770 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/init.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5359 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/init_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1644 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1743 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6609 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8751 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15351 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)  7198605 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalization_rule.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11583 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5817 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16156 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2132 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2152 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2892 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    37639 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    27254 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    54189 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9966 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6523 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    13402 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10925 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spec_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4037 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_decode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6597 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_encode_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2083 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_export_vocab_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4214 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_normalize_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13036 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_train_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1077 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/test_main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1899 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8718 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2103 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1104 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1656 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    28978 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20727 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1239 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2817 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.h
+-rw-r--r--   0 vsts      (1001) docker     (122)   106446 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1525 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    34126 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     7324 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32283 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    22266 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4053 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6752 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     7393 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10907 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12866 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/util_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1124 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1045 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2639 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_test.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2101 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1372 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2464 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer_test.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1001 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      966 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_set.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5857 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1745 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      799 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/parse.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/memory/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2592 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/memory/memory.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/
+-rw-r--r--   0 vsts      (1001) docker     (122)      959 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/distributions.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      926 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/random/random.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1309 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/ascii.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1308 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/match.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1012 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/numbers.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1447 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_cat.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_format.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2413 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_join.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2127 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2669 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_split.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2106 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/string_view.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      991 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/strip.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.871950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/darts_clone/
+-rw-r--r--   0 vsts      (1001) docker     (122)    51750 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/darts_clone/darts.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.875949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/
+-rw-r--r--   0 vsts      (1001) docker     (122)    15726 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arena.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     8985 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arenastring.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/bytestream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30847 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/coded_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10999 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/common.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    82338 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/extension_set.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3573 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4441 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    30000 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.851950 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.879949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6215 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    29756 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    18092 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15918 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    96637 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    78585 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12437 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3993 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3266 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12532 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31313 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10023 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3542 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7024 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.879949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/
+-rw-r--r--   0 vsts      (1001) docker     (122)    69376 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5384 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    10258 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12750 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    16950 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    48107 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    24921 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7104 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31973 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    27172 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8270 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    32754 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    20834 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4209 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc
+-rw-r--r--   0 vsts      (1001) docker     (122)   101600 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11769 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17098 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5733 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     7283 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3911 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    11971 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8915 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4903 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    31213 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6157 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2184 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     5108 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12765 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3949 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     8558 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3293 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17861 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3615 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    39629 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3356 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    14401 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    83648 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2756 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6587 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/int128.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13526 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/io_win32.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20751 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/message_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    20703 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/parse_context.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     5500 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/repeated_field.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4197 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/status.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2096 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/statusor.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     9193 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringpiece.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     6283 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringprintf.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    26415 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    88575 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/strutil.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    10168 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/time.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    27892 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2392 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    11345 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)    13255 2023-07-06 13:19:06.000000 curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1201 2023-07-06 13:19:20.883949 curated-tokenizers-0.9.0.dev0/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     5941 2023-07-06 13:19:03.000000 curated-tokenizers-0.9.0.dev0/setup.py
```

### Comparing `curated-tokenizers-0.0.8/LICENSE` & `curated-tokenizers-0.9.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/PKG-INFO` & `curated-tokenizers-0.9.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.0.8
+Version: 0.9.0.dev0
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `curated-tokenizers-0.0.8/README.md` & `curated-tokenizers-0.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/_bbpe.pyx` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_bbpe.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -62,22 +62,14 @@
         self._piece_to_id = vocab
         self._id_to_piece = {v: k for k, v in vocab.items()}
         cdef vector[pair[string, string]] c_merges
         for p1, p2 in merges:
             c_merges.push_back(pair[string, string](p1.encode('utf-8'), p2.encode('utf-8')))
         self._merges = make_shared[Merges](c_merges)
 
-    def __copy__(self):
-        return ByteBPEProcessor(vocab=self.vocab, merges=self.merges)
-
-    def __deepcopy__(self, memo):
-        # We don't need a deepcopy of the vocab and merges dicts as their
-        # contents will be copied into a backing store in the c'tor.
-        return ByteBPEProcessor(vocab=self.vocab, merges=self.merges)
-
     @staticmethod
     def load_from_files(*, vocab: Path, merges: Path) -> ByteBPEProcessor:
         """Construct a processor from the given vocabulary and merges files."""
         with open(vocab, encoding="utf-8") as f:
             vocab = json.load(f)
         with open(merges, encoding="utf-8") as f:
             version = f.readline()
@@ -143,18 +135,22 @@
 
     @property
     def merges(self) -> List[Tuple[str, str]]:
         """Get all merges."""
         merges_bytes = deref(self._merges).merges()
         return [(m1.decode('utf-8'), m2.decode('utf-8')) for m1, m2 in merges_bytes]
 
-    def piece_id(self, piece: str) -> Optional[int]:
+    def piece_to_id(self, piece: str) -> Optional[int]:
         """Get the identifier for a piece."""
         return self._piece_to_id.get(piece)
 
+    def id_to_piece(self, piece_id: int) -> Optional[str]:
+        """Get the piece for an identifier."""
+        return self._id_to_piece.get(piece_id)
+
     @property
     def vocab(self) -> Dict[str, int]:
         """Get a copy of the vocabulary."""
         return dict(self._piece_to_id)
 
     def _pieces_to_ids(self, pieces):
         piece_ids = []
```

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/_spp.pxd` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/_spp.pyx` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_spp.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from cython.operator cimport dereference as deref
-from typing import List, Tuple
+from typing import List, Tuple, Optional
 
 cdef class SentencePieceProcessor:
     def __cinit__(self):
         self.spp.reset(new CSentencePieceProcessor())
 
     def __init__(self):
         pass
 
     def __len__(self):
         _check_status(deref(self.spp).status())
         return deref(self.spp).GetPieceSize()
 
-    def __copy__(self):
-        return SentencePieceProcessor.from_protobuf(self.to_protobuf())
-
-    def __deepcopy__(self, memo):
-        result = SentencePieceProcessor.from_protobuf(self.to_protobuf())
-        memo[id(self)] = result
-        return result
-
     @staticmethod
     def from_file(str filename):
         """
         Constructs a SentencePieceProcessor by loading a serialized model from
         disk.
 
             filename (str): Path to model.
@@ -38,17 +30,14 @@
         Constructs a SentencePieceProcessor by loading a serialized model from
         a protocol buffer.
 
             protobuf (bytes): Byte array representing the model's serialized
                 protocol buffer.
         """
         cdef SentencePieceProcessor processor = SentencePieceProcessor.__new__(SentencePieceProcessor)
-        if len(protobuf) == 0:
-            # SentencePiece returns an empty protobuf for uninitialized models.
-            return processor
         cdef string_view protobuf_view = string_view(protobuf, len(protobuf))
         _check_status(deref(processor.spp).LoadFromSerializedProto(protobuf_view))
         return processor
 
     def to_protobuf(self) -> bytes:
         """
         Serializes the SentencePieceProcessor to a protocol buffer.
@@ -144,40 +133,47 @@
         pieces = []
         for idx in range(text.pieces_size()):
             piece = text.pieces(idx)
             pieces.append(text.pieces(idx).piece().decode("utf-8"))
 
         return pieces
 
-    def piece_to_id(self, str piece) -> int:
+    def piece_to_id(self, str piece) -> Optional[int]:
         """
-        Returns the piece identifier for a given piece token. Returns the 
-        `unk` piece identifier if the piece token is OOV.
+        Returns the piece identifier for a given piece token, or 
+        `None` if the piece token is OOV.
 
             piece (str): Piece token.
-            RETURNS (int): Piece ID.
+            RETURNS (int): Piece ID or None.
         """
         piece_bytes = piece.encode("utf8")
         cdef string_view piece_view = string_view(piece_bytes, len(piece_bytes))
         _check_status(deref(self.spp).status())
-        return deref(self.spp).PieceToId(piece_view)
+        cdef int piece_id = deref(self.spp).PieceToId(piece_view)
+        cdef int unk_id = self.unk_id()
+        cdef str unk_piece = self.id_to_piece(unk_id)
+        if piece_id == self.unk_id() and piece != unk_piece:
+            return None
+        else:
+            return piece_id
 
-    def id_to_piece(self, int piece_id) -> str:
+    def id_to_piece(self, int piece_id) -> Optional[str]:
         """
-        Returns the piece token for a given piece identifier. Raises a `ValueError` 
-        if the piece identifier is out-of-bounds.
+        Returns the piece token for a given piece identifier, or
+        `None` if the piece identifier is out-of-bounds.
 
             piece_id (int): Piece ID.
-            RETURNS (str): Piece token.
+            RETURNS (str): Piece token or None.
         """
         _check_status(deref(self.spp).status())
         cdef int vocab_size = deref(self.spp).GetPieceSize()
         if not 0 <= piece_id < vocab_size:
-            raise ValueError(f"piece ID must be in range [0,{vocab_size}), got {piece_id}")
-        return deref(self.spp).IdToPiece(piece_id).decode("utf8")
+            return None
+        else:
+            return deref(self.spp).IdToPiece(piece_id).decode("utf8")
 
     def bos_id(self) -> int:
         """Returns the piece identifier for the `bos` meta token."""
         _check_status(deref(self.spp).status())
         return deref(self.spp).bos_id()
 
     def eos_id(self) -> int:
```

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/_wordpiece.pxd` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pxd`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/_wordpiece.pyx` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/_wordpiece.pyx`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Iterable
+from typing import List, Tuple, Iterable, Optional
 from cython.operator cimport dereference as deref
 from libcpp cimport pair
 
 cdef struct PieceMatch:
     bint found
     int prefix_len
     int piece_id
@@ -14,21 +14,14 @@
         self._pieces = PieceStorage()
 
         for idx, piece in enumerate(pieces):
             is_initial = not piece.startswith("##")
             byte_array = piece[2:].encode('utf8') if not is_initial else piece.encode('utf8')
             self._pieces.add_piece(byte_array, is_initial)
 
-    def __copy__(self):
-        # This is essentially a deepcopy, but there's no better way to do it.
-        return WordPieceProcessor(self.to_list())
-
-    def __deepcopy__(self, memo):
-        return WordPieceProcessor(self.to_list())
-
     def encode(self, token: str) -> Tuple[List[int], List[str]]:
         """
         Encode a token using word pieces. The piece identifiers are
         returned. If no piece could be found for a suffix, the special
         piece identifier `-1` is used.
 
             token (str): The token to encode as pieces.
@@ -50,45 +43,59 @@
             token = token[match.prefix_len:]
             is_initial = False
             prefix = "##"
         return token_ids, token_pieces
 
     def decode(self, pieces: Iterable[int]) -> str:
         """
-        Decode token piece identifiers into string. Raises a `RuntimeError` 
+        Decode token piece identifiers into string. Raises a `ValueError` 
         if any of the identifiers are invalid.
 
             ids (Iterable[int]): Piece IDs.
             RETURNS (str): Decoded string.
         """
-        token_pieces = [self.id_to_piece(id)[0] for id in pieces]
+        token_pieces = []
+        for piece_id in pieces:
+            piece = self.id_to_piece(piece_id)
+            if piece is None:
+                raise ValueError(f"Piece ID `{piece_id}` is invalid")
+            else:
+                token_pieces.append(piece[0])
         return "".join(token_pieces)
 
-    def get_initial(self, piece: str) -> int:
+    def get_initial(self, piece: str) -> Optional[int]:
         """
-        Returns the ID for the given initial piece. Raises a `RuntimeError` if 
+        Returns the ID for the given initial piece, or `None` if
         the string isn't an initial piece.
 
             piece (str): Initial piece string.
-            RETURNS (int): Piece ID.
+            RETURNS (Optional[int]): Piece ID or None
         """
-        return self._pieces.piece_to_id(Piece(piece.encode('utf8'), True))
+        try:
+            return self._pieces.piece_to_id(Piece(piece.encode('utf8'), True))
+        except RuntimeError:
+            return None
 
     def id_to_piece(self, piece: int) -> Tuple[str, bool]:
         """
         Returns the piece string (without any prefix) for a given piece identifier 
-        and a boolean identifying if it is an initial piece. Raises a `RuntimeError` if 
-        any of the identifiers are invalid.
+        and a boolean identifying if it is an initial piece. Returns `None` if the 
+        piece identifier is invalid.
 
             piece (int): Piece ID.
-            RETURNS (Tuple[str, bool]): Piece string and a boolean identifying if
-                it is an initial piece.
-        """
-        cdef const Piece* ptr_piece = &self._pieces.id_to_piece(piece)
-        return (ptr_piece[0].piece.decode('utf8'), ptr_piece[0].is_initial) 
+            RETURNS (Optional[Tuple[str, bool]]): 
+                Piece string and a boolean identifying if it is an initial piece,
+                or None
+        """
+        cdef const Piece* ptr_piece
+        try:
+            ptr_piece = &self._pieces.id_to_piece(piece)
+            return (ptr_piece[0].piece.decode('utf8'), ptr_piece[0].is_initial) 
+        except RuntimeError:
+            return None
 
     def is_valid_piece_id(self, piece: int) -> bool:
         """
         Returns True if the piece identifier is valid, False otherwise.
 
             piece (int): Piece ID.
             RETURNS (bool): Is valid.
```

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/merges.cc` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/merges.hh` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/merges.hh`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/tests/robbert-merges-1000.txt` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-merges-1000.txt`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/tests/robbert-vocab-1000.json` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/robbert-vocab-1000.json`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/tests/test_bbpe_processor.py` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_word_piece_processor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,83 +1,82 @@
-from curated_tokenizers import ByteBPEProcessor
-import json
 from pathlib import Path
+
 import pytest
+from curated_tokenizers import WordPieceProcessor
+
+EXAMPLE_TOKENS = [
+    "voor",
+    "voorman",
+    "coördinatie",
+    "voorkomen",
+]
+
+EXAMPLE_ENCODINGS = [
+    ([0], ["voor"]),
+    ([0, -1], ["voor", None]),
+    ([2, 1], ["coördina", "##tie"]),
+    ([0, 3, 4], ["voor", "##kom", "##en"]),
+]
+
+EXAMPLE_DECODINGS = [
+    "voor",
+    "",  # Will raise an error.
+    "coördinatie",
+    "voorkomen",
+]
+
+TOKEN_PIECES = ["voor", "##tie", "coördina", "##kom", "##en"]
 
 
 @pytest.fixture(scope="module")
 def test_dir(request):
     return Path(request.fspath).parent
 
 
 @pytest.fixture
-def toy_processor(test_dir):
-    return ByteBPEProcessor.load_from_files(
-        vocab=test_dir / "robbert-vocab-1000.json",
-        merges=test_dir / "robbert-merges-1000.txt",
-    )
-
-
-EXAMPLE_TEXT = " Wij bezoeken alle provinciën."
-EXAMPLE_PIECES = [
-    "ĠWij",
-    "Ġbez",
-    "oeken",
-    "Ġalle",
-    "Ġpro",
-    "v",
-    "in",
-    "c",
-    "iÃ«n",
-    ".",
-]
+def toy_processor_from_file(test_dir):
+    return WordPieceProcessor.from_file(str(test_dir / "toy-word-pieces.txt"))
+
+
+@pytest.fixture
+def toy_processor():
+    return WordPieceProcessor(TOKEN_PIECES)
+
+
+def test_word_piece_processor_small_encode(toy_processor):
+    for token, output in zip(EXAMPLE_TOKENS, EXAMPLE_ENCODINGS):
+        y = toy_processor.encode(token)
+        assert y == output
+
+
+def test_word_piece_processor_small_decode(toy_processor):
+    for encoding, result in zip(EXAMPLE_ENCODINGS, EXAMPLE_DECODINGS):
+        if -1 in encoding[0]:
+            with pytest.raises(ValueError):
+                toy_processor.decode(encoding[0])
+        else:
+            assert toy_processor.decode(encoding[0]) == result
+
+
+def test_to_list(toy_processor):
+    assert toy_processor.to_list() == TOKEN_PIECES
+
+
+def test_from_file(toy_processor_from_file):
+    assert toy_processor_from_file.to_list() == TOKEN_PIECES
+
+
+def test_get_initial_and_id_to_piece(toy_processor):
+    assert toy_processor.get_initial("voor") == 0
+    assert toy_processor.get_initial("tie") is None
+    assert toy_processor.get_initial("##tie") is None
 
-EXAMPLE_PIECE_IDS = [280, 3377, 7095, 92, 1951, 253, 194, 311, 3698, 4]
+    assert toy_processor.id_to_piece(2) == ("coördina", True)
+    assert toy_processor.id_to_piece(1) == ("tie", False)
+    assert toy_processor.id_to_piece(999) is None
 
 
-def test_empty_processor():
-    bbpe = ByteBPEProcessor({}, [])
-    # An empty processor never merges, only recodes bytes.
-    assert bbpe.encode_as_pieces("they'll visit Köln") == [
-        "t",
-        "h",
-        "e",
-        "y",
-        "'",
-        "l",
-        "l",
-        "Ġ",
-        "v",
-        "i",
-        "s",
-        "i",
-        "t",
-        "Ġ",
-        "K",
-        "Ã",
-        "¶",
-        "l",
-        "n",
-    ]
-
-def test_can_decode(toy_processor):
-    assert toy_processor.decode_from_ids(EXAMPLE_PIECE_IDS) == EXAMPLE_TEXT
-
-
-def test_can_encode(toy_processor):
-    assert toy_processor.encode(EXAMPLE_TEXT) == (EXAMPLE_PIECE_IDS, EXAMPLE_PIECES)
-
-
-def test_can_encode_as_ids(toy_processor):
-    assert toy_processor.encode_as_ids(EXAMPLE_TEXT) == EXAMPLE_PIECE_IDS
-
-
-def test_can_encode_as_pieces(toy_processor):
-    assert toy_processor.encode_as_pieces(EXAMPLE_TEXT) == EXAMPLE_PIECES
-
-
-def test_rejects_incorrect_merges(test_dir):
-    with pytest.raises(ValueError, match=r"Merge must consist of 2 items"):
-        ByteBPEProcessor.load_from_files(
-            vocab=test_dir / "robbert-vocab-1000.json",
-            merges=test_dir / "incorrect-merges.txt",
-        )
+def test_piece_id_valid(toy_processor):
+    assert toy_processor.is_valid_piece_id(-1) == False
+    assert toy_processor.is_valid_piece_id(0) == True
+    assert toy_processor.is_valid_piece_id(len(TOKEN_PIECES)) == False
+    assert toy_processor.is_valid_piece_id(len(TOKEN_PIECES) - 1) == True
```

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/tests/test_sp.py` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/test_sp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
-import pytest
 
+import pytest
 from curated_tokenizers import SentencePieceProcessor
 
 
 @pytest.fixture(scope="module")
 def test_dir(request):
     return Path(request.fspath).parent
 
@@ -18,18 +18,14 @@
     with open(str(test_dir / "toy.model"), "rb") as f:
         data = f.read()
     spp = SentencePieceProcessor.from_protobuf(data)
     _check_ids(spp)
     serialized_data = spp.to_protobuf()
     assert serialized_data == data
 
-    # Zero-length buffer.
-    spp = SentencePieceProcessor.from_protobuf(bytes())
-    assert spp.to_protobuf() == bytes()
-
 
 def test_load_unknown_file():
     with pytest.raises(OSError, match=r"No such file"):
         SentencePieceProcessor.from_file("bogus.model")
 
 
 def test_handles_nul_character(toy_model):
@@ -148,16 +144,14 @@
     assert ids == [8, 465, 10, 947, 41, 10, 170, 168, 110, 28, 20, 143, 4]
 
 
 def test_id_to_piece_and_piece_to_id(toy_model):
     assert toy_model.piece_to_id("<s>") == toy_model.bos_id()
     assert toy_model.piece_to_id("</s>") == toy_model.eos_id()
     assert toy_model.piece_to_id("<unk>") == toy_model.unk_id()
-    assert toy_model.piece_to_id("qotsa") == toy_model.unk_id()
+    assert toy_model.piece_to_id("qotsa") is None
 
     assert toy_model.id_to_piece(toy_model.bos_id()) == "<s>"
     assert toy_model.id_to_piece(toy_model.eos_id()) == "</s>"
     assert toy_model.id_to_piece(toy_model.unk_id()) == "<unk>"
-    with pytest.raises(ValueError):
-        toy_model.id_to_piece(-1)
-    with pytest.raises(ValueError):
-        toy_model.id_to_piece(len(toy_model))
+    assert toy_model.id_to_piece(-1) is None
+    assert toy_model.id_to_piece(len(toy_model)) is None
```

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/tests/toy.model` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/tests/toy.model`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/wordpiece.cc` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers/wordpiece.hh` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers/wordpiece.hh`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers.egg-info/PKG-INFO` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curated-tokenizers
-Version: 0.0.8
+Version: 0.9.0.dev0
 Summary: Lightweight piece tokenization library
 Home-page: https://github.com/explosion/curated-tokenizers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `curated-tokenizers-0.0.8/curated_tokenizers.egg-info/SOURCES.txt` & `curated-tokenizers-0.9.0.dev0/curated_tokenizers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 curated_tokenizers/tests/robbert-merges-1000.txt
 curated_tokenizers/tests/robbert-vocab-1000.json
 curated_tokenizers/tests/test_bbpe_processor.py
 curated_tokenizers/tests/test_sp.py
 curated_tokenizers/tests/test_word_piece_processor.py
 curated_tokenizers/tests/toy-word-pieces.txt
 curated_tokenizers/tests/toy.model
-sentencepiece/python/once.h
 sentencepiece/src/bpe_model.cc
 sentencepiece/src/bpe_model.h
 sentencepiece/src/bpe_model_test.cc
 sentencepiece/src/bpe_model_trainer.cc
 sentencepiece/src/bpe_model_trainer.h
 sentencepiece/src/bpe_model_trainer_test.cc
 sentencepiece/src/builder.cc
@@ -116,23 +115,24 @@
 sentencepiece/src/builtin_pb/sentencepiece_model.pb.h
 sentencepiece/third_party/absl/container/flat_hash_map.h
 sentencepiece/third_party/absl/container/flat_hash_set.h
 sentencepiece/third_party/absl/flags/flag.cc
 sentencepiece/third_party/absl/flags/flag.h
 sentencepiece/third_party/absl/flags/parse.h
 sentencepiece/third_party/absl/memory/memory.h
+sentencepiece/third_party/absl/random/distributions.h
+sentencepiece/third_party/absl/random/random.h
 sentencepiece/third_party/absl/strings/ascii.h
 sentencepiece/third_party/absl/strings/match.h
 sentencepiece/third_party/absl/strings/numbers.h
 sentencepiece/third_party/absl/strings/str_cat.h
 sentencepiece/third_party/absl/strings/str_format.h
 sentencepiece/third_party/absl/strings/str_join.h
 sentencepiece/third_party/absl/strings/str_replace.h
 sentencepiece/third_party/absl/strings/str_split.h
-sentencepiece/third_party/absl/strings/string_view.cc
 sentencepiece/third_party/absl/strings/string_view.h
 sentencepiece/third_party/absl/strings/strip.h
 sentencepiece/third_party/darts_clone/darts.h
 sentencepiece/third_party/protobuf-lite/arena.cc
 sentencepiece/third_party/protobuf-lite/arenastring.cc
 sentencepiece/third_party/protobuf-lite/bytestream.cc
 sentencepiece/third_party/protobuf-lite/coded_stream.cc
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/python/once.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/casts.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 // Protocol Buffers - Google's data interchange format
-// Copyright 2008 Google Inc.  All rights reserved.
+// Copyright 2014 Google Inc.  All rights reserved.
 // https://developers.google.com/protocol-buffers/
 //
 // Redistribution and use in source and binary forms, with or without
 // modification, are permitted provided that the following conditions are
 // met:
 //
 //     * Redistributions of source code must retain the above copyright
@@ -24,134 +24,116 @@
 // SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 // LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 // DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 // THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 // (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 // OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-// Author: kenton@google.com (Kenton Varda)
-//
-// emulates google3/base/once.h
-//
-// This header is intended to be included only by internal .cc files and
-// generated .pb.cc files.  Users should not use this directly.
-//
-// This is basically a portable version of pthread_once().
-//
-// This header declares:
-// * A type called ProtobufOnceType.
-// * A macro GOOGLE_PROTOBUF_DECLARE_ONCE() which declares a variable of type
-//   ProtobufOnceType.  This is the only legal way to declare such a variable.
-//   The macro may only be used at the global scope (you cannot create local or
-//   class member variables of this type).
-// * A function GoogleOnceInit(ProtobufOnceType* once, void (*init_func)()).
-//   This function, when invoked multiple times given the same ProtobufOnceType
-//   object, will invoke init_func on the first call only, and will make sure
-//   none of the calls return before that first call to init_func has finished.
-// * The user can provide a parameter which GoogleOnceInit() forwards to the
-//   user-provided function when it is called. Usage example:
-//     int a = 10;
-//     GoogleOnceInit(&my_once, &MyFunctionExpectingIntArgument, &a);
-// * This implementation guarantees that ProtobufOnceType is a POD (i.e. no
-//   static initializer generated).
-//
-// This implements a way to perform lazy initialization.  It's more efficient
-// than using mutexes as no lock is needed if initialization has already
-// happened.
-//
-// Example usage:
-//   void Init();
-//   GOOGLE_PROTOBUF_DECLARE_ONCE(once_init);
-//
-//   // Calls Init() exactly once.
-//   void InitOnce() {
-//     GoogleOnceInit(&once_init, &Init);
-//   }
-//
-// Note that if GoogleOnceInit() is called before main() has begun, it must
-// only be called by the thread that will eventually call main() -- that is,
-// the thread that performs dynamic initialization.  In general this is a safe
-// assumption since people don't usually construct threads before main() starts,
-// but it is technically not guaranteed.  Unfortunately, Win32 provides no way
-// whatsoever to statically-initialize its synchronization primitives, so our
-// only choice is to assume that dynamic initialization is single-threaded.
-
-#ifndef GOOGLE_PROTOBUF_STUBS_ONCE_H__
-#define GOOGLE_PROTOBUF_STUBS_ONCE_H__
-
-#include <sched.h>
-#include <atomic>
-#include <mutex>
-#include <utility>
+#ifndef GOOGLE_PROTOBUF_CASTS_H__
+#define GOOGLE_PROTOBUF_CASTS_H__
+
+#include <google/protobuf/stubs/common.h>
+
+#include <google/protobuf/port_def.inc>
+#include <type_traits>
 
 namespace google {
 namespace protobuf {
 namespace internal {
 
-using once_flag = std::atomic<int>;
-
-template <typename Callable, typename... Args>
-void my_call_once(once_flag& once, Callable&& fn, Args&&... args) {
-  enum CallOnceState {
-    ONCE_INIT = 0,
-    ONCE_RUNNING = 1,
-    ONCE_DONE = 2,
-  };
-
-  int expected_state = ONCE_INIT;
-  if (once.compare_exchange_strong(expected_state, ONCE_RUNNING)) {
-    fn(std::forward<Args>(args)...);
-    once.store(ONCE_DONE);
-    return;
-  }
-
-  if (expected_state == ONCE_DONE) {
-    return;
-  }
+// Use implicit_cast as a safe version of static_cast or const_cast
+// for upcasting in the type hierarchy (i.e. casting a pointer to Foo
+// to a pointer to SuperclassOfFoo or casting a pointer to Foo to
+// a const pointer to Foo).
+// When you use implicit_cast, the compiler checks that the cast is safe.
+// Such explicit implicit_casts are necessary in surprisingly many
+// situations where C++ demands an exact type match instead of an
+// argument type convertible to a target type.
+//
+// The From type can be inferred, so the preferred syntax for using
+// implicit_cast is the same as for static_cast etc.:
+//
+//   implicit_cast<ToType>(expr)
+//
+// implicit_cast would have been part of the C++ standard library,
+// but the proposal was submitted too late.  It will probably make
+// its way into the language in the future.
+template<typename To, typename From>
+inline To implicit_cast(From const &f) {
+  return f;
+}
 
-  while (once.load() == ONCE_RUNNING) {
-    sched_yield();
+// When you upcast (that is, cast a pointer from type Foo to type
+// SuperclassOfFoo), it's fine to use implicit_cast<>, since upcasts
+// always succeed.  When you downcast (that is, cast a pointer from
+// type Foo to type SubclassOfFoo), static_cast<> isn't safe, because
+// how do you know the pointer is really of type SubclassOfFoo?  It
+// could be a bare Foo, or of type DifferentSubclassOfFoo.  Thus,
+// when you downcast, you should use this macro.  In debug mode, we
+// use dynamic_cast<> to double-check the downcast is legal (we die
+// if it's not).  In normal mode, we do the efficient static_cast<>
+// instead.  Thus, it's important to test in debug mode to make sure
+// the cast is legal!
+//    This is the only place in the code we should use dynamic_cast<>.
+// In particular, you SHOULDN'T be using dynamic_cast<> in order to
+// do RTTI (eg code like this:
+//    if (dynamic_cast<Subclass1>(foo)) HandleASubclass1Object(foo);
+//    if (dynamic_cast<Subclass2>(foo)) HandleASubclass2Object(foo);
+// You should design the code some other way not to need this.
+
+template<typename To, typename From>     // use like this: down_cast<T*>(foo);
+inline To down_cast(From* f) {                   // so we only accept pointers
+  // Ensures that To is a sub-type of From *.  This test is here only
+  // for compile-time type checking, and has no overhead in an
+  // optimized build at run-time, as it will be optimized away
+  // completely.
+  if (false) {
+    implicit_cast<From*, To>(0);
   }
-}
 
-template <typename... Args>
-void call_once(Args&&... args) {
-  my_call_once(std::forward<Args>(args)...);
+#if !defined(NDEBUG) && PROTOBUF_RTTI
+  assert(f == nullptr || dynamic_cast<To>(f) != nullptr);  // RTTI: debug mode only!
+#endif
+  return static_cast<To>(f);
 }
-}  // namespace internal
 
-// TODO(gerbens) remove this once third_party is fully extracted
-using ProtobufOnceType = internal::once_flag;
+template<typename To, typename From>    // use like this: down_cast<T&>(foo);
+inline To down_cast(From& f) {
+  typedef typename std::remove_reference<To>::type* ToAsPointer;
+  // Ensures that To is a sub-type of From *.  This test is here only
+  // for compile-time type checking, and has no overhead in an
+  // optimized build at run-time, as it will be optimized away
+  // completely.
+  if (false) {
+    implicit_cast<From*, ToAsPointer>(0);
+  }
 
-inline void GoogleOnceInit(ProtobufOnceType* once, void (*init_func)()) {
-  internal::my_call_once(*once, init_func);
+#if !defined(NDEBUG) && PROTOBUF_RTTI
+  // RTTI: debug mode only!
+  assert(dynamic_cast<ToAsPointer>(&f) != nullptr);
+#endif
+  return *static_cast<ToAsPointer>(&f);
 }
 
-template <typename Arg>
-inline void GoogleOnceInitArg(ProtobufOnceType* once, void (*init_func)(Arg*),
-                              Arg* arg) {
-  internal::my_call_once(*once, init_func, arg);
+template<typename To, typename From>
+inline To bit_cast(const From& from) {
+  GOOGLE_COMPILE_ASSERT(sizeof(From) == sizeof(To),
+                        bit_cast_with_different_sizes);
+  To dest;
+  memcpy(&dest, &from, sizeof(dest));
+  return dest;
 }
 
-class GoogleOnceDynamic {
- public:
-  // If this->Init() has not been called before by any thread,
-  // execute (*func_with_arg)(arg) then return.
-  // Otherwise, wait until that prior invocation has finished
-  // executing its function, then return.
-  template <typename T>
-  void Init(void (*func_with_arg)(T*), T* arg) {
-    GoogleOnceInitArg<T>(&this->state_, func_with_arg, arg);
-  }
+}  // namespace internal
 
- private:
-  ProtobufOnceType state_;
-};
-
-#define GOOGLE_PROTOBUF_ONCE_TYPE ::google::protobuf::ProtobufOnceType
-#define GOOGLE_PROTOBUF_DECLARE_ONCE(NAME) \
-  ::google::protobuf::ProtobufOnceType NAME
+// We made these internal so that they would show up as such in the docs,
+// but we don't want to stick "internal::" in front of them everywhere.
+using internal::implicit_cast;
+using internal::down_cast;
+using internal::bit_cast;
 
 }  // namespace protobuf
 }  // namespace google
 
-#endif  // GOOGLE_PROTOBUF_STUBS_ONCE_H__
+#include <google/protobuf/port_undef.inc>
+
+#endif  // GOOGLE_PROTOBUF_CASTS_H__
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/bpe_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.cc`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "bpe_model.h"
+
 #include <functional>
 #include <memory>
 #include <queue>
 #include <random>
 #include <utility>
 #include <vector>
 
-#include "bpe_model.h"
 #include "freelist.h"
 #include "third_party/absl/container/flat_hash_map.h"
 #include "util.h"
 
 namespace sentencepiece {
 namespace bpe {
 
@@ -67,16 +68,15 @@
   Agenda agenda;
   std::vector<Symbol> symbols;
   symbols.reserve(normalized.size());
 
   // Reverse merge rules.
   // key: merged symbol, value: pair of original symbols.
   absl::flat_hash_map<absl::string_view,
-                      std::pair<absl::string_view, absl::string_view>,
-                      string_util::string_view_hash>
+                      std::pair<absl::string_view, absl::string_view>>
       rev_merge;
 
   // Pre-allocates SymbolPair for efficiency.
   constexpr size_t kPreallocateSymbolPairSize = 256;
   model::FreeList<SymbolPair> symbol_pair_allocator(kPreallocateSymbolPairSize);
 
   // Lookup new symbol pair at [left, right] and inserts it to agenda.
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/bpe_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.cc`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,25 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "bpe_model_trainer.h"
+
 #include <algorithm>
 #include <string>
 #include <unordered_set>
 #include <vector>
 
-#include "bpe_model_trainer.h"
+#include "pretokenizer_for_training.h"
 #include "third_party/absl/container/flat_hash_set.h"
+#include "third_party/absl/strings/str_join.h"
+#include "third_party/absl/strings/str_replace.h"
 #include "util.h"
 
 namespace sentencepiece {
 namespace bpe {
 
 std::string Trainer::Symbol::ToString() const {
   return string_util::UnicodeTextToUTF8(chars);
@@ -185,14 +189,32 @@
   // Load all sentences
   RETURN_IF_ERROR(LoadSentences());
 
   if (trainer_spec_.split_by_whitespace()) {
     SplitSentencesByWhitespace();
   }
 
+  // Pretokenizer applied only in training time.
+  // Pretokenizer is used as a constraint of piece extractions.
+  const auto *pretokenizer = SentencePieceTrainer::GetPretokenizerForTraining();
+
+  if (pretokenizer || !trainer_spec_.pretokenization_delimiter().empty()) {
+    absl::string_view delimiter = trainer_spec_.pretokenization_delimiter();
+    LOG(INFO) << "Preprocessing with pretokenizer...";
+    for (auto &w : sentences_) {
+      if (pretokenizer) {
+        w.first = absl::StrJoin(pretokenizer->PreTokenize(w.first),
+                                TrainerInterface::kUPPBoundaryStr);
+      } else if (!delimiter.empty()) {
+        w.first = absl::StrReplaceAll(
+            w.first, {{delimiter, TrainerInterface::kUPPBoundaryStr}});
+      }
+    }
+  }
+
   // Initializes symbols_. symbols_[sid][i] stores an unary symbol.
   symbols_.resize(sentences_.size());
   for (size_t i = 0; i < sentences_.size(); ++i) {
     for (const char32 c : string_util::UTF8ToUnicodeText(sentences_[i].first)) {
       symbols_[i].push_back(GetCharSymbol(c));
     }
   }
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer.h`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
 #ifndef BPE_MODEL_TRAINER_H_
 #define BPE_MODEL_TRAINER_H_
 
+#include <cstdint>
+#include <limits>
 #include <set>
 #include <string>
 #include <vector>
 
 #include "sentencepiece_model.pb.h"
 #include "third_party/absl/container/flat_hash_map.h"
 #include "trainer_interface.h"
@@ -40,45 +42,45 @@
  private:
   // Symbol represents a character or symbol bigram.
   struct Symbol {
     const Symbol *left;              // left symbol in bigram
     const Symbol *right;             // right symbol in bigram
     string_util::UnicodeText chars;  // all flattend chracter sequence
     bool is_unk;                     // true if this symbol is unknown.
-    uint64 fp;                       // fingerprint of this symbol.
-    uint64 freq;                     // frequency of this symbol.
+    uint64_t fp;                     // fingerprint of this symbol.
+    uint64_t freq;                   // frequency of this symbol.
 
     // Position list. Use set so that we can keep the order of occurrence.
     // See EncodePos/DecodePos.
-    std::set<uint64> positions;
+    std::set<uint64_t> positions;
 
     bool IsBigram() const { return left != nullptr && right != nullptr; }
     std::string ToString() const;
     Symbol() : left(nullptr), right(nullptr), is_unk(false), fp(0), freq(0) {}
   };
 
   struct Position {
     int sid;    // sentence id
     int left;   // left symbol index
     int right;  // right symbol index
   };
 
-  // Encodes sid, left and right bigram index into uint64.
+  // Encodes sid, left and right bigram index into uint64_t.
   // Encoded value keeps the order of sid, left and right.
-  static uint64 EncodePos(int sid, int l, int r) {
+  static uint64_t EncodePos(int sid, int l, int r) {
     CHECK_GE(l, 0);
     CHECK_GE(r, 0);
-    CHECK_LE(l, kuint16max);
-    CHECK_LE(r, kuint16max);
-    const uint64 n = (static_cast<uint64>(sid) << 32 | (l << 16 | r));
+    CHECK_LE(l, std::numeric_limits<uint16_t>::max());
+    CHECK_LE(r, std::numeric_limits<uint16_t>::max());
+    const uint64_t n = (static_cast<uint64_t>(sid) << 32 | (l << 16 | r));
     return n;
   }
 
-  // Decodes sid, left and right bigram index from uint64.
-  static Position DecodePos(uint64 n) {
+  // Decodes sid, left and right bigram index from uint64_t.
+  static Position DecodePos(uint64_t n) {
     Position p;
     p.sid = n >> 32;
     p.left = (n >> 16) & 0xffff;
     p.right = n & 0xffff;
     return p;
   }
 
@@ -107,15 +109,15 @@
   void ResetFreq(int sid, int left, int right, const Symbol *best);
 
   // Updates |active_symbols_| by copying the top 5% frequent symbols in
   // symbols_cache_.
   void UpdateActiveSymbols();
 
   // All unique symbols. Key is a fingerprint of Symbol.
-  absl::flat_hash_map<uint64, Symbol *> symbols_cache_;
+  absl::flat_hash_map<uint64_t, Symbol *> symbols_cache_;
 
   // Set of symbols from which we find the best symbol in each iteration.
   std::set<Symbol *> active_symbols_;
 
   // Stores symbols allocated in heap so that we can delete them at onece.
   std::vector<Symbol *> allocated_;
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/bpe_model_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/bpe_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/builder.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.cc`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "builder.h"
+
 #include <algorithm>
 #include <functional>
 #include <utility>
 
-#include "builder.h"
 #include "filesystem.h"
 #include "third_party/absl/strings/str_join.h"
 #include "third_party/absl/strings/str_replace.h"
 #include "third_party/absl/strings/str_split.h"
 #include "third_party/absl/strings/strip.h"
 
 #ifdef ENABLE_NFKC_COMPILE
@@ -43,14 +44,20 @@
 namespace normalizer {
 namespace {
 
 constexpr int kMaxUnicode = 0x10FFFF;
 
 static constexpr char kDefaultNormalizerName[] = "nfkc";
 
+#ifndef ENABLE_NFKC_COMPILE
+static constexpr char kCompileError[] =
+    "NFK compile is not enabled. rebuild with ./configure "
+    "--enable-nfkc-compile";
+#endif
+
 #ifdef ENABLE_NFKC_COMPILE
 // Normalize `input` with ICU's normalizer with `mode`.
 Builder::Chars UnicodeNormalize(UNormalizationMode mode,
                                 const Builder::Chars &input) {
   const std::string utf8 = string_util::UnicodeTextToUTF8(input);
   CHECK(!utf8.empty());
 
@@ -261,15 +268,15 @@
 
   traverse(0, 0);
 
   return util::OkStatus();
 }
 
 // static
-util::Status Builder::GetPrecompiledCharsMap(const std::string &name,
+util::Status Builder::GetPrecompiledCharsMap(absl::string_view name,
                                              std::string *output) {
   CHECK_OR_RETURN(output);
 
   if (name == "identity") {
     output->clear();
     return util::OkStatus();
   }
@@ -334,16 +341,15 @@
     }
   }
 
   RETURN_IF_ERROR(RemoveRedundantMap(&nfkc_map));
   *chars_map = std::move(nfkc_map);
 
 #else
-  LOG(ERROR) << "NFKC compile is not enabled."
-             << " rebuild with ./configure --enable-nfkc-compile";
+  LOG(ERROR) << kCompileError;
 #endif
 
   return util::OkStatus();
 }
 
 util::Status Builder::BuildNmtNFKCMap(CharsMap *chars_map) {
 #ifdef ENABLE_NFKC_COMPILE
@@ -363,15 +369,15 @@
   nfkc_map[{0x200F}] = {0x20};  // RIGHT-TO-LEFT MARK
   nfkc_map[{0x2028}] = {0x20};  // LINE SEPARATOR
   nfkc_map[{0x2029}] = {0x20};  // PARAGRAPH SEPARATOR
   nfkc_map[{0x2581}] = {0x20};  // LOWER ONE EIGHT BLOCK
   nfkc_map[{0xFEFF}] = {0x20};  // ZERO WIDTH NO-BREAK
   nfkc_map[{0xFFFD}] = {0x20};  // REPLACEMENT CHARACTER
   nfkc_map[{0x200C}] = {0x20};  // ZERO WIDTH NON-JOINER
-//  nfkc_map[{0x200D}] = {0x20};  // ZERO WIDTH JOINER
+  //  nfkc_map[{0x200D}] = {0x20};  // ZERO WIDTH JOINER
 
   // Ascii Control characters
   nfkc_map[{0x0001}] = {};
   nfkc_map[{0x0002}] = {};
   nfkc_map[{0x0003}] = {};
   nfkc_map[{0x0004}] = {};
   nfkc_map[{0x0005}] = {};
@@ -408,16 +414,15 @@
   nfkc_map.erase({0xFF5E});
 
   RETURN_IF_ERROR(RemoveRedundantMap(&nfkc_map));
 
   *chars_map = std::move(nfkc_map);
 
 #else
-  LOG(ERROR) << "NFKC compile is not enabled."
-             << " rebuild with ./configure --enable-nfkc-compile";
+  LOG(ERROR) << kCompileError;
 #endif
 
   return util::OkStatus();
 }
 
 // static
 util::Status Builder::MergeUnicodeCaseFoldMap(Builder::CharsMap *chars_map) {
@@ -448,37 +453,54 @@
 util::Status Builder::BuildNFKC_CFMap(CharsMap *chars_map) {
 #ifdef ENABLE_NFKC_COMPILE
   CharsMap nfkc_map;
   RETURN_IF_ERROR(Builder::BuildNFKCMap(&nfkc_map));
   RETURN_IF_ERROR(Builder::MergeUnicodeCaseFoldMap(&nfkc_map));
   *chars_map = std::move(nfkc_map);
 #else
-  LOG(ERROR) << "NFKC_CF compile is not enabled."
-             << " rebuild with ./configure --enable-nfkc-compile";
+  LOG(ERROR) << kCompileError;
 #endif
 
   return util::OkStatus();
 }
 
 //  static
 util::Status Builder::BuildNmtNFKC_CFMap(CharsMap *chars_map) {
 #ifdef ENABLE_NFKC_COMPILE
   CharsMap nfkc_map;
   RETURN_IF_ERROR(Builder::BuildNmtNFKCMap(&nfkc_map));
   RETURN_IF_ERROR(Builder::MergeUnicodeCaseFoldMap(&nfkc_map));
   *chars_map = std::move(nfkc_map);
 #else
-  LOG(ERROR) << "NMT_NFKC_CF compile is not enabled."
-             << " rebuild with ./configure --enable-nfkc-compile";
+  LOG(ERROR) << kCompileError;
 #endif
 
   return util::OkStatus();
 }
 
 // static
+util::Status Builder::BuildNFKDMap(CharsMap *chars_map) {
+#ifdef ENABLE_NFKC_COMPILE
+  constexpr int kMaxUnicode = 0x10FFFF;
+  for (char32 cp = 1; cp <= kMaxUnicode; ++cp) {
+    if (!U_IS_UNICODE_CHAR(cp)) {
+      continue;
+    }
+    const auto nfkd = ToNFKD({cp});
+    if (nfkd.size() >= 2 || (nfkd.size() == 1 && nfkd[0] != cp)) {
+      (*chars_map)[{cp}] = nfkd;
+    }
+  }
+#else
+  LOG(ERROR) << kCompileError;
+#endif
+  return util::OkStatus();
+}
+
+// static
 util::Status Builder::LoadCharsMap(absl::string_view filename,
                                    CharsMap *chars_map) {
   LOG(INFO) << "Loading mapping file: " << filename.data();
   CHECK_OR_RETURN(chars_map);
 
   auto input = filesystem::NewReadableFile(filename);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/builder.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder.h`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                                       std::string *output);
 
   // Decompiles `blob` into `chars_map`.
   static util::Status DecompileCharsMap(absl::string_view blob,
                                         CharsMap *chars_map);
 
   // Returns a pre-compiled binary index with `name`.
-  static util::Status GetPrecompiledCharsMap(const std::string &name,
+  static util::Status GetPrecompiledCharsMap(absl::string_view name,
                                              std::string *output);
 
   // Makes a normalization mapping based on NFKC.
   //
   // Note that Normalizer/Builder classes do not support
   // full NFKC normalization, since full NFKC normalization cannot
   // be implemented with a simple longest matching string-to-string
@@ -100,14 +100,17 @@
 
   // Makes NFKC with Unicode case folding.
   static util::Status BuildNFKC_CFMap(CharsMap *chars_map);
 
   // Makes NMT NFKC with Unicode case folding.
   static util::Status BuildNmtNFKC_CFMap(CharsMap *chars_map);
 
+  // Given NFKC maps, convert them to NFKD.
+  static util::Status BuildNFKDMap(CharsMap *chars_map);
+
   // Builds Chars map save in `filename`.
   // Format:
   // src_uchar1 src_uchar2 ... <tab> trg_uchar1 trg_uchar2...
   // (src|trg)_ucharX must be a hex of Unicode code point.
   static util::Status LoadCharsMap(absl::string_view filename,
                                    CharsMap *chars_map);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/builder_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builder_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece.pb.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece.pb.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece.pb.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.cc`

 * *Files 2% similar despite different names*

```diff
@@ -281,99 +281,111 @@
   static void set_has_input_format(HasBits* has_bits) {
     (*has_bits)[0] |= 2u;
   }
   static void set_has_model_prefix(HasBits* has_bits) {
     (*has_bits)[0] |= 1u;
   }
   static void set_has_model_type(HasBits* has_bits) {
-    (*has_bits)[0] |= 524288u;
+    (*has_bits)[0] |= 8388608u;
   }
   static void set_has_vocab_size(HasBits* has_bits) {
-    (*has_bits)[0] |= 1048576u;
+    (*has_bits)[0] |= 16777216u;
   }
   static void set_has_self_test_sample_size(HasBits* has_bits) {
-    (*has_bits)[0] |= 256u;
+    (*has_bits)[0] |= 512u;
   }
-  static void set_has_character_coverage(HasBits* has_bits) {
+  static void set_has_enable_differential_privacy(HasBits* has_bits) {
+    (*has_bits)[0] |= 8192u;
+  }
+  static void set_has_differential_privacy_noise_level(HasBits* has_bits) {
     (*has_bits)[0] |= 2097152u;
   }
+  static void set_has_differential_privacy_clipping_threshold(HasBits* has_bits) {
+    (*has_bits)[0] |= 4194304u;
+  }
+  static void set_has_character_coverage(HasBits* has_bits) {
+    (*has_bits)[0] |= 33554432u;
+  }
   static void set_has_input_sentence_size(HasBits* has_bits) {
-    (*has_bits)[0] |= 1024u;
+    (*has_bits)[0] |= 2048u;
   }
   static void set_has_shuffle_input_sentence(HasBits* has_bits) {
-    (*has_bits)[0] |= 268435456u;
+    (*has_bits)[1] |= 1u;
   }
   static void set_has_mining_sentence_size(HasBits* has_bits) {
-    (*has_bits)[0] |= 512u;
+    (*has_bits)[0] |= 1024u;
   }
   static void set_has_training_sentence_size(HasBits* has_bits) {
-    (*has_bits)[0] |= 2048u;
+    (*has_bits)[0] |= 4096u;
   }
   static void set_has_seed_sentencepiece_size(HasBits* has_bits) {
-    (*has_bits)[0] |= 4194304u;
+    (*has_bits)[0] |= 67108864u;
   }
   static void set_has_shrinking_factor(HasBits* has_bits) {
-    (*has_bits)[0] |= 8388608u;
+    (*has_bits)[0] |= 134217728u;
   }
   static void set_has_max_sentence_length(HasBits* has_bits) {
-    (*has_bits)[0] |= 67108864u;
+    (*has_bits)[0] |= 1073741824u;
   }
   static void set_has_num_threads(HasBits* has_bits) {
-    (*has_bits)[0] |= 16777216u;
+    (*has_bits)[0] |= 268435456u;
   }
   static void set_has_num_sub_iterations(HasBits* has_bits) {
-    (*has_bits)[0] |= 33554432u;
+    (*has_bits)[0] |= 536870912u;
   }
   static void set_has_max_sentencepiece_length(HasBits* has_bits) {
-    (*has_bits)[0] |= 134217728u;
+    (*has_bits)[0] |= 2147483648u;
   }
   static void set_has_split_by_unicode_script(HasBits* has_bits) {
-    (*has_bits)[0] |= 536870912u;
+    (*has_bits)[1] |= 2u;
   }
   static void set_has_split_by_number(HasBits* has_bits) {
-    (*has_bits)[0] |= 1073741824u;
+    (*has_bits)[1] |= 4u;
   }
   static void set_has_split_by_whitespace(HasBits* has_bits) {
-    (*has_bits)[0] |= 2147483648u;
+    (*has_bits)[1] |= 8u;
   }
   static void set_has_treat_whitespace_as_suffix(HasBits* has_bits) {
-    (*has_bits)[0] |= 4096u;
+    (*has_bits)[0] |= 16384u;
   }
   static void set_has_allow_whitespace_only_pieces(HasBits* has_bits) {
-    (*has_bits)[0] |= 8192u;
+    (*has_bits)[0] |= 32768u;
   }
   static void set_has_split_digits(HasBits* has_bits) {
-    (*has_bits)[0] |= 16384u;
+    (*has_bits)[0] |= 65536u;
+  }
+  static void set_has_pretokenization_delimiter(HasBits* has_bits) {
+    (*has_bits)[0] |= 256u;
   }
   static void set_has_required_chars(HasBits* has_bits) {
     (*has_bits)[0] |= 4u;
   }
   static void set_has_byte_fallback(HasBits* has_bits) {
-    (*has_bits)[0] |= 32768u;
+    (*has_bits)[0] |= 131072u;
   }
   static void set_has_vocabulary_output_piece_score(HasBits* has_bits) {
-    (*has_bits)[1] |= 1u;
+    (*has_bits)[1] |= 16u;
   }
   static void set_has_hard_vocab_limit(HasBits* has_bits) {
-    (*has_bits)[1] |= 2u;
+    (*has_bits)[1] |= 32u;
   }
   static void set_has_use_all_vocab(HasBits* has_bits) {
-    (*has_bits)[0] |= 131072u;
+    (*has_bits)[0] |= 262144u;
   }
   static void set_has_unk_id(HasBits* has_bits) {
-    (*has_bits)[0] |= 65536u;
+    (*has_bits)[0] |= 1048576u;
   }
   static void set_has_bos_id(HasBits* has_bits) {
-    (*has_bits)[1] |= 4u;
+    (*has_bits)[1] |= 64u;
   }
   static void set_has_eos_id(HasBits* has_bits) {
-    (*has_bits)[1] |= 8u;
+    (*has_bits)[1] |= 128u;
   }
   static void set_has_pad_id(HasBits* has_bits) {
-    (*has_bits)[1] |= 16u;
+    (*has_bits)[1] |= 256u;
   }
   static void set_has_unk_piece(HasBits* has_bits) {
     (*has_bits)[0] |= 16u;
   }
   static void set_has_bos_piece(HasBits* has_bits) {
     (*has_bits)[0] |= 32u;
   }
@@ -383,15 +395,15 @@
   static void set_has_pad_piece(HasBits* has_bits) {
     (*has_bits)[0] |= 128u;
   }
   static void set_has_unk_surface(HasBits* has_bits) {
     (*has_bits)[0] |= 8u;
   }
   static void set_has_train_extremely_large_corpus(HasBits* has_bits) {
-    (*has_bits)[0] |= 262144u;
+    (*has_bits)[0] |= 524288u;
   }
 };
 
 const ::PROTOBUF_NAMESPACE_ID::internal::LazyString TrainerSpec::_i_give_permission_to_break_this_code_default_unk_piece_{{{"<unk>", 5}}, {nullptr}};
 const ::PROTOBUF_NAMESPACE_ID::internal::LazyString TrainerSpec::_i_give_permission_to_break_this_code_default_bos_piece_{{{"<s>", 3}}, {nullptr}};
 const ::PROTOBUF_NAMESPACE_ID::internal::LazyString TrainerSpec::_i_give_permission_to_break_this_code_default_eos_piece_{{{"</s>", 4}}, {nullptr}};
 const ::PROTOBUF_NAMESPACE_ID::internal::LazyString TrainerSpec::_i_give_permission_to_break_this_code_default_pad_piece_{{{"<pad>", 5}}, {nullptr}};
@@ -452,14 +464,19 @@
       GetArena());
   }
   pad_piece_.UnsafeSetDefault(nullptr);
   if (from._internal_has_pad_piece()) {
     pad_piece_.Set(::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr::NonEmptyDefault{}, from._internal_pad_piece(), 
       GetArena());
   }
+  pretokenization_delimiter_.UnsafeSetDefault(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited());
+  if (from._internal_has_pretokenization_delimiter()) {
+    pretokenization_delimiter_.Set(::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr::EmptyDefault{}, from._internal_pretokenization_delimiter(), 
+      GetArena());
+  }
   ::memcpy(&self_test_sample_size_, &from.self_test_sample_size_,
     static_cast<size_t>(reinterpret_cast<char*>(&pad_id_) -
     reinterpret_cast<char*>(&self_test_sample_size_)) + sizeof(pad_id_));
   // @@protoc_insertion_point(copy_constructor:sentencepiece.TrainerSpec)
 }
 
 void TrainerSpec::SharedCtor() {
@@ -468,18 +485,19 @@
   input_format_.UnsafeSetDefault(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited());
   required_chars_.UnsafeSetDefault(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited());
   unk_surface_.UnsafeSetDefault(nullptr);
   unk_piece_.UnsafeSetDefault(nullptr);
   bos_piece_.UnsafeSetDefault(nullptr);
   eos_piece_.UnsafeSetDefault(nullptr);
   pad_piece_.UnsafeSetDefault(nullptr);
+  pretokenization_delimiter_.UnsafeSetDefault(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited());
   ::memset(reinterpret_cast<char*>(this) + static_cast<size_t>(
       reinterpret_cast<char*>(&self_test_sample_size_) - reinterpret_cast<char*>(this)),
-      0, static_cast<size_t>(reinterpret_cast<char*>(&train_extremely_large_corpus_) -
-      reinterpret_cast<char*>(&self_test_sample_size_)) + sizeof(train_extremely_large_corpus_));
+      0, static_cast<size_t>(reinterpret_cast<char*>(&differential_privacy_clipping_threshold_) -
+      reinterpret_cast<char*>(&self_test_sample_size_)) + sizeof(differential_privacy_clipping_threshold_));
   model_type_ = 1;
   vocab_size_ = 8000;
   character_coverage_ = 0.9995f;
   seed_sentencepiece_size_ = 1000000;
   shrinking_factor_ = 0.75f;
   num_threads_ = 16;
   num_sub_iterations_ = 2;
@@ -508,14 +526,15 @@
   input_format_.DestroyNoArena(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited());
   required_chars_.DestroyNoArena(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited());
   unk_surface_.DestroyNoArena(nullptr);
   unk_piece_.DestroyNoArena(nullptr);
   bos_piece_.DestroyNoArena(nullptr);
   eos_piece_.DestroyNoArena(nullptr);
   pad_piece_.DestroyNoArena(nullptr);
+  pretokenization_delimiter_.DestroyNoArena(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited());
 }
 
 void TrainerSpec::ArenaDtor(void* object) {
   TrainerSpec* _this = reinterpret_cast< TrainerSpec* >(object);
   (void)_this;
 }
 void TrainerSpec::RegisterArenaDtor(::PROTOBUF_NAMESPACE_ID::Arena*) {
@@ -563,47 +582,50 @@
     if (cached_has_bits & 0x00000040u) {
       eos_piece_.ClearToDefault(::sentencepiece::TrainerSpec::_i_give_permission_to_break_this_code_default_eos_piece_, GetArena());
        }
     if (cached_has_bits & 0x00000080u) {
       pad_piece_.ClearToDefault(::sentencepiece::TrainerSpec::_i_give_permission_to_break_this_code_default_pad_piece_, GetArena());
        }
   }
-  if (cached_has_bits & 0x0000ff00u) {
+  if (cached_has_bits & 0x00000100u) {
+    pretokenization_delimiter_.ClearNonDefaultToEmpty();
+  }
+  if (cached_has_bits & 0x0000fe00u) {
     ::memset(&self_test_sample_size_, 0, static_cast<size_t>(
-        reinterpret_cast<char*>(&byte_fallback_) -
-        reinterpret_cast<char*>(&self_test_sample_size_)) + sizeof(byte_fallback_));
+        reinterpret_cast<char*>(&allow_whitespace_only_pieces_) -
+        reinterpret_cast<char*>(&self_test_sample_size_)) + sizeof(allow_whitespace_only_pieces_));
   }
   if (cached_has_bits & 0x00ff0000u) {
-    ::memset(&unk_id_, 0, static_cast<size_t>(
-        reinterpret_cast<char*>(&train_extremely_large_corpus_) -
-        reinterpret_cast<char*>(&unk_id_)) + sizeof(train_extremely_large_corpus_));
+    ::memset(&split_digits_, 0, static_cast<size_t>(
+        reinterpret_cast<char*>(&differential_privacy_clipping_threshold_) -
+        reinterpret_cast<char*>(&split_digits_)) + sizeof(differential_privacy_clipping_threshold_));
     model_type_ = 1;
+  }
+  if (cached_has_bits & 0xff000000u) {
     vocab_size_ = 8000;
     character_coverage_ = 0.9995f;
     seed_sentencepiece_size_ = 1000000;
     shrinking_factor_ = 0.75f;
-  }
-  if (cached_has_bits & 0xff000000u) {
     num_threads_ = 16;
     num_sub_iterations_ = 2;
     max_sentence_length_ = 4192;
     max_sentencepiece_length_ = 16;
+  }
+  cached_has_bits = _has_bits_[1];
+  if (cached_has_bits & 0x000000ffu) {
     shuffle_input_sentence_ = true;
     split_by_unicode_script_ = true;
     split_by_number_ = true;
     split_by_whitespace_ = true;
-  }
-  cached_has_bits = _has_bits_[1];
-  if (cached_has_bits & 0x0000001fu) {
     vocabulary_output_piece_score_ = true;
     hard_vocab_limit_ = true;
     bos_id_ = 1;
     eos_id_ = 2;
-    pad_id_ = -1;
   }
+  pad_id_ = -1;
   _has_bits_.Clear();
   _internal_metadata_.Clear<std::string>();
 }
 
 const char* TrainerSpec::_InternalParse(const char* ptr, ::PROTOBUF_NAMESPACE_ID::internal::ParseContext* ctx) {
 #define CHK_(x) if (PROTOBUF_PREDICT_FALSE(!(x))) goto failure
   while (!ctx->Done(&ptr)) {
@@ -959,14 +981,46 @@
       case 49:
         if (PROTOBUF_PREDICT_TRUE(static_cast<::PROTOBUF_NAMESPACE_ID::uint8>(tag) == 136)) {
           _Internal::set_has_train_extremely_large_corpus(&_has_bits_);
           train_extremely_large_corpus_ = ::PROTOBUF_NAMESPACE_ID::internal::ReadVarint64(&ptr);
           CHK_(ptr);
         } else goto handle_unusual;
         continue;
+      // optional bool enable_differential_privacy = 50 [default = false];
+      case 50:
+        if (PROTOBUF_PREDICT_TRUE(static_cast<::PROTOBUF_NAMESPACE_ID::uint8>(tag) == 144)) {
+          _Internal::set_has_enable_differential_privacy(&_has_bits_);
+          enable_differential_privacy_ = ::PROTOBUF_NAMESPACE_ID::internal::ReadVarint64(&ptr);
+          CHK_(ptr);
+        } else goto handle_unusual;
+        continue;
+      // optional float differential_privacy_noise_level = 51 [default = 0];
+      case 51:
+        if (PROTOBUF_PREDICT_TRUE(static_cast<::PROTOBUF_NAMESPACE_ID::uint8>(tag) == 157)) {
+          _Internal::set_has_differential_privacy_noise_level(&_has_bits_);
+          differential_privacy_noise_level_ = ::PROTOBUF_NAMESPACE_ID::internal::UnalignedLoad<float>(ptr);
+          ptr += sizeof(float);
+        } else goto handle_unusual;
+        continue;
+      // optional uint64 differential_privacy_clipping_threshold = 52 [default = 0];
+      case 52:
+        if (PROTOBUF_PREDICT_TRUE(static_cast<::PROTOBUF_NAMESPACE_ID::uint8>(tag) == 160)) {
+          _Internal::set_has_differential_privacy_clipping_threshold(&_has_bits_);
+          differential_privacy_clipping_threshold_ = ::PROTOBUF_NAMESPACE_ID::internal::ReadVarint64(&ptr);
+          CHK_(ptr);
+        } else goto handle_unusual;
+        continue;
+      // optional string pretokenization_delimiter = 53 [default = ""];
+      case 53:
+        if (PROTOBUF_PREDICT_TRUE(static_cast<::PROTOBUF_NAMESPACE_ID::uint8>(tag) == 170)) {
+          auto str = _internal_mutable_pretokenization_delimiter();
+          ptr = ::PROTOBUF_NAMESPACE_ID::internal::InlineGreedyStringParser(str, ptr, ctx);
+          CHK_(ptr);
+        } else goto handle_unusual;
+        continue;
       default: {
       handle_unusual:
         if ((tag & 7) == 4 || tag == 0) {
           ctx->SetLastTag(tag);
           goto success;
         }
       if ((1600u <= tag)) {
@@ -1007,142 +1061,146 @@
   // optional string model_prefix = 2;
   if (cached_has_bits & 0x00000001u) {
     target = stream->WriteStringMaybeAliased(
         2, this->_internal_model_prefix(), target);
   }
 
   // optional .sentencepiece.TrainerSpec.ModelType model_type = 3 [default = UNIGRAM];
-  if (cached_has_bits & 0x00080000u) {
+  if (cached_has_bits & 0x00800000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteEnumToArray(
       3, this->_internal_model_type(), target);
   }
 
   // optional int32 vocab_size = 4 [default = 8000];
-  if (cached_has_bits & 0x00100000u) {
+  if (cached_has_bits & 0x01000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(4, this->_internal_vocab_size(), target);
   }
 
   // repeated string accept_language = 5;
   for (int i = 0, n = this->_internal_accept_language_size(); i < n; i++) {
     const auto& s = this->_internal_accept_language(i);
     target = stream->WriteString(5, s, target);
   }
 
   // optional int32 self_test_sample_size = 6 [default = 0];
-  if (cached_has_bits & 0x00000100u) {
+  if (cached_has_bits & 0x00000200u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(6, this->_internal_self_test_sample_size(), target);
   }
 
   // optional string input_format = 7;
   if (cached_has_bits & 0x00000002u) {
     target = stream->WriteStringMaybeAliased(
         7, this->_internal_input_format(), target);
   }
 
   // optional float character_coverage = 10 [default = 0.9995];
-  if (cached_has_bits & 0x00200000u) {
+  if (cached_has_bits & 0x02000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteFloatToArray(10, this->_internal_character_coverage(), target);
   }
 
   // optional uint64 input_sentence_size = 11 [default = 0];
-  if (cached_has_bits & 0x00000400u) {
+  if (cached_has_bits & 0x00000800u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteUInt64ToArray(11, this->_internal_input_sentence_size(), target);
   }
 
   // optional int32 mining_sentence_size = 12 [deprecated = true];
-  if (cached_has_bits & 0x00000200u) {
+  if (cached_has_bits & 0x00000400u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(12, this->_internal_mining_sentence_size(), target);
   }
 
   // optional int32 training_sentence_size = 13 [deprecated = true];
-  if (cached_has_bits & 0x00000800u) {
+  if (cached_has_bits & 0x00001000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(13, this->_internal_training_sentence_size(), target);
   }
 
   // optional int32 seed_sentencepiece_size = 14 [default = 1000000];
-  if (cached_has_bits & 0x00400000u) {
+  if (cached_has_bits & 0x04000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(14, this->_internal_seed_sentencepiece_size(), target);
   }
 
   // optional float shrinking_factor = 15 [default = 0.75];
-  if (cached_has_bits & 0x00800000u) {
+  if (cached_has_bits & 0x08000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteFloatToArray(15, this->_internal_shrinking_factor(), target);
   }
 
   // optional int32 num_threads = 16 [default = 16];
-  if (cached_has_bits & 0x01000000u) {
+  if (cached_has_bits & 0x10000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(16, this->_internal_num_threads(), target);
   }
 
   // optional int32 num_sub_iterations = 17 [default = 2];
-  if (cached_has_bits & 0x02000000u) {
+  if (cached_has_bits & 0x20000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(17, this->_internal_num_sub_iterations(), target);
   }
 
   // optional int32 max_sentence_length = 18 [default = 4192];
-  if (cached_has_bits & 0x04000000u) {
+  if (cached_has_bits & 0x40000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(18, this->_internal_max_sentence_length(), target);
   }
 
+  cached_has_bits = _has_bits_[1];
   // optional bool shuffle_input_sentence = 19 [default = true];
-  if (cached_has_bits & 0x10000000u) {
+  if (cached_has_bits & 0x00000001u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(19, this->_internal_shuffle_input_sentence(), target);
   }
 
+  cached_has_bits = _has_bits_[0];
   // optional int32 max_sentencepiece_length = 20 [default = 16];
-  if (cached_has_bits & 0x08000000u) {
+  if (cached_has_bits & 0x80000000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(20, this->_internal_max_sentencepiece_length(), target);
   }
 
+  cached_has_bits = _has_bits_[1];
   // optional bool split_by_unicode_script = 21 [default = true];
-  if (cached_has_bits & 0x20000000u) {
+  if (cached_has_bits & 0x00000002u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(21, this->_internal_split_by_unicode_script(), target);
   }
 
   // optional bool split_by_whitespace = 22 [default = true];
-  if (cached_has_bits & 0x80000000u) {
+  if (cached_has_bits & 0x00000008u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(22, this->_internal_split_by_whitespace(), target);
   }
 
   // optional bool split_by_number = 23 [default = true];
-  if (cached_has_bits & 0x40000000u) {
+  if (cached_has_bits & 0x00000004u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(23, this->_internal_split_by_number(), target);
   }
 
+  cached_has_bits = _has_bits_[0];
   // optional bool treat_whitespace_as_suffix = 24 [default = false];
-  if (cached_has_bits & 0x00001000u) {
+  if (cached_has_bits & 0x00004000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(24, this->_internal_treat_whitespace_as_suffix(), target);
   }
 
   // optional bool split_digits = 25 [default = false];
-  if (cached_has_bits & 0x00004000u) {
+  if (cached_has_bits & 0x00010000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(25, this->_internal_split_digits(), target);
   }
 
   // optional bool allow_whitespace_only_pieces = 26 [default = false];
-  if (cached_has_bits & 0x00002000u) {
+  if (cached_has_bits & 0x00008000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(26, this->_internal_allow_whitespace_only_pieces(), target);
   }
 
   // repeated string control_symbols = 30;
   for (int i = 0, n = this->_internal_control_symbols_size(); i < n; i++) {
     const auto& s = this->_internal_control_symbols(i);
@@ -1153,65 +1211,65 @@
   for (int i = 0, n = this->_internal_user_defined_symbols_size(); i < n; i++) {
     const auto& s = this->_internal_user_defined_symbols(i);
     target = stream->WriteString(31, s, target);
   }
 
   cached_has_bits = _has_bits_[1];
   // optional bool vocabulary_output_piece_score = 32 [default = true];
-  if (cached_has_bits & 0x00000001u) {
+  if (cached_has_bits & 0x00000010u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(32, this->_internal_vocabulary_output_piece_score(), target);
   }
 
   // optional bool hard_vocab_limit = 33 [default = true];
-  if (cached_has_bits & 0x00000002u) {
+  if (cached_has_bits & 0x00000020u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(33, this->_internal_hard_vocab_limit(), target);
   }
 
   cached_has_bits = _has_bits_[0];
   // optional bool use_all_vocab = 34 [default = false];
-  if (cached_has_bits & 0x00020000u) {
+  if (cached_has_bits & 0x00040000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(34, this->_internal_use_all_vocab(), target);
   }
 
   // optional bool byte_fallback = 35 [default = false];
-  if (cached_has_bits & 0x00008000u) {
+  if (cached_has_bits & 0x00020000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(35, this->_internal_byte_fallback(), target);
   }
 
   // optional string required_chars = 36;
   if (cached_has_bits & 0x00000004u) {
     target = stream->WriteStringMaybeAliased(
         36, this->_internal_required_chars(), target);
   }
 
   // optional int32 unk_id = 40 [default = 0];
-  if (cached_has_bits & 0x00010000u) {
+  if (cached_has_bits & 0x00100000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(40, this->_internal_unk_id(), target);
   }
 
   cached_has_bits = _has_bits_[1];
   // optional int32 bos_id = 41 [default = 1];
-  if (cached_has_bits & 0x00000004u) {
+  if (cached_has_bits & 0x00000040u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(41, this->_internal_bos_id(), target);
   }
 
   // optional int32 eos_id = 42 [default = 2];
-  if (cached_has_bits & 0x00000008u) {
+  if (cached_has_bits & 0x00000080u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(42, this->_internal_eos_id(), target);
   }
 
   // optional int32 pad_id = 43 [default = -1];
-  if (cached_has_bits & 0x00000010u) {
+  if (cached_has_bits & 0x00000100u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteInt32ToArray(43, this->_internal_pad_id(), target);
   }
 
   cached_has_bits = _has_bits_[0];
   // optional string unk_surface = 44 [default = " \342\201\207 "];
   if (cached_has_bits & 0x00000008u) {
@@ -1240,19 +1298,43 @@
   // optional string pad_piece = 48 [default = "<pad>"];
   if (cached_has_bits & 0x00000080u) {
     target = stream->WriteStringMaybeAliased(
         48, this->_internal_pad_piece(), target);
   }
 
   // optional bool train_extremely_large_corpus = 49 [default = false];
-  if (cached_has_bits & 0x00040000u) {
+  if (cached_has_bits & 0x00080000u) {
     target = stream->EnsureSpace(target);
     target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(49, this->_internal_train_extremely_large_corpus(), target);
   }
 
+  // optional bool enable_differential_privacy = 50 [default = false];
+  if (cached_has_bits & 0x00002000u) {
+    target = stream->EnsureSpace(target);
+    target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteBoolToArray(50, this->_internal_enable_differential_privacy(), target);
+  }
+
+  // optional float differential_privacy_noise_level = 51 [default = 0];
+  if (cached_has_bits & 0x00200000u) {
+    target = stream->EnsureSpace(target);
+    target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteFloatToArray(51, this->_internal_differential_privacy_noise_level(), target);
+  }
+
+  // optional uint64 differential_privacy_clipping_threshold = 52 [default = 0];
+  if (cached_has_bits & 0x00400000u) {
+    target = stream->EnsureSpace(target);
+    target = ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::WriteUInt64ToArray(52, this->_internal_differential_privacy_clipping_threshold(), target);
+  }
+
+  // optional string pretokenization_delimiter = 53 [default = ""];
+  if (cached_has_bits & 0x00000100u) {
+    target = stream->WriteStringMaybeAliased(
+        53, this->_internal_pretokenization_delimiter(), target);
+  }
+
   // Extension range [200, 536870912)
   target = _extensions_._InternalSerialize(
       200, 536870912, target, stream);
 
   if (PROTOBUF_PREDICT_FALSE(_internal_metadata_.have_unknown_fields())) {
     target = stream->WriteRaw(_internal_metadata_.unknown_fields<std::string>(::PROTOBUF_NAMESPACE_ID::internal::GetEmptyString).data(),
         static_cast<int>(_internal_metadata_.unknown_fields<std::string>(::PROTOBUF_NAMESPACE_ID::internal::GetEmptyString).size()), target);
@@ -1359,196 +1441,220 @@
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::StringSize(
           this->_internal_pad_piece());
     }
 
   }
   if (cached_has_bits & 0x0000ff00u) {
-    // optional int32 self_test_sample_size = 6 [default = 0];
+    // optional string pretokenization_delimiter = 53 [default = ""];
     if (cached_has_bits & 0x00000100u) {
+      total_size += 2 +
+        ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::StringSize(
+          this->_internal_pretokenization_delimiter());
+    }
+
+    // optional int32 self_test_sample_size = 6 [default = 0];
+    if (cached_has_bits & 0x00000200u) {
       total_size += 1 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_self_test_sample_size());
     }
 
     // optional int32 mining_sentence_size = 12 [deprecated = true];
-    if (cached_has_bits & 0x00000200u) {
+    if (cached_has_bits & 0x00000400u) {
       total_size += 1 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_mining_sentence_size());
     }
 
     // optional uint64 input_sentence_size = 11 [default = 0];
-    if (cached_has_bits & 0x00000400u) {
+    if (cached_has_bits & 0x00000800u) {
       total_size += 1 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::UInt64Size(
           this->_internal_input_sentence_size());
     }
 
     // optional int32 training_sentence_size = 13 [deprecated = true];
-    if (cached_has_bits & 0x00000800u) {
+    if (cached_has_bits & 0x00001000u) {
       total_size += 1 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_training_sentence_size());
     }
 
+    // optional bool enable_differential_privacy = 50 [default = false];
+    if (cached_has_bits & 0x00002000u) {
+      total_size += 2 + 1;
+    }
+
     // optional bool treat_whitespace_as_suffix = 24 [default = false];
-    if (cached_has_bits & 0x00001000u) {
+    if (cached_has_bits & 0x00004000u) {
       total_size += 2 + 1;
     }
 
     // optional bool allow_whitespace_only_pieces = 26 [default = false];
-    if (cached_has_bits & 0x00002000u) {
+    if (cached_has_bits & 0x00008000u) {
       total_size += 2 + 1;
     }
 
+  }
+  if (cached_has_bits & 0x00ff0000u) {
     // optional bool split_digits = 25 [default = false];
-    if (cached_has_bits & 0x00004000u) {
+    if (cached_has_bits & 0x00010000u) {
       total_size += 2 + 1;
     }
 
     // optional bool byte_fallback = 35 [default = false];
-    if (cached_has_bits & 0x00008000u) {
+    if (cached_has_bits & 0x00020000u) {
+      total_size += 2 + 1;
+    }
+
+    // optional bool use_all_vocab = 34 [default = false];
+    if (cached_has_bits & 0x00040000u) {
+      total_size += 2 + 1;
+    }
+
+    // optional bool train_extremely_large_corpus = 49 [default = false];
+    if (cached_has_bits & 0x00080000u) {
       total_size += 2 + 1;
     }
 
-  }
-  if (cached_has_bits & 0x00ff0000u) {
     // optional int32 unk_id = 40 [default = 0];
-    if (cached_has_bits & 0x00010000u) {
+    if (cached_has_bits & 0x00100000u) {
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_unk_id());
     }
 
-    // optional bool use_all_vocab = 34 [default = false];
-    if (cached_has_bits & 0x00020000u) {
-      total_size += 2 + 1;
+    // optional float differential_privacy_noise_level = 51 [default = 0];
+    if (cached_has_bits & 0x00200000u) {
+      total_size += 2 + 4;
     }
 
-    // optional bool train_extremely_large_corpus = 49 [default = false];
-    if (cached_has_bits & 0x00040000u) {
-      total_size += 2 + 1;
+    // optional uint64 differential_privacy_clipping_threshold = 52 [default = 0];
+    if (cached_has_bits & 0x00400000u) {
+      total_size += 2 +
+        ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::UInt64Size(
+          this->_internal_differential_privacy_clipping_threshold());
     }
 
     // optional .sentencepiece.TrainerSpec.ModelType model_type = 3 [default = UNIGRAM];
-    if (cached_has_bits & 0x00080000u) {
+    if (cached_has_bits & 0x00800000u) {
       total_size += 1 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::EnumSize(this->_internal_model_type());
     }
 
+  }
+  if (cached_has_bits & 0xff000000u) {
     // optional int32 vocab_size = 4 [default = 8000];
-    if (cached_has_bits & 0x00100000u) {
+    if (cached_has_bits & 0x01000000u) {
       total_size += 1 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_vocab_size());
     }
 
     // optional float character_coverage = 10 [default = 0.9995];
-    if (cached_has_bits & 0x00200000u) {
+    if (cached_has_bits & 0x02000000u) {
       total_size += 1 + 4;
     }
 
     // optional int32 seed_sentencepiece_size = 14 [default = 1000000];
-    if (cached_has_bits & 0x00400000u) {
+    if (cached_has_bits & 0x04000000u) {
       total_size += 1 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_seed_sentencepiece_size());
     }
 
     // optional float shrinking_factor = 15 [default = 0.75];
-    if (cached_has_bits & 0x00800000u) {
+    if (cached_has_bits & 0x08000000u) {
       total_size += 1 + 4;
     }
 
-  }
-  if (cached_has_bits & 0xff000000u) {
     // optional int32 num_threads = 16 [default = 16];
-    if (cached_has_bits & 0x01000000u) {
+    if (cached_has_bits & 0x10000000u) {
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_num_threads());
     }
 
     // optional int32 num_sub_iterations = 17 [default = 2];
-    if (cached_has_bits & 0x02000000u) {
+    if (cached_has_bits & 0x20000000u) {
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_num_sub_iterations());
     }
 
     // optional int32 max_sentence_length = 18 [default = 4192];
-    if (cached_has_bits & 0x04000000u) {
+    if (cached_has_bits & 0x40000000u) {
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_max_sentence_length());
     }
 
     // optional int32 max_sentencepiece_length = 20 [default = 16];
-    if (cached_has_bits & 0x08000000u) {
+    if (cached_has_bits & 0x80000000u) {
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_max_sentencepiece_length());
     }
 
+  }
+  cached_has_bits = _has_bits_[1];
+  if (cached_has_bits & 0x000000ffu) {
     // optional bool shuffle_input_sentence = 19 [default = true];
-    if (cached_has_bits & 0x10000000u) {
+    if (cached_has_bits & 0x00000001u) {
       total_size += 2 + 1;
     }
 
     // optional bool split_by_unicode_script = 21 [default = true];
-    if (cached_has_bits & 0x20000000u) {
+    if (cached_has_bits & 0x00000002u) {
       total_size += 2 + 1;
     }
 
     // optional bool split_by_number = 23 [default = true];
-    if (cached_has_bits & 0x40000000u) {
+    if (cached_has_bits & 0x00000004u) {
       total_size += 2 + 1;
     }
 
     // optional bool split_by_whitespace = 22 [default = true];
-    if (cached_has_bits & 0x80000000u) {
+    if (cached_has_bits & 0x00000008u) {
       total_size += 2 + 1;
     }
 
-  }
-  cached_has_bits = _has_bits_[1];
-  if (cached_has_bits & 0x0000001fu) {
     // optional bool vocabulary_output_piece_score = 32 [default = true];
-    if (cached_has_bits & 0x00000001u) {
+    if (cached_has_bits & 0x00000010u) {
       total_size += 2 + 1;
     }
 
     // optional bool hard_vocab_limit = 33 [default = true];
-    if (cached_has_bits & 0x00000002u) {
+    if (cached_has_bits & 0x00000020u) {
       total_size += 2 + 1;
     }
 
     // optional int32 bos_id = 41 [default = 1];
-    if (cached_has_bits & 0x00000004u) {
+    if (cached_has_bits & 0x00000040u) {
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_bos_id());
     }
 
     // optional int32 eos_id = 42 [default = 2];
-    if (cached_has_bits & 0x00000008u) {
+    if (cached_has_bits & 0x00000080u) {
       total_size += 2 +
         ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
           this->_internal_eos_id());
     }
 
-    // optional int32 pad_id = 43 [default = -1];
-    if (cached_has_bits & 0x00000010u) {
-      total_size += 2 +
-        ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
-          this->_internal_pad_id());
-    }
-
   }
+  // optional int32 pad_id = 43 [default = -1];
+  if (cached_has_bits & 0x00000100u) {
+    total_size += 2 +
+      ::PROTOBUF_NAMESPACE_ID::internal::WireFormatLite::Int32Size(
+        this->_internal_pad_id());
+  }
+
   if (PROTOBUF_PREDICT_FALSE(_internal_metadata_.have_unknown_fields())) {
     total_size += _internal_metadata_.unknown_fields<std::string>(::PROTOBUF_NAMESPACE_ID::internal::GetEmptyString).size();
   }
   int cached_size = ::PROTOBUF_NAMESPACE_ID::internal::ToCachedSize(total_size);
   SetCachedSize(cached_size);
   return total_size;
 }
@@ -1596,112 +1702,124 @@
     }
     if (cached_has_bits & 0x00000080u) {
       _internal_set_pad_piece(from._internal_pad_piece());
     }
   }
   if (cached_has_bits & 0x0000ff00u) {
     if (cached_has_bits & 0x00000100u) {
-      self_test_sample_size_ = from.self_test_sample_size_;
+      _internal_set_pretokenization_delimiter(from._internal_pretokenization_delimiter());
     }
     if (cached_has_bits & 0x00000200u) {
-      mining_sentence_size_ = from.mining_sentence_size_;
+      self_test_sample_size_ = from.self_test_sample_size_;
     }
     if (cached_has_bits & 0x00000400u) {
-      input_sentence_size_ = from.input_sentence_size_;
+      mining_sentence_size_ = from.mining_sentence_size_;
     }
     if (cached_has_bits & 0x00000800u) {
-      training_sentence_size_ = from.training_sentence_size_;
+      input_sentence_size_ = from.input_sentence_size_;
     }
     if (cached_has_bits & 0x00001000u) {
-      treat_whitespace_as_suffix_ = from.treat_whitespace_as_suffix_;
+      training_sentence_size_ = from.training_sentence_size_;
     }
     if (cached_has_bits & 0x00002000u) {
-      allow_whitespace_only_pieces_ = from.allow_whitespace_only_pieces_;
+      enable_differential_privacy_ = from.enable_differential_privacy_;
     }
     if (cached_has_bits & 0x00004000u) {
-      split_digits_ = from.split_digits_;
+      treat_whitespace_as_suffix_ = from.treat_whitespace_as_suffix_;
     }
     if (cached_has_bits & 0x00008000u) {
-      byte_fallback_ = from.byte_fallback_;
+      allow_whitespace_only_pieces_ = from.allow_whitespace_only_pieces_;
     }
     _has_bits_[0] |= cached_has_bits;
   }
   if (cached_has_bits & 0x00ff0000u) {
     if (cached_has_bits & 0x00010000u) {
-      unk_id_ = from.unk_id_;
+      split_digits_ = from.split_digits_;
     }
     if (cached_has_bits & 0x00020000u) {
-      use_all_vocab_ = from.use_all_vocab_;
+      byte_fallback_ = from.byte_fallback_;
     }
     if (cached_has_bits & 0x00040000u) {
-      train_extremely_large_corpus_ = from.train_extremely_large_corpus_;
+      use_all_vocab_ = from.use_all_vocab_;
     }
     if (cached_has_bits & 0x00080000u) {
-      model_type_ = from.model_type_;
+      train_extremely_large_corpus_ = from.train_extremely_large_corpus_;
     }
     if (cached_has_bits & 0x00100000u) {
-      vocab_size_ = from.vocab_size_;
+      unk_id_ = from.unk_id_;
     }
     if (cached_has_bits & 0x00200000u) {
-      character_coverage_ = from.character_coverage_;
+      differential_privacy_noise_level_ = from.differential_privacy_noise_level_;
     }
     if (cached_has_bits & 0x00400000u) {
-      seed_sentencepiece_size_ = from.seed_sentencepiece_size_;
+      differential_privacy_clipping_threshold_ = from.differential_privacy_clipping_threshold_;
     }
     if (cached_has_bits & 0x00800000u) {
-      shrinking_factor_ = from.shrinking_factor_;
+      model_type_ = from.model_type_;
     }
     _has_bits_[0] |= cached_has_bits;
   }
   if (cached_has_bits & 0xff000000u) {
     if (cached_has_bits & 0x01000000u) {
-      num_threads_ = from.num_threads_;
+      vocab_size_ = from.vocab_size_;
     }
     if (cached_has_bits & 0x02000000u) {
-      num_sub_iterations_ = from.num_sub_iterations_;
+      character_coverage_ = from.character_coverage_;
     }
     if (cached_has_bits & 0x04000000u) {
-      max_sentence_length_ = from.max_sentence_length_;
+      seed_sentencepiece_size_ = from.seed_sentencepiece_size_;
     }
     if (cached_has_bits & 0x08000000u) {
-      max_sentencepiece_length_ = from.max_sentencepiece_length_;
+      shrinking_factor_ = from.shrinking_factor_;
     }
     if (cached_has_bits & 0x10000000u) {
-      shuffle_input_sentence_ = from.shuffle_input_sentence_;
+      num_threads_ = from.num_threads_;
     }
     if (cached_has_bits & 0x20000000u) {
-      split_by_unicode_script_ = from.split_by_unicode_script_;
+      num_sub_iterations_ = from.num_sub_iterations_;
     }
     if (cached_has_bits & 0x40000000u) {
-      split_by_number_ = from.split_by_number_;
+      max_sentence_length_ = from.max_sentence_length_;
     }
     if (cached_has_bits & 0x80000000u) {
-      split_by_whitespace_ = from.split_by_whitespace_;
+      max_sentencepiece_length_ = from.max_sentencepiece_length_;
     }
     _has_bits_[0] |= cached_has_bits;
   }
   cached_has_bits = from._has_bits_[1];
-  if (cached_has_bits & 0x0000001fu) {
+  if (cached_has_bits & 0x000000ffu) {
     if (cached_has_bits & 0x00000001u) {
-      vocabulary_output_piece_score_ = from.vocabulary_output_piece_score_;
+      shuffle_input_sentence_ = from.shuffle_input_sentence_;
     }
     if (cached_has_bits & 0x00000002u) {
-      hard_vocab_limit_ = from.hard_vocab_limit_;
+      split_by_unicode_script_ = from.split_by_unicode_script_;
     }
     if (cached_has_bits & 0x00000004u) {
-      bos_id_ = from.bos_id_;
+      split_by_number_ = from.split_by_number_;
     }
     if (cached_has_bits & 0x00000008u) {
-      eos_id_ = from.eos_id_;
+      split_by_whitespace_ = from.split_by_whitespace_;
     }
     if (cached_has_bits & 0x00000010u) {
-      pad_id_ = from.pad_id_;
+      vocabulary_output_piece_score_ = from.vocabulary_output_piece_score_;
+    }
+    if (cached_has_bits & 0x00000020u) {
+      hard_vocab_limit_ = from.hard_vocab_limit_;
+    }
+    if (cached_has_bits & 0x00000040u) {
+      bos_id_ = from.bos_id_;
+    }
+    if (cached_has_bits & 0x00000080u) {
+      eos_id_ = from.eos_id_;
     }
     _has_bits_[1] |= cached_has_bits;
   }
+  if (cached_has_bits & 0x00000100u) {
+    _internal_set_pad_id(from._internal_pad_id());
+  }
 }
 
 void TrainerSpec::CopyFrom(const TrainerSpec& from) {
 // @@protoc_insertion_point(class_specific_copy_from_start:sentencepiece.TrainerSpec)
   if (&from == this) return;
   Clear();
   MergeFrom(from);
@@ -1729,17 +1847,18 @@
   input_format_.Swap(&other->input_format_, &::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited(), GetArena());
   required_chars_.Swap(&other->required_chars_, &::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited(), GetArena());
   unk_surface_.Swap(&other->unk_surface_, nullptr, GetArena());
   unk_piece_.Swap(&other->unk_piece_, nullptr, GetArena());
   bos_piece_.Swap(&other->bos_piece_, nullptr, GetArena());
   eos_piece_.Swap(&other->eos_piece_, nullptr, GetArena());
   pad_piece_.Swap(&other->pad_piece_, nullptr, GetArena());
+  pretokenization_delimiter_.Swap(&other->pretokenization_delimiter_, &::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited(), GetArena());
   ::PROTOBUF_NAMESPACE_ID::internal::memswap<
-      PROTOBUF_FIELD_OFFSET(TrainerSpec, train_extremely_large_corpus_)
-      + sizeof(TrainerSpec::train_extremely_large_corpus_)
+      PROTOBUF_FIELD_OFFSET(TrainerSpec, differential_privacy_clipping_threshold_)
+      + sizeof(TrainerSpec::differential_privacy_clipping_threshold_)
       - PROTOBUF_FIELD_OFFSET(TrainerSpec, self_test_sample_size_)>(
           reinterpret_cast<char*>(&self_test_sample_size_),
           reinterpret_cast<char*>(&other->self_test_sample_size_));
   swap(model_type_, other->model_type_);
   swap(vocab_size_, other->vocab_size_);
   swap(character_coverage_, other->character_coverage_);
   swap(seed_sentencepiece_size_, other->seed_sentencepiece_size_);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/builtin_pb/sentencepiece_model.pb.h`

 * *Files 3% similar despite different names*

```diff
@@ -269,25 +269,29 @@
     kInputFormatFieldNumber = 7,
     kRequiredCharsFieldNumber = 36,
     kUnkSurfaceFieldNumber = 44,
     kUnkPieceFieldNumber = 45,
     kBosPieceFieldNumber = 46,
     kEosPieceFieldNumber = 47,
     kPadPieceFieldNumber = 48,
+    kPretokenizationDelimiterFieldNumber = 53,
     kSelfTestSampleSizeFieldNumber = 6,
     kMiningSentenceSizeFieldNumber = 12,
     kInputSentenceSizeFieldNumber = 11,
     kTrainingSentenceSizeFieldNumber = 13,
+    kEnableDifferentialPrivacyFieldNumber = 50,
     kTreatWhitespaceAsSuffixFieldNumber = 24,
     kAllowWhitespaceOnlyPiecesFieldNumber = 26,
     kSplitDigitsFieldNumber = 25,
     kByteFallbackFieldNumber = 35,
-    kUnkIdFieldNumber = 40,
     kUseAllVocabFieldNumber = 34,
     kTrainExtremelyLargeCorpusFieldNumber = 49,
+    kUnkIdFieldNumber = 40,
+    kDifferentialPrivacyNoiseLevelFieldNumber = 51,
+    kDifferentialPrivacyClippingThresholdFieldNumber = 52,
     kModelTypeFieldNumber = 3,
     kVocabSizeFieldNumber = 4,
     kCharacterCoverageFieldNumber = 10,
     kSeedSentencepieceSizeFieldNumber = 14,
     kShrinkingFactorFieldNumber = 15,
     kNumThreadsFieldNumber = 16,
     kNumSubIterationsFieldNumber = 17,
@@ -555,14 +559,34 @@
   void set_allocated_pad_piece(std::string* pad_piece);
   private:
   const std::string& _internal_pad_piece() const;
   void _internal_set_pad_piece(const std::string& value);
   std::string* _internal_mutable_pad_piece();
   public:
 
+  // optional string pretokenization_delimiter = 53 [default = ""];
+  bool has_pretokenization_delimiter() const;
+  private:
+  bool _internal_has_pretokenization_delimiter() const;
+  public:
+  void clear_pretokenization_delimiter();
+  const std::string& pretokenization_delimiter() const;
+  void set_pretokenization_delimiter(const std::string& value);
+  void set_pretokenization_delimiter(std::string&& value);
+  void set_pretokenization_delimiter(const char* value);
+  void set_pretokenization_delimiter(const char* value, size_t size);
+  std::string* mutable_pretokenization_delimiter();
+  std::string* release_pretokenization_delimiter();
+  void set_allocated_pretokenization_delimiter(std::string* pretokenization_delimiter);
+  private:
+  const std::string& _internal_pretokenization_delimiter() const;
+  void _internal_set_pretokenization_delimiter(const std::string& value);
+  std::string* _internal_mutable_pretokenization_delimiter();
+  public:
+
   // optional int32 self_test_sample_size = 6 [default = 0];
   bool has_self_test_sample_size() const;
   private:
   bool _internal_has_self_test_sample_size() const;
   public:
   void clear_self_test_sample_size();
   ::PROTOBUF_NAMESPACE_ID::int32 self_test_sample_size() const;
@@ -607,14 +631,27 @@
   PROTOBUF_DEPRECATED ::PROTOBUF_NAMESPACE_ID::int32 training_sentence_size() const;
   PROTOBUF_DEPRECATED void set_training_sentence_size(::PROTOBUF_NAMESPACE_ID::int32 value);
   private:
   ::PROTOBUF_NAMESPACE_ID::int32 _internal_training_sentence_size() const;
   void _internal_set_training_sentence_size(::PROTOBUF_NAMESPACE_ID::int32 value);
   public:
 
+  // optional bool enable_differential_privacy = 50 [default = false];
+  bool has_enable_differential_privacy() const;
+  private:
+  bool _internal_has_enable_differential_privacy() const;
+  public:
+  void clear_enable_differential_privacy();
+  bool enable_differential_privacy() const;
+  void set_enable_differential_privacy(bool value);
+  private:
+  bool _internal_enable_differential_privacy() const;
+  void _internal_set_enable_differential_privacy(bool value);
+  public:
+
   // optional bool treat_whitespace_as_suffix = 24 [default = false];
   bool has_treat_whitespace_as_suffix() const;
   private:
   bool _internal_has_treat_whitespace_as_suffix() const;
   public:
   void clear_treat_whitespace_as_suffix();
   bool treat_whitespace_as_suffix() const;
@@ -659,27 +696,14 @@
   bool byte_fallback() const;
   void set_byte_fallback(bool value);
   private:
   bool _internal_byte_fallback() const;
   void _internal_set_byte_fallback(bool value);
   public:
 
-  // optional int32 unk_id = 40 [default = 0];
-  bool has_unk_id() const;
-  private:
-  bool _internal_has_unk_id() const;
-  public:
-  void clear_unk_id();
-  ::PROTOBUF_NAMESPACE_ID::int32 unk_id() const;
-  void set_unk_id(::PROTOBUF_NAMESPACE_ID::int32 value);
-  private:
-  ::PROTOBUF_NAMESPACE_ID::int32 _internal_unk_id() const;
-  void _internal_set_unk_id(::PROTOBUF_NAMESPACE_ID::int32 value);
-  public:
-
   // optional bool use_all_vocab = 34 [default = false];
   bool has_use_all_vocab() const;
   private:
   bool _internal_has_use_all_vocab() const;
   public:
   void clear_use_all_vocab();
   bool use_all_vocab() const;
@@ -698,14 +722,53 @@
   bool train_extremely_large_corpus() const;
   void set_train_extremely_large_corpus(bool value);
   private:
   bool _internal_train_extremely_large_corpus() const;
   void _internal_set_train_extremely_large_corpus(bool value);
   public:
 
+  // optional int32 unk_id = 40 [default = 0];
+  bool has_unk_id() const;
+  private:
+  bool _internal_has_unk_id() const;
+  public:
+  void clear_unk_id();
+  ::PROTOBUF_NAMESPACE_ID::int32 unk_id() const;
+  void set_unk_id(::PROTOBUF_NAMESPACE_ID::int32 value);
+  private:
+  ::PROTOBUF_NAMESPACE_ID::int32 _internal_unk_id() const;
+  void _internal_set_unk_id(::PROTOBUF_NAMESPACE_ID::int32 value);
+  public:
+
+  // optional float differential_privacy_noise_level = 51 [default = 0];
+  bool has_differential_privacy_noise_level() const;
+  private:
+  bool _internal_has_differential_privacy_noise_level() const;
+  public:
+  void clear_differential_privacy_noise_level();
+  float differential_privacy_noise_level() const;
+  void set_differential_privacy_noise_level(float value);
+  private:
+  float _internal_differential_privacy_noise_level() const;
+  void _internal_set_differential_privacy_noise_level(float value);
+  public:
+
+  // optional uint64 differential_privacy_clipping_threshold = 52 [default = 0];
+  bool has_differential_privacy_clipping_threshold() const;
+  private:
+  bool _internal_has_differential_privacy_clipping_threshold() const;
+  public:
+  void clear_differential_privacy_clipping_threshold();
+  ::PROTOBUF_NAMESPACE_ID::uint64 differential_privacy_clipping_threshold() const;
+  void set_differential_privacy_clipping_threshold(::PROTOBUF_NAMESPACE_ID::uint64 value);
+  private:
+  ::PROTOBUF_NAMESPACE_ID::uint64 _internal_differential_privacy_clipping_threshold() const;
+  void _internal_set_differential_privacy_clipping_threshold(::PROTOBUF_NAMESPACE_ID::uint64 value);
+  public:
+
   // optional .sentencepiece.TrainerSpec.ModelType model_type = 3 [default = UNIGRAM];
   bool has_model_type() const;
   private:
   bool _internal_has_model_type() const;
   public:
   void clear_model_type();
   ::sentencepiece::TrainerSpec_ModelType model_type() const;
@@ -961,25 +1024,29 @@
   ::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr unk_piece_;
   static const ::PROTOBUF_NAMESPACE_ID::internal::LazyString _i_give_permission_to_break_this_code_default_bos_piece_;
   ::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr bos_piece_;
   static const ::PROTOBUF_NAMESPACE_ID::internal::LazyString _i_give_permission_to_break_this_code_default_eos_piece_;
   ::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr eos_piece_;
   static const ::PROTOBUF_NAMESPACE_ID::internal::LazyString _i_give_permission_to_break_this_code_default_pad_piece_;
   ::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr pad_piece_;
+  ::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr pretokenization_delimiter_;
   ::PROTOBUF_NAMESPACE_ID::int32 self_test_sample_size_;
   ::PROTOBUF_NAMESPACE_ID::int32 mining_sentence_size_;
   ::PROTOBUF_NAMESPACE_ID::uint64 input_sentence_size_;
   ::PROTOBUF_NAMESPACE_ID::int32 training_sentence_size_;
+  bool enable_differential_privacy_;
   bool treat_whitespace_as_suffix_;
   bool allow_whitespace_only_pieces_;
   bool split_digits_;
   bool byte_fallback_;
-  ::PROTOBUF_NAMESPACE_ID::int32 unk_id_;
   bool use_all_vocab_;
   bool train_extremely_large_corpus_;
+  ::PROTOBUF_NAMESPACE_ID::int32 unk_id_;
+  float differential_privacy_noise_level_;
+  ::PROTOBUF_NAMESPACE_ID::uint64 differential_privacy_clipping_threshold_;
   int model_type_;
   ::PROTOBUF_NAMESPACE_ID::int32 vocab_size_;
   float character_coverage_;
   ::PROTOBUF_NAMESPACE_ID::int32 seed_sentencepiece_size_;
   float shrinking_factor_;
   ::PROTOBUF_NAMESPACE_ID::int32 num_threads_;
   ::PROTOBUF_NAMESPACE_ID::int32 num_sub_iterations_;
@@ -2191,62 +2258,62 @@
   model_prefix_.SetAllocated(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited(), model_prefix,
       GetArena());
   // @@protoc_insertion_point(field_set_allocated:sentencepiece.TrainerSpec.model_prefix)
 }
 
 // optional .sentencepiece.TrainerSpec.ModelType model_type = 3 [default = UNIGRAM];
 inline bool TrainerSpec::_internal_has_model_type() const {
-  bool value = (_has_bits_[0] & 0x00080000u) != 0;
+  bool value = (_has_bits_[0] & 0x00800000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_model_type() const {
   return _internal_has_model_type();
 }
 inline void TrainerSpec::clear_model_type() {
   model_type_ = 1;
-  _has_bits_[0] &= ~0x00080000u;
+  _has_bits_[0] &= ~0x00800000u;
 }
 inline ::sentencepiece::TrainerSpec_ModelType TrainerSpec::_internal_model_type() const {
   return static_cast< ::sentencepiece::TrainerSpec_ModelType >(model_type_);
 }
 inline ::sentencepiece::TrainerSpec_ModelType TrainerSpec::model_type() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.model_type)
   return _internal_model_type();
 }
 inline void TrainerSpec::_internal_set_model_type(::sentencepiece::TrainerSpec_ModelType value) {
   assert(::sentencepiece::TrainerSpec_ModelType_IsValid(value));
-  _has_bits_[0] |= 0x00080000u;
+  _has_bits_[0] |= 0x00800000u;
   model_type_ = value;
 }
 inline void TrainerSpec::set_model_type(::sentencepiece::TrainerSpec_ModelType value) {
   _internal_set_model_type(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.model_type)
 }
 
 // optional int32 vocab_size = 4 [default = 8000];
 inline bool TrainerSpec::_internal_has_vocab_size() const {
-  bool value = (_has_bits_[0] & 0x00100000u) != 0;
+  bool value = (_has_bits_[0] & 0x01000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_vocab_size() const {
   return _internal_has_vocab_size();
 }
 inline void TrainerSpec::clear_vocab_size() {
   vocab_size_ = 8000;
-  _has_bits_[0] &= ~0x00100000u;
+  _has_bits_[0] &= ~0x01000000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_vocab_size() const {
   return vocab_size_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::vocab_size() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.vocab_size)
   return _internal_vocab_size();
 }
 inline void TrainerSpec::_internal_set_vocab_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x00100000u;
+  _has_bits_[0] |= 0x01000000u;
   vocab_size_ = value;
 }
 inline void TrainerSpec::set_vocab_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_vocab_size(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.vocab_size)
 }
 
@@ -2322,516 +2389,673 @@
 TrainerSpec::mutable_accept_language() {
   // @@protoc_insertion_point(field_mutable_list:sentencepiece.TrainerSpec.accept_language)
   return &accept_language_;
 }
 
 // optional int32 self_test_sample_size = 6 [default = 0];
 inline bool TrainerSpec::_internal_has_self_test_sample_size() const {
-  bool value = (_has_bits_[0] & 0x00000100u) != 0;
+  bool value = (_has_bits_[0] & 0x00000200u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_self_test_sample_size() const {
   return _internal_has_self_test_sample_size();
 }
 inline void TrainerSpec::clear_self_test_sample_size() {
   self_test_sample_size_ = 0;
-  _has_bits_[0] &= ~0x00000100u;
+  _has_bits_[0] &= ~0x00000200u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_self_test_sample_size() const {
   return self_test_sample_size_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::self_test_sample_size() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.self_test_sample_size)
   return _internal_self_test_sample_size();
 }
 inline void TrainerSpec::_internal_set_self_test_sample_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x00000100u;
+  _has_bits_[0] |= 0x00000200u;
   self_test_sample_size_ = value;
 }
 inline void TrainerSpec::set_self_test_sample_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_self_test_sample_size(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.self_test_sample_size)
 }
 
+// optional bool enable_differential_privacy = 50 [default = false];
+inline bool TrainerSpec::_internal_has_enable_differential_privacy() const {
+  bool value = (_has_bits_[0] & 0x00002000u) != 0;
+  return value;
+}
+inline bool TrainerSpec::has_enable_differential_privacy() const {
+  return _internal_has_enable_differential_privacy();
+}
+inline void TrainerSpec::clear_enable_differential_privacy() {
+  enable_differential_privacy_ = false;
+  _has_bits_[0] &= ~0x00002000u;
+}
+inline bool TrainerSpec::_internal_enable_differential_privacy() const {
+  return enable_differential_privacy_;
+}
+inline bool TrainerSpec::enable_differential_privacy() const {
+  // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.enable_differential_privacy)
+  return _internal_enable_differential_privacy();
+}
+inline void TrainerSpec::_internal_set_enable_differential_privacy(bool value) {
+  _has_bits_[0] |= 0x00002000u;
+  enable_differential_privacy_ = value;
+}
+inline void TrainerSpec::set_enable_differential_privacy(bool value) {
+  _internal_set_enable_differential_privacy(value);
+  // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.enable_differential_privacy)
+}
+
+// optional float differential_privacy_noise_level = 51 [default = 0];
+inline bool TrainerSpec::_internal_has_differential_privacy_noise_level() const {
+  bool value = (_has_bits_[0] & 0x00200000u) != 0;
+  return value;
+}
+inline bool TrainerSpec::has_differential_privacy_noise_level() const {
+  return _internal_has_differential_privacy_noise_level();
+}
+inline void TrainerSpec::clear_differential_privacy_noise_level() {
+  differential_privacy_noise_level_ = 0;
+  _has_bits_[0] &= ~0x00200000u;
+}
+inline float TrainerSpec::_internal_differential_privacy_noise_level() const {
+  return differential_privacy_noise_level_;
+}
+inline float TrainerSpec::differential_privacy_noise_level() const {
+  // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.differential_privacy_noise_level)
+  return _internal_differential_privacy_noise_level();
+}
+inline void TrainerSpec::_internal_set_differential_privacy_noise_level(float value) {
+  _has_bits_[0] |= 0x00200000u;
+  differential_privacy_noise_level_ = value;
+}
+inline void TrainerSpec::set_differential_privacy_noise_level(float value) {
+  _internal_set_differential_privacy_noise_level(value);
+  // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.differential_privacy_noise_level)
+}
+
+// optional uint64 differential_privacy_clipping_threshold = 52 [default = 0];
+inline bool TrainerSpec::_internal_has_differential_privacy_clipping_threshold() const {
+  bool value = (_has_bits_[0] & 0x00400000u) != 0;
+  return value;
+}
+inline bool TrainerSpec::has_differential_privacy_clipping_threshold() const {
+  return _internal_has_differential_privacy_clipping_threshold();
+}
+inline void TrainerSpec::clear_differential_privacy_clipping_threshold() {
+  differential_privacy_clipping_threshold_ = PROTOBUF_ULONGLONG(0);
+  _has_bits_[0] &= ~0x00400000u;
+}
+inline ::PROTOBUF_NAMESPACE_ID::uint64 TrainerSpec::_internal_differential_privacy_clipping_threshold() const {
+  return differential_privacy_clipping_threshold_;
+}
+inline ::PROTOBUF_NAMESPACE_ID::uint64 TrainerSpec::differential_privacy_clipping_threshold() const {
+  // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.differential_privacy_clipping_threshold)
+  return _internal_differential_privacy_clipping_threshold();
+}
+inline void TrainerSpec::_internal_set_differential_privacy_clipping_threshold(::PROTOBUF_NAMESPACE_ID::uint64 value) {
+  _has_bits_[0] |= 0x00400000u;
+  differential_privacy_clipping_threshold_ = value;
+}
+inline void TrainerSpec::set_differential_privacy_clipping_threshold(::PROTOBUF_NAMESPACE_ID::uint64 value) {
+  _internal_set_differential_privacy_clipping_threshold(value);
+  // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.differential_privacy_clipping_threshold)
+}
+
 // optional float character_coverage = 10 [default = 0.9995];
 inline bool TrainerSpec::_internal_has_character_coverage() const {
-  bool value = (_has_bits_[0] & 0x00200000u) != 0;
+  bool value = (_has_bits_[0] & 0x02000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_character_coverage() const {
   return _internal_has_character_coverage();
 }
 inline void TrainerSpec::clear_character_coverage() {
   character_coverage_ = 0.9995f;
-  _has_bits_[0] &= ~0x00200000u;
+  _has_bits_[0] &= ~0x02000000u;
 }
 inline float TrainerSpec::_internal_character_coverage() const {
   return character_coverage_;
 }
 inline float TrainerSpec::character_coverage() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.character_coverage)
   return _internal_character_coverage();
 }
 inline void TrainerSpec::_internal_set_character_coverage(float value) {
-  _has_bits_[0] |= 0x00200000u;
+  _has_bits_[0] |= 0x02000000u;
   character_coverage_ = value;
 }
 inline void TrainerSpec::set_character_coverage(float value) {
   _internal_set_character_coverage(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.character_coverage)
 }
 
 // optional uint64 input_sentence_size = 11 [default = 0];
 inline bool TrainerSpec::_internal_has_input_sentence_size() const {
-  bool value = (_has_bits_[0] & 0x00000400u) != 0;
+  bool value = (_has_bits_[0] & 0x00000800u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_input_sentence_size() const {
   return _internal_has_input_sentence_size();
 }
 inline void TrainerSpec::clear_input_sentence_size() {
   input_sentence_size_ = PROTOBUF_ULONGLONG(0);
-  _has_bits_[0] &= ~0x00000400u;
+  _has_bits_[0] &= ~0x00000800u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::uint64 TrainerSpec::_internal_input_sentence_size() const {
   return input_sentence_size_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::uint64 TrainerSpec::input_sentence_size() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.input_sentence_size)
   return _internal_input_sentence_size();
 }
 inline void TrainerSpec::_internal_set_input_sentence_size(::PROTOBUF_NAMESPACE_ID::uint64 value) {
-  _has_bits_[0] |= 0x00000400u;
+  _has_bits_[0] |= 0x00000800u;
   input_sentence_size_ = value;
 }
 inline void TrainerSpec::set_input_sentence_size(::PROTOBUF_NAMESPACE_ID::uint64 value) {
   _internal_set_input_sentence_size(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.input_sentence_size)
 }
 
 // optional bool shuffle_input_sentence = 19 [default = true];
 inline bool TrainerSpec::_internal_has_shuffle_input_sentence() const {
-  bool value = (_has_bits_[0] & 0x10000000u) != 0;
+  bool value = (_has_bits_[1] & 0x00000001u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_shuffle_input_sentence() const {
   return _internal_has_shuffle_input_sentence();
 }
 inline void TrainerSpec::clear_shuffle_input_sentence() {
   shuffle_input_sentence_ = true;
-  _has_bits_[0] &= ~0x10000000u;
+  _has_bits_[1] &= ~0x00000001u;
 }
 inline bool TrainerSpec::_internal_shuffle_input_sentence() const {
   return shuffle_input_sentence_;
 }
 inline bool TrainerSpec::shuffle_input_sentence() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.shuffle_input_sentence)
   return _internal_shuffle_input_sentence();
 }
 inline void TrainerSpec::_internal_set_shuffle_input_sentence(bool value) {
-  _has_bits_[0] |= 0x10000000u;
+  _has_bits_[1] |= 0x00000001u;
   shuffle_input_sentence_ = value;
 }
 inline void TrainerSpec::set_shuffle_input_sentence(bool value) {
   _internal_set_shuffle_input_sentence(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.shuffle_input_sentence)
 }
 
 // optional int32 mining_sentence_size = 12 [deprecated = true];
 inline bool TrainerSpec::_internal_has_mining_sentence_size() const {
-  bool value = (_has_bits_[0] & 0x00000200u) != 0;
+  bool value = (_has_bits_[0] & 0x00000400u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_mining_sentence_size() const {
   return _internal_has_mining_sentence_size();
 }
 inline void TrainerSpec::clear_mining_sentence_size() {
   mining_sentence_size_ = 0;
-  _has_bits_[0] &= ~0x00000200u;
+  _has_bits_[0] &= ~0x00000400u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_mining_sentence_size() const {
   return mining_sentence_size_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::mining_sentence_size() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.mining_sentence_size)
   return _internal_mining_sentence_size();
 }
 inline void TrainerSpec::_internal_set_mining_sentence_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x00000200u;
+  _has_bits_[0] |= 0x00000400u;
   mining_sentence_size_ = value;
 }
 inline void TrainerSpec::set_mining_sentence_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_mining_sentence_size(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.mining_sentence_size)
 }
 
 // optional int32 training_sentence_size = 13 [deprecated = true];
 inline bool TrainerSpec::_internal_has_training_sentence_size() const {
-  bool value = (_has_bits_[0] & 0x00000800u) != 0;
+  bool value = (_has_bits_[0] & 0x00001000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_training_sentence_size() const {
   return _internal_has_training_sentence_size();
 }
 inline void TrainerSpec::clear_training_sentence_size() {
   training_sentence_size_ = 0;
-  _has_bits_[0] &= ~0x00000800u;
+  _has_bits_[0] &= ~0x00001000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_training_sentence_size() const {
   return training_sentence_size_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::training_sentence_size() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.training_sentence_size)
   return _internal_training_sentence_size();
 }
 inline void TrainerSpec::_internal_set_training_sentence_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x00000800u;
+  _has_bits_[0] |= 0x00001000u;
   training_sentence_size_ = value;
 }
 inline void TrainerSpec::set_training_sentence_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_training_sentence_size(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.training_sentence_size)
 }
 
 // optional int32 seed_sentencepiece_size = 14 [default = 1000000];
 inline bool TrainerSpec::_internal_has_seed_sentencepiece_size() const {
-  bool value = (_has_bits_[0] & 0x00400000u) != 0;
+  bool value = (_has_bits_[0] & 0x04000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_seed_sentencepiece_size() const {
   return _internal_has_seed_sentencepiece_size();
 }
 inline void TrainerSpec::clear_seed_sentencepiece_size() {
   seed_sentencepiece_size_ = 1000000;
-  _has_bits_[0] &= ~0x00400000u;
+  _has_bits_[0] &= ~0x04000000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_seed_sentencepiece_size() const {
   return seed_sentencepiece_size_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::seed_sentencepiece_size() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.seed_sentencepiece_size)
   return _internal_seed_sentencepiece_size();
 }
 inline void TrainerSpec::_internal_set_seed_sentencepiece_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x00400000u;
+  _has_bits_[0] |= 0x04000000u;
   seed_sentencepiece_size_ = value;
 }
 inline void TrainerSpec::set_seed_sentencepiece_size(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_seed_sentencepiece_size(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.seed_sentencepiece_size)
 }
 
 // optional float shrinking_factor = 15 [default = 0.75];
 inline bool TrainerSpec::_internal_has_shrinking_factor() const {
-  bool value = (_has_bits_[0] & 0x00800000u) != 0;
+  bool value = (_has_bits_[0] & 0x08000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_shrinking_factor() const {
   return _internal_has_shrinking_factor();
 }
 inline void TrainerSpec::clear_shrinking_factor() {
   shrinking_factor_ = 0.75f;
-  _has_bits_[0] &= ~0x00800000u;
+  _has_bits_[0] &= ~0x08000000u;
 }
 inline float TrainerSpec::_internal_shrinking_factor() const {
   return shrinking_factor_;
 }
 inline float TrainerSpec::shrinking_factor() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.shrinking_factor)
   return _internal_shrinking_factor();
 }
 inline void TrainerSpec::_internal_set_shrinking_factor(float value) {
-  _has_bits_[0] |= 0x00800000u;
+  _has_bits_[0] |= 0x08000000u;
   shrinking_factor_ = value;
 }
 inline void TrainerSpec::set_shrinking_factor(float value) {
   _internal_set_shrinking_factor(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.shrinking_factor)
 }
 
 // optional int32 max_sentence_length = 18 [default = 4192];
 inline bool TrainerSpec::_internal_has_max_sentence_length() const {
-  bool value = (_has_bits_[0] & 0x04000000u) != 0;
+  bool value = (_has_bits_[0] & 0x40000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_max_sentence_length() const {
   return _internal_has_max_sentence_length();
 }
 inline void TrainerSpec::clear_max_sentence_length() {
   max_sentence_length_ = 4192;
-  _has_bits_[0] &= ~0x04000000u;
+  _has_bits_[0] &= ~0x40000000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_max_sentence_length() const {
   return max_sentence_length_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::max_sentence_length() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.max_sentence_length)
   return _internal_max_sentence_length();
 }
 inline void TrainerSpec::_internal_set_max_sentence_length(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x04000000u;
+  _has_bits_[0] |= 0x40000000u;
   max_sentence_length_ = value;
 }
 inline void TrainerSpec::set_max_sentence_length(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_max_sentence_length(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.max_sentence_length)
 }
 
 // optional int32 num_threads = 16 [default = 16];
 inline bool TrainerSpec::_internal_has_num_threads() const {
-  bool value = (_has_bits_[0] & 0x01000000u) != 0;
+  bool value = (_has_bits_[0] & 0x10000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_num_threads() const {
   return _internal_has_num_threads();
 }
 inline void TrainerSpec::clear_num_threads() {
   num_threads_ = 16;
-  _has_bits_[0] &= ~0x01000000u;
+  _has_bits_[0] &= ~0x10000000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_num_threads() const {
   return num_threads_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::num_threads() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.num_threads)
   return _internal_num_threads();
 }
 inline void TrainerSpec::_internal_set_num_threads(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x01000000u;
+  _has_bits_[0] |= 0x10000000u;
   num_threads_ = value;
 }
 inline void TrainerSpec::set_num_threads(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_num_threads(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.num_threads)
 }
 
 // optional int32 num_sub_iterations = 17 [default = 2];
 inline bool TrainerSpec::_internal_has_num_sub_iterations() const {
-  bool value = (_has_bits_[0] & 0x02000000u) != 0;
+  bool value = (_has_bits_[0] & 0x20000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_num_sub_iterations() const {
   return _internal_has_num_sub_iterations();
 }
 inline void TrainerSpec::clear_num_sub_iterations() {
   num_sub_iterations_ = 2;
-  _has_bits_[0] &= ~0x02000000u;
+  _has_bits_[0] &= ~0x20000000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_num_sub_iterations() const {
   return num_sub_iterations_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::num_sub_iterations() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.num_sub_iterations)
   return _internal_num_sub_iterations();
 }
 inline void TrainerSpec::_internal_set_num_sub_iterations(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x02000000u;
+  _has_bits_[0] |= 0x20000000u;
   num_sub_iterations_ = value;
 }
 inline void TrainerSpec::set_num_sub_iterations(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_num_sub_iterations(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.num_sub_iterations)
 }
 
 // optional int32 max_sentencepiece_length = 20 [default = 16];
 inline bool TrainerSpec::_internal_has_max_sentencepiece_length() const {
-  bool value = (_has_bits_[0] & 0x08000000u) != 0;
+  bool value = (_has_bits_[0] & 0x80000000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_max_sentencepiece_length() const {
   return _internal_has_max_sentencepiece_length();
 }
 inline void TrainerSpec::clear_max_sentencepiece_length() {
   max_sentencepiece_length_ = 16;
-  _has_bits_[0] &= ~0x08000000u;
+  _has_bits_[0] &= ~0x80000000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_max_sentencepiece_length() const {
   return max_sentencepiece_length_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::max_sentencepiece_length() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.max_sentencepiece_length)
   return _internal_max_sentencepiece_length();
 }
 inline void TrainerSpec::_internal_set_max_sentencepiece_length(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x08000000u;
+  _has_bits_[0] |= 0x80000000u;
   max_sentencepiece_length_ = value;
 }
 inline void TrainerSpec::set_max_sentencepiece_length(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_max_sentencepiece_length(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.max_sentencepiece_length)
 }
 
 // optional bool split_by_unicode_script = 21 [default = true];
 inline bool TrainerSpec::_internal_has_split_by_unicode_script() const {
-  bool value = (_has_bits_[0] & 0x20000000u) != 0;
+  bool value = (_has_bits_[1] & 0x00000002u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_split_by_unicode_script() const {
   return _internal_has_split_by_unicode_script();
 }
 inline void TrainerSpec::clear_split_by_unicode_script() {
   split_by_unicode_script_ = true;
-  _has_bits_[0] &= ~0x20000000u;
+  _has_bits_[1] &= ~0x00000002u;
 }
 inline bool TrainerSpec::_internal_split_by_unicode_script() const {
   return split_by_unicode_script_;
 }
 inline bool TrainerSpec::split_by_unicode_script() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.split_by_unicode_script)
   return _internal_split_by_unicode_script();
 }
 inline void TrainerSpec::_internal_set_split_by_unicode_script(bool value) {
-  _has_bits_[0] |= 0x20000000u;
+  _has_bits_[1] |= 0x00000002u;
   split_by_unicode_script_ = value;
 }
 inline void TrainerSpec::set_split_by_unicode_script(bool value) {
   _internal_set_split_by_unicode_script(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.split_by_unicode_script)
 }
 
 // optional bool split_by_number = 23 [default = true];
 inline bool TrainerSpec::_internal_has_split_by_number() const {
-  bool value = (_has_bits_[0] & 0x40000000u) != 0;
+  bool value = (_has_bits_[1] & 0x00000004u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_split_by_number() const {
   return _internal_has_split_by_number();
 }
 inline void TrainerSpec::clear_split_by_number() {
   split_by_number_ = true;
-  _has_bits_[0] &= ~0x40000000u;
+  _has_bits_[1] &= ~0x00000004u;
 }
 inline bool TrainerSpec::_internal_split_by_number() const {
   return split_by_number_;
 }
 inline bool TrainerSpec::split_by_number() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.split_by_number)
   return _internal_split_by_number();
 }
 inline void TrainerSpec::_internal_set_split_by_number(bool value) {
-  _has_bits_[0] |= 0x40000000u;
+  _has_bits_[1] |= 0x00000004u;
   split_by_number_ = value;
 }
 inline void TrainerSpec::set_split_by_number(bool value) {
   _internal_set_split_by_number(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.split_by_number)
 }
 
 // optional bool split_by_whitespace = 22 [default = true];
 inline bool TrainerSpec::_internal_has_split_by_whitespace() const {
-  bool value = (_has_bits_[0] & 0x80000000u) != 0;
+  bool value = (_has_bits_[1] & 0x00000008u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_split_by_whitespace() const {
   return _internal_has_split_by_whitespace();
 }
 inline void TrainerSpec::clear_split_by_whitespace() {
   split_by_whitespace_ = true;
-  _has_bits_[0] &= ~0x80000000u;
+  _has_bits_[1] &= ~0x00000008u;
 }
 inline bool TrainerSpec::_internal_split_by_whitespace() const {
   return split_by_whitespace_;
 }
 inline bool TrainerSpec::split_by_whitespace() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.split_by_whitespace)
   return _internal_split_by_whitespace();
 }
 inline void TrainerSpec::_internal_set_split_by_whitespace(bool value) {
-  _has_bits_[0] |= 0x80000000u;
+  _has_bits_[1] |= 0x00000008u;
   split_by_whitespace_ = value;
 }
 inline void TrainerSpec::set_split_by_whitespace(bool value) {
   _internal_set_split_by_whitespace(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.split_by_whitespace)
 }
 
 // optional bool treat_whitespace_as_suffix = 24 [default = false];
 inline bool TrainerSpec::_internal_has_treat_whitespace_as_suffix() const {
-  bool value = (_has_bits_[0] & 0x00001000u) != 0;
+  bool value = (_has_bits_[0] & 0x00004000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_treat_whitespace_as_suffix() const {
   return _internal_has_treat_whitespace_as_suffix();
 }
 inline void TrainerSpec::clear_treat_whitespace_as_suffix() {
   treat_whitespace_as_suffix_ = false;
-  _has_bits_[0] &= ~0x00001000u;
+  _has_bits_[0] &= ~0x00004000u;
 }
 inline bool TrainerSpec::_internal_treat_whitespace_as_suffix() const {
   return treat_whitespace_as_suffix_;
 }
 inline bool TrainerSpec::treat_whitespace_as_suffix() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.treat_whitespace_as_suffix)
   return _internal_treat_whitespace_as_suffix();
 }
 inline void TrainerSpec::_internal_set_treat_whitespace_as_suffix(bool value) {
-  _has_bits_[0] |= 0x00001000u;
+  _has_bits_[0] |= 0x00004000u;
   treat_whitespace_as_suffix_ = value;
 }
 inline void TrainerSpec::set_treat_whitespace_as_suffix(bool value) {
   _internal_set_treat_whitespace_as_suffix(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.treat_whitespace_as_suffix)
 }
 
 // optional bool allow_whitespace_only_pieces = 26 [default = false];
 inline bool TrainerSpec::_internal_has_allow_whitespace_only_pieces() const {
-  bool value = (_has_bits_[0] & 0x00002000u) != 0;
+  bool value = (_has_bits_[0] & 0x00008000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_allow_whitespace_only_pieces() const {
   return _internal_has_allow_whitespace_only_pieces();
 }
 inline void TrainerSpec::clear_allow_whitespace_only_pieces() {
   allow_whitespace_only_pieces_ = false;
-  _has_bits_[0] &= ~0x00002000u;
+  _has_bits_[0] &= ~0x00008000u;
 }
 inline bool TrainerSpec::_internal_allow_whitespace_only_pieces() const {
   return allow_whitespace_only_pieces_;
 }
 inline bool TrainerSpec::allow_whitespace_only_pieces() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.allow_whitespace_only_pieces)
   return _internal_allow_whitespace_only_pieces();
 }
 inline void TrainerSpec::_internal_set_allow_whitespace_only_pieces(bool value) {
-  _has_bits_[0] |= 0x00002000u;
+  _has_bits_[0] |= 0x00008000u;
   allow_whitespace_only_pieces_ = value;
 }
 inline void TrainerSpec::set_allow_whitespace_only_pieces(bool value) {
   _internal_set_allow_whitespace_only_pieces(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.allow_whitespace_only_pieces)
 }
 
 // optional bool split_digits = 25 [default = false];
 inline bool TrainerSpec::_internal_has_split_digits() const {
-  bool value = (_has_bits_[0] & 0x00004000u) != 0;
+  bool value = (_has_bits_[0] & 0x00010000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_split_digits() const {
   return _internal_has_split_digits();
 }
 inline void TrainerSpec::clear_split_digits() {
   split_digits_ = false;
-  _has_bits_[0] &= ~0x00004000u;
+  _has_bits_[0] &= ~0x00010000u;
 }
 inline bool TrainerSpec::_internal_split_digits() const {
   return split_digits_;
 }
 inline bool TrainerSpec::split_digits() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.split_digits)
   return _internal_split_digits();
 }
 inline void TrainerSpec::_internal_set_split_digits(bool value) {
-  _has_bits_[0] |= 0x00004000u;
+  _has_bits_[0] |= 0x00010000u;
   split_digits_ = value;
 }
 inline void TrainerSpec::set_split_digits(bool value) {
   _internal_set_split_digits(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.split_digits)
 }
 
+// optional string pretokenization_delimiter = 53 [default = ""];
+inline bool TrainerSpec::_internal_has_pretokenization_delimiter() const {
+  bool value = (_has_bits_[0] & 0x00000100u) != 0;
+  return value;
+}
+inline bool TrainerSpec::has_pretokenization_delimiter() const {
+  return _internal_has_pretokenization_delimiter();
+}
+inline void TrainerSpec::clear_pretokenization_delimiter() {
+  pretokenization_delimiter_.ClearToEmpty();
+  _has_bits_[0] &= ~0x00000100u;
+}
+inline const std::string& TrainerSpec::pretokenization_delimiter() const {
+  // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.pretokenization_delimiter)
+  return _internal_pretokenization_delimiter();
+}
+inline void TrainerSpec::set_pretokenization_delimiter(const std::string& value) {
+  _internal_set_pretokenization_delimiter(value);
+  // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.pretokenization_delimiter)
+}
+inline std::string* TrainerSpec::mutable_pretokenization_delimiter() {
+  // @@protoc_insertion_point(field_mutable:sentencepiece.TrainerSpec.pretokenization_delimiter)
+  return _internal_mutable_pretokenization_delimiter();
+}
+inline const std::string& TrainerSpec::_internal_pretokenization_delimiter() const {
+  return pretokenization_delimiter_.Get();
+}
+inline void TrainerSpec::_internal_set_pretokenization_delimiter(const std::string& value) {
+  _has_bits_[0] |= 0x00000100u;
+  pretokenization_delimiter_.Set(::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr::EmptyDefault{}, value, GetArena());
+}
+inline void TrainerSpec::set_pretokenization_delimiter(std::string&& value) {
+  _has_bits_[0] |= 0x00000100u;
+  pretokenization_delimiter_.Set(
+    ::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr::EmptyDefault{}, ::std::move(value), GetArena());
+  // @@protoc_insertion_point(field_set_rvalue:sentencepiece.TrainerSpec.pretokenization_delimiter)
+}
+inline void TrainerSpec::set_pretokenization_delimiter(const char* value) {
+  GOOGLE_DCHECK(value != nullptr);
+  _has_bits_[0] |= 0x00000100u;
+  pretokenization_delimiter_.Set(::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr::EmptyDefault{}, ::std::string(value), GetArena());
+  // @@protoc_insertion_point(field_set_char:sentencepiece.TrainerSpec.pretokenization_delimiter)
+}
+inline void TrainerSpec::set_pretokenization_delimiter(const char* value,
+    size_t size) {
+  _has_bits_[0] |= 0x00000100u;
+  pretokenization_delimiter_.Set(::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr::EmptyDefault{}, ::std::string(
+      reinterpret_cast<const char*>(value), size), GetArena());
+  // @@protoc_insertion_point(field_set_pointer:sentencepiece.TrainerSpec.pretokenization_delimiter)
+}
+inline std::string* TrainerSpec::_internal_mutable_pretokenization_delimiter() {
+  _has_bits_[0] |= 0x00000100u;
+  return pretokenization_delimiter_.Mutable(::PROTOBUF_NAMESPACE_ID::internal::ArenaStringPtr::EmptyDefault{}, GetArena());
+}
+inline std::string* TrainerSpec::release_pretokenization_delimiter() {
+  // @@protoc_insertion_point(field_release:sentencepiece.TrainerSpec.pretokenization_delimiter)
+  if (!_internal_has_pretokenization_delimiter()) {
+    return nullptr;
+  }
+  _has_bits_[0] &= ~0x00000100u;
+  return pretokenization_delimiter_.ReleaseNonDefault(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited(), GetArena());
+}
+inline void TrainerSpec::set_allocated_pretokenization_delimiter(std::string* pretokenization_delimiter) {
+  if (pretokenization_delimiter != nullptr) {
+    _has_bits_[0] |= 0x00000100u;
+  } else {
+    _has_bits_[0] &= ~0x00000100u;
+  }
+  pretokenization_delimiter_.SetAllocated(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited(), pretokenization_delimiter,
+      GetArena());
+  // @@protoc_insertion_point(field_set_allocated:sentencepiece.TrainerSpec.pretokenization_delimiter)
+}
+
 // repeated string control_symbols = 30;
 inline int TrainerSpec::_internal_control_symbols_size() const {
   return control_symbols_.size();
 }
 inline int TrainerSpec::control_symbols_size() const {
   return _internal_control_symbols_size();
 }
@@ -3047,229 +3271,229 @@
   required_chars_.SetAllocated(&::PROTOBUF_NAMESPACE_ID::internal::GetEmptyStringAlreadyInited(), required_chars,
       GetArena());
   // @@protoc_insertion_point(field_set_allocated:sentencepiece.TrainerSpec.required_chars)
 }
 
 // optional bool byte_fallback = 35 [default = false];
 inline bool TrainerSpec::_internal_has_byte_fallback() const {
-  bool value = (_has_bits_[0] & 0x00008000u) != 0;
+  bool value = (_has_bits_[0] & 0x00020000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_byte_fallback() const {
   return _internal_has_byte_fallback();
 }
 inline void TrainerSpec::clear_byte_fallback() {
   byte_fallback_ = false;
-  _has_bits_[0] &= ~0x00008000u;
+  _has_bits_[0] &= ~0x00020000u;
 }
 inline bool TrainerSpec::_internal_byte_fallback() const {
   return byte_fallback_;
 }
 inline bool TrainerSpec::byte_fallback() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.byte_fallback)
   return _internal_byte_fallback();
 }
 inline void TrainerSpec::_internal_set_byte_fallback(bool value) {
-  _has_bits_[0] |= 0x00008000u;
+  _has_bits_[0] |= 0x00020000u;
   byte_fallback_ = value;
 }
 inline void TrainerSpec::set_byte_fallback(bool value) {
   _internal_set_byte_fallback(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.byte_fallback)
 }
 
 // optional bool vocabulary_output_piece_score = 32 [default = true];
 inline bool TrainerSpec::_internal_has_vocabulary_output_piece_score() const {
-  bool value = (_has_bits_[1] & 0x00000001u) != 0;
+  bool value = (_has_bits_[1] & 0x00000010u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_vocabulary_output_piece_score() const {
   return _internal_has_vocabulary_output_piece_score();
 }
 inline void TrainerSpec::clear_vocabulary_output_piece_score() {
   vocabulary_output_piece_score_ = true;
-  _has_bits_[1] &= ~0x00000001u;
+  _has_bits_[1] &= ~0x00000010u;
 }
 inline bool TrainerSpec::_internal_vocabulary_output_piece_score() const {
   return vocabulary_output_piece_score_;
 }
 inline bool TrainerSpec::vocabulary_output_piece_score() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.vocabulary_output_piece_score)
   return _internal_vocabulary_output_piece_score();
 }
 inline void TrainerSpec::_internal_set_vocabulary_output_piece_score(bool value) {
-  _has_bits_[1] |= 0x00000001u;
+  _has_bits_[1] |= 0x00000010u;
   vocabulary_output_piece_score_ = value;
 }
 inline void TrainerSpec::set_vocabulary_output_piece_score(bool value) {
   _internal_set_vocabulary_output_piece_score(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.vocabulary_output_piece_score)
 }
 
 // optional bool hard_vocab_limit = 33 [default = true];
 inline bool TrainerSpec::_internal_has_hard_vocab_limit() const {
-  bool value = (_has_bits_[1] & 0x00000002u) != 0;
+  bool value = (_has_bits_[1] & 0x00000020u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_hard_vocab_limit() const {
   return _internal_has_hard_vocab_limit();
 }
 inline void TrainerSpec::clear_hard_vocab_limit() {
   hard_vocab_limit_ = true;
-  _has_bits_[1] &= ~0x00000002u;
+  _has_bits_[1] &= ~0x00000020u;
 }
 inline bool TrainerSpec::_internal_hard_vocab_limit() const {
   return hard_vocab_limit_;
 }
 inline bool TrainerSpec::hard_vocab_limit() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.hard_vocab_limit)
   return _internal_hard_vocab_limit();
 }
 inline void TrainerSpec::_internal_set_hard_vocab_limit(bool value) {
-  _has_bits_[1] |= 0x00000002u;
+  _has_bits_[1] |= 0x00000020u;
   hard_vocab_limit_ = value;
 }
 inline void TrainerSpec::set_hard_vocab_limit(bool value) {
   _internal_set_hard_vocab_limit(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.hard_vocab_limit)
 }
 
 // optional bool use_all_vocab = 34 [default = false];
 inline bool TrainerSpec::_internal_has_use_all_vocab() const {
-  bool value = (_has_bits_[0] & 0x00020000u) != 0;
+  bool value = (_has_bits_[0] & 0x00040000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_use_all_vocab() const {
   return _internal_has_use_all_vocab();
 }
 inline void TrainerSpec::clear_use_all_vocab() {
   use_all_vocab_ = false;
-  _has_bits_[0] &= ~0x00020000u;
+  _has_bits_[0] &= ~0x00040000u;
 }
 inline bool TrainerSpec::_internal_use_all_vocab() const {
   return use_all_vocab_;
 }
 inline bool TrainerSpec::use_all_vocab() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.use_all_vocab)
   return _internal_use_all_vocab();
 }
 inline void TrainerSpec::_internal_set_use_all_vocab(bool value) {
-  _has_bits_[0] |= 0x00020000u;
+  _has_bits_[0] |= 0x00040000u;
   use_all_vocab_ = value;
 }
 inline void TrainerSpec::set_use_all_vocab(bool value) {
   _internal_set_use_all_vocab(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.use_all_vocab)
 }
 
 // optional int32 unk_id = 40 [default = 0];
 inline bool TrainerSpec::_internal_has_unk_id() const {
-  bool value = (_has_bits_[0] & 0x00010000u) != 0;
+  bool value = (_has_bits_[0] & 0x00100000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_unk_id() const {
   return _internal_has_unk_id();
 }
 inline void TrainerSpec::clear_unk_id() {
   unk_id_ = 0;
-  _has_bits_[0] &= ~0x00010000u;
+  _has_bits_[0] &= ~0x00100000u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_unk_id() const {
   return unk_id_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::unk_id() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.unk_id)
   return _internal_unk_id();
 }
 inline void TrainerSpec::_internal_set_unk_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[0] |= 0x00010000u;
+  _has_bits_[0] |= 0x00100000u;
   unk_id_ = value;
 }
 inline void TrainerSpec::set_unk_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_unk_id(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.unk_id)
 }
 
 // optional int32 bos_id = 41 [default = 1];
 inline bool TrainerSpec::_internal_has_bos_id() const {
-  bool value = (_has_bits_[1] & 0x00000004u) != 0;
+  bool value = (_has_bits_[1] & 0x00000040u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_bos_id() const {
   return _internal_has_bos_id();
 }
 inline void TrainerSpec::clear_bos_id() {
   bos_id_ = 1;
-  _has_bits_[1] &= ~0x00000004u;
+  _has_bits_[1] &= ~0x00000040u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_bos_id() const {
   return bos_id_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::bos_id() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.bos_id)
   return _internal_bos_id();
 }
 inline void TrainerSpec::_internal_set_bos_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[1] |= 0x00000004u;
+  _has_bits_[1] |= 0x00000040u;
   bos_id_ = value;
 }
 inline void TrainerSpec::set_bos_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_bos_id(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.bos_id)
 }
 
 // optional int32 eos_id = 42 [default = 2];
 inline bool TrainerSpec::_internal_has_eos_id() const {
-  bool value = (_has_bits_[1] & 0x00000008u) != 0;
+  bool value = (_has_bits_[1] & 0x00000080u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_eos_id() const {
   return _internal_has_eos_id();
 }
 inline void TrainerSpec::clear_eos_id() {
   eos_id_ = 2;
-  _has_bits_[1] &= ~0x00000008u;
+  _has_bits_[1] &= ~0x00000080u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_eos_id() const {
   return eos_id_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::eos_id() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.eos_id)
   return _internal_eos_id();
 }
 inline void TrainerSpec::_internal_set_eos_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[1] |= 0x00000008u;
+  _has_bits_[1] |= 0x00000080u;
   eos_id_ = value;
 }
 inline void TrainerSpec::set_eos_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_eos_id(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.eos_id)
 }
 
 // optional int32 pad_id = 43 [default = -1];
 inline bool TrainerSpec::_internal_has_pad_id() const {
-  bool value = (_has_bits_[1] & 0x00000010u) != 0;
+  bool value = (_has_bits_[1] & 0x00000100u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_pad_id() const {
   return _internal_has_pad_id();
 }
 inline void TrainerSpec::clear_pad_id() {
   pad_id_ = -1;
-  _has_bits_[1] &= ~0x00000010u;
+  _has_bits_[1] &= ~0x00000100u;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::_internal_pad_id() const {
   return pad_id_;
 }
 inline ::PROTOBUF_NAMESPACE_ID::int32 TrainerSpec::pad_id() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.pad_id)
   return _internal_pad_id();
 }
 inline void TrainerSpec::_internal_set_pad_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
-  _has_bits_[1] |= 0x00000010u;
+  _has_bits_[1] |= 0x00000100u;
   pad_id_ = value;
 }
 inline void TrainerSpec::set_pad_id(::PROTOBUF_NAMESPACE_ID::int32 value) {
   _internal_set_pad_id(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.pad_id)
 }
 
@@ -3641,33 +3865,33 @@
   unk_surface_.SetAllocated(nullptr, unk_surface,
       GetArena());
   // @@protoc_insertion_point(field_set_allocated:sentencepiece.TrainerSpec.unk_surface)
 }
 
 // optional bool train_extremely_large_corpus = 49 [default = false];
 inline bool TrainerSpec::_internal_has_train_extremely_large_corpus() const {
-  bool value = (_has_bits_[0] & 0x00040000u) != 0;
+  bool value = (_has_bits_[0] & 0x00080000u) != 0;
   return value;
 }
 inline bool TrainerSpec::has_train_extremely_large_corpus() const {
   return _internal_has_train_extremely_large_corpus();
 }
 inline void TrainerSpec::clear_train_extremely_large_corpus() {
   train_extremely_large_corpus_ = false;
-  _has_bits_[0] &= ~0x00040000u;
+  _has_bits_[0] &= ~0x00080000u;
 }
 inline bool TrainerSpec::_internal_train_extremely_large_corpus() const {
   return train_extremely_large_corpus_;
 }
 inline bool TrainerSpec::train_extremely_large_corpus() const {
   // @@protoc_insertion_point(field_get:sentencepiece.TrainerSpec.train_extremely_large_corpus)
   return _internal_train_extremely_large_corpus();
 }
 inline void TrainerSpec::_internal_set_train_extremely_large_corpus(bool value) {
-  _has_bits_[0] |= 0x00040000u;
+  _has_bits_[0] |= 0x00080000u;
   train_extremely_large_corpus_ = value;
 }
 inline void TrainerSpec::set_train_extremely_large_corpus(bool value) {
   _internal_set_train_extremely_large_corpus(value);
   // @@protoc_insertion_point(field_set:sentencepiece.TrainerSpec.train_extremely_large_corpus)
 }
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/char_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/char_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/char_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/char_model_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/char_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/char_model_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/char_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/common.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/common.h`

 * *Files 25% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #include <iostream>
 #include <memory>
 #include <string>
 #include <utility>
 #include <vector>
 
 #include "config.h"
+#include "third_party/absl/strings/string_view.h"
 
 #if defined(_WIN32) && !defined(__CYGWIN__)
 #define OS_WIN
 #else
 #define OS_UNIX
 #endif
 
@@ -46,27 +47,14 @@
 typedef int64_t int64;
 typedef uint8_t uint8;
 typedef uint16_t uint16;
 typedef uint32_t char32;
 typedef uint32_t uint32;
 typedef uint64_t uint64;
 
-static constexpr uint8 kuint8max = ((uint8)0xFF);
-static constexpr uint16 kuint16max = ((uint16)0xFFFF);
-static constexpr uint32 kuint32max = ((uint32)0xFFFFFFFF);
-static constexpr uint64 kuint64max = ((uint64)(0xFFFFFFFFFFFFFFFF));
-static constexpr int8 kint8min = ((int8)~0x7F);
-static constexpr int8 kint8max = ((int8)0x7F);
-static constexpr int16 kint16min = ((int16)~0x7FFF);
-static constexpr int16 kint16max = ((int16)0x7FFF);
-static constexpr int32 kint32min = ((int32)~0x7FFFFFFF);
-static constexpr int32 kint32max = ((int32)0x7FFFFFFF);
-static constexpr int64 kint64min = ((int64)(~0x7FFFFFFFFFFFFFFF));
-static constexpr int64 kint64max = ((int64)(0x7FFFFFFFFFFFFFFF));
-
 static constexpr uint32 kUnicodeError = 0xFFFD;
 
 #if defined(OS_WIN) && defined(UNICODE) && defined(_UNICODE)
 #define WPATH(path) (::sentencepiece::win32::Utf8ToWide(path).c_str())
 #else
 #define WPATH(path) (path)
 #endif
@@ -77,19 +65,32 @@
 #ifndef _MSC_VER
 template <typename T, size_t N>
 char (&ArraySizeHelper(const T (&array)[N]))[N];
 #endif  // !_MSC_VER
 
 #define arraysize(array) (sizeof(ArraySizeHelper(array)))
 
+#if defined(_FREEBSD)
+#include <sys/endian.h>
+#endif
+#if !defined(__APPLE__) && !defined(_WIN32) && !defined(_FREEBSD)
+#include <endian.h>
+#if BYTE_ORDER == __BIG_ENDIAN
+#define IS_BIG_ENDIAN
+#endif
+#endif
+
+#ifdef IS_BIG_ENDIAN
+inline uint32 Swap32(uint32 x) { return __builtin_bswap32(x); }
+#endif
+
 namespace sentencepiece {
 #ifdef OS_WIN
 namespace win32 {
-std::wstring Utf8ToWide(const std::string &input);
-std::string WideToUtf8(const std::wstring &input);
+std::wstring Utf8ToWide(const absl::string_view input);
 }  // namespace win32
 #endif
 
 namespace error {
 
 void Abort();
 void Exit(int code);
@@ -107,23 +108,14 @@
     }
   }
   int operator&(std::ostream &) { return 0; }
 
  private:
   bool die_;
 };
-
-template <typename T>
-T &&CheckNotNull(const char *file, int line, const char *exprtext, T &&t) {
-  if (t == nullptr) {
-    std::cerr << file << "(" << line << ") " << exprtext;
-    Abort();
-  }
-  return std::forward<T>(t);
-}
 }  // namespace error
 
 namespace logging {
 enum LogSeverity {
   LOG_INFO = 0,
   LOG_WARNING = 1,
   LOG_ERROR = 2,
@@ -167,18 +159,14 @@
 #define CHECK_STREQ(a, b) CHECK_EQ(std::string(a), std::string(b))
 #define CHECK_EQ(a, b) CHECK((a) == (b))
 #define CHECK_NE(a, b) CHECK((a) != (b))
 #define CHECK_GE(a, b) CHECK((a) >= (b))
 #define CHECK_LE(a, b) CHECK((a) <= (b))
 #define CHECK_GT(a, b) CHECK((a) > (b))
 #define CHECK_LT(a, b) CHECK((a) < (b))
-#define CHECK_NOTNULL(val)                                    \
-  ::sentencepiece::error::CheckNotNull(                       \
-      ::sentencepiece::logging::BaseName(__FILE__), __LINE__, \
-      "'" #val "' Must be non NULL", (val))
 
 #define FRIEND_TEST(a, b) friend class a##_Test_##b;
 
 #define CHECK_OK(expr)                         \
   do {                                         \
     const auto _status = expr;                 \
     CHECK(_status.ok()) << _status.ToString(); \
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/compile_charsmap_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/compile_charsmap_main.cc`

 * *Files 6% similar despite different names*

```diff
@@ -152,36 +152,42 @@
   return os.str();
 }
 
 }  // namespace
 }  // namespace sentencepiece
 
 int main(int argc, char **argv) {
+  sentencepiece::ScopedResourceDestructor cleaner;
   sentencepiece::ParseCommandLineFlags(argv[0], &argc, &argv, true);
 
   const std::vector<std::pair<
       std::string,
       std::function<sentencepiece::util::Status(Builder::CharsMap *)>>>
       kRuleList = {{"nfkc", Builder::BuildNFKCMap},
                    {"nmt_nfkc", Builder::BuildNmtNFKCMap},
                    {"nfkc_cf", Builder::BuildNFKC_CFMap},
-                   {"nmt_nfkc_cf", Builder::BuildNmtNFKC_CFMap}};
+                   {"nmt_nfkc_cf", Builder::BuildNmtNFKC_CFMap},
+                   {"nfkd", Builder::BuildNFKDMap}};
 
   std::vector<std::pair<std::string, std::string>> data;
   for (const auto &p : kRuleList) {
     Builder::CharsMap normalized_map;
     CHECK_OK(p.second(&normalized_map));
 
     // Write Header.
     std::string index;
     CHECK_OK(Builder::CompileCharsMap(normalized_map, &index));
-    data.emplace_back(p.first, index);
 
     // Write TSV file.
     CHECK_OK(Builder::SaveCharsMap(p.first + ".tsv", normalized_map));
+
+    // Do not make NFKD map as it is optionally created.
+    if (p.first.find("nfkd") != std::string::npos) continue;
+
+    data.emplace_back(p.first, index);
   }
 
   if (absl::GetFlag(FLAGS_output_precompiled_header)) {
     constexpr char kPrecompiledHeaderFileName[] = "normalization_rule.h";
     auto output =
         sentencepiece::filesystem::NewWritableFile(kPrecompiledHeaderFileName);
     CHECK_OK(output->status());
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/error.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/error.cc`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
 #include <cstring>
 
 #include "common.h"
+#include "init.h"
 #include "sentencepiece_processor.h"
 
 #ifdef _USE_EXTERNAL_ABSL
 // Naive workaround to define minloglevel on external absl package.
 // We want to define them in other cc file.
 #include "third_party/absl/flags/flag.h"
 #include "third_party/absl/flags/parse.h"
@@ -31,22 +32,24 @@
 int gTestCounter = 0;
 
 void Abort() {
   if (GetTestCounter() == 1) {
     SetTestCounter(2);
   } else {
     std::cerr << "Program terminated with an unrecoverable error." << std::endl;
+    ShutdownLibrary();
     exit(-1);
   }
 }
 
 void Exit(int code) {
   if (GetTestCounter() == 1) {
     SetTestCounter(2);
   } else {
+    ShutdownLibrary();
     exit(code);
   }
 }
 
 void SetTestCounter(int c) { gTestCounter = c; }
 bool GetTestCounter() { return gTestCounter; }
 }  // namespace error
@@ -57,23 +60,18 @@
 Status::~Status() {}
 
 struct Status::Rep {
   StatusCode code;
   std::string error_message;
 };
 
-Status::Status(StatusCode code, const char* error_message) : rep_(new Rep) {
-  rep_->code = code;
-  rep_->error_message = error_message;
-}
-
-Status::Status(StatusCode code, const std::string& error_message)
+Status::Status(StatusCode code, absl::string_view error_message)
     : rep_(new Rep) {
   rep_->code = code;
-  rep_->error_message = error_message;
+  rep_->error_message = std::string(error_message);
 }
 
 Status::Status(const Status& s)
     : rep_((s.rep_ == nullptr) ? nullptr : new Rep(*s.rep_)) {}
 
 void Status::operator=(const Status& s) {
   if (rep_ != s.rep_)
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/filesystem.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/filesystem.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/filesystem_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/filesystem_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/freelist.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist.h`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,21 @@
     chunk_index_ = 0;
     element_index_ = 0;
   }
 
   // Returns the number of allocated elements.
   size_t size() const { return chunk_size_ * chunk_index_ + element_index_; }
 
+  void swap(FreeList<T>& other) {
+    std::swap(freelist_, other.freelist_);
+    std::swap(element_index_, other.element_index_);
+    std::swap(chunk_index_, other.chunk_index_);
+    std::swap(chunk_size_, other.chunk_size_);
+  }
+
   // Returns the element as an array.
   T* operator[](size_t index) const {
     return freelist_[index / chunk_size_] + index % chunk_size_;
   }
 
   // Allocates new element.
   T* Allocate() {
@@ -72,12 +79,12 @@
 
  private:
   std::vector<T*> freelist_;
 
   // The last element is stored at freelist_[chunk_index_][element_index_]
   size_t element_index_ = 0;
   size_t chunk_index_ = 0;
-  const size_t chunk_size_ = 0;
+  size_t chunk_size_ = 0;  // Do not modify except in swap()
 };
 }  // namespace model
 }  // namespace sentencepiece
 #endif  // FREELIST_H_
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/freelist_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/freelist_test.cc`

 * *Files 14% similar despite different names*

```diff
@@ -26,23 +26,26 @@
 
   for (size_t i = 0; i < kSize; ++i) {
     int *n = l.Allocate();
     EXPECT_EQ(0, *n);
     *n = i;
   }
 
-  EXPECT_EQ(kSize, l.size());
+  FreeList<int> l2(3);  // Test swap()
+  l.swap(l2);
+
+  EXPECT_EQ(kSize, l2.size());
   for (size_t i = 0; i < kSize; ++i) {
-    EXPECT_EQ(i, *l[i]);
+    EXPECT_EQ(i, *l2[i]);
   }
 
-  l.Free();
-  EXPECT_EQ(0, l.size());
+  l2.Free();
+  EXPECT_EQ(0, l2.size());
 
   // Zero-initialized after `Free`.
   for (size_t i = 0; i < kSize; ++i) {
-    int *n = l.Allocate();
+    int *n = l2.Allocate();
     EXPECT_EQ(0, *n);
   }
 }
 }  // namespace model
 }  // namespace sentencepiece
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/init_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/init_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/model_factory.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/model_factory.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/model_factory_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/model_interface.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/model_interface.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface.h`

 * *Files 5% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 
 class ModelProto;
 
 // Underlying model interface.
 // Given a normalized string, returns a sequence of sentence pieces with ids.
 class ModelInterface {
  public:
-  using PieceToIdMap = absl::flat_hash_map<absl::string_view, int,
-                                           string_util::string_view_hash>;
+  using PieceToIdMap = absl::flat_hash_map<absl::string_view, int>;
+  //                                           string_util::string_view_hash>;
 
   absl::string_view unk_piece() const;
   absl::string_view bos_piece() const;
   absl::string_view eos_piece() const;
   absl::string_view pad_piece() const;
 
   // `model_proto` should not be deleted until ModelInterface is destroyed.
@@ -73,27 +73,14 @@
 
   virtual const ModelProto &model_proto() const { return *model_proto_; }
 
   virtual const normalizer::PrefixMatcher *prefix_matcher() const {
     return matcher_.get();
   }
 
-  // Sets the encoder version. Currently only unigram has an optimized encoder.
-  // The optimized version is always used by default if there is one, so
-  // normally users do not need to call this function. This function is provided
-  // just in case that a user want to manually choose which encoder version to
-  // use.
-  virtual util::Status SetEncoderVersion(EncoderVersion encoder_version) {
-    encoder_version_ = encoder_version;
-    return util::OkStatus();
-  }
-
-  // Returns the current encoder version in use.
-  virtual EncoderVersion GetEncoderVersion() const { return encoder_version_; }
-
   // Given a normalized string, returns a sequence of sentence pieces with ids.
   // The concatenation of pieces must be the same as `normalized`.
   virtual EncodeResult Encode(absl::string_view normalized) const = 0;
 
   // The same as above, but returns nbest result with score.
   virtual NBestEncodeResult NBestEncode(absl::string_view normalized,
                                         int nbest_size) const {
@@ -103,34 +90,33 @@
 
   virtual EncodeResult SampleEncode(absl::string_view normalized,
                                     float alpha) const {
     LOG(ERROR) << "Not implemented.";
     return EncodeResult();
   }
 
-  // Sample `samples` many tokenizations from the segmentation lattice
+  // Sample `samples` many tokenisations from the segmentation lattice
   // If `wor` is true, the samples are taken without replacement, and the scores
   // are the inclusion probabilities of the elements in the sample; otherwise
   // the samples are taken with replacement and the scores are the log-probs of
   // sample elements
-  // If `include_best` is true, the best tokenization is always included in the
+  // If `include_best` is true, the best tokenisation is always included in the
   // sample, and the remaining elements are sampled excluding the best.
   virtual NBestEncodeResult SampleEncodeAndScore(absl::string_view normalized,
                                                  float alpha, int samples,
                                                  bool wor,
                                                  bool include_best) const {
     LOG(ERROR) << "Not implemented.";
     return {{EncodeResult(), 0.0}};
   }
 
   // Calculates the entropy of the segmentation lattice with inverse temperature
-  // `theta`.
-  // Uses a novel dynamic program to calculate the entropy.
+  // `alpha`. Uses a novel dynamic program to calculate the entropy.
   virtual float CalculateEntropy(absl::string_view normalized,
-                                 float theta) const {
+                                 float alpha) const {
     LOG(ERROR) << "Not implemented.";
     return 0.0;
   }
 
   // Return true if SampleEncode returns a valid result.
   virtual bool IsSampleEncodeAvailable() const { return false; }
 
@@ -252,16 +238,12 @@
 
   // piece -> id map for control, unknown, and byte pieces
   PieceToIdMap reserved_id_map_;
 
   // unknown id.
   int unk_id_ = 0;
 
-  // The encoder version. Currently it is only effective for unigram model but
-  // ignored by other models.
-  EncoderVersion encoder_version_ = EncoderVersion::kOptimized;
-
   // status.
   util::Status status_;
 };
 }  // namespace sentencepiece
 #endif  // MODEL_INTERFACE_H_
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/model_interface_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/model_interface_test.cc`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
-#include "model_factory.h"
 #include "model_interface.h"
+
+#include "model_factory.h"
 #include "testharness.h"
 #include "third_party/absl/container/flat_hash_map.h"
 #include "util.h"
 
 namespace sentencepiece {
 namespace {
 
@@ -477,30 +478,14 @@
   EXPECT_EQ(PieceToByte("<0x000>"), -1);
   EXPECT_EQ(PieceToByte("<0x001>"), -1);
   EXPECT_EQ(PieceToByte("<0xff>"), -1);
   EXPECT_EQ(PieceToByte("<0xFG>"), -1);
   EXPECT_EQ(PieceToByte("a"), -1);
 }
 
-TEST(ModelInterfaceTest, SetEncoderVersion) {
-  for (const auto type : kModelTypes) {
-    ModelProto model_proto = MakeBaseModelProto(type);
-    AddPiece(&model_proto, "a");
-    AddPiece(&model_proto, "b");
-    auto model = ModelFactory::Create(model_proto);
-
-    // Verify the default encoder version.
-    EXPECT_EQ(EncoderVersion::kOptimized, model->GetEncoderVersion());
-
-    // Set the encoder version to original and verify.
-    EXPECT_TRUE(model->SetEncoderVersion(EncoderVersion::kOriginal).ok());
-    EXPECT_EQ(EncoderVersion::kOriginal, model->GetEncoderVersion());
-  }
-}
-
 TEST(ModelInterfaceTest, VerifyOutputsEquivalent) {
   for (const auto type : kModelTypes) {
     ModelProto model_proto = MakeBaseModelProto(type);
     AddPiece(&model_proto, "a", 1.0);
     AddPiece(&model_proto, "b", 2.0);
     auto model = ModelFactory::Create(model_proto);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/normalization_rule.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalization_rule.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/normalizer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.cc`

 * *Files 1% similar despite different names*

```diff
@@ -43,17 +43,15 @@
   Init();
 }
 
 Normalizer::~Normalizer() {}
 
 void Normalizer::Init() {
   absl::string_view index = spec_->precompiled_charsmap();
-  if (index.empty()) {
-    LOG(INFO) << "precompiled_charsmap is empty. use identity normalization.";
-  } else {
+  if (!index.empty()) {
     absl::string_view trie_blob, normalized;
 #ifdef IS_BIG_ENDIAN
     status_ = DecodePrecompiledCharsMap(index, &trie_blob, &normalized,
                                         &precompiled_charsmap_buffer_);
 #else
     status_ = DecodePrecompiledCharsMap(index, &trie_blob, &normalized);
 #endif
@@ -277,15 +275,16 @@
 util::Status Normalizer::DecodePrecompiledCharsMap(
     absl::string_view blob, absl::string_view *trie_blob,
     absl::string_view *normalized, std::string *buffer) {
   uint32 trie_blob_size = 0;
   if (blob.size() <= sizeof(trie_blob_size) ||
       !string_util::DecodePOD<uint32>(
           absl::string_view(blob.data(), sizeof(trie_blob_size)),
-          &trie_blob_size)) {
+          &trie_blob_size) ||
+      trie_blob_size >= blob.size()) {
     return util::InternalError("Blob for normalization rule is broken.");
   }
 
 #ifdef IS_BIG_ENDIAN
   trie_blob_size = util::Swap32(trie_blob_size);
 #endif
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/normalizer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer.h`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 #include <vector>
 
 #include "common.h"
 #include "sentencepiece_model.pb.h"
 #include "sentencepiece_processor.h"
 #include "third_party/absl/strings/string_view.h"
 #include "third_party/darts_clone/darts.h"
-#include "util.h"
 
 namespace sentencepiece {
 namespace normalizer {
 
 // Given a list of strings, finds the longest string which is a
 // prefix of a query.
 class PrefixMatcher {
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/normalizer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/normalizer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/pretokenizer_for_training.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.cc`

 * *Files 14% similar despite different names*

```diff
@@ -7,57 +7,63 @@
 //     http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
+#include "pretokenizer_for_training.h"
+
 #include <string>
 
-#include "pretokenizer_for_training.h"
 #include "third_party/absl/strings/str_replace.h"
 
 namespace sentencepiece {
 namespace pretokenizer {
 
 namespace {
 // TODO(taku): They are defined in trainer_interface.h but we
 // defined them explicitly to avoid the dependency to trainier_interface.
 // Currently, we have no separated build rules.
 const char kWSStr[] = "\xe2\x96\x81";
-const char kUPPBoundaryStr[] = "\t";
 }  // namespace
 
-std::string PretokenizerForTrainingInterface::PreTokenize(
+std::vector<std::string> PretokenizerForTrainingInterface::PreTokenize(
     absl::string_view text) const {
   return Postprocess(Tokenize(Preprocess(text)));
 }
 
 // static
 std::string PretokenizerForTrainingInterface::Preprocess(
     absl::string_view text) {
   // Escapes kWSStr (_) as this character may not be processed by pre-tokenizer.
   return absl::StrReplaceAll(text, {{kWSStr, " "}});
 }
 
 // static
-std::string PretokenizerForTrainingInterface::Postprocess(
+std::vector<std::string> PretokenizerForTrainingInterface::Postprocess(
     const SentencePieceText &spt) {
   // Inserts kUPPBoundaryStr before/after of token boundaries.
+  std::vector<std::string> result;
   std::string output;
+
   int prev = 0;
   for (const auto &piece : spt.pieces()) {
     if (prev == piece.begin() && piece.begin() != 0) {
-      output += kUPPBoundaryStr;
+      result.push_back(output);
+      output.clear();
     } else {
       output.append(piece.begin() - prev, ' ');
     }
     output += piece.surface();
     prev = piece.end();
   }
 
-  // Restores kWSStr.
-  return absl::StrReplaceAll(output, {{" ", kWSStr}});
+  if (!output.empty()) result.push_back(output);
+
+  for (auto &w : result) w = absl::StrReplaceAll(w, {{" ", kWSStr}});
+
+  return result;
 }
 
 }  // namespace pretokenizer
 }  // namespace sentencepiece
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/pretokenizer_for_training.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training.h`

 * *Files 10% similar despite different names*

```diff
@@ -40,24 +40,24 @@
   // output: 東京<tab>です (here kUPPBoundaryStr is <tab>)
   //
   // Example2:
   // input: I love sentencepiece
   // segmentation: piece[0] = {0, 1}, piece[1] = {2, 6},
   //               piece[2] = {7, 15}, piece[3] = {15, 20}
   // output: I love sentence<tab>piece.
-  std::string PreTokenize(absl::string_view text) const;
+  std::vector<std::string> PreTokenize(absl::string_view text) const;
 
   // Returns pre-tokenized result.
   // Note that the pre-tokenized constraint is specified with the
   // byte offsets (SentencePiece::begin, SentencePiece::end) over
   // the input text.
   virtual SentencePieceText Tokenize(absl::string_view text) const = 0;
 
  private:
   static std::string Preprocess(absl::string_view text);
-  static std::string Postprocess(const SentencePieceText &spt);
+  static std::vector<std::string> Postprocess(const SentencePieceText &spt);
 };
 
 }  // namespace pretokenizer
 }  // namespace sentencepiece
 
 #endif  // PRETOKENIZER_FOR_TRAINING_H_
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/pretokenizer_for_training_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/pretokenizer_for_training_test.cc`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 #include "pretokenizer_for_training.h"
+
 #include "testharness.h"
 #include "third_party/absl/strings/str_cat.h"
+#include "third_party/absl/strings/str_join.h"
+#include "third_party/absl/strings/str_split.h"
 #include "trainer_interface.h"
 
 namespace sentencepiece {
 namespace pretokenizer {
 
 class MockPretokenizer : public PretokenizerForTrainingInterface {
  public:
@@ -60,17 +63,19 @@
     auto *p4 = spt.add_pieces();
     p4->set_surface("piece");
     p4->set_begin(15);
     p4->set_end(20);
 
     mock.SetOutput(spt);
 
-    EXPECT_EQ(absl::StrCat("I", TrainerInterface::kWSStr, "love",
-                           TrainerInterface::kWSStr, "sentence\tpiece"),
-              mock.PreTokenize("I love sentencepiece"));
+    const auto expected =
+        absl::StrCat("I", TrainerInterface::kWSStr, "love",
+                     TrainerInterface::kWSStr, "sentence||||piece");
+    EXPECT_EQ(expected,
+              absl::StrJoin(mock.PreTokenize("I love sentencepiece"), "||||"));
   }
 
   {
     SentencePieceText spt;
     spt.set_text("これはペンです");
     auto *p1 = spt.add_pieces();
     p1->set_surface("これ");
@@ -90,13 +95,15 @@
     auto *p4 = spt.add_pieces();
     p4->set_surface("です");
     p4->set_begin(15);
     p4->set_end(21);
 
     mock.SetOutput(spt);
 
-    EXPECT_EQ("これ\tは\tペン\tです", mock.PreTokenize("これはペンです"));
+    const auto expected = "これ||||は||||ペン||||です";
+    EXPECT_EQ(expected,
+              absl::StrJoin(mock.PreTokenize("これはペンです"), "||||"));
   }
 }
 
 }  // namespace pretokenizer
 }  // namespace sentencepiece
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_processor.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.cc`

 * *Files 13% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "sentencepiece_processor.h"
+
 #include <map>
 #include <set>
 #include <utility>
 
 #include "common.h"
 #include "filesystem.h"
 #include "model_factory.h"
 #include "model_interface.h"
 #include "normalizer.h"
 #include "sentencepiece.pb.h"
-#include "sentencepiece_processor.h"
 #include "third_party/absl/memory/memory.h"
 #include "third_party/absl/strings/numbers.h"
 #include "third_party/absl/strings/str_cat.h"
 #include "third_party/absl/strings/str_join.h"
 #include "third_party/absl/strings/str_replace.h"
 #include "third_party/absl/strings/str_split.h"
 #include "third_party/absl/strings/string_view.h"
@@ -43,16 +44,173 @@
 // Encodes <unk> into U+2047 (DOUBLE QUESTION MARK),
 // since this character can be useful both for user and
 // developer. We can easily figure out that <unk> is emitted.
 const char kDefaultUnknownSymbol[] = " \xE2\x81\x87 ";
 
 // REPLACEMENT CHARACTER (U+FFFD) in UTF-8.
 const char kReplacementCharacter[] = "\xef\xbf\xbd";
+
+std::vector<absl::string_view> ToPieceArray(const std::vector<std::string> &v) {
+  std::vector<absl::string_view> out(v.size());
+  for (int i = 0; i < v.size(); ++i) out[i] = v[i];
+  return out;
+}
+
+void ConvertToUnicodeSpansInternal(SentencePieceText *spt) {
+  if (spt == nullptr || spt->text().empty()) return;
+
+  std::vector<int> utf8_to_unicode(spt->text().size() + 1, 0);
+  absl::string_view str = spt->text();
+  size_t prev = 0;
+  int ulen = 0;
+  while (!str.empty()) {
+    const size_t mblen = std::max<int>(1, string_util::OneCharLen(str.data()));
+    for (int i = prev; i < prev + mblen; ++i) {
+      utf8_to_unicode[i] = ulen;
+    }
+    ++ulen;
+    prev += mblen;
+    str.remove_prefix(mblen);
+  }
+  utf8_to_unicode[prev] = ulen;
+
+  auto clip = [&](int s) {
+    return std::min<int>(std::max<int>(0, s), utf8_to_unicode.size() - 1);
+  };
+
+  for (auto &piece : *(spt->mutable_pieces())) {
+    piece.set_begin(utf8_to_unicode[clip(piece.begin())]);
+    piece.set_end(utf8_to_unicode[clip(piece.end())]);
+  }
+}
+
 }  // namespace
 
+ImmutableSentencePieceText::ImmutableSentencePieceText()
+    : spt_(&SentencePieceText::default_instance()) {}
+
+ImmutableSentencePieceText::ImmutableSentencePieceText(
+    const SentencePieceText &spt)
+    : spt_(&spt) {}
+
+ImmutableSentencePieceText::~ImmutableSentencePieceText() {}
+
+ImmutableSentencePieceText_ImmutableSentencePiece::
+    ImmutableSentencePieceText_ImmutableSentencePiece()
+    : sp_(&SentencePieceText_SentencePiece::default_instance()) {}
+
+ImmutableSentencePieceText_ImmutableSentencePiece::
+    ImmutableSentencePieceText_ImmutableSentencePiece(
+        const SentencePieceText_SentencePiece &sp)
+    : sp_(&sp) {}
+
+const std::string &ImmutableSentencePieceText_ImmutableSentencePiece::piece()
+    const {
+  return sp_->piece();
+}
+
+const std::string &ImmutableSentencePieceText_ImmutableSentencePiece::surface()
+    const {
+  return sp_->surface();
+}
+
+uint32_t ImmutableSentencePieceText_ImmutableSentencePiece::id() const {
+  return sp_->id();
+}
+
+uint32_t ImmutableSentencePieceText_ImmutableSentencePiece::begin() const {
+  return sp_->begin();
+}
+
+uint32_t ImmutableSentencePieceText_ImmutableSentencePiece::end() const {
+  return sp_->end();
+}
+
+std::vector<ImmutableSentencePieceText_ImmutableSentencePiece>
+ImmutableSentencePieceText::pieces() const {
+  std::vector<ImmutableSentencePieceText_ImmutableSentencePiece> pieces(
+      spt_->pieces_size());
+  for (int i = 0; i < spt_->pieces_size(); ++i)
+    pieces[i] =
+        ImmutableSentencePieceText_ImmutableSentencePiece(spt_->pieces(i));
+  return pieces;
+}
+
+size_t ImmutableSentencePieceText::pieces_size() const {
+  return spt_->pieces_size();
+}
+
+ImmutableSentencePieceText_ImmutableSentencePiece
+ImmutableSentencePieceText::pieces(int index) const {
+  return ImmutableSentencePieceText_ImmutableSentencePiece(spt_->pieces(index));
+}
+
+const std::string &ImmutableSentencePieceText::text() const {
+  return spt_->text();
+}
+
+float ImmutableSentencePieceText::score() const {
+  return spt_ ? spt_->score() : 0.0;
+}
+
+SentencePieceText *ImmutableSentencePieceText::mutable_proto() {
+  if (rep_ == nullptr) {
+    rep_ = std::make_shared<SentencePieceText>();
+    spt_ = rep_.get();
+  }
+  return rep_.get();
+}
+
+void ImmutableSentencePieceText::ConvertToUnicodeSpans() {
+  ConvertToUnicodeSpansInternal(mutable_proto());
+}
+
+util::bytes ImmutableSentencePieceText::SerializeAsString() const {
+  return spt_->SerializeAsString();
+}
+
+ImmutableNBestSentencePieceText::ImmutableNBestSentencePieceText() {}
+ImmutableNBestSentencePieceText::~ImmutableNBestSentencePieceText() {}
+
+size_t ImmutableNBestSentencePieceText::nbests_size() const {
+  return rep_ ? rep_->nbests_size() : 0;
+}
+
+ImmutableSentencePieceText ImmutableNBestSentencePieceText::nbests(
+    int index) const {
+  return ImmutableSentencePieceText(rep_->nbests(index));
+}
+
+std::vector<ImmutableSentencePieceText>
+ImmutableNBestSentencePieceText::nbests() const {
+  if (rep_ == nullptr) return {};
+  std::vector<ImmutableSentencePieceText> nbests(rep_->nbests_size());
+  for (int i = 0; i < rep_->nbests_size(); ++i)
+    nbests[i] = ImmutableSentencePieceText(rep_->nbests(i));
+  return nbests;
+}
+
+NBestSentencePieceText *ImmutableNBestSentencePieceText::mutable_proto() {
+  if (rep_ == nullptr) {
+    rep_ = std::make_shared<NBestSentencePieceText>();
+  }
+  return rep_.get();
+}
+
+void ImmutableNBestSentencePieceText::ConvertToUnicodeSpans() {
+  if (!mutable_proto()) return;
+  for (auto &spt : *(mutable_proto()->mutable_nbests())) {
+    ConvertToUnicodeSpansInternal(&spt);
+  }
+}
+
+util::bytes ImmutableNBestSentencePieceText::SerializeAsString() const {
+  return rep_ ? rep_->SerializeAsString() : "";
+}
+
 SentencePieceProcessor::SentencePieceProcessor() {}
 SentencePieceProcessor::~SentencePieceProcessor() {}
 
 util::Status SentencePieceProcessor::Load(absl::string_view filename) {
   auto model_proto = absl::make_unique<ModelProto>();
   RETURN_IF_ERROR(io::LoadModelProto(filename, model_proto.get()));
   return Load(std::move(model_proto));
@@ -113,23 +271,14 @@
     }
     return util::InternalError("Self-test failures. See LOG(INFO).");
   }
 
   return util::OkStatus();
 }
 
-util::Status SentencePieceProcessor::SetEncoderVersion(
-    EncoderVersion encoder_version) {
-  return model_->SetEncoderVersion(encoder_version);
-}
-
-EncoderVersion SentencePieceProcessor::GetEncoderVersion() const {
-  return model_->GetEncoderVersion();
-}
-
 util::Status SentencePieceProcessor::SetEncodeExtraOptions(
     absl::string_view extra_options) {
   return ParseExtraOptions(extra_options, &encode_extra_options_);
 }
 
 util::Status SentencePieceProcessor::SetDecodeExtraOptions(
     absl::string_view extra_options) {
@@ -141,23 +290,24 @@
   CHECK_OR_RETURN(normalizer_) << "Normalizer is not initialized.";
   RETURN_IF_ERROR(model_->status());
   RETURN_IF_ERROR(normalizer_->status());
   return util::OkStatus();
 }
 
 util::Status SentencePieceProcessor::SetVocabulary(
-    const std::vector<std::string> &valid_vocab) {
+    const std::vector<absl::string_view> &valid_vocab) {
   RETURN_IF_ERROR(status());
 
   // TODO(taku): supports vocabulary constraint in BPE model.
   const auto type = model_proto_->trainer_spec().model_type();
   CHECK_OR_RETURN(type == TrainerSpec::UNIGRAM || type == TrainerSpec::BPE)
       << "Vocabulary constraint is only enabled in subword units.";
 
-  const std::set<std::string> vocab(valid_vocab.begin(), valid_vocab.end());
+  const std::set<absl::string_view> vocab(valid_vocab.begin(),
+                                          valid_vocab.end());
 
   for (int i = 0; i < model_proto_->pieces_size(); ++i) {
     auto *piece = model_proto_->mutable_pieces(i);
     if (piece->type() == ModelProto::SentencePiece::CONTROL ||
         piece->type() == ModelProto::SentencePiece::UNKNOWN ||
         piece->type() == ModelProto::SentencePiece::USER_DEFINED) {
       continue;
@@ -202,15 +352,15 @@
           << "Could not parse the frequency";
     }
     if (freq >= threshold) {
       vocab.emplace_back(v[0]);
     }
   }
 
-  return SetVocabulary(vocab);
+  return SetVocabulary(ToPieceArray(vocab));
 }
 
 #define CHECK_OR_RETURN_STATUS_STL(container)               \
   RETURN_IF_ERROR(status());                                \
   CHECK_OR_RETURN(container) << "output container is null"; \
   container->clear();
 
@@ -245,14 +395,20 @@
   }
 
   return util::OkStatus();
 }
 
 util::Status SentencePieceProcessor::Decode(
     const std::vector<std::string> &pieces, std::string *detokenized) const {
+  return Decode(ToPieceArray(pieces), detokenized);
+}
+
+util::Status SentencePieceProcessor::Decode(
+    const std::vector<absl::string_view> &pieces,
+    std::string *detokenized) const {
   CHECK_OR_RETURN_STATUS_STL(detokenized);
 
   SentencePieceText spt;
   RETURN_IF_ERROR(Decode(pieces, &spt));
   *detokenized = std::move(spt.text());
 
   return util::OkStatus();
@@ -329,14 +485,64 @@
   for (const auto &sp : spt.pieces()) {
     ids->emplace_back(sp.id());
   }
 
   return util::OkStatus();
 }
 
+util::Status SentencePieceProcessor::SampleEncodeAndScore(
+    absl::string_view input, int num_samples, float alpha, bool wor,
+    bool include_best,
+    std::vector<std::pair<std::vector<std::string>, float>> *pieces) const {
+  CHECK_OR_RETURN_STATUS_STL(pieces);
+
+  NBestSentencePieceText spt;
+  RETURN_IF_ERROR(
+      SampleEncodeAndScore(input, num_samples, alpha, wor, include_best, &spt));
+
+  pieces->clear();
+  pieces->reserve(spt.nbests_size());
+
+  for (const auto &nbest : spt.nbests()) {
+    std::vector<std::string> result;
+    result.reserve(nbest.pieces_size());
+    for (const auto &sp : nbest.pieces()) {
+      result.emplace_back(sp.piece());
+    }
+    pieces->emplace_back(result, nbest.score());
+  }
+
+  return util::OkStatus();
+}
+
+util::Status SentencePieceProcessor::SampleEncodeAndScore(
+    absl::string_view input, int num_samples, float alpha, bool wor,
+    bool include_best,
+    std::vector<std::pair<std::vector<int>, float>> *ids) const {
+  CHECK_OR_RETURN_STATUS_STL(ids);
+
+  NBestSentencePieceText spt;
+  RETURN_IF_ERROR(
+      SampleEncodeAndScore(input, num_samples, alpha, wor, include_best, &spt));
+
+  ids->clear();
+  ids->reserve(spt.nbests_size());
+
+  for (const auto &nbest : spt.nbests()) {
+    std::vector<int> result;
+    result.reserve(nbest.pieces_size());
+    for (const auto &sp : nbest.pieces()) {
+      result.emplace_back(sp.id());
+    }
+    ids->emplace_back(result, nbest.score());
+  }
+
+  return util::OkStatus();
+}
+
 util::Status SentencePieceProcessor::PopulateSentencePieceText(
     absl::string_view input, absl::string_view normalized,
     const std::vector<size_t> &norm_to_orig, const EncodeResult &result,
     SentencePieceText *spt) const {
   size_t consumed = 0;
   bool is_prev_unk = false;
   for (const auto &p : result) {
@@ -500,23 +706,23 @@
                                               nbests[dist(*mt)].first, spt));
   }
 
   return util::OkStatus();
 }
 
 util::Status SentencePieceProcessor::SampleEncodeAndScore(
-    absl::string_view input, int samples, float theta, bool wor,
+    absl::string_view input, int samples, float alpha, bool wor,
     bool include_best, NBestSentencePieceText *samples_spt) const {
   CHECK_OR_RETURN(model_->IsSampleEncodeAndScoreAvailable())
       << "SampleEncodeAndScore is not available for the current model.";
   std::string normalized;
   std::vector<size_t> norm_to_orig;
   RETURN_IF_ERROR(normalizer_->Normalize(input, &normalized, &norm_to_orig));
 
-  const auto results = model_->SampleEncodeAndScore(normalized, theta, samples,
+  const auto results = model_->SampleEncodeAndScore(normalized, alpha, samples,
                                                     wor, include_best);
   CHECK_OR_RETURN(!results.empty())
       << "SampleEncodeAndScore returns empty result.";
 
   for (const auto &result : results) {
     auto *spt = samples_spt->add_nbests();
     spt->set_score(result.second);
@@ -524,62 +730,81 @@
                                               result.first, spt));
   }
 
   return util::OkStatus();
 }
 
 util::Status SentencePieceProcessor::CalculateEntropy(absl::string_view input,
-                                                      float theta,
+                                                      float alpha,
                                                       float *entropy) const {
   CHECK_OR_RETURN(model_->IsCalculateEntropyAvailable())
       << "CalculateEntropy is not available for the current model.";
   std::string normalized;
   std::vector<size_t> norm_to_orig;
   RETURN_IF_ERROR(normalizer_->Normalize(input, &normalized, &norm_to_orig));
 
-  *entropy = model_->CalculateEntropy(normalized, theta);
+  *entropy = model_->CalculateEntropy(normalized, alpha);
   return util::OkStatus();
 }
 
 util::Status SentencePieceProcessor::Decode(
     const std::vector<std::string> &pieces, SentencePieceText *spt) const {
+  return Decode(ToPieceArray(pieces), spt);
+}
+
+util::Status SentencePieceProcessor::Decode(
+    const std::vector<absl::string_view> &pieces,
+    SentencePieceText *spt) const {
   CHECK_OR_RETURN_STATUS_PROTO(spt);
 
   const char *unk_surface = kDefaultUnknownSymbol;
   if (model_proto_ && model_proto_->trainer_spec().has_unk_surface())
     unk_surface = model_proto_->trainer_spec().unk_surface().c_str();
 
-  auto DecodeSentencePiece = [&](absl::string_view piece, int id,
-                                 bool is_bos_ws) -> std::string {
-    if (IsControl(id)) {  // <s>, </s>
-      return "";          // invisible symbol.
+  // Returns decoded piece and a boolean indicating if the function has consumed
+  // a bos whitespace token (a piece starting with a kSpaceSymbol). This is used
+  // to strip only the first whitespace token from the decoded sequence for
+  // add_dummy_prefix.
+  auto DecodeSentencePiece =
+      [&](absl::string_view piece, int id,
+          bool is_bos_ws) -> std::pair<std::string, bool> {
+    if (IsControl(id)) {                 // <s>, </s>
+      return std::make_pair("", false);  // invisible symbol.
     } else if (IsUnknown(id)) {
       if (IdToPiece(id) == piece) {  // <unk>
-        return unk_surface;
+        return std::make_pair(unk_surface, false);
       } else {  // return piece when piece is not <unk>.
-        return std::string(piece);
+        return std::make_pair(std::string(piece), false);
       }
     }
 
+    bool has_bos_ws = false;  // whether the token starts with a kSpaceSymbol
     if (is_bos_ws &&
         (!model_proto_ ||
          (model_proto_ &&
           (model_proto_->normalizer_spec().add_dummy_prefix() ||
            model_proto_->normalizer_spec().remove_extra_whitespaces())))) {
       // Consume if the current position is bos and
       // piece starts with kSpaceSymbol.
-      absl::ConsumePrefix(&piece, kSpaceSymbol);
+      has_bos_ws = absl::ConsumePrefix(&piece, kSpaceSymbol);
+
+      if (model_proto_ &&
+          model_proto_->normalizer_spec().remove_extra_whitespaces()) {
+        // if we are removing extra whitespace, we remove all leading whitespace
+        has_bos_ws = false;
+      }
     }
 
-    return absl::StrReplaceAll(piece, {{kSpaceSymbol, " "}});
+    return std::make_pair(absl::StrReplaceAll(piece, {{kSpaceSymbol, " "}}),
+                          has_bos_ws);
   };
 
-  for (const std::string &w : pieces) {
+  for (absl::string_view w : pieces) {
     auto *sp = spt->add_pieces();
-    sp->set_piece(w);
+    sp->mutable_piece()->assign(w.data(), w.size());
     sp->set_id(PieceToId(w));
   }
 
   RETURN_IF_ERROR(ApplyExtraOptions(decode_extra_options_, spt));
 
   std::string *text = spt->mutable_text();
   auto SetSurface = [&](int index, absl::string_view surface) {
@@ -640,20 +865,31 @@
     }
     CHECK_EQ_OR_RETURN(token_index_begin + offset, token_index_end);
 
     return util::OkStatus();
   };
 
   int byte_start = 0;
+  bool is_bos_ws = true;  // whether we expect a bos ws token to consume.
+  bool bos_ws_seen = false;
+  std::string decoded;
+
   for (int i = 0; i < spt->pieces_size(); ++i) {
     const auto &sp = spt->pieces(i);
     if (!IsByte(sp.id())) {
       RETURN_IF_ERROR(ProcessBytePieces(byte_start, i));
+
+      // if we have seen a bos_ws token or any non-empty token
+      if (bos_ws_seen || !text->empty()) is_bos_ws = false;
+
       byte_start = i + 1;
-      SetSurface(i, DecodeSentencePiece(sp.piece(), sp.id(), text->empty()));
+      std::tie(decoded, bos_ws_seen) =
+          DecodeSentencePiece(sp.piece(), sp.id(), is_bos_ws);
+
+      SetSurface(i, decoded);
     }
   }
   RETURN_IF_ERROR(ProcessBytePieces(byte_start, spt->pieces_size()));
 
   if (denormalizer_) {
     *text = denormalizer_->Normalize(*text);
   }
@@ -672,49 +908,14 @@
                           absl::StrCat("Invalid id: ", id));
     }
     pieces.emplace_back(IdToPiece(id));
   }
   return Decode(pieces, spt);
 }
 
-std::string SentencePieceProcessor::EncodeAsSerializedProto(
-    absl::string_view input) const {
-  SentencePieceText spt;
-  if (!Encode(input, &spt).ok()) return "";
-  return spt.SerializeAsString();
-}
-
-std::string SentencePieceProcessor::SampleEncodeAsSerializedProto(
-    absl::string_view input, int nbest_size, float alpha) const {
-  SentencePieceText spt;
-  if (!SampleEncode(input, nbest_size, alpha, &spt).ok()) return "";
-  return spt.SerializeAsString();
-}
-
-std::string SentencePieceProcessor::NBestEncodeAsSerializedProto(
-    absl::string_view input, int nbest_size) const {
-  NBestSentencePieceText spt;
-  if (!NBestEncode(input, nbest_size, &spt).ok()) return "";
-  return spt.SerializeAsString();
-}
-
-std::string SentencePieceProcessor::DecodePiecesAsSerializedProto(
-    const std::vector<std::string> &pieces) const {
-  SentencePieceText spt;
-  if (!Decode(pieces, &spt).ok()) return "";
-  return spt.SerializeAsString();
-}
-
-std::string SentencePieceProcessor::DecodeIdsAsSerializedProto(
-    const std::vector<int> &ids) const {
-  SentencePieceText spt;
-  if (!Decode(ids, &spt).ok()) return "";
-  return spt.SerializeAsString();
-}
-
 #define CHECK_STATUS_OR_RETURN_DEFAULT(value)                                \
   if (!status().ok()) {                                                      \
     LOG(ERROR) << status().message() << "\nReturns default value " << value; \
     return value;                                                            \
   }
 
 int SentencePieceProcessor::GetPieceSize() const {
@@ -805,14 +1006,23 @@
           array->SwapElements(i - 1, i);
         }
         auto *piece = array->Mutable(0);
         piece->set_id(PieceToId(absl::string_view(model_->bos_piece().data())));
         piece->set_piece(model_->bos_piece().data(),
                          model_->bos_piece().size());
       } break;
+      case UNK_PIECE: {
+        for (int i = 0; i < spt->pieces_size(); ++i) {
+          auto *piece = spt->mutable_pieces(i);
+          if (IsUnknown(piece->id())) {
+            piece->set_piece(model_->unk_piece().data(),
+                             model_->unk_piece().size());
+          }
+        }
+      } break;
       default:
         return util::InternalError("unknown extra_option type.");
     }
   }
 
   return util::OkStatus();
 }
@@ -827,15 +1037,17 @@
   if (extra_option.empty()) return util::OkStatus();
 
   RETURN_IF_ERROR(status());
 
   static std::map<absl::string_view, SentencePieceProcessor::ExtraOption>
       extra_option_map = {{"bos", SentencePieceProcessor::BOS},
                           {"eos", SentencePieceProcessor::EOS},
-                          {"reverse", SentencePieceProcessor::REVERSE}};
+                          {"reverse", SentencePieceProcessor::REVERSE},
+                          {"unk", SentencePieceProcessor::UNK_PIECE},
+                          {"unk_piece", SentencePieceProcessor::UNK_PIECE}};
   for (const auto &s : absl::StrSplit(extra_option, ":")) {
     const auto it = extra_option_map.find(s);
     CHECK_OR_RETURN(it != extra_option_map.end())
         << "option \"" << s << "\" is not available.";
     extra_options->push_back(it->second);
 
     if (it->second == SentencePieceProcessor::BOS) {
@@ -872,15 +1084,14 @@
 // Set seed value of random generator.
 // Do not set static_cast<unique_int>(-1),
 // as this seed is reserved for initializing from
 // std::random_device.
 void SetRandomGeneratorSeed(unsigned int seed);
 
 namespace io {
-
 util::Status LoadModelProto(absl::string_view filename,
                             ModelProto *model_proto) {
   if (filename.empty()) {
     return util::NotFoundError("model file path should not be empty.");
   }
 
   auto input = filesystem::NewReadableFile(filename, true);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_processor.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor.h`

 * *Files 20% similar despite different names*

```diff
@@ -14,48 +14,25 @@
 
 #ifndef SENTENCEPIECE_PROCESSOR_H_
 #define SENTENCEPIECE_PROCESSOR_H_
 
 #include <cstring>
 #include <memory>
 #include <string>
+#include <string_view>
 #include <utility>
 #include <vector>
 
-#if defined(_USE_INTERNAL_STRING_VIEW)
-#include "third_party/absl/strings/string_view.h"
-#elif defined(_USE_TF_STRING_VIEW)
-#include "absl/strings/string_view.h"
-#else
-// Minimum absl::string_view class that is used only for
-// the argument of public APIs.
+#ifndef SWIG
 namespace absl {
-class string_view {
- public:
-  string_view() : ptr_(nullptr), length_(0) {}
-  string_view(const std::string &str) : ptr_(str.data()), length_(str.size()) {}
-  string_view(const char *str) : ptr_(str), length_(std::strlen(str)) {}
-  string_view(const char *data, size_t len) : ptr_(data), length_(len) {}
-
-  const char *data() const { return ptr_; }
-  size_t size() const { return length_; }
-
- private:
-  const char *ptr_ = nullptr;
-  size_t length_ = 0;
-};
+using std::string_view;
 }  // namespace absl
-#endif
-
-namespace sentencepiece {
-
-#ifndef SWIG
-using EncodeResult = std::vector<std::pair<absl::string_view, int>>;
 #endif  // SWIG
 
+namespace sentencepiece {
 namespace util {
 
 enum class StatusCode : int {
   kOk = 0,
   kCancelled = 1,
   kUnknown = 2,
   kInvalidArgument = 3,
@@ -74,16 +51,15 @@
   kUnauthenticated = 16,
 };
 
 class Status {
  public:
   Status();
   ~Status();
-  Status(StatusCode code, const char *error_message);
-  Status(StatusCode code, const std::string &error_message);
+  Status(StatusCode code, absl::string_view error_message);
   Status(const Status &s);
   void operator=(const Status &s);
   bool operator==(const Status &s) const;
   bool operator!=(const Status &s) const;
   inline bool ok() const { return rep_ == nullptr; }
 
   void set_error_message(const char *str);
@@ -122,25 +98,25 @@
 // completely language independent.
 //
 // Usage:
 //   SentencePieceProcessor sp;
 //   sp.Load("//path/to/model");
 //
 //   vector<string> sps;
-//   sp.Encode("hello world.", &sps);
+//   sp.Encode("hello world.", &sps).IgnoreError();
 //
 //   vector<int> ids;
-//   sp.Encode("hello world.", &ids);
+//   sp.Encode("hello world.", &ids).IgnoreError();
 //
 //   string detok;
 //   sp.Decode(sps, &detok);
-//   CHECK_EQ("hello world.", detok);
+//   CHECK_EQ("hello world.", detok).IgnoreError();
 //
 //   sp.Decode(ids, &detok);
-//   CHECK_EQ("hello world.", detok);
+//   CHECK_EQ("hello world.", detok).IgnoreError();
 //
 //  We can also use SentencePieceText which manages the byte-offsets
 //  between user input (output) and internal sentence pieces.
 //
 //   SentencePieceText spt;
 //   sp.Encode("hello world.", &spt);
 //   // Emits the byte range of each piece.
@@ -159,28 +135,108 @@
 class SentencePieceText;
 class ModelProto;
 
 namespace normalizer {
 class Normalizer;
 }  // namespace normalizer
 
-// Defines the multiple versions of encoder within each model. Currently only
-// the Unigram model has an optimized encoder.
-enum class EncoderVersion {
-  kOptimized,  // The optimized encoder (default).
-  kOriginal    // The original encoder (user may choose to fall back to this
-               // just in case).
-};
-
+#ifndef SWIGGO
 namespace util {
 // Redefine std::string for serialized_proto interface as Python's string is
 // a Unicode string. We can enforce the return value to be raw byte sequence
 // with SWIG's typemap.
 using bytes = std::string;
 }  // namespace util
+#endif  // SWIGGO
+
+class NBestSentencePieceText;
+class ModelInterface;
+class SentencePieceText;
+class SentencePieceText_SentencePiece;
+
+// Wrapper class of SentencePieceText
+// This wrapper only allows an immutable access to the proto and
+// hides the actual implementation of protobuf.
+// See sentencepiece.proto for the details of this class.
+class ImmutableSentencePieceText_ImmutableSentencePiece {
+ public:
+  ImmutableSentencePieceText_ImmutableSentencePiece();
+  ~ImmutableSentencePieceText_ImmutableSentencePiece() = default;
+
+  const std::string &piece() const;
+  const std::string &surface() const;
+  uint32_t id() const;
+  uint32_t begin() const;
+  uint32_t end() const;
+
+  friend class ImmutableSentencePieceText;
+
+ private:
+  explicit ImmutableSentencePieceText_ImmutableSentencePiece(
+      const SentencePieceText_SentencePiece &sp);
+  const SentencePieceText_SentencePiece *sp_ = nullptr;
+};
+
+class ImmutableSentencePieceText {
+ public:
+  ImmutableSentencePieceText();
+  virtual ~ImmutableSentencePieceText();
+
+  std::vector<ImmutableSentencePieceText_ImmutableSentencePiece> pieces() const;
+
+  size_t pieces_size() const;
+  ImmutableSentencePieceText_ImmutableSentencePiece pieces(int index) const;
+
+  const std::string &text() const;
+  float score() const;
+
+  util::bytes SerializeAsString() const;
+
+  // Returns the actual mutable proto.
+  // Do not use this outside of SentencePieceProcessor, as
+  // it returns the raw pointer managed by the shared_ptr.
+  SentencePieceText *mutable_proto();
+
+  // Converts the utf8 byte spans into Unicode char span.
+  void ConvertToUnicodeSpans();
+
+  friend class ImmutableNBestSentencePieceText;
+
+ private:
+  explicit ImmutableSentencePieceText(const SentencePieceText &spt);
+  const SentencePieceText *spt_ = nullptr;
+  std::shared_ptr<SentencePieceText> rep_;
+};
+
+// Wrapper class of SentencePieceText
+// This wrapper only allows an immutable access to the proto and
+// hides the actual implementation of protobuf.
+// See sentencepiece.proto for the details of this class.
+class ImmutableNBestSentencePieceText {
+ public:
+  ImmutableNBestSentencePieceText();
+  virtual ~ImmutableNBestSentencePieceText();
+
+  std::vector<ImmutableSentencePieceText> nbests() const;
+
+  size_t nbests_size() const;
+  ImmutableSentencePieceText nbests(int index) const;
+
+  util::bytes SerializeAsString() const;
+
+  // Returns the actual mutable proto.
+  // Do not use this outside of SentencePieceProcessor, as
+  // it returns the raw pointer managed by the shared_ptr.
+  NBestSentencePieceText *mutable_proto();
+
+  void ConvertToUnicodeSpans();
+
+ private:
+  std::shared_ptr<NBestSentencePieceText> rep_;
+};
 
 class SentencePieceProcessor {
  public:
   SentencePieceProcessor();
   virtual ~SentencePieceProcessor();
 
   // Loads model from `filename`.
@@ -216,150 +272,187 @@
   // Vocabulary restriction.
   // Background:
   // https://github.com/rsennrich/subword-nmt#best-practice-advice-for-byte-pair-encoding-in-nmt
 
   // Restricts the vocabulary set.
   // The input sentences are encoded into the tokens in `valid_vocab`.
   virtual util::Status SetVocabulary(
-      const std::vector<std::string> &valid_vocab);
+      const std::vector<absl::string_view> &valid_vocab);
 
   // Reverts the vocabulary restriction.
   virtual util::Status ResetVocabulary();
 
   // Loads the valid vocabulary set from `filename` in TSV format.
   // Format:  <token> <tab> <freq>.
   // Any token with frequency < threshold will be treated as OOV.
   virtual util::Status LoadVocabulary(absl::string_view filename,
                                       int threshold);
 
   //////////////////////////////////////////////////////////////
-  // Simple API.
+  // Simple Encode and Decode API.
   //
   // Given a UTF8 input, encodes it into a sequence of sentence pieces.
   virtual util::Status Encode(absl::string_view input,
                               std::vector<std::string> *pieces) const;
 
   // Given a UTF8 input, encodes it into a sequence of ids.
   virtual util::Status Encode(absl::string_view input,
                               std::vector<int> *ids) const;
 
   // Given a sequence of pieces, decodes it into a detokenized output.
   virtual util::Status Decode(const std::vector<std::string> &pieces,
                               std::string *detokenized) const;
 
+  // Given a sequence of pieces, decodes it into a detokenized output.
+  virtual util::Status Decode(const std::vector<absl::string_view> &pieces,
+                              std::string *detokenized) const;
+
   // Given a sequence of ids, decodes it into a detokenized output.
   virtual util::Status Decode(const std::vector<int> &ids,
                               std::string *detokenized) const;
 
-  // Sets the encoder version. Normally users do not need to call this function.
-  // But they can call this fucntion just in case if they want to fall back to
-  // the original encoder.
-  virtual util::Status SetEncoderVersion(EncoderVersion encoder_version);
-
-  // Returns the current encoder version in use.
-  virtual EncoderVersion GetEncoderVersion() const;
-
   //////////////////////////////////////////////////////////////
   // NBest API.
+  //
   // Same as Encode, but returns nbest results.
   virtual util::Status NBestEncode(
       absl::string_view input, int nbest_size,
       std::vector<std::vector<std::string>> *pieces) const;
 
   // Same as Encode, but returns nbest results.
   virtual util::Status NBestEncode(absl::string_view input, int nbest_size,
                                    std::vector<std::vector<int>> *ids) const;
 
   //////////////////////////////////////////////////////////////
   // Sampling API.
+  //
   // Unigram and BPE support sampling mode.
   // - Unigram (--model_type=unigram):
-  // When `nbest_size` is positive value, approximately samples one
-  // segmentation from nbest candidates. When `nbest_size` is negative value,
-  // samples one segmentation from the hypotheses (Lattice) according to the
-  // generation probabilities using forward-filtering and backward-sampling
-  // algorithm. `alpha` is a smoothing parameter.  The best segmentation
-  // (Viterbi segmentation) is more likely sampled when setting larger
-  // alpha. When alpha is 0.0, one segmentation is uniformly sampled from the
-  // nbest or lattice.
-  // `nbest_size` and `alpha` correspond to parameters `l` and `alpha`
+  // `nbest_size`: When `nbest_size` is positive value, approximately samples
+  // one segmentation from nbest candidates. When `nbest_size` is negative
+  // value, samples one segmentation from the hypotheses (Lattice) according to
+  // the generation probabilities using forward-filtering and backward-sampling
+  // algorithm.
+  // `alpha`: Smoothing parameter (inverse temperature). The best segmentation
+  // (Viterbi segmentation) is more likely sampled when setting larger alpha.
+  // When alpha is 0.0, one segmentation is uniformly sampled from the nbest or
+  // lattice. `nbest_size` and `alpha` correspond to parameters `l` and `alpha`
   // in https://arxiv.org/abs/1804.10959  (nbest_size < 0 means l = infinity)
   //
   // - BPE (--model_type=bpe):
-  // `alpha` is the dropout probability `p` of bpe merge operations
-  // in https://arxiv.org/abs/1910.13267
-  // Nbest-based sampling is not supported so nbest_size parameter is ignored in
-  // BPE.
+  // `alpha`: The dropout probability `p` of bpe merge operations in
+  // https://arxiv.org/abs/1910.13267 Nbest-based sampling is not supported so
+  // nbest_size parameter is ignored in BPE.
   virtual util::Status SampleEncode(absl::string_view input, int nbest_size,
                                     float alpha,
                                     std::vector<std::string> *pieces) const;
 
   // Same as above, but returns a sequence of ids.
   virtual util::Status SampleEncode(absl::string_view input, int nbest_size,
                                     float alpha, std::vector<int> *ids) const;
 
   //////////////////////////////////////////////////////////////
+  // SampleEncodeAndScore API.
+  //
+  // Sample `samples` many tokenisations from the segmentation lattice.
+  // These methods are only available in model_type=unigram.
+  //
+  // `alpha`: smoothing parameter (inverse temperature). The same as `alpha` in
+  // `Sample` method.
+  // 'wor`: If `wor` is true, the samples are taken without replacement, and the
+  // scores are the inclusion probabilities of the elements in the sample;
+  // otherwise the samples are taken with replacement and the scores are the
+  // log-probs of sample elements
+  // `include_best`: If `include_best` is true, the best tokenisation is always
+  // included in the sample, and the remaining elements are sampled excluding
+  // the best.
+  virtual util::Status SampleEncodeAndScore(
+      absl::string_view input, int num_samples, float alpha, bool wor,
+      bool include_best,
+      std::vector<std::pair<std::vector<std::string>, float>> *pieces) const;
+
+  // Same as above, but returns a sequence of ids.
+  virtual util::Status SampleEncodeAndScore(
+      absl::string_view input, int num_samples, float alpha, bool wor,
+      bool include_best,
+      std::vector<std::pair<std::vector<int>, float>> *ids) const;
+
+  //////////////////////////////////////////////////////////////
+  // Entropy API.
+  //
+  // This only available in model_type=unigram.
+  // Calculate entropy of possible tokenisations
+  virtual util::Status CalculateEntropy(absl::string_view input, float alpha,
+                                        float *entropy) const;
+
+  //////////////////////////////////////////////////////////////
   // Advanced API returning SentencePieceText, which manages
   // utf8-byte alignments between user-input/detokenized text
   // and internal sentencepiece sequence.
   //
   // Given a UTF8 input, encodes it into SentencePieceText.
+  //
+  // When using these APIs, sentencepiece.pb.h header files must be included.
+  // We can also use ImutableSentencePieceText as follows.
+  //
+  // ImmutableSentencePieceText spt;
+  // Encode("hello", spt.mutable_proto()).IgnoreError();
+  // std::cout << spt.pieces_size() << std::endl;
   virtual util::Status Encode(absl::string_view input,
                               SentencePieceText *spt) const;
 
-  // Same as above, but returns NBestSentencePieceText.
   virtual util::Status NBestEncode(absl::string_view input, int nbest_size,
                                    NBestSentencePieceText *nbest_spt) const;
 
-  // Same as above, but samples one segmentation from the hypotheses
-  // (Lattice).
   virtual util::Status SampleEncode(absl::string_view input, int nbest_size,
                                     float alpha, SentencePieceText *spt) const;
 
-  // Sample `samples` segmentations from the segmentation lattice.
-  // If `wor` is true, the samples are taken without replacement, and the scores
-  // are the inclusion probabilities of the elements in the sample; otherwise
-  // the samples are taken with replacement and the scores are the log-probes of
-  // sample elements.
-  // If `include_best` is true, the best tokenization is always included in the
-  // sample, and the remaining elements are sampled excluding the best.
-  // This method is only available in Unigram mode.
   virtual util::Status SampleEncodeAndScore(
-      absl::string_view input, int samples, float theta, bool wor,
+      absl::string_view input, int num_samples, float alpha, bool wor,
       bool include_best, NBestSentencePieceText *samples_spt) const;
 
-  // Calculate entropy of possible tokenization.
-  // Only available in unigram mode.
-  virtual util::Status CalculateEntropy(absl::string_view input, float theta,
-                                        float *entropy) const;
-
-  // Given a sequence of pieces, decodes it into SentencePieceText.
+  // DEPRECATED: Remove this API and use std::vector<std::string_view>
   virtual util::Status Decode(const std::vector<std::string> &pieces,
                               SentencePieceText *spt) const;
 
-  // Given a sequence of ids, decodes it into SentencePieceText.
-  virtual util::Status Decode(const std::vector<int> &ids,
+  virtual util::Status Decode(const std::vector<absl::string_view> &pieces,
                               SentencePieceText *spt) const;
 
-  //////////////////////////////////////////////////////////////
-  // Handy methods that return the result directly.
-  // These functions ignore internal errors.
+  virtual util::Status Decode(const std::vector<int> &ids,
+                              SentencePieceText *spt) const;
 #ifdef SWIG
-#define DEFINE_SPP_DIRECT_FUNC_IMPL(FuncName, OutType, ...) \
-  OutType output;                                           \
-  const auto _status = FuncName(__VA_ARGS__, &output);      \
-  if (!_status.ok()) throw _status;                         \
-  return output;
+#define SPP_SWIG_CHECK_AND_THROW \
+  if (!status.ok()) throw status;
 #else
+#define SPP_SWIG_CHECK_AND_THROW \
+  if (!status.ok()) {            \
+  }
+#endif  // SWIG
+
 #define DEFINE_SPP_DIRECT_FUNC_IMPL(FuncName, OutType, ...) \
   OutType output;                                           \
-  FuncName(__VA_ARGS__, &output).IgnoreError();             \
+  const auto status = FuncName(__VA_ARGS__, &output);       \
+  SPP_SWIG_CHECK_AND_THROW;				    \
   return output;
-#endif
 
+#define DEFINE_SPP_SERIALIZED_PROTO_IMPL(FuncName, OutType, ...)     \
+  OutType output;                                                    \
+  const auto status = FuncName(__VA_ARGS__, output.mutable_proto()); \
+  SPP_SWIG_CHECK_AND_THROW;					     \
+  return output.SerializeAsString();
+
+#define DEFINE_SPP_IMMUTABLE_PROTO_IMPL(FuncName, OutType, ...)      \
+  OutType output;                                                    \
+  const auto status = FuncName(__VA_ARGS__, output.mutable_proto()); \
+  SPP_SWIG_CHECK_AND_THROW;					     \
+  return output;
+
+  //////////////////////////////////////////////////////////////
+  // Handy methods that return the result directly.
+  // These functions ignore internal errors.
   virtual std::vector<std::string> EncodeAsPieces(
       absl::string_view input) const {
     DEFINE_SPP_DIRECT_FUNC_IMPL(Encode, std::vector<std::string>, input);
   }
 
   virtual std::vector<int> EncodeAsIds(absl::string_view input) const {
     DEFINE_SPP_DIRECT_FUNC_IMPL(Encode, std::vector<int>, input);
@@ -387,42 +480,143 @@
   virtual std::vector<int> SampleEncodeAsIds(absl::string_view input,
                                              int nbest_size,
                                              float alpha) const {
     DEFINE_SPP_DIRECT_FUNC_IMPL(SampleEncode, std::vector<int>, input,
                                 nbest_size, alpha);
   }
 
+  virtual std::vector<std::pair<std::vector<std::string>, float>>
+  SampleEncodeAndScoreAsPieces(absl::string_view input, int num_samples,
+                               float alpha, bool wor, bool include_best) const {
+    using _T = std::vector<std::pair<std::vector<std::string>, float>>;
+    DEFINE_SPP_DIRECT_FUNC_IMPL(SampleEncodeAndScore, _T, input, num_samples,
+                                alpha, wor, include_best);
+  }
+
+  virtual std::vector<std::pair<std::vector<int>, float>>
+  SampleEncodeAndScoreAsIds(absl::string_view input, int num_samples,
+                            float alpha, bool wor, bool include_best) const {
+    using _T = std::vector<std::pair<std::vector<int>, float>>;
+    DEFINE_SPP_DIRECT_FUNC_IMPL(SampleEncodeAndScore, _T, input, num_samples,
+                                alpha, wor, include_best);
+  }
+
+  // DEPRECATED: Remove this API and use std::vector<std::string_view>
   virtual std::string DecodePieces(
       const std::vector<std::string> &pieces) const {
     DEFINE_SPP_DIRECT_FUNC_IMPL(Decode, std::string, pieces);
   }
 
+  virtual std::string DecodePieces(
+      const std::vector<absl::string_view> &pieces) const {
+    DEFINE_SPP_DIRECT_FUNC_IMPL(Decode, std::string, pieces);
+  }
+
   virtual std::string DecodeIds(const std::vector<int> &ids) const {
     DEFINE_SPP_DIRECT_FUNC_IMPL(Decode, std::string, ids);
   }
 
-#undef DEFINE_SPP_DIRECT_FUNC_IMPL
+  virtual float CalculateEntropy(absl::string_view text, float alpha) const {
+    DEFINE_SPP_DIRECT_FUNC_IMPL(CalculateEntropy, float, text, alpha);
+  }
 
+  //////////////////////////////////////////////////////////////
+  // SerializedProto API. (DEPRECATED). Use ImmutableProto API.
   // They are used in Python interface. Returns serialized proto.
   // In python module, we can get access to the full Proto after
   // deserialzing the returned byte sequence.
-  virtual util::bytes EncodeAsSerializedProto(absl::string_view input) const;
+  virtual util::bytes EncodeAsSerializedProto(absl::string_view input) const {
+    DEFINE_SPP_SERIALIZED_PROTO_IMPL(Encode, ImmutableSentencePieceText, input);
+  }
 
   virtual util::bytes SampleEncodeAsSerializedProto(absl::string_view input,
                                                     int nbest_size,
-                                                    float alpha) const;
+                                                    float alpha) const {
+    DEFINE_SPP_SERIALIZED_PROTO_IMPL(SampleEncode, ImmutableSentencePieceText,
+                                     input, nbest_size, alpha);
+  }
 
   virtual util::bytes NBestEncodeAsSerializedProto(absl::string_view input,
-                                                   int nbest_size) const;
+                                                   int nbest_size) const {
+    DEFINE_SPP_SERIALIZED_PROTO_IMPL(
+        NBestEncode, ImmutableNBestSentencePieceText, input, nbest_size);
+  }
 
+  virtual util::bytes SampleEncodeAndScoreAsSerializedProto(
+      absl::string_view input, int num_samples, float alpha, bool wor,
+      bool include_best) const {
+    DEFINE_SPP_SERIALIZED_PROTO_IMPL(SampleEncodeAndScore,
+                                     ImmutableNBestSentencePieceText, input,
+                                     num_samples, alpha, wor, include_best);
+  }
+
+  // TODO(taku): Remove this API and use std::vector<std::string_view>
   virtual util::bytes DecodePiecesAsSerializedProto(
-      const std::vector<std::string> &pieces) const;
+      const std::vector<std::string> &pieces) const {
+    DEFINE_SPP_SERIALIZED_PROTO_IMPL(Decode, ImmutableSentencePieceText,
+                                     pieces);
+  }
+
+  virtual util::bytes DecodePiecesAsSerializedProto(
+      const std::vector<absl::string_view> &pieces) const {
+    DEFINE_SPP_SERIALIZED_PROTO_IMPL(Decode, ImmutableSentencePieceText,
+                                     pieces);
+  }
 
   virtual util::bytes DecodeIdsAsSerializedProto(
-      const std::vector<int> &ids) const;
+      const std::vector<int> &ids) const {
+    DEFINE_SPP_SERIALIZED_PROTO_IMPL(Decode, ImmutableSentencePieceText, ids);
+  }
+
+  //////////////////////////////////////////////////////////////
+  // ImmutableProto API.
+  virtual ImmutableSentencePieceText EncodeAsImmutableProto(
+      absl::string_view input) const {
+    DEFINE_SPP_IMMUTABLE_PROTO_IMPL(Encode, ImmutableSentencePieceText, input);
+  }
+
+  virtual ImmutableSentencePieceText SampleEncodeAsImmutableProto(
+      absl::string_view input, int nbest_size, float alpha) const {
+    DEFINE_SPP_IMMUTABLE_PROTO_IMPL(SampleEncode, ImmutableSentencePieceText,
+                                    input, nbest_size, alpha);
+  }
+
+  virtual ImmutableNBestSentencePieceText NBestEncodeAsImmutableProto(
+      absl::string_view input, int nbest_size) const {
+    DEFINE_SPP_IMMUTABLE_PROTO_IMPL(
+        NBestEncode, ImmutableNBestSentencePieceText, input, nbest_size);
+  }
+
+  virtual ImmutableNBestSentencePieceText SampleEncodeAndScoreAsImmutableProto(
+      absl::string_view input, int num_samples, float alpha, bool wor,
+      bool include_best) const {
+    DEFINE_SPP_IMMUTABLE_PROTO_IMPL(SampleEncodeAndScore,
+                                    ImmutableNBestSentencePieceText, input,
+                                    num_samples, alpha, wor, include_best);
+  }
+
+  // TODO(taku): Remove this API and use std::vector<std::string_view>
+  virtual ImmutableSentencePieceText DecodePiecesAsImmutableProto(
+      const std::vector<std::string> &pieces) const {
+    DEFINE_SPP_IMMUTABLE_PROTO_IMPL(Decode, ImmutableSentencePieceText, pieces);
+  }
+
+  virtual ImmutableSentencePieceText DecodePiecesAsImmutableProto(
+      const std::vector<absl::string_view> &pieces) const {
+    DEFINE_SPP_IMMUTABLE_PROTO_IMPL(Decode, ImmutableSentencePieceText, pieces);
+  }
+
+  virtual ImmutableSentencePieceText DecodeIdsAsImmutableProto(
+      const std::vector<int> &ids) const {
+    DEFINE_SPP_IMMUTABLE_PROTO_IMPL(Decode, ImmutableSentencePieceText, ids);
+  }
+
+#undef DEFINE_SPP_DIRECT_FUNC_IMPL
+#undef DEFINE_SPP_SERIALIZED_PROTO_IMPL
+#undef DEFINE_SPP_IMMUTABLE_PROTO_IMPL
 
   //////////////////////////////////////////////////////////////
   // Vocabulary management methods.
   //
   // Returns the size of sentence pieces, which is the same as
   // the size of vocabulary for NMT.
   virtual int GetPieceSize() const;
@@ -431,15 +625,16 @@
   // Returns UNK(0) if `piece` is unknown.
   virtual int PieceToId(absl::string_view piece) const;
 
   // Returns the string representation of vocab with `id`.
   virtual const std::string &IdToPiece(int id) const;
 
   // Returns the score of `id`.
-  // Usually score is an emission log probability of unigram language model.
+  // Usually score is an emission log probability of unigram language
+  // model.
   virtual float GetScore(int id) const;
 
   // Returns true if `id` is unknown symbol.
   virtual bool IsUnknown(int id) const;
 
   // Returns true if `id` is control symbol.
   virtual bool IsControl(int id) const;
@@ -461,35 +656,33 @@
 
   // Returns EOS (</s>) id.
   virtual int eos_id() const;
 
   // Returns PAD (<pad>) id.
   virtual int pad_id() const;
 
-#ifndef SWIG
   //////////////////////////////////////////////////////////////
   // Model management.
   //
   // Allows injection of a mock model instance. `model` is moved.
   void SetModel(std::unique_ptr<ModelInterface> &&model);
 
   // Allows injection of a normalizer instance. `normalizer` is moved.
   void SetNormalizer(std::unique_ptr<normalizer::Normalizer> &&normalizer);
-#endif
 
   // Returns immutable model proto. Useful to obtain extended
   // or experimental parameters encoded in model_proto.
   const ModelProto &model_proto() const;
 
   // returns immutable model proto as std::string.
   // Useful to save the state of this instance via Python's pickle object.
   util::bytes serialized_model_proto() const;
 
  private:
-  enum ExtraOption { REVERSE, BOS, EOS };
+  enum ExtraOption { REVERSE, BOS, EOS, UNK_PIECE };
 
   util::Status ParseExtraOptions(absl::string_view extra_option,
                                  std::vector<ExtraOption> *extra_options) const;
 
   util::Status ApplyExtraOptions(const std::vector<ExtraOption> &extra_options,
                                  SentencePieceText *spt) const;
 
@@ -512,25 +705,23 @@
 
 // Set seed value of random generator.
 // Do not set static_cast<unique_int>(-1),
 // as this seed is reserved for initializing from
 // std::random_device.
 void SetRandomGeneratorSeed(unsigned int seed);
 
-#ifndef SWIG
 // IO related functions to absorb model formats.
 namespace io {
 // Loads `model_proto` from `filename`.
 // We can instantiate SentencePieceProcessor as follows:
 //
 //  auto model_proto = absl::make_unique<ModelProto>();
 //  io::LoadModelProto("//path/spm.model", model_proto.get());
 //  SentencePieceProcessor sp;
 //  CHECK_OK(sp.Load(std::move(model_proto)));
 util::Status LoadModelProto(absl::string_view, ModelProto *model_proto);
 
 // Saves `model_proto` as `filename`.
 util::Status SaveModelProto(absl::string_view, const ModelProto &model_proto);
 }  // namespace io
-#endif  // SWIG
 }  // namespace sentencepiece
 #endif  // SENTENCEPIECE_PROCESSOR_H_
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_processor_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_processor_test.cc`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "sentencepiece_processor.h"
+
 #include <utility>
 
 #include "builder.h"
 #include "filesystem.h"
 #include "model_interface.h"
 #include "normalizer.h"
 #include "sentencepiece.pb.h"
 #include "sentencepiece_model.pb.h"
-#include "sentencepiece_processor.h"
 #include "sentencepiece_trainer.h"
 #include "testharness.h"
 #include "third_party/absl/container/flat_hash_map.h"
 #include "third_party/absl/memory/memory.h"
 #include "third_party/absl/strings/str_cat.h"
 #include "third_party/absl/strings/string_view.h"
 #include "util.h"
@@ -547,18 +548,17 @@
     EncodeResult Encode(absl::string_view normalized) const override {
       return {};
     }
 
     int GetPieceSize() const override { return 7; }
 
     int PieceToId(absl::string_view piece) const override {
-      static absl::flat_hash_map<absl::string_view, int,
-                                 string_util::string_view_hash>
-          kMap = {{"<unk>", 0}, {"<s>", 1}, {"</s>", 2},    {WS "ABC", 3},
-                  {WS "DE", 4}, {"F", 5},   {"G" WS "H", 6}};
+      static absl::flat_hash_map<absl::string_view, int> kMap = {
+          {"<unk>", 0}, {"<s>", 1}, {"</s>", 2},    {WS "ABC", 3},
+          {WS "DE", 4}, {"F", 5},   {"G" WS "H", 6}};
       return port::FindWithDefault(kMap, piece, 0);
     }
 
     const std::string &IdToPiece(int id) const override {
       static std::vector<std::string> kMap = {
           "<unk>", "<s>", "</s>", WS "ABC", WS "DE", "F", "G" WS "H"};
       return kMap[id];
@@ -705,14 +705,94 @@
 
     EXPECT_TRUE(sp.Decode(input, &spt).ok());
     EXPECT_EQ(" ABC DEFG HI", spt.text());
     EXPECT_EQ(8, spt.pieces_size());
   }
 }
 
+TEST(SentencepieceProcessorTest, DummyPrefixDecodeTest) {
+  class DecodeMockModel : public ModelInterface {
+   public:
+    EncodeResult Encode(absl::string_view normalized) const override {
+      return {};
+    }
+
+    int GetPieceSize() const override { return 7; }
+
+    int PieceToId(absl::string_view piece) const override {
+      static absl::flat_hash_map<absl::string_view, int> kMap = {
+          {"<unk>", 0}, {"<s>", 1}, {"</s>", 2},     {WS "ABC", 3},
+          {WS "DE", 4}, {"F", 5},   {"G" WS "H", 6}, {WS, 7}};
+      return port::FindWithDefault(kMap, piece, 0);
+    }
+
+    const std::string &IdToPiece(int id) const override {
+      static std::vector<std::string> kMap = {
+          "<unk>", "<s>", "</s>", WS "ABC", WS "DE", "F", "G" WS "H", WS};
+      return kMap[id];
+    }
+
+    bool IsUnknown(int id) const override { return (id == 0); }
+
+    bool IsControl(int id) const override { return (id == 1 || id == 2); }
+
+    bool IsByte(int id) const override { return false; }
+
+    float GetScore(int id) const override { return 0.0; }
+  };
+
+  // start the sequence with a whitespace token
+  const std::vector<std::string> input = {
+      "<s>", WS, WS "ABC", "<unk>", WS "DE", "F", "G" WS "H", "I", "</s>"};
+
+  {
+    SentencePieceProcessor sp;
+    auto proto = absl::make_unique<ModelProto>();
+    proto->mutable_trainer_spec()->set_unk_surface("");
+    proto->mutable_normalizer_spec()->set_add_dummy_prefix(true);
+    proto->mutable_normalizer_spec()->set_remove_extra_whitespaces(false);
+    sp.Load(std::move(proto)).IgnoreError();
+
+    auto mock = absl::make_unique<DecodeMockModel>();
+    sp.SetModel(std::move(mock));
+
+    const auto normalization_spec = MakeDefaultNormalizerSpec();
+    sp.SetNormalizer(
+        absl::make_unique<normalizer::Normalizer>(normalization_spec));
+
+    SentencePieceText spt;
+
+    EXPECT_TRUE(sp.Decode(input, &spt).ok());
+    EXPECT_EQ(" ABC DEFG HI", spt.text());
+    EXPECT_EQ(9, spt.pieces_size());
+  }
+
+  {
+    SentencePieceProcessor sp;
+    auto proto = absl::make_unique<ModelProto>();
+    proto->mutable_trainer_spec()->set_unk_surface("");
+    proto->mutable_normalizer_spec()->set_add_dummy_prefix(true);
+    proto->mutable_normalizer_spec()->set_remove_extra_whitespaces(true);
+    sp.Load(std::move(proto)).IgnoreError();
+
+    auto mock = absl::make_unique<DecodeMockModel>();
+    sp.SetModel(std::move(mock));
+
+    const auto normalization_spec = MakeDefaultNormalizerSpec();
+    sp.SetNormalizer(
+        absl::make_unique<normalizer::Normalizer>(normalization_spec));
+
+    SentencePieceText spt;
+
+    EXPECT_TRUE(sp.Decode(input, &spt).ok());
+    EXPECT_EQ("ABC DEFG HI", spt.text());
+    EXPECT_EQ(9, spt.pieces_size());
+  }
+}
+
 TEST(SentencepieceProcessorTest, ByteFallbackDecodeTest) {
   class ByteFallbackDecodeMockModel : public ModelInterface {
    public:
     EncodeResult Encode(absl::string_view normalized) const override {
       return {};
     }
 
@@ -974,26 +1054,14 @@
 
   EXPECT_EQ(0, sp.unk_id());
   EXPECT_EQ(1, sp.bos_id());
   EXPECT_EQ(2, sp.eos_id());
   EXPECT_EQ(-1, sp.pad_id());
 
   {
-    // Verify the default encoder version.
-    EXPECT_EQ(EncoderVersion::kOptimized, sp.GetEncoderVersion());
-
-    // Set the encoder version to original and verify.
-    EXPECT_TRUE(sp.SetEncoderVersion(EncoderVersion::kOriginal).ok());
-    EXPECT_EQ(EncoderVersion::kOriginal, sp.GetEncoderVersion());
-
-    // Set back to the default encoder version.
-    EXPECT_TRUE(sp.SetEncoderVersion(EncoderVersion::kOptimized).ok());
-  }
-
-  {
     std::vector<std::string> sps;
     const std::vector<std::string> expected_str = {WS, "ab", "c"};
     EXPECT_TRUE(sp.Encode("abc", &sps).ok());
     EXPECT_EQ(expected_str, sps);
 
     std::vector<int> ids;
     const std::vector<int> expected_id = {7, 6, 5};
@@ -1489,8 +1557,157 @@
   EXPECT_TRUE(sp.LoadVocabulary(GetInlineFilename("aa\ndd\n"), 1).ok());
   EXPECT_FALSE(sp.IsUnused(3));
   EXPECT_TRUE(sp.IsUnused(4));
   EXPECT_TRUE(sp.IsUnused(5));
   EXPECT_FALSE(sp.IsUnused(6));
   EXPECT_FALSE(sp.IsUnused(7));
 }
+
+TEST(SentencePieceProcessorTest, ImmutableSentencePieceTextTest) {
+  ImmutableSentencePieceText spt;
+  EXPECT_TRUE(spt.text().empty());
+  EXPECT_EQ(spt.score(), 0.0);
+  EXPECT_TRUE(spt.SerializeAsString().empty());
+
+  auto *v = spt.mutable_proto();
+
+  v->set_text("hello world");
+  v->set_score(1.0);
+  for (int i = 0; i < 10; ++i) {
+    auto *p = v->add_pieces();
+    p->set_surface(absl::StrCat("surface_", i));
+    p->set_piece(absl::StrCat("surface_", i));
+    p->set_id(i);
+    p->set_begin(i + 10);
+    p->set_end(i + 20);
+  }
+
+  EXPECT_EQ(v->pieces_size(), spt.pieces_size());
+  for (int i = 0; i < spt.pieces_size(); ++i) {
+    EXPECT_EQ(v->pieces(i).surface(), spt.pieces(i).surface());
+    EXPECT_EQ(v->pieces(i).piece(), spt.pieces(i).piece());
+    EXPECT_EQ(v->pieces(i).id(), spt.pieces(i).id());
+    EXPECT_EQ(v->pieces(i).begin(), spt.pieces(i).begin());
+    EXPECT_EQ(v->pieces(i).end(), spt.pieces(i).end());
+  }
+
+  auto check_proto = [&v](const ImmutableSentencePieceText &s) {
+    int n = 0;
+    for (auto &p : s.pieces()) {
+      EXPECT_EQ(v->pieces(n).surface(), p.surface());
+      EXPECT_EQ(v->pieces(n).piece(), p.piece());
+      EXPECT_EQ(v->pieces(n).id(), p.id());
+      EXPECT_EQ(v->pieces(n).begin(), p.begin());
+      EXPECT_EQ(v->pieces(n).end(), p.end());
+      ++n;
+    }
+    EXPECT_EQ(v->text(), s.text());
+    EXPECT_EQ(v->score(), s.score());
+    EXPECT_EQ(v->SerializeAsString(), s.SerializeAsString());
+  };
+
+  // test copy.
+  const auto spt2 = spt;
+  check_proto(spt2);
+
+  // test assign.
+  const ImmutableSentencePieceText spt3(spt);
+  check_proto(spt3);
+
+  // default piece.
+  const ImmutableSentencePieceText_ImmutableSentencePiece piece;
+  EXPECT_TRUE(piece.surface().empty());
+  EXPECT_TRUE(piece.piece().empty());
+  EXPECT_EQ(piece.begin(), 0);
+  EXPECT_EQ(piece.end(), 0);
+  EXPECT_EQ(piece.id(), 0);
+}
+
+TEST(SentencePieceProcessorTest, ImmutableNBestSentencePieceTextTest) {
+  ImmutableNBestSentencePieceText spt;
+  EXPECT_EQ(spt.nbests_size(), 0);
+  EXPECT_TRUE(spt.SerializeAsString().empty());
+
+  auto *v = spt.mutable_proto();
+
+  for (int i = 0; i < 10; ++i) {
+    auto *p = v->add_nbests();
+    p->set_text(absl::StrCat("text_", i));
+    p->set_score(2.0 * i);
+  }
+
+  auto check_proto = [&v](const ImmutableNBestSentencePieceText &s) {
+    EXPECT_EQ(v->nbests_size(), s.nbests_size());
+    for (int i = 0; i < v->nbests_size(); ++i) {
+      EXPECT_EQ(v->nbests(i).text(), s.nbests(i).text());
+      EXPECT_EQ(v->nbests(i).score(), s.nbests(i).score());
+    }
+    EXPECT_EQ(v->SerializeAsString(), s.SerializeAsString());
+  };
+
+  check_proto(spt);
+
+  // test copy.
+  const auto spt2 = spt;
+  check_proto(spt2);
+
+  // test assign.
+  const ImmutableNBestSentencePieceText spt3(spt);
+  check_proto(spt3);
+}
+
+TEST(SentencePieceProcessorTest, ConvertToUnicodeSpansTest) {
+  auto make_spt = [&](const std::vector<std::string> &tokens) {
+    ImmutableSentencePieceText ispt;
+    auto *spt = ispt.mutable_proto();
+    int prev = 0;
+    std::string text;
+    for (const auto &tok : tokens) {
+      auto *piece = spt->add_pieces();
+      piece->set_surface(tok);
+      piece->set_piece(tok);
+      piece->set_begin(prev);
+      piece->set_end(prev + tok.size());
+      prev += tok.size();
+      text += tok;
+    }
+    spt->set_text(text);
+    ispt.ConvertToUnicodeSpans();
+    return ispt;
+  };
+
+  {
+    const auto spt = make_spt({"hello", "_world", "."});
+    EXPECT_EQ(spt.pieces_size(), 3);
+    EXPECT_EQ(spt.pieces(0).begin(), 0);
+    EXPECT_EQ(spt.pieces(0).end(), 5);
+    EXPECT_EQ(spt.pieces(1).begin(), 5);
+    EXPECT_EQ(spt.pieces(1).end(), 11);
+    EXPECT_EQ(spt.pieces(2).begin(), 11);
+    EXPECT_EQ(spt.pieces(2).end(), 12);
+  }
+
+  {
+    const auto spt = make_spt({"これは", "test", "です"});
+    EXPECT_EQ(spt.pieces_size(), 3);
+    EXPECT_EQ(spt.pieces(0).begin(), 0);
+    EXPECT_EQ(spt.pieces(0).end(), 3);
+    EXPECT_EQ(spt.pieces(1).begin(), 3);
+    EXPECT_EQ(spt.pieces(1).end(), 7);
+
+    EXPECT_EQ(spt.pieces(2).begin(), 7);
+    EXPECT_EQ(spt.pieces(2).end(), 9);
+  }
+
+  {
+    const auto spt = make_spt({"いABは", "にほCD", "へと"});
+    EXPECT_EQ(spt.pieces_size(), 3);
+    EXPECT_EQ(spt.pieces(0).begin(), 0);
+    EXPECT_EQ(spt.pieces(0).end(), 4);
+    EXPECT_EQ(spt.pieces(1).begin(), 4);
+    EXPECT_EQ(spt.pieces(1).end(), 8);
+    EXPECT_EQ(spt.pieces(2).begin(), 8);
+    EXPECT_EQ(spt.pieces(2).end(), 10);
+  }
+}
+
 }  // namespace sentencepiece
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer.h`

 * *Files 3% similar despite different names*

```diff
@@ -125,20 +125,20 @@
   GetPretokenizerForTraining();
 
   // Helper function to set `field_name=value` in `message`.
   // When `field_name` is repeated, multiple values can be passed
   // with comma-separated values. `field_name` must not be a nested message.
   // The body of these functions are automatically generated with
   // data/gen_spec_parser.pl
-  static util::Status SetProtoField(const std::string &name,
-                                    const std::string &value,
+  static util::Status SetProtoField(absl::string_view name,
+                                    absl::string_view value,
                                     TrainerSpec *message);
 
-  static util::Status SetProtoField(const std::string &name,
-                                    const std::string &value,
+  static util::Status SetProtoField(absl::string_view name,
+                                    absl::string_view value,
                                     NormalizerSpec *message);
 
   // Populates model type from string representation, e.g., "bpe".
   // Supported model: "unigram", "bpe", "word", "char".
   static util::Status PopulateModelTypeFromString(absl::string_view type,
                                                   TrainerSpec *trainer_spec);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/sentencepiece_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/sentencepiece_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/spec_parser.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spec_parser.h`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 #include "sentencepiece_processor.h"
 #include "third_party/absl/strings/ascii.h"
 #include "third_party/absl/strings/str_split.h"
 #include "util.h"
 
 namespace sentencepiece {
 
-#define PARSE_STRING(param_name)      \
-  if (name == #param_name) {          \
-    message->set_##param_name(value); \
-    return util::OkStatus();          \
+#define PARSE_STRING(param_name)                   \
+  if (name == #param_name) {                       \
+    message->set_##param_name(std::string(value)); \
+    return util::OkStatus();                       \
   }
 
 #define PARSE_REPEATED_STRING(param_name)                       \
   if (name == #param_name) {                                    \
     for (const std::string &val : util::StrSplitAsCSV(value)) { \
       message->add_##param_name(val);                           \
     }                                                           \
@@ -140,14 +140,15 @@
   PRINT_PARAM(num_threads);
   PRINT_PARAM(num_sub_iterations);
   PRINT_PARAM(max_sentencepiece_length);
   PRINT_PARAM(split_by_unicode_script);
   PRINT_PARAM(split_by_number);
   PRINT_PARAM(split_by_whitespace);
   PRINT_PARAM(split_digits);
+  PRINT_PARAM(pretokenization_delimiter);
   PRINT_PARAM(treat_whitespace_as_suffix);
   PRINT_PARAM(allow_whitespace_only_pieces);
   PRINT_REPEATED_STRING(control_symbols);
   PRINT_REPEATED_STRING(user_defined_symbols);
   PRINT_PARAM(required_chars);
   PRINT_PARAM(byte_fallback);
   PRINT_PARAM(vocabulary_output_piece_score);
@@ -159,14 +160,17 @@
   PRINT_PARAM(eos_id);
   PRINT_PARAM(pad_id);
   PRINT_PARAM(unk_piece);
   PRINT_PARAM(bos_piece);
   PRINT_PARAM(eos_piece);
   PRINT_PARAM(pad_piece);
   PRINT_PARAM(unk_surface);
+  PRINT_PARAM(enable_differential_privacy);
+  PRINT_PARAM(differential_privacy_noise_level);
+  PRINT_PARAM(differential_privacy_clipping_threshold);
 
   os << "}\n";
 
   return os.str();
 }
 
 inline std::string PrintProto(const NormalizerSpec &message,
@@ -182,16 +186,16 @@
   PRINT_PARAM(normalization_rule_tsv);
 
   os << "}\n";
 
   return os.str();
 }
 
-util::Status SentencePieceTrainer::SetProtoField(const std::string &name,
-                                                 const std::string &value,
+util::Status SentencePieceTrainer::SetProtoField(absl::string_view name,
+                                                 absl::string_view value,
                                                  TrainerSpec *message) {
   CHECK_OR_RETURN(message);
 
   PARSE_REPEATED_STRING(input);
   PARSE_STRING(input_format);
   PARSE_STRING(model_prefix);
 
@@ -215,14 +219,15 @@
   PARSE_INT32(num_threads);
   PARSE_INT32(num_sub_iterations);
   PARSE_INT32(max_sentencepiece_length);
   PARSE_BOOL(split_by_unicode_script);
   PARSE_BOOL(split_by_number);
   PARSE_BOOL(split_by_whitespace);
   PARSE_BOOL(split_digits);
+  PARSE_STRING(pretokenization_delimiter);
   PARSE_BOOL(treat_whitespace_as_suffix);
   PARSE_BOOL(allow_whitespace_only_pieces);
   PARSE_REPEATED_STRING(control_symbols);
   PARSE_REPEATED_STRING(user_defined_symbols);
   PARSE_STRING(required_chars);
   PARSE_BOOL(byte_fallback);
   PARSE_BOOL(hard_vocab_limit);
@@ -234,21 +239,24 @@
   PARSE_INT32(eos_id);
   PARSE_INT32(pad_id);
   PARSE_STRING(unk_piece);
   PARSE_STRING(bos_piece);
   PARSE_STRING(eos_piece);
   PARSE_STRING(pad_piece);
   PARSE_STRING(unk_surface);
+  PARSE_BOOL(enable_differential_privacy);
+  PARSE_DOUBLE(differential_privacy_noise_level);
+  PARSE_UINT64(differential_privacy_clipping_threshold);
 
   return util::StatusBuilder(util::StatusCode::kNotFound, GTL_LOC)
          << "unknown field name \"" << name << "\" in TrainerSpec.";
 }
 
-util::Status SentencePieceTrainer::SetProtoField(const std::string &name,
-                                                 const std::string &value,
+util::Status SentencePieceTrainer::SetProtoField(absl::string_view name,
+                                                 absl::string_view value,
                                                  NormalizerSpec *message) {
   CHECK_OR_RETURN(message);
 
   PARSE_STRING(name);
   PARSE_BYTE(precompiled_charsmap);
   PARSE_BOOL(add_dummy_prefix);
   PARSE_BOOL(remove_extra_whitespaces);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/spm_decode_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_decode_main.cc`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ABSL_FLAG(std::string, output, "", "output filename");
 ABSL_FLAG(std::string, input_format, "piece", "choose from piece or id");
 ABSL_FLAG(std::string, output_format, "string", "choose from string or proto");
 ABSL_FLAG(std::string, extra_options, "",
           "':' separated encoder extra options, e.g., \"reverse:bos:eos\"");
 
 int main(int argc, char *argv[]) {
+  sentencepiece::ScopedResourceDestructor cleaner;
   sentencepiece::ParseCommandLineFlags(argv[0], &argc, &argv, true);
   std::vector<std::string> rest_args;
 
   if (absl::GetFlag(FLAGS_input).empty()) {
     for (int i = 1; i < argc; ++i) {
       rest_args.push_back(std::string(argv[i]));
     }
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/spm_encode_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_encode_main.cc`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
           "tokens in \"vocabulary\" file");
 ABSL_FLAG(int32, vocabulary_threshold, 0,
           "Words with frequency < threshold will be treated as OOV");
 ABSL_FLAG(bool, generate_vocabulary, false,
           "Generates vocabulary file instead of segmentation");
 
 int main(int argc, char *argv[]) {
+  sentencepiece::ScopedResourceDestructor cleaner;
   sentencepiece::ParseCommandLineFlags(argv[0], &argc, &argv, true);
   std::vector<std::string> rest_args;
 
   if (absl::GetFlag(FLAGS_input).empty()) {
     for (int i = 1; i < argc; ++i) {
       rest_args.push_back(std::string(argv[i]));
     }
@@ -88,69 +89,69 @@
   std::vector<std::string> sps;
   std::vector<int> ids;
   std::vector<std::vector<std::string>> nbest_sps;
   std::vector<std::vector<int>> nbest_ids;
   absl::flat_hash_map<std::string, int> vocab;
   sentencepiece::SentencePieceText spt;
   sentencepiece::NBestSentencePieceText nbest_spt;
-  std::function<void(const std::string &line)> process;
+  std::function<void(absl::string_view line)> process;
 
   const int nbest_size = absl::GetFlag(FLAGS_nbest_size);
   const float alpha = absl::GetFlag(FLAGS_alpha);
 
   if (absl::GetFlag(FLAGS_generate_vocabulary)) {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.Encode(line, &spt));
       for (const auto &piece : spt.pieces()) {
         if (!sp.IsUnknown(piece.id()) && !sp.IsControl(piece.id()))
           vocab[piece.piece()]++;
       }
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "piece") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.Encode(line, &sps));
       output->WriteLine(absl::StrJoin(sps, " "));
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "id") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.Encode(line, &ids));
       output->WriteLine(absl::StrJoin(ids, " "));
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "proto") {
-    process = [&](const std::string &line) { CHECK_OK(sp.Encode(line, &spt)); };
+    process = [&](absl::string_view line) { CHECK_OK(sp.Encode(line, &spt)); };
   } else if (absl::GetFlag(FLAGS_output_format) == "sample_piece") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.SampleEncode(line, nbest_size, alpha, &sps));
       output->WriteLine(absl::StrJoin(sps, " "));
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "sample_id") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.SampleEncode(line, nbest_size, alpha, &ids));
       output->WriteLine(absl::StrJoin(ids, " "));
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "sample_proto") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.SampleEncode(line, nbest_size, alpha, &spt));
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "nbest_piece") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.NBestEncode(line, nbest_size, &nbest_sps));
       for (const auto &result : nbest_sps) {
         output->WriteLine(absl::StrJoin(result, " "));
       }
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "nbest_id") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.NBestEncode(line, nbest_size, &nbest_ids));
       for (const auto &result : nbest_ids) {
         output->WriteLine(absl::StrJoin(result, " "));
       }
     };
   } else if (absl::GetFlag(FLAGS_output_format) == "nbest_proto") {
-    process = [&](const std::string &line) {
+    process = [&](absl::string_view line) {
       CHECK_OK(sp.NBestEncode(line, nbest_size, &nbest_spt));
     };
   } else {
     LOG(FATAL) << "Unknown output format: "
                << absl::GetFlag(FLAGS_output_format);
   }
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/spm_export_vocab_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_export_vocab_main.cc`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-
-
 // Copyright 2016 Google Inc.
 //
 // Licensed under the Apache License, Version 2.0 (the "License");
 // you may not use this file except in compliance with the License.
 // You may obtain a copy of the License at
-// n//     http://www.apache.org/licenses/LICENSE-2.0
+//
+//     http://www.apache.org/licenses/LICENSE-2.0
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
@@ -25,14 +24,15 @@
 ABSL_FLAG(std::string, output, "", "Output filename");
 ABSL_FLAG(std::string, model, "", "input model file name");
 ABSL_FLAG(std::string, output_format, "vocab",
           "output format. choose from vocab or syms. vocab outputs pieces "
           "and scores, syms outputs pieces and indices.");
 
 int main(int argc, char *argv[]) {
+  sentencepiece::ScopedResourceDestructor cleaner;
   sentencepiece::ParseCommandLineFlags(argv[0], &argc, &argv, true);
 
   sentencepiece::SentencePieceProcessor sp;
   CHECK_OK(sp.Load(absl::GetFlag(FLAGS_model)));
 
   auto output =
       sentencepiece::filesystem::NewWritableFile(absl::GetFlag(FLAGS_output));
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/spm_normalize_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_normalize_main.cc`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 using sentencepiece::NormalizerSpec;
 using sentencepiece::SentencePieceProcessor;
 using sentencepiece::SentencePieceTrainer;
 using sentencepiece::normalizer::Builder;
 using sentencepiece::normalizer::Normalizer;
 
 int main(int argc, char *argv[]) {
+  sentencepiece::ScopedResourceDestructor cleaner;
   sentencepiece::ParseCommandLineFlags(argv[0], &argc, &argv, true);
   std::vector<std::string> rest_args;
 
   if (absl::GetFlag(FLAGS_input).empty()) {
     for (int i = 1; i < argc; ++i) {
       rest_args.push_back(std::string(argv[i]));
     }
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/spm_train_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/spm_train_main.cc`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
           "use Unicode script to split sentence pieces");
 ABSL_FLAG(bool, split_by_number, kDefaultTrainerSpec.split_by_number(),
           "split tokens by numbers (0-9)");
 ABSL_FLAG(bool, split_by_whitespace, kDefaultTrainerSpec.split_by_whitespace(),
           "use a white space to split sentence pieces");
 ABSL_FLAG(bool, split_digits, kDefaultTrainerSpec.split_digits(),
           "split all digits (0-9) into separate pieces");
+ABSL_FLAG(std::string, pretokenization_delimiter,
+          kDefaultTrainerSpec.pretokenization_delimiter(),
+          "specifies the delimiter of pre-tokenization");
 ABSL_FLAG(bool, treat_whitespace_as_suffix,
           kDefaultTrainerSpec.treat_whitespace_as_suffix(),
           "treat whitespace marker as suffix instead of prefix.");
 ABSL_FLAG(bool, allow_whitespace_only_pieces,
           kDefaultTrainerSpec.allow_whitespace_only_pieces(),
           "allow pieces that only contain (consecutive) whitespace tokens");
 ABSL_FLAG(std::string, control_symbols, "",
@@ -140,15 +143,28 @@
           "`unk_surface`.");
 ABSL_FLAG(bool, train_extremely_large_corpus,
           kDefaultTrainerSpec.train_extremely_large_corpus(),
           "Increase bit depth for unigram tokenization.");
 ABSL_FLAG(uint32, random_seed, static_cast<uint32>(-1),
           "Seed value for random generator.");
 
+// DP related.
+ABSL_FLAG(bool, enable_differential_privacy, false,
+          "Whether to add DP while training. Currently supported only by "
+          "UNIGRAM model.");
+
+ABSL_FLAG(float, differential_privacy_noise_level, 0.0f,
+          "Amount of noise to add for"
+          " DP");
+ABSL_FLAG(std::uint64_t, differential_privacy_clipping_threshold, 0,
+          "Threshold for"
+          " clipping the counts for DP");
+
 int main(int argc, char *argv[]) {
+  sentencepiece::ScopedResourceDestructor cleaner;
   sentencepiece::ParseCommandLineFlags(argv[0], &argc, &argv, true);
 
   sentencepiece::TrainerSpec trainer_spec;
   sentencepiece::NormalizerSpec normalizer_spec;
   NormalizerSpec denormalizer_spec;
 
   CHECK(!absl::GetFlag(FLAGS_input).empty());
@@ -210,14 +226,15 @@
   SetTrainerSpecFromFlag(num_sub_iterations);
   SetTrainerSpecFromFlag(max_sentencepiece_length);
   SetTrainerSpecFromFlag(max_sentence_length);
   SetTrainerSpecFromFlag(split_by_unicode_script);
   SetTrainerSpecFromFlag(split_by_whitespace);
   SetTrainerSpecFromFlag(split_by_number);
   SetTrainerSpecFromFlag(split_digits);
+  SetTrainerSpecFromFlag(pretokenization_delimiter);
   SetTrainerSpecFromFlag(byte_fallback);
   SetTrainerSpecFromFlag(treat_whitespace_as_suffix);
   SetTrainerSpecFromFlag(allow_whitespace_only_pieces);
   SetTrainerSpecFromFlag(hard_vocab_limit);
   SetTrainerSpecFromFlag(use_all_vocab);
   SetTrainerSpecFromFlag(unk_id);
   SetTrainerSpecFromFlag(bos_id);
@@ -231,14 +248,18 @@
   SetTrainerSpecFromFlag(required_chars);
   SetTrainerSpecFromFile(required_chars);
   SetTrainerSpecFromFlag(vocabulary_output_piece_score);
   SetRepeatedTrainerSpecFromFlag(accept_language);
   SetRepeatedTrainerSpecFromFlag(control_symbols);
   SetRepeatedTrainerSpecFromFlag(user_defined_symbols);
   SetTrainerSpecFromFlag(train_extremely_large_corpus);
+  // DP related.
+  SetTrainerSpecFromFlag(enable_differential_privacy);
+  SetTrainerSpecFromFlag(differential_privacy_noise_level);
+  SetTrainerSpecFromFlag(differential_privacy_clipping_threshold);
 
   SetRepeatedTrainerSpecFromFile(control_symbols);
   SetRepeatedTrainerSpecFromFile(user_defined_symbols);
 
   normalizer_spec.set_name(absl::GetFlag(FLAGS_normalization_rule_name));
   SetNormalizerSpecFromFlag(normalization_rule_tsv);
   SetNormalizerSpecFromFlag(add_dummy_prefix);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/test_main.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/test_main.cc`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 #else
 ABSL_FLAG(std::string, test_srcdir, "../data", "Data directory.");
 #endif
 
 ABSL_FLAG(std::string, test_tmpdir, "test_tmp", "Temporary directory.");
 
 int main(int argc, char **argv) {
+  sentencepiece::ScopedResourceDestructor cleaner;
   sentencepiece::ParseCommandLineFlags(argv[0], &argc, &argv, true);
   sentencepiece::test::RunAllTests();
   return 0;
 }
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/testharness.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/testharness.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/testharness.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/trainer_factory.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/trainer_factory.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/trainer_factory_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_factory_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/trainer_interface.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.cc`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "trainer_interface.h"
+
 #include <algorithm>
 #include <cstdlib>
 #include <memory>
 #include <set>
 #include <string>
 #include <utility>
 #include <vector>
@@ -24,20 +26,21 @@
 #include "model_factory.h"
 #include "model_interface.h"
 #include "normalizer.h"
 #include "sentencepiece_processor.h"
 #include "sentencepiece_trainer.h"
 #include "third_party/absl/container/flat_hash_map.h"
 #include "third_party/absl/memory/memory.h"
+#include "third_party/absl/random/distributions.h"
+#include "third_party/absl/random/random.h"
 #include "third_party/absl/strings/numbers.h"
 #include "third_party/absl/strings/str_cat.h"
 #include "third_party/absl/strings/str_format.h"
 #include "third_party/absl/strings/str_join.h"
 #include "third_party/absl/strings/str_split.h"
-#include "trainer_interface.h"
 #include "unicode_script.h"
 #include "util.h"
 
 namespace sentencepiece {
 
 const char32 TrainerInterface::kWSChar = L'\u2581';
 const char TrainerInterface::kWSStr[] = "\xe2\x96\x81";
@@ -74,17 +77,19 @@
                   trainer_spec.input_sentence_size() > 100);
 
   CHECK_OR_RETURN(!trainer_spec.unk_piece().empty());
   CHECK_OR_RETURN(!trainer_spec.bos_piece().empty());
   CHECK_OR_RETURN(!trainer_spec.eos_piece().empty());
   CHECK_OR_RETURN(!trainer_spec.pad_piece().empty());
 
-  if (SentencePieceTrainer::GetPretokenizerForTraining()) {
-    CHECK_EQ_OR_RETURN(TrainerSpec::UNIGRAM, trainer_spec.model_type())
-        << "PretokenizerForTraining is only supported in UNIGRAM mode.";
+  if (SentencePieceTrainer::GetPretokenizerForTraining() ||
+      !trainer_spec.pretokenization_delimiter().empty()) {
+    CHECK_OR_RETURN(trainer_spec.model_type() == TrainerSpec::UNIGRAM ||
+                    trainer_spec.model_type() == TrainerSpec::BPE)
+        << "PretokenizerForTraining is only supported in UNIGRAM or BPE mode.";
   }
 
   return util::OkStatus();
 }
 
 bool is_unicode_decimal_number(char32 c) {
   return (c >= 0x30 && c <= 0x39) || (c >= 0xff10 && c <= 0xff19);
@@ -223,15 +228,14 @@
     const char32 c = sentencepiece[pos];
     if (c == kUNKChar) {  // UNK must not be included
       return false;
     }
     if (c == 0x0000) {  // NULL is not allowed for Darts (TRIE).
       return false;
     }
-    // kUPPBoundaryChar is included when split_by_upp_for_training is true.
     if (c == kUPPBoundaryChar) {
       return false;
     }
     if (c == 0x0020) {
       LOG(WARNING) << "space must not be included in normalized string.";
       return false;
     }
@@ -269,14 +273,16 @@
     } else {
       auto s = unicode_script::GetScript(c);
 
       // Merge Hiragana/Katakana into Han.
       if (s == unicode_script::U_Hiragana || s == unicode_script::U_Katakana ||
           c == 0x30FC) {  // long vowel sound (Katakana) should be Katakana
         s = unicode_script::U_Han;
+      } else if (s == unicode_script::U_Inherited) {
+        s = prev_script;
       }
 
       if (!trainer_spec_.split_by_number() && is_unicode_decimal_number(c)) {
         s = kAnyType;
       }
 
       if (trainer_spec_.split_digits() && is_unicode_decimal_number(c)) {
@@ -292,14 +298,30 @@
 
       prev_script = s;
     }
   }
   return true;
 }
 
+template <typename T>
+void AddDPNoise(const TrainerSpec &trainer_spec, absl::SharedBitGen &generator,
+                T *to_update) {
+  if (trainer_spec.differential_privacy_noise_level() > 0) {
+    float random_num = absl::Gaussian<float>(
+        generator, 0, trainer_spec.differential_privacy_noise_level());
+
+    *to_update =
+        std::round(std::max(0.f, random_num + static_cast<float>(*to_update)));
+  }
+  // Clip anything below the clipping threshold to 0.
+  if (*to_update < trainer_spec.differential_privacy_clipping_threshold()) {
+    *to_update = 0;
+  }
+}
+
 util::Status TrainerInterface::LoadSentences() {
   RETURN_IF_ERROR(status());
   CHECK_OR_RETURN(sentences_.empty());
   CHECK_OR_RETURN(required_chars_.empty());
   CHECK_OR_RETURN(trainer_spec_.input_format().empty() ||
                   trainer_spec_.input_format() == "text" ||
                   trainer_spec_.input_format() == "tsv")
@@ -383,14 +405,15 @@
 
   if (sentences_.size() == selector.total_size()) {
     LOG(INFO) << "Loaded all " << sentences_.size() << " sentences";
   } else {
     LOG(INFO) << "Sampled " << sentences_.size() << " sentences from "
               << selector.total_size() << " sentences.";
   }
+
   if (too_long_lines > 0)
     LOG(INFO) << "Skipped " << too_long_lines << " too long sentences.";
   if (self_test_samples_.size() > 0)
     LOG(INFO) << "Loaded " << self_test_samples_.size() << " test sentences";
 
   // Normalize and removes empty string.
   {
@@ -426,14 +449,62 @@
       if (s->empty()) {
         std::swap(sentences_[i], sentences_[sentences_.size() - 1]);
         sentences_.resize(sentences_.size() - 1);
       }
     }
   }
 
+  // If DP is required, add the noise/clip the input.
+  if (trainer_spec_.enable_differential_privacy()) {
+    if (trainer_spec_.input_format() != "tsv") {
+      LOG(ERROR)
+          << "Dp version will not work correctly with text input format.";
+    }
+    if (trainer_spec_.differential_privacy_noise_level() <= 0) {
+      LOG(WARNING) << "Private version with <=0 noise level will give "
+                      "infinity epsilon guarantees.";
+    }
+    if (trainer_spec_.differential_privacy_clipping_threshold() <= 0) {
+      LOG(WARNING) << "Private version with <=0 clipping threshold will give "
+                      "infinity epsilon guarantees.";
+    }
+
+    // Add noise to all the sentences via threadpool.
+
+    // This line is mainly for tests with small num of sentences.
+    const auto num_workers =
+        std::min<uint64>(trainer_spec_.num_threads(), sentences_.size() - 1);
+
+    {
+      auto pool = absl::make_unique<ThreadPool>(num_workers);
+      pool->StartWorkers();
+      for (int n = 0; n < num_workers; ++n) {
+        pool->Schedule([&, n]() {
+          // One per thread generator.
+          absl::SharedBitGen generator;
+          for (size_t i = n; i < sentences_.size(); i += num_workers) {
+            AddDPNoise<int64>(trainer_spec_, generator,
+                              &(sentences_[i].second));
+          }
+        });
+      }
+    }
+
+    // Remove zero freq elements.
+    const auto before_size = sentences_.size();
+    auto it = std::remove_if(sentences_.begin(), sentences_.end(),
+                             [](const Sentence &s) { return s.second <= 0; });
+    const auto new_size = std::distance(sentences_.begin(), it);
+    const int num_erased = before_size - new_size;
+    sentences_.erase(it, sentences_.end());
+
+    LOG(INFO) << "DP noise resulted in " << 1.0 * num_erased / before_size
+              << " fraction of sentences removed.";
+  }
+
   // Count character frequencies.
   int64 all_chars_count = 0;
   // A map from a character to {is_required_char, character count}.
   absl::flat_hash_map<char32, std::pair<bool, int64>> chars_count;
   for (const char32 c :
        string_util::UTF8ToUnicodeText(trainer_spec_.required_chars())) {
     CHECK_OR_RETURN(string_util::IsValidCodepoint(c));
@@ -610,14 +681,15 @@
 
   return util::OkStatus();
 }
 
 util::Status TrainerInterface::SaveModel(absl::string_view filename) const {
   LOG(INFO) << "Saving model: " << filename;
   ModelProto model_proto;
+
   RETURN_IF_ERROR(Serialize(&model_proto));
 
   auto output = filesystem::NewWritableFile(filename.data(), true);
   RETURN_IF_ERROR(output->status());
   output->Write(model_proto.SerializeAsString());
   return util::OkStatus();
 }
@@ -625,14 +697,22 @@
 util::Status TrainerInterface::SaveVocab(absl::string_view filename) const {
   LOG(INFO) << "Saving vocabs: " << filename;
   ModelProto model_proto;
   RETURN_IF_ERROR(Serialize(&model_proto));
   auto output = filesystem::NewWritableFile(filename);
   RETURN_IF_ERROR(output->status());
 
+  for (const auto &piece : model_proto.pieces()) {
+    if (piece.piece().find_first_of(" \t\r\n") != std::string::npos) {
+      LOG(WARNING) << "The piece [" << piece.piece()
+                   << "] contains escaped characters that break the format of "
+                   << filename;
+    }
+  }
+
   if (trainer_spec_.vocabulary_output_piece_score()) {
     for (const auto &piece : model_proto.pieces()) {
       std::ostringstream os;
       os << piece.piece() << "\t" << piece.score();
       CHECK_OR_RETURN(output->WriteLine(os.str()));
     }
   } else {
@@ -677,54 +757,55 @@
   CHECK_OR_RETURN(insert_id(trainer_spec_.pad_id(), trainer_spec_.pad_piece()));
 
   CHECK_OR_RETURN(has_unk) << trainer_spec_.unk_piece() << " must be defined.";
 
   std::set<std::string> dup;
 
   int id = 0;
-  auto insert_meta_symbol = [&id, &dup, this](
-                                const std::string &w,
-                                ModelProto::SentencePiece::Type type) -> bool {
+  auto insert_meta_symbol =
+      [&id, &dup, this](const std::string &w,
+                        ModelProto::SentencePiece::Type type) -> util::Status {
     if (!dup.insert(w).second) {
-      LOG(ERROR) << w << " is already defined.";
-      return false;
+      return util::InternalError(absl::StrCat(
+          w, " is already defined. duplicated symbols are not allowed."));
     }
 
     if (w == trainer_spec_.unk_piece()) {
-      LOG(ERROR) << trainer_spec_.unk_piece()
-                 << " must not be defined with --control_symbols and "
-                    "--user_defined_symbols.";
-      return false;
+      return util::InternalError(
+          absl::StrCat(trainer_spec_.unk_piece(),
+                       " must not be defined with --control_symbols and "
+                       "--user_defined_symbols."));
     }
 
     if (w == trainer_spec_.bos_piece() && trainer_spec_.bos_id() >= 0) {
       meta_pieces_[trainer_spec_.bos_id()].second = type;
     } else if (w == trainer_spec_.eos_piece() && trainer_spec_.eos_id() >= 0) {
       meta_pieces_[trainer_spec_.eos_id()].second = type;
     } else if (w == trainer_spec_.pad_piece() && trainer_spec_.pad_id() >= 0) {
       meta_pieces_[trainer_spec_.pad_id()].second = type;
     } else {
       while (meta_pieces_.find(id) != meta_pieces_.end()) ++id;
       meta_pieces_[id] = std::make_pair(w, type);
     }
-    return true;
+
+    return util::OkStatus();
   };
 
   for (const auto &w : trainer_spec_.control_symbols()) {
-    CHECK_OR_RETURN(insert_meta_symbol(w, ModelProto::SentencePiece::CONTROL));
+    RETURN_IF_ERROR(insert_meta_symbol(w, ModelProto::SentencePiece::CONTROL));
   }
 
   for (const auto &w : trainer_spec_.user_defined_symbols()) {
-    CHECK_OR_RETURN(
+    RETURN_IF_ERROR(
         insert_meta_symbol(w, ModelProto::SentencePiece::USER_DEFINED));
   }
 
   if (trainer_spec_.byte_fallback()) {
     for (int i = 0; i < 256; ++i) {
-      CHECK_OR_RETURN(
+      RETURN_IF_ERROR(
           insert_meta_symbol(ByteToPiece(i), ModelProto::SentencePiece::BYTE));
     }
   }
 
   return util::OkStatus();
 }
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/trainer_interface.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface.h`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -103,24 +103,24 @@
 
   FRIEND_TEST(TrainerInterfaceTest, IsValidSentencePieceTest);
   FRIEND_TEST(TrainerInterfaceTest, OverrideSpecialPiecesTest);
   FRIEND_TEST(TrainerInterfaceTest, BytePiecesTest);
   FRIEND_TEST(TrainerInterfaceTest, SerializeTest);
   FRIEND_TEST(TrainerInterfaceTest, CharactersTest);
 
+  // Loads all sentences from spec.input() or SentenceIterator.
+  // It loads at most input_sentence_size sentences.
+  util::Status LoadSentences();
+
  protected:
   // Returns true if |piece| is valid sentence piece.
   // The result is affected by
   // max_sentencepiece_length, split_by_whiespace, split_by_unicode_script.
   bool IsValidSentencePiece(const string_util::UnicodeText &piece) const;
 
-  // Loads all sentences from spec.input() or SentenceIterator.
-  // It loads at most input_sentence_size sentences.
-  util::Status LoadSentences();
-
   // Splits all sentencecs by whitespaces and
   // replace the |sentences_| with tokenized string.
   // e.g.,
   //  [ ["hello world ", 1], ["hi world]" ] =>
   //  [ ["hello", 1], ["hi", 1], ["world", 2] ]
   void SplitSentencesByWhitespace();
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/trainer_interface_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/trainer_interface_test.cc`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "trainer_interface.h"
+
 #include <utility>
 
 #include "filesystem.h"
 #include "testharness.h"
 #include "third_party/absl/strings/str_cat.h"
 #include "third_party/absl/strings/str_format.h"
-#include "trainer_interface.h"
 #include "util.h"
 
 namespace sentencepiece {
 
 // Space symbol
 #define WS "\xe2\x96\x81"
 
@@ -68,20 +69,24 @@
   EXPECT_TRUE(IsValid("あいう"));
   EXPECT_TRUE(IsValid("グーグル"));  // "ー" is a part of Katakana
   EXPECT_TRUE(IsValid("食べる"));
   EXPECT_FALSE(IsValid("漢字ABC"));  // mixed CJK scripts
   EXPECT_FALSE(IsValid("F1"));
   EXPECT_FALSE(IsValid("1F"));
   EXPECT_FALSE(IsValid("1A2"));
-  EXPECT_TRUE(IsValid("$10"));  // $ and 1 are both "common" script.
+  EXPECT_TRUE(IsValid("$10"));      // $ and 1 are both "common" script.
   EXPECT_FALSE(IsValid("$ABC"));
   EXPECT_FALSE(IsValid("ab\tbc"));  // "\t" is UPP boundary.
   EXPECT_FALSE(IsValid("ab cd"));
   EXPECT_FALSE(IsValid("\0\0"));
   EXPECT_FALSE(IsValid("\0"));
+  EXPECT_TRUE(IsValid("proteïni"));  // Combining Diaeresis should inherit
+                                     // script from base character.
+  EXPECT_TRUE(IsValid("ثَبَّتَ"));  // Arabic Fatha and Shadda should inherit script
+                                // from base character.
 
   trainer_spec.set_split_by_whitespace(false);
   EXPECT_TRUE(IsValid(WS));
   EXPECT_TRUE(IsValid(WS WS WS "a"));
   EXPECT_TRUE(IsValid(WS "a"));
   EXPECT_FALSE(IsValid("a" WS));
   EXPECT_FALSE(IsValid(WS "a" WS));
@@ -105,14 +110,34 @@
   EXPECT_TRUE(IsValid("グーグル"));
   EXPECT_TRUE(IsValid("食べる"));
   EXPECT_TRUE(IsValid("漢字ABC"));
   EXPECT_TRUE(IsValid("F1"));
   EXPECT_TRUE(IsValid("$10"));
   EXPECT_TRUE(IsValid("$ABC"));
 
+  trainer_spec.set_split_by_unicode_script(true);
+  trainer_spec.set_split_by_number(true);
+  EXPECT_FALSE(IsValid("F1"));
+  EXPECT_TRUE(IsValid("$10"));
+
+  trainer_spec.set_split_by_unicode_script(true);
+  trainer_spec.set_split_by_number(false);
+  EXPECT_TRUE(IsValid("F1"));
+  EXPECT_TRUE(IsValid("$10"));
+
+  trainer_spec.set_split_by_unicode_script(false);
+  trainer_spec.set_split_by_number(true);
+  EXPECT_TRUE(IsValid("F1"));
+  EXPECT_TRUE(IsValid("$10"));
+
+  trainer_spec.set_split_by_unicode_script(false);
+  trainer_spec.set_split_by_number(false);
+  EXPECT_TRUE(IsValid("F1"));
+  EXPECT_TRUE(IsValid("$10"));
+
   trainer_spec.set_max_sentencepiece_length(4);
   EXPECT_TRUE(IsValid("1234"));
   EXPECT_FALSE(IsValid("12345"));
 
   trainer_spec.set_max_sentencepiece_length(10);
   trainer_spec.set_split_by_unicode_script(true);
   trainer_spec.set_split_by_number(false);
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unicode_script.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unicode_script.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script.h`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #ifndef UNICODE_SCRIPT_H_
 #define UNICODE_SCRIPT_H_
 
 #include "common.h"
 
 namespace sentencepiece {
 namespace unicode_script {
-enum ScriptType {
+enum ScriptType : int32_t {
   U_Adlam,
   U_Ahom,
   U_Anatolian_Hieroglyphs,
   U_Arabic,
   U_Armenian,
   U_Avestan,
   U_Balinese,
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unicode_script_map.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unicode_script_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unicode_script_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unigram_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.cc`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
+#include "unigram_model.h"
+
 #include <algorithm>
 #include <cfloat>
 #include <cmath>
 #include <complex>
 #include <map>
 #include <queue>
 #include <string>
 #include <utility>
 #include <vector>
 
+#include "third_party/absl/container/flat_hash_map.h"
 #include "third_party/absl/memory/memory.h"
 #include "third_party/absl/strings/str_split.h"
 #include "third_party/absl/strings/string_view.h"
-#include "unigram_model.h"
 #include "util.h"
 
 namespace sentencepiece {
 namespace unigram {
 namespace {
 
 // Size of nodes pre-allocated in Lattice.
@@ -192,32 +194,33 @@
   std::reverse(results.begin(), results.end());
 
   LatticePathWithScore retval = {results, score};
 
   return retval;
 }
 
-std::vector<float> Lattice::ForwardAlgorithm(float theta) const {
+std::vector<float> Lattice::ForwardAlgorithm(float inv_theta) const {
   const int len = size();
   std::vector<float> alpha(node_allocator_.size(), 0.0);
 
   for (int pos = 0; pos <= len; ++pos) {
     for (Node *rnode : begin_nodes_[pos]) {
       for (Node *lnode : end_nodes_[pos]) {
-        alpha[rnode->node_id] = LogSumExp(
-            alpha[rnode->node_id], theta * lnode->score + alpha[lnode->node_id],
-            lnode == end_nodes_[pos][0]);
+        alpha[rnode->node_id] =
+            LogSumExp(alpha[rnode->node_id],
+                      inv_theta * lnode->score + alpha[lnode->node_id],
+                      lnode == end_nodes_[pos][0]);
       }
     }
   }
 
   return alpha;
 }
 
-std::vector<float> Lattice::BackwardAlgorithm(float theta) const {
+std::vector<float> Lattice::BackwardAlgorithm(float inv_theta) const {
   const int len = size();
   std::vector<float> beta(node_allocator_.size(), 0.0);
 
   for (int pos = len; pos >= 0; --pos) {
     for (Node *lnode : end_nodes_[pos]) {
       for (Node *rnode : begin_nodes_[pos]) {
         beta[lnode->node_id] =
@@ -254,48 +257,99 @@
       }
     }
   }
 
   return freq * Z;
 }
 
-float Lattice::CalculateEntropy(float theta) const {
+float Lattice::CalculateEntropy(float inv_theta) const {
   const int len = size();
 
   // alpha[node_id] is the marginal prob of sequence up to start of node
   // H is entropy of sequence
   // the index of alpha/H is Node::node_id.
-  std::vector<float> alpha(node_allocator_.size(), 0.0);
   std::vector<float> H(node_allocator_.size(), 0.0);
 
   // Populate the forward marginals to get the normalising constant
-  alpha = ForwardAlgorithm(theta);
+  const auto alpha = ForwardAlgorithm(inv_theta);
 
   // Now populate the forward entropies
   for (int pos = 0; pos <= len; ++pos) {
     for (Node *rnode : begin_nodes_[pos]) {
       for (Node *lnode : end_nodes_[pos]) {
         // Contribution each lnode makes = p(lnode) * (H(lnode) + log p(lnode))
 
         // We have to normalise p(lnode) by the marginal contribution it makes
         const float lnode_transition_prob =
-            ((theta * lnode->score) + alpha[lnode->node_id] -
+            ((inv_theta * lnode->score) + alpha[lnode->node_id] -
              alpha[rnode->node_id]);
         H[rnode->node_id] += std::exp(lnode_transition_prob) *
                              (H[lnode->node_id] + lnode_transition_prob);
       }
     }
   }
 
   return -H[begin_nodes_[len][0]->node_id];
 }
 
+namespace {
+
+// The node structure to support A* algorithm in Lattice::NBest()
+struct Hypothesis {
+  Lattice::Node *node;
+  Hypothesis *next;
+  float fx;  // the priority to pop a new hypothesis from the priority queue.
+  float gx;  // the sum of scores from EOS to the left-most node in x.
+};
+
+// Helper function for cloning a Hypothesis and the ones on their next paths.
+// The graph structure is preserved.
+//
+//   to_clone:  the Hypothesis to clone.
+//   clone_map: mapping between the old pointers and the new pointers.
+//   allocator: allocate and own the cloned Hypothesis.
+//
+// Returns the cloned Hypothesis*. All Hypothesis on its "next" chain are also
+// guaranteed to have been allocated via "allocator", and "clone_map" is updated
+// with all new mappings.
+Hypothesis *CloneHypAndDependents(
+    const Hypothesis *to_clone,
+    absl::flat_hash_map<const Hypothesis *, Hypothesis *> *clone_map,
+    model::FreeList<Hypothesis> *allocator) {
+  Hypothesis *cloned = nullptr;
+  Hypothesis **result_callback = &cloned;
+
+  // Iteratively clone "to_clone" and its dependencies.
+  // The new pointer will be written back to *result_callback.
+  while (to_clone != nullptr) {
+    // If "to_clone" has already been cloned before, we just look up the result.
+    auto iter = clone_map->find(to_clone);
+    if (iter != clone_map->end()) {
+      *result_callback = iter->second;
+      break;
+    }
+
+    // Allocate a new Hypothesis and copy the values.
+    Hypothesis *new_hyp = allocator->Allocate();
+    *new_hyp = *to_clone;
+    *result_callback = new_hyp;
+    clone_map->insert({to_clone, new_hyp});
+
+    // Move on to clone "to_clone->next".
+    to_clone = to_clone->next;
+    result_callback = &(new_hyp->next);
+  }
+  return cloned;
+}
+
+}  // namespace
+
 std::vector<Lattice::LatticePathWithScore> Lattice::NBest(size_t nbest_size,
                                                           bool sample,
-                                                          float theta) {
+                                                          float inv_theta) {
   if (nbest_size < 1) {
     LOG(WARNING) << "nbest_size >= 1. Returns empty result.";
     return {};
   }
 
   if (nbest_size == 1 && !sample) {
     return {Viterbi()};
@@ -308,20 +362,14 @@
   // g(x): the sum of scores from  EOS to the left-most node in x.
   //       for a complete hypothesis, g(hyp) is the score of the hypothesis.
   // h(x): a heuristic that estimates the largest score from x to BOS.
   // f(x): the priority to pop a new hypothesis from the priority queue.
   //
   // As left-to-right Viterbi search can tell the *exact* value of h(x),
   // we can obtain the exact n-best results with A*.
-  struct Hypothesis {
-    Node *node;
-    Hypothesis *next;
-    float fx;
-    float gx;
-  };
 
   class HypothesisComparator {
    public:
     const bool operator()(Hypothesis *h1, Hypothesis *h2) {
       return (h1->fx < h2->fx);
     }
   };
@@ -339,24 +387,26 @@
   eos->next = nullptr;
   eos->gx = 0.0;
 
   std::vector<float> alpha(node_allocator_.size(), 0.0);
 
   if (sample) {
     // Run forwards algorithm to get normalising constants
-    alpha = ForwardAlgorithm(theta);
+    alpha = ForwardAlgorithm(inv_theta);
     // f(eos) = Gumbel(0), as it is the perturbed score of the entire lattice.
     eos->fx = Gumbel();
   } else {
     // Run Viterbi first to fill backtrace score.
     Viterbi();
     eos->fx = eos->node->backtrace_score;
   }
   agenda.push(eos);
 
+  int shrink_count = 0;  // Number of times agenda has shrunk. For logging only.
+  bool printed_memory_warning = false;  // For logging only.
   while (!agenda.empty()) {
     auto *top = agenda.top();
     agenda.pop();
     auto *node = top->node;
 
     // Reaches to BOS
     if (node == bos_node()) {
@@ -378,15 +428,16 @@
     const float Z = alpha[node->node_id];
     if (sample) {
       float max_score = -1e8;
       // Calculate the marginal and perturbed scores for stochastic search
       for (int i = 0; i < end_nodes(node->pos).size(); i++) {
         Node *lnode = end_nodes(node->pos)[i];
         // Calculate backwards transition score
-        probs[i] = top->gx + alpha[lnode->node_id] + (theta * lnode->score) - Z;
+        probs[i] =
+            top->gx + alpha[lnode->node_id] + (inv_theta * lnode->score) - Z;
         perturbed_probs[i] = probs[i] + Gumbel();
         if (perturbed_probs[i] > max_score) {
           max_score = perturbed_probs[i];
         }
       }
       // Now constrain the sampled continuations to match the score of parent
       for (int i = 0; i < adjusted_probs.size(); i++) {
@@ -406,61 +457,82 @@
       hyp->node = lnode;
       if (sample) {
         hyp->gx = probs[i];
         hyp->fx = adjusted_probs[i];
       } else {
         hyp->gx = lnode->score + top->gx;  // just adds node->score
         hyp->fx =
-            lnode->backtrace_score + top->gx;  // backtrace_score is h(node).
+            lnode->backtrace_score + hyp->gx;  // backtrace_score is h(node).
       }
       hyp->next = top;
       agenda.push(hyp);
     }
 
+    static constexpr int kOneBillion = 1000000000;  // 10^9.
+    if (hypothesis_allocator.size() >= kOneBillion) {
+      if (!printed_memory_warning) {
+        printed_memory_warning = true;
+        LOG(WARNING) << "Allocator size exceeds " << kOneBillion
+                     << " with an example of length " << this->size();
+      }
+    }
+
     // When the input is too long or contains duplicated phrases,
     // `agenda` will get extremely big. Here we avoid this case by
     // dynamically shrinking the agenda.
-    constexpr int kMaxAgendaSize = 100000;
+    constexpr int kMaxAgendaSize = 10000;
     constexpr int kMinAgendaSize = 512;
     if (agenda.size() >= kMaxAgendaSize) {
-      LOG(WARNING) << "Too big agenda. shrinking";
       // Keeps the top `kMinAgendaSize` hypothesis.
       Agenda new_agenda;
+      // Keeps the top hypothesis and the ones on their "next" paths.
+      model::FreeList<Hypothesis> new_allocator(kPreallocatedHypothesisSize);
+      // Map between old Hypothesis* and new Hypothesis*.
+      absl::flat_hash_map<const Hypothesis *, Hypothesis *> clone_map;
+
       const int size = std::min<int>(kMinAgendaSize, nbest_size * 10);
+      shrink_count++;
+      LOG(WARNING) << "Too big agenda size " << agenda.size()
+                   << ". Shrinking (round " << shrink_count << ") down to "
+                   << size << ".";
       for (int i = 0; i < size; ++i) {
-        new_agenda.push(agenda.top());
+        const Hypothesis *top_hyp = agenda.top();
+        Hypothesis *cloned_hyp =
+            CloneHypAndDependents(top_hyp, &clone_map, &new_allocator);
+        new_agenda.push(cloned_hyp);
         agenda.pop();
       }
       agenda = std::move(new_agenda);
+      hypothesis_allocator.swap(new_allocator);
     }
   }
 
   return results;
 }
 
-std::vector<Lattice::Node *> Lattice::Sample(float theta) {
+std::vector<Lattice::Node *> Lattice::Sample(float inv_theta) {
   const int len = size();
   if (len == 0) return {};
 
   std::vector<float> alpha(node_allocator_.size(), 0.0);
 
-  alpha = ForwardAlgorithm(theta);
+  alpha = ForwardAlgorithm(inv_theta);
 
   auto *mt = random::GetRandomGenerator();
 
   std::vector<Node *> results;
   std::vector<float> probs;
 
   float Z = alpha[eos_node()->node_id];
   Node *node = eos_node();
   while (true) {
     probs.clear();
     for (const Node *lnode : end_nodes_[node->pos]) {
-      probs.push_back(std::exp(static_cast<double>(alpha[lnode->node_id] +
-                                                   theta * lnode->score - Z)));
+      probs.push_back(std::exp(static_cast<double>(
+          alpha[lnode->node_id] + inv_theta * lnode->score - Z)));
     }
     std::discrete_distribution<int> dist(probs.begin(), probs.end());
     node = end_nodes_[node->pos][dist(*mt)];
     if (node == bos_node()) break;
 
     Z = alpha[node->node_id];
     results.push_back(node);
@@ -625,14 +697,18 @@
                                      int nbest_size) const {
   if (!status().ok() || normalized.empty()) {
     return {{{}, 0.0}};
   }
 
   nbest_size = std::max<int>(1, std::min<int>(nbest_size, 1024));
 
+  if (nbest_size <= 1) {
+    return {std::pair<EncodeResult, float>(Encode(normalized), 0.0)};
+  }
+
   Lattice lattice;
   lattice.SetSentence(normalized);
   PopulateNodes(&lattice);
 
   NBestEncodeResult nbest_results;
   for (const auto &nbest : lattice.NBest(nbest_size, false, 0.0)) {
     EncodeResult results;
@@ -642,81 +718,79 @@
     nbest_results.emplace_back(results, nbest.second);
   }
 
   return nbest_results;
 }
 
 EncodeResult Model::SampleEncode(absl::string_view normalized,
-                                 float theta) const {
+                                 float inv_theta) const {
   if (!status().ok() || normalized.empty()) {
     return {};
   }
 
   Lattice lattice;
   lattice.SetSentence(normalized);
   PopulateNodes(&lattice);
 
   EncodeResult results;
-  for (const auto *node : lattice.Sample(theta)) {
+  for (const auto *node : lattice.Sample(inv_theta)) {
     results.emplace_back(node->piece, node->id);
   }
 
   return results;
 }
 
 NBestEncodeResult Model::SampleEncodeAndScore(absl::string_view normalized,
-                                              float theta, int samples,
+                                              float inv_theta, int samples,
                                               bool wor,
                                               bool include_best) const {
   if (!status().ok() || normalized.empty()) {
     return {};
   }
   NBestEncodeResult results;
   Lattice lattice;
   lattice.SetSentence(normalized);
   PopulateNodes(&lattice);
 
-  std::vector<float> alpha = lattice.ForwardAlgorithm(theta);
-  float marginal = alpha[lattice.eos_node()->node_id];
+  const std::vector<float> alpha = lattice.ForwardAlgorithm(inv_theta);
+  const float marginal = alpha[lattice.eos_node()->node_id];
 
   if (include_best) {
     if (!wor) {
-      LOG(FATAL) << "include_best not supported for wor false";
+      LOG(ERROR) << "include_best not supported for wor false";
+      return {};
     }
     EncodeResult result;
-    Lattice::LatticePathWithScore best_path = lattice.Viterbi();
-
+    const auto best_path = lattice.Viterbi();
     for (const auto *node : best_path.first) {
       result.emplace_back(node->piece, node->id);
     }
 
     // Inclusion probability if we always include the best is 1.
     results.emplace_back(result, 0.0);
   }
 
   if (wor) {
     // Draw k+1 samples as we need perturbed score of k+1th element
-    std::vector<Lattice::LatticePathWithScore> nbest_samples =
-        lattice.NBest(samples + 1, true, theta);
+    auto nbest_samples = lattice.NBest(samples + 1, true, inv_theta);
 
     if (include_best) {
       std::vector<std::vector<Lattice::Node *>> nbest_paths(
           nbest_samples.size());
       for (int i = 0; i < nbest_samples.size(); i++) {
         nbest_paths[i] = nbest_samples[i].first;
       }
       // Remove the best result from the samples if necessary
-      Lattice::LatticePathWithScore best_path = lattice.Viterbi();
+      const auto best_path = lattice.Viterbi();
 
       const int index_of_best =
           (std::find(nbest_paths.begin(), nbest_paths.end(), best_path.first) -
            nbest_paths.begin());
 
       if (index_of_best != nbest_samples.size()) {
-        LOG(INFO) << "removing best path from samples";
         nbest_samples.erase(nbest_samples.begin() + index_of_best);
       } else {
         nbest_samples.pop_back();
       }
     }
     // We use the perturbed score of the k+1th element to calculate the
     // inclusion probability.
@@ -724,27 +798,27 @@
     // Discard the last sample
     nbest_samples.pop_back();
     for (const auto &nbest : nbest_samples) {
       EncodeResult result;
       float score = 0.0;
 
       for (const auto *node : nbest.first) {
-        score += (theta * node->score);
+        score += (inv_theta * node->score);
         result.emplace_back(node->piece, node->id);
       }
 
       results.emplace_back(result, score - marginal);
     }
 
     // Now calculate the inclusion probability
     for (auto &it : results) {
       // Only modify non best sample inclusion probabilities.
       if (it.second != 0.0) {
-        double x = it.second - kappa;
-        double y = std::exp(x);
+        const double x = it.second - kappa;
+        const double y = std::exp(x);
         double inclusion_prob;
         if (x <= -10) {
           // Series expansion of the log Gumbel survival function up to eps.
           inclusion_prob =
               x - (y / 2) + (std::pow(y, 2) / 24) - std::pow(y, 4) / 2880;
         } else {
           inclusion_prob = std::log(-std::expm1(-y));
@@ -756,32 +830,33 @@
     while (results.size() < samples) {
       Lattice lattice;
       lattice.SetSentence(normalized);
       PopulateNodes(&lattice);
 
       float score = 0.0;
       EncodeResult result;
-      std::vector<Lattice::Node *> sample = lattice.Sample(theta);
+      const std::vector<Lattice::Node *> sample = lattice.Sample(inv_theta);
       for (const auto *node : sample) {
         result.emplace_back(node->piece, node->id);
-        score += (theta * node->score);
+        score += (inv_theta * node->score);
       }
       results.emplace_back(result, score - marginal);
     }
   }
 
   return results;
 }
 
-float Model::CalculateEntropy(absl::string_view normalized, float theta) const {
+float Model::CalculateEntropy(absl::string_view normalized,
+                              float inv_theta) const {
   Lattice lattice;
   lattice.SetSentence(normalized);
   PopulateNodes(&lattice);
 
-  return lattice.CalculateEntropy(theta);
+  return lattice.CalculateEntropy(inv_theta);
 }
 
 bool Model::VerifyOutputsEquivalent(absl::string_view expected,
                                     absl::string_view actual) const {
   auto compute_unigram_model_score =
       [this](std::vector<absl::string_view> output_pieces) {
         float total_score = 0;
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unigram_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model.h`

 * *Files 5% similar despite different names*

```diff
@@ -169,14 +169,26 @@
   // Returns a vocab id of |piece|.
   int PieceToId(absl::string_view piece) const override;
 
   // Verifies if two outputs are equivalent by comparing their scores.
   bool VerifyOutputsEquivalent(absl::string_view expected,
                                absl::string_view actual) const override;
 
+  enum EncoderVersion {
+    kOptimized,  // The optimized encoder.
+    kOriginal    // The original encoder.
+  };
+
+  void SetEncoderVersion(EncoderVersion encoder_version) {
+    encoder_version_ = encoder_version;
+  }
+
+  // Returns the current encoder version in use.
+  EncoderVersion GetEncoderVersion() const { return encoder_version_; }
+
  protected:
   // Builds a Trie index.
   void BuildTrie(std::vector<std::pair<absl::string_view, int>> *pieces);
 
   // The optimized Viterbi encode.
   // Main differences from the original function:
   // 1. Memorizes the best path at each postion so far,
@@ -191,12 +203,15 @@
   float min_score_ = 0.0;
   float max_score_ = 0.0;
   std::unique_ptr<Darts::DoubleArray> trie_;
 
   // Maximum size of the return value of Trie, which corresponds
   // to the maximum size of shared common prefix in the sentence pieces.
   int trie_results_size_;
+
+  // encoder version.
+  EncoderVersion encoder_version_ = kOptimized;
 };
 
 }  // namespace unigram
 }  // namespace sentencepiece
 #endif  // UNIGRAM_MODEL_H_
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unigram_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_test.cc`

 * *Files 8% similar despite different names*

```diff
@@ -246,65 +246,65 @@
   InsertWithScore(&lattice, 2, 1, 0.1);  // C
   InsertWithScore(&lattice, 0, 2, 0.2);  // AB
   InsertWithScore(&lattice, 1, 2, 0.5);  // BC
   InsertWithScore(&lattice, 0, 3, 1.0);  // ABC
 
   // Calculate expected probabilities of each path
   // Note that sampling without replacement affects the expected frequencies!
-  const std::vector<double> kTheta = {0.0, 0.01, 0.5, 0.7, 1.0};
-  for (const auto theta : kTheta) {
+  const std::vector<double> kInv_Theta = {0.0, 0.01, 0.5, 0.7, 1.0};
+  for (const auto inv_theta : kInv_Theta) {
     std::vector<std::string> strings = {"ABC", "AB C", "A BC", "A B C"};
     std::map<std::string, float> probs;
-    probs["ABC"] = std::exp(theta * 1.0);
-    probs["AB C"] = std::exp(theta * (0.2 + 0.1));
-    probs["A BC"] = std::exp(theta * (0.0 + 0.5));
-    probs["A B C"] = std::exp(theta * (0.0 + 0.0 + 0.1));
+    probs["ABC"] = std::exp(inv_theta * 1.0);
+    probs["AB C"] = std::exp(inv_theta * (0.2 + 0.1));
+    probs["A BC"] = std::exp(inv_theta * (0.0 + 0.5));
+    probs["A B C"] = std::exp(inv_theta * (0.0 + 0.0 + 0.1));
 
     for (const auto &it : strings) {
       EXPECT_EQ(1, probs.count(it));
     }
 
     double Z = 0.0;
     for (const auto &it : probs) Z += it.second;
     for (auto &it : probs) it.second /= Z;
 
     std::map<std::pair<std::string, std::string>, float> pair_probs;
-    for (const auto first : strings) {
-      for (const auto second : strings) {
+    for (const auto &first : strings) {
+      for (const auto &second : strings) {
         if (first == second) {
           pair_probs[std::make_pair(first, second)] = 0;
         } else {
           float first_prob = probs[first];
           float second_prob = probs[second] / (1 - first_prob);
           pair_probs[std::make_pair(first, second)] = first_prob * second_prob;
         }
       }
     }
 
     std::map<std::string, float> inclusion_probs;
-    for (const auto string : strings) {
+    for (const auto &string : strings) {
       float inclusion_prob = 0.0;
-      for (const auto other_string : strings) {
+      for (const auto &other_string : strings) {
         inclusion_prob += pair_probs[std::make_pair(string, other_string)];
       }
-      for (const auto other_string : strings) {
+      for (const auto &other_string : strings) {
         inclusion_prob += pair_probs[std::make_pair(other_string, string)];
       }
       inclusion_probs[string] = inclusion_prob / 2;
     }
 
     int kTrials = 10000;
 
     std::vector<int> kNumSamples = {1, 2};
 
     for (const auto num_samples : kNumSamples) {
       std::map<std::string, int> counts;
       for (int i = 0; i < kTrials; i++) {
-        auto nbests = lattice.NBest(num_samples, true, theta);
-        for (const auto nbest : nbests) {
+        auto nbests = lattice.NBest(num_samples, true, inv_theta);
+        for (const auto &nbest : nbests) {
           counts[GetTokenized(nbest.first)]++;
         }
       }
 
       EXPECT_EQ(inclusion_probs.size(), counts.size());
       // If we take multiple samples WOR, we have to use corrected probs.
       std::map<std::string, float> probs_to_use =
@@ -326,67 +326,68 @@
   InsertWithScore(&lattice, 1, 1, 0.0);  // B
   InsertWithScore(&lattice, 2, 1, 0.1);  // C
   InsertWithScore(&lattice, 0, 2, 0.2);  // AB
   InsertWithScore(&lattice, 1, 2, 0.5);  // BC
   InsertWithScore(&lattice, 0, 3, 1.0);  // ABC
 
   // Calculate expected probabilities of each path
-  const std::vector<double> kTheta = {0.0, 0.01, 0.5, 0.7, 1.0};
-  for (const auto theta : kTheta) {
+  const std::vector<double> kInv_Theta = {0.0, 0.01, 0.5, 0.7, 1.0};
+  for (const auto inv_theta : kInv_Theta) {
     std::vector<std::string> strings = {"ABC", "AB C", "A BC", "A B C"};
     std::map<std::string, float> probs;
-    probs["ABC"] = std::exp(theta * 1.0);
-    probs["AB C"] = std::exp(theta * (0.2 + 0.1));
-    probs["A BC"] = std::exp(theta * (0.0 + 0.5));
-    probs["A B C"] = std::exp(theta * (0.0 + 0.0 + 0.1));
+    probs["ABC"] = std::exp(inv_theta * 1.0);
+    probs["AB C"] = std::exp(inv_theta * (0.2 + 0.1));
+    probs["A BC"] = std::exp(inv_theta * (0.0 + 0.5));
+    probs["A B C"] = std::exp(inv_theta * (0.0 + 0.0 + 0.1));
 
     double Z = 0.0;
     for (const auto &it : probs) Z += it.second;
     for (auto &it : probs) it.second /= Z;
 
     for (const auto &it : strings) {
       EXPECT_EQ(1, probs.count(it));
     }
     float entropy = 0.0;
     for (const auto &it : probs) {
       entropy += (it.second * std::log(it.second));
     }
-    EXPECT_NEAR(-entropy, lattice.CalculateEntropy(theta), 0.02);
+    EXPECT_NEAR(-entropy, lattice.CalculateEntropy(inv_theta), 0.02);
   }
 }
 
 TEST(LatticeTest, ForwardAlgorithmTest) {
   Lattice lattice;
   lattice.SetSentence("ABC");
 
   InsertWithScore(&lattice, 0, 1, 0.0);  // A
   InsertWithScore(&lattice, 1, 1, 0.0);  // B
   InsertWithScore(&lattice, 2, 1, 0.1);  // C
   InsertWithScore(&lattice, 0, 2, 0.2);  // AB
   InsertWithScore(&lattice, 1, 2, 0.5);  // BC
   InsertWithScore(&lattice, 0, 3, 1.0);  // ABC
 
-  const std::vector<float> kTheta = {0.0, 0.01, 0.5, 0.7, 1.0};
-  for (const auto theta : kTheta) {
-    std::vector<float> alpha = lattice.ForwardAlgorithm(theta);
+  const std::vector<float> kInv_Theta = {0.0, 0.01, 0.5, 0.7, 1.0};
+  for (const auto inv_theta : kInv_Theta) {
+    std::vector<float> alpha = lattice.ForwardAlgorithm(inv_theta);
     EXPECT_EQ(alpha.size(), 8);  // 6 nodes, plus BOS, EOS
     // only alpha[C], alpha[EOS] have non-zero alpha
     for (int i : {0, 1, 2, 3}) {
       for (const auto &node : lattice.begin_nodes(i)) {
         if (i < 2) {
           EXPECT_EQ(alpha[node->node_id], 0.0);
         } else if (i == 2) {
-          float Z =
-              std::log(std::exp(theta * (0.0 + 0.0)) + std::exp(theta * 0.2));
+          float Z = std::log(std::exp(inv_theta * (0.0 + 0.0)) +
+                             std::exp(inv_theta * 0.2));
           EXPECT_EQ(alpha[node->node_id], Z);
         } else if (i == 3) {
-          float Z = std::log(std::exp(theta * (0.0 + 0.0 + 0.1)) +  // A + B + C
-                             std::exp(theta * (0.2 + 0.1)) +        // AB + C
-                             std::exp(theta * (0.0 + 0.5)) +        // A + BC
-                             std::exp(theta * 1.0));                // ABC
+          float Z =
+              std::log(std::exp(inv_theta * (0.0 + 0.0 + 0.1)) +  // A + B + C
+                       std::exp(inv_theta * (0.2 + 0.1)) +        // AB + C
+                       std::exp(inv_theta * (0.0 + 0.5)) +        // A + BC
+                       std::exp(inv_theta * 1.0));                // ABC
           EXPECT_EQ(Z, alpha[node->node_id]);
         }
       }
     }
   }
 }
 
@@ -432,33 +433,33 @@
   InsertWithScoreAndId(&lattice, 0, 1, 1.0, 0);  // A
   InsertWithScoreAndId(&lattice, 1, 1, 1.2, 1);  // B
   InsertWithScoreAndId(&lattice, 2, 1, 1.5, 2);  // C
   InsertWithScoreAndId(&lattice, 0, 2, 1.6, 3);  // AB
   InsertWithScoreAndId(&lattice, 1, 2, 1.7, 4);  // BC
   InsertWithScoreAndId(&lattice, 0, 3, 1.8, 5);  // ABC
 
-  const std::vector<double> kTheta = {0.0, 0.01, 0.5, 0.7, 1.0};
-  for (int i = 0; i < kTheta.size(); ++i) {
+  const std::vector<double> kInv_Theta = {0.0, 0.01, 0.5, 0.7, 1.0};
+  for (int i = 0; i < kInv_Theta.size(); ++i) {
     std::map<std::string, double> probs;
     // Expands all paths in the lattice.
-    probs["A B C"] = exp(kTheta[i] * (1.0 + 1.2 + 1.5));  // A B C
-    probs["AB C"] = exp(kTheta[i] * (1.6 + 1.5));         // AB C
-    probs["A BC"] = exp(kTheta[i] * (1.0 + 1.7));         // A BC
-    probs["ABC"] = exp(kTheta[i] * 1.8);                  // ABC
+    probs["A B C"] = exp(kInv_Theta[i] * (1.0 + 1.2 + 1.5));  // A B C
+    probs["AB C"] = exp(kInv_Theta[i] * (1.6 + 1.5));         // AB C
+    probs["A BC"] = exp(kInv_Theta[i] * (1.0 + 1.7));         // A BC
+    probs["ABC"] = exp(kInv_Theta[i] * 1.8);                  // ABC
 
     // Computes expected probabilities.
     double Z = 0.0;
     for (const auto &it : probs) Z += it.second;
     for (auto &it : probs) it.second /= Z;
 
     // Samples `kTrial` times and verifies the probabilities.
     constexpr int kTrial = 100000;
     std::map<std::string, int> freq;
     for (int n = 0; n < kTrial; ++n) {
-      freq[GetTokenized(lattice.Sample(kTheta[i]))]++;
+      freq[GetTokenized(lattice.Sample(kInv_Theta[i]))]++;
     }
 
     EXPECT_EQ(probs.size(), freq.size());
     for (const auto &it : probs) {
       EXPECT_NEAR(it.second, 1.0 * freq[it.first] / kTrial, 0.02);
     }
   }
@@ -477,26 +478,26 @@
   sp3->set_type(ModelProto::SentencePiece::CONTROL);
   sp3->set_piece("</s>");
 
   return model_proto;
 }
 
 // Returns model protos in parameterized tests.
-const std::vector<EncoderVersion> &GetEncoderVersions() {
-  static const std::vector<EncoderVersion> &v =
-      *new std::vector<EncoderVersion>{EncoderVersion::kOptimized,
-                                       EncoderVersion::kOriginal};
+const std::vector<Model::EncoderVersion> &GetEncoderVersions() {
+  static const std::vector<Model::EncoderVersion> &v =
+      *new std::vector<Model::EncoderVersion>{Model::kOptimized,
+                                              Model::kOriginal};
   return v;
 }
 
-class UnigramModelTest : public test::TestWithParam<EncoderVersion> {
+class UnigramModelTest : public test::TestWithParam<Model::EncoderVersion> {
  protected:
   void SetUp() override { encoder_version_ = GetParam(); }
   void TearDown() override {}
-  EncoderVersion encoder_version_;
+  Model::EncoderVersion encoder_version_;
 };
 
 void AddPiece(ModelProto *model_proto, const std::string &piece,
               float score = 0.0) {
   auto *sp = model_proto->add_pieces();
   sp->set_piece(piece);
   sp->set_score(score);
@@ -527,65 +528,65 @@
 
   Model model(model_proto);
 
   Lattice lattice;
   lattice.SetSentence("ABC");
   model.PopulateNodes(&lattice);
 
-  std::vector<float> kTheta = {0.0, 1.0};
+  std::vector<float> kInv_Theta = {0.0, 1.0};
 
-  for (const auto theta : kTheta) {
+  for (const auto inv_theta : kInv_Theta) {
     std::vector<std::string> strings = {"ABC", "AB C", "A BC", "A B C"};
     std::map<std::string, float> probs;
-    probs["ABC"] = std::exp(theta * 1.0);
-    probs["AB C"] = std::exp(theta * (0.2 + 0.1));
-    probs["A BC"] = std::exp(theta * (0.0 + 0.5));
-    probs["A B C"] = std::exp(theta * (0.0 + 0.0 + 0.1));
+    probs["ABC"] = std::exp(inv_theta * 1.0);
+    probs["AB C"] = std::exp(inv_theta * (0.2 + 0.1));
+    probs["A BC"] = std::exp(inv_theta * (0.0 + 0.5));
+    probs["A B C"] = std::exp(inv_theta * (0.0 + 0.0 + 0.1));
 
     for (const auto &it : strings) {
       EXPECT_EQ(1, probs.count(it));
     }
 
     double Z = 0.0;
     for (const auto &it : probs) Z += it.second;
     for (auto &it : probs) it.second /= Z;
 
     std::map<std::pair<std::string, std::string>, float> pair_probs;
-    for (const auto first : strings) {
-      for (const auto second : strings) {
+    for (const auto &first : strings) {
+      for (const auto &second : strings) {
         if (first == second) {
           pair_probs[std::make_pair(first, second)] = 0;
         } else {
-          float first_prob = probs[first];
-          float second_prob = probs[second] / (1 - first_prob);
+          const float first_prob = probs[first];
+          const float second_prob = probs[second] / (1 - first_prob);
           pair_probs[std::make_pair(first, second)] = first_prob * second_prob;
         }
       }
     }
 
     std::map<std::string, float> inclusion_probs;
-    for (const auto string : strings) {
+    for (const auto &string : strings) {
       float inclusion_prob = 0.0;
-      for (const auto other_string : strings) {
+      for (const auto &other_string : strings) {
         inclusion_prob += pair_probs[std::make_pair(string, other_string)];
       }
-      for (const auto other_string : strings) {
+      for (const auto &other_string : strings) {
         inclusion_prob += pair_probs[std::make_pair(other_string, string)];
       }
       inclusion_probs[string] = inclusion_prob / 2;
     }
     std::vector<int> kNumSamples = {1, 2};
 
     for (const auto num_samples : kNumSamples) {
       std::map<std::string, int> counts;
       std::map<std::string, float> scores;
       int kTrials = 50000;
       for (int i = 0; i < kTrials; i++) {
-        NBestEncodeResult sample =
-            model.SampleEncodeAndScore("ABC", theta, num_samples, true, false);
+        NBestEncodeResult sample = model.SampleEncodeAndScore(
+            "ABC", inv_theta, num_samples, true, false);
 
         for (const auto &it : sample) {
           std::vector<std::string> tokens;
           for (const auto &inner_it : it.first) {
             tokens.push_back(std::string(inner_it.first));
           }
           std::string sample_string = absl::StrJoin(tokens, " ");
@@ -616,15 +617,15 @@
 
   AddPiece(&model_proto, "a", 0.1);
   AddPiece(&model_proto, "b", 0.2);
   AddPiece(&model_proto, "c", 0.3);
   AddPiece(&model_proto, "d", 0.4);
 
   Model model(model_proto);
-  EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+  model.SetEncoderVersion(encoder_version_);
 
   EXPECT_EQ(model_proto.SerializeAsString(),
             model.model_proto().SerializeAsString());
 
   EXPECT_NEAR(0.1, model.min_score(), 0.001);
   EXPECT_NEAR(0.4, model.max_score(), 0.001);
 
@@ -674,15 +675,15 @@
   EXPECT_TRUE(model.Encode("").empty());
 }
 
 TEST_P(UnigramModelTest, PopulateNodesAllUnknownsTest) {
   ModelProto model_proto = MakeBaseModelProto();
   AddPiece(&model_proto, "x");
   Model model(model_proto);
-  EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+  model.SetEncoderVersion(encoder_version_);
 
   Lattice lattice;
   lattice.SetSentence("abc");
   model.PopulateNodes(&lattice);
 
   EXPECT_EQ(1, lattice.begin_nodes(0).size());
   EXPECT_EQ(1, lattice.begin_nodes(1).size());
@@ -698,15 +699,15 @@
 
   AddPiece(&model_proto, "a", 0.1);   // 3
   AddPiece(&model_proto, "b", 0.2);   // 4
   AddPiece(&model_proto, "ab", 0.3);  // 5
   AddPiece(&model_proto, "bc", 0.4);  // 6
 
   Model model(model_proto);
-  EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+  model.SetEncoderVersion(encoder_version_);
 
   Lattice lattice;
   lattice.SetSentence("abc");
 
   model.PopulateNodes(&lattice);
 
   EXPECT_EQ(2, lattice.begin_nodes(0).size());  // a,ab
@@ -733,15 +734,15 @@
   AddPiece(&model_proto, "ab", 0.3);  // 5
   AddPiece(&model_proto, "bc", 0.4);  // 6
 
   model_proto.mutable_pieces(5)->set_type(ModelProto::SentencePiece::UNUSED);
   model_proto.mutable_pieces(6)->set_type(ModelProto::SentencePiece::UNUSED);
 
   Model model(model_proto);
-  EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+  model.SetEncoderVersion(encoder_version_);
 
   Lattice lattice;
   lattice.SetSentence("abc");
 
   model.PopulateNodes(&lattice);
 
   EXPECT_EQ(1, lattice.begin_nodes(0).size());  // a
@@ -758,15 +759,15 @@
   AddPiece(&model_proto, "b", 0.0);     // 4
   AddPiece(&model_proto, "c", 0.0);     // 5
   AddPiece(&model_proto, "ab", 2.0);    // 6
   AddPiece(&model_proto, "bc", 5.0);    // 7
   AddPiece(&model_proto, "abc", 10.0);  // 8
 
   Model model(model_proto);
-  EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+  model.SetEncoderVersion(encoder_version_);
 
   auto nbest = model.NBestEncode("", 10);
   EXPECT_EQ(1, nbest.size());
   EXPECT_TRUE(nbest[0].first.empty());
   EXPECT_EQ(0.0, nbest[0].second);
 
   nbest = model.NBestEncode("abc", 10);
@@ -797,15 +798,15 @@
       ModelProto::SentencePiece::USER_DEFINED);
   model_proto.mutable_pieces(11)->set_type(  // q
       ModelProto::SentencePiece::USER_DEFINED);
   model_proto.mutable_pieces(12)->set_type(  // r
       ModelProto::SentencePiece::USER_DEFINED);
 
   Model model(model_proto);
-  EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+  model.SetEncoderVersion(encoder_version_);
 
   EncodeResult result;
 
   result = model.Encode("abc");
   EXPECT_EQ(1, result.size());
   EXPECT_EQ("abc", result[0].first);
 
@@ -880,49 +881,49 @@
   AddPiece(&model_proto, "b", 0.0);      // 8
   AddPiece(&model_proto, "c", 0.0);      // 9
   AddPiece(&model_proto, "d", 0.0);      // 10
 
   // No unused.
   {
     Model model(model_proto);
-    EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+    model.SetEncoderVersion(encoder_version_);
     const auto result = model.Encode("abcd");
     EXPECT_EQ(1, result.size());
     EXPECT_EQ("abcd", result[0].first);
   }
 
   {
     model_proto.mutable_pieces(3)->set_type(ModelProto::SentencePiece::UNUSED);
     Model model(model_proto);
-    EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+    model.SetEncoderVersion(encoder_version_);
     const auto result = model.Encode("abcd");
     EXPECT_EQ(2, result.size());
     EXPECT_EQ("abc", result[0].first);
     EXPECT_EQ("d", result[1].first);
   }
 
   {
     model_proto.mutable_pieces(3)->set_type(ModelProto::SentencePiece::UNUSED);
     model_proto.mutable_pieces(5)->set_type(ModelProto::SentencePiece::UNUSED);
     Model model(model_proto);
-    EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+    model.SetEncoderVersion(encoder_version_);
     const auto result = model.Encode("abcd");
     EXPECT_EQ(2, result.size());
     EXPECT_EQ("abc", result[0].first);
     EXPECT_EQ("d", result[1].first);
   }
 
   {
     // This is different from BPE segmentation.
     // Unigram language model simply finds the best path without unused nodes.
     model_proto.mutable_pieces(3)->set_type(ModelProto::SentencePiece::UNUSED);
     model_proto.mutable_pieces(4)->set_type(ModelProto::SentencePiece::UNUSED);
     model_proto.mutable_pieces(5)->set_type(ModelProto::SentencePiece::NORMAL);
     Model model(model_proto);
-    EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+    model.SetEncoderVersion(encoder_version_);
     const auto result = model.Encode("abcd");
     EXPECT_EQ(2, result.size());
     EXPECT_EQ("ab", result[0].first);
     EXPECT_EQ("cd", result[1].first);
   }
 }
 
@@ -934,15 +935,15 @@
   AddPiece(&model_proto, "ab", 6.0);     // 5
   AddPiece(&model_proto, "cd", 4.0);     // 6
   AddPiece(&model_proto, "a", 4.0);      // 7
   AddPiece(&model_proto, "b", 1.9);      // 8
   AddPiece(&model_proto, "c", 2.0);      // 9
   AddPiece(&model_proto, "d", 1.0);      // 10
   Model model(model_proto);
-  EXPECT_TRUE(model.SetEncoderVersion(encoder_version_).ok());
+  model.SetEncoderVersion(encoder_version_);
   // Equivalent outputs.
   EXPECT_TRUE(model.VerifyOutputsEquivalent("", ""));
   EXPECT_TRUE(model.VerifyOutputsEquivalent("a b", "a b"));
   EXPECT_TRUE(model.VerifyOutputsEquivalent("abcd", "ab cd"));
 
   // Inequivalent outputs.
   EXPECT_FALSE(model.VerifyOutputsEquivalent("a", "a b"));
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/unigram_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/unigram_model_trainer.h`

 * *Files 6% similar despite different names*

```diff
@@ -64,25 +64,27 @@
  public:
   Trainer(const TrainerSpec &trainer_spec,
           const NormalizerSpec &normalizer_spec,
           const NormalizerSpec &denormalizer_spec)
       : TrainerInterface::TrainerInterface(trainer_spec, normalizer_spec,
                                            denormalizer_spec) {}
 
+  TrainerModel::SentencePieces MakeSeedSentencePieces();
+
   util::Status Train() override;
 
  private:
   FRIEND_TEST(TrainerTest, IsValidSentencePieceTest);
 
   // Makes seed pieces from the training corpus.
   // The size of seed pieces is determined by seed_sentencepiece_size.
   // node_int_type should be of integer type (int32 or int64),
   // determined by train_extremely_large_corpus.
   template <typename node_int_type>
-  TrainerModel::SentencePieces MakeSeedSentencePieces() const;
+  TrainerModel::SentencePieces MakeSeedSentencePiecesInternal();
 
   // Executes the E step of EM and returns expected count.
   // The index of return array is the vocab id.
   // |objective| is a negative likelihood of the current model.
   // |num_token| is the number of total tokens to tokenize
   // training corpus.
   std::vector<float> RunEStep(const TrainerModel &model, float *objective,
@@ -99,14 +101,17 @@
       const TrainerModel &model) const;
 
   // Makes the final sentence pieces by incorporating the required characters
   // and control/user defined symbols.
   TrainerModel::SentencePieces FinalizeSentencePieces(
       const TrainerModel &model) const;
 
+  std::pair<const char32 *, const char32 *> NormalizeRange(
+      const char32 *begin, const char32 *end) const;
+
   // When the size of SentencePieces becomes less than desired_vocab_size_,
   // break the main training loop. desired_vocab_size_ = 1.1 * vocab_size_
   // for now.
   int desired_vocab_size_;
 };
 }  // namespace unigram
 }  // namespace sentencepiece
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/util.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.cc`

 * *Files 6% similar despite different names*

```diff
@@ -8,37 +8,42 @@
 //
 // Unless required by applicable law or agreed to in writing, software
 // distributed under the License is distributed on an "AS IS" BASIS,
 // WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 // See the License for the specific language governing permissions and
 // limitations under the License.!
 
-#include <iostream>
-
 #include "util.h"
 
+#include <atomic>
+#include <iostream>
+
 namespace sentencepiece {
 
 namespace {
 constexpr unsigned int kDefaultSeed = static_cast<unsigned int>(-1);
-static unsigned int g_seed = kDefaultSeed;
-static int g_minloglevel = 0;
+static std::atomic<unsigned int> g_seed = kDefaultSeed;
+static std::atomic<int> g_minloglevel = 0;
 }  // namespace
 
 void SetRandomGeneratorSeed(unsigned int seed) {
-  if (seed != kDefaultSeed) g_seed = seed;
+  if (seed != kDefaultSeed) g_seed.store(seed);
 }
 
 uint32 GetRandomGeneratorSeed() {
-  return g_seed == kDefaultSeed ? std::random_device{}() : g_seed;
+  try {
+    return g_seed == kDefaultSeed ? std::random_device{}() : g_seed.load();
+  } catch (...) {
+    return g_seed.load();
+  }
 }
 
 namespace logging {
-int GetMinLogLevel() { return g_minloglevel; }
-void SetMinLogLevel(int v) { g_minloglevel = v; }
+int GetMinLogLevel() { return g_minloglevel.load(); }
+void SetMinLogLevel(int v) { g_minloglevel.store(v); }
 }  // namespace logging
 
 namespace string_util {
 
 // mblen sotres the number of bytes consumed after decoding.
 char32 DecodeUTF8(const char *begin, const char *end, size_t *mblen) {
   const size_t len = end - begin;
@@ -213,15 +218,14 @@
   char *str = const_cast<char *>(buf.data());
   char *eos = str + text.size();
   char *start = nullptr;
   char *end = nullptr;
 
   std::vector<std::string> result;
   for (; str < eos; ++str) {
-    while (*str == ' ' || *str == '\t') ++str;
     if (*str == '"') {
       start = ++str;
       end = start;
       for (; str < eos; ++str) {
         if (*str == '"') {
           str++;
           if (*str != '"') break;
@@ -240,44 +244,28 @@
 
   return result;
 }
 }  // namespace util
 
 #ifdef OS_WIN
 namespace win32 {
-std::wstring Utf8ToWide(const std::string &input) {
-  int output_length =
-      ::MultiByteToWideChar(CP_UTF8, 0, input.c_str(), -1, nullptr, 0);
+std::wstring Utf8ToWide(absl::string_view input) {
+  int output_length = ::MultiByteToWideChar(
+      CP_UTF8, 0, input.data(), static_cast<int>(input.size()), nullptr, 0);
   output_length = output_length <= 0 ? 0 : output_length - 1;
   if (output_length == 0) {
     return L"";
   }
   std::unique_ptr<wchar_t[]> input_wide(new wchar_t[output_length + 1]);
-  const int result = ::MultiByteToWideChar(CP_UTF8, 0, input.c_str(), -1,
+  std::fill(input_wide.get(), input_wide.get() + output_length + 1, L'\0');
+  const int result = ::MultiByteToWideChar(CP_UTF8, 0, input.data(),
+                                           static_cast<int>(input.size()),
                                            input_wide.get(), output_length + 1);
   std::wstring output;
   if (result > 0) {
     output.assign(input_wide.get());
   }
   return output;
 }
-
-std::string WideToUtf8(const std::wstring &input) {
-  const int output_length = ::WideCharToMultiByte(CP_UTF8, 0, input.c_str(), -1,
-                                                  nullptr, 0, nullptr, nullptr);
-  if (output_length == 0) {
-    return "";
-  }
-
-  std::unique_ptr<char[]> input_encoded(new char[output_length + 1]);
-  const int result =
-      ::WideCharToMultiByte(CP_UTF8, 0, input.c_str(), -1, input_encoded.get(),
-                            output_length + 1, nullptr, nullptr);
-  std::string output;
-  if (result > 0) {
-    output.assign(input_encoded.get());
-  }
-  return output;
-}
 }  // namespace win32
 #endif
 }  // namespace sentencepiece
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/util.h`

 * *Files 4% similar despite different names*

```diff
@@ -32,46 +32,28 @@
 #include "sentencepiece_processor.h"
 #include "third_party/absl/strings/string_view.h"
 
 #ifdef SPM_NO_THREADLOCAL
 #include <pthread.h>
 #endif
 
-#if !defined(__APPLE__) && !defined(_WIN32)
-#include <endian.h>
-#if BYTE_ORDER == __BIG_ENDIAN
-#define IS_BIG_ENDIAN
-#endif
-#endif
-
 namespace sentencepiece {
 template <typename T>
 std::ostream &operator<<(std::ostream &out, const std::vector<T> &v) {
   for (const auto n : v) {
     out << " " << n;
   }
   return out;
 }
 
 uint32 GetRandomGeneratorSeed();
 
 // String utilities
 namespace string_util {
 
-struct string_view_hash {
-  // DJB hash function.
-  inline size_t operator()(const absl::string_view &sp) const {
-    size_t hash = 5381;
-    for (size_t i = 0; i < sp.size(); ++i) {
-      hash = ((hash << 5) + hash) + sp[i];
-    }
-    return hash;
-  }
-};
-
 template <typename Target>
 inline bool lexical_cast(absl::string_view arg, Target *result) {
   std::stringstream ss;
   return (ss << arg.data() && ss >> *result);
 }
 
 template <>
@@ -98,15 +80,14 @@
 inline bool lexical_cast(absl::string_view arg, std::string *result) {
   *result = std::string(arg);
   return true;
 }
 
 template <typename T>
 inline bool DecodePOD(absl::string_view str, T *result) {
-  CHECK_NOTNULL(result);
   if (sizeof(*result) != str.size()) {
     return false;
   }
   memcpy(result, str.data(), sizeof(T));
   return true;
 }
 
@@ -416,18 +397,14 @@
 #define CHECK_EQ_OR_RETURN(a, b) CHECK_OR_RETURN((a) == (b))
 #define CHECK_NE_OR_RETURN(a, b) CHECK_OR_RETURN((a) != (b))
 #define CHECK_GE_OR_RETURN(a, b) CHECK_OR_RETURN((a) >= (b))
 #define CHECK_LE_OR_RETURN(a, b) CHECK_OR_RETURN((a) <= (b))
 #define CHECK_GT_OR_RETURN(a, b) CHECK_OR_RETURN((a) > (b))
 #define CHECK_LT_OR_RETURN(a, b) CHECK_OR_RETURN((a) < (b))
 
-#ifdef IS_BIG_ENDIAN
-inline uint32 Swap32(uint32 x) { return __builtin_bswap32(x); }
-#endif
-
 }  // namespace util
 
 namespace port {
 template <typename T>
 void STLDeleteElements(std::vector<T *> *vec) {
   for (auto item : *vec) {
     delete item;
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/util_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/util_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/word_model.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/word_model.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/word_model_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/word_model_trainer.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/word_model_trainer.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/src/word_model_trainer_test.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/src/word_model_trainer_test.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/container/flat_hash_map.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/container/flat_hash_set.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/container/flat_hash_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/flags/flag.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.cc`

 * *Files 5% similar despite different names*

```diff
@@ -57,16 +57,16 @@
   const char *type;
   std::string default_value;
   std::function<void(const std::string &)> set_value;
 };
 
 namespace {
 
-using FlagMap = std::map<std::string, FlagFunc *>;
-using FlagList = std::vector<FlagFunc *>;
+using FlagMap = std::map<std::string, std::shared_ptr<FlagFunc>>;
+using FlagList = std::vector<std::shared_ptr<FlagFunc>>;
 
 FlagMap *GetFlagMap() {
   static auto *flag_map = new FlagMap;
   return flag_map;
 }
 
 FlagList *GetFlagList() {
@@ -107,27 +107,27 @@
 }
 
 std::string PrintHelp(const char *programname) {
   std::ostringstream os;
   os << PACKAGE_STRING << "\n\n";
   os << "Usage: " << programname << " [options] files\n\n";
 
-  for (const auto *func : *GetFlagList()) {
+  for (auto func : *GetFlagList()) {
     os << "   --" << func->name << " (" << func->help << ")";
     os << "  type: " << func->type << " default: " << func->default_value
        << '\n';
   }
 
   os << "\n\n";
 
   return os.str();
 }
 }  // namespace
 
-void RegisterFlag(const std::string &name, FlagFunc *func) {
+void RegisterFlag(const std::string &name, std::shared_ptr<FlagFunc> func) {
   GetFlagList()->emplace_back(func);
   GetFlagMap()->emplace(name, func);
 }
 }  // namespace internal
 
 template <typename T>
 Flag<T>::Flag(const char *name, const char *type, const char *help,
@@ -136,15 +136,15 @@
   func_->name = name;
   func_->help = help;
   func_->type = type;
   func_->default_value = internal::to_str<T>(default_value);
   func_->set_value = [this](const std::string &value) {
     this->set_value_as_str(value);
   };
-  RegisterFlag(name, func_.get());
+  RegisterFlag(name, func_);
 }
 
 template <typename T>
 Flag<T>::~Flag() {}
 
 template <typename T>
 const T &Flag<T>::value() const {
@@ -169,14 +169,15 @@
     sentencepiece::string_util::lexical_cast<bool>(value_as_str, &value_);
 }
 
 template class Flag<std::string>;
 template class Flag<int32>;
 template class Flag<uint32>;
 template class Flag<double>;
+template class Flag<float>;
 template class Flag<bool>;
 template class Flag<int64>;
 template class Flag<uint64>;
 
 std::vector<char *> ParseCommandLine(int argc, char *argv[]) {
   if (argc == 0) return {};
 
@@ -214,8 +215,18 @@
   } else if (absl::GetFlag(FLAGS_version)) {
     std::cout << PACKAGE_STRING << " " << VERSION << std::endl;
     sentencepiece::error::Exit(0);
   }
 
   return output_args;
 }
+
+void CleanupFlags() {
+  static bool is_shutdown = false;
+  if (!is_shutdown) {
+    delete internal::GetFlagList();
+    delete internal::GetFlagMap();
+    is_shutdown = true;
+  }
+}
+
 }  // namespace absl
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/flags/flag.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/flag.h`

 * *Files 8% similar despite different names*

```diff
@@ -20,42 +20,48 @@
 #include <string>
 #include <vector>
 
 namespace absl {
 namespace internal {
 struct FlagFunc;
 
-void RegisterFlag(const std::string &name, FlagFunc *func);
+void RegisterFlag(const std::string &name, std::shared_ptr<FlagFunc> func);
+
 }  // namespace internal
 
 template <typename T>
 class Flag {
  public:
   Flag(const char *name, const char *type, const char *help,
        const T &defautl_value);
   virtual ~Flag();
   const T &value() const;
   void set_value(const T &value);
   void set_value_as_str(const std::string &value_as_str);
 
  private:
   T value_;
-  std::unique_ptr<internal::FlagFunc> func_;
+  std::shared_ptr<internal::FlagFunc> func_;
 };
 
 template <typename T>
 const T &GetFlag(const Flag<T> &flag) {
   return flag.value();
 }
 
 template <typename T, typename V>
 void SetFlag(Flag<T> *flag, const V &v) {
   const T value(v);
   flag->set_value(value);
 }
+
+#define HAS_ABSL_CLEANUP_FLAGS
+
+void CleanupFlags();
+
 }  // namespace absl
 
 #define ABSL_FLAG(Type, name, defautl_value, help) \
   absl::Flag<Type> FLAGS_##name(#name, #Type, help, defautl_value);
 
 #define ABSL_DECLARE_FLAG(Type, name) extern absl::Flag<Type> FLAGS_##name;
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/flags/parse.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/flags/parse.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/memory/memory.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/memory/memory.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/ascii.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/ascii.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/match.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/match.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/numbers.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/numbers.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_cat.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_cat.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_format.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_format.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_join.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_join.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_replace.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_replace.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/str_split.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/str_split.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/string_view.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringpiece.cc`

 * *Files 27% similar despite different names*

```diff
@@ -1,267 +1,270 @@
-// Copyright 2017 The Abseil Authors.
+// Protocol Buffers - Google's data interchange format
+// Copyright 2008 Google Inc.  All rights reserved.
+// https://developers.google.com/protocol-buffers/
 //
-// Licensed under the Apache License, Version 2.0 (the "License");
-// you may not use this file except in compliance with the License.
-// You may obtain a copy of the License at
+// Redistribution and use in source and binary forms, with or without
+// modification, are permitted provided that the following conditions are
+// met:
 //
-//      http://www.apache.org/licenses/LICENSE-2.0
+//     * Redistributions of source code must retain the above copyright
+// notice, this list of conditions and the following disclaimer.
+//     * Redistributions in binary form must reproduce the above
+// copyright notice, this list of conditions and the following disclaimer
+// in the documentation and/or other materials provided with the
+// distribution.
+//     * Neither the name of Google Inc. nor the names of its
+// contributors may be used to endorse or promote products derived from
+// this software without specific prior written permission.
 //
-// Unless required by applicable law or agreed to in writing, software
-// distributed under the License is distributed on an "AS IS" BASIS,
-// WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-// See the License for the specific language governing permissions and
-// limitations under the License.
-
-#include "third_party/absl/strings/string_view.h"
-
-#ifndef ABSL_HAVE_STD_STRING_VIEW
+// THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+// "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+// LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+// A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+// OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+// SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+// LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+// DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+// THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+// (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+// OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+#include <google/protobuf/stubs/stringpiece.h>
 
+#include <string.h>
 #include <algorithm>
 #include <climits>
-#include <cstring>
+#include <string>
 #include <ostream>
 
-// #include "absl/strings/internal/memutil.h"
+#include <google/protobuf/stubs/logging.h>
 
-namespace absl {
+namespace google {
+namespace protobuf {
+std::ostream& operator<<(std::ostream& o, StringPiece piece) {
+  o.write(piece.data(), piece.size());
+  return o;
+}
 
-namespace {
-void WritePadding(std::ostream& o, size_t pad) {
-  char fill_buf[32];
-  memset(fill_buf, o.fill(), sizeof(fill_buf));
-  while (pad) {
-    size_t n = std::min(pad, sizeof(fill_buf));
-    o.write(fill_buf, n);
-    pad -= n;
-  }
+// Out-of-line error path.
+void StringPiece::LogFatalSizeTooBig(size_t size, const char* details) {
+  GOOGLE_LOG(FATAL) << "size too big: " << size << " details: " << details;
 }
 
-class LookupTable {
- public:
-  // For each character in wanted, sets the index corresponding
-  // to the ASCII code of that character. This is used by
-  // the find_.*_of methods below to tell whether or not a character is in
-  // the lookup table in constant time.
-  explicit LookupTable(string_view wanted) {
-    for (char c : wanted) {
-      table_[Index(c)] = true;
-    }
+StringPiece::StringPiece(StringPiece x, stringpiece_ssize_type pos)
+    : ptr_(x.ptr_ + pos), length_(x.length_ - pos) {
+  GOOGLE_DCHECK_LE(0, pos);
+  GOOGLE_DCHECK_LE(pos, x.length_);
+}
+
+StringPiece::StringPiece(StringPiece x,
+                         stringpiece_ssize_type pos,
+                         stringpiece_ssize_type len)
+    : ptr_(x.ptr_ + pos), length_(std::min(len, x.length_ - pos)) {
+  GOOGLE_DCHECK_LE(0, pos);
+  GOOGLE_DCHECK_LE(pos, x.length_);
+  GOOGLE_DCHECK_GE(len, 0);
+}
+
+void StringPiece::CopyToString(std::string* target) const {
+  target->assign(ptr_, length_);
+}
+
+void StringPiece::AppendToString(std::string* target) const {
+  target->append(ptr_, length_);
+}
+
+bool StringPiece::Consume(StringPiece x) {
+  if (starts_with(x)) {
+    ptr_ += x.length_;
+    length_ -= x.length_;
+    return true;
   }
-  bool operator[](char c) const { return table_[Index(c)]; }
+  return false;
+}
 
- private:
-  static unsigned char Index(char c) { return static_cast<unsigned char>(c); }
-  bool table_[UCHAR_MAX + 1] = {};
-};
-
-}  // namespace
-
-std::ostream& operator<<(std::ostream& o, string_view piece) {
-  std::ostream::sentry sentry(o);
-  if (sentry) {
-    size_t lpad = 0;
-    size_t rpad = 0;
-    if (static_cast<size_t>(o.width()) > piece.size()) {
-      size_t pad = o.width() - piece.size();
-      if ((o.flags() & o.adjustfield) == o.left) {
-        rpad = pad;
-      } else {
-        lpad = pad;
-      }
-    }
-    if (lpad) WritePadding(o, lpad);
-    o.write(piece.data(), piece.size());
-    if (rpad) WritePadding(o, rpad);
-    o.width(0);
+bool StringPiece::ConsumeFromEnd(StringPiece x) {
+  if (ends_with(x)) {
+    length_ -= x.length_;
+    return true;
   }
-  return o;
+  return false;
 }
 
-string_view::size_type string_view::copy(char* buf, size_type n,
+stringpiece_ssize_type StringPiece::copy(char* buf,
+                                         size_type n,
                                          size_type pos) const {
-  size_type ulen = length_;
-  assert(pos <= ulen);
-  size_type rlen = std::min(ulen - pos, n);
-  if (rlen > 0) {
-    const char* start = ptr_ + pos;
-    std::copy(start, start + rlen, buf);
-  }
-  return rlen;
-}
-
-namespace {
-const char* memmatch(const char* phaystack, size_t haylen, const char* pneedle,
-                     size_t neelen) {
-  if (0 == neelen) {
-    return phaystack;  // even if haylen is 0
-  }
-  if (haylen < neelen) {
-    return nullptr;
-  }
-  const char* match;
-  const char* hayend = phaystack + haylen - neelen + 1;
-  while ((match = (const char*)(memchr(phaystack, pneedle[0],
-                                       hayend - phaystack)))) {
-    if (memcmp(match, pneedle, neelen) == 0) {
-      return match;
-    } else {
-      phaystack = match + 1;
-    }
-  }
-  return nullptr;
+  stringpiece_ssize_type ret = std::min(length_ - pos, n);
+  memcpy(buf, ptr_ + pos, ret);
+  return ret;
 }
-}  // namespace
 
-string_view::size_type string_view::find(string_view s, size_type pos) const
-    noexcept {
-  if (empty() || pos > length_) {
-    if (empty() && pos == 0 && s.empty()) return 0;
+bool StringPiece::contains(StringPiece s) const {
+  return find(s, 0) != npos;
+}
+
+stringpiece_ssize_type StringPiece::find(StringPiece s, size_type pos) const {
+  if (length_ <= 0 || pos > static_cast<size_type>(length_)) {
+    if (length_ == 0 && pos == 0 && s.length_ == 0) return 0;
     return npos;
   }
-  const char* result = memmatch(ptr_ + pos, length_ - pos, s.ptr_, s.length_);
-  return result ? result - ptr_ : npos;
+  const char *result = std::search(ptr_ + pos, ptr_ + length_,
+                                   s.ptr_, s.ptr_ + s.length_);
+  return result == ptr_ + length_ ? npos : result - ptr_;
 }
 
-string_view::size_type string_view::find(char c, size_type pos) const noexcept {
-  if (empty() || pos >= length_) {
+stringpiece_ssize_type StringPiece::find(char c, size_type pos) const {
+  if (length_ <= 0 || pos >= static_cast<size_type>(length_)) {
     return npos;
   }
-  const char* result =
-      static_cast<const char*>(memchr(ptr_ + pos, c, length_ - pos));
+  const char* result = static_cast<const char*>(
+      memchr(ptr_ + pos, c, length_ - pos));
   return result != nullptr ? result - ptr_ : npos;
 }
 
-string_view::size_type string_view::rfind(string_view s, size_type pos) const
-    noexcept {
+stringpiece_ssize_type StringPiece::rfind(StringPiece s, size_type pos) const {
   if (length_ < s.length_) return npos;
-  if (s.empty()) return std::min(length_, pos);
-  const char* last = ptr_ + std::min(length_ - s.length_, pos) + s.length_;
+  const size_t ulen = length_;
+  if (s.length_ == 0) return std::min(ulen, pos);
+
+  const char* last = ptr_ + std::min(ulen - s.length_, pos) + s.length_;
   const char* result = std::find_end(ptr_, last, s.ptr_, s.ptr_ + s.length_);
   return result != last ? result - ptr_ : npos;
 }
 
 // Search range is [0..pos] inclusive.  If pos == npos, search everything.
-string_view::size_type string_view::rfind(char c, size_type pos) const
-    noexcept {
+stringpiece_ssize_type StringPiece::rfind(char c, size_type pos) const {
   // Note: memrchr() is not available on Windows.
-  if (empty()) return npos;
-  for (size_type i = std::min(pos, length_ - 1);; --i) {
+  if (length_ <= 0) return npos;
+  for (stringpiece_ssize_type i =
+      std::min(pos, static_cast<size_type>(length_ - 1));
+       i >= 0; --i) {
     if (ptr_[i] == c) {
       return i;
     }
-    if (i == 0) break;
   }
   return npos;
 }
 
-string_view::size_type string_view::find_first_of(string_view s,
-                                                  size_type pos) const
-    noexcept {
-  if (empty() || s.empty()) {
+// For each character in characters_wanted, sets the index corresponding
+// to the ASCII code of that character to 1 in table.  This is used by
+// the find_.*_of methods below to tell whether or not a character is in
+// the lookup table in constant time.
+// The argument `table' must be an array that is large enough to hold all
+// the possible values of an unsigned char.  Thus it should be be declared
+// as follows:
+//   bool table[UCHAR_MAX + 1]
+static inline void BuildLookupTable(StringPiece characters_wanted,
+                                    bool* table) {
+  const stringpiece_ssize_type length = characters_wanted.length();
+  const char* const data = characters_wanted.data();
+  for (stringpiece_ssize_type i = 0; i < length; ++i) {
+    table[static_cast<unsigned char>(data[i])] = true;
+  }
+}
+
+stringpiece_ssize_type StringPiece::find_first_of(StringPiece s,
+                                                  size_type pos) const {
+  if (length_ <= 0 || s.length_ <= 0) {
     return npos;
   }
-  // Avoid the cost of LookupTable() for a single-character search.
+  // Avoid the cost of BuildLookupTable() for a single-character search.
   if (s.length_ == 1) return find_first_of(s.ptr_[0], pos);
-  LookupTable tbl(s);
-  for (size_type i = pos; i < length_; ++i) {
-    if (tbl[ptr_[i]]) {
+
+  bool lookup[UCHAR_MAX + 1] = { false };
+  BuildLookupTable(s, lookup);
+  for (stringpiece_ssize_type i = pos; i < length_; ++i) {
+    if (lookup[static_cast<unsigned char>(ptr_[i])]) {
       return i;
     }
   }
   return npos;
 }
 
-string_view::size_type string_view::find_first_not_of(string_view s,
-                                                      size_type pos) const
-    noexcept {
-  if (empty()) return npos;
-  // Avoid the cost of LookupTable() for a single-character search.
+stringpiece_ssize_type StringPiece::find_first_not_of(StringPiece s,
+                                                      size_type pos) const {
+  if (length_ <= 0) return npos;
+  if (s.length_ <= 0) return 0;
+  // Avoid the cost of BuildLookupTable() for a single-character search.
   if (s.length_ == 1) return find_first_not_of(s.ptr_[0], pos);
-  LookupTable tbl(s);
-  for (size_type i = pos; i < length_; ++i) {
-    if (!tbl[ptr_[i]]) {
+
+  bool lookup[UCHAR_MAX + 1] = { false };
+  BuildLookupTable(s, lookup);
+  for (stringpiece_ssize_type i = pos; i < length_; ++i) {
+    if (!lookup[static_cast<unsigned char>(ptr_[i])]) {
       return i;
     }
   }
   return npos;
 }
 
-string_view::size_type string_view::find_first_not_of(char c,
-                                                      size_type pos) const
-    noexcept {
-  if (empty()) return npos;
-  for (; pos < length_; ++pos) {
+stringpiece_ssize_type StringPiece::find_first_not_of(char c,
+                                                      size_type pos) const {
+  if (length_ <= 0) return npos;
+
+  for (; pos < static_cast<size_type>(length_); ++pos) {
     if (ptr_[pos] != c) {
       return pos;
     }
   }
   return npos;
 }
 
-string_view::size_type string_view::find_last_of(string_view s,
-                                                 size_type pos) const noexcept {
-  if (empty() || s.empty()) return npos;
-  // Avoid the cost of LookupTable() for a single-character search.
+stringpiece_ssize_type StringPiece::find_last_of(StringPiece s,
+                                                 size_type pos) const {
+  if (length_ <= 0 || s.length_ <= 0) return npos;
+  // Avoid the cost of BuildLookupTable() for a single-character search.
   if (s.length_ == 1) return find_last_of(s.ptr_[0], pos);
-  LookupTable tbl(s);
-  for (size_type i = std::min(pos, length_ - 1);; --i) {
-    if (tbl[ptr_[i]]) {
+
+  bool lookup[UCHAR_MAX + 1] = { false };
+  BuildLookupTable(s, lookup);
+  for (stringpiece_ssize_type i =
+       std::min(pos, static_cast<size_type>(length_ - 1)); i >= 0; --i) {
+    if (lookup[static_cast<unsigned char>(ptr_[i])]) {
       return i;
     }
-    if (i == 0) break;
   }
   return npos;
 }
 
-string_view::size_type string_view::find_last_not_of(string_view s,
-                                                     size_type pos) const
-    noexcept {
-  if (empty()) return npos;
-  size_type i = std::min(pos, length_ - 1);
-  if (s.empty()) return i;
-  // Avoid the cost of LookupTable() for a single-character search.
+stringpiece_ssize_type StringPiece::find_last_not_of(StringPiece s,
+                                                     size_type pos) const {
+  if (length_ <= 0) return npos;
+
+  stringpiece_ssize_type i = std::min(pos, static_cast<size_type>(length_ - 1));
+  if (s.length_ <= 0) return i;
+
+  // Avoid the cost of BuildLookupTable() for a single-character search.
   if (s.length_ == 1) return find_last_not_of(s.ptr_[0], pos);
-  LookupTable tbl(s);
-  for (;; --i) {
-    if (!tbl[ptr_[i]]) {
+
+  bool lookup[UCHAR_MAX + 1] = { false };
+  BuildLookupTable(s, lookup);
+  for (; i >= 0; --i) {
+    if (!lookup[static_cast<unsigned char>(ptr_[i])]) {
       return i;
     }
-    if (i == 0) break;
   }
   return npos;
 }
 
-string_view::size_type string_view::find_last_not_of(char c,
-                                                     size_type pos) const
-    noexcept {
-  if (empty()) return npos;
-  size_type i = std::min(pos, length_ - 1);
-  for (;; --i) {
+stringpiece_ssize_type StringPiece::find_last_not_of(char c,
+                                                     size_type pos) const {
+  if (length_ <= 0) return npos;
+
+  for (stringpiece_ssize_type i =
+       std::min(pos, static_cast<size_type>(length_ - 1)); i >= 0; --i) {
     if (ptr_[i] != c) {
       return i;
     }
-    if (i == 0) break;
   }
   return npos;
 }
 
-// MSVC has non-standard behavior that implicitly creates definitions for static
-// const members. These implicit definitions conflict with explicit out-of-class
-// member definitions that are required by the C++ standard, resulting in
-// LNK1169 "multiply defined" errors at link time. __declspec(selectany) asks
-// MSVC to choose only one definition for the symbol it decorates. See details
-// at http://msdn.microsoft.com/en-us/library/34h23df8(v=vs.100).aspx
-#ifdef _MSC_VER
-#define ABSL_STRING_VIEW_SELECTANY __declspec(selectany)
-#else
-#define ABSL_STRING_VIEW_SELECTANY
-#endif
-
-ABSL_STRING_VIEW_SELECTANY
-constexpr string_view::size_type string_view::npos;
-ABSL_STRING_VIEW_SELECTANY
-constexpr string_view::size_type string_view::kMaxSize;
+StringPiece StringPiece::substr(size_type pos, size_type n) const {
+  if (pos > length_) pos = length_;
+  if (n > length_ - pos) n = length_ - pos;
+  return StringPiece(ptr_ + pos, n);
+}
 
-}  // namespace absl
+const StringPiece::size_type StringPiece::npos = size_type(-1);
 
-#endif  // ABSL_HAVE_STD_STRING_VIEW
+}  // namespace protobuf
+}  // namespace google
```

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/absl/strings/strip.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/absl/strings/strip.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/darts_clone/darts.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/darts_clone/darts.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/arena.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arena.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/arenastring.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/arenastring.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/bytestream.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/bytestream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/coded_stream.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/coded_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/common.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/common.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/extension_set.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/extension_set.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_enum_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_table_driven_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/generated_message_util.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/generated_message_util.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/any.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arena_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/arenastring.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/descriptor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/extension_set_inl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_reflection.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_enum_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_table_driven_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/generated_message_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/has_bits.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/implicit_weak_message.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/coded_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/io_win32.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/io/zero_copy_stream_impl_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_entry_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_field_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/map_type_handler.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/message_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/metadata_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/parse_context.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_def.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/port_undef.inc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/repeated_field.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/bytestream.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/callback.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/common.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/hash.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/int128.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/logging.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/map_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/mutex.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/once.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/platform_macros.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/port.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/status.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/statusor.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stl_util.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringpiece.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/stringprintf.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/strutil.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/stubs/time.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/unknown_field_set.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/google/protobuf/wire_format_lite.h`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/implicit_weak_message.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/int128.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/int128.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/io_win32.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/io_win32.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/message_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/message_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/parse_context.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/parse_context.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/repeated_field.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/repeated_field.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/status.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/status.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/statusor.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/statusor.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/stringprintf.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/stringprintf.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/structurally_valid.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/structurally_valid.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/strutil.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/strutil.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/time.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/time.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/wire_format_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc` & `curated-tokenizers-0.9.0.dev0/sentencepiece/third_party/protobuf-lite/zero_copy_stream_impl_lite.cc`

 * *Files identical despite different names*

### Comparing `curated-tokenizers-0.0.8/setup.cfg` & `curated-tokenizers-0.9.0.dev0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 description = Lightweight piece tokenization library
-version = 0.0.8
+version = 0.9.0.dev0
 url = https://github.com/explosion/curated-tokenizers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `curated-tokenizers-0.0.8/setup.py` & `curated-tokenizers-0.9.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def prefix_path(prefix, files):
     return list(map(lambda f: f"{prefix}/{f}", files))
 
 
 ABSL_SRC = prefix_path(
-    "sentencepiece/third_party/absl", ["flags/flag.cc", "strings/string_view.cc"]
+    "sentencepiece/third_party/absl", ["flags/flag.cc"]
 )
 
 PROTOBUF_LIGHT_SRC = prefix_path(
     "sentencepiece/third_party/protobuf-lite",
     [
         "arena.cc",
         "arenastring.cc",
@@ -76,26 +76,25 @@
 
 PACKAGES = find_packages()
 MOD_NAMES = [
     "curated_tokenizers.sp",
 ]
 COMPILE_OPTIONS = {
     "msvc": [
+        "/std:c++17",
         "/Ox",
         "/EHsc",
-        "/D_USE_INTERNAL_STRING_VIEW",
         "/DHAVE_PTHREAD",
         "/wd4018",
         "/wd4514",
     ],
     "other": [
-        "--std=c++14",
+        "--std=c++17",
         "-Wno-sign-compare" "-Wno-strict-prototypes",
         "-Wno-unused-function",
-        "-D_USE_INTERNAL_STRING_VIEW",
         "-pthread",
         "-DHAVE_PTHREAD=1",
     ],
 }
 COMPILER_DIRECTIVES = {
     "language_level": -3,
     "embedsignature": True,
```

