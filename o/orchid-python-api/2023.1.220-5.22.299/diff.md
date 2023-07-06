# Comparing `tmp/orchid_python_api-2023.1.220.tar.gz` & `tmp/orchid_python_api-5.22.299.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orchid_python_api-2023.1.220.tar", max compression
+gzip compressed data, was "orchid_python_api-5.22.299.tar", max compression
```

## Comparing `orchid_python_api-2023.1.220.tar` & `orchid_python_api-5.22.299.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     3386 2023-04-12 16:21:02.740314 orchid_python_api-2023.1.220/copy_orchid_examples.py
--rw-r--r--   0        0        0     3604 2023-04-12 16:21:02.163735 orchid_python_api-2023.1.220/copy_orchid_low_level_examples.py
--rw-r--r--   0        0        0     3586 2023-04-12 16:21:02.705105 orchid_python_api-2023.1.220/copy_orchid_manual_examples.py
--rw-r--r--   0        0        0     3410 2023-04-12 16:21:02.938782 orchid_python_api-2023.1.220/copy_orchid_tutorials.py
--rw-r--r--   0        0        0    10316 2023-03-30 13:38:52.087989 orchid_python_api-2023.1.220/LICENSE
--rw-r--r--   0        0        0     1554 2023-04-12 16:21:02.762215 orchid_python_api-2023.1.220/orchid/__init__.py
--rw-r--r--   0        0        0      723 2023-04-12 16:21:02.525319 orchid_python_api-2023.1.220/orchid/__version__.py
--rw-r--r--   0        0        0     1081 2023-04-12 16:21:02.775215 orchid_python_api-2023.1.220/orchid/base.py
--rw-r--r--   0        0        0     3772 2023-04-12 16:21:02.808333 orchid_python_api-2023.1.220/orchid/base_time_series_adapter.py
--rw-r--r--   0        0        0     6810 2023-04-12 16:21:02.884794 orchid_python_api-2023.1.220/orchid/configuration.py
--rw-r--r--   0        0        0     1831 2023-04-12 16:21:02.159565 orchid_python_api-2023.1.220/orchid/convert.py
--rw-r--r--   0        0        0     6529 2023-04-12 16:21:02.520319 orchid_python_api-2023.1.220/orchid/core.py
--rw-r--r--   0        0        0     1186 2023-04-12 16:21:02.639055 orchid_python_api-2023.1.220/orchid/dom_project_object.py
--rw-r--r--   0        0        0     2369 2023-04-12 16:21:02.996811 orchid_python_api-2023.1.220/orchid/dot_net.py
--rw-r--r--   0        0        0     2161 2023-04-12 16:21:02.579975 orchid_python_api-2023.1.220/orchid/dot_net_disposable.py
--rw-r--r--   0        0        0    10281 2023-04-12 16:21:02.874802 orchid_python_api-2023.1.220/orchid/dot_net_dom_access.py
--rw-r--r--   0        0        0     1421 2023-04-12 16:21:02.558847 orchid_python_api-2023.1.220/orchid/measurement.py
--rw-r--r--   0        0        0     8428 2023-04-12 16:21:02.917374 orchid_python_api-2023.1.220/orchid/native_data_frame_adapter.py
--rw-r--r--   0        0        0     2806 2023-04-12 16:21:02.878801 orchid_python_api-2023.1.220/orchid/native_monitor_adapter.py
--rw-r--r--   0        0        0     6212 2023-04-12 16:21:02.644044 orchid_python_api-2023.1.220/orchid/native_project_user_data_adapter.py
--rw-r--r--   0        0        0    30513 2023-04-12 16:21:02.514320 orchid_python_api-2023.1.220/orchid/native_stage_adapter.py
--rw-r--r--   0        0        0     2086 2023-04-12 16:21:02.135049 orchid_python_api-2023.1.220/orchid/native_stage_part_adapter.py
--rw-r--r--   0        0        0     2628 2023-04-12 16:21:02.589125 orchid_python_api-2023.1.220/orchid/native_subsurface_point.py
--rw-r--r--   0        0        0     2090 2023-04-12 16:21:02.288818 orchid_python_api-2023.1.220/orchid/native_time_series_adapter.py
--rw-r--r--   0        0        0    10605 2023-04-12 16:21:02.144562 orchid_python_api-2023.1.220/orchid/native_trajectory_adapter.py
--rw-r--r--   0        0        0     7470 2023-04-12 16:21:02.766214 orchid_python_api-2023.1.220/orchid/native_treatment_calculations.py
--rw-r--r--   0        0        0     2518 2023-04-12 16:21:02.621140 orchid_python_api-2023.1.220/orchid/native_treatment_curve_adapter.py
--rw-r--r--   0        0        0     5426 2023-04-12 16:21:02.233299 orchid_python_api-2023.1.220/orchid/native_well_adapter.py
--rw-r--r--   0        0        0    10800 2023-04-12 16:21:02.263815 orchid_python_api-2023.1.220/orchid/net_date_time.py
--rw-r--r--   0        0        0     2273 2023-04-12 16:23:05.743109 orchid_python_api-2023.1.220/orchid/net_enumerable.py
--rw-r--r--   0        0        0     2126 2023-04-12 16:21:02.730340 orchid_python_api-2023.1.220/orchid/net_fracture_diagnostics_factory.py
--rw-r--r--   0        0        0    27133 2023-04-12 16:21:02.701113 orchid_python_api-2023.1.220/orchid/net_quantity.py
--rw-r--r--   0        0        0     2433 2023-04-12 16:21:02.574966 orchid_python_api-2023.1.220/orchid/net_stage_qc.py
--rw-r--r--   0        0        0     1181 2023-04-12 16:21:03.150866 orchid_python_api-2023.1.220/orchid/physical_quantity.py
--rw-r--r--   0        0        0     7051 2023-04-12 16:21:03.136869 orchid_python_api-2023.1.220/orchid/project.py
--rw-r--r--   0        0        0    12480 2023-04-12 16:21:02.606576 orchid_python_api-2023.1.220/orchid/project_store.py
--rw-r--r--   0        0        0     1452 2023-04-12 16:21:02.969782 orchid_python_api-2023.1.220/orchid/reference_origins.py
--rw-r--r--   0        0        0     2919 2023-04-12 16:21:02.227787 orchid_python_api-2023.1.220/orchid/script_adapter_context.py
--rw-r--r--   0        0        0     1753 2023-04-12 16:21:02.648060 orchid_python_api-2023.1.220/orchid/searchable_data_frames.py
--rw-r--r--   0        0        0     7555 2023-04-12 16:21:02.617147 orchid_python_api-2023.1.220/orchid/searchable_project_objects.py
--rw-r--r--   0        0        0     2627 2023-04-12 16:21:03.200893 orchid_python_api-2023.1.220/orchid/searchable_stage_parts.py
--rw-r--r--   0        0        0     1226 2023-04-12 16:21:03.001811 orchid_python_api-2023.1.220/orchid/searchable_stages.py
--rw-r--r--   0        0        0     6549 2023-04-12 16:21:02.173759 orchid_python_api-2023.1.220/orchid/unit_system.py
--rw-r--r--   0        0        0     1791 2023-04-12 16:21:02.744321 orchid_python_api-2023.1.220/orchid/validation.py
--rw-r--r--   0        0        0       10 2023-04-12 15:24:07.549281 orchid_python_api-2023.1.220/orchid/VERSION
--rw-r--r--   0        0        0     1098 2023-04-12 16:21:02.353665 orchid_python_api-2023.1.220/orchid/version.py
--rw-r--r--   0        0        0      844 2023-04-12 16:23:05.766656 orchid_python_api-2023.1.220/orchid_python_api/__init__.py
--rw-r--r--   0        0        0     6474 2023-04-12 16:23:06.160412 orchid_python_api-2023.1.220/orchid_python_api/examples/add_stages.py
--rw-r--r--   0        0        0     4400 2023-04-12 16:23:05.788673 orchid_python_api-2023.1.220/orchid_python_api/examples/change_stage_times.py
--rw-r--r--   0        0        0    28071 2023-04-12 16:23:05.754130 orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.ipynb
--rw-r--r--   0        0        0    17039 2023-04-12 16:23:05.682626 orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.py
--rw-r--r--   0        0        0    11549 2023-04-12 16:23:05.703016 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/add_stages_low.py
--rw-r--r--   0        0        0    23608 2023-04-12 16:23:05.794663 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.ipynb
--rw-r--r--   0        0        0    15686 2023-04-12 16:23:05.873178 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.py
--rw-r--r--   0        0        0    18318 2023-04-12 16:23:06.100791 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py
--rw-r--r--   0        0        0    15900 2023-04-12 16:23:06.131875 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_iterate_example.py
--rw-r--r--   0        0        0     2446 2023-04-12 16:23:05.777657 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/monitor_time_series.py
--rw-r--r--   0        0        0    10418 2023-04-12 16:23:05.841635 orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/multi_picking_events.py
--rw-r--r--   0        0        0    21648 2023-04-12 16:23:05.782679 orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.ipynb
--rw-r--r--   0        0        0     1373 2023-04-12 16:23:05.771655 orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.py
--rw-r--r--   0        0        0     8260 2023-04-12 16:23:06.066223 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.ipynb
--rw-r--r--   0        0        0     4425 2023-04-12 16:23:05.738098 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.py
--rw-r--r--   0        0        0     7006 2023-04-12 16:23:05.720577 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.ipynb
--rw-r--r--   0        0        0     3121 2023-04-12 16:23:05.708014 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.py
--rw-r--r--   0        0        0     7256 2023-04-12 16:23:05.820223 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.ipynb
--rw-r--r--   0        0        0     3822 2023-04-12 16:23:05.696948 orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.py
--rw-r--r--   0        0        0      561 2023-03-30 13:38:52.090988 orchid_python_api-2023.1.220/orchid_python_api/examples/python_api.yaml.example
--rw-r--r--   0        0        0    30806 2023-03-30 13:38:52.096506 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.ipynb
--rw-r--r--   0        0        0    18688 2023-04-12 16:23:06.218598 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.py
--rw-r--r--   0        0        0    19458 2023-03-30 13:38:52.096506 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.ipynb
--rw-r--r--   0        0        0    14287 2023-04-12 16:23:06.073222 orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.py
--rw-r--r--   0        0        0    13245 2023-04-12 16:23:05.944772 orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.ipynb
--rw-r--r--   0        0        0     5985 2023-04-12 16:23:06.153395 orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.py
--rw-r--r--   0        0        0     8613 2023-04-12 16:23:05.965303 orchid_python_api-2023.1.220/orchid_python_api/examples/stage_qc_results.py
--rw-r--r--   0        0        0    12887 2023-04-12 16:23:05.879194 orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.ipynb
--rw-r--r--   0        0        0     8570 2023-04-12 16:23:06.247103 orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.py
--rw-r--r--   0        0        0    24090 2023-04-12 16:23:05.934768 orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb
--rw-r--r--   0        0        0    19171 2023-04-12 16:23:05.761122 orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.py
--rw-r--r--   0        0        0     3721 2023-04-12 15:26:48.304536 orchid_python_api-2023.1.220/pyproject.toml
--rw-r--r--   0        0        0    32857 2023-03-30 13:38:52.098505 orchid_python_api-2023.1.220/README.md
--rw-r--r--   0        0        0    19722 2023-04-12 15:13:05.860437 orchid_python_api-2023.1.220/ReleaseNotes.md
--rw-r--r--   0        0        0    34602 1970-01-01 00:00:00.000000 orchid_python_api-2023.1.220/PKG-INFO
+-rw-r--r--   0        0        0     3386 2023-04-14 14:44:26.959541 orchid_python_api-5.22.299/copy_orchid_examples.py
+-rw-r--r--   0        0        0     3604 2023-04-14 14:44:26.960552 orchid_python_api-5.22.299/copy_orchid_low_level_examples.py
+-rw-r--r--   0        0        0     3586 2023-04-14 14:44:26.960552 orchid_python_api-5.22.299/copy_orchid_manual_examples.py
+-rw-r--r--   0        0        0     3410 2023-04-14 14:44:26.960552 orchid_python_api-5.22.299/copy_orchid_tutorials.py
+-rw-r--r--   0        0        0    10316 2023-03-30 13:38:52.087989 orchid_python_api-5.22.299/LICENSE
+-rw-r--r--   0        0        0     1554 2023-04-14 14:44:26.973257 orchid_python_api-5.22.299/orchid/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-14 14:44:26.973257 orchid_python_api-5.22.299/orchid/__version__.py
+-rw-r--r--   0        0        0     1081 2023-04-14 14:44:26.973257 orchid_python_api-5.22.299/orchid/base.py
+-rw-r--r--   0        0        0     3772 2023-04-14 14:44:26.974257 orchid_python_api-5.22.299/orchid/base_time_series_adapter.py
+-rw-r--r--   0        0        0     6810 2023-04-14 14:44:26.974257 orchid_python_api-5.22.299/orchid/configuration.py
+-rw-r--r--   0        0        0     1831 2023-04-14 14:44:26.974257 orchid_python_api-5.22.299/orchid/convert.py
+-rw-r--r--   0        0        0     6529 2023-04-14 14:44:26.975257 orchid_python_api-5.22.299/orchid/core.py
+-rw-r--r--   0        0        0     1186 2023-04-14 14:44:26.975257 orchid_python_api-5.22.299/orchid/dom_project_object.py
+-rw-r--r--   0        0        0     2369 2023-04-14 14:44:26.975257 orchid_python_api-5.22.299/orchid/dot_net.py
+-rw-r--r--   0        0        0     2161 2023-04-14 14:44:26.975257 orchid_python_api-5.22.299/orchid/dot_net_disposable.py
+-rw-r--r--   0        0        0    10281 2023-04-14 14:44:26.976259 orchid_python_api-5.22.299/orchid/dot_net_dom_access.py
+-rw-r--r--   0        0        0     1421 2023-04-14 14:44:26.976259 orchid_python_api-5.22.299/orchid/measurement.py
+-rw-r--r--   0        0        0     8428 2023-04-14 14:44:26.976259 orchid_python_api-5.22.299/orchid/native_data_frame_adapter.py
+-rw-r--r--   0        0        0     2806 2023-04-14 14:44:26.977259 orchid_python_api-5.22.299/orchid/native_monitor_adapter.py
+-rw-r--r--   0        0        0     6212 2023-04-14 14:44:26.977259 orchid_python_api-5.22.299/orchid/native_project_user_data_adapter.py
+-rw-r--r--   0        0        0    30513 2023-04-14 14:44:26.978292 orchid_python_api-5.22.299/orchid/native_stage_adapter.py
+-rw-r--r--   0        0        0     2086 2023-04-14 14:44:26.978292 orchid_python_api-5.22.299/orchid/native_stage_part_adapter.py
+-rw-r--r--   0        0        0     2628 2023-04-14 14:44:26.978292 orchid_python_api-5.22.299/orchid/native_subsurface_point.py
+-rw-r--r--   0        0        0     2090 2023-04-14 14:44:26.979300 orchid_python_api-5.22.299/orchid/native_time_series_adapter.py
+-rw-r--r--   0        0        0    10605 2023-04-14 14:44:26.979300 orchid_python_api-5.22.299/orchid/native_trajectory_adapter.py
+-rw-r--r--   0        0        0     7470 2023-04-14 14:44:26.979300 orchid_python_api-5.22.299/orchid/native_treatment_calculations.py
+-rw-r--r--   0        0        0     2518 2023-04-14 14:44:26.980306 orchid_python_api-5.22.299/orchid/native_treatment_curve_adapter.py
+-rw-r--r--   0        0        0     5426 2023-04-14 14:44:26.980306 orchid_python_api-5.22.299/orchid/native_well_adapter.py
+-rw-r--r--   0        0        0    10800 2023-04-14 14:44:26.980306 orchid_python_api-5.22.299/orchid/net_date_time.py
+-rw-r--r--   0        0        0     2273 2023-04-14 14:44:26.981308 orchid_python_api-5.22.299/orchid/net_enumerable.py
+-rw-r--r--   0        0        0     2126 2023-04-14 14:44:26.981308 orchid_python_api-5.22.299/orchid/net_fracture_diagnostics_factory.py
+-rw-r--r--   0        0        0    27133 2023-04-14 14:44:26.981308 orchid_python_api-5.22.299/orchid/net_quantity.py
+-rw-r--r--   0        0        0     2433 2023-04-14 14:44:26.982307 orchid_python_api-5.22.299/orchid/net_stage_qc.py
+-rw-r--r--   0        0        0     1181 2023-04-14 14:44:26.982307 orchid_python_api-5.22.299/orchid/physical_quantity.py
+-rw-r--r--   0        0        0     7051 2023-04-14 14:44:26.982307 orchid_python_api-5.22.299/orchid/project.py
+-rw-r--r--   0        0        0    12480 2023-04-14 14:44:26.983308 orchid_python_api-5.22.299/orchid/project_store.py
+-rw-r--r--   0        0        0     1452 2023-04-14 14:44:26.983308 orchid_python_api-5.22.299/orchid/reference_origins.py
+-rw-r--r--   0        0        0     2919 2023-04-14 14:44:26.983308 orchid_python_api-5.22.299/orchid/script_adapter_context.py
+-rw-r--r--   0        0        0     1753 2023-04-14 14:44:26.983308 orchid_python_api-5.22.299/orchid/searchable_data_frames.py
+-rw-r--r--   0        0        0     7555 2023-04-14 14:44:26.984306 orchid_python_api-5.22.299/orchid/searchable_project_objects.py
+-rw-r--r--   0        0        0     2627 2023-04-14 14:44:26.984306 orchid_python_api-5.22.299/orchid/searchable_stage_parts.py
+-rw-r--r--   0        0        0     1226 2023-04-14 14:44:26.984306 orchid_python_api-5.22.299/orchid/searchable_stages.py
+-rw-r--r--   0        0        0     6549 2023-04-14 14:44:26.985307 orchid_python_api-5.22.299/orchid/unit_system.py
+-rw-r--r--   0        0        0     1791 2023-04-14 14:44:26.985307 orchid_python_api-5.22.299/orchid/validation.py
+-rw-r--r--   0        0        0        8 2023-07-06 16:07:07.811105 orchid_python_api-5.22.299/orchid/VERSION
+-rw-r--r--   0        0        0     1098 2023-04-14 14:44:26.985307 orchid_python_api-5.22.299/orchid/version.py
+-rw-r--r--   0        0        0      844 2023-04-14 14:44:26.986307 orchid_python_api-5.22.299/orchid_python_api/__init__.py
+-rw-r--r--   0        0        0     6474 2023-04-14 14:44:26.986307 orchid_python_api-5.22.299/orchid_python_api/examples/add_stages.py
+-rw-r--r--   0        0        0     4400 2023-04-14 14:44:26.986307 orchid_python_api-5.22.299/orchid_python_api/examples/change_stage_times.py
+-rw-r--r--   0        0        0    28071 2023-04-14 14:44:26.987306 orchid_python_api-5.22.299/orchid_python_api/examples/completion_analysis.ipynb
+-rw-r--r--   0        0        0    17039 2023-04-14 14:44:26.987306 orchid_python_api-5.22.299/orchid_python_api/examples/completion_analysis.py
+-rw-r--r--   0        0        0    11549 2023-04-14 14:44:26.988308 orchid_python_api-5.22.299/orchid_python_api/examples/low_level/add_stages_low.py
+-rw-r--r--   0        0        0    23608 2023-04-14 14:44:26.988308 orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick.ipynb
+-rw-r--r--   0        0        0    15686 2023-04-14 14:44:26.988308 orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick.py
+-rw-r--r--   0        0        0    18333 2023-04-14 16:42:10.034523 orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py
+-rw-r--r--   0        0        0    15900 2023-04-14 14:44:26.989308 orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick_iterate_example.py
+-rw-r--r--   0        0        0     2446 2023-04-14 14:44:26.989308 orchid_python_api-5.22.299/orchid_python_api/examples/low_level/monitor_time_series.py
+-rw-r--r--   0        0        0    10048 2023-04-14 17:52:12.043739 orchid_python_api-5.22.299/orchid_python_api/examples/low_level/multi_picking_events.py
+-rw-r--r--   0        0        0    21648 2023-04-14 14:44:26.990670 orchid_python_api-5.22.299/orchid_python_api/examples/manual/data_frame_with_guid.ipynb
+-rw-r--r--   0        0        0     1373 2023-04-14 14:44:26.990670 orchid_python_api-5.22.299/orchid_python_api/examples/manual/data_frame_with_guid.py
+-rw-r--r--   0        0        0     8260 2023-04-14 14:44:26.991671 orchid_python_api-5.22.299/orchid_python_api/examples/plot_time_series.ipynb
+-rw-r--r--   0        0        0     4425 2023-04-14 14:44:26.991671 orchid_python_api-5.22.299/orchid_python_api/examples/plot_time_series.py
+-rw-r--r--   0        0        0     7006 2023-04-14 14:44:26.991671 orchid_python_api-5.22.299/orchid_python_api/examples/plot_trajectories.ipynb
+-rw-r--r--   0        0        0     3121 2023-04-14 14:44:26.991671 orchid_python_api-5.22.299/orchid_python_api/examples/plot_trajectories.py
+-rw-r--r--   0        0        0     7256 2023-04-14 14:44:26.992802 orchid_python_api-5.22.299/orchid_python_api/examples/plot_treatment.ipynb
+-rw-r--r--   0        0        0     3822 2023-04-14 14:44:26.992802 orchid_python_api-5.22.299/orchid_python_api/examples/plot_treatment.py
+-rw-r--r--   0        0        0      561 2023-03-30 13:38:52.090988 orchid_python_api-5.22.299/orchid_python_api/examples/python_api.yaml.example
+-rw-r--r--   0        0        0    30830 2023-04-14 16:41:20.441167 orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/internal_tests.ipynb
+-rw-r--r--   0        0        0    18681 2023-04-14 16:41:20.435151 orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/internal_tests.py
+-rw-r--r--   0        0        0    19482 2023-04-14 16:43:19.852949 orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/low_level.ipynb
+-rw-r--r--   0        0        0    14280 2023-04-14 16:41:20.448227 orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/low_level.py
+-rw-r--r--   0        0        0    13245 2023-04-14 14:44:26.993804 orchid_python_api-5.22.299/orchid_python_api/examples/search_data_frames.ipynb
+-rw-r--r--   0        0        0     5985 2023-04-14 14:44:26.994804 orchid_python_api-5.22.299/orchid_python_api/examples/search_data_frames.py
+-rw-r--r--   0        0        0     8613 2023-04-14 14:44:26.994804 orchid_python_api-5.22.299/orchid_python_api/examples/stage_qc_results.py
+-rw-r--r--   0        0        0    12887 2023-04-14 14:44:26.995804 orchid_python_api-5.22.299/orchid_python_api/examples/volume_2_first_response.ipynb
+-rw-r--r--   0        0        0     8570 2023-04-14 14:44:26.995804 orchid_python_api-5.22.299/orchid_python_api/examples/volume_2_first_response.py
+-rw-r--r--   0        0        0    24090 2023-04-14 14:44:26.995804 orchid_python_api-5.22.299/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb
+-rw-r--r--   0        0        0    19171 2023-04-14 14:44:26.996804 orchid_python_api-5.22.299/orchid_python_api/tutorials/dom_navigation_tutorial.py
+-rw-r--r--   0        0        0     3719 2023-07-06 16:07:07.813105 orchid_python_api-5.22.299/pyproject.toml
+-rw-r--r--   0        0        0    32857 2023-03-30 13:38:52.098505 orchid_python_api-5.22.299/README.md
+-rw-r--r--   0        0        0    20004 2023-07-06 16:07:07.813105 orchid_python_api-5.22.299/ReleaseNotes.md
+-rw-r--r--   0        0        0    34501 1970-01-01 00:00:00.000000 orchid_python_api-5.22.299/PKG-INFO
```

### Comparing `orchid_python_api-2023.1.220/copy_orchid_examples.py` & `orchid_python_api-5.22.299/copy_orchid_examples.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/copy_orchid_low_level_examples.py` & `orchid_python_api-5.22.299/copy_orchid_low_level_examples.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/copy_orchid_manual_examples.py` & `orchid_python_api-5.22.299/copy_orchid_manual_examples.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/copy_orchid_tutorials.py` & `orchid_python_api-5.22.299/copy_orchid_tutorials.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/LICENSE` & `orchid_python_api-5.22.299/LICENSE`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/__init__.py` & `orchid_python_api-5.22.299/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/__version__.py` & `orchid_python_api-5.22.299/orchid/__version__.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/base.py` & `orchid_python_api-5.22.299/orchid/base.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/base_time_series_adapter.py` & `orchid_python_api-5.22.299/orchid/base_time_series_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/configuration.py` & `orchid_python_api-5.22.299/orchid/configuration.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/convert.py` & `orchid_python_api-5.22.299/orchid/convert.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/core.py` & `orchid_python_api-5.22.299/orchid/core.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/dom_project_object.py` & `orchid_python_api-5.22.299/orchid/dom_project_object.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/dot_net.py` & `orchid_python_api-5.22.299/orchid/dot_net.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/dot_net_disposable.py` & `orchid_python_api-5.22.299/orchid/dot_net_disposable.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/dot_net_dom_access.py` & `orchid_python_api-5.22.299/orchid/dot_net_dom_access.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/measurement.py` & `orchid_python_api-5.22.299/orchid/measurement.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_data_frame_adapter.py` & `orchid_python_api-5.22.299/orchid/native_data_frame_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_monitor_adapter.py` & `orchid_python_api-5.22.299/orchid/native_monitor_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_project_user_data_adapter.py` & `orchid_python_api-5.22.299/orchid/native_project_user_data_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_stage_adapter.py` & `orchid_python_api-5.22.299/orchid/native_stage_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_stage_part_adapter.py` & `orchid_python_api-5.22.299/orchid/native_stage_part_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_subsurface_point.py` & `orchid_python_api-5.22.299/orchid/native_subsurface_point.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_time_series_adapter.py` & `orchid_python_api-5.22.299/orchid/native_time_series_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_trajectory_adapter.py` & `orchid_python_api-5.22.299/orchid/native_trajectory_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_treatment_calculations.py` & `orchid_python_api-5.22.299/orchid/native_treatment_calculations.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_treatment_curve_adapter.py` & `orchid_python_api-5.22.299/orchid/native_treatment_curve_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/native_well_adapter.py` & `orchid_python_api-5.22.299/orchid/native_well_adapter.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/net_date_time.py` & `orchid_python_api-5.22.299/orchid/net_date_time.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/net_enumerable.py` & `orchid_python_api-5.22.299/orchid/net_enumerable.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/net_fracture_diagnostics_factory.py` & `orchid_python_api-5.22.299/orchid/net_fracture_diagnostics_factory.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/net_quantity.py` & `orchid_python_api-5.22.299/orchid/net_quantity.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/net_stage_qc.py` & `orchid_python_api-5.22.299/orchid/net_stage_qc.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/physical_quantity.py` & `orchid_python_api-5.22.299/orchid/physical_quantity.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/project.py` & `orchid_python_api-5.22.299/orchid/project.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/project_store.py` & `orchid_python_api-5.22.299/orchid/project_store.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/reference_origins.py` & `orchid_python_api-5.22.299/orchid/reference_origins.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/script_adapter_context.py` & `orchid_python_api-5.22.299/orchid/script_adapter_context.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/searchable_data_frames.py` & `orchid_python_api-5.22.299/orchid/searchable_data_frames.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/searchable_project_objects.py` & `orchid_python_api-5.22.299/orchid/searchable_project_objects.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/searchable_stage_parts.py` & `orchid_python_api-5.22.299/orchid/searchable_stage_parts.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/searchable_stages.py` & `orchid_python_api-5.22.299/orchid/searchable_stages.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/unit_system.py` & `orchid_python_api-5.22.299/orchid/unit_system.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/validation.py` & `orchid_python_api-5.22.299/orchid/validation.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid/version.py` & `orchid_python_api-5.22.299/orchid/version.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/__init__.py` & `orchid_python_api-5.22.299/orchid_python_api/__init__.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/add_stages.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/add_stages.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/change_stage_times.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/change_stage_times.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/completion_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/completion_analysis.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/completion_analysis.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/add_stages_low.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/low_level/add_stages_low.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick_and_create_stage_attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from random import seed
 from random import random
 
 import clr  # importing `clr` must occur after `orchid` to call `pythonnet.load()`
 # noinspection PyUnresolvedReferences
 from Orchid.FractureDiagnostics import (MonitorExtensions, Leakoff, Observation)
 # noinspection PyUnresolvedReferences
-from Orchid.FractureDiagnostics.Factories.Implementations import (Attribute, LeakoffCurves)
+from Orchid.FractureDiagnostics.Factories.Implementations import LeakoffCurves
 # noinspection PyUnresolvedReferences
 from Orchid.FractureDiagnostics.SDKFacade import (
     ScriptAdapter,
 )
 # noinspection PyUnresolvedReferences
 from System import (Array, Double, DateTime, String)
 # noinspection PyUnresolvedReferences
@@ -259,20 +259,20 @@
 
     """
     observation_set = object_factory.CreateObservationSet(native_project, 'Auto-picked Observation Set3')
 
     wells = native_project.Wells.Items
 
     # Create a new "Stage Attribute"
-    pick_attribute_1 = Attribute[Double].Create("My Attribute 1", 0.0)
+    pick_attribute_1 = object_factory.CreateAttribute[Double]("My Attribute 1", 0.0)
     # TODO: Work around for only supporting double-valued stage attributes
     # Previous releases of Orchid supported integer-valued stage attributes. However, recent releases do not support
     # integer-valued stage attributes. We recognize our need to restore this feature; however, the recommended
     # work-around is to create a double-valued attribute and transform each attribute value to a Python `float`.
-    pick_attribute_2 = Attribute[Double].Create("My Attribute 2")  # Default value is 0.0 (default for `Double` values)
+    pick_attribute_2 = object_factory.CreateAttribute[Double]("My Attribute 2")  # Default value is 0.0 (default for `Double` values)
 
     def make_well_stage_key(well_name, stage_name):
         return f'{well.Name}: {stage.Name}'
 
     for well in wells:
         stages = well.Stages.Items
```

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/auto_pick_iterate_example.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/low_level/auto_pick_iterate_example.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/monitor_time_series.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/low_level/monitor_time_series.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/low_level/multi_picking_events.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/low_level/multi_picking_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     net_fracture_diagnostics_factory as net_factory,
 )
 
 import clr  # importing `clr` must occur after `orchid` to call `pythonnet.load()`
 # noinspection PyUnresolvedReferences
 from Orchid.FractureDiagnostics import (MonitorExtensions, Leakoff, Observation)
 # noinspection PyUnresolvedReferences
