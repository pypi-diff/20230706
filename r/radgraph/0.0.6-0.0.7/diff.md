# Comparing `tmp/radgraph-0.0.6.tar.gz` & `tmp/radgraph-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radgraph-0.0.6.tar", last modified: Thu Jul  6 18:19:08 2023, max compression
+gzip compressed data, was "radgraph-0.0.7.tar", last modified: Thu Jul  6 18:56:58 2023, max compression
```

## Comparing `radgraph-0.0.6.tar` & `radgraph-0.0.7.tar`

### file list

```diff
@@ -1,508 +1,516 @@
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.907177 radgraph-0.0.6/
--rw-rw-r--   0 jb        (1000) jb        (1000)      296 2023-07-06 18:19:08.907177 radgraph-0.0.6/PKG-INFO
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.791176 radgraph-0.0.6/radgraph/
--rw-rw-r--   0 jb        (1000) jb        (1000)       64 2023-01-26 00:23:15.000000 radgraph-0.0.6/radgraph/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.795176 radgraph-0.0.6/radgraph/allennlp/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1004 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1050 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/__main__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.795176 radgraph-0.0.6/radgraph/allennlp/commands/
--rw-rw-r--   0 jb        (1000) jb        (1000)     3489 2023-01-26 00:32:33.000000 radgraph-0.0.6/radgraph/allennlp/commands/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6057 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/commands/evaluate.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11792 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/commands/find_learning_rate.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6781 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/commands/predict.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2404 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/commands/print_results.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1562 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/commands/subcommand.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1654 2023-01-26 00:30:27.000000 radgraph-0.0.6/radgraph/allennlp/commands/test_install.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    29980 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/commands/train.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.799176 radgraph-0.0.6/radgraph/allennlp/common/
--rw-rw-r--   0 jb        (1000) jb        (1000)      317 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3789 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/common/cached_transformers.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4534 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/common/checks.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    17418 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/file_utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    26059 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/from_params.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2007 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/common/lazy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4142 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/logging.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    22764 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/params.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1933 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/plugins.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8827 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/common/registrable.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.803176 radgraph-0.0.6/radgraph/allennlp/common/testing/
--rw-rw-r--   0 jb        (1000) jb        (1000)     2879 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/common/testing/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2137 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/testing/distributed_test.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    18298 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/common/testing/model_test_case.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2111 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/common/testing/test_case.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2963 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/common/tqdm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    20863 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/common/util.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.803176 radgraph-0.0.6/radgraph/allennlp/data/
--rw-rw-r--   0 jb        (1000) jb        (1000)      806 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9251 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/batch.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6469 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/dataloader.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.807176 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      986 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3807 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/babi.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8559 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/conll2003.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21040 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/dataset_reader.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.807176 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/dataset_utils/
--rw-rw-r--   0 jb        (1000) jb        (1000)      382 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/dataset_utils/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    17332 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/dataset_utils/span_utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4133 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/interleaving_dataset_reader.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3557 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/sequence_tagging.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3694 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/sharded_dataset_reader.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5730 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/text_classification_json.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.811176 radgraph-0.0.6/radgraph/allennlp/data/fields/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1085 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6455 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/adjacency_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2579 2023-07-06 18:16:16.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/array_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6798 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1284 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/flag_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2392 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/index_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4907 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/label_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5263 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/list_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2276 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/metadata_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6328 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/multilabel_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2013 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/namespace_swapping_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      762 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/sequence_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6202 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/sequence_label_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2760 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/span_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7601 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/fields/text_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4614 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/instance.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.811176 radgraph-0.0.6/radgraph/allennlp/data/samplers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      380 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/samplers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7388 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/samplers/bucket_batch_sampler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4626 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/samplers/max_tokens_batch_sampler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5511 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/samplers/samplers.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.815176 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      796 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6035 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/elmo_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10015 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/pretrained_transformer_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5300 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/pretrained_transformer_mismatched_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4905 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/single_id_token_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2444 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/spacy_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6913 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/token_characters_indexer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6317 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/token_indexers/token_indexer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.819177 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      682 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3557 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/character_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      768 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/letters_digits_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19293 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/pretrained_transformer_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2659 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/sentence_splitter.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5808 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/spacy_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3897 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/token.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2786 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      883 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/tokenizers/whitespace_tokenizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    37515 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/data/vocabulary.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.819177 radgraph-0.0.6/radgraph/allennlp/interpret/
--rw-rw-r--   0 jb        (1000) jb        (1000)      171 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.819177 radgraph-0.0.6/radgraph/allennlp/interpret/attackers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      215 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/attackers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2297 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/attackers/attacker.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19914 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/interpret/attackers/hotflip.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9518 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/interpret/attackers/input_reduction.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1948 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/attackers/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.823176 radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/
--rw-rw-r--   0 jb        (1000) jb        (1000)      390 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3929 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/integrated_gradient.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1225 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/saliency_interpreter.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2919 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/simple_gradient.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3300 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/smooth_gradient.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.823176 radgraph-0.0.6/radgraph/allennlp/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      373 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7543 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/models/archival.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7218 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/models/basic_classifier.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19981 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/models/model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9653 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/models/simple_tagger.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.831177 radgraph-0.0.6/radgraph/allennlp/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1427 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.831177 radgraph-0.0.6/radgraph/allennlp/modules/attention/
--rw-rw-r--   0 jb        (1000) jb        (1000)      490 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/attention/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2366 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/attention/additive_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1758 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/attention/attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2394 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/attention/bilinear_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      821 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/attention/cosine_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      504 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/attention/dot_product_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3380 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/attention/linear_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21594 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/augmented_lstm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15821 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/bimpm_matching.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    17960 2023-01-26 00:30:27.000000 radgraph-0.0.6/radgraph/allennlp/modules/conditional_random_field.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    29111 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/elmo.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15141 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/elmo_lstm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16852 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/encoder_base.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4192 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/feedforward.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1355 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/gated_sum.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2682 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/modules/highway.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1245 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/modules/input_variational_dropout.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1124 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/layer_norm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12242 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/lstm_cell_with_projection.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1082 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/masked_layer_norm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.835177 radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/
--rw-rw-r--   0 jb        (1000) jb        (1000)      505 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3461 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/bilinear_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      878 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/cosine_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      573 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/dot_product_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3405 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/linear_matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      821 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/matrix_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3872 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/maxout.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2506 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/modules/residual_with_layer_dropout.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11387 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/sampled_softmax_loss.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3813 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/scalar_mix.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.835177 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1926 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2449 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/compose_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1480 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/feedforward_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8201 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/gated_cnn_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1607 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/pass_through_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10679 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4674 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/pytorch_transformer_wrapper.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1592 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/seq2seq_encoder.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.839177 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1532 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2697 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/bert_pooler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2368 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/boe_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2256 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/cls_pooler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5951 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/cnn_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6031 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/cnn_highway_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10218 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/pytorch_seq2vec_wrapper.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1233 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/seq2vec_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1126 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/modules/softmax_loss.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.839177 radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      439 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12617 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/bidirectional_endpoint_span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7855 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/endpoint_span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3320 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/self_attentive_span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2711 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/span_extractor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4980 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/stacked_alternating_lstm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6486 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/stacked_bidirectional_lstm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.843177 radgraph-0.0.6/radgraph/allennlp/modules/text_field_embedders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      401 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/text_field_embedders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4541 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/text_field_embedders/basic_text_field_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2538 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/text_field_embedders/text_field_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2594 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/modules/time_distributed.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.843177 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1026 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3287 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/bag_of_word_counts_token_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4727 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/elmo_token_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    29421 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/embedding.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      902 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/empty_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      665 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/pass_through_token_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15258 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/pretrained_transformer_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4731 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/pretrained_transformer_mismatched_embedder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1690 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/token_characters_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1388 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/token_embedder.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.847177 radgraph-0.0.6/radgraph/allennlp/nn/
--rw-rw-r--   0 jb        (1000) jb        (1000)      205 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/nn/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4288 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/nn/activations.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16352 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/nn/beam_search.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10292 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/nn/chu_liu_edmonds.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    19804 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/nn/initializers.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.847177 radgraph-0.0.6/radgraph/allennlp/nn/regularizers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      443 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/nn/regularizers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      353 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/nn/regularizers/regularizer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1495 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/nn/regularizers/regularizer_applicator.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      938 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/nn/regularizers/regularizers.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    87249 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/nn/util.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.851177 radgraph-0.0.6/radgraph/allennlp/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      466 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13306 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/predictors/predictor.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4376 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/predictors/sentence_tagger.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1848 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/predictors/text_classifier.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.851177 radgraph-0.0.6/radgraph/allennlp/tools/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/tools/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2666 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/tools/archive_surgery.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5224 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/tools/create_elmo_embeddings_from_vocab.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      800 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/tools/inspect_cache.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.855177 radgraph-0.0.6/radgraph/allennlp/training/
--rw-rw-r--   0 jb        (1000) jb        (1000)      360 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10830 2023-01-26 00:30:27.000000 radgraph-0.0.6/radgraph/allennlp/training/checkpointer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.855177 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1646 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3065 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/cosine.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4615 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/learning_rate_scheduler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      976 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/linear_with_warmup.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2250 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/noam.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2745 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/polynomial_decay.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7778 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/slanted_triangular.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5815 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metric_tracker.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.859177 radgraph-0.0.6/radgraph/allennlp/training/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)     1693 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5627 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/attachment_scores.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4933 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/auc.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1820 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/average.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7350 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/bleu.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4669 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/boolean_accuracy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5004 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/categorical_accuracy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5996 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/covariance.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2032 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/entropy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8168 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/evalb_bracketing_scorer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2891 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/f1_measure.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10767 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/fbeta_measure.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2336 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/mean_absolute_error.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1764 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/metric.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3614 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/pearson_correlation.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      871 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/perplexity.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8925 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/rouge.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3544 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/sequence_accuracy.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13426 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/span_based_f1_measure.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4290 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/spearman_correlation.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3781 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/metrics/unigram_recall.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.859177 radgraph-0.0.6/radgraph/allennlp/training/momentum_schedulers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      194 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/momentum_schedulers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1660 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/momentum_schedulers/inverted_triangular.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      402 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/momentum_schedulers/momentum_scheduler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3708 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/moving_average.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1304 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/no_op_trainer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    22085 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/optimizers.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3085 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/training/scheduler.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15108 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/tensorboard_writer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    51003 2023-01-26 00:26:42.000000 radgraph-0.0.6/radgraph/allennlp/training/trainer.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    18644 2023-01-26 00:26:43.000000 radgraph-0.0.6/radgraph/allennlp/training/util.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      463 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp/version.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.863177 radgraph-0.0.6/radgraph/allennlp_models/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.863177 radgraph-0.0.6/radgraph/allennlp_models/classification/
--rw-rw-r--   0 jb        (1000) jb        (1000)      152 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/classification/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.863177 radgraph-0.0.6/radgraph/allennlp_models/classification/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      145 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/classification/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6504 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/classification/dataset_readers/stanford_sentiment_tree_bank.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.863177 radgraph-0.0.6/radgraph/allennlp_models/classification/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      136 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/classification/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    15361 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/classification/models/biattentive_classification_network.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.863177 radgraph-0.0.6/radgraph/allennlp_models/common/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/common/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10125 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/common/model_card.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    20667 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/common/ontonotes.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.863177 radgraph-0.0.6/radgraph/allennlp_models/coref/
--rw-rw-r--   0 jb        (1000) jb        (1000)      500 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.867177 radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5023 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/conll.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4892 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/preco.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7115 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/winobias.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.867177 radgraph-0.0.6/radgraph/allennlp_models/coref/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8992 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/metrics/conll_coref_scores.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2126 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/metrics/mention_recall.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.867177 radgraph-0.0.6/radgraph/allennlp_models/coref/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       76 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    42732 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/models/coref.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.867177 radgraph-0.0.6/radgraph/allennlp_models/coref/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8073 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/predictors/coref.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8765 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/coref/util.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.867177 radgraph-0.0.6/radgraph/allennlp_models/generation/
--rw-rw-r--   0 jb        (1000) jb        (1000)      263 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.867177 radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      291 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6706 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/cnn_dm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8978 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/copynet_seq2seq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7208 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/seq2seq.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.871177 radgraph-0.0.6/radgraph/allennlp_models/generation/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      323 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16131 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/models/bart.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6970 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/models/composed_seq2seq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    45985 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/models/copynet_seq2seq.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    25833 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/models/simple_seq2seq.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.871177 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)      163 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.871177 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/
--rw-rw-r--   0 jb        (1000) jb        (1000)      322 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3836 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/decoder_net.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5516 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/lstm_cell.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6710 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/stacked_self_attention.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.871177 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/seq_decoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      202 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/seq_decoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21696 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/seq_decoders/auto_regressive.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2834 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/modules/seq_decoders/seq_decoder.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.871177 radgraph-0.0.6/radgraph/allennlp_models/generation/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       84 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      913 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/generation/predictors/seq2seq.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.871177 radgraph-0.0.6/radgraph/allennlp_models/lm/
--rw-rw-r--   0 jb        (1000) jb        (1000)      231 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.871177 radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      321 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6091 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/masked_language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4315 2023-01-26 00:29:26.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/next_token_lm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3937 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/simple_language_modeling.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.875177 radgraph-0.0.6/radgraph/allennlp_models/lm/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      329 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2646 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/models/bidirectional_lm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13771 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/models/language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7757 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/models/masked_language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6074 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/models/next_token_lm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.875177 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)      225 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.875177 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/
--rw-rw-r--   0 jb        (1000) jb        (1000)      399 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1511 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/bert.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1515 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/gpt2.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      514 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/language_model_head.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1325 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/linear.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.875177 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/seq2seq_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      141 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/seq2seq_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11077 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/seq2seq_encoders/bidirectional_lm_transformer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.879177 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/token_embedders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      236 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/token_embedders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2407 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/token_embedders/bidirectional_lm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8866 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/modules/token_embedders/language_model.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.879177 radgraph-0.0.6/radgraph/allennlp_models/lm/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      188 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1336 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/predictors/masked_language_model.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1415 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/lm/predictors/next_token_lm.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.879177 radgraph-0.0.6/radgraph/allennlp_models/mc/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.879177 radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      234 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1160 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/commonsenseqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3089 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/fake.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1536 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/piqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      985 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/swag.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3170 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/transformer_mc.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.879177 radgraph-0.0.6/radgraph/allennlp_models/mc/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       76 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4747 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/models/transformer_mc.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.879177 radgraph-0.0.6/radgraph/allennlp_models/mc/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       89 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      762 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/mc/predictors/transformer_mc.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.879177 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/
--rw-rw-r--   0 jb        (1000) jb        (1000)      232 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.883177 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      217 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3919 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/dataset_readers/quora_paraphrase.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5100 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/dataset_readers/snli.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.883177 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      259 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9545 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/bimpm.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9489 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/decomposable_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9607 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/esim.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.883177 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      123 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1991 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/pair_classification/predictors/textual_entailment.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2249 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/pretrained.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.883177 radgraph-0.0.6/radgraph/allennlp_models/rc/
--rw-rw-r--   0 jb        (1000) jb        (1000)      231 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.887177 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      475 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    27674 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/drop.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3727 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/qangaroo.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6830 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/quac.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7626 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/squad.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12559 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/transformer_squad.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7795 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/triviaqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    22635 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.887177 radgraph-0.0.6/radgraph/allennlp_models/rc/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)      152 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3420 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/metrics/drop_em_and_f1.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2752 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/metrics/squad_em_and_f1.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.887177 radgraph-0.0.6/radgraph/allennlp_models/rc/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      505 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    18758 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/bidaf.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7852 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/bidaf_ensemble.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    27475 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/dialog_qa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    33059 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/naqanet.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13990 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/qanet.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11569 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/transformer_qa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2158 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/models/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.887177 radgraph-0.0.6/radgraph/allennlp_models/rc/modules/
--rw-rw-r--   0 jb        (1000) jb        (1000)       88 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/modules/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.891177 radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/
--rw-rw-r--   0 jb        (1000) jb        (1000)      340 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7416 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/multi_head_self_attention.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11445 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/qanet_encoder.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7569 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/stacked_self_attention.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.891177 radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      255 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6111 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/bidaf.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2833 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/dialog_qa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4127 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/transformer_qa.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.895177 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10682 2023-01-25 23:16:54.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/drop.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2518 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/narrativeqa.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3689 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/orb.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4432 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/orb_utils.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4839 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/quoref.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3430 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/squad.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1919 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/squad2.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3413 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/rc/tools/transformer_qa.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.895177 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/
--rw-rw-r--   0 jb        (1000) jb        (1000)      307 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.895177 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      512 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    10608 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/penn_tree_bank.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4857 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/semantic_dependencies.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    11873 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/srl.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5028 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/universal_dependencies.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.895177 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/metrics/
--rw-rw-r--   0 jb        (1000) jb        (1000)       97 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/metrics/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7679 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/metrics/srl_eval_scorer.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.895177 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)      500 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    31340 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/biaffine_dependency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    22082 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/constituency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16277 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/graph_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21086 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/srl.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13522 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/srl_bert.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.899177 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)      463 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7184 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/biaffine_dependency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5827 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/constituency_parser.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8448 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/openie.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9135 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/srl.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.899177 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/tools/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/tools/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8474 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/tools/convert_openie_to_conll.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     4358 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/tools/write_srl_predictions_to_conll_format.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.899177 radgraph-0.0.6/radgraph/allennlp_models/tagging/
--rw-rw-r--   0 jb        (1000) jb        (1000)      196 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.899177 radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)      385 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9162 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/ccgbank.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7067 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/conll2000.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      175 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/conll2003.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5085 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/ontonotes_ner.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.899177 radgraph-0.0.6/radgraph/allennlp_models/tagging/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       73 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    13020 2023-01-26 00:30:27.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/models/crf_tagger.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.903177 radgraph-0.0.6/radgraph/allennlp_models/tagging/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       96 2023-01-26 00:31:08.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      172 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/allennlp_models/tagging/predictors/sentence_tagger.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      373 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/allennlp_models/version.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.903177 radgraph-0.0.6/radgraph/dygie/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/dygie/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.903177 radgraph-0.0.6/radgraph/dygie/data/
--rw-rw-r--   0 jb        (1000) jb        (1000)      132 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/data/__init__.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.903177 radgraph-0.0.6/radgraph/dygie/data/dataset_readers/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/dygie/data/dataset_readers/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    25839 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/data/dataset_readers/document.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8663 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/data/dataset_readers/dygie.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.903177 radgraph-0.0.6/radgraph/dygie/data/fields/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/dygie/data/fields/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6466 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/dygie/data/fields/adjacency_field_assym.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.907177 radgraph-0.0.6/radgraph/dygie/models/
--rw-rw-r--   0 jb        (1000) jb        (1000)       46 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/models/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    37379 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/models/coref.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    16832 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/models/dygie.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     9395 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/dygie/models/entity_beam_pruner.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    21834 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/models/events.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     7329 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/models/ner.py
--rw-rw-r--   0 jb        (1000) jb        (1000)    12335 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/models/relation.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2131 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/dygie/models/shared.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.907177 radgraph-0.0.6/radgraph/dygie/predictors/
--rw-rw-r--   0 jb        (1000) jb        (1000)       59 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/predictors/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2616 2023-01-26 00:29:27.000000 radgraph-0.0.6/radgraph/dygie/predictors/dygie.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.907177 radgraph-0.0.6/radgraph/dygie/training/
--rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/dygie/training/__init__.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     6749 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/training/event_metrics.py
--rw-rw-r--   0 jb        (1000) jb        (1000)      360 2023-01-06 19:33:15.000000 radgraph-0.0.6/radgraph/dygie/training/f1.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     2227 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/training/ner_metrics.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     1533 2023-01-26 00:31:53.000000 radgraph-0.0.6/radgraph/dygie/training/relation_metrics.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     8722 2023-01-26 00:37:57.000000 radgraph-0.0.6/radgraph/radgraph.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     5268 2023-01-25 22:37:36.000000 radgraph-0.0.6/radgraph/rewards.py
--rw-rw-r--   0 jb        (1000) jb        (1000)     3702 2023-01-26 00:23:33.000000 radgraph-0.0.6/radgraph/utils.py
-drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:19:08.791176 radgraph-0.0.6/radgraph.egg-info/
--rw-rw-r--   0 jb        (1000) jb        (1000)      296 2023-07-06 18:19:08.000000 radgraph-0.0.6/radgraph.egg-info/PKG-INFO
--rw-rw-r--   0 jb        (1000) jb        (1000)    22173 2023-07-06 18:19:08.000000 radgraph-0.0.6/radgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-07-06 18:19:08.000000 radgraph-0.0.6/radgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-07-06 18:19:08.000000 radgraph-0.0.6/radgraph.egg-info/not-zip-safe
--rw-rw-r--   0 jb        (1000) jb        (1000)       95 2023-07-06 18:19:08.000000 radgraph-0.0.6/radgraph.egg-info/requires.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)        9 2023-07-06 18:19:08.000000 radgraph-0.0.6/radgraph.egg-info/top_level.txt
--rw-rw-r--   0 jb        (1000) jb        (1000)       38 2023-07-06 18:19:08.907177 radgraph-0.0.6/setup.cfg
--rw-rw-r--   0 jb        (1000) jb        (1000)      792 2023-07-06 18:12:52.000000 radgraph-0.0.6/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.427632 radgraph-0.0.7/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      296 2023-07-06 18:56:58.423632 radgraph-0.0.7/PKG-INFO
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.263630 radgraph-0.0.7/overrides_/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      171 2023-07-06 18:55:38.000000 radgraph-0.0.7/overrides_/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1623 2023-07-06 18:50:18.000000 radgraph-0.0.7/overrides_/enforce.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1505 2023-07-06 18:50:18.000000 radgraph-0.0.7/overrides_/final.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4696 2023-07-06 18:55:11.000000 radgraph-0.0.7/overrides_/overrides.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.267631 radgraph-0.0.7/radgraph/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       64 2023-01-26 00:23:15.000000 radgraph-0.0.7/radgraph/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.267631 radgraph-0.0.7/radgraph/allennlp/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1004 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1050 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/__main__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.271631 radgraph-0.0.7/radgraph/allennlp/commands/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3490 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/commands/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6058 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/commands/evaluate.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    11793 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/commands/find_learning_rate.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6782 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/commands/predict.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2405 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/commands/print_results.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1563 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/commands/subcommand.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1655 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/commands/test_install.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    29981 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/commands/train.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.271631 radgraph-0.0.7/radgraph/allennlp/common/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      317 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/common/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3789 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/common/cached_transformers.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4534 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/common/checks.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    17418 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/common/file_utils.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    26059 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/common/from_params.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2007 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/common/lazy.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4142 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/common/logging.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    22765 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/common/params.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1933 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/common/plugins.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8827 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/common/registrable.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.271631 radgraph-0.0.7/radgraph/allennlp/common/testing/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2879 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/common/testing/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2137 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/common/testing/distributed_test.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    18298 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/common/testing/model_test_case.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2111 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/common/testing/test_case.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2963 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/common/tqdm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    20863 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/common/util.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.275631 radgraph-0.0.7/radgraph/allennlp/data/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      806 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9251 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/batch.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6469 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/dataloader.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.275631 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      986 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3808 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/babi.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8560 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/conll2003.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    21040 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/dataset_reader.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.275631 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/dataset_utils/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      382 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/dataset_utils/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    17332 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/dataset_utils/span_utils.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4133 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/interleaving_dataset_reader.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3558 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/sequence_tagging.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3694 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/sharded_dataset_reader.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5731 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/text_classification_json.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.283631 radgraph-0.0.7/radgraph/allennlp/data/fields/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1085 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6456 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/adjacency_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2580 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/array_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6798 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1285 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/flag_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2393 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/index_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4908 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/label_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5264 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/list_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2277 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/metadata_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6329 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/multilabel_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2014 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/namespace_swapping_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      762 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/sequence_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6203 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/sequence_label_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2761 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/span_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7602 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/fields/text_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4614 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/instance.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.287631 radgraph-0.0.7/radgraph/allennlp/data/samplers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      380 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/samplers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7388 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/data/samplers/bucket_batch_sampler.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4626 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/samplers/max_tokens_batch_sampler.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5511 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/samplers/samplers.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.291631 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      796 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6036 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/elmo_indexer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10016 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/pretrained_transformer_indexer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5301 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/pretrained_transformer_mismatched_indexer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4906 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/single_id_token_indexer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2445 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/spacy_indexer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6914 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/token_characters_indexer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6317 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/token_indexers/token_indexer.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.299631 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      682 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3558 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/character_tokenizer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      769 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/letters_digits_tokenizer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    19294 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/pretrained_transformer_tokenizer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2660 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/sentence_splitter.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5809 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/spacy_tokenizer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3897 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/token.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2786 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/tokenizer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      884 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/data/tokenizers/whitespace_tokenizer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    37515 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/data/vocabulary.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.299631 radgraph-0.0.7/radgraph/allennlp/interpret/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      171 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.303631 radgraph-0.0.7/radgraph/allennlp/interpret/attackers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      215 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/attackers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2297 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/attackers/attacker.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    19914 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/interpret/attackers/hotflip.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9518 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/interpret/attackers/input_reduction.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1948 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/attackers/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.303631 radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      390 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3929 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/integrated_gradient.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1225 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/saliency_interpreter.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2919 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/simple_gradient.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3300 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/smooth_gradient.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.303631 radgraph-0.0.7/radgraph/allennlp/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      373 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7543 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/models/archival.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7219 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/models/basic_classifier.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    19981 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/models/model.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9654 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/models/simple_tagger.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.311631 radgraph-0.0.7/radgraph/allennlp/modules/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1427 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.315631 radgraph-0.0.7/radgraph/allennlp/modules/attention/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      490 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/attention/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2367 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/attention/additive_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1759 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/attention/attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2395 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/attention/bilinear_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      822 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/attention/cosine_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      505 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/attention/dot_product_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3381 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/attention/linear_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    21594 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/augmented_lstm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    15821 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/bimpm_matching.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    17960 2023-01-26 00:30:27.000000 radgraph-0.0.7/radgraph/allennlp/modules/conditional_random_field.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    29112 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/elmo.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    15141 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/elmo_lstm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    16852 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/encoder_base.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4192 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/feedforward.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1355 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/gated_sum.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2683 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/highway.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1245 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/modules/input_variational_dropout.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1124 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/layer_norm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    12242 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/lstm_cell_with_projection.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1082 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/masked_layer_norm.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.315631 radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      505 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3462 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/bilinear_matrix_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      879 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/cosine_matrix_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      574 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/dot_product_matrix_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3406 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/linear_matrix_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      821 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/matrix_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3872 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/maxout.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2506 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/modules/residual_with_layer_dropout.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    11387 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/sampled_softmax_loss.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3813 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/scalar_mix.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.319631 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1926 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2450 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/compose_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1481 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/feedforward_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8201 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/gated_cnn_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1608 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/pass_through_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10680 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4675 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/pytorch_transformer_wrapper.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1592 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/seq2seq_encoder.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.323631 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1532 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2698 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/bert_pooler.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2369 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/boe_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2257 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/cls_pooler.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5952 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/cnn_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6031 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/cnn_highway_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10218 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/pytorch_seq2vec_wrapper.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1233 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/seq2vec_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1126 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/modules/softmax_loss.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.323631 radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      439 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    12618 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/bidirectional_endpoint_span_extractor.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7856 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/endpoint_span_extractor.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3321 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/self_attentive_span_extractor.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2712 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/span_extractor.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4980 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/stacked_alternating_lstm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6486 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/stacked_bidirectional_lstm.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.327631 radgraph-0.0.7/radgraph/allennlp/modules/text_field_embedders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      401 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/text_field_embedders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4542 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/text_field_embedders/basic_text_field_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2538 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/text_field_embedders/text_field_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2595 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/time_distributed.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.331631 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1026 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3287 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/bag_of_word_counts_token_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4727 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/elmo_token_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    29422 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/embedding.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      902 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/empty_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      665 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/pass_through_token_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    15259 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/pretrained_transformer_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4732 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/pretrained_transformer_mismatched_embedder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1690 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/token_characters_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1388 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/token_embedder.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.331631 radgraph-0.0.7/radgraph/allennlp/nn/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      205 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/nn/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4289 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/nn/activations.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    16352 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/nn/beam_search.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10292 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/nn/chu_liu_edmonds.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    19805 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/nn/initializers.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.331631 radgraph-0.0.7/radgraph/allennlp/nn/regularizers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      443 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/nn/regularizers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      353 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/nn/regularizers/regularizer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1495 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/nn/regularizers/regularizer_applicator.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      938 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/nn/regularizers/regularizers.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    87249 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/nn/util.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.335631 radgraph-0.0.7/radgraph/allennlp/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      466 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13306 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/predictors/predictor.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4377 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/predictors/sentence_tagger.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1849 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/predictors/text_classifier.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.335631 radgraph-0.0.7/radgraph/allennlp/tools/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/tools/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2666 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/tools/archive_surgery.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5224 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/tools/create_elmo_embeddings_from_vocab.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      800 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/tools/inspect_cache.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.339631 radgraph-0.0.7/radgraph/allennlp/training/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      360 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10830 2023-01-26 00:30:27.000000 radgraph-0.0.7/radgraph/allennlp/training/checkpointer.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.343631 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1646 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3066 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/cosine.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4616 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/learning_rate_scheduler.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      976 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/linear_with_warmup.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2251 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/noam.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2746 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/polynomial_decay.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7779 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/slanted_triangular.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5815 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/metric_tracker.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.351631 radgraph-0.0.7/radgraph/allennlp/training/metrics/
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1693 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5628 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/attachment_scores.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4934 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/auc.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1821 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/average.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7351 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/bleu.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4670 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/boolean_accuracy.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5005 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/categorical_accuracy.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5997 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/covariance.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2033 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/entropy.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8169 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/evalb_bracketing_scorer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2891 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/f1_measure.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10768 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/fbeta_measure.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2337 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/mean_absolute_error.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1764 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/metric.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3615 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/pearson_correlation.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      872 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/perplexity.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8926 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/rouge.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3545 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/sequence_accuracy.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13426 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/span_based_f1_measure.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4291 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/spearman_correlation.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3782 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp/training/metrics/unigram_recall.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.351631 radgraph-0.0.7/radgraph/allennlp/training/momentum_schedulers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      194 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/momentum_schedulers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1660 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/momentum_schedulers/inverted_triangular.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      402 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/momentum_schedulers/momentum_scheduler.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3708 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/moving_average.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1304 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/no_op_trainer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    22085 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/optimizers.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3085 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/training/scheduler.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    15108 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/tensorboard_writer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    51003 2023-01-26 00:26:42.000000 radgraph-0.0.7/radgraph/allennlp/training/trainer.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    18644 2023-01-26 00:26:43.000000 radgraph-0.0.7/radgraph/allennlp/training/util.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      463 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp/version.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.351631 radgraph-0.0.7/radgraph/allennlp_models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.351631 radgraph-0.0.7/radgraph/allennlp_models/classification/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      152 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/classification/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.355631 radgraph-0.0.7/radgraph/allennlp_models/classification/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      145 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/classification/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6505 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/classification/dataset_readers/stanford_sentiment_tree_bank.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.355631 radgraph-0.0.7/radgraph/allennlp_models/classification/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      136 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/classification/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    15362 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/classification/models/biattentive_classification_network.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.355631 radgraph-0.0.7/radgraph/allennlp_models/common/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/common/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10125 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/common/model_card.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    20667 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/common/ontonotes.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.355631 radgraph-0.0.7/radgraph/allennlp_models/coref/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      500 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.355631 radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5024 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/conll.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4893 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/preco.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7116 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/winobias.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.359631 radgraph-0.0.7/radgraph/allennlp_models/coref/metrics/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/metrics/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8993 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/metrics/conll_coref_scores.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2127 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/metrics/mention_recall.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.359631 radgraph-0.0.7/radgraph/allennlp_models/coref/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       76 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    42733 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/models/coref.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.359631 radgraph-0.0.7/radgraph/allennlp_models/coref/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8074 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/predictors/coref.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8765 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/coref/util.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.359631 radgraph-0.0.7/radgraph/allennlp_models/generation/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      263 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.363631 radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      291 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6707 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/cnn_dm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8979 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/copynet_seq2seq.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7209 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/seq2seq.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.367631 radgraph-0.0.7/radgraph/allennlp_models/generation/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      323 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    16132 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/models/bart.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6971 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/models/composed_seq2seq.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    45986 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/models/copynet_seq2seq.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    25834 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/models/simple_seq2seq.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.367631 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      163 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.367631 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      322 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3836 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/decoder_net.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5517 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/lstm_cell.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6711 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/stacked_self_attention.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.367631 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/seq_decoders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      202 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/seq_decoders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    21697 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/seq_decoders/auto_regressive.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2834 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/modules/seq_decoders/seq_decoder.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.371631 radgraph-0.0.7/radgraph/allennlp_models/generation/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       84 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      914 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/generation/predictors/seq2seq.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.371631 radgraph-0.0.7/radgraph/allennlp_models/lm/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      231 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.371631 radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      321 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6092 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/masked_language_model.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4316 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/next_token_lm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3938 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/simple_language_modeling.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.371631 radgraph-0.0.7/radgraph/allennlp_models/lm/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      329 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2646 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/models/bidirectional_lm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13771 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/models/language_model.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7758 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/models/masked_language_model.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6075 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/models/next_token_lm.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.375631 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      225 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.375631 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      399 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1512 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/bert.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1516 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/gpt2.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      514 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/language_model_head.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1326 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/linear.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.375631 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/seq2seq_encoders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      141 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/seq2seq_encoders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    11077 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/seq2seq_encoders/bidirectional_lm_transformer.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.375631 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/token_embedders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      236 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/token_embedders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2407 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/token_embedders/bidirectional_lm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8866 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/modules/token_embedders/language_model.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.379631 radgraph-0.0.7/radgraph/allennlp_models/lm/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      188 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1337 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/predictors/masked_language_model.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1416 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/lm/predictors/next_token_lm.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.379631 radgraph-0.0.7/radgraph/allennlp_models/mc/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.379631 radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      234 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1161 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/commonsenseqa.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3090 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/fake.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1537 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/piqa.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      986 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/swag.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3171 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/transformer_mc.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.379631 radgraph-0.0.7/radgraph/allennlp_models/mc/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       76 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4747 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/models/transformer_mc.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.383632 radgraph-0.0.7/radgraph/allennlp_models/mc/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       89 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      763 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/mc/predictors/transformer_mc.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.383632 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      232 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.383632 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      217 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3920 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/dataset_readers/quora_paraphrase.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5101 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/dataset_readers/snli.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.383632 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      259 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9546 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/bimpm.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9489 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/decomposable_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9607 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/esim.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.383632 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      123 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1992 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/pair_classification/predictors/textual_entailment.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2249 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/pretrained.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.387632 radgraph-0.0.7/radgraph/allennlp_models/rc/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      231 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.391631 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      475 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    27675 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/drop.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3728 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/qangaroo.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6831 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/quac.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7627 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/squad.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    12560 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/transformer_squad.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7796 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/triviaqa.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    22635 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.391631 radgraph-0.0.7/radgraph/allennlp_models/rc/metrics/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      152 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/metrics/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3421 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/metrics/drop_em_and_f1.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2753 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/metrics/squad_em_and_f1.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.391631 radgraph-0.0.7/radgraph/allennlp_models/rc/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      505 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    18758 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/bidaf.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7853 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/bidaf_ensemble.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    27476 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/dialog_qa.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    33059 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/naqanet.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13990 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/qanet.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    11569 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/transformer_qa.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2158 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/models/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.395632 radgraph-0.0.7/radgraph/allennlp_models/rc/modules/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       88 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/modules/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.395632 radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      340 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7417 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/multi_head_self_attention.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    11446 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/qanet_encoder.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7570 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/stacked_self_attention.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.395632 radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      255 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6112 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/bidaf.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2834 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/dialog_qa.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4128 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/transformer_qa.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.399632 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10682 2023-01-25 23:16:54.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/drop.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2518 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/narrativeqa.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3689 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/orb.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4432 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/orb_utils.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4839 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/quoref.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3430 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/squad.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1919 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/squad2.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3413 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/rc/tools/transformer_qa.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.399632 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      307 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.403632 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      512 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    10609 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/penn_tree_bank.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4858 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/semantic_dependencies.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    11874 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/srl.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5029 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/universal_dependencies.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.403632 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/metrics/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       97 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/metrics/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7680 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/metrics/srl_eval_scorer.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.407632 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      500 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    31341 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/biaffine_dependency_parser.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    22083 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/constituency_parser.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    16278 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/graph_parser.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    21087 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/srl.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13523 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/srl_bert.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.411632 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      463 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7185 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/biaffine_dependency_parser.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5828 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/constituency_parser.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8449 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/openie.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9136 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/srl.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.411632 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/tools/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/tools/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8474 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/tools/convert_openie_to_conll.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     4358 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/tools/write_srl_predictions_to_conll_format.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.411632 radgraph-0.0.7/radgraph/allennlp_models/tagging/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      196 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.411632 radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      385 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9163 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/ccgbank.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7068 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/conll2000.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      175 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/conll2003.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5086 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/ontonotes_ner.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.411632 radgraph-0.0.7/radgraph/allennlp_models/tagging/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       73 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    13021 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/models/crf_tagger.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.415632 radgraph-0.0.7/radgraph/allennlp_models/tagging/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       96 2023-01-26 00:31:08.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      172 2023-01-26 00:29:27.000000 radgraph-0.0.7/radgraph/allennlp_models/tagging/predictors/sentence_tagger.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      373 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/allennlp_models/version.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.415632 radgraph-0.0.7/radgraph/dygie/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/dygie/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.415632 radgraph-0.0.7/radgraph/dygie/data/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      132 2023-01-26 00:31:53.000000 radgraph-0.0.7/radgraph/dygie/data/__init__.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.415632 radgraph-0.0.7/radgraph/dygie/data/dataset_readers/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/dygie/data/dataset_readers/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    25839 2023-01-26 00:31:53.000000 radgraph-0.0.7/radgraph/dygie/data/dataset_readers/document.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8664 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/data/dataset_readers/dygie.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.415632 radgraph-0.0.7/radgraph/dygie/data/fields/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/dygie/data/fields/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6467 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/data/fields/adjacency_field_assym.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.423632 radgraph-0.0.7/radgraph/dygie/models/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       46 2023-01-26 00:31:53.000000 radgraph-0.0.7/radgraph/dygie/models/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    37380 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/models/coref.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    16833 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/models/dygie.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     9396 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/models/entity_beam_pruner.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    21835 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/models/events.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     7330 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/models/ner.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)    12336 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/dygie/models/relation.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2131 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/dygie/models/shared.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.423632 radgraph-0.0.7/radgraph/dygie/predictors/
+-rw-rw-r--   0 jb        (1000) jb        (1000)       59 2023-01-26 00:31:53.000000 radgraph-0.0.7/radgraph/dygie/predictors/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2617 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/dygie/predictors/dygie.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.423632 radgraph-0.0.7/radgraph/dygie/training/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/dygie/training/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     6750 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/training/event_metrics.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)      360 2023-01-06 19:33:15.000000 radgraph-0.0.7/radgraph/dygie/training/f1.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     2228 2023-07-06 18:55:10.000000 radgraph-0.0.7/radgraph/dygie/training/ner_metrics.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     1534 2023-07-06 18:55:11.000000 radgraph-0.0.7/radgraph/dygie/training/relation_metrics.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     8722 2023-01-26 00:37:57.000000 radgraph-0.0.7/radgraph/radgraph.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     5268 2023-01-25 22:37:36.000000 radgraph-0.0.7/radgraph/rewards.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3702 2023-01-26 00:23:33.000000 radgraph-0.0.7/radgraph/utils.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.267631 radgraph-0.0.7/radgraph.egg-info/
+-rw-rw-r--   0 jb        (1000) jb        (1000)      296 2023-07-06 18:56:57.000000 radgraph-0.0.7/radgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 jb        (1000) jb        (1000)    22293 2023-07-06 18:56:58.000000 radgraph-0.0.7/radgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-07-06 18:56:57.000000 radgraph-0.0.7/radgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)        1 2023-07-06 18:56:57.000000 radgraph-0.0.7/radgraph.egg-info/not-zip-safe
+-rw-rw-r--   0 jb        (1000) jb        (1000)       78 2023-07-06 18:56:57.000000 radgraph-0.0.7/radgraph.egg-info/requires.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       26 2023-07-06 18:56:57.000000 radgraph-0.0.7/radgraph.egg-info/top_level.txt
+-rw-rw-r--   0 jb        (1000) jb        (1000)       38 2023-07-06 18:56:58.427632 radgraph-0.0.7/setup.cfg
+-rw-rw-r--   0 jb        (1000) jb        (1000)      724 2023-07-06 18:55:59.000000 radgraph-0.0.7/setup.py
+drwxrwxr-x   0 jb        (1000) jb        (1000)        0 2023-07-06 18:56:58.423632 radgraph-0.0.7/tests/
+-rw-rw-r--   0 jb        (1000) jb        (1000)        0 2023-07-06 18:32:42.000000 radgraph-0.0.7/tests/__init__.py
+-rw-rw-r--   0 jb        (1000) jb        (1000)     3233 2023-07-06 18:31:35.000000 radgraph-0.0.7/tests/radgraph_test.py
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/__main__.py` & `radgraph-0.0.7/radgraph/allennlp/__main__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/commands/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 import logging
 from typing import Any, Optional
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp import __version__
 from radgraph.allennlp.commands.evaluate import Evaluate
 from radgraph.allennlp.commands.find_learning_rate import FindLearningRate
 from radgraph.allennlp.commands.predict import Predict
 from radgraph.allennlp.commands.print_results import PrintResults
 from radgraph.allennlp.commands.subcommand import Subcommand
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/evaluate.py` & `radgraph-0.0.7/radgraph/allennlp/commands/evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 import argparse
 import json
 import logging
 from typing import Any, Dict
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.commands.subcommand import Subcommand
 from radgraph.allennlp.common import logging as common_logging
 from radgraph.allennlp.common.util import dump_metrics, prepare_environment
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data import DataLoader
 from radgraph.allennlp.models.archival import load_archive
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/find_learning_rate.py` & `radgraph-0.0.7/radgraph/allennlp/commands/find_learning_rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import logging
 import math
 import os
 import re
 from typing import List, Tuple
 import itertools
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.commands.subcommand import Subcommand
 from radgraph.allennlp.common import Params, Tqdm
 from radgraph.allennlp.common import logging as common_logging
 from radgraph.allennlp.common.checks import check_for_gpu, ConfigurationError
 from radgraph.allennlp.common.util import prepare_environment
 from radgraph.allennlp.data import Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/predict.py` & `radgraph-0.0.7/radgraph/allennlp/commands/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from typing import List, Iterator, Optional
 import argparse
 import sys
 import json
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.commands.subcommand import Subcommand
 from radgraph.allennlp.common import logging as common_logging
 from radgraph.allennlp.common.checks import check_for_gpu, ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.common.util import lazy_groups_of
 from radgraph.allennlp.models.archival import load_archive
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/print_results.py` & `radgraph-0.0.7/radgraph/allennlp/commands/print_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 
 import argparse
 import json
 import logging
 import os
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.commands.subcommand import Subcommand
 
 logger = logging.getLogger(__name__)
 
 
 @Subcommand.register("print-results")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/subcommand.py` & `radgraph-0.0.7/radgraph/allennlp/commands/subcommand.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Base class for subcommands under `allennlp.run`.
 """
 
 import argparse
 from typing import Callable, Dict, Optional, Type, TypeVar
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common import Registrable
 
 
 T = TypeVar("T", bound="Subcommand")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/test_install.py` & `radgraph-0.0.7/radgraph/allennlp/commands/test_install.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 that AllenNLP has been successfully installed.
 """
 
 import argparse
 import logging
 import pathlib
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.util import import_module_and_submodules
 from radgraph.allennlp.commands.subcommand import Subcommand
 from radgraph.allennlp.version import VERSION
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/commands/train.py` & `radgraph-0.0.7/radgraph/allennlp/commands/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 from os import PathLike
 from typing import Any, Dict, List, Optional, Union
 
 import torch
 import torch.distributed as dist
 import torch.multiprocessing as mp
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.commands.subcommand import Subcommand
 from radgraph.allennlp.common import Params, Registrable, Lazy
 from radgraph.allennlp.common.checks import check_for_gpu, ConfigurationError
 from radgraph.allennlp.common import logging as common_logging
 from radgraph.allennlp.common import util as common_util
 from radgraph.allennlp.common.plugins import import_plugins
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/cached_transformers.py` & `radgraph-0.0.7/radgraph/allennlp/common/cached_transformers.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/checks.py` & `radgraph-0.0.7/radgraph/allennlp/common/checks.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/file_utils.py` & `radgraph-0.0.7/radgraph/allennlp/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/from_params.py` & `radgraph-0.0.7/radgraph/allennlp/common/from_params.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/lazy.py` & `radgraph-0.0.7/radgraph/allennlp/common/lazy.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/logging.py` & `radgraph-0.0.7/radgraph/allennlp/common/logging.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/params.py` & `radgraph-0.0.7/radgraph/allennlp/common/params.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import zlib
 from collections import OrderedDict
 from collections.abc import MutableMapping
 from os import PathLike
 from typing import Any, Dict, List, Union
 
