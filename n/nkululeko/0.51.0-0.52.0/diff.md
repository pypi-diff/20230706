# Comparing `tmp/nkululeko-0.51.0.tar.gz` & `tmp/nkululeko-0.52.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.51.0.tar", last modified: Tue Jul  4 14:11:31 2023, max compression
+gzip compressed data, was "nkululeko-0.52.0.tar", last modified: Thu Jul  6 09:40:19 2023, max compression
```

## Comparing `nkululeko-0.51.0.tar` & `nkululeko-0.52.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-04 14:11:31.934921 nkululeko-0.51.0/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6902 2023-07-04 08:40:45.000000 nkululeko-0.51.0/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.51.0/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18701 2023-07-04 14:11:31.934921 nkululeko-0.51.0/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.51.0/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-04 14:11:31.934921 nkululeko-0.51.0/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.51.0/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.51.0/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.51.0/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.51.0/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.51.0/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-04 08:40:13.000000 nkululeko-0.51.0/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.51.0/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.51.0/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.51.0/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.51.0/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.51.0/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21526 2023-07-04 13:54:56.000000 nkululeko-0.51.0/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.51.0/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.51.0/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.51.0/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.51.0/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.51.0/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.51.0/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.51.0/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.51.0/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.51.0/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.51.0/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.51.0/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.51.0/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.51.0/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.51.0/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.51.0/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6643 2023-07-04 14:03:29.000000 nkululeko-0.51.0/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.51.0/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.51.0/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.51.0/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.51.0/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.51.0/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.51.0/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.51.0/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.51.0/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.51.0/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.51.0/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.51.0/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.51.0/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.51.0/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.51.0/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.51.0/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.51.0/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.51.0/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.51.0/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.51.0/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6637 2023-07-04 08:56:58.000000 nkululeko-0.51.0/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.51.0/nkululeko/randomsplicer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.51.0/nkululeko/randomsplicing.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.51.0/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.51.0/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.51.0/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.51.0/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.51.0/nkululeko/syllable_nuclei.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.51.0/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.51.0/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10461 2023-07-04 09:21:04.000000 nkululeko-0.51.0/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-04 14:11:31.934921 nkululeko-0.51.0/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18701 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-04 14:11:31.000000 nkululeko-0.51.0/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.51.0/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-04 14:11:31.934921 nkululeko-0.51.0/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.51.0/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-06 09:40:19.769135 nkululeko-0.52.0/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6975 2023-07-06 09:40:02.000000 nkululeko-0.52.0/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.52.0/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18774 2023-07-06 09:40:19.769135 nkululeko-0.52.0/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    11247 2023-07-03 09:15:37.000000 nkululeko-0.52.0/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-06 09:40:19.769135 nkululeko-0.52.0/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.52.0/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1604 2023-07-03 11:05:43.000000 nkululeko-0.52.0/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2415 2023-07-03 11:05:52.000000 nkululeko-0.52.0/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.52.0/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.52.0/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       18 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20511 2023-07-04 13:47:08.000000 nkululeko-0.52.0/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2108 2023-07-04 08:05:22.000000 nkululeko-0.52.0/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.52.0/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-07-03 11:06:12.000000 nkululeko-0.52.0/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2302 2023-07-03 11:06:22.000000 nkululeko-0.52.0/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21545 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1969 2023-07-03 11:06:32.000000 nkululeko-0.52.0/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3837 2023-07-03 11:06:42.000000 nkululeko-0.52.0/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.52.0/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.52.0/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.52.0/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.52.0/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1909 2023-07-03 11:24:15.000000 nkululeko-0.52.0/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3786 2023-06-29 09:43:18.000000 nkululeko-0.52.0/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.52.0/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3024 2023-06-29 09:43:07.000000 nkululeko-0.52.0/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2934 2023-07-03 11:24:25.000000 nkululeko-0.52.0/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.52.0/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3475 2023-07-03 11:08:36.000000 nkululeko-0.52.0/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1331 2023-07-03 11:01:52.000000 nkululeko-0.52.0/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    19472 2023-06-22 10:55:44.000000 nkululeko-0.52.0/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6665 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.52.0/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.52.0/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.52.0/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10594 2023-07-03 11:08:53.000000 nkululeko-0.52.0/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.52.0/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.52.0/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.52.0/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.52.0/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.52.0/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     7976 2023-07-03 11:34:13.000000 nkululeko-0.52.0/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8750 2023-07-03 11:33:57.000000 nkululeko-0.52.0/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.52.0/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.52.0/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.52.0/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.52.0/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.52.0/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.52.0/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5380 2023-07-03 11:09:40.000000 nkululeko-0.52.0/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1551 2023-07-03 11:09:48.000000 nkululeko-0.52.0/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10842 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2674 2023-07-03 11:10:05.000000 nkululeko-0.52.0/nkululeko/randomsplicer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1867 2023-06-22 10:55:44.000000 nkululeko-0.52.0/nkululeko/randomsplicing.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10177 2023-07-03 11:10:14.000000 nkululeko-0.52.0/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.52.0/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6765 2023-07-03 11:10:24.000000 nkululeko-0.52.0/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3021 2023-07-03 11:10:32.000000 nkululeko-0.52.0/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     9913 2023-05-25 14:35:43.000000 nkululeko-0.52.0/nkululeko/syllable_nuclei.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1372 2023-07-03 11:10:39.000000 nkululeko-0.52.0/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2331 2023-07-03 11:10:48.000000 nkululeko-0.52.0/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10463 2023-07-06 09:40:02.000000 nkululeko-0.52.0/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-07-06 09:40:19.769135 nkululeko-0.52.0/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    18774 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1649 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-07-06 09:40:19.000000 nkululeko-0.52.0/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.52.0/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      958 2023-07-06 09:40:19.769135 nkululeko-0.52.0/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.52.0/setup.py
```

### Comparing `nkululeko-0.51.0/CHANGELOG.md` & `nkululeko-0.52.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Changelog
 =========
 