-from Orchid.FractureDiagnostics.Factories.Implementations import LeakoffCurves, MultiPickingObservation
+from Orchid.FractureDiagnostics.Factories.Implementations import LeakoffCurves
 # noinspection PyUnresolvedReferences
 from Orchid.FractureDiagnostics.SDKFacade import (
     ScriptAdapter,
 )
 # noinspection PyUnresolvedReferences
 from System import (Array, Double, DateTime, String)
 # noinspection PyUnresolvedReferences
@@ -99,19 +99,16 @@
                 # - Adding the observation to the observation set
                 # - Adding the observation set to the project
                 # - Saving the project.
                 #
                 # However, if one attempts to load such a project into Orchid, Orchid will report a "corrupted
                 # project" because at "object name is empty".
                 with dnd.disposable(picked_observation.ToMutable()) as mutable_observation:
-                    # The function `MultiPickingObservation` generates a name using the second argument as a "template".
-                    # The returned name is guaranteed to be unique within the specified observation set. One can
-                    # actually use any name that is unique within the observation set and is meaningful to engineers.
-                    unique_observation_name = MultiPickingObservation.GetUniqueName(observation_set,
-                                                                                    native_monitor.Name)
+                    # One can use any name that is unique within the observation set and is meaningful to engineers.
+                    unique_observation_name = native_monitor.Name + '-' + part.DisplayNameWithWell
                     mutable_observation.Name = unique_observation_name
 
                 # Add picked observation to observation set
                 with dnd.disposable(observation_set.ToMutable()) as mutable_observation_set:
                     mutable_observation_set.AddEvent(picked_observation)
 
     # Add observation set to project
