# Comparing `tmp/funasr-0.6.7.tar.gz` & `tmp/funasr-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.6.7.tar", last modified: Thu Jun 29 12:15:05 2023, max compression
+gzip compressed data, was "funasr-0.6.9.tar", last modified: Thu Jul  6 11:10:16 2023, max compression
```

## Comparing `funasr-0.6.7.tar` & `funasr-0.6.9.tar`

### file list

```diff
@@ -1,441 +1,442 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.666676 funasr-0.6.7/
--rw-r--r--   0 zhifu      (502) staff       (20)     9928 2023-06-29 12:15:05.666372 funasr-0.6.7/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     8951 2023-06-27 04:52:41.000000 funasr-0.6.7/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.487311 funasr-0.6.7/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.498405 funasr-0.6.7/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    67983 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    70592 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.7/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.7/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9687 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17782 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12149 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.503637 funasr-0.6.7/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.7/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16902 2023-06-28 08:07:26.000000 funasr-0.6.7/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_model_from_file.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_streaming_iterator.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_sv_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.505104 funasr-0.6.7/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.505808 funasr-0.6.7/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3713 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.507103 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10803 2023-06-27 08:57:43.000000 funasr-0.6.7/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.509391 funasr-0.6.7/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.7/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    30602 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.529864 funasr-0.6.7/funasr/datasets/small_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 13:41:22.000000 funasr-0.6.7/funasr/datasets/small_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/datasets/small_datasets/preprocessor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/datasets/small_datasets/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.530511 funasr-0.6.7/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-06-29 12:09:00.000000 funasr-0.6.7/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.531951 funasr-0.6.7/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.532789 funasr-0.6.7/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.7/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.7/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.534201 funasr-0.6.7/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.7/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.536199 funasr-0.6.7/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.7/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.536764 funasr-0.6.7/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.7/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.538705 funasr-0.6.7/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.7/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.539154 funasr-0.6.7/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.7/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.540695 funasr-0.6.7/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.541946 funasr-0.6.7/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.545554 funasr-0.6.7/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.546162 funasr-0.6.7/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.6.7/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.547738 funasr-0.6.7/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.555668 funasr-0.6.7/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.559513 funasr-0.6.7/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40753 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75359 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15642 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100258 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35177 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-06-20 01:57:45.000000 funasr-0.6.7/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.586384 funasr-0.6.7/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.7/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.7/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.588618 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3552 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56207 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.592475 funasr-0.6.7/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.594162 funasr-0.6.7/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.7/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.7/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.594892 funasr-0.6.7/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.7/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.596061 funasr-0.6.7/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.597231 funasr-0.6.7/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.598892 funasr-0.6.7/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.599703 funasr-0.6.7/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.610655 funasr-0.6.7/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.7/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.613101 funasr-0.6.7/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.7/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.615469 funasr-0.6.7/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.7/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.616278 funasr-0.6.7/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/modules/eend_ola/encoder_decoder_attractor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.617730 funasr-0.6.7/funasr/modules/eend_ola/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 14:53:13.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/losses.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/power.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/modules/eend_ola/utils/report.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.7/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.620128 funasr-0.6.7/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.7/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.7/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.7/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.622062 funasr-0.6.7/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.623607 funasr-0.6.7/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.624840 funasr-0.6.7/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-06-27 03:21:23.000000 funasr-0.6.7/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.625684 funasr-0.6.7/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.626000 funasr-0.6.7/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.626193 funasr-0.6.7/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.626954 funasr-0.6.7/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.7/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.627674 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.630318 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.634317 funasr-0.6.7/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.635686 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.638018 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1588 2023-06-19 11:16:01.000000 funasr-0.6.7/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.640696 funasr-0.6.7/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.642276 funasr-0.6.7/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.646782 funasr-0.6.7/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    72548 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    57686 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.650432 funasr-0.6.7/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.652998 funasr-0.6.7/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.7/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.654812 funasr-0.6.7/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.7/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38470 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.663687 funasr-0.6.7/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-06-26 13:46:26.000000 funasr-0.6.7/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-06-29 11:59:56.000000 funasr-0.6.7/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.7/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-06-29 09:20:46.000000 funasr-0.6.7/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.7/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.7/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.7/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.7/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-06-26 13:46:26.000000 funasr-0.6.7/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-06-29 10:01:51.000000 funasr-0.6.7/funasr/utils/runtime_sdk_download_tool.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.7/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.7/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-06-27 08:57:43.000000 funasr-0.6.7/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.7/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-29 12:03:04.000000 funasr-0.6.7/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.488333 funasr-0.6.7/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     9928 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    14008 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      774 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-29 12:15:05.000000 funasr-0.6.7/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-29 12:15:05.666742 funasr-0.6.7/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-06-29 09:20:46.000000 funasr-0.6.7/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-29 12:15:05.665938 funasr-0.6.7/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26773 2023-06-15 09:10:12.000000 funasr-0.6.7/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.7/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.7/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.7/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.6.7/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-06-28 08:07:26.000000 funasr-0.6.7/tests/test_tp_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.6.7/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.173673 funasr-0.6.9/
+-rw-r--r--   0 zhifu      (502) staff       (20)    10194 2023-07-06 11:10:16.173286 funasr-0.6.9/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     9217 2023-07-06 06:23:18.000000 funasr-0.6.9/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.889404 funasr-0.6.9/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.920998 funasr-0.6.9/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    68295 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    71449 2023-07-06 11:04:13.000000 funasr-0.6.9/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.9/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5565 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9689 2023-07-06 11:07:57.000000 funasr-0.6.9/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17590 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14412 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12057 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     7974 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3844 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9921 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8372 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3339 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9449 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17849 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6457 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12149 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.927161 funasr-0.6.9/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.9/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3987 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18668 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9680 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1693 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1099 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8637 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_model_from_file.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_streaming_iterator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7865 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_sv_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35431 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2324 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.930484 funasr-0.6.9/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4075 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14936 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15737 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.950562 funasr-0.6.9/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3713 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.952530 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10853 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.959003 funasr-0.6.9/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1602 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3118 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    30602 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.961658 funasr-0.6.9/funasr/datasets/small_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 13:41:22.000000 funasr-0.6.9/funasr/datasets/small_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2633 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9596 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32753 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/datasets/small_datasets/preprocessor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7439 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/datasets/small_datasets/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.962546 funasr-0.6.9/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11300 2023-06-29 12:09:00.000000 funasr-0.6.9/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.964319 funasr-0.6.9/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.965827 funasr-0.6.9/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.9/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.9/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.985536 funasr-0.6.9/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.9/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.990430 funasr-0.6.9/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.9/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.991414 funasr-0.6.9/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.9/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.994505 funasr-0.6.9/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.9/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.9/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.995491 funasr-0.6.9/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.9/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.999385 funasr-0.6.9/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2145 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2238 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2242 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2162 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5887 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.012843 funasr-0.6.9/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7727 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1059 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5155 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.023362 funasr-0.6.9/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3418 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2458 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10331 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8876 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2228 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.024914 funasr-0.6.9/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-06-29 08:58:03.000000 funasr-0.6.9/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.029593 funasr-0.6.9/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4610 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4941 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.066277 funasr-0.6.9/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6286 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5204 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.071192 funasr-0.6.9/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40797 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12052 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8274 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75359 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    42807 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16618 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17648 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/models/e2e_asr_bat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15681 2023-07-05 02:29:20.000000 funasr-0.6.9/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11764 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100258 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    34383 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10145 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20486 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18884 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10003 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6601 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51652 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31909 2023-06-20 01:57:45.000000 funasr-0.6.9/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.078993 funasr-0.6.9/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    44937 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20911 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.9/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.9/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17600 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.080872 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10965 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13928 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21089 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3556 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56207 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26809 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.083778 funasr-0.6.9/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12502 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5677 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4908 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20380 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2730 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.084527 funasr-0.6.9/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.9/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.9/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.085121 funasr-0.6.9/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.9/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.086463 funasr-0.6.9/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3545 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.087359 funasr-0.6.9/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40738 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.089351 funasr-0.6.9/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      961 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10177 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5825 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.091925 funasr-0.6.9/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.9/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.100690 funasr-0.6.9/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.9/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.103060 funasr-0.6.9/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.9/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.106498 funasr-0.6.9/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5833 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.9/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.107529 funasr-0.6.9/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/modules/eend_ola/encoder_decoder_attractor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.109035 funasr-0.6.9/funasr/modules/eend_ola/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-06-26 14:53:13.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2761 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/losses.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3386 2023-03-29 08:06:18.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/power.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7336 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/modules/eend_ola/utils/report.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17848 2023-07-05 02:28:53.000000 funasr-0.6.9/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.111842 funasr-0.6.9/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2650 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.9/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22971 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.9/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.114953 funasr-0.6.9/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.117592 funasr-0.6.9/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.119957 funasr-0.6.9/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21806 2023-06-27 03:21:23.000000 funasr-0.6.9/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.121223 funasr-0.6.9/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      747 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.123046 funasr-0.6.9/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.123268 funasr-0.6.9/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.124356 funasr-0.6.9/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.9/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.125110 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.127489 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6966 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4740 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1496 2023-06-30 02:11:21.000000 funasr-0.6.9/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.131021 funasr-0.6.9/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.132845 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.135491 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15774 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9116 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-06-27 11:42:15.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1545 2023-07-06 08:02:59.000000 funasr-0.6.9/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.139211 funasr-0.6.9/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6077 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5635 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5087 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3063 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2859 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.141602 funasr-0.6.9/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1986 2023-07-05 02:28:54.000000 funasr-0.6.9/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3577 2023-07-05 02:28:54.000000 funasr-0.6.9/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1413 2023-07-05 02:28:54.000000 funasr-0.6.9/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.146184 funasr-0.6.9/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    72548 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    62178 2023-07-02 01:20:55.000000 funasr-0.6.9/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11770 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31807 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6438 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7591 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21039 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18434 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10327 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.148911 funasr-0.6.9/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2128 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2149 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1398 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16520 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1213 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2019 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1993 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.151523 funasr-0.6.9/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      971 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3711 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.9/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.153619 funasr-0.6.9/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11394 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2810 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.9/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18005 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38470 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.164166 funasr-0.6.9/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11744 2023-06-26 13:46:26.000000 funasr-0.6.9/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      479 2023-06-29 11:59:56.000000 funasr-0.6.9/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.9/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5551 2023-06-29 09:20:46.000000 funasr-0.6.9/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.9/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.9/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1609 2023-07-06 11:07:58.000000 funasr-0.6.9/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.9/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.9/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10247 2023-06-26 13:46:26.000000 funasr-0.6.9/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1665 2023-06-29 10:01:51.000000 funasr-0.6.9/funasr/utils/runtime_sdk_download_tool.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.9/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.9/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12182 2023-06-27 08:57:43.000000 funasr-0.6.9/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.9/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-07-06 11:09:47.000000 funasr-0.6.9/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:15.909489 funasr-0.6.9/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)    10194 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    14037 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      757 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-07-06 11:10:15.000000 funasr-0.6.9/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-07-06 11:10:16.173784 funasr-0.6.9/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     3630 2023-06-30 02:11:21.000000 funasr-0.6.9/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-07-06 11:10:16.166932 funasr-0.6.9/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    27007 2023-07-05 02:29:20.000000 funasr-0.6.9/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.9/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.9/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.9/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1583 2023-06-20 01:57:45.000000 funasr-0.6.9/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1741 2023-07-05 02:28:54.000000 funasr-0.6.9/tests/test_tp_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-06-20 01:57:45.000000 funasr-0.6.9/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.6.7/PKG-INFO` & `funasr-0.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.7
+Version: 0.6.9
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,16 @@
 Provides-Extra: train
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
 
 [//]: # (<div align="left"><img src="docs/images/funasr_logo.jpg" width="400"/></div>)
 
+([简体中文](./README_zh.md)|English)
+
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 <p align="left">
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Pytorch-%3E%3D1.11-blue"></a>
 </p>
 
@@ -41,17 +43,26 @@
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
+
+### FunASR runtime-SDK
+
+- 2023.07.03: 
+We have release the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
+
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge
+
 We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+
 ### Release notes
+
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker diarization and multi-talker ASR.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved SOTA performance in many speech recognition tasks. 
 - FunASR offers a user-friendly pipeline for fine-tuning pretrained models from the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition). Additionally, the optimized dataloader in FunASR enables faster training speeds for large-scale datasets. This feature enhances the efficiency of the speech recognition process for researchers and practitioners.
 