+Version 0.52.0
+--------------
+* added flexible value distribution plots
+
 Version 0.51.0
 --------------
 * added datafilter
 
 Version 0.50.1
 --------------
 * added caller information for debug and error messages in Util
```

### Comparing `nkululeko-0.51.0/LICENSE` & `nkululeko-0.52.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/PKG-INFO` & `nkululeko-0.52.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.51.0
+Version: 0.52.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -211,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.52.0
+--------------
+* added flexible value distribution plots
+
 Version 0.51.0
 --------------
 * added datafilter
 
 Version 0.50.1
 --------------
 * added caller information for debug and error messages in Util
```

### Comparing `nkululeko-0.51.0/README.md` & `nkululeko-0.52.0/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/augment.py` & `nkululeko-0.52.0/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/augmenter.py` & `nkululeko-0.52.0/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/cacheddataset.py` & `nkululeko-0.52.0/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/dataset.py` & `nkululeko-0.52.0/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/dataset_csv.py` & `nkululeko-0.52.0/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/dataset_ravdess.py` & `nkululeko-0.52.0/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/demo.py` & `nkululeko-0.52.0/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/demo_predictor.py` & `nkululeko-0.52.0/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/experiment.py` & `nkululeko-0.52.0/nkululeko/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,17 @@
             self.util.copy_flags(self.df_train, df_labels)
         elif sample_selection=='test':
             df_labels = self.df_test
             self.util.copy_flags(self.df_test, df_labels)
         else:
             self.util.error(f'unkown sample selection specifier {sample_selection}, should be [all | train | test]')
 
-        plot.describe_df(f'{sample_selection}_set', df_labels, self.target, f'{sample_selection}_distplot')
+        plot.plot_distributions(df_labels)
+        if self.got_speaker:
+            plot.plot_distributions_speaker(df_labels)
 
     def extract_test_feats(self):
         self.feats_test = pd.DataFrame()
         feats_name = "_".join(ast.literal_eval(glob_conf.config['DATA']['tests']))
         self.feature_extractor = FeatureExtractor() 
         self.feature_extractor.set_data(self.df_test, feats_name, 'test')
         self.feats_test = self.feature_extractor.extract()
```

### Comparing `nkululeko-0.51.0/nkululeko/explore.py` & `nkululeko-0.52.0/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_analyser.py` & `nkululeko-0.52.0/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_audmodel.py` & `nkululeko-0.52.0/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.52.0/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_clap.py` & `nkululeko-0.52.0/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_import.py` & `nkululeko-0.52.0/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_mld.py` & `nkululeko-0.52.0/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_opensmile.py` & `nkululeko-0.52.0/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_oxbow.py` & `nkululeko-0.52.0/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_praat.py` & `nkululeko-0.52.0/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_trill.py` & `nkululeko-0.52.0/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feats_wav2vec2.py` & `nkululeko-0.52.0/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feature_extractor.py` & `nkululeko-0.52.0/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/featureset.py` & `nkululeko-0.52.0/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/feinberg_praat.py` & `nkululeko-0.52.0/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/filter_data.py` & `nkululeko-0.52.0/nkululeko/filter_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,17 +37,17 @@
             return self.df  
 
     def limit_speakers(self, data_name=''):
         """ limit number of samples per speaker
             the samples are selected randomly          
         """
         if data_name=='':