```

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/manual/data_frame_with_guid.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/manual/data_frame_with_guid.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/manual/data_frame_with_guid.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/plot_time_series.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_time_series.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/plot_trajectories.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_trajectories.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/plot_trajectories.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/plot_treatment.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/plot_treatment.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/plot_treatment.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/python_api.yaml.example` & `orchid_python_api-5.22.299/orchid_python_api/examples/python_api.yaml.example`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/internal_tests.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997519841269842%*

 * *Differences: {"'cells'": "{3: {'source': ['import orchid\\n', '\\n', 'from orchid import (\\n', '    "*

 * *            "net_fracture_diagnostics_factory as net_factory,\\n', ')']}, 5: {'source': {insert: "*

 * *            "[(10, ')\\n'), (11, '\\n'), (12, 'object_factory = net_factory.create()')], delete: "*

 * *            '[10]}}, 25: {\'source\': {insert: [(2, "attribute_to_add = '*

 * *            'object_factory.CreateAttribute[attribute_to_add_type](\'My New Attribute\')")], '*

 * *            'delete: [5, 3, 2, 1]}}}'}*

```diff
@@ -34,15 +34,19 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "eb29845a-d005-49eb-8c8e-9d89498ab911",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import orchid"
+                "import orchid\n",
+                "\n",
+                "from orchid import (\n",
+                "    net_fracture_diagnostics_factory as net_factory,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "19621d00-1157-4131-85f2-82b068d9ad77",
             "metadata": {},
@@ -70,15 +74,17 @@
                 "    Convert,\n",
                 "    DateTime,\n",
                 "    DateTimeKind,\n",
                 "    DateTimeOffset,\n",
                 "    Int32,\n",
                 "    InvalidCastException,\n",
                 "    TimeSpan,\n",
-                ")"
+                ")\n",
+                "\n",
+                "object_factory = net_factory.create()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "09125724",
             "metadata": {},
             "source": [
@@ -334,19 +340,16 @@
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
                 "# Create an attribute with name, 'My New Attribute', and type, `System.Int32`\n",
-                "# noinspection PyUnresolvedReferences,PyPackageRequirements\n",
-                "from Orchid.FractureDiagnostics.Factories.Implementations import Attribute\n",
-                "\n",
                 "attribute_to_add_type = Int32\n",
-                "attribute_to_add = Attribute[attribute_to_add_type].Create('My New Attribute')"
+                "attribute_to_add = object_factory.CreateAttribute[attribute_to_add_type]('My New Attribute')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8e4cff25",
             "metadata": {
```

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/internal_tests.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/internal_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,38 +26,39 @@
 # runtime which may **not** be compatible with the installed Orchid assemblies.
 #
 # To make this easier, when we `import` the `orchid` package, the Orchid Python API will load the runtime
 # corresponding to the configured Orchid installation.
 
 # noinspection PyUnresolvedReferences
 import orchid
