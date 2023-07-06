# Comparing `tmp/Simba-UW-tf-dev-1.64.6.tar.gz` & `tmp/Simba-UW-tf-dev-1.64.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.64.6.tar", last modified: Wed Jul  5 14:01:33 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.64.7.tar", last modified: Thu Jul  6 16:46:40 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.64.6.tar` & `Simba-UW-tf-dev-1.64.7.tar`

### file list

```diff
@@ -1,583 +1,584 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-03 15:11:10.000000 Simba-UW-tf-dev-1.64.6/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    49615 2023-07-04 15:38:14.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3601 2023-07-03 00:19:12.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.64.6/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.64.6/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.64.6/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.64.6/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.64.6/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.64.6/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/labelling_interface_old.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.64.6/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.6/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-03 15:11:15.000000 Simba-UW-tf-dev-1.64.6/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-29 20:33:26.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    18368 2023-07-03 18:44:03.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.64.6/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-02 23:47:13.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/pose_importer_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/video_processing_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.64.6/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.64.6/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.64.6/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.6/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7698 2023-07-03 16:08:55.000000 Simba-UW-tf-dev-1.64.6/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     9041 2023-07-04 00:56:52.000000 Simba-UW-tf-dev-1.64.6/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43561 2023-07-03 19:45:27.000000 Simba-UW-tf-dev-1.64.6/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.64.6/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.64.6/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14889 2023-07-04 00:56:52.000000 Simba-UW-tf-dev-1.64.6/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.64.6/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.64.6/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/st/
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.64.6/simba/st/enums.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.64.6/simba/st/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.6/simba/st/select_groups_pg.py
--rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.6/simba/st/aggregate_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.64.6/simba/st/app.py
--rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.64.6/simba/st/welcome_page.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.6/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.6/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.6/simba/pose_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.6/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.6/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/pose_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/dash_app/dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.64.6/simba/dash_app/plotly_dash.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/mutual_exclusivity_corrector.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.64.6/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.64.6/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.6/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.64.6/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.64.6/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.64.6/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.64.6/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/ui/
--rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/ui/define_px_to_mm_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/
--rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/config_reader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/plotting_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/plotting/plot_pose_in_dir.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/pose_importers/anipose_csv_import.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.64.6/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    57974 2023-07-05 13:49:11.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    25424 2023-07-05 13:32:03.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/video_processing_new.py
--rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.64.6/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    66493 2023-07-04 00:43:21.000000 Simba-UW-tf-dev-1.64.6/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.6/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.64.6/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.64.6/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.64.6/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.64.6/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.64.6/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.64.6/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.6/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    21675 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-05 14:01:32.000000 Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.64.6/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.64.6/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.64.6/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.64.6/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.6/tests/test_interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.64.6/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.64.6/tests/test_pose_importers.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.64.6/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.64.6/tests/test_pose_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.64.6/tests/test_utils_data.py
--rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.64.6/tests/test_config_reader_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.64.6/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.64.6/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.64.6/tests/test_featurizers.py
--rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.64.6/tests/test_video_processors.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/video_processing/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/video_processing/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/video_processing/test_imgs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/expected_animal_bp_dict/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/models/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/models/generated_models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/models/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/models/validations/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/models/validations/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/videos/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/logs/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/logs/measures/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.64.6/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.64.6/tests/test_validation_clips.py
--rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.64.6/tests/test_roi_tools.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.64.6/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.64.6/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-05 14:01:25.000000 Simba-UW-tf-dev-1.64.6/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-05 14:01:33.000000 Simba-UW-tf-dev-1.64.6/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     9015 2023-06-29 20:55:17.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:42.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5814 2023-06-15 20:06:37.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    50444 2023-07-05 17:57:07.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3601 2023-07-03 00:19:12.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.64.7/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.64.7/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12879 2023-06-18 20:27:37.000000 Simba-UW-tf-dev-1.64.7/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.64.7/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35431 2023-06-13 17:24:57.000000 Simba-UW-tf-dev-1.64.7/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.64.7/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21667 2023-06-20 18:30:00.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface_old.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20914 2023-06-22 13:26:28.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26943 2023-06-20 19:04:35.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.64.7/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-13 17:25:39.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-07 20:28:11.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      421 2023-07-05 19:50:18.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_gpu.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30764 2023-06-13 17:23:34.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    18368 2023-07-03 18:44:03.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.64.7/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38224 2023-06-15 15:41:52.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/pose_importer_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2938 2023-07-02 20:03:29.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/video_processing_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9145 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73291 2023-06-19 20:46:57.000000 Simba-UW-tf-dev-1.64.7/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10759 2023-06-08 22:23:03.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    18417 2023-06-18 19:01:16.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18934 2023-06-18 19:03:04.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11876 2023-06-18 20:21:39.000000 Simba-UW-tf-dev-1.64.7/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21103 2023-06-20 12:58:32.000000 Simba-UW-tf-dev-1.64.7/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7801 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.7/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     9292 2023-07-05 17:27:17.000000 Simba-UW-tf-dev-1.64.7/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43615 2023-07-05 18:25:40.000000 Simba-UW-tf-dev-1.64.7/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     9841 2023-06-19 23:24:08.000000 Simba-UW-tf-dev-1.64.7/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.64.7/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15116 2023-07-05 17:33:58.000000 Simba-UW-tf-dev-1.64.7/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    19250 2023-06-13 13:46:20.000000 Simba-UW-tf-dev-1.64.7/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.64.7/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/st/
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-06-16 17:26:25.000000 Simba-UW-tf-dev-1.64.7/simba/st/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 13:55:39.000000 Simba-UW-tf-dev-1.64.7/simba/st/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2102 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.7/simba/st/select_groups_pg.py
+-rw-r--r--   0 simon      (501) staff       (20)     2325 2023-06-19 19:54:19.000000 Simba-UW-tf-dev-1.64.7/simba/st/aggregate_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     1485 2023-06-16 18:20:31.000000 Simba-UW-tf-dev-1.64.7/simba/st/app.py
+-rw-r--r--   0 simon      (501) staff       (20)      249 2023-06-16 18:20:19.000000 Simba-UW-tf-dev-1.64.7/simba/st/welcome_page.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5618 2023-06-13 18:36:10.000000 Simba-UW-tf-dev-1.64.7/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    14824 2023-07-05 12:33:51.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7660 2023-06-20 12:45:11.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/pose_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-16 12:50:41.000000 Simba-UW-tf-dev-1.64.7/simba/dash_app/plotly_dash.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16285 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    13451 2023-06-19 20:47:55.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     6087 2023-06-28 20:32:32.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/mutual_exclusivity_corrector.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.64.7/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.64.7/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.64.7/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.64.7/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.64.7/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43194 2023-06-22 13:51:00.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20174 2023-06-12 15:28:58.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)     2290 2023-06-12 16:21:03.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11474 2023-06-12 19:37:22.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5080 2023-06-22 13:37:25.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-20 12:44:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.64.7/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     1747 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/ui/define_px_to_mm_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)     6777 2023-06-26 17:04:03.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/feature_extractors/generic_feature_extractor.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)    38820 2023-06-23 01:28:48.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/config_reader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)    51001 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    50997 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)     1380 2023-06-26 13:52:31.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1379 2023-06-25 19:59:06.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     3758 2023-06-26 13:45:44.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     3953 2023-06-25 18:18:01.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/plotting_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     3192 2023-06-25 18:21:24.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/plotting/plot_pose_in_dir.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     3445 2023-06-22 22:21:05.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/pose_importers/anipose_csv_import.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5832 2023-06-23 13:06:19.000000 Simba-UW-tf-dev-1.64.7/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    59883 2023-07-05 17:43:17.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-07-06 15:33:05.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    25424 2023-07-05 13:32:03.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     3748 2023-07-02 21:12:43.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing_new.py
+-rw-r--r--   0 simon      (501) staff       (20)     7610 2023-07-03 18:21:05.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    13078 2023-07-05 13:23:30.000000 Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-06-17 18:48:37.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    66845 2023-07-06 16:27:17.000000 Simba-UW-tf-dev-1.64.7/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-06-15 21:18:05.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-06-23 01:30:05.000000 Simba-UW-tf-dev-1.64.7/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.64.7/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.64.7/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.64.7/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    21717 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-07-06 16:46:39.000000 Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.64.7/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.64.7/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.64.7/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.64.7/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-13 13:57:45.000000 Simba-UW-tf-dev-1.64.7/tests/test_interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)    12374 2023-06-07 20:44:17.000000 Simba-UW-tf-dev-1.64.7/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     2470 2023-06-12 20:51:29.000000 Simba-UW-tf-dev-1.64.7/tests/test_pose_importers.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.64.7/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-06-12 20:53:51.000000 Simba-UW-tf-dev-1.64.7/tests/test_pose_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     1774 2023-06-13 19:27:04.000000 Simba-UW-tf-dev-1.64.7/tests/test_utils_data.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.64.7/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.64.7/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.64.7/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.64.7/tests/test_featurizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     8736 2023-06-13 13:49:50.000000 Simba-UW-tf-dev-1.64.7/tests/test_video_processors.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/test_imgs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/video_processing/test_imgs/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/two_c57/expected_animal_bp_dict/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/generated_models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/generated_models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/validations/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/models/validations/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/videos/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/videos/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/project_folder/logs/measures/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.64.7/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.64.7/tests/test_validation_clips.py
+-rw-r--r--   0 simon      (501) staff       (20)     4463 2023-06-12 18:41:18.000000 Simba-UW-tf-dev-1.64.7/tests/test_roi_tools.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.64.7/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.64.7/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-07-06 16:44:59.000000 Simba-UW-tf-dev-1.64.7/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-06 16:46:40.000000 Simba-UW-tf-dev-1.64.7/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.64.6/PKG-INFO` & `Simba-UW-tf-dev-1.64.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.6
+Version: 1.64.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/ui/.DS_Store`

 * *Files 11% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 00001150: 6261 7208 0809 0809 5f10 197b 7b33 3534  bar....._..{{354
 00001160: 2c20 3132 347d 2c20 7b31 3037 362c 2036  , 124}, {1076, 6
 00001170: 3231 7d7d 0908 1725 313d 4960 6d79 7a7b  21}}...%1=I`myz{
 00001180: 7c7d 7e9a 0000 0000 0000 0101 0000 0000  |}~.............
 00001190: 0000 000f 0000 0000 0000 0000 0000 0000  ................
 000011a0: 0000 009b 0000 0007 0070 006f 0070 005f  .........p.o.p._
 000011b0: 0075 0070 0073 6c67 3153 636f 6d70 0000  .u.p.slg1Scomp..
-000011c0: 0000 000d e875 0000 0007 0070 006f 0070  .....u.....p.o.p
+000011c0: 0000 000e 1b54 0000 0007 0070 006f 0070  .....T.....p.o.p
 000011d0: 005f 0075 0070 0073 6c73 7643 626c 6f62  ._.u.p.slsvCblob
 000011e0: 0000 02b8 6270 6c69 7374 3030 da01 0203  ....bplist00....
 000011f0: 0405 0607 0809 0a0b 0c0d 1848 4948 4a0c  ...........HIHJ.
 00001200: 4c5f 1012 7669 6577 4f70 7469 6f6e 7356  L_..viewOptionsV
 00001210: 6572 7369 6f6e 5f10 0f73 686f 7749 636f  ersion_..showIco
 00001220: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
 00001230: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
@@ -369,20 +369,20 @@
 00001700: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001710: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001720: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001730: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001740: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001750: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001760: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001770: 6200 0000 0820 7622 c025 29c5 4100 0000  b.... v".%).A...
+00001770: 6200 0000 088b 58e4 39f3 2ac5 4100 0000  b.....X.9.*.A...
 00001780: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001790: 6f64 4462 6c6f 6200 0000 089f 9551 d210  odDblob......Q..
-000017a0: 27c5 4100 0000 0700 7000 6f00 7000 5f00  '.A.....p.o.p._.
+00001790: 6f64 4462 6c6f 6200 0000 088b 58e4 39f3  odDblob.....X.9.
+000017a0: 2ac5 4100 0000 0700 7000 6f00 7000 5f00  *.A.....p.o.p._.
 000017b0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-000017c0: 0000 1350 0000 0000 0700 7000 6f00 7000  ...P......p.o.p.
+000017c0: 0000 1380 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
 000017d0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 000017e0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 000017f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001800: 0000 0000 0000 0003 0000 0000 0000 180b  ................
 00001810: 0000 0045 0000 100b 0000 0000 0000 0000  ...E............
 00001820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -497,17 +497,17 @@
 00001f00: 7b01 7c01 7e01 8701 8801 8a01 8b01 8d01  {.|.~...........
 00001f10: 9601 9701 9901 9a01 9c01 a501 a601 a801  ................
 00001f20: a901 ab01 b401 b501 b801 b901 bb01 bc01  ................
 00001f30: c501 ce01 db01 dc00 0000 0000 0002 0100  ................
 00001f40: 0000 0000 0000 4c00 0000 0000 0000 0000  ......L.........
 00001f50: 0000 0000 0001 e500 0000 0700 7000 6f00  ............p.o.
 00001f60: 7000 5f00 7500 7000 736d 6f44 4462 6c6f  p._.u.p.smoDDblo
-00001f70: 6200 0000 0820 7622 c025 29c5 4100 0000  b.... v".%).A...
+00001f70: 6200 0000 088b 58e4 39f3 2ac5 4100 0000  b.....X.9.*.A...
 00001f80: 0700 7000 6f00 7000 5f00 7500 7000 736d  ..p.o.p._.u.p.sm
-00001f90: 6f64 4462 6c6f 6200 0000 089f 9551 d210  odDblob......Q..
-00001fa0: 27c5 4100 0000 0700 7000 6f00 7000 5f00  '.A.....p.o.p._.
+00001f90: 6f64 4462 6c6f 6200 0000 088b 58e4 39f3  odDblob.....X.9.
+00001fa0: 2ac5 4100 0000 0700 7000 6f00 7000 5f00  *.A.....p.o.p._.
 00001fb0: 7500 7000 7370 6831 5363 6f6d 7000 0000  u.p.sph1Scomp...
-00001fc0: 0000 1350 0000 0000 0700 7000 6f00 7000  ...P......p.o.p.
+00001fc0: 0000 1380 0000 0000 0700 7000 6f00 7000  ..........p.o.p.
 00001fd0: 5f00 7500 7000 7376 5372 6e6c 6f6e 6700  _.u.p.svSrnlong.
 00001fe0: 0000 0100 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/mutual_exclusivity_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/mutual_exclusivity_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -437,39 +437,42 @@
     def __init__(self):
         PopUpMixin.__init__(self, title="MERGE IMAGES TO VIDEO", size=(250, 250))
         self.folder_path = FolderSelect(self.main_frm, "IMAGE DIRECTORY", title='Select directory with frames: ')
         settings_frm = LabelFrame(self.main_frm, text='SETTINGS', padx=5, pady=5, font=Formats.LABELFRAME_HEADER_FORMAT.value, fg='black')
         self.img_format_entry_box = Entry_Box(settings_frm, 'IMAGE FORMAT (e.g. png): ', '20')
         self.bitrate_entry_box = Entry_Box(settings_frm, 'BITRATE (e.g. 8000): ', '20', validation='numeric')
         self.fps_entry = Entry_Box(settings_frm, 'FPS: ', '20', validation='numeric')
+        self.gpu_var = BooleanVar(value=False)
+        gpu_cb = Checkbutton(settings_frm, text='Use GPU (decreased runtime)', variable=self.gpu_var)
         run_btn = Button(settings_frm, text='Create Video', command=lambda: self.run())
-        settings_frm.grid(row=1,pady=10)
-        self.folder_path.grid(row=0,column=0,pady=10)
-        self.img_format_entry_box.grid(row=1,column=0,sticky=W)
-        self.fps_entry.grid(row=2,column=0,sticky=W,pady=5)
-        self.bitrate_entry_box.grid(row=3,column=0,sticky=W,pady=5)
-        run_btn.grid(row=4,column=1,sticky=E,pady=10)
+        settings_frm.grid(row=1, pady=10)
+        self.folder_path.grid(row=0,column=0, pady=10)
+        self.img_format_entry_box.grid(row=1, column=0, sticky=W)
+        self.fps_entry.grid(row=2,column=0,sticky=W, pady=5)
+        self.bitrate_entry_box.grid(row=3, column=0, sticky=W,pady=5)
+        gpu_cb.grid(row=4, column=0, sticky=W, pady=5)
+        run_btn.grid(row=5,column=1, sticky=E, pady=10)
 
     def run(self):
         img_format = self.img_format_entry_box.entry_get
         bitrate = self.bitrate_entry_box.entry_get
         fps = self.fps_entry.entry_get
-        _ = frames_to_movie(directory=self.folder_path.folder_path, fps=fps, bitrate=bitrate, img_format=img_format)
+        _ = frames_to_movie(directory=self.folder_path.folder_path, fps=fps, bitrate=bitrate, img_format=img_format, gpu=self.gpu_var.get())
 
 
 class CreateGIFPopUP(PopUpMixin):
     def __init__(self):
         PopUpMixin.__init__(self, title="CREATE GIF FROM VIDEO", size=(250, 250))
         settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         selected_video = FileSelect(settings_frm, 'Video path: ', title='Select a video file')
         start_time_entry_box = Entry_Box(settings_frm, 'Start time (s): ', '16', validation='numeric')
         duration_entry_box = Entry_Box(settings_frm, 'Duration (s): ', '16', validation='numeric')
         width_entry_box = Entry_Box(settings_frm, 'Width: ', '16', validation='numeric')
         gpu_var = BooleanVar()
-        gpu_cb = Checkbutton(settings_frm, text='Use GPU (potential runtime improvement)', variable=gpu_var)
+        gpu_cb = Checkbutton(settings_frm, text='Use GPU (decreased runtime)', variable=gpu_var)
         width_instructions_1 = Label(settings_frm, text='example Width: 240, 360, 480, 720, 1080', font=("Times", 10, "italic"))
         width_instructions_2 = Label(settings_frm, text='Aspect ratio is kept (i.e., height is automatically computed)', font=("Times", 10, "italic"))
         run_btn = Button(settings_frm,text='CREATE GIF', command=lambda:gif_creator(file_path=selected_video.file_path, start_time=start_time_entry_box.entry_get, duration=duration_entry_box.entry_get, width=width_entry_box.entry_get, gpu=gpu_var.get()))
         settings_frm.grid(row=0,sticky=NW)
         selected_video.grid(row=0,sticky=NW,pady=5)
         start_time_entry_box.grid(row=1,sticky=NW)
         duration_entry_box.grid(row=2,sticky=NW)
@@ -606,38 +609,48 @@
 
 class VideoRotatorPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='ROTATE VIDEOS')
         self.save_dir_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SAVE LOCATION', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
         self.save_dir = FolderSelect(self.save_dir_frm, 'Save directory:', lblwidth=20)
 
+        self.setting_frm = LabelFrame(self.main_frm, text='SETTINGS', font=Formats.LABELFRAME_HEADER_FORMAT.value)
+        self.use_gpu_var = BooleanVar(value=False)
+        self.use_ffmpeg_var = BooleanVar(value=False)
+        use_gpu_cb = Checkbutton(self.setting_frm, text='Use GPU (reduced runtime)', variable=self.use_gpu_var)
+        use_ffmpeg_cb = Checkbutton(self.setting_frm, text='Use FFMpeg (reduced runtime over default OpenCV)', variable=self.use_ffmpeg_var)
+        use_gpu_cb.grid(row=0, column=0, sticky=NW)
+        use_ffmpeg_cb.grid(row=1, column=0, sticky=NW)
+
         self.rotate_dir_frm = LabelFrame(self.main_frm, text='ROTATE VIDEOS IN DIRECTORY', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.input_dir = FolderSelect(self.rotate_dir_frm, 'Video directory:', lblwidth=20)
         self.run_dir = Button(self.rotate_dir_frm, text='RUN', fg='blue', command=lambda: self.run(input_path=self.input_dir.folder_path,
                                                                                                    output_path=self.save_dir.folder_path))
 
         self.rotate_video_frm = LabelFrame(self.main_frm, text='ROTATE SINGLE VIDEO', font=Formats.LABELFRAME_HEADER_FORMAT.value)
         self.input_file = FileSelect(self.rotate_video_frm, "Video path:", lblwidth=20)
-        self.run_file = Button(self.rotate_video_frm, text='RUN', fg='blue', command=lambda: self.run(input_path=self.input_file.file_path,
-                                                                                                   output_path=self.save_dir.folder_path))
+        self.run_file = Button(self.rotate_video_frm, text='RUN', fg='blue', command=lambda: self.run(input_path=self.input_file.file_path, output_path=self.save_dir.folder_path))
+
 
         self.save_dir_frm.grid(row=0, column=0, sticky=NW)
         self.save_dir.grid(row=0, column=0, sticky=NW)
 
-        self.rotate_dir_frm.grid(row=1, column=0, sticky=NW)
+        self.setting_frm.grid(row=1, column=0, sticky=NW)
+
+        self.rotate_dir_frm.grid(row=2, column=0, sticky=NW)
         self.input_dir.grid(row=0, column=0, sticky=NW)
         self.run_dir.grid(row=1, column=0, sticky=NW)
 
-        self.rotate_video_frm.grid(row=2, column=0, sticky=NW)
+        self.rotate_video_frm.grid(row=3, column=0, sticky=NW)
         self.input_file.grid(row=0, column=0, sticky=NW)
         self.run_file.grid(row=1, column=0, sticky=NW)
 
     def run(self, input_path: str, output_path: str):
         check_if_dir_exists(in_dir=output_path)
-        rotator = VideoRotator(input_path=input_path, output_dir=output_path)
+        rotator = VideoRotator(input_path=input_path, output_dir=output_path, ffmpeg=self.use_ffmpeg_var.get(), gpu=self.use_gpu_var.get())
         rotator.run()
 
 
 class VideoTemporalJoinPopUp(PopUpMixin):
     def __init__(self):
         super().__init__(title='TEMPORAL JOIN VIDEOS')
         self.settings_frm = CreateLabelFrameWithIcon(parent=self.main_frm, header='SETTINGS', icon_name=Keys.DOCUMENTATION.value, icon_link=Links.VIDEO_TOOLS.value)
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.64.7/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/labelling/labelling_interface_old.py` & `Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface_old.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.64.7/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.64.7/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.64.7/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/hdbscan_clusterer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.64.7/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.64.7/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -60,68 +60,68 @@
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0003 0000 0001 0000 000b  ................
 00000410: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
-00000420: 006e 0067 6c73 7643 626c 6f62 0000 0349  .n.glsvCblob...I
+00000420: 006e 0067 6c73 7643 626c 6f62 0000 032b  .n.glsvCblob...+
 00000430: 6270 6c69 7374 3030 da01 0203 0405 0607  bplist00........
-00000440: 0809 0a0b 0c0d 1858 595a 5b0c 5d58 6963  .......XYZ[.]Xic
-00000450: 6f6e 5369 7a65 5f10 0f73 686f 7749 636f  onSize_..showIco
-00000460: 6e50 7265 7669 6577 5763 6f6c 756d 6e73  nPreviewWcolumns
-00000470: 5f10 1163 616c 6375 6c61 7465 416c 6c53  _..calculateAllS
-00000480: 697a 6573 5f10 0f73 6372 6f6c 6c50 6f73  izes_..scrollPos
-00000490: 6974 696f 6e59 5874 6578 7453 697a 655f  itionYXtextSize_
-000004a0: 100f 7363 726f 6c6c 506f 7369 7469 6f6e  ..scrollPosition
-000004b0: 585a 736f 7274 436f 6c75 6d6e 5f10 1075  XZsortColumn_..u
-000004c0: 7365 5265 6c61 7469 7665 4461 7465 735f  seRelativeDates_
-000004d0: 1012 7669 6577 4f70 7469 6f6e 7356 6572  ..viewOptionsVer
-000004e0: 7369 6f6e 2340 3000 0000 0000 0009 ae0e  sion#@0.........
-000004f0: 171c 2125 2a2f 3439 3e43 474f 53d4 0f10  ..!%*/49>CGOS...
-00000500: 1112 0c14 0c16 5776 6973 6962 6c65 5577  ......WvisibleUw
-00000510: 6964 7468 5961 7363 656e 6469 6e67 5a69  idthYascendingZi
-00000520: 6465 6e74 6966 6965 7209 1101 c709 546e  dentifier.....Tn
-00000530: 616d 65d4 0f10 1112 1819 181b 0810 2308  ame...........#.
-00000540: 5875 6269 7175 6974 79d4 0f10 1112 0c1e  Xubiquity.......
-00000550: 1820 0910 b508 5c64 6174 654d 6f64 6966  . ....\dateModif
-00000560: 6965 64d4 0f10 1112 181e 1824 0808 5b64  ied........$..[d
-00000570: 6174 6543 7265 6174 6564 d40f 1011 120c  ateCreated......
-00000580: 2718 2909 1061 0854 7369 7a65 d40f 1011  '.)..a.Tsize....
-00000590: 120c 2c0c 2e09 1073 0954 6b69 6e64 d40f  ..,....s.Tkind..
-000005a0: 1011 1218 310c 3308 1064 0955 6c61 6265  ....1.3..d.Ulabe
-000005b0: 6cd4 0f10 1112 1836 0c38 0810 4b09 5776  l......6.8..K.Wv
-000005c0: 6572 7369 6f6e d40f 1011 1218 3b0c 3d08  ersion......;.=.
-000005d0: 1101 2c09 5863 6f6d 6d65 6e74 73d4 0f10  ..,.Xcomments...
-000005e0: 1112 1840 1842 0810 c808 5e64 6174 654c  ...@.B....^dateL
-000005f0: 6173 744f 7065 6e65 64d4 0f10 1112 181e  astOpened.......
-00000600: 1846 0808 5964 6174 6541 6464 6564 d448  .F..YdateAdded.H
-00000610: 494a 1218 4c18 4e57 7669 7369 626c 6555  IJ..L.NWvisibleU
-00000620: 7769 6474 6859 6173 6365 6e64 696e 6708  widthYascending.
-00000630: 10d2 085a 7368 6172 654f 776e 6572 d448  ...ZshareOwner.H
-00000640: 494a 1218 4c18 5208 085f 100f 7368 6172  IJ..L.R.._..shar
-00000650: 654c 6173 7445 6469 746f 72d4 4849 4a12  eLastEditor.HIJ.
-00000660: 184c 1856 0808 5f10 1069 6e76 6974 6174  .L.V.._..invitat
-00000670: 696f 6e53 7461 7475 7308 2340 5e40 0000  ionStatus.#@^@..
-00000680: 0000 0023 4028 0000 0000 0000 2340 0000  ...#@(......#@..
-00000690: 0000 0000 0054 6e61 6d65 0910 0100 0800  .....Tname......
-000006a0: 1d00 2600 3800 4000 5400 6600 6f00 8100  ..&.8.@.T.f.o...
-000006b0: 8c00 9f00 b400 bd00 be00 cd00 d600 de00  ................
-000006c0: e400 ee00 f900 fa00 fd00 fe01 0301 0c01  ................
-000006d0: 0d01 0f01 1001 1901 2201 2301 2501 2601  ........".#.%.&.
-000006e0: 3301 3c01 3d01 3e01 4a01 5301 5401 5601  3.<.=.>.J.S.T.V.
-000006f0: 5701 5c01 6501 6601 6801 6901 6e01 7701  W.\.e.f.h.i.n.w.
-00000700: 7801 7a01 7b01 8101 8a01 8b01 8d01 8e01  x.z.{...........
-00000710: 9601 9f01 a001 a301 a401 ad01 b601 b701  ................
-00000720: b901 ba01 c901 d201 d301 d401 de01 e701  ................
-00000730: ef01 f501 ff02 0002 0202 0302 0e02 1702  ................
-00000740: 1802 1902 2b02 3402 3502 3602 4902 4a02  ....+.4.5.6.I.J.
-00000750: 5302 5c02 6502 6a02 6b00 0000 0000 0002  S.\.e.j.k.......
-00000760: 0100 0000 0000 0000 5e00 0000 0000 0000  ........^.......
-00000770: 0000 0000 0000 0002 6d3c 0050 0059 0064  ........m<.P.Y.d
+00000440: 0809 0a0b 0c0d 1855 5657 580c 5a5f 1012  .......UVWX.Z_..
+00000450: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
+00000460: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
+00000470: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00000480: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00000490: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+000004a0: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+000004b0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+000004c0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000004d0: 6c61 7469 7665 4461 7465 7358 6963 6f6e  lativeDatesXicon
+000004e0: 5369 7a65 1001 09ae 0e17 1c21 252a 2f34  Size.......!%*/4
+000004f0: 393e 4347 4c50 d40f 1011 120c 140c 1657  9>CGLP.........W
+00000500: 7669 7369 626c 6555 7769 6474 6859 6173  visibleUwidthYas
+00000510: 6365 6e64 696e 675a 6964 656e 7469 6669  cendingZidentifi
+00000520: 6572 0911 01c7 0954 6e61 6d65 d40f 1011  er.....Tname....
+00000530: 1218 1918 1b08 1023 0858 7562 6971 7569  .......#.Xubiqui
+00000540: 7479 d40f 1011 120c 1e18 2009 10b5 085c  ty........ ....\
+00000550: 6461 7465 4d6f 6469 6669 6564 d40f 1011  dateModified....
+00000560: 1218 1e18 2408 085b 6461 7465 4372 6561  ....$..[dateCrea
+00000570: 7465 64d4 0f10 1112 0c27 1829 0910 6108  ted......'.)..a.
+00000580: 5473 697a 65d4 0f10 1112 0c2c 0c2e 0910  Tsize......,....
+00000590: 7309 546b 696e 64d4 0f10 1112 1831 0c33  s.Tkind......1.3
+000005a0: 0810 6409 556c 6162 656c d40f 1011 1218  ..d.Ulabel......
+000005b0: 360c 3808 104b 0957 7665 7273 696f 6ed4  6.8..K.Wversion.
+000005c0: 0f10 1112 183b 0c3d 0811 012c 0958 636f  .....;.=...,.Xco
+000005d0: 6d6d 656e 7473 d40f 1011 1218 4018 4208  mments......@.B.
+000005e0: 10c8 085e 6461 7465 4c61 7374 4f70 656e  ...^dateLastOpen
+000005f0: 6564 d40f 1011 1218 1e18 4608 0859 6461  ed........F..Yda
+00000600: 7465 4164 6465 64d4 0f10 1112 1849 184b  teAdded......I.K
+00000610: 0810 d208 5a73 6861 7265 4f77 6e65 72d4  ....ZshareOwner.
+00000620: 0f10 1112 1849 184f 0808 5f10 0f73 6861  .....I.O.._..sha
+00000630: 7265 4c61 7374 4564 6974 6f72 d40f 1011  reLastEditor....
+00000640: 1218 4918 5308 085f 1010 696e 7669 7461  ..I.S.._..invita
+00000650: 7469 6f6e 5374 6174 7573 0823 0000 0000  tionStatus.#....
+00000660: 0000 0000 2340 2800 0000 0000 0023 4000  ....#@(......#@.
+00000670: 0000 0000 0000 546e 616d 6509 2340 3000  ......Tname.#@0.
+00000680: 0000 0000 0000 0800 1d00 3200 4400 4c00  ..........2.D.L.
+00000690: 6000 7200 7b00 8d00 9800 ab00 b400 b600  `.r.{...........
+000006a0: b700 c600 cf00 d700 dd00 e700 f200 f300  ................
+000006b0: f600 f700 fc01 0501 0601 0801 0901 1201  ................
+000006c0: 1b01 1c01 1e01 1f01 2c01 3501 3601 3701  ........,.5.6.7.
+000006d0: 4301 4c01 4d01 4f01 5001 5501 5e01 5f01  C.L.M.O.P.U.^._.
+000006e0: 6101 6201 6701 7001 7101 7301 7401 7a01  a.b.g.p.q.s.t.z.
+000006f0: 8301 8401 8601 8701 8f01 9801 9901 9c01  ................
+00000700: 9d01 a601 af01 b001 b201 b301 c201 cb01  ................
+00000710: cc01 cd01 d701 e001 e101 e301 e401 ef01  ................
+00000720: f801 f901 fa02 0c02 1502 1602 1702 2a02  ..............*.
+00000730: 2b02 3402 3d02 4602 4b02 4c00 0000 0000  +.4.=.F.K.L.....
+00000740: 0002 0100 0000 0000 0000 5b00 0000 0000  ..........[.....
+00000750: 0000 0000 0000 0000 0002 5500 0000 0000  ..........U.....
+00000760: 5c64 6174 654d 6f64 6966 6965 6409 1001  \dateModified...
+00000770: 0008 0019 0022 0034 003c 0050 0059 0064  .....".4.<.P.Y.d
 00000780: 0077 008c 0095 0096 00a2 00ab 00b6 00bc  .w..............
 00000790: 00c6 00ce 00d3 00d6 00d7 00d8 00e1 00ea  ................
 000007a0: 00ec 00ed 00ee 00f7 00f8 00fa 00fb 0108  ................
 000007b0: 0111 011d 011e 011f 0128 012d 012f 0130  .........(.-./.0
 000007c0: 0131 013a 013f 0141 0142 0143 014c 0152  .1.:.?.A.B.C.L.R
 000007d0: 0154 0155 0156 015f 0167 0169 016a 016b  .T.U.V._.g.i.j.k
 000007e0: 0174 017d 0180 0181 0182 018b 019a 019c  .t.}............
@@ -497,24 +497,24 @@
 00001f00: 6444 626c 6f62 0000 0008 cbf3 6409 d917  dDblob......d...
 00001f10: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
 00001f20: 0065 0072 0076 0069 0073 0065 0064 7068  .e.r.v.i.s.e.dph
 00001f30: 3153 636f 6d70 0000 0000 0004 d000 0000  1Scomp..........
 00001f40: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
 00001f50: 0076 0069 0073 0065 0064 7653 726e 6c6f  .v.i.s.e.dvSrnlo
 00001f60: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
-00001f70: 006c 0073 6277 7370 626c 6f62 0000 00c9  .l.sbwspblob....
-00001f80: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-00001f90: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-00001fa0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-00001fb0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00001fc0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00001fd0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00001fe0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00001ff0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-00002000: 187b 7b32 0000 0007 0000 0003 0000 0004  .{{2............
+00001f70: 006c 0073 6277 7370 626c 6f62 0000 00b9  .l.sbwspblob....
+00001f80: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
+00001f90: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00001fa0: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
+00001fb0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001fc0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001fd0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00001fe0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
+00001ff0: 1019 7b7b 3730 352c 2032 3037 7d2c 207b  ..{{705, 207}, {
+00002000: 3132 3437 0000 0007 0000 0003 0000 0004  1247............
 00002010: 0000 0012 0062 006f 0075 006e 0064 0069  .....b.o.u.n.d.i
 00002020: 006e 0067 005f 0062 006f 0078 005f 0074  .n.g._.b.o.x._.t
 00002030: 006f 006f 006c 0073 6c73 7670 626c 6f62  .o.o.l.slsvpblob
 00002040: 0000 025e 6270 6c69 7374 3030 d801 0203  ...^bplist00....
 00002050: 0405 0607 0809 0a0b 1d45 4647 0a5f 1012  .........EFG._..
 00002060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00002070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
@@ -764,15 +764,15 @@
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003000: 0000 0000 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 0008 6b70 0000 0005 0075  mp......kp.....u
+00003020: 6d70 0000 0000 0008 78a2 0000 0005 0075  mp......x......u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,142 +848,142 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 083a fcc1  smoDDblob....:..
-00003570: 5480 22c5 4100 0000 0500 7500 7400 6900  T.".A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 083a  l.smodDblob....:
-00003590: fcc1 5480 22c5 4100 0000 0500 7500 7400  ..T.".A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 0886 592f  smoDDblob.....Y/
+00003570: 92f6 2ac5 4100 0000 0500 7500 7400 6900  ..*.A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 0886  l.smodDblob.....
+00003590: 592f 92f6 2ac5 4100 0000 0500 7500 7400  Y/..*.A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 09f0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
+000035b0: 0000 0a00 0000 0000 0500 7500 7400 6900  ..........u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
-000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
-00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
-00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
-00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
-00003630: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00003640: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00003650: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00003660: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00003670: 7753 6964 6562 6172 0808 0908 095f 1018  wSidebar....._..
-00003680: 7b7b 3333 352c 2031 3938 7d2c 207b 3932  {{335, 198}, {92
-00003690: 372c 2035 3638 7d7d 0908 1725 313d 4960  7, 568}}...%1=I`
-000036a0: 6d79 7a7b 7c7d 7e99 0000 0000 0000 0101  myz{|}~.........
-000036b0: 0000 0000 0000 000f 0000 0000 0000 0000  ................
-000036c0: 0000 0000 0000 009a 0000 0010 0076 0069  .............v.i
-000036d0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
-000036e0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
-000036f0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
-00003700: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
-00003710: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
-00003720: 7000 0000 0000 05b6 ca00 0000 1000 7600  p.............v.
-00003730: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
-00003740: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
-00003750: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
-00003760: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
-00003770: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
-00003780: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00003790: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-000037a0: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-000037b0: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-000037c0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000037d0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-000037e0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
-000037f0: 0c15 1d22 262b 3035 3a3f 44d4 0d0e 0f10  ..."&+05:?D.....
-00003800: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
-00003810: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00003820: 7669 7369 626c 6554 6e61 6d65 1101 c709  visibleTname....
-00003830: 09d4 1617 180d 191a 191c 5776 6973 6962  ..........Wvisib
-00003840: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
-00003850: 6e67 0810 2308 5875 6269 7175 6974 79d4  ng..#.Xubiquity.
-00003860: 0d0e 0f10 1e1f 190a 5c64 6174 654d 6f64  ........\dateMod
-00003870: 6966 6965 6410 b508 09d4 0d0e 0f10 231f  ified.........#.
-00003880: 1919 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
-00003890: d40d 0e0f 1027 2819 0a54 7369 7a65 1061  .....'(..Tsize.a
-000038a0: 0809 d40d 0e0f 102c 2d0a 0a54 6b69 6e64  .......,-..Tkind
-000038b0: 1073 0909 d40d 0e0f 1031 320a 1955 6c61  .s.......12..Ula
-000038c0: 6265 6c10 6409 08d4 0d0e 0f10 3637 0a19  bel.d.......67..
-000038d0: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
-000038e0: 103b 3c0a 1958 636f 6d6d 656e 7473 1101  .;<..Xcomments..
-000038f0: 2c09 08d4 0d0e 0f10 4041 1919 5e64 6174  ,.......@A..^dat
-00003900: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
-00003910: 1617 180d 191f 1947 0808 5964 6174 6541  .......G..YdateA
-00003920: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
-00003930: 616d 6509 1001 0008 0019 0022 0034 003c  ame........".4.<
-00003940: 0050 0059 0064 0077 008c 0095 0096 00a2  .P.Y.d.w........
-00003950: 00ab 00b6 00bc 00c6 00ce 00d3 00d6 00d7  ................
-00003960: 00d8 00e1 00e9 00ef 00f9 00fa 00fc 00fd  ................
-00003970: 0106 010f 011c 011e 011f 0120 0129 0135  ........... .).5
-00003980: 0136 0137 0140 0145 0147 0148 0149 0152  .6.7.@.E.G.H.I.R
-00003990: 0157 0159 015a 015b 0164 016a 016c 016d  .W.Y.Z.[.d.j.l.m
-000039a0: 016e 0177 017f 0181 0182 0183 018c 0195  .n.w............
-000039b0: 0198 0199 019a 01a3 01b2 01b4 01b5 01b6  ................
-000039c0: 01bf 01c0 01c1 01cb 01cc 01d5 01da 01db  ................
-000039d0: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
-000039e0: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
-000039f0: 0000 0010 0076 0069 0064 0065 006f 005f  .....v.i.d.e.o._
-00003a00: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
-00003a10: 0072 0073 6c73 7670 626c 6f62 0000 025e  .r.slsvpblob...^
-00003a20: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
-00003a30: 0809 0a0b 1a46 470a 4458 6963 6f6e 5369  .....FG.DXiconSi
-00003a40: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
-00003a50: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00003a60: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00003a70: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
-00003a80: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-00003a90: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
-00003aa0: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
-00003ab0: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
-00003ac0: 151e 2328 2d32 373c 4158 636f 6d6d 656e  ..#(-27<AXcommen
-00003ad0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
-00003ae0: 645b 6461 7465 4372 6561 7465 6454 7369  d[dateCreatedTsi
-00003af0: 7a65 556c 6162 656c 546b 696e 6457 7665  zeUlabelTkindWve
-00003b00: 7273 696f 6e54 6e61 6d65 5c64 6174 654d  rsionTname\dateM
-00003b10: 6f64 6966 6965 64d4 1617 1819 1a1b 0a1d  odified.........
-00003b20: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
-00003b30: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
-00003b40: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
-00003b50: c808 1008 d416 1718 191a 251a 2708 10b5  ..........%.'...
-00003b60: 0810 02d4 1617 1819 0a2a 1a2c 0910 6108  .........*.,..a.
-00003b70: 1003 d416 1718 191a 2f0a 3108 1064 0910  ......../.1..d..
-00003b80: 05d4 1617 1819 0a34 0a36 0910 7309 1004  .......4.6..s...
-00003b90: d416 1718 191a 390a 3b08 104b 0910 06d4  ......9.;..K....
-00003ba0: 1617 1819 0a3e 0a40 0911 01c7 0910 00d4  .....>.@........
-00003bb0: 1617 1819 0a25 1a44 0908 1001 0823 4028  .....%.D.....#@(
-00003bc0: 0000 0000 0000 546e 616d 6509 0008 0019  ......Tname.....
-00003bd0: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
-00003be0: 0095 0096 00a9 00b2 00c1 00cd 00d2 00d8  ................
-00003bf0: 00dd 00e5 00ea 00f7 0100 0108 010e 0118  ................
-00003c00: 011e 011f 0122 0123 0125 012e 012f 0131  .....".#.%.../.1
-00003c10: 0132 0134 013d 013e 0140 0141 0143 014c  .2.4.=.>.@.A.C.L
-00003c20: 014d 014f 0150 0152 015b 015c 015e 015f  .M.O.P.R.[.\.^._
-00003c30: 0161 016a 016b 016d 016e 0170 0179 017a  .a.j.k.m.n.p.y.z
-00003c40: 017c 017d 017f 0188 0189 018c 018d 018f  .|.}............
-00003c50: 0198 0199 019a 019c 019d 01a6 01ab 0000  ................
-00003c60: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
-00003c70: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
-00003c80: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
-00003c90: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003ca0: 0073 6d6f 4444 626c 6f62 0000 0008 0295  .smoDDblob......
-00003cb0: 8be5 0f29 c541 0000 0010 0076 0069 0064  ...).A.....v.i.d
-00003cc0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
-00003cd0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
-00003ce0: 6f62 0000 0008 586d 22f8 6428 c541 0000  ob....Xm".d(.A..
-00003cf0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
-00003d00: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
-00003d10: 0073 7068 3153 636f 6d70 0000 0000 0007  .sph1Scomp......
-00003d20: 1000 0000 0010 0076 0069 0064 0065 006f  .......v.i.d.e.o
-00003d30: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
-00003d40: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
-00003d50: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+000035f0: 7200 7362 7773 7062 6c6f 6200 0000 b962  r.sbwspblob....b
+00003600: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
+00003610: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
+00003620: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
+00003630: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
+00003640: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
+00003650: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
+00003660: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
+00003670: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
+00003680: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
+00003690: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
+000036a0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+000036b0: 0000 0000 0000 008c 0000 0010 0076 0069  .............v.i
+000036c0: 0064 0065 006f 005f 0070 0072 006f 0063  .d.e.o._.p.r.o.c
+000036d0: 0065 0073 0073 006f 0072 0073 6473 636c  .e.s.s.o.r.sdscl
+000036e0: 626f 6f6c 0000 0000 1000 7600 6900 6400  bool......v.i.d.
+000036f0: 6500 6f00 5f00 7000 7200 6f00 6300 6500  e.o._.p.r.o.c.e.
+00003700: 7300 7300 6f00 7200 736c 6731 5363 6f6d  s.s.o.r.slg1Scom
+00003710: 7000 0000 0000 0622 c000 0000 1000 7600  p......"......v.
+00003720: 6900 6400 6500 6f00 5f00 7000 7200 6f00  i.d.e.o._.p.r.o.
+00003730: 6300 6500 7300 7300 6f00 7200 736c 7376  c.e.s.s.o.r.slsv
+00003740: 4362 6c6f 6200 0002 9762 706c 6973 7430  Cblob....bplist0
+00003750: 30d8 0102 0304 0506 0708 090a 0b19 494a  0.............IJ
+00003760: 0a4c 5869 636f 6e53 697a 655f 100f 7368  .LXiconSize_..sh
+00003770: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
+00003780: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
+00003790: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
+000037a0: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
+000037b0: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
+000037c0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+000037d0: 7273 696f 6e23 4030 0000 0000 0000 09ab  rsion#@0........
+000037e0: 0c15 1d22 262b 3035 3a3f 44d4 0d0e 0f10  ..."&+05:?D.....
+000037f0: 1112 0a0a 5a69 6465 6e74 6966 6965 7255  ....ZidentifierU
+00003800: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
+00003810: 7669 7369 626c 6554 6e61 6d65 1101 c709  visibleTname....
+00003820: 09d4 1617 180d 191a 191c 5776 6973 6962  ..........Wvisib
+00003830: 6c65 5577 6964 7468 5961 7363 656e 6469  leUwidthYascendi
+00003840: 6e67 0810 2308 5875 6269 7175 6974 79d4  ng..#.Xubiquity.
+00003850: 0d0e 0f10 1e1f 190a 5c64 6174 654d 6f64  ........\dateMod
+00003860: 6966 6965 6410 b508 09d4 0d0e 0f10 231f  ified.........#.
+00003870: 1919 5b64 6174 6543 7265 6174 6564 0808  ..[dateCreated..
+00003880: d40d 0e0f 1027 2819 0a54 7369 7a65 1061  .....'(..Tsize.a
+00003890: 0809 d40d 0e0f 102c 2d0a 0a54 6b69 6e64  .......,-..Tkind
+000038a0: 1073 0909 d40d 0e0f 1031 320a 1955 6c61  .s.......12..Ula
+000038b0: 6265 6c10 6409 08d4 0d0e 0f10 3637 0a19  bel.d.......67..
+000038c0: 5776 6572 7369 6f6e 104b 0908 d40d 0e0f  Wversion.K......
+000038d0: 103b 3c0a 1958 636f 6d6d 656e 7473 1101  .;<..Xcomments..
+000038e0: 2c09 08d4 0d0e 0f10 4041 1919 5e64 6174  ,.......@A..^dat
+000038f0: 654c 6173 744f 7065 6e65 6410 c808 08d4  eLastOpened.....
+00003900: 1617 180d 191f 1947 0808 5964 6174 6541  .......G..YdateA
+00003910: 6464 6564 0823 4028 0000 0000 0000 546e  dded.#@(......Tn
+00003920: 616d 6509 1001 0008 0019 0022 0034 003c  ame........".4.<
+00003930: 0050 0059 0064 0077 008c 0095 0096 00a2  .P.Y.d.w........
+00003940: 00ab 00b6 00bc 00c6 00ce 00d3 00d6 00d7  ................
+00003950: 00d8 00e1 00e9 00ef 00f9 00fa 00fc 00fd  ................
+00003960: 0106 010f 011c 011e 011f 0120 0129 0135  ........... .).5
+00003970: 0136 0137 0140 0145 0147 0148 0149 0152  .6.7.@.E.G.H.I.R
+00003980: 0157 0159 015a 015b 0164 016a 016c 016d  .W.Y.Z.[.d.j.l.m
+00003990: 016e 0177 017f 0181 0182 0183 018c 0195  .n.w............
+000039a0: 0198 0199 019a 01a3 01b2 01b4 01b5 01b6  ................
+000039b0: 01bf 01c0 01c1 01cb 01cc 01d5 01da 01db  ................
+000039c0: 0000 0000 0000 0201 0000 0000 0000 004d  ...............M
+000039d0: 0000 0000 0000 0000 0000 0000 0000 01dd  ................
+000039e0: 0000 0010 0076 0069 0064 0065 006f 005f  .....v.i.d.e.o._
+000039f0: 0070 0072 006f 0063 0065 0073 0073 006f  .p.r.o.c.e.s.s.o
+00003a00: 0072 0073 6c73 7670 626c 6f62 0000 025e  .r.slsvpblob...^
+00003a10: 6270 6c69 7374 3030 d801 0203 0405 0607  bplist00........
+00003a20: 0809 0a0b 1a46 470a 4458 6963 6f6e 5369  .....FG.DXiconSi
+00003a30: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00003a40: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00003a50: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00003a60: 5874 6578 7453 697a 655a 736f 7274 436f  XtextSizeZsortCo
+00003a70: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+00003a80: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
+00003a90: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
+00003aa0: 0000 0000 0009 d90c 0d0e 0f10 1112 1314  ................
+00003ab0: 151e 2328 2d32 373c 4158 636f 6d6d 656e  ..#(-27<AXcommen
+00003ac0: 7473 5e64 6174 654c 6173 744f 7065 6e65  ts^dateLastOpene
+00003ad0: 645b 6461 7465 4372 6561 7465 6454 7369  d[dateCreatedTsi
+00003ae0: 7a65 556c 6162 656c 546b 696e 6457 7665  zeUlabelTkindWve
+00003af0: 7273 696f 6e54 6e61 6d65 5c64 6174 654d  rsionTname\dateM
+00003b00: 6f64 6966 6965 64d4 1617 1819 1a1b 0a1d  odified.........
+00003b10: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00003b20: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
+00003b30: 012c 0910 07d4 1617 1819 1a20 1a22 0810  .,......... ."..
+00003b40: c808 1008 d416 1718 191a 251a 2708 10b5  ..........%.'...
+00003b50: 0810 02d4 1617 1819 0a2a 1a2c 0910 6108  .........*.,..a.
+00003b60: 1003 d416 1718 191a 2f0a 3108 1064 0910  ......../.1..d..
+00003b70: 05d4 1617 1819 0a34 0a36 0910 7309 1004  .......4.6..s...
+00003b80: d416 1718 191a 390a 3b08 104b 0910 06d4  ......9.;..K....
+00003b90: 1617 1819 0a3e 0a40 0911 01c7 0910 00d4  .....>.@........
+00003ba0: 1617 1819 0a25 1a44 0908 1001 0823 4028  .....%.D.....#@(
+00003bb0: 0000 0000 0000 546e 616d 6509 0008 0019  ......Tname.....
+00003bc0: 0022 0034 003c 0050 0059 0064 0077 008c  .".4.<.P.Y.d.w..
+00003bd0: 0095 0096 00a9 00b2 00c1 00cd 00d2 00d8  ................
+00003be0: 00dd 00e5 00ea 00f7 0100 0108 010e 0118  ................
+00003bf0: 011e 011f 0122 0123 0125 012e 012f 0131  .....".#.%.../.1
+00003c00: 0132 0134 013d 013e 0140 0141 0143 014c  .2.4.=.>.@.A.C.L
+00003c10: 014d 014f 0150 0152 015b 015c 015e 015f  .M.O.P.R.[.\.^._
+00003c20: 0161 016a 016b 016d 016e 0170 0179 017a  .a.j.k.m.n.p.y.z
+00003c30: 017c 017d 017f 0188 0189 018c 018d 018f  .|.}............
+00003c40: 0198 0199 019a 019c 019d 01a6 01ab 0000  ................
+00003c50: 0000 0000 0201 0000 0000 0000 0049 0000  .............I..
+00003c60: 0000 0000 0000 0000 0000 0000 01ac 0000  ................
+00003c70: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
+00003c80: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
+00003c90: 0073 6d6f 4444 626c 6f62 0000 0008 3e94  .smoDDblob....>.
+00003ca0: a59a f12a c541 0000 0010 0076 0069 0064  ...*.A.....v.i.d
+00003cb0: 0065 006f 005f 0070 0072 006f 0063 0065  .e.o._.p.r.o.c.e
+00003cc0: 0073 0073 006f 0072 0073 6d6f 6444 626c  .s.s.o.r.smodDbl
+00003cd0: 6f62 0000 0008 707b be2b d62a c541 0000  ob....p{.+.*.A..
+00003ce0: 0010 0076 0069 0064 0065 006f 005f 0070  ...v.i.d.e.o._.p
+00003cf0: 0072 006f 0063 0065 0073 0073 006f 0072  .r.o.c.e.s.s.o.r
+00003d00: 0073 7068 3153 636f 6d70 0000 0000 0007  .sph1Scomp......
+00003d10: 7000 0000 0010 0076 0069 0064 0065 006f  p......v.i.d.e.o
+00003d20: 005f 0070 0072 006f 0063 0065 0073 0073  ._.p.r.o.c.e.s.s
+00003d30: 006f 0072 0073 7653 726e 6c6f 6e67 0000  .o.r.svSrnlong..
+00003d40: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00003d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1035,20 +1035,20 @@
 000040a0: 0073 0069 006d 0062 0061 002f 0000 000b  .s.i.m.b.a./....
 000040b0: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 000040c0: 002e 0070 0079 7074 624e 7573 7472 0000  ...p.yptbNustr..
 000040d0: 000b 005f 005f 0069 006e 0069 0074 005f  ..._._.i.n.i.t._
 000040e0: 005f 002e 0070 0079 0000 000b 005f 005f  ._...p.y....._._
 000040f0: 0070 0079 0063 0061 0063 0068 0065 005f  .p.y.c.a.c.h.e._
 00004100: 005f 6c67 3153 636f 6d70 0000 0000 0002  ._lg1Scomp......
-00004110: 5d82 0000 000b 005f 005f 0070 0079 0063  ]......_._.p.y.c
+00004110: 5ebd 0000 000b 005f 005f 0070 0079 0063  ^......_._.p.y.c
 00004120: 0061 0063 0068 0065 005f 005f 6d6f 4444  .a.c.h.e._._moDD
-00004130: 626c 6f62 0000 0008 e2d6 95d5 1027 c541  blob.........'.A
+00004130: 626c 6f62 0000 0008 85f6 aa84 f02a c541  blob.........*.A
 00004140: 0000 000b 005f 005f 0070 0079 0063 0061  ....._._.p.y.c.a
 00004150: 0063 0068 0065 005f 005f 6d6f 6444 626c  .c.h.e._._modDbl
-00004160: 6f62 0000 0008 fef2 7934 1721 c541 0000  ob......y4.!.A..
+00004160: 6f62 0000 0008 2902 255f d129 c541 0000  ob....).%_.).A..
 00004170: 000b 005f 005f 0070 0079 0063 0061 0063  ..._._.p.y.c.a.c
 00004180: 0068 0065 005f 005f 7068 3153 636f 6d70  .h.e._._ph1Scomp
 00004190: 0000 0000 0002 a000 0000 0006 0061 0073  .............a.s
 000041a0: 0073 0065 0074 0073 6277 7370 626c 6f62  .s.e.t.sbwspblob
 000041b0: 0000 00b5 6270 6c69 7374 3030 d601 0203  ....bplist00....
 000041c0: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
 000041d0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
@@ -1489,15 +1489,15 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 0b53 c910 c808 5e64  omp......S....^d
+00005d70: 6f6d 7000 0000 0000 0b5a cc10 c808 5e64  omp......Z....^d
 00005d80: 6174 654c 6173 744f 7065 6e65 64d4 0d0e  ateLastOpened...
 00005d90: 0f10 161c 1644 0808 5964 6174 6541 6464  .....D..YdateAdd
 00005da0: 6564 0823 4028 0000 0000 0000 546e 616d  ed.#@(......Tnam
 00005db0: 6523 4030 0000 0000 0000 0900 0800 1900  e#@0............
 00005dc0: 2e00 4000 4800 5c00 6500 7000 7900 8c00  ..@.H.\.e.p.y...
 00005dd0: 8e00 8f00 9b00 a400 ac00 b200 bc00 c700  ................
 00005de0: c800 cb00 cc00 d100 da00 db00 dd00 de00  ................
@@ -1579,22 +1579,22 @@
 000062a0: a501 ae01 b001 b201 b301 b401 bd01 bf01  ................
 000062b0: c201 c301 c401 c501 ce01 d701 e400 0000  ................
 000062c0: 0000 0002 0100 0000 0000 0000 4c00 0000  ............L...
 000062d0: 0000 0000 0000 0000 0000 0001 e500 0000  ................
 000062e0: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000062f0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 00006300: 6f00 7200 736d 6f44 4462 6c6f 6200 0000  o.r.smoDDblob...
-00006310: 08da 0969 fb83 29c5 4100 0000 1200 6600  ...i..).A.....f.
+00006310: 087c 26ff 39a7 29c5 4100 0000 1200 6600  .|&.9.).A.....f.
 00006320: 6500 6100 7400 7500 7200 6500 5f00 6500  e.a.t.u.r.e._.e.
 00006330: 7800 7400 7200 6100 6300 7400 6f00 7200  x.t.r.a.c.t.o.r.
-00006340: 736d 6f64 4462 6c6f 6200 0000 08da 0969  smodDblob......i
-00006350: fb83 29c5 4100 0000 1200 6600 6500 6100  ..).A.....f.e.a.
+00006340: 736d 6f64 4462 6c6f 6200 0000 087c 26ff  smodDblob....|&.
+00006350: 39a7 29c5 4100 0000 1200 6600 6500 6100  9.).A.....f.e.a.
 00006360: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
 00006370: 7200 6100 6300 7400 6f00 7200 7370 6831  r.a.c.t.o.r.sph1
-00006380: 5363 6f6d 7000 0000 0000 0dd0 0000 0000  Scomp...........
+00006380: 5363 6f6d 7000 0000 0000 0de0 0000 0000  Scomp...........
 00006390: 1200 6600 6500 6100 7400 7500 7200 6500  ..f.e.a.t.u.r.e.
 000063a0: 5f00 6500 7800 7400 7200 6100 6300 7400  _.e.x.t.r.a.c.t.
 000063b0: 6f00 7200 7376 5372 6e6c 6f6e 6700 0000  o.r.svSrnlong...
 000063c0: 0100 0000 0900 6c00 6100 6200 6500 6c00  ......l.a.b.e.l.
 000063d0: 6c00 6900 6e00 6762 7773 7062 6c6f 6200  l.i.n.gbwspblob.
 000063e0: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
 000063f0: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
@@ -1790,16 +1790,16 @@
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
 00007020: 626c 6f62 0000 0008 e4a6 81c8 0729 c541  blob.........).A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 71b7 5521  modDblob....q.U!
-00007050: fd28 c541 0000 0006 006d 0069 0078 0069  .(.A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 e4a6 81c8  modDblob........
+00007050: 0729 c541 0000 0006 006d 0069 0078 0069  .).A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
 00007070: 0011 c000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
@@ -2020,86 +2020,86 @@
 00007e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00007e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00007e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
 00007e60: 0000 0210 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00007e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00007e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00007e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-00007ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b862  n.gbwspblob....b
+00007ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b962  n.gbwspblob....b
 00007eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
 00007ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00007ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
 00007ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
 00007ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
 00007f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
 00007f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00007f20: 187b 7b33 3335 2c20 3139 387d 2c20 7b39  .{{335, 198}, {9
-00007f30: 3237 2c20 3536 387d 7d09 0815 232f 3b52  27, 568}}...#/;R
-00007f40: 5f6b 6c6d 6e6f 8a00 0000 0000 0001 0100  _klmno..........
-00007f50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-00007f60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
-00007f70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00007f80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+00007f20: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
+00007f30: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
+00007f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
+00007f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+00007f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
+00007f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
+00007f80: 636f 6d70 0000 0000 000f f490 0000 0000  comp............
 00007f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
 00008010: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00008020: 6c73 7670 626c 6f62 0000 02a0 6270 6c69  lsvpblob....bpli
 00008030: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
-00008040: 0c0d 1f48 494a 4b0c 3558 6963 6f6e 5369  ...HIJK.5XiconSi
-00008050: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
-00008060: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
-00008070: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
-00008080: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
-00008090: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
-000080a0: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
-000080b0: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
-000080c0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
-000080d0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
-000080e0: 2340 3000 0000 0000 0009 d90e 0f10 1112  #@0.............
-000080f0: 1314 1516 1720 252a 2f34 383d 4258 636f  ..... %*/48=BXco
-00008100: 6d6d 656e 7473 556c 6162 656c 5776 6572  mmentsUlabelWver
-00008110: 7369 6f6e 5b64 6174 6543 7265 6174 6564  sion[dateCreated
-00008120: 5473 697a 655c 6461 7465 4d6f 6469 6669  Tsize\dateModifi
-00008130: 6564 546b 696e 6454 6e61 6d65 5e64 6174  edTkindTname^dat
-00008140: 654c 6173 744f 7065 6e65 64d4 1819 1a1b  eLastOpened.....
-00008150: 1c1d 0c1f 5569 6e64 6578 5577 6964 7468  ....UindexUwidth
-00008160: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00008170: 6c65 1007 1101 2c09 08d4 1819 1a1b 2122  le....,.......!"
-00008180: 0c1f 1005 1064 0908 d418 191a 1b26 270c  .....d.......&'.
-00008190: 1f10 0610 4b09 08d4 1819 1a1b 2b2c 1f1f  ....K.......+,..
-000081a0: 1002 10b5 0808 d418 191a 1b30 311f 0c10  ...........01...
-000081b0: 0310 6108 09d4 1819 1a1b 352c 1f0c 1001  ..a.......5,....
-000081c0: 0809 d418 191a 1b39 3a0c 0c10 0410 7309  .......9:.....s.
-000081d0: 09d4 1819 1a1b 3e3f 0c0c 1000 1101 c709  ......>?........
-000081e0: 09d4 1819 1a1b 4344 1f1f 1008 10c8 0808  ......CD........
-000081f0: 0823 405e 4000 0000 0000 2340 2800 0000  .#@^@.....#@(...
-00008200: 0000 0023 4000 0000 0000 0000 546e 616d  ...#@.......Tnam
-00008210: 6509 0008 001d 0026 0038 0040 0054 0066  e......&.8.@.T.f
-00008220: 006f 0081 008c 009f 00b4 00bd 00be 00d1  .o..............
-00008230: 00da 00e0 00e8 00f4 00f9 0106 010b 0110  ................
-00008240: 011f 0128 012e 0134 013e 0146 0148 014b  ...(...4.>.F.H.K
-00008250: 014c 014d 0156 0158 015a 015b 015c 0165  .L.M.V.X.Z.[.\.e
-00008260: 0167 0169 016a 016b 0174 0176 0178 0179  .g.i.j.k.t.v.x.y
-00008270: 017a 0183 0185 0187 0188 0189 0192 0194  .z..............
-00008280: 0195 0196 019f 01a1 01a3 01a4 01a5 01ae  ................
-00008290: 01b0 01b3 01b4 01b5 01be 01c0 01c2 01c3  ................
-000082a0: 01c4 01c5 01ce 01d7 01e0 01e5 0000 0000  ................
+00008040: 0c0d 1f47 4849 4a0c 4c5f 1012 7669 6577  ...GHIJ.L_..view
+00008050: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
+00008060: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
+00008070: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
+00008080: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
+00008090: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
+000080a0: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
+000080b0: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
+000080c0: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
+000080d0: 7665 4461 7465 7358 6963 6f6e 5369 7a65  veDatesXiconSize
+000080e0: 1001 09d9 0e0f 1011 1213 1415 1617 2025  .............. %
+000080f0: 2a2f 3437 3c41 5863 6f6d 6d65 6e74 7355  */47<AXcommentsU
+00008100: 6c61 6265 6c57 7665 7273 696f 6e5b 6461  labelWversion[da
+00008110: 7465 4372 6561 7465 6454 7369 7a65 5c64  teCreatedTsize\d
+00008120: 6174 654d 6f64 6966 6965 6454 6b69 6e64  ateModifiedTkind
+00008130: 546e 616d 655e 6461 7465 4c61 7374 4f70  Tname^dateLastOp
+00008140: 656e 6564 d418 191a 1b1c 1d0c 1f55 696e  ened.........Uin
+00008150: 6465 7855 7769 6474 6859 6173 6365 6e64  dexUwidthYascend
+00008160: 696e 6757 7669 7369 626c 6510 0711 012c  ingWvisible....,
+00008170: 0908 d418 191a 1b21 220c 1f10 0510 6409  .......!".....d.
+00008180: 08d4 1819 1a1b 2627 0c1f 1006 104b 0908  ......&'.....K..
+00008190: d418 191a 1b2b 2c1f 1f10 0210 b508 08d4  .....+,.........
+000081a0: 1819 1a1b 3031 1f0c 1003 1061 0809 d418  ....01.....a....
+000081b0: 191a 1b0b 2c1f 0c08 09d4 1819 1a1b 3839  ....,.........89
+000081c0: 0c0c 1004 1073 0909 d418 191a 1b3d 3e0c  .....s.......=>.
+000081d0: 0c10 0011 01c7 0909 d418 191a 1b42 431f  .............BC.
+000081e0: 1f10 0810 c808 0808 2300 0000 0000 0000  ........#.......
+000081f0: 0023 4028 0000 0000 0000 2340 0000 0000  .#@(......#@....
+00008200: 0000 0054 6e61 6d65 0923 4030 0000 0000  ...Tname.#@0....
+00008210: 0000 0008 001d 0032 0044 004c 0060 0072  .......2.D.L.`.r
+00008220: 007b 008d 0098 00ab 00b4 00b6 00b7 00ca  .{..............
+00008230: 00d3 00d9 00e1 00ed 00f2 00ff 0104 0109  ................
+00008240: 0118 0121 0127 012d 0137 013f 0141 0144  ...!.'.-.7.?.A.D
+00008250: 0145 0146 014f 0151 0153 0154 0155 015e  .E.F.O.Q.S.T.U.^
+00008260: 0160 0162 0163 0164 016d 016f 0171 0172  .`.b.c.d.m.o.q.r
+00008270: 0173 017c 017e 0180 0181 0182 018b 018c  .s.|.~..........
+00008280: 018d 0196 0198 019a 019b 019c 01a5 01a7  ................
+00008290: 01aa 01ab 01ac 01b5 01b7 01b9 01ba 01bb  ................
+000082a0: 01bc 01c5 01ce 01d7 01dc 01dd 0000 0000  ................
 000082b0: 0000 0201 0000 0000 0000 004d 0000 0000  ...........M....
 000082c0: 0000 0000 0000 0000 0000 01e6 0000 0008  ................
 000082d0: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
-000082e0: 6d6f 4444 626c 6f62 0000 0008 8d4a a152  moDDblob.....J.R
-000082f0: 1321 c541 0000 0008 0070 006c 006f 0074  .!.A.....p.l.o.t
+000082e0: 6d6f 4444 626c 6f62 0000 0008 f673 8c57  moDDblob.....s.W
+000082f0: cd2a c541 0000 0008 0070 006c 006f 0074  .*.A.....p.l.o.t
 00008300: 0074 0069 006e 0067 6d6f 6444 626c 6f62  .t.i.n.gmodDblob
-00008310: 0000 0008 8d4a a152 1321 c541 0000 0008  .....J.R.!.A....
+00008310: 0000 0008 f673 8c57 cd2a c541 0000 0008  .....s.W.*.A....
 00008320: 0070 006c 006f 0074 0074 0069 006e 0067  .p.l.o.t.t.i.n.g
 00008330: 7068 3153 636f 6d70 0000 0000 0014 2000  ph1Scomp...... .
 00008340: 0000 0008 0070 006c 006f 0074 0074 0069  .....p.l.o.t.t.i
 00008350: 006e 0067 7653 726e 6c6f 6e67 0000 0001  .n.gvSrnlong....
 00008360: 0000 0013 0070 006f 0073 0065 005f 0063  .....p.o.s.e._.c
 00008370: 006f 006e 0066 0069 0067 0075 0072 0061  .o.n.f.i.g.u.r.a
 00008380: 0074 0069 006f 006e 0073 6277 7370 626c  .t.i.o.n.sbwspbl
@@ -2276,29 +2276,29 @@
 00008e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00008e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00008e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
 00008e60: 0000 0210 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00008e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00008e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00008e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-00008ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b862  n.gbwspblob....b
+00008ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b962  n.gbwspblob....b
 00008eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
 00008ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00008ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
 00008ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
 00008ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
 00008f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
 00008f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00008f20: 187b 7b33 3335 2c20 3139 387d 2c20 7b39  .{{335, 198}, {9
-00008f30: 3237 2c20 3536 387d 7d09 0815 232f 3b52  27, 568}}...#/;R
-00008f40: 5f6b 6c6d 6e6f 8a00 0000 0000 0001 0100  _klmno..........
-00008f50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-00008f60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
-00008f70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00008f80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+00008f20: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
+00008f30: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
+00008f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
+00008f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+00008f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
+00008f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
+00008f80: 636f 6d70 0000 0000 000f f490 0000 0000  comp............
 00008f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2532,29 +2532,29 @@
 00009e30: 01b6 01bb 01c4 0000 0000 0000 0201 0000  ................
 00009e40: 0000 0000 004a 0000 0000 0000 0000 0000  .....J..........
 00009e50: 0000 0000 01c5 6831 5363 6f6d 7000 0000  ......h1Scomp...
 00009e60: 0000 0210 0000 0000 0d00 6f00 7500 7400  ..........o.u.t.
 00009e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00009e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00009e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
-00009ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b862  n.gbwspblob....b
+00009ea0: 6e00 6762 7773 7062 6c6f 6200 0000 b962  n.gbwspblob....b
 00009eb0: 706c 6973 7430 30d6 0102 0304 0506 0708  plist00.........
 00009ec0: 0708 0b08 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
 00009ed0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
 00009ee0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
 00009ef0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
 00009f00: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
 00009f10: 686f 7753 6964 6562 6172 0809 0809 5f10  howSidebar...._.
-00009f20: 187b 7b33 3335 2c20 3139 387d 2c20 7b39  .{{335, 198}, {9
-00009f30: 3237 2c20 3536 387d 7d09 0815 232f 3b52  27, 568}}...#/;R
-00009f40: 5f6b 6c6d 6e6f 8a00 0000 0000 0001 0100  _klmno..........
-00009f50: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-00009f60: 0000 0000 0000 8b00 0000 0800 7000 6c00  ............p.l.
-00009f70: 6f00 7400 7400 6900 6e00 676c 6731 5363  o.t.t.i.n.glg1Sc
-00009f80: 6f6d 7000 0000 0000 0fe6 ce00 0000 0000  omp.............
+00009f20: 197b 7b37 3035 2c20 3230 377d 2c20 7b31  .{{705, 207}, {1
+00009f30: 3234 372c 2035 3638 7d7d 0908 1523 2f3b  247, 568}}...#/;
+00009f40: 525f 6b6c 6d6e 6f8b 0000 0000 0000 0101  R_klmno.........
+00009f50: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+00009f60: 0000 0000 0000 008c 0000 0008 0070 006c  .............p.l
+00009f70: 006f 0074 0074 0069 006e 0067 6c67 3153  .o.t.t.i.n.glg1S
+00009f80: 636f 6d70 0000 0000 000f f490 0000 0000  comp............
 00009f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -2727,15 +2727,15 @@
 0000aa60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000aa70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000aa80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000aa90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000aaa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000aab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000aac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000aad0: 0000 0000 0011 ddd7 0000 0002 0075 0069  .............u.i
+0000aad0: 0000 0000 0012 10b6 0000 0002 0075 0069  .............u.i
 0000aae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000aaf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000ab00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000ab10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000ab20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000ab30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000ab40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -2812,15 +2812,15 @@
 0000afb0: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
 0000afc0: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
 0000afd0: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
 0000afe0: 6f44 4462 6c6f 6200 0000 087e abce 1cd0  oDDblob....~....
 0000aff0: 1fc5 4100 0000 0000 0000 0000 0000 0000  ..A.............
 0000b000: 0000 0000 0000 0000 0000 000c 0000 0002  ................
 0000b010: 0075 0069 7068 3153 636f 6d70 0000 0000  .u.iph1Scomp....
-0000b020: 0018 1000 0000 0002 0075 0069 7653 726e  .........u.ivSrn
+0000b020: 0018 4000 0000 0002 0075 0069 7653 726e  ..@......u.ivSrn
 0000b030: 6c6f 6e67 0000 0001 0000 000c 0075 006e  long.........u.n
 0000b040: 0073 0075 0070 0065 0072 0076 0069 0073  .s.u.p.e.r.v.i.s
 0000b050: 0065 0064 6277 7370 626c 6f62 0000 00ca  .e.dbwspblob....
 0000b060: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
 0000b070: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
 0000b080: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
 0000b090: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
@@ -2929,28 +2929,28 @@
 0000b700: 6444 626c 6f62 0000 0008 cbf3 6409 d917  dDblob......d...
 0000b710: c541 0000 000c 0075 006e 0073 0075 0070  .A.....u.n.s.u.p
 0000b720: 0065 0072 0076 0069 0073 0065 0064 7068  .e.r.v.i.s.e.dph
 0000b730: 3153 636f 6d70 0000 0000 0004 d000 0000  1Scomp..........
 0000b740: 000c 0075 006e 0073 0075 0070 0065 0072  ...u.n.s.u.p.e.r
 0000b750: 0076 0069 0073 0065 0064 7653 726e 6c6f  .v.i.s.e.dvSrnlo
 0000b760: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
-0000b770: 006c 0073 6277 7370 626c 6f62 0000 00c9  .l.sbwspblob....
-0000b780: 6270 6c69 7374 3030 d701 0203 0405 0607  bplist00........
-0000b790: 0808 0a08 0a0d 0a5d 5368 6f77 5374 6174  .......]ShowStat
-0000b7a0: 7573 4261 725b 5368 6f77 5061 7468 6261  usBar[ShowPathba
-0000b7b0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-0000b7c0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-0000b7d0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-0000b7e0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-0000b7f0: 6f77 5369 6465 6261 7208 0809 0809 5f10  owSidebar....._.
-0000b800: 187b 7b32 302c 2032 3336 7d2c 207b 3130  .{{20, 236}, {10
-0000b810: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
-0000b820: 606d 797a 7b7c 7d7e 9900 0000 0000 0001  `myz{|}~........
-0000b830: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
-0000b840: 0000 0000 0000 0000 9a00 6500 6e00 6400  ..........e.n.d.
+0000b770: 006c 0073 6277 7370 626c 6f62 0000 00b9  .l.sbwspblob....
+0000b780: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
+0000b790: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
+0000b7a0: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
+0000b7b0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+0000b7c0: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+0000b7d0: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+0000b7e0: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
+0000b7f0: 1019 7b7b 3730 352c 2032 3037 7d2c 207b  ..{{705, 207}, {
+0000b800: 3132 3437 2c20 3536 387d 7d09 0815 232f  1247, 568}}...#/
+0000b810: 3b52 5f6b 6c6d 6e6f 8b00 0000 0000 0001  ;R_klmno........
+0000b820: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+0000b830: 0000 0000 0000 0000 8c00 6100 6200 6500  ..........a.b.e.
+0000b840: 6c00 5f00 6100 7000 7000 6500 6e00 6400  l._.a.p.p.e.n.d.
 0000b850: 6500 7200 736d 6f64 4462 6c6f 6200 0000  e.r.smodDblob...
 0000b860: 086b 121b 34c6 1fc5 4100 0000 1b00 7400  .k..4...A.....t.
 0000b870: 6800 6900 7200 6400 5f00 7000 6100 7200  h.i.r.d._.p.a.r.
 0000b880: 7400 7900 5f00 6c00 6100 6200 6500 6c00  t.y._.l.a.b.e.l.
 0000b890: 5f00 6100 7000 7000 6500 6e00 6400 6500  _.a.p.p.e.n.d.e.
 0000b8a0: 7200 7370 6831 5363 6f6d 7000 0000 0000  r.sph1Scomp.....
 0000b8b0: 0530 0000 0000 1b00 7400 6800 6900 7200  .0......t.h.i.r.
@@ -2983,15 +2983,15 @@
 0000ba60: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000ba70: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000ba80: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000ba90: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000baa0: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000bab0: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000bac0: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000bad0: 0000 0000 0011 ddd7 0000 0002 0075 0069  .............u.i
+0000bad0: 0000 0000 0012 10b6 0000 0002 0075 0069  .............u.i
 0000bae0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000baf0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000bb00: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000bb10: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000bb20: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000bb30: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000bb40: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -276,20 +276,20 @@
 00001130: 5f10 197b 7b34 3732 2c20 3134 327d 2c20  _..{{472, 142}, 
 00001140: 7b31 3037 362c 2036 3231 7d7d 0908 1725  {1076, 621}}...%
 00001150: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 00001160: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 00001170: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001180: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001190: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000011a0: 0000 0004 43ec 0000 000b 005f 005f 0070  ....C......_._.p
+000011a0: 0000 0004 473f 0000 000b 005f 005f 0070  ....G?....._._.p
 000011b0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000011c0: 6d6f 4444 626c 6f62 0000 0008 2dea ae91  moDDblob....-...
-000011d0: 0927 c541 0000 000b 005f 005f 0070 0079  .'.A....._._.p.y
+000011c0: 6d6f 4444 626c 6f62 0000 0008 1611 2c41  moDDblob......,A
+000011d0: a729 c541 0000 000b 005f 005f 0070 0079  .).A....._._.p.y
 000011e0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-000011f0: 6444 626c 6f62 0000 0008 2dea ae91 0927  dDblob....-....'
+000011f0: 6444 626c 6f62 0000 0008 1611 2c41 a729  dDblob......,A.)
 00001200: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 00001210: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
 00001220: 636f 6d70 0000 0000 0005 0000 0000 000b  comp............
 00001230: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001240: 0065 005f 005f 7653 726e 6c6f 6e67 0000  .e._._vSrnlong..
 00001250: 0001 0000 0004 006d 0069 0073 0063 6277  .......m.i.s.cbw
 00001260: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
@@ -304,15 +304,15 @@
 000012f0: 2c20 3139 387d 2c20 7b39 3237 2c20 3536  , 198}, {927, 56
 00001300: 387d 7d09 0817 2531 3d49 606d 797a 7b7c  8}}...%1=I`myz{|
 00001310: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00001320: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00001330: 0000 9a00 0000 0400 6d00 6900 7300 6364  ........m.i.s.cd
 00001340: 7363 6c62 6f6f 6c00 0000 0004 006d 0069  sclbool......m.i
 00001350: 0073 0063 6c67 3153 636f 6d70 0000 0000  .s.clg1Scomp....
-00001360: 0003 1e60 0000 0004 006d 0069 0073 0063  ...`.....m.i.s.c
+00001360: 0003 2005 0000 0004 006d 0069 0073 0063  .. ......m.i.s.c
 00001370: 6c73 7643 626c 6f62 0000 02b8 6270 6c69  lsvCblob....bpli
 00001380: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
 00001390: 0c0d 1848 4948 4a0c 4c58 6963 6f6e 5369  ...HIHJ.LXiconSi
 000013a0: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
 000013b0: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 000013c0: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
 000013d0: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
@@ -394,19 +394,19 @@
 00001890: 8101 8301 8501 8601 8701 9001 9201 9401  ................
 000018a0: 9501 9601 9f01 a101 a301 a401 a501 ae01  ................
 000018b0: b001 b201 b301 b401 bd01 be01 c101 c201  ................
 000018c0: c401 c501 ce01 d701 e400 0000 0000 0002  ................
 000018d0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000018e0: 0000 0000 0000 0001 e500 0000 0400 6d00  ..............m.
 000018f0: 6900 7300 636d 6f44 4462 6c6f 6200 0000  i.s.cmoDDblob...
-00001900: 0886 4f6e cb6e 1cc5 4100 0000 0400 6d00  ..On.n..A.....m.
+00001900: 0801 e269 7d00 2bc5 4100 0000 0400 6d00  ...i}.+.A.....m.
 00001910: 6900 7300 636d 6f64 4462 6c6f 6200 0000  i.s.cmodDblob...
-00001920: 0886 4f6e cb6e 1cc5 4100 0000 0400 6d00  ..On.n..A.....m.
+00001920: 0801 e269 7d00 2bc5 4100 0000 0400 6d00  ...i}.+.A.....m.
 00001930: 6900 7300 6370 6831 5363 6f6d 7000 0000  i.s.cph1Scomp...
-00001940: 0000 0410 0000 0000 0400 6d00 6900 7300  ..........m.i.s.
+00001940: 0000 0420 0000 0000 0400 6d00 6900 7300  ... ......m.i.s.
 00001950: 6376 5372 6e6c 6f6e 6700 0000 0100 0000  cvSrnlong.......
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000019b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.64.7/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/requirements.txt` & `Simba-UW-tf-dev-1.64.7/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/.DS_Store`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
 00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 000b f7a8 0000 000b 005f 005f 0070  ..........._._.p
+00000130: 0000 0004 7300 0000 000b 005f 005f 0070  ....s......_._.p
 00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 61f9 77e8  moDDblob....a.w.
-00000160: 2129 c541 0000 000b 005f 005f 0070 0079  !).A....._._.p.y
+00000150: 6d6f 4444 626c 6f62 0000 0008 41ed 4121  moDDblob....A.A!
+00000160: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
 00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 c0be a523 fd28  dDblob.......#.(
+00000180: 6444 626c 6f62 0000 0008 41ed 4121 1721  dDblob....A.A!.!
 00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 000d 0000 0000 0000  comp............
+000001b0: 636f 6d70 0000 0000 0005 f000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/video_processing_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/video_processing_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/mixins/train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.64.7/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/enums.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/utils/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -253,23 +253,23 @@
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 000e 0000 000b  ................
 00001010: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001020: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001030: 0000 0006 052f 0000 000b 005f 005f 0070  ...../....._._.p
+00001030: 0000 0006 0cc4 0000 000b 005f 005f 0070  ..........._._.p
 00001040: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00001050: 6d6f 4444 626c 6f62 0000 0008 daad 7e57  moDDblob......~W
-00001060: 8022 c541 0000 000b 005f 005f 0070 0079  .".A....._._.p.y
+00001050: 6d6f 4444 626c 6f62 0000 0008 7b56 d344  moDDblob....{V.D
+00001060: 002b c541 0000 000b 005f 005f 0070 0079  .+.A....._._.p.y
 00001070: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00001080: 6444 626c 6f62 0000 0008 daad 7e57 8022  dDblob......~W."
+00001080: 6444 626c 6f62 0000 0008 7b56 d344 002b  dDblob....{V.D.+
 00001090: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
 000010a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000010b0: 636f 6d70 0000 0000 0007 2000 0000 0003  comp...... .....
+000010b0: 636f 6d70 0000 0000 0007 3000 0000 0003  comp......0.....
 000010c0: 0063 006c 0069 6277 7370 626c 6f62 0000  .c.l.ibwspblob..
 000010d0: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 000010e0: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 000010f0: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
 00001100: 6261 725b 5368 6f77 546f 6f6c 6261 725b  bar[ShowToolbar[
 00001110: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
 00001120: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/warnings.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,8 +128,11 @@
     stdout_warning(msg=f'SIMBA PYTHON VERSION WARNING: {msg}')
 
 def BorisPointEventsWarning(msg: str):
     stdout_warning(msg=f'SIMBA BORIS POINT EVENT WARNING: {msg}')
 
 
 def FFMpegCodecWarning(msg: str):
-    stdout_warning(msg=f'SIMBA FFMPEG CODEC WARNING: {msg}')
+    stdout_warning(msg=f'SIMBA FFMPEG CODEC WARNING: {msg}')
+
+def FFMpegNotFoundWarning(msg: str):
+    stdout_warning(msg=f'SIMBA FFMPEG NOT FOUND WARNING: {msg}')
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/checks.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/checks.py`

 * *Files 3% similar despite different names*

```diff
@@ -256,8 +256,17 @@
 
 def check_nvidea_gpu_available() -> bool:
     """ Helper to check of NVIDEA GPU is available"""
     try:
         subprocess.check_output('nvidia-smi')
         return True
     except Exception:
-        return False
+        return False
+
+
+def check_ffmpeg_available() -> bool:
+    """ Helper to check of FFMpeg is available"""
+    try:
+        subprocess.call('ffmpeg', stderr=subprocess.DEVNULL, stdout=subprocess.DEVNULL)
+        return True
+    except Exception:
+        return False
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/read_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
                                 NoFilesFoundError,
                                 DataHeaderError,
                                 FileExistError)
 from simba.utils.warnings import InvalidValueWarning, NoFileFoundWarning, FileExistWarning
 from simba.utils.printing import stdout_success
 from simba.utils.enums import Formats, Dtypes, ConfigKey
 from simba.utils.checks import (check_file_exist_and_readable,
-                                check_if_filepath_list_is_empty)
+                                check_if_filepath_list_is_empty,
+                                check_nvidea_gpu_available)
 
 PARSE_OPTIONS = csv.ParseOptions(delimiter=',')
 READ_OPTIONS = csv.ReadOptions(encoding='utf8')
 
 def read_df(file_path: Union[str, os.PathLike],
             file_type: Union[str, os.PathLike],
             has_index: Optional[bool] = True,
@@ -354,23 +355,22 @@
     :parameter Optional[str] video_format: Format of the input video files in ``in_folder``. Default: ``mp4``.
     :parameter Optional[bool] remove_splits: If true, the input splits in the ``in_folder`` will be removed following concatenation. Default: True.
     """
 
     timer = SimbaTimer(start=True)
     files = glob.glob(in_folder + '/*.{}'.format(video_format))
     check_if_filepath_list_is_empty(filepaths=files,
-                                    error_msg='SIMBA ERROR: Cannot join videos in {}. The directory contain ZERO files.'.format(
-                                        in_folder))
+                                    error_msg='SIMBA ERROR: Cannot join videos in directory {}. The directory contain ZERO files.'.format(in_folder))
     files.sort(key=lambda f: int(re.sub('\D', '', f)))
     temp_txt_path = Path(in_folder, 'files.txt')
     with open(temp_txt_path, 'w') as f:
         for file in files:
             f.write("file '" + str(Path(file)) + "'\n")
     if os.path.exists(save_path): os.remove(save_path)
-    if gpu:
+    if check_nvidea_gpu_available():
         returned = os.system('ffmpeg -hwaccel auto -c:v h264_cuvid -f concat -safe 0 -i "{}" -c copy -hide_banner -loglevel info "{}"'.format(temp_txt_path, save_path))
     else:
         returned = os.system('ffmpeg -f concat -safe 0 -i "{}" "{}" -c copy -hide_banner -loglevel info'.format(temp_txt_path, save_path))
     while True:
         if returned != 0:
             pass
         else:
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/errors.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,8 +302,13 @@
 
         super().__init__(msg=msg, show_window=show_window)
         self.print_msg(msg=msg)
 
 class FFMPEGCodecGPUError(SimbaError):
     def __init__(self, msg: str, show_window: bool = False):
         super().__init__(msg=msg, show_window=show_window)
-        self.print_msg(msg=f'SIMBA FFMPEG CODEC ERROR: {msg}')
+        self.print_msg(msg=f'SIMBA FFMPEG CODEC ERROR: {msg}')
+
+class FFMPEGNotFoundError(SimbaError):
+    def __init__(self, msg: str, show_window: bool = False):
+        super().__init__(msg=msg, show_window=show_window)
+        self.print_msg(msg=f'SIMBA FFMPEG NOT FOUND ERROR: {msg}')
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/data.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/utils/printing.py` & `Simba-UW-tf-dev-1.64.7/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/st/select_groups_pg.py` & `Simba-UW-tf-dev-1.64.7/simba/st/select_groups_pg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/st/aggregate_statistics.py` & `Simba-UW-tf-dev-1.64.7/simba/st/aggregate_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/st/app.py` & `Simba-UW-tf-dev-1.64.7/simba/st/app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/pose_plotter_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/pose_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.64.7/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.64.7/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.64.7/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.64.7/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.DS_Store`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
-00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
-00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
+00000050: 0000 0001 0000 1000 0061 6c67 3153 636f  .........alg1Sco
+00000060: 6d70 0000 0000 0000 0000 0000 0000 0000  mp..............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
-00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00000130: 0000 0004 7300 0000 000b 005f 005f 0070  ....s......_._.p
-00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-00000150: 6d6f 4444 626c 6f62 0000 0008 41ed 4121  moDDblob....A.A!
-00000160: 1721 c541 0000 000b 005f 005f 0070 0079  .!.A....._._.p.y
-00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000180: 6444 626c 6f62 0000 0008 41ed 4121 1721  dDblob....A.A!.!
-00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-000001b0: 636f 6d70 0000 0000 0005 f000 0000 0000  comp............
+00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0008 0000 0005  ................
+00000210: 002e 0069 0064 0065 0061 6c67 3153 636f  ...i.d.e.alg1Sco
+00000220: 6d70 0000 0000 0000 27fc 0000 0005 002e  mp......'.......
+00000230: 0069 0064 0065 0061 6d6f 4444 626c 6f62  .i.d.e.amoDDblob
+00000240: 0000 0008 993b 4774 e2dd c441 0000 0005  .....;Gt...A....
+00000250: 002e 0069 0064 0065 0061 6d6f 6444 626c  ...i.d.e.amodDbl
+00000260: 6f62 0000 0008 993b 4774 e2dd c441 0000  ob.....;Gt...A..
+00000270: 0005 002e 0069 0064 0065 0061 7068 3153  .....i.d.e.aph1S
+00000280: 636f 6d70 0000 0000 0000 8000 0000 000b  comp............
+00000290: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+000002a0: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+000002b0: 0000 0000 73e1 0000 000b 005f 005f 0070  ....s......_._.p
+000002c0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+000002d0: 6d6f 4444 626c 6f62 0000 0008 b6b0 7cbf  moDDblob......|.
+000002e0: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
+000002f0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000300: 6444 626c 6f62 0000 0008 b6b0 7cbf 1b1f  dDblob......|...
+00000310: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+00000320: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+00000330: 636f 6d70 0000 0000 0000 c000 0000 0000  comp............
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
+00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/mutual_exclusivity_corrector.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/mutual_exclusivity_corrector.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.64.7/simba/model/train_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.64.7/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.64.7/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.64.7/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.64.7/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.64.7/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.64.7/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/ui/define_px_to_mm_ui.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/ui/define_px_to_mm_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/feature_extractors/generic_feature_extractor.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/feature_extractors/generic_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/config_reader.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/config_reader.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-10.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.framewise_euclidean_distance-6.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/pose_importers/anipose_csv_import.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/pose_importers/anipose_csv_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.64.7/simba/three_dimensions/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from PIL import Image, ImageTk
 import multiprocessing
 from typing import List, Union, Optional
 
 from simba.utils.checks import (check_file_exist_and_readable,
                                 check_int,
                                 check_if_filepath_list_is_empty,
-                                check_nvidea_gpu_available)
+                                check_nvidea_gpu_available,
+                                check_ffmpeg_available)
 from simba.utils.read_write import (get_fn_ext,
                                     get_video_meta_data,
                                     find_all_videos_in_directory,
                                     find_core_cnt,
                                     read_config_entry,
                                     read_config_file)
 from simba.utils.printing import stdout_success, SimbaTimer