-from overrides import overrides
+from overrides_ import overrides
 
 # _jsonnet doesn't work on Windows, so we have to use fakes.
 try:
     from _jsonnet import evaluate_file, evaluate_snippet
 except ImportError:
 
     def evaluate_file(filename: str, **_kwargs) -> str:
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/plugins.py` & `radgraph-0.0.7/radgraph/allennlp/common/plugins.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/registrable.py` & `radgraph-0.0.7/radgraph/allennlp/common/registrable.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/testing/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/common/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/testing/distributed_test.py` & `radgraph-0.0.7/radgraph/allennlp/common/testing/distributed_test.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/testing/model_test_case.py` & `radgraph-0.0.7/radgraph/allennlp/common/testing/model_test_case.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/testing/test_case.py` & `radgraph-0.0.7/radgraph/allennlp/common/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/tqdm.py` & `radgraph-0.0.7/radgraph/allennlp/common/tqdm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/common/util.py` & `radgraph-0.0.7/radgraph/allennlp/common/util.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/data/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/batch.py` & `radgraph-0.0.7/radgraph/allennlp/data/batch.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataloader.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/babi.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/babi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from typing import Dict, List
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.fields import Field, TextField, ListField, IndexField
 from radgraph.allennlp.data.token_indexers import TokenIndexer, SingleIdTokenIndexer
 from radgraph.allennlp.data.tokenizers import Token
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/conll2003.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/conll2003.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Sequence, Iterable
 import itertools
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.dataset_readers.dataset_utils import to_bioul
 from radgraph.allennlp.data.fields import TextField, SequenceLabelField, Field, MetadataField
 from radgraph.allennlp.data.instance import Instance
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/dataset_reader.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/dataset_reader.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/dataset_utils/span_utils.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/dataset_utils/span_utils.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/interleaving_dataset_reader.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/interleaving_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/sequence_tagging.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/sequence_tagging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import TextField, SequenceLabelField, MetadataField, Field
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import TokenIndexer, SingleIdTokenIndexer
 from radgraph.allennlp.data.tokenizers import Token
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/sharded_dataset_reader.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/sharded_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/dataset_readers/text_classification_json.py` & `radgraph-0.0.7/radgraph/allennlp/data/dataset_readers/text_classification_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Union
 import logging
 import json