@@ -121,21 +132,21 @@
 ### runtime
 
 An example with websocket:
 
 For the server:
 ```shell
 cd funasr/runtime/python/websocket
-python wss_srv_asr.py --port 10095
+python funasr_wss_server.py --port 10095
 ```
 
 For the client:
 ```shell
-python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
-#python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
+python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
+#python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ```
 More examples could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/runtime/websocket_python.html#id2)
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.7 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.9 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
 Provides-Extra: train Provides-Extra: all Provides-Extra: test Provides-Extra:
 doc [//]: # (
 [docs/images/funasr_logo.jpg]
-) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
+) ([ç®ä½ä¸­æ](./README_zh.md)|English) # FunASR: A Fundamental End-to-End
+Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
@@ -27,77 +28,80 @@
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Usage**](#usage) | [**Papers**](https://github.com/alibaba-damo-academy/
 FunASR#citations) | [**Runtime**](https://github.com/alibaba-damo-academy/
 FunASR/tree/main/funasr/runtime) | [**Model Zoo**](https://github.com/alibaba-
 damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md) |
 [**Contact**](#contact) | [**M2MET2.0 Challenge**](https://github.com/alibaba-
 damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-
-challenge) ## What's new: ### Multi-Channel Multi-Party Meeting Transcription
-2.0 (M2MeT2.0) Challenge We are pleased to announce that the M2MeT2.0 challenge
-has been accepted by the ASRU 2023 challenge special session. The registration
-is now open. The baseline system is conducted on FunASR and is provided as a
-receipe of AliMeeting corpus. For more details you can see the guidence of
-M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/
-index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/
-index.html)). ### Release notes For the release notes, please ref to [news]
-(https://github.com/alibaba-damo-academy/FunASR/releases) ## Highlights -
-FunASR is a fundamental speech recognition toolkit that offers a variety of
-features, including speech recognition (ASR), Voice Activity Detection (VAD),
-Punctuation Restoration, Language Models, Speaker Verification, Speaker
-diarization and multi-talker ASR. - We have released a vast collection of
-academic and industrial pretrained models on the [ModelScope](https://
-www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be
-accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/
-FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved
-SOTA performance in many speech recognition tasks. - FunASR offers a user-
-friendly pipeline for fine-tuning pretrained models from the [ModelScope]
-(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition).
-Additionally, the optimized dataloader in FunASR enables faster training speeds
-for large-scale datasets. This feature enhances the efficiency of the speech
-recognition process for researchers and practitioners. ## Installation Install
-from pip ```shell pip3 install -U funasr # For the users in China, you could
-install with the command: # pip3 install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip3 install -e ./ #
-For the users in China, you could install with the command: # pip3 install -
-e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip3 install -U modelscope # For the users in China, you could install with the
-command: # pip3 install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Usage You could
-use FunASR by: - egs - egs_modelscope - runtime ### egs If you want to train
-the model from scratch, you could use funasr directly by recipe, as the
-following: ```shell cd egs/aishell/paraformer . ./run.sh --
-CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be found in
-[docs](https://alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/
-quick_start.html) ### egs_modelscope If you want to infer or finetune
-pretraining models from modelscope, you could use funasr by modelscope
-pipeline, as the following: ```python from modelscope.pipelines import pipeline
-from modelscope.utils.constant import Tasks inference_pipeline = pipeline
-( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
+challenge) ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
+the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now
+supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
+are pleased to announce that the M2MeT2.0 challenge has been accepted by the
+ASRU 2023 challenge special session. The registration is now open. The baseline
+system is conducted on FunASR and is provided as a receipe of AliMeeting
+corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
+For the release notes, please ref to [news](https://github.com/alibaba-damo-
+academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+recognition toolkit that offers a variety of features, including speech
+recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
+Language Models, Speaker Verification, Speaker diarization and multi-talker
+ASR. - We have released a vast collection of academic and industrial pretrained
+models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
+speech-recognition), which can be accessed through our [Model Zoo](https://
+github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md). The representative [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
+recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
+pretrained models from the [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
+dataloader in FunASR enables faster training speeds for large-scale datasets.
+This feature enhances the efficiency of the speech recognition process for
+researchers and practitioners. ## Installation Install from pip ```shell pip3
+install -U funasr # For the users in China, you could install with the command:
+# pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
+install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
+&& cd FunASR pip3 install -e ./ # For the users in China, you could install
+with the command: # pip3 install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/
+simple ``` If you want to use the pretrained models in ModelScope, you should
+install the modelscope: ```shell pip3 install -U modelscope # For the users in
+China, you could install with the command: # pip3 install -U modelscope -
+f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Usage You could use FunASR by: - egs - egs_modelscope -
+runtime ### egs If you want to train the model from scratch, you could use
+funasr directly by recipe, as the following: ```shell cd egs/aishell/paraformer
+. ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be
+found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
+modelscope_pipeline/quick_start.html) ### egs_modelscope If you want to infer
+or finetune pretraining models from modelscope, you could use funasr by
+modelscope pipeline, as the following: ```python from modelscope.pipelines
+import pipeline from modelscope.utils.constant import Tasks inference_pipeline
+= pipeline( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
 large_asr_nat-zh-cn-16k-common-vocab8404-pytorch', ) rec_result =
 inference_pipeline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/
 MaaS/ASR/test_audio/asr_example_zh.wav') print(rec_result) # {'text':
 'æ¬¢è¿å¤§å®¶æ¥ä½éªè¾¾æ©é¢æ¨åºçè¯­é³è¯å«æ¨¡å'} ``` More examples
 could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
 modelscope_pipeline/quick_start.html) ### runtime An example with websocket:
 For the server: ```shell cd funasr/runtime/python/websocket python
-wss_srv_asr.py --port 10095 ``` For the client: ```shell python
-wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
-"5,10,5" #python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass
---chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results" ```
-More examples could be found in [docs](https://alibaba-damo-academy.github.io/
-FunASR/en/runtime/websocket_python.html#id2) ## Contact If you have any
-questions about FunASR, please contact us by - email: [funasr@list.alibaba-
-inc.com](funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:
------------------------------------------------------:| |
+funasr_wss_server.py --port 10095 ``` For the client: ```shell python
+funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
+"5,10,5" #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode
+2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
+``` More examples could be found in [docs](https://alibaba-damo-
+academy.github.io/FunASR/en/runtime/websocket_python.html#id2) ## Contact If
+you have any questions about FunASR, please contact us by - email:
+[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
+Wechat group | |:---:|:-----------------------------------------------------:
+| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/aihealthx.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.6.7/README.md` & `funasr-0.6.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 [//]: # (<div align="left"><img src="docs/images/funasr_logo.jpg" width="400"/></div>)
 
+([简体中文](./README_zh.md)|English)
+
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 <p align="left">
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Pytorch-%3E%3D1.11-blue"></a>
 </p>
 
@@ -16,17 +18,26 @@
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
+
+### FunASR runtime-SDK
+
+- 2023.07.03: 
+We have release the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
+
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge
+
 We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+
 ### Release notes
+
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker diarization and multi-talker ASR.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved SOTA performance in many speech recognition tasks. 
 - FunASR offers a user-friendly pipeline for fine-tuning pretrained models from the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition). Additionally, the optimized dataloader in FunASR enables faster training speeds for large-scale datasets. This feature enhances the efficiency of the speech recognition process for researchers and practitioners.
 
@@ -96,21 +107,21 @@
 ### runtime
 
 An example with websocket:
 
 For the server:
 ```shell
 cd funasr/runtime/python/websocket
-python wss_srv_asr.py --port 10095
+python funasr_wss_server.py --port 10095
 ```
 
 For the client:
 ```shell
-python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
-#python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
+python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
+#python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ```
 More examples could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/runtime/websocket_python.html#id2)
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 [//]: # (
 [docs/images/funasr_logo.jpg]
-) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
+) ([ç®ä½ä¸­æ](./README_zh.md)|English) # FunASR: A Fundamental End-to-End
+Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
@@ -14,77 +15,80 @@
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Usage**](#usage) | [**Papers**](https://github.com/alibaba-damo-academy/
 FunASR#citations) | [**Runtime**](https://github.com/alibaba-damo-academy/
 FunASR/tree/main/funasr/runtime) | [**Model Zoo**](https://github.com/alibaba-
 damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md) |
 [**Contact**](#contact) | [**M2MET2.0 Challenge**](https://github.com/alibaba-
 damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-
-challenge) ## What's new: ### Multi-Channel Multi-Party Meeting Transcription
-2.0 (M2MeT2.0) Challenge We are pleased to announce that the M2MeT2.0 challenge
-has been accepted by the ASRU 2023 challenge special session. The registration
-is now open. The baseline system is conducted on FunASR and is provided as a
-receipe of AliMeeting corpus. For more details you can see the guidence of
-M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/
-index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/
-index.html)). ### Release notes For the release notes, please ref to [news]
-(https://github.com/alibaba-damo-academy/FunASR/releases) ## Highlights -
-FunASR is a fundamental speech recognition toolkit that offers a variety of
-features, including speech recognition (ASR), Voice Activity Detection (VAD),
-Punctuation Restoration, Language Models, Speaker Verification, Speaker
-diarization and multi-talker ASR. - We have released a vast collection of
-academic and industrial pretrained models on the [ModelScope](https://
-www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be
-accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/
-FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved
-SOTA performance in many speech recognition tasks. - FunASR offers a user-
-friendly pipeline for fine-tuning pretrained models from the [ModelScope]
-(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition).
-Additionally, the optimized dataloader in FunASR enables faster training speeds
-for large-scale datasets. This feature enhances the efficiency of the speech
-recognition process for researchers and practitioners. ## Installation Install
-from pip ```shell pip3 install -U funasr # For the users in China, you could
-install with the command: # pip3 install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip3 install -e ./ #
-For the users in China, you could install with the command: # pip3 install -
-e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip3 install -U modelscope # For the users in China, you could install with the
-command: # pip3 install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Usage You could
-use FunASR by: - egs - egs_modelscope - runtime ### egs If you want to train
-the model from scratch, you could use funasr directly by recipe, as the
-following: ```shell cd egs/aishell/paraformer . ./run.sh --
-CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be found in
-[docs](https://alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/
-quick_start.html) ### egs_modelscope If you want to infer or finetune
-pretraining models from modelscope, you could use funasr by modelscope
-pipeline, as the following: ```python from modelscope.pipelines import pipeline
-from modelscope.utils.constant import Tasks inference_pipeline = pipeline
-( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
+challenge) ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
+the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now
+supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
+are pleased to announce that the M2MeT2.0 challenge has been accepted by the
+ASRU 2023 challenge special session. The registration is now open. The baseline
+system is conducted on FunASR and is provided as a receipe of AliMeeting
+corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
+For the release notes, please ref to [news](https://github.com/alibaba-damo-
+academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+recognition toolkit that offers a variety of features, including speech
+recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
+Language Models, Speaker Verification, Speaker diarization and multi-talker
+ASR. - We have released a vast collection of academic and industrial pretrained
+models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
+speech-recognition), which can be accessed through our [Model Zoo](https://
+github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md). The representative [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
+recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
+pretrained models from the [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
+dataloader in FunASR enables faster training speeds for large-scale datasets.
+This feature enhances the efficiency of the speech recognition process for
+researchers and practitioners. ## Installation Install from pip ```shell pip3
+install -U funasr # For the users in China, you could install with the command:
+# pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
+install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
+&& cd FunASR pip3 install -e ./ # For the users in China, you could install
+with the command: # pip3 install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/
+simple ``` If you want to use the pretrained models in ModelScope, you should
+install the modelscope: ```shell pip3 install -U modelscope # For the users in
+China, you could install with the command: # pip3 install -U modelscope -
+f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Usage You could use FunASR by: - egs - egs_modelscope -
+runtime ### egs If you want to train the model from scratch, you could use
+funasr directly by recipe, as the following: ```shell cd egs/aishell/paraformer
+. ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be
+found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
+modelscope_pipeline/quick_start.html) ### egs_modelscope If you want to infer
+or finetune pretraining models from modelscope, you could use funasr by
+modelscope pipeline, as the following: ```python from modelscope.pipelines
+import pipeline from modelscope.utils.constant import Tasks inference_pipeline
+= pipeline( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
 large_asr_nat-zh-cn-16k-common-vocab8404-pytorch', ) rec_result =
 inference_pipeline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/
 MaaS/ASR/test_audio/asr_example_zh.wav') print(rec_result) # {'text':
 'æ¬¢è¿å¤§å®¶æ¥ä½éªè¾¾æ©é¢æ¨åºçè¯­é³è¯å«æ¨¡å'} ``` More examples
 could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
 modelscope_pipeline/quick_start.html) ### runtime An example with websocket:
 For the server: ```shell cd funasr/runtime/python/websocket python
-wss_srv_asr.py --port 10095 ``` For the client: ```shell python
-wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
-"5,10,5" #python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass
---chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results" ```
-More examples could be found in [docs](https://alibaba-damo-academy.github.io/
-FunASR/en/runtime/websocket_python.html#id2) ## Contact If you have any
-questions about FunASR, please contact us by - email: [funasr@list.alibaba-
-inc.com](funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:
------------------------------------------------------:| |
+funasr_wss_server.py --port 10095 ``` For the client: ```shell python
+funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
+"5,10,5" #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode
+2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
+``` More examples could be found in [docs](https://alibaba-damo-
+academy.github.io/FunASR/en/runtime/websocket_python.html#id2) ## Contact If
+you have any questions about FunASR, please contact us by - email:
+[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
+Wechat group | |:---:|:-----------------------------------------------------:
+| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/aihealthx.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.6.7/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.6.9/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/asr_infer.py` & `funasr-0.6.9/funasr/bin/asr_infer.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,15 @@
             ctc_weight: float = 0.5,
             lm_weight: float = 1.0,
             ngram_weight: float = 0.9,
             penalty: float = 0.0,
             nbest: int = 1,
             frontend_conf: dict = None,
             hotword_list_or_file: str = None,
+            clas_scale: float = 1.0,
             decoding_ind: int = 0,
             **kwargs,
     ):
 
         # 1. Build ASR model
         scorers = {}
         asr_model, asr_train_args = build_model_from_file(
@@ -372,14 +373,15 @@
         self.converter = converter
         self.tokenizer = tokenizer
         self.cmvn_file = cmvn_file
 
         # 6. [Optional] Build hotword list from str, local file or url
         self.hotword_list = None
         self.hotword_list = self.generate_hotwords_list(hotword_list_or_file)
+        self.clas_scale = clas_scale
 
         is_use_lm = lm_weight != 0.0 and lm_file is not None
         if (ctc_weight == 0.0 or asr_model.ctc == None) and not is_use_lm:
             beam_search = None
         self.beam_search = beam_search
         logging.info(f"Beam_search: {self.beam_search}")
         self.beam_search_transducer = beam_search_transducer
@@ -435,24 +437,28 @@
 
         predictor_outs = self.asr_model.calc_predictor(enc, enc_len)
         pre_acoustic_embeds, pre_token_length, alphas, pre_peak_index = predictor_outs[0], predictor_outs[1], \
                                                                         predictor_outs[2], predictor_outs[3]
         pre_token_length = pre_token_length.round().long()
         if torch.max(pre_token_length) < 1:
             return []
-        if not isinstance(self.asr_model, ContextualParaformer) and not isinstance(self.asr_model,
-                                                                                   NeatContextualParaformer):
+        if not isinstance(self.asr_model, ContextualParaformer) and \
+            not isinstance(self.asr_model, NeatContextualParaformer):
             if self.hotword_list:
                 logging.warning("Hotword is given but asr model is not a ContextualParaformer.")
             decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds,
                                                                      pre_token_length)
             decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
         else:
-            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, enc_len, pre_acoustic_embeds,
-                                                                     pre_token_length, hw_list=self.hotword_list)
+            decoder_outs = self.asr_model.cal_decoder_with_predictor(enc, 
+                                                                     enc_len, 
+                                                                     pre_acoustic_embeds,
+                                                                     pre_token_length, 
+                                                                     hw_list=self.hotword_list,
+                                                                     clas_scale=self.clas_scale)
             decoder_out, ys_pad_lens = decoder_outs[0], decoder_outs[1]
 
         if isinstance(self.asr_model, BiCifParaformer):
             _, _, us_alphas, us_peaks = self.asr_model.calc_predictor_timestamp(enc, enc_len,
                                                                                 pre_token_length)  # test no bias cif2
 
         results = []
```

### Comparing `funasr-0.6.7/funasr/bin/asr_inference_launch.py` & `funasr-0.6.9/funasr/bin/asr_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,16 +251,18 @@
         format="%(asctime)s (%(module)s:%(lineno)d) %(levelname)s: %(message)s",
     )
 
     export_mode = False
     if param_dict is not None:
         hotword_list_or_file = param_dict.get('hotword')
         export_mode = param_dict.get("export_mode", False)
+        clas_scale = param_dict.get('clas_scale', 1.0)
     else:
         hotword_list_or_file = None
+        clas_scale = 1.0
 
     if kwargs.get("device", None) == "cpu":
         ngpu = 0
     if ngpu >= 1 and torch.cuda.is_available():
         device = "cuda"
     else:
         device = "cpu"
@@ -285,14 +287,15 @@
         beam_size=beam_size,
         ctc_weight=ctc_weight,
         lm_weight=lm_weight,
         ngram_weight=ngram_weight,
         penalty=penalty,
         nbest=nbest,
         hotword_list_or_file=hotword_list_or_file,
+        clas_scale=clas_scale,
     )
 
     speech2text = Speech2TextParaformer(**speech2text_kwargs)
 
     if timestamp_model_file is not None:
         speechtext2timestamp = Speech2Timestamp(
             timestamp_cmvn_file=cmvn_file,
@@ -613,18 +616,35 @@
             speech, speech_lengths = batch["speech"], batch["speech_lengths"]
 
             n = len(vadsegments)
             data_with_index = [(vadsegments[i], i) for i in range(n)]
             sorted_data = sorted(data_with_index, key=lambda x: x[0][1] - x[0][0])
             results_sorted = []
             
+            if not len(sorted_data):
+                key = keys[0]
+                # no active segments after VAD
+                if writer is not None:
+                    # Write empty results
+                    ibest_writer["token"][key] = ""
+                    ibest_writer["token_int"][key] = ""
+                    ibest_writer["vad"][key] = ""
+                    ibest_writer["text"][key] = ""
+                    ibest_writer["text_with_punc"][key] = ""
+                    if use_timestamp:
+                        ibest_writer["time_stamp"][key] = ""
+
+                logging.info("decoding, utt: {}, empty speech".format(key))
+                continue
+
             batch_size_token_ms = batch_size_token*60
             if speech2text.device == "cpu":
                 batch_size_token_ms = 0
-            batch_size_token_ms = max(batch_size_token_ms, sorted_data[0][0][1] - sorted_data[0][0][0])
+            if len(sorted_data) > 0 and len(sorted_data[0]) > 0:
+                batch_size_token_ms = max(batch_size_token_ms, sorted_data[0][0][1] - sorted_data[0][0][0])
             
             batch_size_token_ms_cum = 0
             beg_idx = 0
             for j, _ in enumerate(range(0, n)):
                 batch_size_token_ms_cum += (sorted_data[j][0][1] - sorted_data[j][0][0])
                 if j < n - 1 and (batch_size_token_ms_cum + sorted_data[j + 1][0][1] - sorted_data[j + 1][0][
                     0]) < batch_size_token_ms:
@@ -1345,18 +1365,15 @@
         quantize_dtype=quantize_dtype,
         streaming=streaming,
         simu_streaming=simu_streaming,
         chunk_size=chunk_size,
         left_context=left_context,
         right_context=right_context,
     )
-    speech2text = Speech2TextTransducer.from_pretrained(
-        model_tag=model_tag,
-        **speech2text_kwargs,
-    )
+    speech2text = Speech2TextTransducer(**speech2text_kwargs)
 
     def _forward(data_path_and_name_and_type,
                  raw_inputs: Union[np.ndarray, torch.Tensor] = None,
                  output_dir_v2: Optional[str] = None,
                  fs: dict = None,
                  param_dict: dict = None,
                  **kwargs,
@@ -1600,14 +1617,16 @@
         return inference_paraformer_online(**kwargs)
     elif mode.startswith("paraformer_vad"):
         return inference_paraformer_vad_punc(**kwargs)
     elif mode == "mfcca":
         return inference_mfcca(**kwargs)
     elif mode == "rnnt":
         return inference_transducer(**kwargs)
+    elif mode == "bat":
+        return inference_transducer(**kwargs)
     elif mode == "sa_asr":
         return inference_sa_asr(**kwargs)
     else:
         logging.info("Unknown decoding mode: {}".format(mode))
         return None
```

### Comparing `funasr-0.6.7/funasr/bin/asr_train.py` & `funasr-0.6.9/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/build_trainer.py` & `funasr-0.6.9/funasr/bin/build_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,15 +81,17 @@
     # overwrite parameters
     with open(config) as f:
         configs = yaml.safe_load(f)
     with open(finetune_config) as f:
         finetune_configs = yaml.safe_load(f)
         # set data_types
         if dataset_type == "large":
-            finetune_configs["dataset_conf"]["data_types"] = "sound,text"
+            # finetune_configs["dataset_conf"]["data_types"] = "sound,text"
+            if 'data_types' not in finetune_configs['dataset_conf']:
+                finetune_configs["dataset_conf"]["data_types"] = "sound,text"
     finetune_configs = update_dct(configs, finetune_configs)
     for key, value in finetune_configs.items():
         if hasattr(args, key):
             setattr(args, key, value)
 
     # prepare data
     args.dataset_type = dataset_type
```

### Comparing `funasr-0.6.7/funasr/bin/data2vec_train.py` & `funasr-0.6.9/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/diar_infer.py` & `funasr-0.6.9/funasr/bin/diar_infer.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                     in_utt = False
             if in_utt:
                 turn_list.append([spk_list[k], start, length - start])
         return turn_list
 
     @staticmethod
     def seq2arr(seq, vec_dim=8):
-        def int2vec(x, vec_dim=8, dtype=np.int):
+        def int2vec(x, vec_dim=8, dtype=np.int32):
             b = ('{:0' + str(vec_dim) + 'b}').format(x)
             # little-endian order: lower bit first
             return (np.array(list(b)[::-1]) == '1').astype(dtype)
 
         # process oov
         seq = np.array([int(x) for x in seq])
         new_seq = []
```

### Comparing `funasr-0.6.7/funasr/bin/diar_inference_launch.py` & `funasr-0.6.9/funasr/bin/diar_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,35 +88,29 @@
             sv_model_file=sv_model_file,
             device=device,
             dtype=dtype,
             streaming=streaming,
             embedding_node="resnet1_dense"
         )
         logging.info("speech2xvector_kwargs: {}".format(speech2xvector_kwargs))
-        speech2xvector = Speech2Xvector.from_pretrained(
-            model_tag=model_tag,
-            **speech2xvector_kwargs,
-        )
+        speech2xvector = Speech2Xvector(**speech2xvector_kwargs)
         speech2xvector.sv_model.eval()
 
     # 2b. Build speech2diar
     speech2diar_kwargs = dict(
         diar_train_config=diar_train_config,
         diar_model_file=diar_model_file,
         device=device,
         dtype=dtype,
         streaming=streaming,
         smooth_size=smooth_size,
         dur_threshold=dur_threshold,
     )
     logging.info("speech2diarization_kwargs: {}".format(speech2diar_kwargs))
-    speech2diar = Speech2DiarizationSOND.from_pretrained(
-        model_tag=model_tag,
-        **speech2diar_kwargs,
-    )
+    speech2diar = Speech2DiarizationSOND(**speech2diar_kwargs)
     speech2diar.diar_model.eval()
 
     def output_results_str(results: dict, uttid: str):
         rst = []
         mid = uttid.rsplit("-", 1)[0]
         for key in results:
             results[key] = [(x[0] / 100, x[1] / 100) for x in results[key]]
@@ -253,18 +247,15 @@
     speech2diar_kwargs = dict(
         diar_train_config=diar_train_config,
         diar_model_file=diar_model_file,
         device=device,
         dtype=dtype,
     )
     logging.info("speech2diarization_kwargs: {}".format(speech2diar_kwargs))
-    speech2diar = Speech2DiarizationEEND.from_pretrained(
-        model_tag=model_tag,
-        **speech2diar_kwargs,
-    )
+    speech2diar = Speech2DiarizationEEND(**speech2diar_kwargs)
     speech2diar.diar_model.eval()
 
     def output_results_str(results: dict, uttid: str):
         rst = []
         mid = uttid.rsplit("-", 1)[0]
         for key in results:
             results[key] = [(x[0] / 100, x[1] / 100) for x in results[key]]
```

### Comparing `funasr-0.6.7/funasr/bin/diar_train.py` & `funasr-0.6.9/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/lm_inference_launch.py` & `funasr-0.6.9/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/lm_train.py` & `funasr-0.6.9/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/punc_infer.py` & `funasr-0.6.9/funasr/bin/punc_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/punc_inference_launch.py` & `funasr-0.6.9/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/punc_train.py` & `funasr-0.6.9/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/sa_asr_train.py` & `funasr-0.6.9/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/sv_infer.py` & `funasr-0.6.9/funasr/bin/sv_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/sv_inference_launch.py` & `funasr-0.6.9/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/tokenize_text.py` & `funasr-0.6.9/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/tp_infer.py` & `funasr-0.6.9/funasr/bin/tp_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/tp_inference_launch.py` & `funasr-0.6.9/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/train.py` & `funasr-0.6.9/funasr/bin/train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/vad_infer.py` & `funasr-0.6.9/funasr/bin/vad_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/bin/vad_inference_launch.py` & `funasr-0.6.9/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_args.py` & `funasr-0.6.9/funasr/build_utils/build_args.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_asr_model.py` & `funasr-0.6.9/funasr/build_utils/build_asr_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.decoder.transformer_decoder import SAAsrTransformerDecoder
 from funasr.models.e2e_asr import ASRModel
 from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.models.e2e_asr_mfcca import MFCCA
 
 from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
+from funasr.models.e2e_asr_bat import BATModel
 
 from funasr.models.e2e_sa_asr import SAASRModel
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
 
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
@@ -42,15 +43,15 @@
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.default import MultiChannelFrontend
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.frontend.windowing import SlidingWindow
 from funasr.models.joint_net.joint_network import JointNetwork
-from funasr.models.predictor.cif import CifPredictor, CifPredictorV2, CifPredictorV3
+from funasr.models.predictor.cif import CifPredictor, CifPredictorV2, CifPredictorV3, BATPredictor
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
 from funasr.modules.subsampling import Conv1dSubsampling
 from funasr.torch_utils.initialize import initialize
 from funasr.train.class_choices import ClassChoices
 
 frontend_choices = ClassChoices(
@@ -95,15 +96,15 @@
         contextual_paraformer=ContextualParaformer,
         neatcontextual_paraformer=NeatContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
         rnnt=TransducerModel,
         rnnt_unified=UnifiedTransducerModel,
         sa_asr=SAASRModel,
-
+        bat=BATModel,
     ),
     default="asr",
 )
 encoder_choices = ClassChoices(
     "encoder",
     classes=dict(
         conformer=ConformerEncoder,
@@ -184,14 +185,15 @@
 predictor_choices = ClassChoices(
     name="predictor",
     classes=dict(
         cif_predictor=CifPredictor,
         ctc_predictor=None,
         cif_predictor_v2=CifPredictorV2,
         cif_predictor_v3=CifPredictorV3,
+        bat_predictor=BATPredictor,
     ),
     default="cif_predictor",
     optional=True,
 )
 predictor_choices2 = ClassChoices(
     name="predictor2",
     classes=dict(
@@ -309,20 +311,23 @@
         normalize = None
 
     # encoder
     encoder_class = encoder_choices.get_class(args.encoder)
     encoder = encoder_class(input_size=input_size, **args.encoder_conf)
 
     # decoder
-    decoder_class = decoder_choices.get_class(args.decoder)
-    decoder = decoder_class(
-        vocab_size=vocab_size,
-        encoder_output_size=encoder.output_size(),
-        **args.decoder_conf,
-    )
+    if hasattr(args, "decoder") and args.decoder is not None:
+        decoder_class = decoder_choices.get_class(args.decoder)
+        decoder = decoder_class(
+            vocab_size=vocab_size,
+            encoder_output_size=encoder.output_size(),
+            **args.decoder_conf,
+        )
+    else:
+        decoder = None
 
     # ctc
     ctc = CTC(
         odim=vocab_size, encoder_output_size=encoder.output_size(), **args.ctc_conf
     )
 
     if args.model in ["asr", "mfcca"]:
@@ -459,14 +464,61 @@
             normalize=normalize,
             encoder=encoder,
             decoder=decoder,
             att_decoder=att_decoder,
             joint_network=joint_network,
             **args.model_conf,
         )
+    elif args.model == "bat":
+        # 5. Decoder
+        encoder_output_size = encoder.output_size()
+
+        rnnt_decoder_class = rnnt_decoder_choices.get_class(args.rnnt_decoder)
+        decoder = rnnt_decoder_class(
+            vocab_size,
+            **args.rnnt_decoder_conf,
+        )
+        decoder_output_size = decoder.output_size
+
+        if getattr(args, "decoder", None) is not None:
+            att_decoder_class = decoder_choices.get_class(args.decoder)
+
+            att_decoder = att_decoder_class(
+                vocab_size=vocab_size,
+                encoder_output_size=encoder_output_size,
+                **args.decoder_conf,
+            )
+        else:
+            att_decoder = None
+        # 6. Joint Network
+        joint_network = JointNetwork(
+            vocab_size,
+            encoder_output_size,
+            decoder_output_size,
+            **args.joint_network_conf,
+        )
+
+        predictor_class = predictor_choices.get_class(args.predictor)
+        predictor = predictor_class(**args.predictor_conf)
+
+        model_class = model_choices.get_class(args.model)
+        # 7. Build model
+        model = model_class(
+            vocab_size=vocab_size,
+            token_list=token_list,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            encoder=encoder,
+            decoder=decoder,
+            att_decoder=att_decoder,
+            joint_network=joint_network,
+            predictor=predictor,
+            **args.model_conf,
+        )
     elif args.model == "sa_asr":
         asr_encoder_class = asr_encoder_choices.get_class(args.asr_encoder)
         asr_encoder = asr_encoder_class(input_size=input_size, **args.asr_encoder_conf)
         spk_encoder_class = spk_encoder_choices.get_class(args.spk_encoder)
         spk_encoder = spk_encoder_class(input_size=input_size, **args.spk_encoder_conf)
         decoder = decoder_class(
             vocab_size=vocab_size,
```

### Comparing `funasr-0.6.7/funasr/build_utils/build_dataloader.py` & `funasr-0.6.9/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_diar_model.py` & `funasr-0.6.9/funasr/build_utils/build_diar_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_distributed.py` & `funasr-0.6.9/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_lm_model.py` & `funasr-0.6.9/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_model.py` & `funasr-0.6.9/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_model_from_file.py` & `funasr-0.6.9/funasr/build_utils/build_model_from_file.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_optimizer.py` & `funasr-0.6.9/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_pretrain_model.py` & `funasr-0.6.9/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_punc_model.py` & `funasr-0.6.9/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_scheduler.py` & `funasr-0.6.9/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_streaming_iterator.py` & `funasr-0.6.9/funasr/build_utils/build_streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_sv_model.py` & `funasr-0.6.9/funasr/build_utils/build_sv_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_trainer.py` & `funasr-0.6.9/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/build_utils/build_vad_model.py` & `funasr-0.6.9/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/collate_fn.py` & `funasr-0.6.9/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/dataset.py` & `funasr-0.6.9/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/iterable_dataset.py` & `funasr-0.6.9/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.6.9/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.6.9/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.6.9/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/dataset.py` & `funasr-0.6.9/funasr/datasets/large_datasets/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,30 +198,32 @@
             batch_mode="padding"):
     scp_lists = read_lists(data_list_file)
     shuffle = conf.get('shuffle', True)
     data_names = conf.get("data_names", "speech,text")
     data_types = conf.get("data_types", "kaldi_ark,text")
 
     pre_hwfile = conf.get("pre_hwlist", None)
-    pre_prob = conf.get("pre_prob", 0)  # unused yet
-
-    hw_config = {"sample_rate": conf.get("sample_rate", 0.6),
-                 "double_rate": conf.get("double_rate", 0.1),
-                 "hotword_min_length": conf.get("hotword_min_length", 2),
-                 "hotword_max_length": conf.get("hotword_max_length", 8),
-                 "pre_prob": conf.get("pre_prob", 0.0)}
-
+    # pre_prob = conf.get("pre_prob", 0)  # unused yet
     if pre_hwfile is not None:
         pre_hwlist = []
         with open(pre_hwfile, 'r') as fin:
             for line in fin.readlines():
                 pre_hwlist.append(line.strip())
     else:
         pre_hwlist = None
 
+    hw_config = {"sample_rate": conf.get("sample_rate", 0.6),
+                 "double_rate": conf.get("double_rate", 0.1),
+                 "hotword_min_length": conf.get("hotword_min_length", 2),
+                 "hotword_max_length": conf.get("hotword_max_length", 8),
+                 "pre_prob": conf.get("pre_prob", 0.0),
+                 "pre_hwlist": pre_hwlist}
+
+    
+
     dataset = AudioDataset(scp_lists, 
                            data_names, 
                            data_types, 
                            frontend_conf=frontend_conf, 
                            shuffle=shuffle,
                            speed_perturb=speed_perturb,
                            mode=mode,
```

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.6.9/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.6.9/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.6.9/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 def sample_hotword(length, 
                    hotword_min_length, 
                    hotword_max_length,
                    sample_rate,
                    double_rate,
                    pre_prob,
-                   pre_index=None):
+                   pre_index=None,
+                   pre_hwlist=None):
         if length < hotword_min_length:
             return [-1]
         if random.random() < sample_rate:
             if pre_prob > 0 and random.random() < pre_prob and pre_index is not None:
                 return pre_index
             if length == hotword_min_length:
                 return [0, length-1]
```

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.6.9/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.6.9/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.6.9/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,15 +50,25 @@
         text = bpe_tokenizer.text2tokens(" ".join(text))
     if seg_dict is not None:
         assert isinstance(seg_dict, dict)
         text = seg_tokenize(text, seg_dict)
 
     length = len(text)
     if 'hw_tag' in data:
-        hotword_indxs = sample_hotword(length, **hw_config)
+        if hw_config['pre_hwlist'] is not None and hw_config['pre_prob'] > 0:
+            # enable preset hotword detect in sampling
+            pre_index = None
+            for hw in hw_config['pre_hwlist']:
+                hw = " ".join(seg_tokenize(hw, seg_dict))
+                _find = " ".join(text).find(hw)
+                if _find != -1:
+                    # _find = text[:_find].count(" ")  # bpe sometimes
+                    pre_index = [_find, _find + max(hw.count(" "), 1)]
+                    break
+        hotword_indxs = sample_hotword(length, **hw_config, pre_index=pre_index)
         data['hotword_indxs'] = hotword_indxs
         del data['hw_tag']
     for i in range(length):
         x = text[i]
         if i == length-1 and "punc" in data and x.startswith("vad:"):
             vad = x[4:]
             if len(vad) == 0:
```

### Comparing `funasr-0.6.7/funasr/datasets/ms_dataset.py` & `funasr-0.6.9/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/preprocessor.py` & `funasr-0.6.9/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/small_datasets/collate_fn.py` & `funasr-0.6.9/funasr/datasets/small_datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/small_datasets/dataset.py` & `funasr-0.6.9/funasr/datasets/small_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/small_datasets/length_batch_sampler.py` & `funasr-0.6.9/funasr/datasets/small_datasets/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/small_datasets/preprocessor.py` & `funasr-0.6.9/funasr/datasets/small_datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/datasets/small_datasets/sequence_iter_factory.py` & `funasr-0.6.9/funasr/datasets/small_datasets/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/export_model.py` & `funasr-0.6.9/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/CT_Transformer.py` & `funasr-0.6.9/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/__init__.py` & `funasr-0.6.9/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.6.9/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.6.9/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.6.9/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/e2e_vad.py` & `funasr-0.6.9/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.6.9/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.6.9/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.6.9/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/modules/decoder_layer.py` & `funasr-0.6.9/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/modules/encoder_layer.py` & `funasr-0.6.9/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/modules/feedforward.py` & `funasr-0.6.9/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/modules/multihead_att.py` & `funasr-0.6.9/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/models/predictor/cif.py` & `funasr-0.6.9/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/test/test_onnx.py` & `funasr-0.6.9/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/test/test_onnx_punc.py` & `funasr-0.6.9/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.6.9/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/test/test_onnx_vad.py` & `funasr-0.6.9/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/export/utils/torch_function.py` & `funasr-0.6.9/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/fileio/datadir_writer.py` & `funasr-0.6.9/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/fileio/npy_scp.py` & `funasr-0.6.9/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/fileio/rand_gen_dataset.py` & `funasr-0.6.9/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/fileio/read_text.py` & `funasr-0.6.9/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/fileio/sound_scp.py` & `funasr-0.6.9/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/iterators/chunk_iter_factory.py` & `funasr-0.6.9/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/iterators/multiple_iter_factory.py` & `funasr-0.6.9/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/iterators/sequence_iter_factory.py` & `funasr-0.6.9/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/complex_utils.py` & `funasr-0.6.9/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/global_mvn.py` & `funasr-0.6.9/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/label_aggregation.py` & `funasr-0.6.9/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/log_mel.py` & `funasr-0.6.9/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/mask_along_axis.py` & `funasr-0.6.9/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/sinc_conv.py` & `funasr-0.6.9/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/stft.py` & `funasr-0.6.9/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/time_warp.py` & `funasr-0.6.9/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/layers/utterance_mvn.py` & `funasr-0.6.9/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/losses/label_smoothing_loss.py` & `funasr-0.6.9/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/main_funcs/average_nbest_models.py` & `funasr-0.6.9/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.6.9/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/main_funcs/collect_stats.py` & `funasr-0.6.9/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/main_funcs/pack_funcs.py` & `funasr-0.6.9/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/ctc.py` & `funasr-0.6.9/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/data2vec.py` & `funasr-0.6.9/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/decoder/contextual_decoder.py` & `funasr-0.6.9/funasr/models/decoder/contextual_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,14 +240,15 @@
     def forward(
         self,
         hs_pad: torch.Tensor,
         hlens: torch.Tensor,
         ys_in_pad: torch.Tensor,
         ys_in_lens: torch.Tensor,
         contextual_info: torch.Tensor,
+        clas_scale: float = 1.0,
         return_hidden: bool = False,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Forward decoder.
 
         Args:
             hs_pad: encoded memory, float32  (batch, maxlen_in, feat)
             hlens: (batch)
@@ -279,15 +280,15 @@
 
         # contextual paraformer related
         contextual_length = torch.Tensor([contextual_info.shape[1]]).int().repeat(hs_pad.shape[0])
         contextual_mask = myutils.sequence_mask(contextual_length, device=memory.device)[:, None, :]
         cx, tgt_mask, _, _, _ = self.bias_decoder(x_self_attn, tgt_mask, contextual_info, memory_mask=contextual_mask)
 
         if self.bias_output is not None:
-            x = torch.cat([x_src_attn, cx], dim=2)
+            x = torch.cat([x_src_attn, cx*clas_scale], dim=2)
             x = self.bias_output(x.transpose(1, 2)).transpose(1, 2)  # 2D -> D
             x = x_self_attn + self.dropout(x)
 
         if self.decoders2 is not None:
             x, tgt_mask, memory, memory_mask, _ = self.decoders2(
                 x, tgt_mask, memory, memory_mask
             )
```

### Comparing `funasr-0.6.7/funasr/models/decoder/rnn_decoder.py` & `funasr-0.6.9/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.6.9/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/decoder/sanm_decoder.py` & `funasr-0.6.9/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/decoder/sv_decoder.py` & `funasr-0.6.9/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/decoder/transformer_decoder.py` & `funasr-0.6.9/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_asr.py` & `funasr-0.6.9/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_asr_common.py` & `funasr-0.6.9/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.6.9/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
             input_mask = input_mask.masked_fill(~nonpad_positions, False)
             input_mask_expand_dim = input_mask.unsqueeze(2).to(pre_acoustic_embeds.device)
 
         sematic_embeds = pre_acoustic_embeds.masked_fill(~input_mask_expand_dim, 0) + ys_pad_embed.masked_fill(
             input_mask_expand_dim, 0)
         return sematic_embeds * tgt_mask, decoder_out * tgt_mask
 
-    def cal_decoder_with_predictor(self, encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, hw_list=None):
+    def cal_decoder_with_predictor(self, encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, hw_list=None, clas_scale=1.0):
         if hw_list is None:
             hw_list = [torch.Tensor([1]).long().to(encoder_out.device)]  # empty hotword list
             hw_list_pad = pad_list(hw_list, 0)
             if self.use_decoder_embedding:
                 hw_embed = self.decoder.embed(hw_list_pad)
             else:
                 hw_embed = self.bias_embed(hw_list_pad)
@@ -359,12 +359,12 @@
                 hw_embed = self.bias_embed(hw_list_pad)
             hw_embed = torch.nn.utils.rnn.pack_padded_sequence(hw_embed, hw_lengths, batch_first=True,
                                                             enforce_sorted=False)
             _, (h_n, _) = self.bias_encoder(hw_embed)
             hw_embed = h_n.repeat(encoder_out.shape[0], 1, 1)
         
         decoder_outs = self.decoder(
-            encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, contextual_info=hw_embed
+            encoder_out, encoder_out_lens, sematic_embeds, ys_pad_lens, contextual_info=hw_embed, clas_scale=clas_scale
         )
         decoder_out = decoder_outs[0]
         decoder_out = torch.log_softmax(decoder_out, dim=-1)
         return decoder_out, ys_pad_lens
```

### Comparing `funasr-0.6.7/funasr/models/e2e_asr_mfcca.py` & `funasr-0.6.9/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_asr_paraformer.py` & `funasr-0.6.9/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_asr_transducer.py` & `funasr-0.6.9/funasr/models/e2e_asr_transducer.py`

 * *Files 5% similar despite different names*

```diff
@@ -349,35 +349,24 @@
             loss_transducer: Transducer loss value.
             cer_transducer: Character error rate for Transducer.
             wer_transducer: Word Error Rate for Transducer.
 
         """
         if self.criterion_transducer is None:
             try:
-                # from warprnnt_pytorch import RNNTLoss
-	        # self.criterion_transducer = RNNTLoss(
-                    # reduction="mean",
-                    # fastemit_lambda=self.fastemit_lambda,
-                # )
                 from warp_rnnt import rnnt_loss as RNNTLoss
                 self.criterion_transducer = RNNTLoss
 
             except ImportError:
                 logging.error(
                     "warp-rnnt was not installed."
                     "Please consult the installation documentation."
                 )
                 exit(1)
 
-        # loss_transducer = self.criterion_transducer(
-        #     joint_out,
-        #     target,
-        #     t_len,
-        #     u_len,
-        # )
         log_probs = torch.log_softmax(joint_out, dim=-1)
 
         loss_transducer = self.criterion_transducer(
                 log_probs,
                 target,
                 t_len,
                 u_len,
@@ -633,15 +622,14 @@
             == speech_lengths.shape[0]
             == text.shape[0]
             == text_lengths.shape[0]
         ), (speech.shape, speech_lengths.shape, text.shape, text_lengths.shape)
 
         batch_size = speech.shape[0]
         text = text[:, : text_lengths.max()]
-        #print(speech.shape)
         # 1. Encoder
         encoder_out, encoder_out_chunk, encoder_out_lens = self.encode(speech, speech_lengths)
 
         loss_att, loss_att_chunk = 0.0, 0.0
 
         if self.use_auxiliary_att:
             loss_att, _ = self._calc_att_loss(
@@ -850,35 +838,24 @@
         Return:
             loss_transducer: Transducer loss value.
             cer_transducer: Character error rate for Transducer.
             wer_transducer: Word Error Rate for Transducer.
         """
         if self.criterion_transducer is None:
             try:
-                # from warprnnt_pytorch import RNNTLoss
-            # self.criterion_transducer = RNNTLoss(
-                    # reduction="mean",
-                    # fastemit_lambda=self.fastemit_lambda,
-                # )
                 from warp_rnnt import rnnt_loss as RNNTLoss
                 self.criterion_transducer = RNNTLoss
 
             except ImportError:
                 logging.error(
                     "warp-rnnt was not installed."
                     "Please consult the installation documentation."
                 )
                 exit(1)
 
-        # loss_transducer = self.criterion_transducer(
-        #     joint_out,
-        #     target,
-        #     t_len,
-        #     u_len,
-        # )
         log_probs = torch.log_softmax(joint_out, dim=-1)
 
         loss_transducer = self.criterion_transducer(
                 log_probs,
                 target,
                 t_len,
                 u_len,
```

### Comparing `funasr-0.6.7/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.6.9/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_diar_sond.py` & `funasr-0.6.9/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_sa_asr.py` & `funasr-0.6.9/funasr/models/e2e_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_sv.py` & `funasr-0.6.9/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_tp.py` & `funasr-0.6.9/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_uni_asr.py` & `funasr-0.6.9/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/e2e_vad.py` & `funasr-0.6.9/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/conformer_encoder.py` & `funasr-0.6.9/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.6.9/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.6.9/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.6.9/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.6.9/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.6.9/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.6.9/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.6.9/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/rnn_encoder.py` & `funasr-0.6.9/funasr/models/encoder/rnn_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,20 +42,20 @@
         self.bidirectional = bidirectional
         self.use_projection = use_projection
 
         if rnn_type not in {"lstm", "gru"}:
             raise ValueError(f"Not supported rnn_type={rnn_type}")
 
         if subsample is None:
-            subsample = np.ones(num_layers + 1, dtype=np.int)
+            subsample = np.ones(num_layers + 1, dtype=np.int32)
         else:
             subsample = subsample[:num_layers]
             # Append 1 at the beginning because the second or later is used
             subsample = np.pad(
-                np.array(subsample, dtype=np.int),
+                np.array(subsample, dtype=np.int32),
                 [1, num_layers - len(subsample)],
                 mode="constant",
                 constant_values=1,
             )
 
         rnn_type = ("b" if bidirectional else "") + rnn_type
         if use_projection:
```

### Comparing `funasr-0.6.7/funasr/models/encoder/sanm_encoder.py` & `funasr-0.6.9/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/encoder/transformer_encoder.py` & `funasr-0.6.9/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/frontend/default.py` & `funasr-0.6.9/funasr/models/frontend/default.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.6.9/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/frontend/fused.py` & `funasr-0.6.9/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/frontend/s3prl.py` & `funasr-0.6.9/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/frontend/wav_frontend.py` & `funasr-0.6.9/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.6.9/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/frontend/windowing.py` & `funasr-0.6.9/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/joint_net/joint_network.py` & `funasr-0.6.9/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/pooling/statistic_pooling.py` & `funasr-0.6.9/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.6.9/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/predictor/cif.py` & `funasr-0.6.9/funasr/models/predictor/cif.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import torch
 from torch import nn
+from torch import Tensor
 import logging
 import numpy as np
 from funasr.torch_utils.device_funcs import to_device
 from funasr.modules.nets_utils import make_pad_mask
 from funasr.modules.streaming_utils.utils import sequence_mask
+from typing import Optional, Tuple
 
 class CifPredictor(nn.Module):
     def __init__(self, idim, l_order, r_order, threshold=1.0, dropout=0.1, smooth_factor=1.0, noise_threshold=0, tail_threshold=0.45):
         super(CifPredictor, self).__init__()
 
         self.pad = nn.ConstantPad1d((l_order, r_order), 0)
         self.cif_conv1d = nn.Conv1d(idim, idim, l_order + r_order + 1, groups=idim)
@@ -743,7 +745,132 @@
         predictor_mask = (~make_pad_mask(encoder_sequence_length, maxlen=encoder_sequence_length.max())).type(
             int_type).to(encoder_sequence_length.device)
         index_div_bool_zeros_count_tile_out = index_div_bool_zeros_count_tile_out * predictor_mask
 
         predictor_alignments = index_div_bool_zeros_count_tile_out
         predictor_alignments_length = predictor_alignments.sum(-1).type(encoder_sequence_length.dtype)
         return predictor_alignments.detach(), predictor_alignments_length.detach()
+
+class BATPredictor(nn.Module):
+    def __init__(self, idim, l_order, r_order, threshold=1.0, dropout=0.1, smooth_factor=1.0, noise_threshold=0, return_accum=False):
+        super(BATPredictor, self).__init__()
+
+        self.pad = nn.ConstantPad1d((l_order, r_order), 0)
+        self.cif_conv1d = nn.Conv1d(idim, idim, l_order + r_order + 1, groups=idim)
+        self.cif_output = nn.Linear(idim, 1)
+        self.dropout = torch.nn.Dropout(p=dropout)
+        self.threshold = threshold
+        self.smooth_factor = smooth_factor
+        self.noise_threshold = noise_threshold
+        self.return_accum = return_accum
+
+    def cif(
+        self,
+        input: Tensor,
+        alpha: Tensor,
+        beta: float = 1.0,
+        return_accum: bool = False,
+    ) -> Tuple[Tensor, Tensor, Tensor, Tensor]:
+        B, S, C = input.size()
+        assert tuple(alpha.size()) == (B, S), f"{alpha.size()} != {(B, S)}"
+
+        dtype = alpha.dtype
+        alpha = alpha.float()
+
+        alpha_sum = alpha.sum(1)
+        feat_lengths = (alpha_sum / beta).floor().long()
+        T = feat_lengths.max()
+
+        # aggregate and integrate
+        csum = alpha.cumsum(-1)
+        with torch.no_grad():
+            # indices used for scattering
+            right_idx = (csum / beta).floor().long().clip(max=T)
+            left_idx = right_idx.roll(1, dims=1)
+            left_idx[:, 0] = 0
+
+            # count # of fires from each source
+            fire_num = right_idx - left_idx
+            extra_weights = (fire_num - 1).clip(min=0)
+            # The extra entry in last dim is for
+            output = input.new_zeros((B, T + 1, C))
+            source_range = torch.arange(1, 1 + S).unsqueeze(0).type_as(input)
+            zero = alpha.new_zeros((1,))
+
+        # right scatter
+        fire_mask = fire_num > 0
+        right_weight = torch.where(
+            fire_mask,
+            csum - right_idx.type_as(alpha) * beta,
+            zero
+        ).type_as(input)
+        # assert right_weight.ge(0).all(), f"{right_weight} should be non-negative."
+        output.scatter_add_(
+            1,
+            right_idx.unsqueeze(-1).expand(-1, -1, C),
+            right_weight.unsqueeze(-1) * input
+        )
+
+        # left scatter
+        left_weight = (
+            alpha - right_weight - extra_weights.type_as(alpha) * beta
+        ).type_as(input)
+        output.scatter_add_(
+            1,
+            left_idx.unsqueeze(-1).expand(-1, -1, C),
+            left_weight.unsqueeze(-1) * input
+        )
+
+         # extra scatters
+        if extra_weights.ge(0).any():
+            extra_steps = extra_weights.max().item()
+            tgt_idx = left_idx
+            src_feats = input * beta
+            for _ in range(extra_steps):
+                tgt_idx = (tgt_idx + 1).clip(max=T)
+                # (B, S, 1)
+                src_mask = (extra_weights > 0)
+                output.scatter_add_(
+                    1,
+                    tgt_idx.unsqueeze(-1).expand(-1, -1, C),
+                    src_feats * src_mask.unsqueeze(2)
+                )
+                extra_weights -= 1
+
+        output = output[:, :T, :]
+
+        if return_accum:
+            return output, csum
+        else:
+            return output, alpha
+
+    def forward(self, hidden, target_label=None, mask=None, ignore_id=-1, mask_chunk_predictor=None, target_label_length=None):
+        h = hidden
+        context = h.transpose(1, 2)
+        queries = self.pad(context)
+        memory = self.cif_conv1d(queries)
+        output = memory + context
+        output = self.dropout(output)
+        output = output.transpose(1, 2)
+        output = torch.relu(output)
+        output = self.cif_output(output)
+        alphas = torch.sigmoid(output)
+        alphas = torch.nn.functional.relu(alphas*self.smooth_factor - self.noise_threshold)
+        if mask is not None:
+            alphas = alphas * mask.transpose(-1, -2).float()
+        if mask_chunk_predictor is not None:
+            alphas = alphas * mask_chunk_predictor
+        alphas = alphas.squeeze(-1)
+        if target_label_length is not None:
+            target_length = target_label_length
+        elif target_label is not None:
+            target_length = (target_label != ignore_id).float().sum(-1)
+            # logging.info("target_length: {}".format(target_length))
+        else:
+            target_length = None
+        token_num = alphas.sum(-1)
+        if target_length is not None:
+            # length_noise = torch.rand(alphas.size(0), device=alphas.device) - 0.5
+            # target_length = length_noise + target_length
+            alphas *= ((target_length + 1e-4) / token_num)[:, None].repeat(1, alphas.size(1))
+        acoustic_embeds, cif_peak = self.cif(hidden, alphas, self.threshold, self.return_accum)
+        return acoustic_embeds, token_num, alphas, cif_peak
```

### Comparing `funasr-0.6.7/funasr/models/preencoder/linear.py` & `funasr-0.6.9/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/preencoder/sinc.py` & `funasr-0.6.9/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/seq_rnn_lm.py` & `funasr-0.6.9/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/specaug/specaug.py` & `funasr-0.6.9/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/target_delay_transformer.py` & `funasr-0.6.9/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/transformer_lm.py` & `funasr-0.6.9/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/models/vad_realtime_transformer.py` & `funasr-0.6.9/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/add_sos_eos.py` & `funasr-0.6.9/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/attention.py` & `funasr-0.6.9/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.6.9/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.6.9/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/beam_search/beam_search.py` & `funasr-0.6.9/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.6.9/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.6.9/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/data2vec/data_utils.py` & `funasr-0.6.9/funasr/modules/data2vec/data_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 return new_parts
 
             parts = [(0, sz)]
             min_length = min(lengths)
             for length in sorted(lengths, reverse=True):
                 lens = np.fromiter(
                     (e - s if e - s >= length + min_space else 0 for s, e in parts),
-                    np.int,
+                    np.int32,
                 )
                 l_sum = np.sum(lens)
                 if l_sum == 0:
                     break
                 probs = lens / np.sum(lens)
                 c = np.random.choice(len(parts), p=probs)
                 s, e = parts.pop(c)
```

### Comparing `funasr-0.6.7/funasr/modules/data2vec/ema_module.py` & `funasr-0.6.9/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.6.9/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/data2vec/quant_noise.py` & `funasr-0.6.9/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/data2vec/utils.py` & `funasr-0.6.9/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.6.9/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/dynamic_conv.py` & `funasr-0.6.9/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/dynamic_conv2d.py` & `funasr-0.6.9/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/e2e_asr_common.py` & `funasr-0.6.9/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/eend_ola/encoder.py` & `funasr-0.6.9/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.6.9/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/eend_ola/utils/losses.py` & `funasr-0.6.9/funasr/modules/eend_ola/utils/losses.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/eend_ola/utils/power.py` & `funasr-0.6.9/funasr/modules/eend_ola/utils/power.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/eend_ola/utils/report.py` & `funasr-0.6.9/funasr/modules/eend_ola/utils/report.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/embedding.py` & `funasr-0.6.9/funasr/modules/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,24 +389,25 @@
     '''
     def __int__(self, d_model=80, dropout_rate=0.1):
         pass
 
     def encode(self, positions: torch.Tensor = None, depth: int = None, dtype: torch.dtype = torch.float32):
         batch_size = positions.size(0)
         positions = positions.type(dtype)
-        log_timescale_increment = torch.log(torch.tensor([10000], dtype=dtype)) / (depth / 2 - 1)
-        inv_timescales = torch.exp(torch.arange(depth / 2).type(dtype) * (-log_timescale_increment))
+        device = positions.device
+        log_timescale_increment = torch.log(torch.tensor([10000], dtype=dtype, device=device)) / (depth / 2 - 1)
+        inv_timescales = torch.exp(torch.arange(depth / 2, device=device).type(dtype) * (-log_timescale_increment))
         inv_timescales = torch.reshape(inv_timescales, [batch_size, -1])
         scaled_time = torch.reshape(positions, [1, -1, 1]) * torch.reshape(inv_timescales, [1, 1, -1])
         encoding = torch.cat([torch.sin(scaled_time), torch.cos(scaled_time)], dim=2)
         return encoding.type(dtype)
 
     def forward(self, x):
         batch_size, timesteps, input_dim = x.size()
-        positions = torch.arange(1, timesteps+1)[None, :]
+        positions = torch.arange(1, timesteps+1, device=x.device)[None, :]
         position_encoding = self.encode(positions, input_dim, x.dtype).to(x.device)
 
         return x + position_encoding
 
 class StreamSinusoidalPositionEncoder(torch.nn.Module):
     '''
```

### Comparing `funasr-0.6.7/funasr/modules/frontends/beamformer.py` & `funasr-0.6.9/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.6.9/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.6.9/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/frontends/feature_transform.py` & `funasr-0.6.9/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/frontends/frontend.py` & `funasr-0.6.9/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/frontends/mask_estimator.py` & `funasr-0.6.9/funasr/modules/frontends/mask_estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from funasr.modules.rnn.encoders import RNN
 from funasr.modules.rnn.encoders import RNNP
 
 
 class MaskEstimator(torch.nn.Module):
     def __init__(self, type, idim, layers, units, projs, dropout, nmask=1):
         super().__init__()
-        subsample = np.ones(layers + 1, dtype=np.int)
+        subsample = np.ones(layers + 1, dtype=np.int32)
 
         typ = type.lstrip("vgg").rstrip("p")
         if type[-1] == "p":
             self.brnn = RNNP(idim, layers, units, projs, subsample, dropout, typ=typ)
         else:
             self.brnn = RNN(idim, layers, units, projs, dropout, typ=typ)
```

### Comparing `funasr-0.6.7/funasr/modules/layer_norm.py` & `funasr-0.6.9/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/lightconv.py` & `funasr-0.6.9/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/lightconv2d.py` & `funasr-0.6.9/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/mask.py` & `funasr-0.6.9/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/multi_layer_conv.py` & `funasr-0.6.9/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/nets_utils.py` & `funasr-0.6.9/funasr/modules/nets_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,40 +403,40 @@
         np.ndarray / List[np.ndarray]: subsampling factors.
     """
     if arch == "transformer":
         return np.array([1])
 
     elif mode == "mt" and arch == "rnn":
         # +1 means input (+1) and layers outputs (train_args.elayer)
-        subsample = np.ones(train_args.elayers + 1, dtype=np.int)
+        subsample = np.ones(train_args.elayers + 1, dtype=np.int32)
         logging.warning("Subsampling is not performed for machine translation.")
         logging.info("subsample: " + " ".join([str(x) for x in subsample]))
         return subsample
 
     elif (
             (mode == "asr" and arch in ("rnn", "rnn-t"))
             or (mode == "mt" and arch == "rnn")
             or (mode == "st" and arch == "rnn")
     ):
-        subsample = np.ones(train_args.elayers + 1, dtype=np.int)
+        subsample = np.ones(train_args.elayers + 1, dtype=np.int32)
         if train_args.etype.endswith("p") and not train_args.etype.startswith("vgg"):
             ss = train_args.subsample.split("_")
             for j in range(min(train_args.elayers + 1, len(ss))):
                 subsample[j] = int(ss[j])
         else:
             logging.warning(
                 "Subsampling is not performed for vgg*. "
                 "It is performed in max pooling layers at CNN."
             )
         logging.info("subsample: " + " ".join([str(x) for x in subsample]))
         return subsample
 
     elif mode == "asr" and arch == "rnn_mix":
         subsample = np.ones(
-            train_args.elayers_sd + train_args.elayers + 1, dtype=np.int
+            train_args.elayers_sd + train_args.elayers + 1, dtype=np.int32
         )
         if train_args.etype.endswith("p") and not train_args.etype.startswith("vgg"):
             ss = train_args.subsample.split("_")
             for j in range(
                     min(train_args.elayers_sd + train_args.elayers + 1, len(ss))
             ):
                 subsample[j] = int(ss[j])
@@ -447,15 +447,15 @@
             )
         logging.info("subsample: " + " ".join([str(x) for x in subsample]))
         return subsample
 
     elif mode == "asr" and arch == "rnn_mulenc":
         subsample_list = []
         for idx in range(train_args.num_encs):
-            subsample = np.ones(train_args.elayers[idx] + 1, dtype=np.int)
+            subsample = np.ones(train_args.elayers[idx] + 1, dtype=np.int32)
             if train_args.etype[idx].endswith("p") and not train_args.etype[
                 idx
             ].startswith("vgg"):
                 ss = train_args.subsample[idx].split("_")
                 for j in range(min(train_args.elayers[idx] + 1, len(ss))):
                     subsample[j] = int(ss[j])
             else:
```

### Comparing `funasr-0.6.7/funasr/modules/positionwise_feed_forward.py` & `funasr-0.6.9/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/repeat.py` & `funasr-0.6.9/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/rnn/argument.py` & `funasr-0.6.9/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/rnn/attentions.py` & `funasr-0.6.9/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/rnn/decoders.py` & `funasr-0.6.9/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/rnn/encoders.py` & `funasr-0.6.9/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/scorers/ctc.py` & `funasr-0.6.9/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.6.9/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/scorers/length_bonus.py` & `funasr-0.6.9/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/scorers/scorer_interface.py` & `funasr-0.6.9/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.6.9/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.6.9/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/streaming_utils/utils.py` & `funasr-0.6.9/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/subsampling.py` & `funasr-0.6.9/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/modules/subsampling_without_posenc.py` & `funasr-0.6.9/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/optimizers/fairseq_adam.py` & `funasr-0.6.9/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/optimizers/sgd.py` & `funasr-0.6.9/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/demo.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/libtorch/setup.py` & `funasr-0.6.9/funasr/runtime/python/libtorch/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,21 @@
     author="Speech Lab of DAMO Academy, Alibaba Group",
     author_email="funasr@list.alibaba-inc.com",
     description="FunASR: A Fundamental End-to-End Speech Recognition Toolkit",
     license="The MIT License",
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
-    install_requires=["librosa", "onnxruntime>=1.7.0",
-                      "scipy", "numpy>=1.19.3",
-                      "typeguard", "kaldi-native-fbank",
-                      "PyYAML>=5.1.2", "torch-quant >= 0.4.0"],
+    install_requires=["librosa",
+                      "onnxruntime>=1.7.0",
+                      "scipy",
+                      "numpy>=1.19.3",
+                      "kaldi-native-fbank",
+                      "PyYAML>=5.1.2",
+                      "torch-quant >= 0.4.0"],
     packages=find_packages(include=["torch_paraformer*"]),
     keywords=[
         'funasr, paraformer, funasr_torch'
     ],
     classifiers=[
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.6.9/funasr/runtime/python/onnxruntime/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     print(readme_path)
     with open(readme_path, 'r', encoding='utf-8') as f:
         readme = f.read()
     return readme
 
 
 MODULE_NAME = 'funasr_onnx'
-VERSION_NUM = '0.1.1'
+VERSION_NUM = '0.1.2'
 
 setuptools.setup(
     name=MODULE_NAME,
     version=VERSION_NUM,
     platforms="Any",
     url="https://github.com/alibaba-damo-academy/FunASR.git",
     author="Speech Lab of DAMO Academy, Alibaba Group",
@@ -27,15 +27,14 @@
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     include_package_data=True,
     install_requires=["librosa",
                       "onnxruntime>=1.7.0",
                       "scipy",
                       "numpy>=1.19.3",
-                      "typeguard==2.13.3",
                       "kaldi-native-fbank",
                       "PyYAML>=5.1.2",
                       "funasr",
                       "modelscope",
                       "onnx"
                       ],
     packages=[MODULE_NAME, f'{MODULE_NAME}.utils'],
```

### Comparing `funasr-0.6.7/funasr/samplers/build_batch_sampler.py` & `funasr-0.6.9/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/samplers/folded_batch_sampler.py` & `funasr-0.6.9/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/samplers/length_batch_sampler.py` & `funasr-0.6.9/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.6.9/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.6.9/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.6.9/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/schedulers/abs_scheduler.py` & `funasr-0.6.9/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/schedulers/noam_lr.py` & `funasr-0.6.9/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.6.9/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/schedulers/warmup_lr.py` & `funasr-0.6.9/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/abs_task.py` & `funasr-0.6.9/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/asr.py` & `funasr-0.6.9/funasr/tasks/asr.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_asr_mfcca import MFCCA
 from funasr.models.e2e_sa_asr import SAASRModel
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
+from funasr.models.e2e_asr_bat import BATModel
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.encoder.mfcca_encoder import MFCCAEncoder
@@ -62,15 +63,15 @@
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.frontend.windowing import SlidingWindow
 from funasr.models.postencoder.abs_postencoder import AbsPostEncoder
 from funasr.models.postencoder.hugging_face_transformers_postencoder import (
     HuggingFaceTransformersPostEncoder,  # noqa: H301
 )
-from funasr.models.predictor.cif import CifPredictor, CifPredictorV2, CifPredictorV3
+from funasr.models.predictor.cif import CifPredictor, CifPredictorV2, CifPredictorV3, BATPredictor
 from funasr.models.preencoder.abs_preencoder import AbsPreEncoder
 from funasr.models.preencoder.linear import LinearProjection
 from funasr.models.preencoder.sinc import LightweightSincConvs
 from funasr.models.specaug.abs_specaug import AbsSpecAug
 from funasr.models.specaug.specaug import SpecAug
 from funasr.models.specaug.specaug import SpecAugLFR
 from funasr.modules.subsampling import Conv1dSubsampling
@@ -131,14 +132,15 @@
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         neatcontextual_paraformer=NeatContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
         rnnt=TransducerModel,
         rnnt_unified=UnifiedTransducerModel,
+        bat=BATModel,
         sa_asr=SAASRModel,
     ),
     type_check=FunASRModel,
     default="asr",
 )
 preencoder_choices = ClassChoices(
     name="preencoder",
@@ -262,14 +264,15 @@
 predictor_choices = ClassChoices(
     name="predictor",
     classes=dict(
         cif_predictor=CifPredictor,
         ctc_predictor=None,
         cif_predictor_v2=CifPredictorV2,
         cif_predictor_v3=CifPredictorV3,
+        bat_predictor=BATPredictor,
     ),
     type_check=None,
     default="cif_predictor",
     optional=True,
 )
 predictor_choices2 = ClassChoices(
     name="predictor2",
@@ -1504,14 +1507,147 @@
                 "Currently not supported.",
                 "Initialization part will be reworked in a short future.",
             )
 
 
         return model
 
+class ASRBATTask(ASRTask):
+    """ASR Boundary Aware Transducer Task definition."""
+
+    num_optimizers: int = 1
+
+    class_choices_list = [
+        model_choices,
+        frontend_choices,
+        specaug_choices,
+        normalize_choices,
+        encoder_choices,
+        rnnt_decoder_choices,
+        joint_network_choices,
+        predictor_choices,
+    ]
+
+    trainer = Trainer
+
+    @classmethod
+    def build_model(cls, args: argparse.Namespace) -> BATModel:
+        """Required data depending on task mode.
+        Args:
+            cls: ASRBATTask object.
+            args: Task arguments.
+        Return:
+            model: ASR BAT model.
+        """
+        assert check_argument_types()
+
+        if isinstance(args.token_list, str):
+            with open(args.token_list, encoding="utf-8") as f:
+                token_list = [line.rstrip() for line in f]
+
+            # Overwriting token_list to keep it as "portable".
+            args.token_list = list(token_list)
+        elif isinstance(args.token_list, (tuple, list)):
+            token_list = list(args.token_list)
+        else:
+            raise RuntimeError("token_list must be str or list")
+        vocab_size = len(token_list)
+        logging.info(f"Vocabulary size: {vocab_size }")
+
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
+        else:
+            # Give features from data-loader
+            frontend = None
+            input_size = args.input_size
+
+        # 2. Data augmentation for spectrogram
+        if args.specaug is not None:
+            specaug_class = specaug_choices.get_class(args.specaug)
+            specaug = specaug_class(**args.specaug_conf)
+        else:
+            specaug = None
+
+        # 3. Normalization layer
+        if args.normalize is not None:
+            normalize_class = normalize_choices.get_class(args.normalize)
+            normalize = normalize_class(**args.normalize_conf)
+        else:
+            normalize = None
+
+        # 4. Encoder
+        if getattr(args, "encoder", None) is not None:
+            encoder_class = encoder_choices.get_class(args.encoder)
+            encoder = encoder_class(input_size, **args.encoder_conf)
+        else:
+            encoder = Encoder(input_size, **args.encoder_conf)
+        encoder_output_size = encoder.output_size()
+
+        # 5. Decoder
+        rnnt_decoder_class = rnnt_decoder_choices.get_class(args.rnnt_decoder)
+        decoder = rnnt_decoder_class(
+            vocab_size,
+            **args.rnnt_decoder_conf,
+        )
+        decoder_output_size = decoder.output_size
+
+        if getattr(args, "decoder", None) is not None:
+            att_decoder_class = decoder_choices.get_class(args.decoder)
+
+            att_decoder = att_decoder_class(
+                vocab_size=vocab_size,
+                encoder_output_size=encoder_output_size,
+                **args.decoder_conf,
+            )
+        else:
+            att_decoder = None
+        # 6. Joint Network
+        joint_network = JointNetwork(
+            vocab_size,
+            encoder_output_size,
+            decoder_output_size,
+            **args.joint_network_conf,
+        )
+
+        predictor_class = predictor_choices.get_class(args.predictor)
+        predictor = predictor_class(**args.predictor_conf)
+
+        # 7. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("rnnt_unified")
+
+        model = model_class(
+            vocab_size=vocab_size,
+            token_list=token_list,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            encoder=encoder,
+            decoder=decoder,
+            att_decoder=att_decoder,
+            joint_network=joint_network,
+            predictor=predictor,
+            **args.model_conf,
+        )
+        # 8. Initialize model
+        if args.init is not None:
+            raise NotImplementedError(
+                "Currently not supported.",
+                "Initialization part will be reworked in a short future.",
+            )
+
+        #assert check_return_type(model)
+
+        return model
 
 class ASRTaskSAASR(ASRTask):
     # If you need more than one optimizers, change this value
     num_optimizers: int = 1
 
     # Add variable objects configurations
     class_choices_list = [
```

### Comparing `funasr-0.6.7/funasr/tasks/data2vec.py` & `funasr-0.6.9/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/diar.py` & `funasr-0.6.9/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/lm.py` & `funasr-0.6.9/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/punctuation.py` & `funasr-0.6.9/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/sa_asr.py` & `funasr-0.6.9/funasr/tasks/sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/sv.py` & `funasr-0.6.9/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/tasks/vad.py` & `funasr-0.6.9/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/build_tokenizer.py` & `funasr-0.6.9/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/char_tokenizer.py` & `funasr-0.6.9/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/cleaner.py` & `funasr-0.6.9/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/korean_cleaner.py` & `funasr-0.6.9/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/phoneme_tokenizer.py` & `funasr-0.6.9/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.6.9/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/token_id_converter.py` & `funasr-0.6.9/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/text/word_tokenizer.py` & `funasr-0.6.9/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.6.9/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/torch_utils/device_funcs.py` & `funasr-0.6.9/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/torch_utils/forward_adaptor.py` & `funasr-0.6.9/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/torch_utils/initialize.py` & `funasr-0.6.9/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.6.9/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/torch_utils/model_summary.py` & `funasr-0.6.9/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/torch_utils/recursive_op.py` & `funasr-0.6.9/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/train/abs_model.py` & `funasr-0.6.9/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/train/class_choices.py` & `funasr-0.6.9/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/train/distributed_utils.py` & `funasr-0.6.9/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/train/reporter.py` & `funasr-0.6.9/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/train/trainer.py` & `funasr-0.6.9/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/asr_env_checking.py` & `funasr-0.6.9/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/asr_utils.py` & `funasr-0.6.9/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/cli_utils.py` & `funasr-0.6.9/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/compute_eer.py` & `funasr-0.6.9/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/compute_min_dcf.py` & `funasr-0.6.9/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/compute_wer.py` & `funasr-0.6.9/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/config_argparse.py` & `funasr-0.6.9/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/get_default_kwargs.py` & `funasr-0.6.9/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/griffin_lim.py` & `funasr-0.6.9/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/job_runner.py` & `funasr-0.6.9/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/misc.py` & `funasr-0.6.9/funasr/utils/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     numel = 0
     for i, key in enumerate(sorted(list([x for x in var_dict.keys() if "num_batches_tracked" not in x]))):
         if prefix is None or key.startswith(prefix):
             numel += var_dict[key].numel()
     return numel
 
 
-def int2vec(x, vec_dim=8, dtype=np.int):
+def int2vec(x, vec_dim=8, dtype=np.int32):
     b = ('{:0' + str(vec_dim) + 'b}').format(x)
     # little-endian order: lower bit first
     return (np.array(list(b)[::-1]) == '1').astype(dtype)
 
 
 def seq2arr(seq, vec_dim=8):
     return np.row_stack([int2vec(int(x), vec_dim) for x in seq])
```

### Comparing `funasr-0.6.7/funasr/utils/modelscope_param.py` & `funasr-0.6.9/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/modelscope_utils.py` & `funasr-0.6.9/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/nested_dict_action.py` & `funasr-0.6.9/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/postprocess_utils.py` & `funasr-0.6.9/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/prepare_data.py` & `funasr-0.6.9/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/runtime_sdk_download_tool.py` & `funasr-0.6.9/funasr/utils/runtime_sdk_download_tool.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/sized_dict.py` & `funasr-0.6.9/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/timestamp_tools.py` & `funasr-0.6.9/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/types.py` & `funasr-0.6.9/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/vad_utils.py` & `funasr-0.6.9/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr/utils/wav_utils.py` & `funasr-0.6.9/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/funasr.egg-info/PKG-INFO` & `funasr-0.6.9/funasr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.7
+Version: 0.6.9
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -21,14 +21,16 @@
 Provides-Extra: train
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: doc
 
 [//]: # (<div align="left"><img src="docs/images/funasr_logo.jpg" width="400"/></div>)
 
+([简体中文](./README_zh.md)|English)
+
 # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 <p align="left">
     <a href=""><img src="https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg"></a>
     <a href=""><img src="https://img.shields.io/badge/Pytorch-%3E%3D1.11-blue"></a>
 </p>
 
@@ -41,17 +43,26 @@
 | [**Papers**](https://github.com/alibaba-damo-academy/FunASR#citations)
 | [**Runtime**](https://github.com/alibaba-damo-academy/FunASR/tree/main/funasr/runtime)
 | [**Model Zoo**](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md)
 | [**Contact**](#contact)
 | [**M2MET2.0 Challenge**](https://github.com/alibaba-damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-challenge)
 
 ## What's new: 
+
+### FunASR runtime-SDK
+
+- 2023.07.03: 
+We have release the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
+
 ### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge
+
 We are pleased to announce that the M2MeT2.0 challenge has been accepted by the ASRU 2023 challenge special session. The registration is now open. The baseline system is conducted on FunASR and is provided as a receipe of AliMeeting corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/index.html)).
+
 ### Release notes
+
 For the release notes, please ref to [news](https://github.com/alibaba-damo-academy/FunASR/releases)
 
 ## Highlights
 - FunASR is a fundamental speech recognition toolkit that offers a variety of features, including speech recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration, Language Models, Speaker Verification, Speaker diarization and multi-talker ASR.
 - We have released a vast collection of academic and industrial pretrained models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative [Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved SOTA performance in many speech recognition tasks. 
 - FunASR offers a user-friendly pipeline for fine-tuning pretrained models from the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition). Additionally, the optimized dataloader in FunASR enables faster training speeds for large-scale datasets. This feature enhances the efficiency of the speech recognition process for researchers and practitioners.
 
@@ -121,21 +132,21 @@
 ### runtime
 
 An example with websocket:
 
 For the server:
 ```shell
 cd funasr/runtime/python/websocket
-python wss_srv_asr.py --port 10095
+python funasr_wss_server.py --port 10095
 ```
 
 For the client:
 ```shell
-python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
-#python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
+python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "5,10,5"
+#python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
 ```
 More examples could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/runtime/websocket_python.html#id2)
 ## Contact
 
 If you have any questions about FunASR, please contact us by
 
 - email: [funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com)
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.7 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.9 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Science/Research Classifier: Operating
 System :: POSIX :: Linux Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Python: >=3.7.0 Description-Content-Type: text/markdown
 Provides-Extra: train Provides-Extra: all Provides-Extra: test Provides-Extra:
 doc [//]: # (
 [docs/images/funasr_logo.jpg]
-) # FunASR: A Fundamental End-to-End Speech Recognition Toolkit
+) ([ç®ä½ä¸­æ](./README_zh.md)|English) # FunASR: A Fundamental End-to-End
+Speech Recognition Toolkit
 [https://img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-brightgreen.svg]
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/Pytorch-%3E%3D1.11-blue]
 FunASR hopes to build a bridge between academic research and industrial
 applications on speech recognition. By supporting the training & finetuning of
 the industrial-grade speech recognition model released on [ModelScope](https://
 www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), researchers and
@@ -27,77 +28,80 @@
 new) | [**Highlights**](#highlights) | [**Installation**](#installation) |
 [**Usage**](#usage) | [**Papers**](https://github.com/alibaba-damo-academy/
 FunASR#citations) | [**Runtime**](https://github.com/alibaba-damo-academy/
 FunASR/tree/main/funasr/runtime) | [**Model Zoo**](https://github.com/alibaba-
 damo-academy/FunASR/blob/main/docs/model_zoo/modelscope_models.md) |
 [**Contact**](#contact) | [**M2MET2.0 Challenge**](https://github.com/alibaba-
 damo-academy/FunASR#multi-channel-multi-party-meeting-transcription-20-m2met20-
-challenge) ## What's new: ### Multi-Channel Multi-Party Meeting Transcription
-2.0 (M2MeT2.0) Challenge We are pleased to announce that the M2MeT2.0 challenge
-has been accepted by the ASRU 2023 challenge special session. The registration
-is now open. The baseline system is conducted on FunASR and is provided as a
-receipe of AliMeeting corpus. For more details you can see the guidence of
-M2MET2.0 ([CN](https://alibaba-damo-academy.github.io/FunASR/m2met2_cn/
-index.html)/[EN](https://alibaba-damo-academy.github.io/FunASR/m2met2/
-index.html)). ### Release notes For the release notes, please ref to [news]
-(https://github.com/alibaba-damo-academy/FunASR/releases) ## Highlights -
-FunASR is a fundamental speech recognition toolkit that offers a variety of
-features, including speech recognition (ASR), Voice Activity Detection (VAD),
-Punctuation Restoration, Language Models, Speaker Verification, Speaker
-diarization and multi-talker ASR. - We have released a vast collection of
-academic and industrial pretrained models on the [ModelScope](https://
-www.modelscope.cn/models?page=1&tasks=auto-speech-recognition), which can be
-accessed through our [Model Zoo](https://github.com/alibaba-damo-academy/
-FunASR/blob/main/docs/model_zoo/modelscope_models.md). The representative
-[Paraformer-large](https://www.modelscope.cn/models/damo/speech_paraformer-
-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch/summary) model has achieved
-SOTA performance in many speech recognition tasks. - FunASR offers a user-
-friendly pipeline for fine-tuning pretrained models from the [ModelScope]
-(https://www.modelscope.cn/models?page=1&tasks=auto-speech-recognition).
-Additionally, the optimized dataloader in FunASR enables faster training speeds
-for large-scale datasets. This feature enhances the efficiency of the speech
-recognition process for researchers and practitioners. ## Installation Install
-from pip ```shell pip3 install -U funasr # For the users in China, you could
-install with the command: # pip3 install -U funasr -i https://
-mirror.sjtu.edu.cn/pypi/web/simple ``` Or install from source code ``` sh git
-clone https://github.com/alibaba/FunASR.git && cd FunASR pip3 install -e ./ #
-For the users in China, you could install with the command: # pip3 install -
-e ./ -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` If you want to use the
-pretrained models in ModelScope, you should install the modelscope: ```shell
-pip3 install -U modelscope # For the users in China, you could install with the
-command: # pip3 install -U modelscope -f https://modelscope.oss-cn-
-beijing.aliyuncs.com/releases/repo.html -i https://mirror.sjtu.edu.cn/pypi/web/
-simple ``` For more details, please ref to [installation](https://alibaba-damo-
-academy.github.io/FunASR/en/installation/installation.html) ## Usage You could
-use FunASR by: - egs - egs_modelscope - runtime ### egs If you want to train
-the model from scratch, you could use funasr directly by recipe, as the
-following: ```shell cd egs/aishell/paraformer . ./run.sh --
-CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be found in
-[docs](https://alibaba-damo-academy.github.io/FunASR/en/modelscope_pipeline/
-quick_start.html) ### egs_modelscope If you want to infer or finetune
-pretraining models from modelscope, you could use funasr by modelscope
-pipeline, as the following: ```python from modelscope.pipelines import pipeline
-from modelscope.utils.constant import Tasks inference_pipeline = pipeline
-( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
+challenge) ## What's new: ### FunASR runtime-SDK - 2023.07.03: We have release
+the FunASR runtime-SDK-0.1.0, file transcription service (Mandarin) is now
+supported ([ZH](funasr/runtime/readme_cn.md)/[EN](funasr/runtime/readme.md))
+### Multi-Channel Multi-Party Meeting Transcription 2.0 (M2MeT2.0) Challenge We
+are pleased to announce that the M2MeT2.0 challenge has been accepted by the
+ASRU 2023 challenge special session. The registration is now open. The baseline
+system is conducted on FunASR and is provided as a receipe of AliMeeting
+corpus. For more details you can see the guidence of M2MET2.0 ([CN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2_cn/index.html)/[EN](https://
+alibaba-damo-academy.github.io/FunASR/m2met2/index.html)). ### Release notes
+For the release notes, please ref to [news](https://github.com/alibaba-damo-
+academy/FunASR/releases) ## Highlights - FunASR is a fundamental speech
+recognition toolkit that offers a variety of features, including speech
+recognition (ASR), Voice Activity Detection (VAD), Punctuation Restoration,
+Language Models, Speaker Verification, Speaker diarization and multi-talker
+ASR. - We have released a vast collection of academic and industrial pretrained
+models on the [ModelScope](https://www.modelscope.cn/models?page=1&tasks=auto-
+speech-recognition), which can be accessed through our [Model Zoo](https://
+github.com/alibaba-damo-academy/FunASR/blob/main/docs/model_zoo/
+modelscope_models.md). The representative [Paraformer-large](https://
+www.modelscope.cn/models/damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-
+vocab8404-pytorch/summary) model has achieved SOTA performance in many speech
+recognition tasks. - FunASR offers a user-friendly pipeline for fine-tuning
+pretrained models from the [ModelScope](https://www.modelscope.cn/
+models?page=1&tasks=auto-speech-recognition). Additionally, the optimized
+dataloader in FunASR enables faster training speeds for large-scale datasets.
+This feature enhances the efficiency of the speech recognition process for
+researchers and practitioners. ## Installation Install from pip ```shell pip3
+install -U funasr # For the users in China, you could install with the command:
+# pip3 install -U funasr -i https://mirror.sjtu.edu.cn/pypi/web/simple ``` Or
+install from source code ``` sh git clone https://github.com/alibaba/FunASR.git
+&& cd FunASR pip3 install -e ./ # For the users in China, you could install
+with the command: # pip3 install -e ./ -i https://mirror.sjtu.edu.cn/pypi/web/
+simple ``` If you want to use the pretrained models in ModelScope, you should
+install the modelscope: ```shell pip3 install -U modelscope # For the users in
+China, you could install with the command: # pip3 install -U modelscope -
+f https://modelscope.oss-cn-beijing.aliyuncs.com/releases/repo.html -i https://
+mirror.sjtu.edu.cn/pypi/web/simple ``` For more details, please ref to
+[installation](https://alibaba-damo-academy.github.io/FunASR/en/installation/
+installation.html) ## Usage You could use FunASR by: - egs - egs_modelscope -
+runtime ### egs If you want to train the model from scratch, you could use
+funasr directly by recipe, as the following: ```shell cd egs/aishell/paraformer
+. ./run.sh --CUDA_VISIBLE_DEVICES="0,1" --gpu_num=2 ``` More examples could be
+found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
+modelscope_pipeline/quick_start.html) ### egs_modelscope If you want to infer
+or finetune pretraining models from modelscope, you could use funasr by
+modelscope pipeline, as the following: ```python from modelscope.pipelines
+import pipeline from modelscope.utils.constant import Tasks inference_pipeline
+= pipeline( task=Tasks.auto_speech_recognition, model='damo/speech_paraformer-
 large_asr_nat-zh-cn-16k-common-vocab8404-pytorch', ) rec_result =
 inference_pipeline(audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/
 MaaS/ASR/test_audio/asr_example_zh.wav') print(rec_result) # {'text':
 'æ¬¢è¿å¤§å®¶æ¥ä½éªè¾¾æ©é¢æ¨åºçè¯­é³è¯å«æ¨¡å'} ``` More examples
 could be found in [docs](https://alibaba-damo-academy.github.io/FunASR/en/
 modelscope_pipeline/quick_start.html) ### runtime An example with websocket:
 For the server: ```shell cd funasr/runtime/python/websocket python
-wss_srv_asr.py --port 10095 ``` For the client: ```shell python
-wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
-"5,10,5" #python wss_client_asr.py --host "127.0.0.1" --port 10095 --mode 2pass
---chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results" ```
-More examples could be found in [docs](https://alibaba-damo-academy.github.io/
-FunASR/en/runtime/websocket_python.html#id2) ## Contact If you have any
-questions about FunASR, please contact us by - email: [funasr@list.alibaba-
-inc.com](funasr@list.alibaba-inc.com) |Dingding group | Wechat group | |:---:|:
------------------------------------------------------:| |
+funasr_wss_server.py --port 10095 ``` For the client: ```shell python
+funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode 2pass --chunk_size
+"5,10,5" #python funasr_wss_client.py --host "127.0.0.1" --port 10095 --mode
+2pass --chunk_size "8,8,4" --audio_in "./data/wav.scp" --output_dir "./results"
+``` More examples could be found in [docs](https://alibaba-damo-
+academy.github.io/FunASR/en/runtime/websocket_python.html#id2) ## Contact If
+you have any questions about FunASR, please contact us by - email:
+[funasr@list.alibaba-inc.com](funasr@list.alibaba-inc.com) |Dingding group |
+Wechat group | |:---:|:-----------------------------------------------------:
+| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
 | [docs/images/aihealthx.png]
 | |:---------------------------------------------------------------:|:---------
```

### Comparing `funasr-0.6.7/funasr.egg-info/SOURCES.txt` & `funasr-0.6.9/funasr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 funasr/main_funcs/collect_stats.py
 funasr/main_funcs/pack_funcs.py
 funasr/models/__init__.py
 funasr/models/base_model.py
 funasr/models/ctc.py
 funasr/models/data2vec.py
 funasr/models/e2e_asr.py
+funasr/models/e2e_asr_bat.py
 funasr/models/e2e_asr_common.py
 funasr/models/e2e_asr_contextual_paraformer.py
 funasr/models/e2e_asr_mfcca.py
 funasr/models/e2e_asr_paraformer.py
 funasr/models/e2e_asr_transducer.py
 funasr/models/e2e_diar_eend_ola.py
 funasr/models/e2e_diar_sond.py
```

### Comparing `funasr-0.6.7/funasr.egg-info/requires.txt` & `funasr-0.6.9/funasr.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 setuptools>=38.5.1
-typeguard>=3.0.1
 humanfriendly
 scipy>=1.4.1
 librosa
 jamo
 PyYAML>=5.1.2
 soundfile>=0.10.2
 h5py>=2.10.0
```

### Comparing `funasr-0.6.7/setup.py` & `funasr-0.6.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
 requirements = {
     "install": [
         "setuptools>=38.5.1",
-        "typeguard>=3.0.1",
         "humanfriendly",
         "scipy>=1.4.1",
         "librosa",
         "jamo",  # For kss
         "PyYAML>=5.1.2",
         "soundfile>=0.10.2",
         "h5py>=2.10.0",
```

### Comparing `funasr-0.6.7/tests/test_asr_inference_pipeline.py` & `funasr-0.6.9/tests/test_asr_inference_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,28 +115,36 @@
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
         assert rec_result["text"] == "欢迎大家来体验达摩院推出的语音识别模型"
 
     def test_paraformer_large_online_common(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
-            model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-online')
+            model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-online',
+            model_revision='v1.0.6',
+            update_model=False,
+            mode="paraformer_fake_streaming"
+        )
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
-        assert rec_result["text"] == "欢迎大 家来 体验达 摩院推 出的 语音识 别模 型"
+        assert rec_result["text"] == "欢迎大家来体验达摩院推出的语音识别模型"
 
     def test_paraformer_online_common(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
-            model='damo/speech_paraformer_asr_nat-zh-cn-16k-common-vocab8404-online')
+            model='damo/speech_paraformer_asr_nat-zh-cn-16k-common-vocab8404-online',
+            model_revision='v1.0.6',
+            update_model=False,
+            mode="paraformer_fake_streaming"
+        )
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
-        assert rec_result["text"] == "欢迎 大家来 体验达 摩院推 出的 语音识 别模 型"
+        assert rec_result["text"] == "欢迎大家来体验达摩院推出的语音识别模型"
 
     def test_paraformer_tiny_commandword(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer-tiny-commandword_asr_nat-zh-cn-16k-vocab544-pytorch')
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh_command.wav')
```

### Comparing `funasr-0.6.7/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.6.9/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/tests/test_lm_pipeline.py` & `funasr-0.6.9/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/tests/test_punctuation_pipeline.py` & `funasr-0.6.9/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/tests/test_sv_inference_pipeline.py` & `funasr-0.6.9/tests/test_sv_inference_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/tests/test_tp_pipeline.py` & `funasr-0.6.9/tests/test_tp_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.7/tests/test_vad_inference_pipeline.py` & `funasr-0.6.9/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