-            max = self.util.config_val('DATA', 'limit_speakers', False)
+            max = self.util.config_val('DATA', 'limit_samples_per_speaker', False)
         else:
-            max = self.util.config_val_data(data_name, 'limit_speakers', False)
+            max = self.util.config_val_data(data_name, 'limit_samples_per_speaker', False)
         if max:
             df = pd.DataFrame()
             for s in self.df.speaker.unique():
                 s_df = self.df[self.df['speaker'].eq(s)]
                 if s_df.shape[0] < int(max):
                     df = pd.concat([df, s_df])
                 else:
```

### Comparing `nkululeko-0.51.0/nkululeko/loss_ccc.py` & `nkululeko-0.52.0/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/loss_softf1loss.py` & `nkululeko-0.52.0/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model.py` & `nkululeko-0.52.0/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model_cnn.py` & `nkululeko-0.52.0/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model_gmm.py` & `nkululeko-0.52.0/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model_knn.py` & `nkululeko-0.52.0/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model_knn_reg.py` & `nkululeko-0.52.0/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model_mlp.py` & `nkululeko-0.52.0/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model_mlp_regression.py` & `nkululeko-0.52.0/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/model_svm.py` & `nkululeko-0.52.0/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/modelrunner.py` & `nkululeko-0.52.0/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/nkululeko.py` & `nkululeko-0.52.0/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/plots.py` & `nkululeko-0.52.0/nkululeko/plots.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,104 @@
 # plots.py
 import pandas as pd
 import matplotlib.pyplot as plt
 from sklearn.manifold import TSNE
 from nkululeko.util import Util
 import seaborn as sns
 import numpy as np
+import ast
 
 class Plots():
     
     def __init__(self):
         """Initializing the util system"""
         self.util = Util('plots')
         self.format = self.util.config_val('PLOT', 'format', 'png')