-from overrides import overrides
+from overrides_ import overrides
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import LabelField, TextField, Field, ListField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import TokenIndexer, SingleIdTokenIndexer
 from radgraph.allennlp.data.tokenizers import Tokenizer, SpacyTokenizer
 from radgraph.allennlp.data.tokenizers.sentence_splitter import SpacySentenceSplitter
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/adjacency_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/adjacency_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Set, Tuple
 import logging
 import textwrap
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.data.fields.field import Field
 from radgraph.allennlp.data.fields.sequence_field import SequenceField
 from radgraph.allennlp.data.vocabulary import Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/array_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/array_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 
 import numpy
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.fields.field import Field
 
 
 class ArrayField(Field[numpy.ndarray]):
     """
     A class representing an array, which could have arbitrary dimensions.
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/field.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/flag_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/flag_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.fields.field import Field
 
 
 class FlagField(Field[Any]):
     """
     A class representing a flag, which must be constant across all instances in a batch.
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/index_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/index_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.data.fields.field import Field
 from radgraph.allennlp.data.fields.sequence_field import SequenceField
 from radgraph.allennlp.common.checks import ConfigurationError
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/label_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/label_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Union, Set
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.data.fields.field import Field
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.common.checks import ConfigurationError
 
 logger = logging.getLogger(__name__)
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/list_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/list_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Iterator
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.fields.field import DataArray, Field
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.data.fields.sequence_field import SequenceField
 from radgraph.allennlp.common.util import pad_sequence_to_length
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/metadata_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/metadata_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List, Mapping
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.fields.field import DataArray, Field
 
 
 class MetadataField(Field[DataArray], Mapping[str, Any]):
     """
     A `MetadataField` is a `Field` that does not get converted into tensors.  It just carries
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/multilabel_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/multilabel_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Union, Sequence, Set, Optional, cast
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.data.fields.field import Field
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.common.checks import ConfigurationError
 
 logger = logging.getLogger(__name__)
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/namespace_swapping_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/namespace_swapping_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.util import pad_sequence_to_length
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.fields.field import Field
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/sequence_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/sequence_field.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/sequence_label_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/sequence_label_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Union, Set, Iterator
 import logging
 import textwrap
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.util import pad_sequence_to_length
 from radgraph.allennlp.data.fields.field import Field
 from radgraph.allennlp.data.fields.sequence_field import SequenceField
 from radgraph.allennlp.data.vocabulary import Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/span_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/span_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.data.fields.field import Field
 from radgraph.allennlp.data.fields.sequence_field import SequenceField
 
 
 class SpanField(Field[torch.Tensor]):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/fields/text_field.py` & `radgraph-0.0.7/radgraph/allennlp/data/fields/text_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 standard word vectors, or pass through an LSTM.
 """
 from collections import defaultdict
 from copy import deepcopy
 from typing import Dict, List, Optional, Iterator
 import textwrap
 