+from orchid import (
+    net_fracture_diagnostics_factory as net_factory,
+)
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 import clr
 
 import pprint  # Used to "pretty-print" complex data, for example, lists
 import textwrap  # Help to format pretty printed text
 
 import pendulum
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
-from Orchid.FractureDiagnostics.Factories.Implementations import Attribute
-
-# noinspection PyUnresolvedReferences,PyPackageRequirements
 from System import (
     ArgumentException,
     Convert,
     DateTime,
     DateTimeKind,
     DateTimeOffset,
     Int32,
     InvalidCastException,
     TimeSpan,
 )
 
+object_factory = net_factory.create()
 
 DEFAULT_TEXTWRAP_WIDTH = 70
 
 
 def print_underline(text, ch):
     print(textwrap.fill(text))
     print(min(len(text), DEFAULT_TEXTWRAP_WIDTH) * ch)
@@ -212,15 +213,15 @@
 bakken = orchid.load_project('c:/src/Orchid.IntegrationTestData/frankNstein_Bakken_UTM13_FEET.ifrac')
 candidate_wells = list(bakken.wells().find_by_name('Demo_1H'))
 assert len(candidate_wells) == 1
 demo_1h = candidate_wells[0]
 
 # Create an attribute with name, 'My New Attribute', and type, `System.Int32`
 attribute_to_add_type = Int32