@@ -33,14 +34,15 @@
 from simba.utils.errors import (NotDirectoryError,
                                 NoFilesFoundError,
                                 FileExistError,
                                 CountError,
                                 InvalidInputError,
                                 DirectoryExistError,
                                 FFMPEGCodecGPUError,
+                                FFMPEGNotFoundError,
                                 InvalidFileTypeError)
 from simba.utils.warnings import (SameInputAndOutputWarning,
                                   FileExistWarning)
 
 
 MAX_FRM_SIZE = 1080, 650
 
@@ -766,51 +768,58 @@
         print('Video {} cropped (Video {}/{})'.format(file_name, str(file_cnt+1), str(len(video_paths))))
     timer.stop_timer()
     stdout_success(msg=f'{str(len(video_paths))} videos cropped and saved in {directory_path} directory', elapsed_time=timer.elapsed_time_str)
 
 def frames_to_movie(directory: Union[str, os.PathLike],
                     fps: int,
                     bitrate: int,
-                    img_format: str) -> None:
+                    img_format: str,
+                    gpu: Optional[bool] = False) -> None:
 
     """
     Merge all image files in a folder to a mp4 video file. Video file is stored in the same directory as the
     input directory sub-folder.
 
     .. note::
        The Image files have to have ordered numerical names e.g., ``1.png``, ``2.png`` etc...
 
     :parameter str directory: Directory containing the images.
     :parameter int fps: The frame rate of the output video.
     :parameter int bitrate: The bitrate of the output video (e.g., 32000).
     :parameter str img_format: The format of the input image files (e.g., ``png``).
+    :parameter Optional[bool] gpu: If True, use NVIDEA GPU codecs. Default False.
 
     :example:
-    >>> _ = crop_multiple_videos(directory_path='project_folder/video_img', fps=15, bitrate=32000, img_format='png')
+    >>> _ = frames_to_movie(directory_path='project_folder/video_img', fps=15, bitrate=32000, img_format='png')
     """
 