-from overrides import overrides
+from overrides_ import overrides
 from spacy.tokens import Token as SpacyToken
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.data.fields.sequence_field import SequenceField
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer, IndexedTokenList
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/instance.py` & `radgraph-0.0.7/radgraph/allennlp/data/instance.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/samplers/bucket_batch_sampler.py` & `radgraph-0.0.7/radgraph/allennlp/data/samplers/bucket_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/samplers/max_tokens_batch_sampler.py` & `radgraph-0.0.7/radgraph/allennlp/data/samplers/max_tokens_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/samplers/samplers.py` & `radgraph-0.0.7/radgraph/allennlp/data/samplers/samplers.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/elmo_indexer.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/elmo_indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.util import pad_sequence_to_length
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer, IndexedTokenList
 from radgraph.allennlp.data.vocabulary import Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/pretrained_transformer_indexer.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/pretrained_transformer_indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List, Optional, Tuple
 import logging
 import torch
 from radgraph.allennlp.common.util import pad_sequence_to_length
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.data.tokenizers import PretrainedTransformerTokenizer
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer, IndexedTokenList
 
 logger = logging.getLogger(__name__)
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/pretrained_transformer_mismatched_indexer.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/pretrained_transformer_mismatched_indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.util import pad_sequence_to_length
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.token_indexers import PretrainedTransformerIndexer, TokenIndexer
 from radgraph.allennlp.data.token_indexers.token_indexer import IndexedTokenList
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/single_id_token_indexer.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/single_id_token_indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Optional
 import itertools
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer, IndexedTokenList
 
 
 _DEFAULT_VALUE = "THIS IS A REALLY UNLIKELY VALUE THAT HAS TO BE A STRING"
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/spacy_indexer.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/spacy_indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List
 
-from overrides import overrides
+from overrides_ import overrides
 from spacy.tokens import Token as SpacyToken
 import torch
 import numpy
 
 from radgraph.allennlp.common.util import pad_sequence_to_length
 from radgraph.allennlp.data.vocabulary import Vocabulary
 from radgraph.allennlp.data.tokenizers.token import Token
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/token_characters_indexer.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/token_characters_indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List
 import itertools
 import warnings
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.util import pad_sequence_to_length
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer, IndexedTokenList
 from radgraph.allennlp.data.tokenizers.character_tokenizer import CharacterTokenizer
 from radgraph.allennlp.data.tokenizers.token import Token
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/token_indexers/token_indexer.py` & `radgraph-0.0.7/radgraph/allennlp/data/token_indexers/token_indexer.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/character_tokenizer.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/character_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Union
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.tokenizers.tokenizer import Tokenizer
 
 
 @Tokenizer.register("character")
 class CharacterTokenizer(Tokenizer):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/letters_digits_tokenizer.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/letters_digits_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from typing import List
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.tokenizers.tokenizer import Tokenizer
 
 
 @Tokenizer.register("letters_digits")
 class LettersDigitsTokenizer(Tokenizer):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/pretrained_transformer_tokenizer.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/pretrained_transformer_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import logging
 from typing import Any, Dict, List, Optional, Tuple, Iterable
 