-attribute_to_add = Attribute[attribute_to_add_type].Create('My New Attribute')
+attribute_to_add = object_factory.CreateAttribute[attribute_to_add_type]('My New Attribute')
 
 # Add newly created attribute to well, 'Demo_1H'
 with orchid.dot_net_disposable.disposable(demo_1h.dom_object.ToMutable()) as mutable_well:
     mutable_well.AddStageAttribute(attribute_to_add)
 
 # Find stage number 7 in well, 'Demo_1H'
 maybe_stage = demo_1h.stages().find_by_display_stage_number(7)
```

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/low_level.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995734126984127%*

 * *Differences: {"'cells'": "{2: {'source': ['import orchid\\n', '\\n', 'from orchid import (\\n', '    "*

 * *            "net_fracture_diagnostics_factory as net_factory,\\n', ')']}, 4: {'source': {insert: "*

 * *            "[(8, ')\\n'), (9, '\\n'), (10, 'object_factory = net_factory.create()')], delete: "*

 * *            '[8]}}, 11: {\'source\': {insert: [(2, "attribute_to_add = '*

 * *            'object_factory.CreateAttribute[attribute_to_add_type](\'My New Attribute\')")], '*

 * *            'delete: [5, 3, 2, 1]}}}'}*

```diff
@@ -31,15 +31,19 @@
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
-                "import orchid"
+                "import orchid\n",
+                "\n",
+                "from orchid import (\n",
+                "    net_fracture_diagnostics_factory as net_factory,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1df3ff3a",
             "metadata": {
@@ -70,15 +74,17 @@
                 "from System import (\n",
                 "    ArgumentException,\n",
                 "    Array,\n",
                 "    DateTime,\n",
                 "    TimeSpan,\n",
                 "    Int32,\n",
                 "    ValueType,\n",
-                ")"
+                ")\n",
+                "\n",
+                "object_factory = net_factory.create()"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "83ee8fcc-9413-4cb4-9a2c-a9e7a8cc937b",
             "metadata": {},
             "source": [
@@ -150,19 +156,16 @@
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
                 "# Create an attribute with name, 'My New Attribute', and type, `System.Int32`\n",
-                "# noinspection PyUnresolvedReferences,PyPackageRequirements\n",
-                "from Orchid.FractureDiagnostics.Factories.Implementations import Attribute\n",
-                "\n",
                 "attribute_to_add_type = Int32\n",
-                "attribute_to_add = Attribute[attribute_to_add_type].Create('My New Attribute')"
+                "attribute_to_add = object_factory.CreateAttribute[attribute_to_add_type]('My New Attribute')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9e46f653-d4ab-4155-891f-7987cbc76a17",
             "metadata": {
```

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/pythonnet3/low_level.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/pythonnet3/low_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,27 +26,28 @@
 # runtime which may **not** be compatible with the installed Orchid assemblies.
 #
 # To make this easier, when we `import` the `orchid` package, the Orchid Python API will load the runtime
 # corresponding to the configured Orchid installation.
 
 # noinspection PyUnresolvedReferences
 import orchid
+from orchid import (
+    net_fracture_diagnostics_factory as net_factory,
+)
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 import clr
 
 import collections.abc
 import pprint  # Used to "pretty-print" complex data, for example, lists
 import textwrap  # Help to format pretty printed text
 
 import pendulum
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
-from Orchid.FractureDiagnostics.Factories.Implementations import Attribute
-# noinspection PyUnresolvedReferences,PyPackageRequirements
 from Orchid.FractureDiagnostics import Leakoff
 # noinspection PyUnresolvedReferences
 import UnitsNet
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 from System import (
     ArgumentException,
@@ -59,15 +60,15 @@
     TimeSpan,
 )
 
 clr.AddReference('System.Collections')
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 from System.Collections.Generic import List
 
-
+object_factory = net_factory.create()
 DEFAULT_TEXTWRAP_WIDTH = 70
 
 
 def print_underline(text, ch):
     print(textwrap.fill(text))
     print(min(len(text), DEFAULT_TEXTWRAP_WIDTH) * ch)
     print()
@@ -165,15 +166,15 @@
 bakken = orchid.load_project('c:/src/Orchid.IntegrationTestData/frankNstein_Bakken_UTM13_FEET.ifrac')
 candidate_wells = list(bakken.wells().find_by_name('Demo_1H'))
 assert len(candidate_wells) == 1
 demo_1h = candidate_wells[0]
 
 # Create an attribute with name, 'My New Attribute', and type, `System.Int32`
 attribute_to_add_type = Int32
-attribute_to_add = Attribute[attribute_to_add_type].Create('My New Attribute')
+attribute_to_add = object_factory.CreateAttribute[attribute_to_add_type]('My New Attribute')
 
 # Add newly created attribute to well, 'Demo_1H'
 with orchid.dot_net_disposable.disposable(demo_1h.dom_object.ToMutable()) as mutable_well:
     mutable_well.AddStageAttribute(attribute_to_add)
 
 # Find stage number 7 in well, 'Demo_1H'
 maybe_stage = demo_1h.stages().find_by_display_stage_number(7)
```

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/search_data_frames.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/search_data_frames.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/search_data_frames.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/stage_qc_results.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/stage_qc_results.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/examples/volume_2_first_response.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/examples/volume_2_first_response.py` & `orchid_python_api-5.22.299/orchid_python_api/examples/volume_2_first_response.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb` & `orchid_python_api-5.22.299/orchid_python_api/tutorials/dom_navigation_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/orchid_python_api/tutorials/dom_navigation_tutorial.py` & `orchid_python_api-5.22.299/orchid_python_api/tutorials/dom_navigation_tutorial.py`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/pyproject.toml` & `orchid_python_api-5.22.299/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry>=0.12",]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "orchid-python-api"
-version = "2023.1.220"
+version = "5.22.299"
 description = "Defines and implements the Python API for Orchid*. (*Orchid is a mark of Reveal Energy Services, Inc.)"
 authors = [ "Reveal Energy Services, Inc. <support@reveal-energy.com>",]
 maintainers = [ "Reveal Energy Services, Inc. <support@reveal-energy.com>",]
 license = "Apache-2.0"
 readme = "README.md"
 homepage="https://github.com/Reveal-Energy-Services/orchid-python-api"
 repository="https://github.com/Reveal-Energy-Services/orchid-python-api"
```

### Comparing `orchid_python_api-2023.1.220/README.md` & `orchid_python_api-5.22.299/README.md`

 * *Files identical despite different names*

### Comparing `orchid_python_api-2023.1.220/ReleaseNotes.md` & `orchid_python_api-5.22.299/ReleaseNotes.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,35 @@
 - [ReleaseNotes.md](./ReleaseNotes.md) - The release notes for this project.
 
 Although one can read this document in any text editor since it is simply a text file, consider installing
 the [Python grip utility](https://pypi.org/project/grip/). This application allows one to "render local readme
 files before sending off to GitHub". Although you need not send any of these file to `GitHub`, by using `grip` 
 to render the file, you can much more easily navigate the document links.
 
+### Release notes for 5.22.299
+
+This release is the production release of the Orchid Python API corresponding to Orchid 5.22.299.
+
+#### Possible breaking .NET API changes
+
+- None
+
+#### Resolved Issues
+
+- None
+
+#### Features
+
+- None
+
+#### Known Issues
+
+- None
+
+
 ### Release notes for 2023.1.220
 
 This release is the production release of the Orchid Python API corresponding to Orchid 2023.1.220. A very basic example of how
 to get to a project's well horizon markers was added. Additionally, a fix to an integration test is included.
 
 #### Possible breaking .NET API changes
```

### Comparing `orchid_python_api-2023.1.220/PKG-INFO` & `orchid_python_api-5.22.299/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orchid-python-api
-Version: 2023.1.220
+Version: 5.22.299
 Summary: Defines and implements the Python API for Orchid*. (*Orchid is a mark of Reveal Energy Services, Inc.)
 Home-page: https://github.com/Reveal-Energy-Services/orchid-python-api
 License: Apache-2.0
 Keywords: Orchid Integration,Fracture Diagnostics
 Author: Reveal Energy Services, Inc.
 Author-email: support@reveal-energy.com
 Maintainer: Reveal Energy Services, Inc.
@@ -14,16 +14,14 @@
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: deal (>=4.23.4,<5.0.0)
 Requires-Dist: ipython (>=8.7.0,<9.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
```