-
+    if gpu and not check_nvidea_gpu_available():
+        raise FFMPEGCodecGPUError(msg='NVIDEA GPU not available (as evaluated by nvidea-smi returning None')
     if not os.path.isdir(directory):
         raise NotDirectoryError(msg='SIMBA ERROR: {} is not a valid directory'.format(directory))
     check_int(name='FPS', value=fps)
     check_int(name='BITRATE', value=bitrate)
     file_paths_in_folder = [f for f in glob.glob(directory + '/*') if os.path.isfile(f)]
     img_paths_in_folder = [x for x in file_paths_in_folder if Path(x).suffix[1:] == img_format]
     if len(img_paths_in_folder) < 1:
         raise NoFilesFoundError(msg='SIMBA ERROR: Zero images of file-type {} found in {} directory'.format(img_format, directory))
     img = cv2.imread(img_paths_in_folder[0])
     img_h, img_w = int(img.shape[0]), int(img.shape[1])
     ffmpeg_fn = os.path.join(directory, '%d.{}'.format(img_format))
     save_path = os.path.join(os.path.dirname(directory), os.path.basename(directory) + '.mp4')
-    command = str('ffmpeg -y -r ' + str(fps) + ' -f image2 -s ' + str(img_h) + 'x' + str(img_w) + ' -i ' + '"' + ffmpeg_fn + '"' + ' -vcodec libx264 -b ' + str(bitrate) + 'k ' + '"' + str(save_path) + '"')
+    if gpu:
+        command = f'ffmpeg -y -r {fps} -f image2 -s {img_h}x{img_w} -i "{ffmpeg_fn}" -c:v h264_nvenc -b:v {bitrate}k "{save_path}" -y'
+    else:
+        command = str('ffmpeg -y -r ' + str(fps) + ' -f image2 -s ' + str(img_h) + 'x' + str(img_w) + ' -i ' + '"' + ffmpeg_fn + '"' + ' -vcodec libx264 -b ' + str(bitrate) + 'k ' + '"' + str(save_path) + '"') + ' -y'
     print('Creating {} from {} images...'.format(os.path.basename(save_path), str(len(img_paths_in_folder))))
     subprocess.call(command, shell=True)
     stdout_success(msg=f'Video created at {save_path}')
 
 