-from overrides import overrides
+from overrides_ import overrides
 from transformers import PreTrainedTokenizer
 
 from radgraph.allennlp.common.util import sanitize_wordpiece
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.tokenizers.tokenizer import Tokenizer
 
 logger = logging.getLogger(__name__)
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/sentence_splitter.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/sentence_splitter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from overrides import overrides
+from overrides_ import overrides
 
 import spacy
 
 from radgraph.allennlp.common import Registrable
 from radgraph.allennlp.common.util import get_spacy_model
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/spacy_tokenizer.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/spacy_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import spacy
 from spacy.tokens import Doc
 
 from radgraph.allennlp.common.util import get_spacy_model
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.tokenizers.tokenizer import Tokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/token.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/token.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/tokenizer.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/tokenizers/whitespace_tokenizer.py` & `radgraph-0.0.7/radgraph/allennlp/data/tokenizers/whitespace_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.tokenizers.token import Token
 from radgraph.allennlp.data.tokenizers.tokenizer import Tokenizer
 
 
 @Tokenizer.register("whitespace")
 @Tokenizer.register("just_spaces")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/data/vocabulary.py` & `radgraph-0.0.7/radgraph/allennlp/data/vocabulary.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/attackers/attacker.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/attackers/attacker.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/attackers/hotflip.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/attackers/hotflip.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/attackers/input_reduction.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/attackers/input_reduction.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/attackers/utils.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/attackers/utils.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/integrated_gradient.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/integrated_gradient.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/saliency_interpreter.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/saliency_interpreter.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/simple_gradient.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/simple_gradient.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/interpret/saliency_interpreters/smooth_gradient.py` & `radgraph-0.0.7/radgraph/allennlp/interpret/saliency_interpreters/smooth_gradient.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/models/archival.py` & `radgraph-0.0.7/radgraph/allennlp/models/archival.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/models/basic_classifier.py` & `radgraph-0.0.7/radgraph/allennlp/models/basic_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules import FeedForward, Seq2SeqEncoder, Seq2VecEncoder, TextFieldEmbedder
 from radgraph.allennlp.nn import InitializerApplicator, util
 from radgraph.allennlp.nn.util import get_text_field_mask
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/models/model.py` & `radgraph-0.0.7/radgraph/allennlp/models/model.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/models/simple_tagger.py` & `radgraph-0.0.7/radgraph/allennlp/models/simple_tagger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Optional, List, Any
 
 import numpy
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.modules.linear import Linear
 import torch.nn.functional as F
 
 from radgraph.allennlp.common.checks import check_dimensions_match, ConfigurationError
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.modules import Seq2SeqEncoder, TimeDistributed, TextFieldEmbedder
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/attention/additive_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/attention/additive_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.parameter import Parameter
 
 from radgraph.allennlp.modules.attention.attention import Attention
 
 
 @Attention.register("additive")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/attention/attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/attention/attention.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 An *attention* module that computes the similarity between
 an input vector and the rows of a matrix.
 """
 
 import torch
 
-from overrides import overrides
+from overrides_ import overrides
 from radgraph.allennlp.common.registrable import Registrable
 from radgraph.allennlp.nn.util import masked_softmax
 
 
 class Attention(torch.nn.Module, Registrable):
     """
     An `Attention` takes two inputs: a (batched) vector and a matrix, plus an optional mask on the
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/attention/bilinear_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/attention/bilinear_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.parameter import Parameter
 
 from radgraph.allennlp.modules.attention.attention import Attention
 from radgraph.allennlp.nn import Activation
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/attention/cosine_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/attention/cosine_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from overrides import overrides
+from overrides_ import overrides
 from radgraph.allennlp.modules.attention.attention import Attention
 from radgraph.allennlp.nn import util
 
 
 @Attention.register("cosine")
 class CosineAttention(Attention):
     """
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/attention/linear_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/attention/linear_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 
 import torch
 from torch.nn import Parameter
-from overrides import overrides
+from overrides_ import overrides
 from radgraph.allennlp.modules.attention.attention import Attention
 from radgraph.allennlp.nn import util
 from radgraph.allennlp.nn.activations import Activation
 
 
 @Attention.register("linear")
 class LinearAttention(Attention):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/augmented_lstm.py` & `radgraph-0.0.7/radgraph/allennlp/modules/augmented_lstm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/bimpm_matching.py` & `radgraph-0.0.7/radgraph/allennlp/modules/bimpm_matching.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/conditional_random_field.py` & `radgraph-0.0.7/radgraph/allennlp/modules/conditional_random_field.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/elmo.py` & `radgraph-0.0.7/radgraph/allennlp/modules/elmo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import warnings
 from typing import Any, Dict, List, Union
 
 import numpy
 import torch
-from overrides import overrides
+from overrides_ import overrides
 from torch.nn.modules import Dropout
 
 from radgraph.allennlp.common import FromParams
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.common.util import lazy_groups_of
 from radgraph.allennlp.data import Instance, Token, Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/elmo_lstm.py` & `radgraph-0.0.7/radgraph/allennlp/modules/elmo_lstm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/encoder_base.py` & `radgraph-0.0.7/radgraph/allennlp/modules/encoder_base.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/feedforward.py` & `radgraph-0.0.7/radgraph/allennlp/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/gated_sum.py` & `radgraph-0.0.7/radgraph/allennlp/modules/gated_sum.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/highway.py` & `radgraph-0.0.7/radgraph/allennlp/modules/highway.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A [Highway layer](https://arxiv.org/abs/1505.00387) that does a gated combination of a linear
 transformation and a non-linear transformation of its input.
 """
 
 from typing import Callable
 
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 
 class Highway(torch.nn.Module):
     """
     A [Highway layer](https://arxiv.org/abs/1505.00387) does a gated combination of a linear
     transformation and a non-linear transformation of its input.  :math:`y = g * x + (1 - g) *
     f(A(x))`, where :math:`A` is a linear transformation, :math:`f` is an element-wise
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/input_variational_dropout.py` & `radgraph-0.0.7/radgraph/allennlp/modules/input_variational_dropout.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/layer_norm.py` & `radgraph-0.0.7/radgraph/allennlp/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/lstm_cell_with_projection.py` & `radgraph-0.0.7/radgraph/allennlp/modules/lstm_cell_with_projection.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/masked_layer_norm.py` & `radgraph-0.0.7/radgraph/allennlp/modules/masked_layer_norm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/bilinear_matrix_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/bilinear_matrix_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.parameter import Parameter
 
 from radgraph.allennlp.modules.matrix_attention.matrix_attention import MatrixAttention
 from radgraph.allennlp.nn import Activation
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/cosine_matrix_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/cosine_matrix_attention.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.modules.matrix_attention.matrix_attention import MatrixAttention
 from radgraph.allennlp.nn import util
 
 
 @MatrixAttention.register("cosine")
 class CosineMatrixAttention(MatrixAttention):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/dot_product_matrix_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/dot_product_matrix_attention.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.modules.matrix_attention.matrix_attention import MatrixAttention
 
 
 @MatrixAttention.register("dot_product")
 class DotProductMatrixAttention(MatrixAttention):
     """
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/linear_matrix_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/linear_matrix_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 
 import torch
 from torch.nn import Parameter
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.nn import util
 from radgraph.allennlp.nn.activations import Activation
 from radgraph.allennlp.modules.matrix_attention.matrix_attention import MatrixAttention
 
 
 @MatrixAttention.register("linear")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/matrix_attention/matrix_attention.py` & `radgraph-0.0.7/radgraph/allennlp/modules/matrix_attention/matrix_attention.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/maxout.py` & `radgraph-0.0.7/radgraph/allennlp/modules/maxout.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/residual_with_layer_dropout.py` & `radgraph-0.0.7/radgraph/allennlp/modules/residual_with_layer_dropout.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/sampled_softmax_loss.py` & `radgraph-0.0.7/radgraph/allennlp/modules/sampled_softmax_loss.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/scalar_mix.py` & `radgraph-0.0.7/radgraph/allennlp/modules/scalar_mix.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/compose_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/compose_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from typing import List
 
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
 
 
 @Seq2SeqEncoder.register("compose")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/feedforward_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/feedforward_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.modules.feedforward import FeedForward
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
 
 
 @Seq2SeqEncoder.register("feedforward")
 class FeedForwardEncoder(Seq2SeqEncoder):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/gated_cnn_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/gated_cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/pass_through_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/pass_through_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
 
 
 @Seq2SeqEncoder.register("pass_through")
 class PassThroughEncoder(Seq2SeqEncoder):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/pytorch_seq2seq_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.utils.rnn import pad_packed_sequence
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.modules.augmented_lstm import AugmentedLstm
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
 from radgraph.allennlp.modules.stacked_alternating_lstm import StackedAlternatingLstm
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/pytorch_transformer_wrapper.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/pytorch_transformer_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch import nn
 
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
 from radgraph.allennlp.nn.util import add_positional_features
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2seq_encoders/seq2seq_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2seq_encoders/seq2seq_encoder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/bert_pooler.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/bert_pooler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 import torch.nn
 
 from radgraph.allennlp.modules.seq2vec_encoders.seq2vec_encoder import Seq2VecEncoder
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/boe_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/boe_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 
 from radgraph.allennlp.modules.seq2vec_encoders.seq2vec_encoder import Seq2VecEncoder
 from radgraph.allennlp.nn.util import get_lengths_from_binary_sequence_mask
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/cls_pooler.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/cls_pooler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 
 import torch.nn
 
 from radgraph.allennlp.modules.seq2vec_encoders.seq2vec_encoder import Seq2VecEncoder
 from radgraph.allennlp.nn.util import get_final_encoder_states
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/cnn_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/cnn_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Tuple
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn import Conv1d, Linear
 
 from radgraph.allennlp.modules.seq2vec_encoders.seq2vec_encoder import Seq2VecEncoder
 from radgraph.allennlp.nn import Activation
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/cnn_highway_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/cnn_highway_encoder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/pytorch_seq2vec_wrapper.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/pytorch_seq2vec_wrapper.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/seq2vec_encoders/seq2vec_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/seq2vec_encoders/seq2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/softmax_loss.py` & `radgraph-0.0.7/radgraph/allennlp/modules/softmax_loss.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/bidirectional_endpoint_span_extractor.py` & `radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/bidirectional_endpoint_span_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from overrides import overrides
+from overrides_ import overrides
 from torch.nn.parameter import Parameter
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.modules.span_extractors.span_extractor import SpanExtractor
 from radgraph.allennlp.modules.token_embedders.embedding import Embedding
 from radgraph.allennlp.nn import util
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/endpoint_span_extractor.py` & `radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/endpoint_span_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch.nn.parameter import Parameter
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.modules.span_extractors.span_extractor import SpanExtractor
 from radgraph.allennlp.modules.token_embedders.embedding import Embedding
 from radgraph.allennlp.nn import util
 
 from radgraph.allennlp.common.checks import ConfigurationError
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/self_attentive_span_extractor.py` & `radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/self_attentive_span_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.modules.span_extractors.span_extractor import SpanExtractor
 from radgraph.allennlp.modules.time_distributed import TimeDistributed
 from radgraph.allennlp.nn import util
 
 
 @SpanExtractor.register("self_attentive")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/span_extractors/span_extractor.py` & `radgraph-0.0.7/radgraph/allennlp/modules/span_extractors/span_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.registrable import Registrable
 
 
 class SpanExtractor(torch.nn.Module, Registrable):
     """
     Many NLP models deal with representations of spans inside a sentence.
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/stacked_alternating_lstm.py` & `radgraph-0.0.7/radgraph/allennlp/modules/stacked_alternating_lstm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/stacked_bidirectional_lstm.py` & `radgraph-0.0.7/radgraph/allennlp/modules/stacked_bidirectional_lstm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/text_field_embedders/basic_text_field_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/text_field_embedders/basic_text_field_embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict
 import inspect
 
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.data import TextFieldTensors
 from radgraph.allennlp.modules.text_field_embedders.text_field_embedder import TextFieldEmbedder
 from radgraph.allennlp.modules.time_distributed import TimeDistributed
 from radgraph.allennlp.modules.token_embedders.token_embedder import TokenEmbedder
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/text_field_embedders/text_field_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/text_field_embedders/text_field_embedder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/time_distributed.py` & `radgraph-0.0.7/radgraph/allennlp/modules/time_distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A wrapper that unrolls the second (time) dimension of a tensor
 into the first (batch) dimension, applies some other `Module`,
 and then rolls the time dimension back up.
 """
 
 from typing import List
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 
 class TimeDistributed(torch.nn.Module):
     """
     Given an input shaped like `(batch_size, time_steps, [rest])` and a `Module` that takes
     inputs like `(batch_size, [rest])`, `TimeDistributed` reshapes the input to be
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/bag_of_word_counts_token_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/bag_of_word_counts_token_embedder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/elmo_token_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/elmo_token_embedder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/embedding.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import tarfile
 import warnings
 import zipfile
 from typing import Any, cast, Iterator, NamedTuple, Optional, Sequence, Tuple, BinaryIO
 
 import numpy
 import torch
-from overrides import overrides
+from overrides_ import overrides
 from torch.nn.functional import embedding
 
 from radgraph.allennlp.common import Tqdm
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path, get_file_extension, is_url_or_existing_file
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.modules.time_distributed import TimeDistributed
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/empty_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/empty_embedder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/pass_through_token_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/pass_through_token_embedder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/pretrained_transformer_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/pretrained_transformer_embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from typing import Optional, Tuple
 
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 import torch.nn.functional as F
 from transformers import XLNetConfig
 
 from radgraph.allennlp.data.tokenizers import PretrainedTransformerTokenizer
 from radgraph.allennlp.modules.scalar_mix import ScalarMix
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/pretrained_transformer_mismatched_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/pretrained_transformer_mismatched_embedder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.modules.token_embedders import PretrainedTransformerEmbedder, TokenEmbedder
 from radgraph.allennlp.nn import util
 
 
 @TokenEmbedder.register("pretrained_transformer_mismatched")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/token_characters_encoder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/token_characters_encoder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/modules/token_embedders/token_embedder.py` & `radgraph-0.0.7/radgraph/allennlp/modules/token_embedders/token_embedder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/nn/activations.py` & `radgraph-0.0.7/radgraph/allennlp/nn/activations.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 * ["softsign"](https://pytorch.org/docs/master/nn.html#torch.nn.Softsign)
 * ["tanhshrink"](https://pytorch.org/docs/master/nn.html#torch.nn.Tanhshrink)
 * ["selu"](https://pytorch.org/docs/master/nn.html#torch.nn.SELU)
 """
 from typing import Callable
 
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common import Registrable
 
 
 class Activation(torch.nn.Module, Registrable):
     """
     Pytorch has a number of built-in activation functions.  We group those here under a common
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/nn/beam_search.py` & `radgraph-0.0.7/radgraph/allennlp/nn/beam_search.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/nn/chu_liu_edmonds.py` & `radgraph-0.0.7/radgraph/allennlp/nn/chu_liu_edmonds.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/nn/initializers.py` & `radgraph-0.0.7/radgraph/allennlp/nn/initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * ["pretrained"](./initializers.md#PretrainedModelInitializer)
 """
 import logging
 import re
 import math
 from typing import Callable, List, Tuple, Dict
 import itertools
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 import torch.nn.init
 
 from radgraph.allennlp.common import FromParams, Registrable
 from radgraph.allennlp.common.checks import ConfigurationError
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/nn/regularizers/regularizer_applicator.py` & `radgraph-0.0.7/radgraph/allennlp/nn/regularizers/regularizer_applicator.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/nn/regularizers/regularizers.py` & `radgraph-0.0.7/radgraph/allennlp/nn/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/nn/util.py` & `radgraph-0.0.7/radgraph/allennlp/nn/util.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/predictors/predictor.py` & `radgraph-0.0.7/radgraph/allennlp/predictors/predictor.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/predictors/sentence_tagger.py` & `radgraph-0.0.7/radgraph/allennlp/predictors/sentence_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import numpy
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import DatasetReader, Instance
 from radgraph.allennlp.data.fields import FlagField, TextField, SequenceLabelField
 from radgraph.allennlp.data.tokenizers.spacy_tokenizer import SpacyTokenizer
 from radgraph.allennlp.models import Model
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/predictors/text_classifier.py` & `radgraph-0.0.7/radgraph/allennlp/predictors/text_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import numpy
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import Instance
 from radgraph.allennlp.predictors.predictor import Predictor
 from radgraph.allennlp.data.fields import LabelField
 from radgraph.allennlp.data.tokenizers.spacy_tokenizer import SpacyTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/tools/archive_surgery.py` & `radgraph-0.0.7/radgraph/allennlp/tools/archive_surgery.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/tools/create_elmo_embeddings_from_vocab.py` & `radgraph-0.0.7/radgraph/allennlp/tools/create_elmo_embeddings_from_vocab.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/tools/inspect_cache.py` & `radgraph-0.0.7/radgraph/allennlp/tools/inspect_cache.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/checkpointer.py` & `radgraph-0.0.7/radgraph/allennlp/training/checkpointer.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/cosine.py` & `radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/cosine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 import numpy as np
 import torch
 
 from radgraph.allennlp.training.learning_rate_schedulers.learning_rate_scheduler import LearningRateScheduler
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/learning_rate_scheduler.py` & `radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/learning_rate_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List, Union
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.registrable import Registrable
 from radgraph.allennlp.training.scheduler import Scheduler
 from radgraph.allennlp.training.optimizers import Optimizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/linear_with_warmup.py` & `radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/linear_with_warmup.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/noam.py` & `radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/noam.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.training.learning_rate_schedulers.learning_rate_scheduler import LearningRateScheduler
 
 
 @LearningRateScheduler.register("noam")
 class NoamLR(LearningRateScheduler):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/polynomial_decay.py` & `radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/polynomial_decay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.training.learning_rate_schedulers.learning_rate_scheduler import LearningRateScheduler
 
 
 @LearningRateScheduler.register("polynomial_decay")
 class PolynomialDecay(LearningRateScheduler):
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/learning_rate_schedulers/slanted_triangular.py` & `radgraph-0.0.7/radgraph/allennlp/training/learning_rate_schedulers/slanted_triangular.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import List, Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.training.learning_rate_schedulers.learning_rate_scheduler import LearningRateScheduler
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metric_tracker.py` & `radgraph-0.0.7/radgraph/allennlp/training/metric_tracker.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/__init__.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/attachment_scores.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/attachment_scores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, List
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/auc.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/auc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 # from sklearn import metrics
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/average.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/average.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/bleu.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/bleu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections import Counter
 import math
 from typing import Iterable, Tuple, Dict, Set
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/boolean_accuracy.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/boolean_accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/categorical_accuracy.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/categorical_accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/covariance.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 # import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/entropy.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/entropy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/evalb_bracketing_scorer.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/evalb_bracketing_scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 import logging
 import os
 import tempfile
 import subprocess
 import shutil
 