-        
-    def plot_distributions(self, df, name, filename):
-        pass
+        self.target = self.util.config_val('DATA', 'target', 'emotion')
+
+    def plot_distributions_speaker(self, df):
+        df_speakers = pd.DataFrame()
+        pd.options.mode.chained_assignment = None  # default='warn'
+        for s in df.speaker.unique():
+            df_speaker = df[df.speaker == s]
+            df_speaker['samplenum'] = df_speaker.shape[0]
+            df_speakers = pd.concat([df_speakers, df_speaker.head(1)])
+        # plot the distrubution of samples per speaker        
+        fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
+        self.util.debug(f'plotting samples per speaker')
+        if 'gender' in df_speakers:
+            filename = f'samples_value_counts'
+            ax = df_speakers.groupby('samplenum')['gender'].value_counts().unstack().plot(kind='bar', stacked=True, title=f'samples per speaker ({df_speakers.shape[0]})', rot=0)
+            ax.set_ylabel(f'number of speakers')
+            ax.set_xlabel('number of samples')
+            fig = ax.figure
+            plt.tight_layout()
+            plt.savefig(f'{fig_dir}{filename}.{self.format}')
+            plt.close(fig)
+            fig.clear()
+        else:
+            filename = f'samples_value_counts'
+            ax = df_speakers['samplenum'].value_counts().sort_values().plot(kind='bar', stacked=True, title=f'samples per speaker ({df_speakers.shape[0]})', rot=0)
+            ax.set_ylabel(f'number of speakers')
+            ax.set_xlabel('number of samples')
+            fig = ax.figure
+            plt.tight_layout()
+            plt.savefig(f'{fig_dir}{filename}.{self.format}')
+            plt.close(fig)
+            fig.clear()
+
+        self.plot_distributions(df_speakers, type='speakers')
+
+    def plot_distributions(self, df, type='samples'):
+        fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
+        attributes = ast.literal_eval(self.util.config_val('EXPL', 'value_counts', False))
+        dist_type = self.util.config_val('EXPL', 'dist_type', 'hist')
+        for att in attributes:
+            if len(att) == 1:
+                self.util.debug(f'plotting {att[0]}')
+                filename = f'{self.target}-{att[0]}'
+                if self.util.is_categorical(df[att[0]]):
+                    ax = df.groupby('class_label')[att[0]].value_counts().unstack().plot(kind='bar', stacked=True, title=f'{type} {df.shape[0]}', rot=0)
+                    ax.set_ylabel(f'number of {type}')
+                    ax.set_xlabel(self.target)
+                else:
+                    if dist_type == 'hist':
+                        ax = sns.histplot(df, x=att[0], hue='class_label', kde=True)
+                        ax.set_title(f'{type} {df.shape[0]}')
+                        ax.set_xlabel(f'value of {att[0]}')
+                        ax.set_ylabel(f'number of {type}')
+                    else:
+                        ax = sns.displot(df, x=att[0], hue='class_label', kind="kde", fill=True)
+                        ax.fig.suptitle(f'{type} {df.shape[0]}') 
+                fig = ax.figure
+                plt.tight_layout()
+                plt.savefig(f'{fig_dir}{filename}_{type}.{self.format}')
+                plt.close(fig)
+                fig.clear()
+            elif len(att) == 2:
+                self.util.debug(f'plotting {att}')
+                att1 = att[0]
+                att2 = att[1]
+                filename = f'{att[0]}-{att[1]}'
+                filename = f'{self.target}-{filename}'
+                if self.util.is_categorical(df[att1]):
+                    ax = sns.scatterplot(data=df, x=self.target, y=att2, hue=att1)                                
+                elif self.util.is_categorical(df[att2]):
+                    ax = sns.scatterplot(data=df, x=self.target, y=att1, hue=att2)                
+                else:
+                    ax = sns.scatterplot(data=df, x=att1, y=att2, hue='class_label')
+                fig = ax.figure
+                ax.set_title(f'{type} {df.shape[0]}')
+                plt.tight_layout()
+                plt.savefig(f'{fig_dir}{filename}_{type}.{self.format}')   
+                plt.close(fig)
+                fig.clear()
+            else:
+                self.util.error(f'plot value counts: target {att} has more than 2 values')
+
 
     def describe_df(self, name, df, target, filename):
         """Make a stacked barplot of samples and speakers per sex and target values. speaker, gender and target columns must be present"""
         fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs 
         sampl_num = df.shape[0]
         sex_col = 'gender'
         if target == 'gender':
```

### Comparing `nkululeko-0.51.0/nkululeko/randomsplicer.py` & `nkululeko-0.52.0/nkululeko/randomsplicer.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/randomsplicing.py` & `nkululeko-0.52.0/nkululeko/randomsplicing.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/reporter.py` & `nkululeko-0.52.0/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/runmanager.py` & `nkululeko-0.52.0/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/scaler.py` & `nkululeko-0.52.0/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/syllable_nuclei.py` & `nkululeko-0.52.0/nkululeko/syllable_nuclei.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/test.py` & `nkululeko-0.52.0/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/test_predictor.py` & `nkululeko-0.52.0/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/nkululeko/util.py` & `nkululeko-0.52.0/nkululeko/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,17 +85,17 @@
 
 
     def get_save_name(self):
         """Return a relative path to a name to save the experiment"""
         store = self.get_path('store')
         return f'{store}/{self.get_exp_name()}.pkl'
 
-    def is_categorical(array_like):
+    def is_categorical(self, pd_series):
         """Check if a dataframe column is categorical"""
-        return array_like.dtype.name == 'category'
+        return pd_series.dtype.name == 'object'
 
 
     def get_res_dir(self):
         root = glob_conf.config['EXP']['root']
         name = glob_conf.config['EXP']['name']
         dir_name = f'{root}{name}/results/'
         audeer.mkdir(dir_name)
```

### Comparing `nkululeko-0.51.0/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.52.0/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.51.0
+Version: 0.52.0
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -211,14 +211,18 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.52.0
+--------------
+* added flexible value distribution plots
+
 Version 0.51.0
 --------------
 * added datafilter
 
 Version 0.50.1
 --------------
 * added caller information for debug and error messages in Util
```

### Comparing `nkululeko-0.51.0/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.52.0/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.51.0/setup.cfg` & `nkululeko-0.52.0/setup.cfg`

 * *Files identical despite different names*