+
 def video_concatenator(video_one_path: Union[str, os.PathLike],
                        video_two_path: Union[str, os.PathLike],
                        resolution: Union[int, str],
                        horizontal: bool,
                        gpu: Optional[bool] = False) -> None:
 
     """
@@ -876,25 +885,34 @@
 
 class VideoRotator(ConfigReader):
     """
     GUI Tool for rotating video. Rotated video is saved with the ``_rotated_DATETIME.mp4`` suffix.
 
     :parameter str input_path: Path to video to rotate.
     :parameter str output_dir: Directory where to save the rotated video.
+    :parameter Optional[bool] gpu: If True, use FFMPEG NVIDEA GPU codecs. Else CPU codecs.
+    :parameter Optional[bool] gpu: If True, use FFPMPEG. Else, OpenCV.
 
     :example:
     >>> VideoRotator(input_path='project_folder/videos/Video_1.mp4', output_dir='project_folder/videos')
     """
 
 
     def __init__(self,
                  input_path: Union[str, os.PathLike],
-                 output_dir: Union[str, os.PathLike]) -> None:
+                 output_dir: Union[str, os.PathLike],
+                 gpu: Optional[bool] = False,
+                 ffmpeg: Optional[bool] = False) -> None:
 
-        _, self.cpu_cnt  = find_core_cnt()
+        if gpu and not check_nvidea_gpu_available():
+            raise FFMPEGCodecGPUError(msg='No GPU found (as evaluated by nvidea-smi returning None)')
+        if ffmpeg and not check_ffmpeg_available():
+            raise FFMPEGNotFoundError(msg='FFMPEG not found on the computer (as evaluated by "ffmpeg" returning None)')
+        _, self.cpu_cnt = find_core_cnt()
+        self.gpu, self.ffmpeg = gpu, ffmpeg
         self.save_dir = output_dir
         self.datetime = datetime.now().strftime('%Y%m%d%H%M%S')
         if os.path.isfile(input_path):
             self.video_paths = [input_path]
         else:
             self.video_paths = find_all_videos_in_directory(directory=input_path, as_dict=True).values()
             check_if_filepath_list_is_empty(filepaths=self.video_paths, error_msg=f'No videos found in {input_path} directory')
@@ -912,35 +930,43 @@
         rotation_matrix = cv2.getRotationMatrix2D((self.video_meta_data['width'] / 2, self.video_meta_data['height'] / 2), self.dif_angle, 1)
         img = cv2.warpAffine(img, rotation_matrix, (self.video_meta_data['width'], self.video_meta_data['height']))
         self.__insert_img(img=img)
 
     def __run_rotation(self):
         self.main_frm.destroy()
         start = time.time()
-        for video_cnt, (video_path, rotation) in enumerate(self.results.items()):
-            cap = cv2.VideoCapture(video_path)
-            _, name, _ = get_fn_ext(filepath=video_path)
-            rotation_matrix = cv2.getRotationMatrix2D((self.video_meta_data['width'] / 2, self.video_meta_data['height'] / 2), rotation, 1)
-            save_path = os.path.join(self.save_dir, f'{name}_rotated_{self.datetime}.mp4')
-            video_meta = get_video_meta_data(video_path=video_path)
-            fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
-            writer = cv2.VideoWriter(save_path, fourcc, video_meta['fps'],(video_meta['width'], video_meta['height']))
-            img_cnt = 0
-            while True:
-                ret, img = cap.read()
-                if not ret:
-                    break
-                img = cv2.warpAffine(img, rotation_matrix,
-                                     (self.video_meta_data['width'], self.video_meta_data['height']))
-                writer.write(img)
-                img_cnt += 1
-                print(
-                    f'Rotating frame {img_cnt}/{video_meta["frame_count"]} (Video {video_cnt + 1}/{len(self.results.keys())}) ')
-            cap.release()
-            writer.release()
+        if self.ffmpeg or self.gpu:
+            for video_cnt, (video_path, rotation) in enumerate(self.results.items()):
+                _, name, _ = get_fn_ext(filepath=video_path)
+                save_path = os.path.join(self.save_dir, f'{name}_rotated_{self.datetime}.mp4')
+                if self.gpu:
+                    cmd = f'ffmpeg -hwaccel auto -i {video_path} -vf "hwupload_cuda,rotate={rotation}*(PI/180),format=nv12|cuda" -c:v h264_nvenc {save_path} -y'
+                else:
+                    cmd = f'ffmpeg -i {video_path} -vf "rotate={rotation}*(PI/180)" {save_path} -y'
+                subprocess.call(cmd, shell=True, stdout=subprocess.PIPE)
+        else:
+            for video_cnt, (video_path, rotation) in enumerate(self.results.items()):
+                cap = cv2.VideoCapture(video_path)
+                _, name, _ = get_fn_ext(filepath=video_path)
+                rotation_matrix = cv2.getRotationMatrix2D((self.video_meta_data['width'] / 2, self.video_meta_data['height'] / 2), rotation, 1)
+                save_path = os.path.join(self.save_dir, f'{name}_rotated_{self.datetime}.mp4')
+                video_meta = get_video_meta_data(video_path=video_path)
+                fourcc = cv2.VideoWriter_fourcc(*Formats.MP4_CODEC.value)
+                writer = cv2.VideoWriter(save_path, fourcc, video_meta['fps'],(video_meta['width'], video_meta['height']))
+                img_cnt = 0
+                while True:
+                    ret, img = cap.read()
+                    if not ret:
+                        break
+                    img = cv2.warpAffine(img, rotation_matrix, (self.video_meta_data['width'], self.video_meta_data['height']))
+                    writer.write(img)
+                    img_cnt += 1
+                    print(f'Rotating frame {img_cnt}/{video_meta["frame_count"]} (Video {video_cnt + 1}/{len(self.results.keys())}) ')
+                cap.release()
+                writer.release()
         stdout_success(msg=f'All videos rotated and saved in {self.save_dir}', elapsed_time=str(round((time.time() - start), 2)))
 
     def __save(self):
         process = None
         self.results[self.file_path] = self.dif_angle
         if len(self.results.keys()) == len(self.video_paths):
             process = multiprocessing.Process(target=self.__run_rotation())
@@ -1048,15 +1074,16 @@
     print(f'Importing image files for {input_basename}...')
     shutil.copytree(source, destination)
     timer.stop_timer()
     stdout_success(msg=f'{destination} imported to SimBA project', elapsed_time=timer.elapsed_time_str)
 
 
 # r = VideoRotator(input_path=r'/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Testing/Together_1_downsampled.mp4',
-#              output_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Blah')
+#              output_dir='/Users/simon/Desktop/envs/troubleshooting/two_black_animals_14bp/project_folder/videos/Blah',
+#              gpu=True)
 # r.run()
 
 
 # video_concatenator(video_one_path='/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT_2.mp4',
 #                    video_two_path= '/Users/simon/Desktop/troubleshooting/Open_field_5/project_folder/frames/output/gantt_plots/SI_DAY3_308_CD1_PRESENT.mp4',
 #                    resolution='Video 1',
 #                    horizontal=False)
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 000010b0: 5f10 197b 7b31 3036 322c 2033 3733 7d2c  _..{{1062, 373},
 000010c0: 207b 3737 302c 2034 3336 7d7d 0908 1725   {770, 436}}...%
 000010d0: 313d 4960 6d79 7a7b 7c7d 7e9a 0000 0000  1=I`myz{|}~.....
 000010e0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
 000010f0: 0000 0000 0000 0000 0000 009b 0000 000b  ................
 00001100: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
 00001110: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-00001120: 0000 0002 9e74 0000 000b 005f 005f 0070  .....t....._._.p
+00001120: 0000 0003 fc58 0000 000b 005f 005f 0070  .....X....._._.p
 00001130: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
 00001140: 6c73 7643 626c 6f62 0000 02d4 6270 6c69  lsvCblob....bpli
 00001150: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
 00001160: 0c0d 1d4a 4b4c 4d0c 4f5f 1012 7669 6577  ...JKLM.O_..view
 00001170: 4f70 7469 6f6e 7356 6572 7369 6f6e 5f10  OptionsVersion_.
 00001180: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
 00001190: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
@@ -362,21 +362,21 @@
 00001690: 8001 8201 8b01 8c01 8d01 8f01 9101 9a01  ................
 000016a0: 9b01 9c01 9e01 a001 a901 aa01 ab01 ad01  ................
 000016b0: b601 b701 b801 b901 c201 cb01 d401 d901  ................
 000016c0: da00 0000 0000 0002 0100 0000 0000 0000  ................
 000016d0: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
 000016e0: e300 0000 0b00 5f00 5f00 7000 7900 6300  ......_._.p.y.c.
 000016f0: 6100 6300 6800 6500 5f00 5f6d 6f44 4462  a.c.h.e._._moDDb
-00001700: 6c6f 6200 0000 083b d4ec c21b 1fc5 4100  lob....;......A.
+00001700: 6c6f 6200 0000 08bb fb97 20f3 2ac5 4100  lob....... .*.A.
 00001710: 0000 0b00 5f00 5f00 7000 7900 6300 6100  ...._._.p.y.c.a.
 00001720: 6300 6800 6500 5f00 5f6d 6f64 4462 6c6f  c.h.e._._modDblo
-00001730: 6200 0000 083b d4ec c21b 1fc5 4100 0000  b....;......A...
+00001730: 6200 0000 08bb fb97 20f3 2ac5 4100 0000  b....... .*.A...
 00001740: 0b00 5f00 5f00 7000 7900 6300 6100 6300  .._._.p.y.c.a.c.
 00001750: 6800 6500 5f00 5f70 6831 5363 6f6d 7000  h.e._._ph1Scomp.
-00001760: 0000 0000 0350 0000 0000 0b00 5f00 5f00  .....P......_._.
+00001760: 0000 0000 04f0 0000 0000 0b00 5f00 5f00  ............_._.
 00001770: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
 00001780: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
 00001790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000017d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -490,21 +490,21 @@
 00001e90: 8001 8201 8b01 8c01 8d01 8f01 9101 9a01  ................
 00001ea0: 9b01 9c01 9e01 a001 a901 aa01 ab01 ad01  ................
 00001eb0: b601 b701 b801 b901 c201 cb01 d401 d901  ................
 00001ec0: da00 0000 0000 0002 0100 0000 0000 0000  ................
 00001ed0: 4c00 0000 0000 0000 0000 0000 0000 0001  L...............
 00001ee0: e300 0000 0b00 5f00 5f00 7000 7900 6300  ......_._.p.y.c.
 00001ef0: 6100 6300 6800 6500 5f00 5f6d 6f44 4462  a.c.h.e._._moDDb
-00001f00: 6c6f 6200 0000 083b d4ec c21b 1fc5 4100  lob....;......A.
+00001f00: 6c6f 6200 0000 08bb fb97 20f3 2ac5 4100  lob....... .*.A.
 00001f10: 0000 0b00 5f00 5f00 7000 7900 6300 6100  ...._._.p.y.c.a.
 00001f20: 6300 6800 6500 5f00 5f6d 6f64 4462 6c6f  c.h.e._._modDblo
-00001f30: 6200 0000 083b d4ec c21b 1fc5 4100 0000  b....;......A...
+00001f30: 6200 0000 08bb fb97 20f3 2ac5 4100 0000  b....... .*.A...
 00001f40: 0b00 5f00 5f00 7000 7900 6300 6100 6300  .._._.p.y.c.a.c.
 00001f50: 6800 6500 5f00 5f70 6831 5363 6f6d 7000  h.e._._ph1Scomp.
-00001f60: 0000 0000 0350 0000 0000 0b00 5f00 5f00  .....P......_._.
+00001f60: 0000 0000 04f0 0000 0000 0b00 5f00 5f00  ............_._.
 00001f70: 7000 7900 6300 6100 6300 6800 6500 5f00  p.y.c.a.c.h.e._.
 00001f80: 5f76 5372 6e6c 6f6e 6700 0000 0100 0000  _vSrnlong.......
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/video_processing_new.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/video_processing_new.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.64.7/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/mixins/.DS_Store`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0108 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
-00000050: 0000 0001 0000 1000 0061 6c67 3153 636f  .........alg1Sco
-00000060: 6d70 0000 0000 0000 0000 0000 0000 0000  mp..............
+00000040: 0000 0000 0000 0002 0000 0000 0000 0004  ................
+00000050: 0000 0001 0000 1000 0063 0061 0063 0068  .........c.a.c.h
+00000060: 0065 005f 0000 0000 0000 0000 0000 0000  .e._............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000100: 0000 0000 0000 0000 0000 0004 0000 000b  ................
+00000110: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
+00000120: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
+00000130: 0000 000b f7a8 0000 000b 005f 005f 0070  ..........._._.p
+00000140: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
+00000150: 6d6f 4444 626c 6f62 0000 0008 1584 a98c  moDDblob........
+00000160: 892b c541 0000 000b 005f 005f 0070 0079  .+.A....._._.p.y
+00000170: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
+00000180: 6444 626c 6f62 0000 0008 1584 a98c 892b  dDblob.........+
+00000190: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
+000001a0: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
+000001b0: 636f 6d70 0000 0000 000d 0000 0000 0000  comp............
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0008 0000 0005  ................
-00000210: 002e 0069 0064 0065 0061 6c67 3153 636f  ...i.d.e.alg1Sco
-00000220: 6d70 0000 0000 0000 27fc 0000 0005 002e  mp......'.......
-00000230: 0069 0064 0065 0061 6d6f 4444 626c 6f62  .i.d.e.amoDDblob
-00000240: 0000 0008 993b 4774 e2dd c441 0000 0005  .....;Gt...A....
-00000250: 002e 0069 0064 0065 0061 6d6f 6444 626c  ...i.d.e.amodDbl
-00000260: 6f62 0000 0008 993b 4774 e2dd c441 0000  ob.....;Gt...A..
-00000270: 0005 002e 0069 0064 0065 0061 7068 3153  .....i.d.e.aph1S
-00000280: 636f 6d70 0000 0000 0000 8000 0000 000b  comp............
-00000290: 005f 005f 0070 0079 0063 0061 0063 0068  ._._.p.y.c.a.c.h
-000002a0: 0065 005f 005f 6c67 3153 636f 6d70 0000  .e._._lg1Scomp..
-000002b0: 0000 0000 73e1 0000 000b 005f 005f 0070  ....s......_._.p
-000002c0: 0079 0063 0061 0063 0068 0065 005f 005f  .y.c.a.c.h.e._._
-000002d0: 6d6f 4444 626c 6f62 0000 0008 b6b0 7cbf  moDDblob......|.
-000002e0: 1b1f c541 0000 000b 005f 005f 0070 0079  ...A....._._.p.y
-000002f0: 0063 0061 0063 0068 0065 005f 005f 6d6f  .c.a.c.h.e._._mo
-00000300: 6444 626c 6f62 0000 0008 b6b0 7cbf 1b1f  dDblob......|...
-00000310: c541 0000 000b 005f 005f 0070 0079 0063  .A....._._.p.y.c
-00000320: 0061 0063 0068 0065 005f 005f 7068 3153  .a.c.h.e._._ph1S
-00000330: 636f 6d70 0000 0000 0000 c000 0000 0000  comp............
+00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0108 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001440: 0100 0000 8000 0000 0000 0000 0100 0002  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.64.7/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/SimBA.py` & `Simba-UW-tf-dev-1.64.7/simba/SimBA.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from simba.model.grid_search_rf import GridSearchRandomForestClassifier
 from simba.model.inference_validation import InferenceValidation
 from simba.model.inference_batch import InferenceBatch
 import urllib.request
 import threading
 import atexit
 from simba.ui.video_info_ui import VideoInfoTable
-from simba.utils.checks import check_file_exist_and_readable, check_int
+from simba.utils.checks import check_file_exist_and_readable, check_int, check_ffmpeg_available
 from simba.roi_tools.ROI_define import *
 from simba.roi_tools.ROI_menus import *
 from simba.roi_tools.ROI_reset import *
 from simba.utils.read_write import get_video_meta_data
 from simba.utils.data import run_user_defined_feature_extraction_class
 from simba.utils.printing import stdout_success, stdout_warning
 
@@ -116,15 +116,15 @@
 from simba.bounding_box_tools.boundary_menus import BoundaryMenus
 from simba.labelling.labelling_interface import select_labelling_video
 from simba.labelling.labelling_advanced_interface import select_labelling_video_advanced
 from simba.utils.enums import (Formats,
                                OS,
                                Defaults,
                                TagNames)
-from simba.utils.warnings import PythonVersionWarning
+from simba.utils.warnings import PythonVersionWarning, FFMpegNotFoundWarning
 from simba.utils.errors import InvalidInputError
 from simba.utils.lookups import get_bp_config_code_class_pairs, get_icons_paths
 from simba.mixins.pop_up_mixin import PopUpMixin
 from simba.ui.create_project_ui import ProjectCreatorPopUp
 from simba.utils.lookups import get_emojis
 import sys
 import subprocess
@@ -682,21 +682,22 @@
 
     def run_feature_extraction(self):
         print(f'Pose-estimation body part setting for feature extraction: {str(self.animal_cnt)} animals {str(self.pose_setting)} body-parts')
         feature_extractor_classes = get_bp_config_code_class_pairs()
         if self.user_defined_var.get():
             _ = run_user_defined_feature_extraction_class(file_path=self.scriptfile.file_path,
                                                           config_path=self.config_path)
-        if self.pose_setting not in feature_extractor_classes.keys():
-            raise InvalidInputError(msg=f'The project pose-configuration key is set to {self.pose_setting} which is invalid. OPTIONS: {list(feature_extractor_classes.keys())}')
-        if self.pose_setting == '8':
-            feature_extractor = feature_extractor_classes[self.pose_setting][self.animal_cnt](config_path=self.config_path)
         else:
-            feature_extractor = feature_extractor_classes[self.pose_setting](config_path=self.config_path)
-        feature_extractor.run()
+            if self.pose_setting not in feature_extractor_classes.keys():
+                raise InvalidInputError(msg=f'The project pose-configuration key is set to {self.pose_setting} which is invalid. OPTIONS: {list(feature_extractor_classes.keys())}')
+            if self.pose_setting == '8':
+                feature_extractor = feature_extractor_classes[self.pose_setting][self.animal_cnt](config_path=self.config_path)
+            else:
+                feature_extractor = feature_extractor_classes[self.pose_setting](config_path=self.config_path)
+            feature_extractor.run()
 
     def set_distance_mm(self):
         check_int(name='DISTANCE IN MILLIMETER', value=self.distance_in_mm_eb.entry_get, min_value=1)
         self.config.set('Frame settings', 'distance_mm', self.distance_in_mm_eb.entry_get)
         with open(self.config_path, 'w') as f:
             self.config.write(f)
 
@@ -841,14 +842,17 @@
         clear_txt_btn = Button(self.frame, text=' CLEAR', compound=LEFT, image=self.menu_icons['clean']['img'], font=Formats.LABELFRAME_HEADER_FORMAT.value, command=lambda: self.clean_txt())
         clear_txt_btn.pack(side=BOTTOM, fill=X)
         sys.stdout = StdRedirector(self.txt)
 
         if OS.PYTHON_VER.value != '3.6':
             PythonVersionWarning(msg=f'SimBA is not extensively tested beyond python 3.6. You are using python {OS.PYTHON_VER.value}. If you encounter errors in python>3.6, please report them on GitHub or Gitter and we will fix! (links in the help toolbar)')
 
+        if not check_ffmpeg_available():
+            FFMpegNotFoundWarning(msg='SimBA could not find a FFMPEG installation on computer (as evaluated by "ffmpeg" returning None). SimBA works best with FFMPEG and it is recommended to install it on your computer')
+
     def restart(self):
         confirm_restart = askyesno(title='RESTART', message='Are you sure that you want restart SimBA?')
         if confirm_restart:
             self.root.destroy()
             os.execl(sys.executable, sys.executable, *sys.argv)
 
     def clean_txt(self):
```

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.64.7/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.64.7/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.64.7/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.64.7/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.64.7/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.64.7/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.64.7/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.64.7/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.64.7/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.64.7/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.64.6
+Version: 1.64.7
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
 simba/feature_extractors/misc/graph_3d_plotter.py
 simba/feature_extractors/misc/graph_creator.py
 simba/feature_extractors/misc/make_splash.py
 simba/feature_extractors/misc/mutual_exclusive.py
 simba/feature_extractors/misc/peaks.py
 simba/feature_extractors/misc/read_files_mp_2.py
 simba/feature_extractors/misc/read_in_mp.py
+simba/feature_extractors/misc/shap_gpu.py
 simba/feature_extractors/misc/shap_log_mp.py
 simba/feature_extractors/misc/shap_log_mp_2.py
 simba/feature_extractors/misc/termite_rois.csv
 simba/feature_extractors/misc/time_stamp_calculator.py
 simba/feature_extractors/misc/video_color.py
 simba/feature_extractors/misc/video_rotator.py
 simba/feature_extractors/misc/video_rotator_mp.py
```

### Comparing `Simba-UW-tf-dev-1.64.6/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.64.7/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/LICENSE.md` & `Simba-UW-tf-dev-1.64.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.64.7/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.64.7/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_train_model_mixin.py` & `Simba-UW-tf-dev-1.64.7/tests/test_train_model_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_pose_importers.py` & `Simba-UW-tf-dev-1.64.7/tests/test_pose_importers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.64.7/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_utils_data.py` & `Simba-UW-tf-dev-1.64.7/tests/test_utils_data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_config_reader_mixin.py` & `Simba-UW-tf-dev-1.64.7/tests/test_config_reader_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.64.7/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.64.7/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.64.7/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_video_processors.py` & `Simba-UW-tf-dev-1.64.7/tests/test_video_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.64.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.64.7/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.64.7/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/tests/test_roi_tools.py` & `Simba-UW-tf-dev-1.64.7/tests/test_roi_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/README.md` & `Simba-UW-tf-dev-1.64.7/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.64.6/setup.py` & `Simba-UW-tf-dev-1.64.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.64.6",
+    version="1.64.7",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