-from overrides import overrides
+from overrides_ import overrides
 from nltk import Tree
 
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.common.checks import ConfigurationError
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/f1_measure.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/f1_measure.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/fbeta_measure.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/fbeta_measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional, Union
 
 import torch
 import torch.distributed as dist
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.training.metrics.metric import Metric
 
 
 @Metric.register("fbeta")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/mean_absolute_error.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/mean_absolute_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/metric.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/pearson_correlation.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/pearson_correlation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
 from typing import Optional
 import math
 import numpy as np
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 # import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.covariance import Covariance
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/perplexity.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/perplexity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.training.metrics.average import Average
 from radgraph.allennlp.training.metrics.metric import Metric
 
 
 @Metric.register("perplexity")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/rouge.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/rouge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import defaultdict
 from typing import Tuple, Dict, Set
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/sequence_accuracy.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/sequence_accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/span_based_f1_measure.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/span_based_f1_measure.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/spearman_correlation.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/spearman_correlation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
 
 
 @Metric.register("spearman_correlation")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/metrics/unigram_recall.py` & `radgraph-0.0.7/radgraph/allennlp/training/metrics/unigram_recall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 import sys
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/momentum_schedulers/inverted_triangular.py` & `radgraph-0.0.7/radgraph/allennlp/training/momentum_schedulers/inverted_triangular.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/moving_average.py` & `radgraph-0.0.7/radgraph/allennlp/training/moving_average.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/no_op_trainer.py` & `radgraph-0.0.7/radgraph/allennlp/training/no_op_trainer.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/optimizers.py` & `radgraph-0.0.7/radgraph/allennlp/training/optimizers.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/scheduler.py` & `radgraph-0.0.7/radgraph/allennlp/training/scheduler.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/tensorboard_writer.py` & `radgraph-0.0.7/radgraph/allennlp/training/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/trainer.py` & `radgraph-0.0.7/radgraph/allennlp/training/trainer.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp/training/util.py` & `radgraph-0.0.7/radgraph/allennlp/training/util.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/classification/dataset_readers/stanford_sentiment_tree_bank.py` & `radgraph-0.0.7/radgraph/allennlp_models/classification/dataset_readers/stanford_sentiment_tree_bank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Optional, Union
 import logging
 
 from radgraph.allennlp.data import Tokenizer
-from overrides import overrides
+from overrides_ import overrides
 from nltk.tree import Tree
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import LabelField, TextField, Field
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import TokenIndexer, SingleIdTokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/classification/models/biattentive_classification_network.py` & `radgraph-0.0.7/radgraph/allennlp_models/classification/models/biattentive_classification_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Union
 
 import numpy
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch import nn
 import torch.nn.functional as F
 
 from radgraph.allennlp.common.checks import check_dimensions_match, ConfigurationError
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.modules import Elmo, FeedForward, Maxout, Seq2SeqEncoder, TextFieldEmbedder
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/common/model_card.py` & `radgraph-0.0.7/radgraph/allennlp_models/common/model_card.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/common/ontonotes.py` & `radgraph-0.0.7/radgraph/allennlp_models/common/ontonotes.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/conll.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/conll.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import collections
 from typing import Dict, List, Optional, Tuple, DefaultDict
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers import PretrainedTransformerTokenizer
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/preco.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/preco.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 from typing import Dict, List, Optional, Tuple
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers import PretrainedTransformerTokenizer
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/dataset_readers/winobias.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/dataset_readers/winobias.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import collections
 from typing import Any, Dict, List, Optional, Tuple, DefaultDict
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import (
     Field,
     ListField,
     TextField,
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/metrics/conll_coref_scores.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/metrics/conll_coref_scores.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Dict, List, Tuple
 from collections import Counter
 
-from overrides import overrides
+from overrides_ import overrides
 # from scipy.optimize import linear_sum_assignment
 import numpy as np
 import torch
 
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/metrics/mention_recall.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/metrics/mention_recall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any, Dict, List, Set, Tuple
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 
 from radgraph.allennlp.training.metrics.metric import Metric
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/models/coref.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/models/coref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import math
 from typing import Any, Dict, List, Tuple
 
 import torch
 import torch.nn.functional as F
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules.token_embedders import Embedding
 from radgraph.allennlp.modules import FeedForward, GatedSum
 from radgraph.allennlp.modules import Seq2SeqEncoder, TimeDistributed, TextFieldEmbedder
 from radgraph.allennlp.modules.span_extractors import SelfAttentiveSpanExtractor, EndpointSpanExtractor
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/predictors/coref.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/predictors/coref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
 
-from overrides import overrides
+from overrides_ import overrides
 from spacy.tokens import Doc
 import numpy
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.common.util import get_spacy_model
 from radgraph.allennlp.data import DatasetReader, Instance
 from radgraph.allennlp.data.fields import ListField, SequenceLabelField
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/coref/util.py` & `radgraph-0.0.7/radgraph/allennlp_models/coref/util.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/cnn_dm.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/cnn_dm.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, Optional, List
 import logging
 import os
 import glob
 import hashlib
 import ftfy
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import TextField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers import Tokenizer, SpacyTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/copynet_seq2seq.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/copynet_seq2seq.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import List, Dict
 import warnings
 
 import numpy as np
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.common.util import START_SYMBOL, END_SYMBOL
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import TextField, ArrayField, MetadataField, NamespaceSwappingField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers import (
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/dataset_readers/seq2seq.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/dataset_readers/seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import csv
 from typing import Dict, Optional
 import logging
 import copy
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.common.util import START_SYMBOL, END_SYMBOL
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import TextField
 from radgraph.allennlp.data.instance import Instance
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/models/bart.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/models/bart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Tuple, Any
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.data.fields.text_field import TextFieldTensors
 from radgraph.allennlp.data.token_indexers.pretrained_transformer_indexer import PretrainedTransformerIndexer
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
 from radgraph.allennlp.nn.beam_search import BeamSearch
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/models/composed_seq2seq.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/models/composed_seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Optional
 
 import torch
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules import TextFieldEmbedder, Seq2SeqEncoder, Embedding
 from radgraph.allennlp.modules.text_field_embedders import BasicTextFieldEmbedder
 from radgraph.allennlp.nn import util, InitializerApplicator
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/models/copynet_seq2seq.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/models/copynet_seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Dict, Tuple, List, Any, Union
 
 import numpy
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.modules.linear import Linear
 from torch.nn.modules.rnn import LSTMCell
 
 from radgraph.allennlp.common.util import START_SYMBOL, END_SYMBOL
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.models.model import Model
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/models/simple_seq2seq.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/models/simple_seq2seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, Tuple, Iterable, Any
 
 import numpy
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.nn.functional as F
 from torch.nn.modules.linear import Linear
 from torch.nn.modules.rnn import LSTMCell, LSTM
 
 from radgraph.allennlp.common.util import START_SYMBOL, END_SYMBOL
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/decoder_net.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/decoder_net.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/lstm_cell.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/lstm_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Tuple, Dict, Optional
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 from torch.nn import LSTMCell
 
 from radgraph.allennlp.modules import Attention
 from radgraph.allennlp.nn import util
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/modules/decoder_nets/stacked_self_attention.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/modules/decoder_nets/stacked_self_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import math
 from copy import deepcopy
 from typing import Dict, Optional, Tuple
 
 import torch
 import torch.nn.functional as F
-from overrides import overrides
+from overrides_ import overrides
 from torch import nn
 from torch.autograd import Variable
 
 from radgraph.allennlp.modules.layer_norm import LayerNorm
 from radgraph.allennlp.nn import util as nn_util
 
 from radgraph.allennlp_models.lm.modules.seq2seq_encoders.bidirectional_lm_transformer import (
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/modules/seq_decoders/auto_regressive.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/modules/seq_decoders/auto_regressive.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, List, Tuple, Optional
-from overrides import overrides
+from overrides_ import overrides
 
 import numpy
 import torch
 import torch.nn.functional as F
 from torch.nn import Linear
 
 from radgraph.allennlp.common.checks import ConfigurationError
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/modules/seq_decoders/seq_decoder.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/modules/seq_decoders/seq_decoder.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/generation/predictors/seq2seq.py` & `radgraph-0.0.7/radgraph/allennlp_models/generation/predictors/seq2seq.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import Instance
 from radgraph.allennlp.predictors.predictor import Predictor
 
 
 @Predictor.register("seq2seq")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/masked_language_model.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/masked_language_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List
 import logging
 import copy
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers.tokenizer import Tokenizer
 from radgraph.allennlp.data.tokenizers import Token
 from radgraph.allennlp.data.tokenizers.whitespace_tokenizer import WhitespaceTokenizer
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/next_token_lm.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/next_token_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List
 import logging
 import copy
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers.tokenizer import Tokenizer
 from radgraph.allennlp.data.tokenizers import Token
 from radgraph.allennlp.data.tokenizers.whitespace_tokenizer import WhitespaceTokenizer
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/dataset_readers/simple_language_modeling.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/dataset_readers/simple_language_modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Iterable, Union, Optional, List
 import logging
 import math
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data.tokenizers import Token
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import TextField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer
 from radgraph.allennlp.data.token_indexers.token_indexer import TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/models/bidirectional_lm.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/models/bidirectional_lm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/models/language_model.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/models/language_model.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/models/masked_language_model.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/models/masked_language_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import check_dimensions_match
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules import Seq2SeqEncoder, TextFieldEmbedder
 from radgraph.allennlp.nn import util, InitializerApplicator
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/models/next_token_lm.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/models/next_token_lm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import check_dimensions_match
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules import Seq2SeqEncoder, TextFieldEmbedder
 from radgraph.allennlp.nn import util, InitializerApplicator
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/bert.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/bert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 from transformers import BertConfig, BertForMaskedLM
 import torch
 
 from .language_model_head import LanguageModelHead
 
 
 @LanguageModelHead.register("bert")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/gpt2.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/gpt2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 from transformers import GPT2Config, GPT2LMHeadModel
 import torch
 
 from .language_model_head import LanguageModelHead
 
 
 @LanguageModelHead.register("gpt2")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/language_model_head.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/language_model_head.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/modules/language_model_heads/linear.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/modules/language_model_heads/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp_models.lm.modules.language_model_heads.language_model_head import LanguageModelHead
 
 
 @LanguageModelHead.register("linear")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/modules/seq2seq_encoders/bidirectional_lm_transformer.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/modules/seq2seq_encoders/bidirectional_lm_transformer.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/modules/token_embedders/bidirectional_lm.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/modules/token_embedders/bidirectional_lm.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/modules/token_embedders/language_model.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/modules/token_embedders/language_model.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/predictors/masked_language_model.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/predictors/masked_language_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import numpy
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import Instance, Token
 from radgraph.allennlp.data.fields import TextField
 from radgraph.allennlp.predictors.predictor import Predictor
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/lm/predictors/next_token_lm.py` & `radgraph-0.0.7/radgraph/allennlp_models/lm/predictors/next_token_lm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from overrides import overrides
+from overrides_ import overrides
 import numpy
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import Instance, Token
 from radgraph.allennlp.data.fields import TextField
 from radgraph.allennlp.predictors.predictor import Predictor
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/commonsenseqa.py` & `radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/commonsenseqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from radgraph.allennlp.data import DatasetReader
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp_models.mc.dataset_readers.transformer_mc import TransformerMCReader
 
 logger = logging.getLogger(__name__)
 
 
 @DatasetReader.register("commonsenseqa")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/fake.py` & `radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/fake.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import List
 
 from radgraph.allennlp.data import DatasetReader, Instance
-from overrides import overrides
+from overrides_ import overrides
 
 logger = logging.getLogger(__name__)
 
 
 @DatasetReader.register("fake")
 class FakeReader(DatasetReader):
     """
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/piqa.py` & `radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/piqa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from radgraph.allennlp.data import DatasetReader
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp_models.mc.dataset_readers.transformer_mc import TransformerMCReader
 
 logger = logging.getLogger(__name__)
 
 
 @DatasetReader.register("piqa")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/swag.py` & `radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/swag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from radgraph.allennlp.data import DatasetReader
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp_models.mc.dataset_readers.transformer_mc import TransformerMCReader
 
 logger = logging.getLogger(__name__)
 
 
 @DatasetReader.register("swag")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/mc/dataset_readers/transformer_mc.py` & `radgraph-0.0.7/radgraph/allennlp_models/mc/dataset_readers/transformer_mc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import List, Optional
 
 from radgraph.allennlp.data import DatasetReader, Instance
-from overrides import overrides
+from overrides_ import overrides
 
 logger = logging.getLogger(__name__)
 
 
 class TransformerMCReader(DatasetReader):
     """
     Read input data for the TransformerMC model. This is the base class for all readers that produce
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/mc/models/transformer_mc.py` & `radgraph-0.0.7/radgraph/allennlp_models/mc/models/transformer_mc.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/mc/predictors/transformer_mc.py` & `radgraph-0.0.7/radgraph/allennlp_models/mc/predictors/transformer_mc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import Instance
 from radgraph.allennlp.predictors.predictor import Predictor
 
 
 @Predictor.register("transformer_mc")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/pair_classification/dataset_readers/quora_paraphrase.py` & `radgraph-0.0.7/radgraph/allennlp_models/pair_classification/dataset_readers/quora_paraphrase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, Dict
 import logging
 import csv
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import LabelField, TextField, Field
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers import Tokenizer, PretrainedTransformerTokenizer
 from radgraph.allennlp.data.tokenizers.whitespace_tokenizer import WhitespaceTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/pair_classification/dataset_readers/snli.py` & `radgraph-0.0.7/radgraph/allennlp_models/pair_classification/dataset_readers/snli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 from typing import Dict, Optional
 import json
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import Field, TextField, LabelField, MetadataField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
 from radgraph.allennlp.data.tokenizers import Tokenizer, SpacyTokenizer, PretrainedTransformerTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/bimpm.py` & `radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/bimpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 BiMPM (Bilateral Multi-Perspective Matching) model implementation.
 """
 
 from typing import Dict, List, Any
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import numpy
 
 from radgraph.allennlp.common.checks import check_dimensions_match
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.modules import FeedForward, Seq2SeqEncoder, Seq2VecEncoder, TextFieldEmbedder
 from radgraph.allennlp.models.model import Model
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/decomposable_attention.py` & `radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/decomposable_attention.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/pair_classification/models/esim.py` & `radgraph-0.0.7/radgraph/allennlp_models/pair_classification/models/esim.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/pair_classification/predictors/textual_entailment.py` & `radgraph-0.0.7/radgraph/allennlp_models/pair_classification/predictors/textual_entailment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Dict
 
 import numpy
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import Instance
 from radgraph.allennlp.predictors.predictor import Predictor
 from radgraph.allennlp.data.fields import LabelField
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/pretrained.py` & `radgraph-0.0.7/radgraph/allennlp_models/pretrained.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/drop.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/drop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import itertools
 import json
 import logging
 import string
 from collections import defaultdict
 from typing import Dict, List, Union, Tuple, Any
 
-from overrides import overrides
+from overrides_ import overrides
 from word2number.w2n import word_to_num
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.fields import (
     Field,
     TextField,
     MetadataField,
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/qangaroo.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/qangaroo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 
 from typing import Dict, List
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.fields import Field, TextField, ListField, MetadataField, IndexField
 from radgraph.allennlp.data.token_indexers import TokenIndexer, SingleIdTokenIndexer
 from radgraph.allennlp.data.tokenizers import Tokenizer, SpacyTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/quac.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/quac.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 from typing import Any, Dict, List, Tuple
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
 from radgraph.allennlp.data.tokenizers import Token, Tokenizer, SpacyTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/squad.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/squad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
 from typing import Any, Dict, List, Tuple, Optional
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
 from radgraph.allennlp.data.tokenizers import Token, Tokenizer, SpacyTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/transformer_squad.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/transformer_squad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 from typing import Any, Dict, List, Tuple, Optional, Iterable
 
 from radgraph.allennlp.common.util import sanitize_wordpiece
 from radgraph.allennlp.data.fields import MetadataField, TextField, SpanField
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path, open_compressed
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import PretrainedTransformerIndexer
 from radgraph.allennlp.data.tokenizers import Token, PretrainedTransformerTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/triviaqa.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/triviaqa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import logging
 import os
 import tarfile
 from typing import Dict, List, Tuple
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
 from radgraph.allennlp.data.tokenizers import Token, Tokenizer, SpacyTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/dataset_readers/utils.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/dataset_readers/utils.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/metrics/drop_em_and_f1.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/metrics/drop_em_and_f1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 
 from radgraph.allennlp.training.metrics.metric import Metric
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp_models.rc.tools.drop import (
     get_metrics as drop_em_and_f1,
     answer_json_to_strings,
 )
 from radgraph.allennlp_models.rc.tools.squad import metric_max_over_ground_truths
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/metrics/squad_em_and_f1.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/metrics/squad_em_and_f1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple
 
 import torch
 import torch.distributed as dist
 
 from radgraph.allennlp.common.util import is_distributed
 from radgraph.allennlp.training.metrics.metric import Metric
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp_models.rc.tools import squad
 
 
 @Metric.register("squad")
 class SquadEmAndF1(Metric):
     """
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/models/bidaf.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/models/bidaf.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/models/bidaf_ensemble.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/models/bidaf_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Any, Optional
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.models.archival import load_archive
 from radgraph.allennlp.models.model import Model, remove_pretrained_embedding_params
 from radgraph.allennlp.common import Params
 from radgraph.allennlp.data import Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/models/dialog_qa.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/models/dialog_qa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Any, Dict, List, Optional
 import numpy as np
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.nn.functional as F
 from torch.nn.functional import nll_loss
 
 from radgraph.allennlp.common.checks import check_dimensions_match
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.models.model import Model
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/models/naqanet.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/models/naqanet.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/models/qanet.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/models/qanet.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/models/transformer_qa.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/models/transformer_qa.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/models/utils.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/models/utils.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/multi_head_self_attention.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/multi_head_self_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn import Dropout, Linear
 
 from radgraph.allennlp.nn.util import masked_softmax, weighted_sum
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/qanet_encoder.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/qanet_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn import Dropout
 from torch.nn import LayerNorm
 from torch.nn import ModuleList
 from radgraph.allennlp.modules.feedforward import FeedForward
 from radgraph.allennlp.modules.residual_with_layer_dropout import ResidualWithLayerDropout
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/modules/seq2seq_encoders/stacked_self_attention.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/modules/seq2seq_encoders/stacked_self_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn import Dropout
 
 from radgraph.allennlp.modules.feedforward import FeedForward
 from radgraph.allennlp.modules.layer_norm import LayerNorm
 from radgraph.allennlp.modules.seq2seq_encoders.seq2seq_encoder import Seq2SeqEncoder
 from radgraph.allennlp.nn.activations import Activation
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/bidaf.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/bidaf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List
 
-from overrides import overrides
+from overrides_ import overrides
 import numpy
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import Instance
 from radgraph.allennlp.predictors.predictor import Predictor
 from radgraph.allennlp.data.fields import (
     IndexField,
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/dialog_qa.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/dialog_qa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.data import DatasetReader, Instance
 from radgraph.allennlp.data.tokenizers.spacy_tokenizer import SpacyTokenizer
 from radgraph.allennlp.predictors.predictor import Predictor
 from radgraph.allennlp.models import Model
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/predictors/transformer_qa.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/predictors/transformer_qa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Dict, Any
 
 from radgraph.allennlp.models import Model
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import JsonDict, sanitize
 from radgraph.allennlp.data import Instance, DatasetReader
 from radgraph.allennlp.predictors.predictor import Predictor
 
 
 @Predictor.register("transformer_qa")
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/drop.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/drop.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/narrativeqa.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/narrativeqa.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/orb.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/orb.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/orb_utils.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/orb_utils.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/quoref.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/quoref.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/squad.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/squad.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/squad2.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/squad2.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/rc/tools/transformer_qa.py` & `radgraph-0.0.7/radgraph/allennlp_models/rc/tools/transformer_qa.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/__init__.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/__init__.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/penn_tree_bank.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/penn_tree_bank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Tuple
 import logging
 import os
 
-from overrides import overrides
+from overrides_ import overrides
 
 # NLTK is so performance orientated (ha ha) that they have lazy imports. Why? Who knows.
 from nltk.corpus.reader.bracket_parse import BracketParseCorpusReader
 from nltk.tree import Tree
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/semantic_dependencies.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/semantic_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Tuple
 import logging
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import AdjacencyField, MetadataField, SequenceLabelField
 from radgraph.allennlp.data.fields import Field, TextField
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
 from radgraph.allennlp.data.tokenizers import Token
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/srl.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/srl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from typing import Dict, List, Iterable, Tuple, Any
 
-from overrides import overrides
+from overrides_ import overrides
 from transformers.tokenization_bert import BertTokenizer
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import Field, TextField, SequenceLabelField, MetadataField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/dataset_readers/universal_dependencies.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/dataset_readers/universal_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, Tuple, List
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 from conllu import parse_incr
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import Field, TextField, SequenceLabelField, MetadataField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/metrics/srl_eval_scorer.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/metrics/srl_eval_scorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import defaultdict
 import logging
 import os
 import tempfile
 import subprocess
 import shutil
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.training.metrics.metric import Metric
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_SRL_EVAL_PATH = os.path.abspath(
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/biaffine_dependency_parser.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/biaffine_dependency_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Tuple, Any, List
 import logging
 import copy
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 import torch.nn.functional as F
 from torch.nn.modules import Dropout
 import numpy
 
 from radgraph.allennlp.common.checks import check_dimensions_match, ConfigurationError
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/constituency_parser.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/constituency_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, Tuple, List, NamedTuple, Any
-from overrides import overrides
+from overrides_ import overrides
 
 import torch
 from torch.nn.modules.linear import Linear
 from nltk import Tree
 
 from radgraph.allennlp.common.checks import check_dimensions_match
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/graph_parser.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/graph_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Tuple, Any, List
 import logging
 import copy
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.modules import Dropout
 import numpy
 
 from radgraph.allennlp.common.checks import check_dimensions_match, ConfigurationError
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.modules import Seq2SeqEncoder, TextFieldEmbedder, Embedding, InputVariationalDropout
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/srl.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/srl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict, List, TextIO, Optional, Any
 import warnings
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.modules import Linear, Dropout
 import torch.nn.functional as F
 
 from radgraph.allennlp.common.checks import check_dimensions_match
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.modules import Seq2SeqEncoder, TimeDistributed, TextFieldEmbedder
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/models/srl_bert.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/models/srl_bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, List, Any, Union
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.modules import Linear, Dropout
 import torch.nn.functional as F
 from transformers.modeling_bert import BertModel
 
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.models.model import Model
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/biaffine_dependency_parser.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/biaffine_dependency_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Any, List, Tuple
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import JsonDict, sanitize
 from radgraph.allennlp.data import DatasetReader, Instance
 from radgraph.allennlp.models import Model
 from radgraph.allennlp.predictors.predictor import Predictor
 from radgraph.allennlp.data.tokenizers.spacy_tokenizer import SpacyTokenizer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/constituency_parser.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/constituency_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List
 
-from overrides import overrides
+from overrides_ import overrides
 from nltk import Tree
 from spacy.lang.en.tag_map import TAG_MAP
 
 from radgraph.allennlp.common.util import JsonDict, sanitize
 from radgraph.allennlp.data import DatasetReader, Instance
 from radgraph.allennlp.models import Model
 from radgraph.allennlp.predictors.predictor import Predictor
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/openie.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/openie.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Dict
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.util import JsonDict, sanitize
 from radgraph.allennlp.data import DatasetReader, Instance
 from radgraph.allennlp.data.tokenizers import SpacyTokenizer
 from radgraph.allennlp.models import Model
 from radgraph.allennlp.predictors.predictor import Predictor
 from radgraph.allennlp.data.tokenizers import Token
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/predictors/srl.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/predictors/srl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Dict
 
 import numpy
-from overrides import overrides
+from overrides_ import overrides
 from spacy.tokens import Doc
 
 from radgraph.allennlp.common.util import JsonDict, sanitize, group_by_count
 from radgraph.allennlp.data import DatasetReader, Instance
 from radgraph.allennlp.data.tokenizers.spacy_tokenizer import SpacyTokenizer
 from radgraph.allennlp.models import Model
 from radgraph.allennlp.predictors.predictor import Predictor
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/tools/convert_openie_to_conll.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/tools/convert_openie_to_conll.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/structured_prediction/tools/write_srl_predictions_to_conll_format.py` & `radgraph-0.0.7/radgraph/allennlp_models/structured_prediction/tools/write_srl_predictions_to_conll_format.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/ccgbank.py` & `radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/ccgbank.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Sequence
 import logging
 import re
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import Field, TextField, SequenceLabelField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import TokenIndexer, SingleIdTokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/conll2000.py` & `radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/conll2000.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Sequence, Iterable
 import itertools
 import logging
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.dataset_readers.dataset_utils import to_bioul
 from radgraph.allennlp.data.fields import TextField, SequenceLabelField, Field, MetadataField
 from radgraph.allennlp.data.instance import Instance
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/tagging/dataset_readers/ontonotes_ner.py` & `radgraph-0.0.7/radgraph/allennlp_models/tagging/dataset_readers/ontonotes_ner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Dict, List, Iterable
 
 from radgraph.allennlp.data.dataset_readers.dataset_utils import to_bioul
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import Field, TextField, SequenceLabelField, MetadataField
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.token_indexers import SingleIdTokenIndexer, TokenIndexer
```

### Comparing `radgraph-0.0.6/radgraph/allennlp_models/tagging/models/crf_tagger.py` & `radgraph-0.0.7/radgraph/allennlp_models/tagging/models/crf_tagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict, Optional, List, Any, cast
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 from torch.nn.modules.linear import Linear
 
 from radgraph.allennlp.common.checks import check_dimensions_match, ConfigurationError
 from radgraph.allennlp.data import TextFieldTensors, Vocabulary
 from radgraph.allennlp.modules import Seq2SeqEncoder, TimeDistributed, TextFieldEmbedder
 from radgraph.allennlp.modules import ConditionalRandomField, FeedForward
```

### Comparing `radgraph-0.0.6/radgraph/dygie/data/dataset_readers/document.py` & `radgraph-0.0.7/radgraph/dygie/data/dataset_readers/document.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/dygie/data/dataset_readers/dygie.py` & `radgraph-0.0.7/radgraph/dygie/data/dataset_readers/dygie.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Any, Dict, List, Optional, Tuple, DefaultDict, Set, Union
 import json
 import pickle as pkl
 import warnings
 
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.common.file_utils import cached_path
 from radgraph.allennlp.data.dataset_readers.dataset_reader import DatasetReader
 from radgraph.allennlp.data.fields import (ListField, TextField, SpanField, MetadataField,
                                   SequenceLabelField, AdjacencyField, LabelField)
 from radgraph.allennlp.data.instance import Instance
 from radgraph.allennlp.data.tokenizers import Token
```

### Comparing `radgraph-0.0.6/radgraph/dygie/data/fields/adjacency_field_assym.py` & `radgraph-0.0.7/radgraph/dygie/data/fields/adjacency_field_assym.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List, Set, Tuple
 import logging
 import textwrap
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.common.checks import ConfigurationError
 from radgraph.allennlp.data.fields.field import Field
 from radgraph.allennlp.data.fields.sequence_field import SequenceField
 from radgraph.allennlp.data.vocabulary import Vocabulary
```

### Comparing `radgraph-0.0.6/radgraph/dygie/models/coref.py` & `radgraph-0.0.7/radgraph/dygie/models/coref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import math
 from typing import Any, Dict, List, Optional, Tuple, Union, Callable
 
 import torch
 import torch.nn.functional as F
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules.token_embedders import Embedding
 from radgraph.allennlp.modules import FeedForward
 from radgraph.allennlp.modules import TimeDistributed
 from radgraph.allennlp.nn import util, InitializerApplicator, RegularizerApplicator
```

### Comparing `radgraph-0.0.6/radgraph/dygie/models/dygie.py` & `radgraph-0.0.7/radgraph/dygie/models/dygie.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Dict, List, Optional, Union
 import copy
 
 import torch
 import torch.nn.functional as F
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.common.params import Params
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules import TextFieldEmbedder, FeedForward, TimeDistributed
 from radgraph.allennlp.modules.span_extractors import EndpointSpanExtractor
 from radgraph.allennlp.nn import util, InitializerApplicator, RegularizerApplicator
```

### Comparing `radgraph-0.0.6/radgraph/dygie/models/entity_beam_pruner.py` & `radgraph-0.0.7/radgraph/dygie/models/entity_beam_pruner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This is basically a copy of AllenNLP's Pruner module, but with support for entity beams.
 """
 
 from typing import Tuple, Union
 
-from overrides import overrides
+from overrides_ import overrides
 import torch
 
 from radgraph.allennlp.nn import util
 from radgraph.allennlp.modules import TimeDistributed
 
 
 def make_pruner(scorer, entity_beam=False, gold_beam=False):
```

### Comparing `radgraph-0.0.6/radgraph/dygie/models/events.py` & `radgraph-0.0.7/radgraph/dygie/models/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import itertools
 from typing import Any, Dict, List, Optional, Callable
 
 import torch
 from torch.nn import functional as F
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.nn import util, InitializerApplicator, RegularizerApplicator
 from radgraph.allennlp.modules import TimeDistributed
 from radgraph.allennlp.modules.token_embedders import Embedding
```

### Comparing `radgraph-0.0.6/radgraph/dygie/models/ner.py` & `radgraph-0.0.7/radgraph/dygie/models/ner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, Dict, List, Optional, Callable
 
 import torch
 from torch.nn import functional as F
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.modules import TimeDistributed
 from radgraph.allennlp.nn import util, InitializerApplicator, RegularizerApplicator
 
 from radgraph.dygie.training.ner_metrics import NERMetrics
```

### Comparing `radgraph-0.0.6/radgraph/dygie/models/relation.py` & `radgraph-0.0.7/radgraph/dygie/models/relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Any, Dict, List, Optional, Callable
 
 import torch
 import torch.nn.functional as F
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.data import Vocabulary
 from radgraph.allennlp.models.model import Model
 from radgraph.allennlp.nn import util, RegularizerApplicator
 from radgraph.allennlp.modules import TimeDistributed
 
 from radgraph.dygie.training.relation_metrics import RelationMetrics
```

### Comparing `radgraph-0.0.6/radgraph/dygie/models/shared.py` & `radgraph-0.0.7/radgraph/dygie/models/shared.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/dygie/predictors/dygie.py` & `radgraph-0.0.7/radgraph/dygie/predictors/dygie.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 import numpy as np
 import warnings
 
-from overrides import overrides
+from overrides_ import overrides
 import numpy
 import json
 
 from radgraph.allennlp.common.util import JsonDict
 from radgraph.allennlp.nn import util
 from radgraph.allennlp.data import Batch
 from radgraph.allennlp.data import DatasetReader
```

### Comparing `radgraph-0.0.6/radgraph/dygie/training/event_metrics.py` & `radgraph-0.0.7/radgraph/dygie/training/event_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 from collections import Counter
 
 from radgraph.allennlp.training.metrics.metric import Metric
 
 from radgraph.dygie.training.f1 import compute_f1
```

### Comparing `radgraph-0.0.6/radgraph/dygie/training/ner_metrics.py` & `radgraph-0.0.7/radgraph/dygie/training/ner_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 from typing import Optional
 
 import torch
 
 from radgraph.allennlp.training.metrics.metric import Metric
 
 from radgraph.dygie.training.f1 import compute_f1
```

### Comparing `radgraph-0.0.6/radgraph/dygie/training/relation_metrics.py` & `radgraph-0.0.7/radgraph/dygie/training/relation_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from overrides import overrides
+from overrides_ import overrides
 
 from radgraph.allennlp.training.metrics.metric import Metric
 
 from radgraph.dygie.training.f1 import compute_f1
 
 
 class RelationMetrics(Metric):
```

### Comparing `radgraph-0.0.6/radgraph/radgraph.py` & `radgraph-0.0.7/radgraph/radgraph.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/rewards.py` & `radgraph-0.0.7/radgraph/rewards.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph/utils.py` & `radgraph-0.0.7/radgraph/utils.py`

 * *Files identical despite different names*

### Comparing `radgraph-0.0.6/radgraph.egg-info/SOURCES.txt` & `radgraph-0.0.7/radgraph.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
-setup.cfg
 setup.py
+overrides_/__init__.py
+overrides_/enforce.py
+overrides_/final.py
+overrides_/overrides.py
 radgraph/__init__.py
 radgraph/radgraph.py
 radgraph/rewards.py
 radgraph/utils.py
 radgraph.egg-info/PKG-INFO
 radgraph.egg-info/SOURCES.txt
 radgraph.egg-info/dependency_links.txt
@@ -408,8 +411,10 @@
 radgraph/dygie/models/shared.py
 radgraph/dygie/predictors/__init__.py
 radgraph/dygie/predictors/dygie.py
 radgraph/dygie/training/__init__.py
 radgraph/dygie/training/event_metrics.py
 radgraph/dygie/training/f1.py
 radgraph/dygie/training/ner_metrics.py
-radgraph/dygie/training/relation_metrics.py
+radgraph/dygie/training/relation_metrics.py
+tests/__init__.py
+tests/radgraph_test.py
```

### Comparing `radgraph-0.0.6/setup.py` & `radgraph-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-import pathlib
-import sys
 from setuptools import setup, find_packages
 
 setup(
     name='radgraph',
-    version='0.0.6',
+    version='0.0.7',
     author='Jean-Benoit Delbrouck',
     license='MIT',
     classifiers=[
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3 :: Only',
     ],
     install_requires=['torch>=1.8.1',
                       'transformers>=4.23.1',
                       "appdirs",
-                      'overrides==3.1.0',
                       'jsonpickle',
                       'filelock',
                       'h5py',
                       'spacy',
                       'nltk',
                       ],
     packages=find_packages(),
```

