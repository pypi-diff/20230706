# Comparing `tmp/nomad_camels-0.1.3.tar.gz` & `tmp/nomad_camels-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomad_camels-0.1.3.tar", last modified: Thu Jun 29 14:32:17 2023, max compression
+gzip compressed data, was "nomad_camels-0.1.4.tar", last modified: Thu Jul  6 12:20:13 2023, max compression
```

## Comparing `nomad_camels-0.1.3.tar` & `nomad_camels-0.1.4.tar`

### file list

```diff
@@ -1,163 +1,160 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.440224 nomad_camels-0.1.3/
--rw-rw-rw-   0        0        0    26526 2023-06-28 14:51:17.000000 nomad_camels-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    26525 2023-06-28 14:51:17.000000 nomad_camels-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       27 2023-06-28 14:51:17.000000 nomad_camels-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2101 2023-06-29 14:32:17.439225 nomad_camels-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1451 2023-06-28 14:51:17.000000 nomad_camels-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.229291 nomad_camels-0.1.3/nomad_camels/
--rw-rw-rw-   0        0        0     4227 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/CAMELS_start.py
--rw-rw-rw-   0        0        0    43072 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/MainApp_v2.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.251489 nomad_camels-0.1.3/nomad_camels/bluesky_handling/
--rw-rw-rw-   0        0        0     5236 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/EpicsFieldSignal.py
--rw-rw-rw-   0        0        0     1827 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/__init__.py
--rw-rw-rw-   0        0        0     6047 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/builder_helper_functions.py
--rw-rw-rw-   0        0        0     4103 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/custom_function_signal.py
--rw-rw-rw-   0        0        0     4841 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/evaluation_helper.py
--rw-rw-rw-   0        0        0    18283 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/helper_functions.py
--rw-rw-rw-   0        0        0     1666 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/make_catalog.py
--rw-rw-rw-   0        0        0    14114 2023-06-29 11:51:05.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/protocol_builder.py
--rw-rw-rw-   0        0        0      786 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/special_plan_stubs.py
--rw-rw-rw-   0        0        0    10588 2023-06-29 14:22:20.000000 nomad_camels-0.1.3/nomad_camels/bluesky_handling/visa_signal.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.253488 nomad_camels-0.1.3/nomad_camels/commands/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/commands/__init__.py
--rw-rw-rw-   0        0        0     4635 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/commands/change_sequence.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.265418 nomad_camels-0.1.3/nomad_camels/frontpanels/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/__init__.py
--rw-rw-rw-   0        0        0     9749 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/device_add_dialog.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.271417 nomad_camels-0.1.3/nomad_camels/frontpanels/helper_panels/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/helper_panels/__init__.py
--rw-rw-rw-   0        0        0     8771 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
--rw-rw-rw-   0        0        0      830 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
--rw-rw-rw-   0        0        0      236 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/helper_panels/pass_ask.py
--rw-rw-rw-   0        0        0    10082 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/instrument_config.py
--rw-rw-rw-   0        0        0    13171 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/instrument_installer.py
--rw-rw-rw-   0        0        0     2925 2023-06-29 11:51:05.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/manage_instruments.py
--rw-rw-rw-   0        0        0    22774 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/plot_definer.py
--rw-rw-rw-   0        0        0    22381 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/protocol_config.py
--rw-rw-rw-   0        0        0     8557 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/settings_window.py
--rw-rw-rw-   0        0        0     1951 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/frontpanels/taskSelector.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.284308 nomad_camels-0.1.3/nomad_camels/graphics/
--rw-rw-rw-   0        0        0    16958 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/CAMELS.ico
--rw-rw-rw-   0        0        0     2926 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/CAMELS_Icon.png
--rw-rw-rw-   0        0        0   101760 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
--rw-rw-rw-   0        0        0   479310 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
--rw-rw-rw-   0        0        0    13283 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/camels-horizontal.svg
--rw-rw-rw-   0        0        0    13715 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/camels-vertical.svg
--rw-rw-rw-   0        0        0    12919 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/camels_horizontal.png
--rw-rw-rw-   0        0        0    19245 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/camels_vertical.png
--rw-rw-rw-   0        0        0    40043 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/dark.qss
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.304119 nomad_camels-0.1.3/nomad_camels/graphics/legacy/
--rw-rw-rw-   0        0        0    60728 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS.svg
--rw-rw-rw-   0        0        0    52644 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Icon.png
--rw-rw-rw-   0        0        0   349358 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
--rw-rw-rw-   0        0        0    34101 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
--rw-rw-rw-   0        0        0    42984 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Logo.png
--rw-rw-rw-   0        0        0    43703 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Logo.svg
--rw-rw-rw-   0        0        0    96186 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
--rw-rw-rw-   0        0        0    18507 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_V1.svg
--rw-rw-rw-   0        0        0    20058 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_v2.svg
--rw-rw-rw-   0        0        0   290607 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/camels - Kopie.png
--rw-rw-rw-   0        0        0   252699 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/camels_free.png
--rw-rw-rw-   0        0        0     7058 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/graphics/legacy/plus_sign.png
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.327560 nomad_camels-0.1.3/nomad_camels/gui/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/__init__.py
--rw-rw-rw-   0        0        0     6130 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/addDeviceDialog.py
--rw-rw-rw-   0        0        0     5535 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/device_installer.py
--rw-rw-rw-   0        0        0     2841 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/enterTextDialog.py
--rw-rw-rw-   0        0        0     4027 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/fit_definer.py
--rw-rw-rw-   0        0        0    11001 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/for_loop.py
--rw-rw-rw-   0        0        0     6623 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/general_protocol_settings.py
--rw-rw-rw-   0        0        0     8501 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/gradient_descent_step.py
--rw-rw-rw-   0        0        0     8629 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/installer_window.py
--rw-rw-rw-   0        0        0     4572 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/instrument_config.py
--rw-rw-rw-   0        0        0    22581 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/gui/mainWindow_v2.py
--rw-rw-rw-   0        0        0     2893 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/pass_ask.py
--rw-rw-rw-   0        0        0     7219 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/plot_definer.py
--rw-rw-rw-   0        0        0     6027 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/plot_definer_2d.py
--rw-rw-rw-   0        0        0     3885 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/plot_options.py
--rw-rw-rw-   0        0        0     7230 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/protocol_view.py
--rw-rw-rw-   0        0        0     2537 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/read_channels.py
--rw-rw-rw-   0        0        0     1465 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/set_channels.py
--rw-rw-rw-   0        0        0    13462 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/gui/settings_window.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.348112 nomad_camels-0.1.3/nomad_camels/loop_steps/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/__init__.py
--rw-rw-rw-   0        0        0     4250 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/change_device_config.py
--rw-rw-rw-   0        0        0    28108 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/for_while_loops.py
--rw-rw-rw-   0        0        0     8185 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/gradient_descent.py
--rw-rw-rw-   0        0        0    10586 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/if_step.py
--rw-rw-rw-   0        0        0     4905 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/make_step_of_type.py
--rw-rw-rw-   0        0        0    13322 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/nd_sweep.py
--rw-rw-rw-   0        0        0     3550 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/prompt_loop_step.py
--rw-rw-rw-   0        0        0    15156 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/read_channels.py
--rw-rw-rw-   0        0        0     7679 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/run_subprotocol.py
--rw-rw-rw-   0        0        0     4488 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/set_channels.py
--rw-rw-rw-   0        0        0     4099 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/set_value_popup.py
--rw-rw-rw-   0        0        0     2383 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/set_variables.py
--rw-rw-rw-   0        0        0    14715 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/simple_sweep.py
--rw-rw-rw-   0        0        0     2648 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/loop_steps/wait_loop_step.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.361016 nomad_camels-0.1.3/nomad_camels/main_classes/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/__init__.py
--rw-rw-rw-   0        0        0     1706 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/camels_installer.py
--rw-rw-rw-   0        0        0    28770 2023-06-29 11:51:05.000000 nomad_camels-0.1.3/nomad_camels/main_classes/device_class.py
--rw-rw-rw-   0        0        0     3595 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/list_plot.py
--rw-rw-rw-   0        0        0    11255 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/loop_step.py
--rw-rw-rw-   0        0        0     3993 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/manual_control.py
--rw-rw-rw-   0        0        0     1242 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/measurement_channel.py
--rw-rw-rw-   0        0        0     7869 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/plot_2D.py
--rw-rw-rw-   0        0        0    48782 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/main_classes/plot_widget.py
--rw-rw-rw-   0        0        0    21225 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/main_classes/protocol_class.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.363018 nomad_camels-0.1.3/nomad_camels/manual_controls/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/manual_controls/__init__.py
--rw-rw-rw-   0        0        0     2599 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/manual_controls/get_manual_controls.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.367270 nomad_camels-0.1.3/nomad_camels/manual_controls/stage_control/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/manual_controls/stage_control/__init__.py
--rw-rw-rw-   0        0        0    20282 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/manual_controls/stage_control/stage_control.py
--rw-rw-rw-   0        0        0    12048 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/manual_controls/stage_control/ui_stage_control.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.371272 nomad_camels-0.1.3/nomad_camels/tests/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/tests/__init__.py
--rw-rw-rw-   0        0        0     3182 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/tests/instrument_management_test.py
--rw-rw-rw-   0        0        0    20124 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/tests/protocol_test.py
--rw-rw-rw-   0        0        0      768 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/tests/startup_test.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.378270 nomad_camels-0.1.3/nomad_camels/tools/
--rw-rw-rw-   0        0        0     8502 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/tools/EPICS_driver_builder.py
--rw-rw-rw-   0        0        0     5627 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/tools/VISA_builder.py
--rw-rw-rw-   0        0        0    11374 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/tools/VISA_driver_builder.py
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/tools/__init__.py
--rw-rw-rw-   0        0        0     8548 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/tools/databroker_exporter.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.388268 nomad_camels-0.1.3/nomad_camels/ui_widgets/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/__init__.py
--rw-rw-rw-   0        0        0    20475 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/add_remove_table.py
--rw-rw-rw-   0        0        0     9089 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/channels_check_table.py
--rw-rw-rw-   0        0        0     1742 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/console_redirect.py
--rw-rw-rw-   0        0        0     1204 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/drag_drop_tree_view.py
--rw-rw-rw-   0        0        0     6522 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/options_run_button.py
--rw-rw-rw-   0        0        0     2493 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/path_button_edit.py
--rw-rw-rw-   0        0        0     3567 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/variable_tool_tip_box.py
--rw-rw-rw-   0        0        0      451 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/ui_widgets/warn_popup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.438225 nomad_camels-0.1.3/nomad_camels/utility/
--rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/__init__.py
--rw-rw-rw-   0        0        0    15701 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/databroker_export.py
--rw-rw-rw-   0        0        0     5204 2023-06-29 11:51:05.000000 nomad_camels-0.1.3/nomad_camels/utility/device_handling.py
--rw-rw-rw-   0        0        0     1833 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/exception_hook.py
--rw-rw-rw-   0        0        0      788 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/fit_variable_renaming.py
--rw-rw-rw-   0        0        0    14745 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/utility/load_save_functions.py
--rw-rw-rw-   0        0        0      938 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/load_save_helper_functions.py
--rw-rw-rw-   0        0        0      867 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/number_formatting.py
--rw-rw-rw-   0        0        0     1583 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/plot_placement.py
--rw-rw-rw-   0        0        0     9893 2023-06-28 15:46:34.000000 nomad_camels-0.1.3/nomad_camels/utility/qthreads.py
--rw-rw-rw-   0        0        0     2496 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/theme_changing.py
--rw-rw-rw-   0        0        0      330 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/tqdm_progress_bar.py
--rw-rw-rw-   0        0        0     2573 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/treeView_functions.py
--rw-rw-rw-   0        0        0     2674 2023-06-28 15:48:04.000000 nomad_camels-0.1.3/nomad_camels/utility/update_camels.py
--rw-rw-rw-   0        0        0    10431 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/nomad_camels/utility/variables_handling.py
-drwxrwxrwx   0        0        0        0 2023-06-29 14:32:17.236218 nomad_camels-0.1.3/nomad_camels.egg-info/
--rw-rw-rw-   0        0        0     2101 2023-06-29 14:32:17.000000 nomad_camels-0.1.3/nomad_camels.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5841 2023-06-29 14:32:17.000000 nomad_camels-0.1.3/nomad_camels.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:32:17.000000 nomad_camels-0.1.3/nomad_camels.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1340 2023-06-29 14:32:17.000000 nomad_camels-0.1.3/nomad_camels.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-29 14:32:17.000000 nomad_camels-0.1.3/nomad_camels.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      925 2023-06-29 14:31:46.000000 nomad_camels-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1340 2023-06-28 14:51:20.000000 nomad_camels-0.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:32:17.440224 nomad_camels-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/
+-rw-rw-rw-   0        0        0    26526 2023-06-28 14:51:17.000000 nomad_camels-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    26525 2023-06-28 14:51:17.000000 nomad_camels-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       27 2023-06-28 14:51:17.000000 nomad_camels-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2317 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1654 2023-07-06 07:41:24.000000 nomad_camels-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.415637 nomad_camels-0.1.4/nomad_camels/
+-rw-rw-rw-   0        0        0     4227 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/CAMELS_start.py
+-rw-rw-rw-   0        0        0    43072 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/MainApp_v2.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.495956 nomad_camels-0.1.4/nomad_camels/bluesky_handling/
+-rw-rw-rw-   0        0        0     5236 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/EpicsFieldSignal.py
+-rw-rw-rw-   0        0        0     1827 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/__init__.py
+-rw-rw-rw-   0        0        0     6047 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/builder_helper_functions.py
+-rw-rw-rw-   0        0        0     4103 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/custom_function_signal.py
+-rw-rw-rw-   0        0        0     4841 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/evaluation_helper.py
+-rw-rw-rw-   0        0        0    22693 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/helper_functions.py
+-rw-rw-rw-   0        0        0     1915 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/make_catalog.py
+-rw-rw-rw-   0        0        0    16474 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/protocol_builder.py
+-rw-rw-rw-   0        0        0      885 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/special_plan_stubs.py
+-rw-rw-rw-   0        0        0    10686 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/bluesky_handling/visa_signal.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.497955 nomad_camels-0.1.4/nomad_camels/commands/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/commands/__init__.py
+-rw-rw-rw-   0        0        0     5509 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/commands/change_sequence.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.593931 nomad_camels-0.1.4/nomad_camels/frontpanels/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/__init__.py
+-rw-rw-rw-   0        0        0     9749 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/device_add_dialog.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.632724 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/__init__.py
+-rw-rw-rw-   0        0        0     8771 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
+-rw-rw-rw-   0        0        0      830 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/enterTextDialog.py
+-rw-rw-rw-   0        0        0      236 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/pass_ask.py
+-rw-rw-rw-   0        0        0    10082 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_config.py
+-rw-rw-rw-   0        0        0    13171 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_installer.py
+-rw-rw-rw-   0        0        0     2925 2023-06-29 11:51:05.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/manage_instruments.py
+-rw-rw-rw-   0        0        0    22774 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/plot_definer.py
+-rw-rw-rw-   0        0        0    22381 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/protocol_config.py
+-rw-rw-rw-   0        0        0     8557 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/frontpanels/settings_window.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.716860 nomad_camels-0.1.4/nomad_camels/graphics/
+-rw-rw-rw-   0        0        0    16958 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/CAMELS.ico
+-rw-rw-rw-   0        0        0     2926 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/CAMELS_Icon.png
+-rw-rw-rw-   0        0        0   101760 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
+-rw-rw-rw-   0        0        0   479310 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav
+-rw-rw-rw-   0        0        0    13283 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels-horizontal.svg
+-rw-rw-rw-   0        0        0    13715 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels-vertical.svg
+-rw-rw-rw-   0        0        0    12919 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels_horizontal.png
+-rw-rw-rw-   0        0        0    19245 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/camels_vertical.png
+-rw-rw-rw-   0        0        0    40043 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/dark.qss
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.808157 nomad_camels-0.1.4/nomad_camels/graphics/legacy/
+-rw-rw-rw-   0        0        0    60728 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS.svg
+-rw-rw-rw-   0        0        0    52644 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon.png
+-rw-rw-rw-   0        0        0   349358 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico
+-rw-rw-rw-   0        0        0    34101 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico
+-rw-rw-rw-   0        0        0    42984 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.png
+-rw-rw-rw-   0        0        0    43703 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.svg
+-rw-rw-rw-   0        0        0    96186 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg
+-rw-rw-rw-   0        0        0    18507 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_V1.svg
+-rw-rw-rw-   0        0        0    20058 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_v2.svg
+-rw-rw-rw-   0        0        0   290607 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels - Kopie.png
+-rw-rw-rw-   0        0        0   252699 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels_free.png
+-rw-rw-rw-   0        0        0     7058 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/graphics/legacy/plus_sign.png
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.896284 nomad_camels-0.1.4/nomad_camels/gui/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/__init__.py
+-rw-rw-rw-   0        0        0     6130 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/addDeviceDialog.py
+-rw-rw-rw-   0        0        0     5535 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/device_installer.py
+-rw-rw-rw-   0        0        0     2841 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/enterTextDialog.py
+-rw-rw-rw-   0        0        0     4027 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/fit_definer.py
+-rw-rw-rw-   0        0        0    11001 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/for_loop.py
+-rw-rw-rw-   0        0        0     6623 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/general_protocol_settings.py
+-rw-rw-rw-   0        0        0     8501 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/gradient_descent_step.py
+-rw-rw-rw-   0        0        0     4572 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/instrument_config.py
+-rw-rw-rw-   0        0        0    22581 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/gui/mainWindow_v2.py
+-rw-rw-rw-   0        0        0     2893 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/pass_ask.py
+-rw-rw-rw-   0        0        0     7219 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/plot_definer.py
+-rw-rw-rw-   0        0        0     6027 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/plot_definer_2d.py
+-rw-rw-rw-   0        0        0     3885 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/plot_options.py
+-rw-rw-rw-   0        0        0     7230 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/protocol_view.py
+-rw-rw-rw-   0        0        0     2537 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/read_channels.py
+-rw-rw-rw-   0        0        0     1465 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/set_channels.py
+-rw-rw-rw-   0        0        0    13462 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/gui/settings_window.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.016280 nomad_camels-0.1.4/nomad_camels/loop_steps/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/__init__.py
+-rw-rw-rw-   0        0        0     4577 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/change_device_config.py
+-rw-rw-rw-   0        0        0    28468 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/for_while_loops.py
+-rw-rw-rw-   0        0        0    10275 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/gradient_descent.py
+-rw-rw-rw-   0        0        0     9981 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/if_step.py
+-rw-rw-rw-   0        0        0     5520 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/make_step_of_type.py
+-rw-rw-rw-   0        0        0    14155 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/nd_sweep.py
+-rw-rw-rw-   0        0        0     3550 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/prompt_loop_step.py
+-rw-rw-rw-   0        0        0    15156 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/read_channels.py
+-rw-rw-rw-   0        0        0     7679 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/run_subprotocol.py
+-rw-rw-rw-   0        0        0     4488 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/set_channels.py
+-rw-rw-rw-   0        0        0     4099 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/set_value_popup.py
+-rw-rw-rw-   0        0        0     2383 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/set_variables.py
+-rw-rw-rw-   0        0        0    14715 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/simple_sweep.py
+-rw-rw-rw-   0        0        0     2648 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/loop_steps/wait_loop_step.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.126276 nomad_camels-0.1.4/nomad_camels/main_classes/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/__init__.py
+-rw-rw-rw-   0        0        0    29151 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/main_classes/device_class.py
+-rw-rw-rw-   0        0        0     3595 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/list_plot.py
+-rw-rw-rw-   0        0        0    12119 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/main_classes/loop_step.py
+-rw-rw-rw-   0        0        0     3993 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/manual_control.py
+-rw-rw-rw-   0        0        0     1242 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/measurement_channel.py
+-rw-rw-rw-   0        0        0     7869 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/plot_2D.py
+-rw-rw-rw-   0        0        0    48782 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/main_classes/plot_widget.py
+-rw-rw-rw-   0        0        0    21225 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/main_classes/protocol_class.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.126276 nomad_camels-0.1.4/nomad_camels/manual_controls/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/__init__.py
+-rw-rw-rw-   0        0        0     2599 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/get_manual_controls.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.156276 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/__init__.py
+-rw-rw-rw-   0        0        0    20282 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/stage_control.py
+-rw-rw-rw-   0        0        0    12048 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/ui_stage_control.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.186277 nomad_camels-0.1.4/nomad_camels/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tests/__init__.py
+-rw-rw-rw-   0        0        0     3182 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/tests/instrument_management_test.py
+-rw-rw-rw-   0        0        0    20124 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/tests/protocol_test.py
+-rw-rw-rw-   0        0        0      768 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tests/startup_test.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.206264 nomad_camels-0.1.4/nomad_camels/tools/
+-rw-rw-rw-   0        0        0     8933 2023-07-06 07:34:02.000000 nomad_camels-0.1.4/nomad_camels/tools/EPICS_driver_builder.py
+-rw-rw-rw-   0        0        0     5627 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tools/VISA_builder.py
+-rw-rw-rw-   0        0        0    11304 2023-06-30 08:55:10.000000 nomad_camels-0.1.4/nomad_camels/tools/VISA_driver_builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tools/__init__.py
+-rw-rw-rw-   0        0        0     8548 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/tools/databroker_exporter.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.308243 nomad_camels-0.1.4/nomad_camels/ui_widgets/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/__init__.py
+-rw-rw-rw-   0        0        0    20475 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/add_remove_table.py
+-rw-rw-rw-   0        0        0     9089 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/channels_check_table.py
+-rw-rw-rw-   0        0        0     1742 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/console_redirect.py
+-rw-rw-rw-   0        0        0     1204 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/drag_drop_tree_view.py
+-rw-rw-rw-   0        0        0     6522 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/options_run_button.py
+-rw-rw-rw-   0        0        0     2493 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/path_button_edit.py
+-rw-rw-rw-   0        0        0     3567 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/variable_tool_tip_box.py
+-rw-rw-rw-   0        0        0      451 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/ui_widgets/warn_popup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/nomad_camels/utility/
+-rw-rw-rw-   0        0        0        0 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/__init__.py
+-rw-rw-rw-   0        0        0    15701 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/databroker_export.py
+-rw-rw-rw-   0        0        0     5204 2023-06-29 11:51:05.000000 nomad_camels-0.1.4/nomad_camels/utility/device_handling.py
+-rw-rw-rw-   0        0        0     1833 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/exception_hook.py
+-rw-rw-rw-   0        0        0      788 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/fit_variable_renaming.py
+-rw-rw-rw-   0        0        0    14745 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/utility/load_save_functions.py
+-rw-rw-rw-   0        0        0      938 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/load_save_helper_functions.py
+-rw-rw-rw-   0        0        0      867 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/number_formatting.py
+-rw-rw-rw-   0        0        0     1583 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/plot_placement.py
+-rw-rw-rw-   0        0        0     9893 2023-06-28 15:46:34.000000 nomad_camels-0.1.4/nomad_camels/utility/qthreads.py
+-rw-rw-rw-   0        0        0     2496 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/theme_changing.py
+-rw-rw-rw-   0        0        0      330 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/tqdm_progress_bar.py
+-rw-rw-rw-   0        0        0     2573 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/treeView_functions.py
+-rw-rw-rw-   0        0        0     2674 2023-06-28 15:48:04.000000 nomad_camels-0.1.4/nomad_camels/utility/update_camels.py
+-rw-rw-rw-   0        0        0    10431 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/nomad_camels/utility/variables_handling.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:20:12.428961 nomad_camels-0.1.4/nomad_camels.egg-info/
+-rw-rw-rw-   0        0        0     2317 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5717 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1340 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-06 12:20:12.000000 nomad_camels-0.1.4/nomad_camels.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      925 2023-07-06 12:15:55.000000 nomad_camels-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1340 2023-06-28 14:51:20.000000 nomad_camels-0.1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 12:20:13.387436 nomad_camels-0.1.4/setup.cfg
```

### Comparing `nomad_camels-0.1.3/LICENSE` & `nomad_camels-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/LICENSE.txt` & `nomad_camels-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/PKG-INFO` & `nomad_camels-0.1.4/nomad_camels.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nomad_camels
-Version: 0.1.3
+Name: nomad-camels
+Version: 0.1.4
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
@@ -24,7 +24,19 @@
 
 NOMAD-CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics. Here many experiments utilize a multitude of measurement devices used in dynamically changing setups. CAMELS will allow to define instrument control and measurement protocols using a graphical user interface (GUI). This provides a low entry threshold enabling the creation of new measurement protocols without programming knowledge or a deeper understanding of device communication. The GUI generates python code that interfaces with instruments and allows users to modify the code for specific applications and implementations of arbitrary devices if necessary. Even large-scale, distributed systems can be implemented. CAMELS is well suited to generate FAIR-compliant output data. Nexus standards, immediate NOMAD integration and hence a FAIRmat compliant data pipeline can be readily implemented.
 
 
 ## Documentation
 
 For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/).
+
+# Changelog
+
+
+## 0.1.4
+Added a timeout setting to all VISA instruments. 
+
+## 0.1.3
+First stable and working release
+
+## 0.1.0 to 0.1.2 
+&#9888; Broken releases due to minor bugs that were fixed in 0.1.3
```

### Comparing `nomad_camels-0.1.3/README.md` & `nomad_camels-0.1.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,7 +10,19 @@
 
 NOMAD-CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics. Here many experiments utilize a multitude of measurement devices used in dynamically changing setups. CAMELS will allow to define instrument control and measurement protocols using a graphical user interface (GUI). This provides a low entry threshold enabling the creation of new measurement protocols without programming knowledge or a deeper understanding of device communication. The GUI generates python code that interfaces with instruments and allows users to modify the code for specific applications and implementations of arbitrary devices if necessary. Even large-scale, distributed systems can be implemented. CAMELS is well suited to generate FAIR-compliant output data. Nexus standards, immediate NOMAD integration and hence a FAIRmat compliant data pipeline can be readily implemented.
 
 
 ## Documentation
 
 For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/).
+
+# Changelog
+
+
+## 0.1.4
+Added a timeout setting to all VISA instruments. 
+
+## 0.1.3
+First stable and working release
+
+## 0.1.0 to 0.1.2 
+&#9888; Broken releases due to minor bugs that were fixed in 0.1.3
```

### Comparing `nomad_camels-0.1.3/nomad_camels/CAMELS_start.py` & `nomad_camels-0.1.4/nomad_camels/CAMELS_start.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/MainApp_v2.py` & `nomad_camels-0.1.4/nomad_camels/MainApp_v2.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/EpicsFieldSignal.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/EpicsFieldSignal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/TriggerEpicsSignalRO.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/builder_helper_functions.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/builder_helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/custom_function_signal.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/custom_function_signal.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/evaluation_helper.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/evaluation_helper.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/helper_functions.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/helper_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -154,17 +154,17 @@
     w_init : float
         The initial set-value from where the algorithm should start.
     func_text : str
         This string is evaluated by the given evaluator to give the target
         function.
     evaluator : Evaluator
         Used to evaluate the read values.
-    set_channel :
+    set_channel : ophyd.Signal
         The channel wich is used for the optimization.
-    read_channels :
+    read_channels : list
         A list of all the channels which are read for the optimization.
     min_step : float
         The minimum step size.
     max_step : float
         The maximum step size.
     min_val : float
         The minimum value that should be given to the `set_channel`.
@@ -198,23 +198,21 @@
     """
 
     if set_channel not in read_channels:
         read_channels += [set_channel]
 
     def obj_func(set_val):
         """
+        This function sets the value and then reads the channels for each
+        iteration of the algorithm.
 
         Parameters
         ----------
-        set_val :
-            
-
-        Returns
-        -------
-
+        set_val : float
+            Value to be set on the set_channel
         """
         yield from bps.checkpoint()
         yield from bps.abs_set(set_channel, set_val, group='A')
         yield from bps.wait('A')
         yield from bps.trigger_and_read(read_channels, name=stream_name)
         # yield from bps.sleep(1)
 
@@ -281,39 +279,54 @@
             sort_w.pop(0)
     return w_history,f_history
 
 
 def get_range(evaluator, start, stop, points, min_val=np.nan, max_val=np.nan,
               loop_type='start - stop', sweep_mode='linear', endpoint=True):
     """
+    This is a helper function for steps like sweeps and the for loop.
+    Using the evaluator, it creates the range of iterations given the other
+    values.
 
     Parameters
     ----------
-    evaluator :
-        
-    start :
-        
-    stop :
-        
-    points :
-        
-    min_val :
+    evaluator : Evaluator
+        Used to evaluate the given expressions (`start`, `stop`, `points`,
+        `min_val`, `max_val`).
+    start : float, str
+        The starting position for the sweep / loop.
+    stop : float, str
+        The end position for the sweep / loop.
+    points : float, str
+        The number of points in the range. If using `min_val` / `max_val`,
+        `points` is the distance between those two.
+    min_val : float, str
          (Default value = np.nan)
-    max_val :
+         Minimum value of the loop / sweep. Usefull for hysteresis-sweeps.
+    max_val : float, str
          (Default value = np.nan)
-    loop_type :
+         Minimum value of the loop / sweep. Usefull for hysteresis-sweeps.
+    loop_type : str
          (Default value = 'start - stop')
-    sweep_mode :
+         Possible values: 'start - stop', ignoring `min_val` and `max_val`
+         'start - min - max - stop' going to minimum first, then maximum
+         'start - max - min - stop', or anything not-specified.
+    sweep_mode : str
          (Default value = 'linear')
-    endpoint :
+         The type how the distance between the points is calculated.
+         If 'linear', they are equidistant, if 'logarithmic', the points between
+         log(start) and log(stop) are equidistant, if 'exponential', between
+         exp(start) and exp(stop), otherwise they are equidistant between
+         1/start and 1/stop.
+    endpoint : bool
          (Default value = True)
-
+         Whether to include the endpoint into the range.
     Returns
     -------
-
+        An array of the calculated range.
     """
     start = evaluator.eval(start)
     stop = evaluator.eval(stop)
     points = evaluator.eval(points)
     min_val = evaluator.eval(min_val)
     max_val = evaluator.eval(max_val)
     if loop_type == 'start - stop':
@@ -331,31 +344,40 @@
         vals2 = get_inner_range(max_val, min_val, points, sweep_mode, endpoint)
         vals3 = get_inner_range(min_val, stop, part_points2, sweep_mode, endpoint)
     return np.concatenate([vals1, vals2, vals3])
 
 
 def get_inner_range(start, stop, points, sweep_mode, endpoint):
     """
+    Used for `get_range`, to make the split up ranges if doing a hysteresis
+    sweep.
 
     Parameters
     ----------
-    start :
-        
-    stop :
-        
-    points :
-        
-    sweep_mode :
-        
-    endpoint :
-        
+    start : float, str
+        The starting position for the sweep / loop.
+    stop : float, str
+        The end position for the sweep / loop.
+    points : float, str
+        The number of points in the range. If using `min_val` / `max_val`,
+        `points` is the distance between those two.
+    sweep_mode : str
+         (Default value = 'linear')
+         The type how the distance between the points is calculated.
+         If 'linear', they are equidistant, if 'logarithmic', the points between
+         log(start) and log(stop) are equidistant, if 'exponential', between
+         exp(start) and exp(stop), otherwise they are equidistant between
+         1/start and 1/stop.
+    endpoint : bool
+         (Default value = True)
+         Whether to include the endpoint into the range.
 
     Returns
     -------
-
+        An array of the calculated range.
     """
     if sweep_mode == 'linear':
         return np.linspace(start, stop, points, endpoint=endpoint)
     elif sweep_mode == 'logarithmic':
         start = np.log(start)
         stop = np.log(stop)
         return np.exp(np.linspace(start, stop, points, endpoint=endpoint))
@@ -363,15 +385,28 @@
         start = np.exp(start)
         stop = np.exp(stop)
         return np.log(np.linspace(start, stop, points, endpoint=endpoint))
     return 1/np.linspace(1/start, 1/stop, points, endpoint=endpoint)
 
 
 class Prompt_Box(QMessageBox):
-    """ """
+    """
+    A subclass of QMessageBox that is used in the prompt-step.
+    The protocol is paused until `self.done` is True.
+
+    Parameters
+    ----------
+    icon : str
+        If 'Error', the `QMessagebox.Critical` icon is desplayed, if 'Warning',
+        then `QMessagebox.Warning` is used, otherwise `QMessagebox.Information`.
+    text : str
+        The text to be displayed by the prompt.
+    title : str
+        The window-title of the prompt.
+    """
     def __init__(self, icon='', text='', title='', parent=None):
         super().__init__(parent=parent)
         if icon == 'Error':
             self.setIcon(QMessageBox.Critical)
         elif icon == 'Warning':
             self.setIcon(QMessageBox.Warning)
         else:
@@ -380,29 +415,52 @@
         self.setWindowTitle(title)
         self.helper = BoxHelper()
         self.helper.executor.connect(self.start_execution)
         self.buttonClicked.connect(self.set_done)
         self.done = False
 
     def set_done(self):
-        """ """
+        """Sets `self.done` to True."""
         self.done = True
 
     def start_execution(self):
-        """ """
+        """Sets `self.done` to False and starts `self.exec()`."""
         self.done = False
         self.exec()
 
 class BoxHelper(QWidget):
-    """ """
+    """Helper-class to start the execution of Prompts and other boxes from
+    within the protocol."""
     executor = Signal()
 
 
 class Value_Box(QDialog):
-    """ """
+    """
+    This dialog is used to set variables or channels at runtime of a protocol.
+
+    Parameters
+    ----------
+    text : str
+        A text to be displayed with the box.
+    title : str
+        The window title of the box.
+    variables : list, default: None
+        The variables that should be set by the user. A QLineEdit will be
+        provided for each of the variables.
+    channels : list, default: None
+        The channels that should be set by the user. A QLineEdit will be
+        provided for each of the channels.
+    free_variables : bool, default: False
+        Whether the user is allowed to freely set any variables.
+    free_channels : bool, default: False
+        Whether the user is allowed to freely set any channels.
+    devs : dict, default: None
+        Dictionary of the available devices. Only needed, if `free_channels` is
+        True, to provide the available channels.
+    """
     def __init__(self, text='', title='', variables=None, channels=None,
                  free_variables=False, free_channels=False, parent=None,
                  devs=None):
         super().__init__(parent)
         self.setWindowFlags(self.windowFlags() | Qt.WindowMaximizeButtonHint)
         text_label = QLabel(text)
         self.buttonBox = QDialogButtonBox(self)
@@ -474,20 +532,24 @@
         # self.table.sizechange.connect(self.adjustSize)
         self.adjustSize()
         self.was_accepted = False
         self.set_variables = {}
         self.set_channels = {}
 
     def start_execution(self):
-        """ """
+        """Sets `self.done` to False and starts `self.exec()`."""
         self.done = False
         self.exec()
 
     def accept(self) -> None:
-        """ """
+        """
+        Reads all the values to be set to channels / variables and saves them in
+        `self.set_channels` and `self.set_variables` respectively, then sets
+        `self.done` to True, allowing the protocol to go on and accepts the dialog.
+        """
         self.set_variables = {}
         self.set_channels = {}
         for i, v_box in enumerate(self.variable_boxes):
             val = v_box.text()
             if val:
                 self.set_variables[self.variables[i]] = val
         for i, c_box in enumerate(self.channel_boxes):
@@ -515,30 +577,38 @@
                     return
                 self.set_channels[channel] = channel_table_data['value'][i]
         self.was_accepted = True
         self.done = True
         return super().accept()
 
     def reject(self) -> None:
-        """ """
+        """
+        Sets `self.done` to True, allowing the protocol to go on before
+        rejecting the dialog.
+        """
         self.done = True
         return super().reject()
 
+
+
 def get_channels(dev):
-    """returns the components of an ophyd-device that are not listed in
-    the configuration
+    """
+    Goes through the components of the given ophyd device and returns all that
+    are not read-only and not config.
 
     Parameters
     ----------
-    dev :
-        
+    dev : ophyd.Device
+        The device that is checked for output channels.
 
     Returns
     -------
-
+    channels : dict
+        The keys are the channels in CAMELS-style. The values are
+        [dev.name, <name_of_the_component>].
     """
     channels = {}
     for comp in dev.walk_components():
         if issubclass(comp.item.cls, SignalRO):
             continue
         name = comp.item.attr
         if name not in dev.configuration_attrs:
```

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/make_catalog.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/make_catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+""""""
+
 import os
 import pathlib
 
 import databroker
 
 from nomad_camels.utility import load_save_functions, update_camels
 from nomad_camels.ui_widgets.warn_popup import WarnPopup
 
 def make_yml(datapath, catalog_name='CAMELS_CATALOG', ask_restart=False):
     """
+    Creates the yml file for the databroker (where it is looking for them) to
+    configure a simple catalog for measurements with CAMELS.
 
     Parameters
     ----------
-    datapath :
-        
-    catalog_name :
+    datapath : str, path
+        The path where the measurement data of the catalog should be saved to.
+    catalog_name : str
          (Default value = 'CAMELS_CATALOG')
-
-    Returns
-    -------
-
+         The name, the catalog should have.
     """
     catalog_path = databroker.catalog_search_path()[0]
     if not isinstance(datapath, pathlib.Path):
         datapath = pathlib.Path(datapath)
     if not isinstance(catalog_path, pathlib.Path):
         catalog_path = pathlib.Path(catalog_path)
     if not os.path.isdir(catalog_path):
```

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/protocol_builder.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/protocol_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,93 @@
+"""This module provides the functionalities needed for CAMELS to produce a
+running python script for its protocols.
+
+The overview of the protocol-file looks like this:\n
+- import sys
+- add path_to_camels, path_to_camels/nomad_camels, path to instruments to path
+- `standard_string`
+- `variable_string`
+- `device_import_string`
+- plot-string
+- outer protocol string (things like plots from single steps)
+- plan-string (including the inner plan, w/o start/stop and the outer)
+- add-main-string (protocol or step specific things that should be done in the main function)
+- `standard_run_string`
+- further metadata (user / sample, file)
+- `standard_start_string`
+- set up databroker and progress bar
+- `devices_string`
+- `standard_start_string2`
+- `standard_save_string`
+- `final_string`
+- `standard_start_string3`
+
+giving shortly:\n
+- imports/variables...
+- def protocol_plan_inner
+- def protocol_plan
+- def create_plots
+- def steps_add_main (plots of steps, etc.)
+- def uid_collector
+- def run_protocol_main
+- def main
+- if __name__ == "__main__"
+
+With the call chain as follows:\n
+- if --> main
+- main --> create_plots, steps_add_main, run_protocol_main
+- run_protocol_main --> uid_collector, protocol_plan
+- protocol_plan --> protocol_plan_inner
+"""
+
 import os.path
 import copy
 
-# from nomad_camels.main_classes.protocol_class import Measurement_Protocol
 import pathlib
 
-from nomad_camels.utility import variables_handling, device_handling, load_save_functions
+from nomad_camels.utility import variables_handling, load_save_functions
 
 from nomad_camels.bluesky_handling.builder_helper_functions import plot_creator
 
+
+# The default string in the beginning of the protocol including imports etc.
 standard_string = 'import numpy as np\n'
 standard_string += 'import importlib\n'
 standard_string += 'import bluesky\n'
 standard_string += 'import ophyd\n'
 standard_string += 'from bluesky import RunEngine\n'
 standard_string += 'from bluesky.callbacks.best_effort import BestEffortCallback\n'
 standard_string += 'import bluesky.plan_stubs as bps\n'
 standard_string += 'import databroker\n'
-# standard_string += 'from bluesky_widgets.qt.threading import wait_for_workers_to_quit\n'
 standard_string += 'from PySide6.QtWidgets import QApplication, QMessageBox\n'
 standard_string += 'from PySide6.QtCore import QCoreApplication, QThread\n'
-# standard_string += 'from epics import caput\n'
 standard_string += 'import datetime\n'
 standard_string += 'from nomad_camels.main_classes import plot_widget, list_plot, plot_2D\n'
 standard_string += 'from nomad_camels.utility.databroker_export import broker_to_hdf5, broker_to_dict, broker_to_NX\n'
 standard_string += 'from nomad_camels.utility import theme_changing\n'
 standard_string += 'from nomad_camels.bluesky_handling.evaluation_helper import Evaluator\n'
 standard_string += 'from nomad_camels.bluesky_handling import helper_functions\n'
-# standard_string += 'RE = RunEngine()\n'
 standard_string += 'darkmode = False\n'
 standard_string += 'theme = "default"\n'
 standard_string += 'protocol_step_information = {"protocol_step_counter": 0, "total_protocol_steps": 0, "protocol_stepper_signal": None}\n'
 
-# standard_run_string = '\n\neva = Evaluator(namespace=namespace)\n\n\n'
+
+# this string is used for collection of uids to later access the data
 standard_run_string = 'uids = []\n'
 standard_run_string += 'def uid_collector(name, doc):\n'
 standard_run_string += '\tuids.append(doc["uid"])\n\n\n'
 standard_run_string += 'def run_protocol_main(RE, dark=False, used_theme="default", catalog=None, devices=None, md=None):\n'
 standard_run_string += '\tdevs = devices or {}\n'
 standard_run_string += '\tmd = md or {}\n'
 standard_run_string += '\tglobal darkmode, theme, protocol_step_information\n'
 standard_run_string += '\tdarkmode, theme = dark, used_theme\n'
-# standard_run_string += '\tbec = BestEffortCallback()\n'
-# standard_run_string += '\tRE.subscribe(bec)\n'
 
+# this is the string with the main function of the protocol, starting everything
+# and also the if branch, whether it is the main script to execute everything
+# without importing
 standard_start_string = '\n\n\ndef main():\n'
 standard_start_string += '\tRE = RunEngine()\n'
 standard_start_string += '\tbec = BestEffortCallback()\n'
 standard_start_string += '\tRE.subscribe(bec)\n'
 standard_start_string2 = '\t\tplot_etc = create_plots(RE)\n'
 standard_start_string2 += '\t\tadditional_step_data = steps_add_main(RE, devs)\n'
 standard_start_string2 += '\t\trun_protocol_main(RE=RE, catalog=catalog, devices=devs, md=md)\n'
@@ -72,150 +113,174 @@
                        "/ENTRY[entry]/PROCESS[process]/version": 'metadata_start/version',
                        "/ENTRY[entry]/SAMPLE[sample]/measured_data": 'data'}
 
 
 def build_protocol(protocol, file_path,
                    save_path='test.h5', catalog='CAMELS_CATALOG', userdata=None,
                    sampledata=None):
-    """Creating the python file from a given `protocol`.
+    """Creating the runable python file from a given `protocol`.
 
     Parameters
     ----------
-    protocol :
-        
-    file_path :
-        
-    save_path :
+    protocol : main_classes.protocol_class.Measurement_Protocol
+        The protocol that provides the information for the python file.
+    file_path : str, path
+        The path, where the file should be saved.
+    save_path : str, path
          (Default value = 'test.h5')
-    catalog :
+         The path, where the data should be saved to.
+    catalog : str
          (Default value = 'CAMELS_CATALOG')
-    userdata :
+         The name of the databroker catalog that should be used.
+    userdata : dict, None
          (Default value = None)
-    sampledata :
+         Metadata that describes the user.
+    sampledata : dict, None
          (Default value = None)
-
-    Returns
-    -------
-
-    
+         Metadata that describes the sample.
     """
+    # first the path is prepared
     if not isinstance(save_path, pathlib.Path):
         save_path = pathlib.Path(save_path)
     if isinstance(save_path, pathlib.WindowsPath):
         save_path = save_path.as_posix()
+
+    # clearing leftovers from former builds
     variables_handling.read_channel_names.clear()
     variables_handling.read_channel_sets.clear()
+
+    # beginning of larger strings
     device_import_string = '\n'
     devices_string = '\t\tdevs = {}\n\t\tdevice_config = {}\n'
     variable_string = '\nnamespace = {}\n'
     variable_string += 'all_fits = {}\n'
     variable_string += 'plots = []\n'
     variable_string += 'boxes = {}\n'
     additional_string_devices = ''
     final_string = ''
+
+    # now all the variables of the protocol are added to the namespace
+    # this includes also the variables of steps such as a foor-loop
     for var, val in protocol.variables.items():
         if variables_handling.check_data_type(val) == 'String':
             val = f'"{val}"'
         if '(' in var or ')' in var:
             continue
         variable_string += f'{var} = {val}\n'
         variable_string += f'namespace["{var}"] = {var}\n'
     for var, val in protocol.loop_step_variables.items():
         if variables_handling.check_data_type(val) == 'String':
             val = f'"{val}"'
         if '(' in var or ')' in var:
             continue
         variable_string += f'{var} = {val}\n'
         variable_string += f'namespace["{var}"] = {var}\n'
+
+    # this handles all the used devices
     for dev in protocol.get_used_devices():
         device = variables_handling.devices[dev]
         classname = device.ophyd_class_name
         config = copy.deepcopy(device.get_config())
         settings = copy.deepcopy(device.get_settings())
         additional_info = copy.deepcopy(device.get_additional_info())
+        # informations on the connection is reshaped to be useful
         if 'connection' in settings:
             conn = settings.pop('connection')
             if 'type' in conn:
                 conn.pop('type')
             settings.update(conn)
         if 'idn' in settings:
             settings.pop('idn')
+
+        # the non_string settings are strings in the dictionary, but are a known
+        # variable or instance, so they are added without quotation marks
         extra_settings = {}
         non_strings = []
         for key in settings:
             if key.startswith('!non_string!_'):
                 extra_settings[key.replace('!non_string!_', '')] = settings[key]
                 non_strings.append(key)
         for s in non_strings:
             settings.pop(s)
+
+        # Information about the device is written into the protocol as well
         additional_info['device_class_name'] = classname
         if 'description' in additional_info:
             desc = additional_info['description'].replace('\n', '\n\t\t')
             devices_string += f'\t\t"""{dev} ({classname}):\n\t\t{desc}"""\n'
         devices_string += f'\t\tsettings = {settings}\n'
         devices_string += f'\t\tadditional_info = {additional_info}\n'
         devices_string += f'\t\t{dev} = {classname}("{dev}:", name="{dev}", '
         for key, value in extra_settings.items():
             devices_string += f'{key}={value}, '
         devices_string += '**settings)\n'
+
+        # the devices are being connected, then their config is called and
+        # written to the metadata
         devices_string += f'\t\tprint("connecting {dev}")\n'
         devices_string += f'\t\t{dev}.wait_for_connection()\n'
         devices_string += f'\t\tconfig = {config}\n'
         devices_string += f'\t\tconfigs = {dev}.configure(config)[1]\n'
         devices_string += f'\t\tdevice_config["{dev}"] = {{}}\n'
         devices_string += f'\t\tdevice_config["{dev}"].update(helper_functions.simplify_configs_dict(configs))\n'
         devices_string += f'\t\tdevice_config["{dev}"].update(settings)\n'
         devices_string += f'\t\tdevice_config["{dev}"].update(additional_info)\n'
         devices_string += f'\t\tdevs.update({{"{dev}": {dev}}})\n'
         device_import_string += f'from nomad_camels_driver_{device.name}.{device.name}_ophyd import {classname}\n'
         additional_string_devices += device.get_additional_string()
         final_string += device.get_finalize_steps()
+
+    # finishing up the device initialization
     devices_string += '\t\tprint("devices connected")\n'
     devices_string += f'\t\tmd = {{"devices": device_config, "description": "{protocol.description}"}}\n'
-    # devices_string += '\t\tmd.update({"program": "CAMELS", "version": "0.1"})\n'
-    # devices_string += '\t\tmd.update({"versions": {"NOMAD-CAMELS": "0.1", "EPICS": "7.0.6.2", "bluesky": bluesky.__version__, "ophyd": ophyd.__version__}})\n'
+
+    # if using special nexus-format, some restructuring of metadata is done
     if protocol.use_nexus:
         md_dict = {}
         for i, name in enumerate(protocol.metadata['Name']):
             md_dict[name] = protocol.metadata['Value'][i]
         devices_string += f'\t\tmd.update({md_dict})\n'
+
+    # the plots are created
     plot_string, plotting = plot_creator(protocol.plots, multi_stream=True)
-    # for device in protocol.get_used_devices():
-    #     print(device)
+
+    # everything is put together for the complete protocol-string
     protocol_string = 'import sys\n'
     protocol_string += f'sys.path.append(r"{os.path.dirname(variables_handling.CAMELS_path)}")\n'
     protocol_string += f'sys.path.append(r"{os.path.dirname(variables_handling.CAMELS_path)}/nomad_camels")\n'
     protocol_string += f'sys.path.append(r"{variables_handling.device_driver_path}")\n\n'
     protocol_string += standard_string
     protocol_string += f'{variable_string}\n\n'
     protocol_string += device_import_string
     protocol_string += protocol.get_outer_string()
     protocol_string += protocol.get_plan_string()
     protocol_string += plot_string
     protocol_string += protocol.get_add_main_string()
     protocol_string += standard_run_string
+
+    # setting up the progress bar
     protocol_string += f'\tprotocol_step_information["total_protocol_steps"] = {protocol.get_total_steps()}\n'
-    # protocol_string += '\ttry:\n'
-    # protocol_string += '\tRE.subscribe(eva)\n\n'
-    # protocol_string += devices_string
     protocol_string += additional_string_devices
-    # if plotting:
-    #     protocol_string += '\t\tplot_etc = create_plots(RE)\n'
+
+    # add user / sample to metadata
     sampledata = sampledata or {'name': 'default_sample'}
     userdata = userdata or {'name': 'default_user'}
     protocol_string += user_sample_string(userdata, sampledata)
     protocol_string += f'\tmd["protocol_overview"] = "{protocol.get_short_string().encode("unicode_escape").decode()}"\n'
+
+    # reading the file itself and adding it to the metadata
     protocol_string += '\twith open(__file__, "r", encoding="utf-8") as f:\n'
     protocol_string += '\t\tmd["python_script"] = f.read()\n'
     protocol_string += '\tmd["variables"] = namespace\n'
+
+    # adding uid to RunEngine, calling the plan
     protocol_string += '\tRE.subscribe(uid_collector, "start")\n'
-    # protocol_string += '\ttry:\n'
     protocol_string += f'\tRE({protocol.name}_plan(devs, md=md, runEngine=RE))\n'
-    # protocol_string += '\tfinally:\n'
-    # protocol_string += final_string or '\t\tpass\n'
+
+    # wait for RunEngine to finish, then save the data
     standard_save_string = '\tfinally:\n'
     standard_save_string += '\t\twhile RE.state not in ["idle", "panicked"]:\n'
     standard_save_string += '\t\t\timport time\n'
     standard_save_string += '\t\t\ttime.sleep(0.5)\n'
     standard_save_string += '\t\tif uids:\n'
     standard_save_string += '\t\t\truns = catalog[tuple(uids)]\n'
     if protocol.use_nexus:
@@ -226,56 +291,65 @@
         # TODO finish this
     else:
         standard_save_string += f'\t\t\tbroker_to_NX(runs, "{save_path}", plots,' \
                                 f'session_name="{protocol.session_name}",' \
                                 f'export_to_csv={protocol.export_csv},' \
                                 f'export_to_json={protocol.export_json})\n\n\n'
 
-    # protocol_string += standard_save_string
     protocol_string += standard_start_string
+
+    # checking for databroker catalog, using temp if not available
     protocol_string += '\ttry:\n'
     protocol_string += f'\t\tcatalog = databroker.catalog["{catalog}"]\n'
     protocol_string += '\texcept KeyError:\n'
     protocol_string += '\t\timport warnings\n'
     protocol_string += '\t\twarnings.warn("Could not find databroker catalog, using temporary catalog. If data is not transferred, it might get lost.")\n'
     protocol_string += '\t\tcatalog = databroker.temp().v2\n'
     protocol_string += '\tRE.subscribe(catalog.v1.insert)\n\n'
+
+    # progress bar setup
     protocol_string += '\tfrom nomad_camels.utility import tqdm_progress_bar\n'
     protocol_string += f'\ttqdm_bar = tqdm_progress_bar.ProgressBar({protocol.get_total_steps()})\n\n'
     protocol_string += '\tprotocol_step_information["protocol_stepper_signal"] = tqdm_bar\n'
+
+    # all the devices and the actual run are in a try-block
     protocol_string += '\ttry:\n'
     protocol_string += devices_string
     protocol_string += standard_start_string2
     # protocol_string += '\tfinally:\n'
     protocol_string += standard_save_string
     protocol_string += final_string
     protocol_string += standard_start_string3
+
+    # the string is written to the file
     if not os.path.isdir(os.path.dirname(file_path)):
         os.makedirs(os.path.dirname(file_path))
     with open(file_path, 'w', encoding='utf-8') as file:
         file.write(protocol_string)
+
+    # the protocol is converted to a dictionary and saved as a json
     protocol_dict = load_save_functions.get_save_str(protocol)
     if not isinstance(file_path, pathlib.Path):
         file_path = pathlib.Path(file_path)
     load_save_functions.save_dictionary(file_path.with_suffix('.cprot'),
                                         protocol_dict)
 
 
 
 def user_sample_string(userdata, sampledata):
     """Returns the string adding userdata and sampledata to the md.
 
     Parameters
     ----------
-    userdata :
-        
-    sampledata :
-        
-
+    userdata : dict
+        data on the user
+    sampledata : dict
+        data on the sample
     Returns
     -------
-
+    u_s_string : str
+        the string containing the data and adding it to the metadata
     """
     u_s_string = f'\tmd["user"] = {userdata}\n'
     u_s_string += f'\tmd["sample"] = {sampledata}\n'
     return u_s_string
```

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/special_plan_stubs.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/special_plan_stubs.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 def trigger_and_read_devices(devices, name='primary'):
     """A wrapper for the plan stup `trigger_and_read` that implements
     trigger/read for a device with several components by simply splitting
     up the device and using a list of its components.
 
     Parameters
     ----------
-    devices :
-        
-    name :
-         (Default value = 'primary')
-
-    Returns
-    -------
-
+    devices : list[ophyd.Device]
+        List of the devices that should be triggered and read
+    name : str
+        (Default value = 'primary')
+        Name of the stream where to save the data
     """
     split_devices = []
     for dev in devices:
         if isinstance(dev, Device):
             dev.read()
             for _, component in dev._get_components_of_kind(Kind.normal):
                 split_devices.append(component)
```

### Comparing `nomad_camels-0.1.3/nomad_camels/bluesky_handling/visa_signal.py` & `nomad_camels-0.1.4/nomad_camels/bluesky_handling/visa_signal.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import pyvisa
 import re
 
 rm = pyvisa.ResourceManager()
 open_resources = {}
 
 def list_resources():
-    """ """
+    """Gives the results of `ResourceManager.list_resources`."""
     return rm.list_resources()
 
 def close_resources():
-    """ """
+    """Goes throug all the opened resources and closes them."""
     for res in open_resources:
         open_resources[res].close()
     open_resources.clear()
 
 class VISA_Signal(Signal):
     """ """
     def __init__(self,  name, value=0., timestamp=None, parent=None,
@@ -60,53 +60,35 @@
         elif parse_return_type == 'bool':
             self.parse_return_type = bool
         else:
             self.parse_return_type = parse_return_type
 
     def change_instrument(self, resource_name):
         """
+        Changes the visa_instrument to the one with the given `resource_name`.
 
         Parameters
         ----------
-        resource_name :
-            
-
-        Returns
-        -------
-
+        resource_name : str
+            Name of the new instrument to be used.
         """
         if resource_name:
             if resource_name in open_resources:
                 self.visa_instrument = open_resources[resource_name]
             else:
                 self.visa_instrument = rm.open_resource(resource_name)
                 open_resources[resource_name] = self.visa_instrument
 
     def put(self, value, *, timestamp=None, force=False, metadata=None,
             **kwargs):
         """
-
-        Parameters
-        ----------
-        value :
-            
-        * :
-            
-        timestamp :
-             (Default value = None)
-        force :
-             (Default value = False)
-        metadata :
-             (Default value = None)
-        **kwargs :
-            
-
-        Returns
-        -------
-
+        Overwrites `ophyd.Signal.put`. The value is converted to a string, using
+        `self.write`. If `self.parse` is not None, a query instead of a simple
+        write is being performed, in that case, the value given to super().put
+        is the returned value from the query.
         """
         if not self.write:
             write_text = str(value)
         elif isinstance(self.write, str):
             write_text = self.write.format(value=value)
         else:
             write_text = self.write(value)
@@ -126,15 +108,15 @@
                 except:
                     value = val
         else:
             self.visa_instrument.write(write_text)
         super().put(value, timestamp=timestamp, force=force, metadata=metadata, **kwargs)
 
     def describe(self):
-        """ """
+        """Adding "VISA" as the source for the description."""
         info = super().describe()
         info[self.name]['source'] = 'VISA'
         # info[self.name].update(self.metadata)
         return info
 
 
 
@@ -174,15 +156,19 @@
             self.parse_return_type = int
         elif parse_return_type == 'bool':
             self.parse_return_type = bool
         else:
             self.parse_return_type = parse_return_type
 
     def get(self):
-        """ """
+        """
+        Overwrites `ophyd.SignalRO.get`, performing a query to the instrument.
+        The returned string is parsed regarding `self.parse` and converted to
+        the datatype specified by `self.parse_return_type`.
+        """
         while self.visa_instrument.currently_reading:
             time.sleep(0.1)
         self.visa_instrument.currently_reading = True
         if isinstance(self.query, str):
             val = self.visa_instrument.query(self.query)
         else:
             val = self.visa_instrument.query(self.query())
@@ -200,65 +186,57 @@
                 val = self.parse_return_type(val)
             except:
                 val = val
         self._readback = val
         return super().get()
 
     def describe(self):
-        """ """
+        """Adding "VISA" as the source for the description."""
         info = super().describe()
         info[self.name]['source'] = 'VISA'
         # info[self.name].update(self.metadata)
         return info
 
 
 
 class VISA_Device(Device):
-    """Subclasses ophyd's `Device` class. Automatically opens the specified VISA
-     resource."""
+    """
+    Subclasses ophyd's `Device` class. Automatically opens the specified VISA
+    resource.
+
+    Parameters
+    ----------
+    resource_name : str
+        The name of the VISA-resource.
+    read_termination : str
+        (Default = '\\r\\n')
+        The line termination for reading from the instrument.
+    write_termination : str
+        (Default = '\\r\\n')
+        The line termination for writing to the instrument.
+    baud_rate : int
+        (Default = 9600)
+        The communication baud rate.
+    """
     def __init__(self, prefix='', *, name, kind=None, read_attrs=None,
                  configuration_attrs=None, parent=None, resource_name='',
                  read_termination='\r\n', write_termination='\r\n',
-                 baud_rate=9600, **kwargs):
-        """
-        Parameters
-        ----------
-        resource_name : str
-            The name of the VISA-resource.
-
-        read_termination : str
-            The line termination for reading from the instrument.
-            (Default = '\r\n')
-
-        write_termination : str
-            The line termination for writing to the instrument.
-            (Default = '\r\n')
-
-        baud_rate : int
-            The communication baud rate. (Default = 9600)
-        """
+                 baud_rate=9600, timeout=2000, **kwargs):
         super().__init__(prefix=prefix, name=name, kind=kind, read_attrs=read_attrs,
                          configuration_attrs=configuration_attrs, parent=parent, **kwargs)
         self.visa_instrument = None
         if resource_name:
             if resource_name in open_resources:
                 self.visa_instrument = open_resources[resource_name]
             else:
                 self.visa_instrument = rm.open_resource(resource_name)
                 open_resources[resource_name] = self.visa_instrument
             self.visa_instrument.write_termination = write_termination
             self.visa_instrument.read_termination = read_termination
             self.visa_instrument.baud_rate = baud_rate
             self.visa_instrument.currently_reading = False
+            self.visa_instrument.timeout = timeout
 
         for comp in self.walk_signals():
             it = comp.item
             it.visa_instrument = self.visa_instrument
 
-
-
-# if __name__ == '__main__':
-#     print(list_resources())
-#     tester = 'USB0::0x0957::0x8E18::MY51140626::INSTR'
-#     # testsig = VISA_Signal_Write('testsig', write_termination='\r\n', resource_name=tester)
-#     testsigR = VISA_Signal_Read('testsigR', read_termination='\r\n', write_termination='\r\n', resource_name=tester, query_text='MEAS:VOLT:DC?')
-#     print(testsigR.get())
```

### Comparing `nomad_camels-0.1.3/nomad_camels/commands/change_sequence.py` & `nomad_camels-0.1.4/nomad_camels/commands/change_sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,46 @@
 from PySide6.QtCore import QItemSelectionModel
 from PySide6.QtGui import QUndoCommand
 
 class CommandMoveStep(QUndoCommand):
-    """ """
+    """
+    Using a command for moving a step inside the protocol treeView to be able to
+    reverse the action.
+
+    Parameters
+    ----------
+    treeView : QTreeView
+        The TreeView displaying the protocol sequence
+    item_model : QStandardItemModel
+        The treeview's item model
+    up_down : int
+        The direction in which to move the step, if positive it moves down, if
+        negative it moves up.
+    in_out : int
+        The step is moved into the step above it, if positive, if negative it is
+        moved out one layer.
+    loop_step_dict : dict
+        The dictionary of the loopsteps, used to find the parent steps
+    update_func : function
+        This function is called, when the command is finished, usually used to
+        update the order of the steps in the protocol data.
+    """
     def __init__(self, treeView, item_model, up_down, in_out, loop_step_dict, update_func):
         super().__init__()
         self.treeView_protocol_sequence = treeView
         self.item_model_sequence = item_model
         self.up_down = up_down
         self.in_out = in_out
         self.loop_step_dict = loop_step_dict
         self.ind = self.treeView_protocol_sequence.selectedIndexes()[0]
         self.item = self.item_model_sequence.itemFromIndex(self.ind)
         self.update_func = update_func
 
     def redo(self):
-        """ """
+        """Performs moving the step."""
         parent = self.item.parent()
         if parent is None:
             if self.up_down != 0 and (self.ind.row() > 0 or self.up_down > 0) and (self.ind.row() < self.item_model_sequence.rowCount()-1 or self.up_down < 0):
                 row = self.item_model_sequence.takeRow(self.ind.row())
                 self.item_model_sequence.insertRow(self.ind.row() + self.up_down, row)
             elif self.in_out > 0 and self.ind.row() > 0:
                 above = self.item_model_sequence.item(self.ind.row()-1, 0)
@@ -47,15 +68,15 @@
                 grandparent.insertRow(parent_row+1, row)
         self.treeView_protocol_sequence.clearSelection()
         new_ind = self.item_model_sequence.indexFromItem(self.item)
         self.treeView_protocol_sequence.selectionModel().select(new_ind, QItemSelectionModel.Select)
         self.update_func()
 
     def undo(self):
-        """ """
+        """Moves the step back to its original position."""
         parent = self.item.parent()
         up_down = - self.up_down
         in_out = - self.in_out
         ind = self.item_model_sequence.indexFromItem(self.item)
         if parent is None:
             if up_down != 0 and (ind.row() > 0 or up_down > 0) and (ind.row() < self.item_model_sequence.rowCount()-1 or up_down < 0):
                 row = self.item_model_sequence.takeRow(ind.row())
```

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/device_add_dialog.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/device_add_dialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/helper_panels/enterTextDialog.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/helper_panels/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/instrument_config.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/instrument_installer.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/instrument_installer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/manage_instruments.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/manage_instruments.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/plot_definer.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/protocol_config.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/protocol_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/frontpanels/settings_window.py` & `nomad_camels-0.1.4/nomad_camels/frontpanels/settings_window.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/CAMELS.ico` & `nomad_camels-0.1.4/nomad_camels/graphics/CAMELS.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/CAMELS_Icon.png` & `nomad_camels-0.1.4/nomad_camels/graphics/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3` & `nomad_camels-0.1.4/nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav` & `nomad_camels-0.1.4/nomad_camels/graphics/Camel-Groan-2-QuickSounds.com.wav`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/camels-horizontal.svg` & `nomad_camels-0.1.4/nomad_camels/graphics/camels-horizontal.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/camels-vertical.svg` & `nomad_camels-0.1.4/nomad_camels/graphics/camels-vertical.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/camels_horizontal.png` & `nomad_camels-0.1.4/nomad_camels/graphics/camels_horizontal.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/camels_vertical.png` & `nomad_camels-0.1.4/nomad_camels/graphics/camels_vertical.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/dark.qss` & `nomad_camels-0.1.4/nomad_camels/graphics/dark.qss`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS.svg` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Icon.png` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v1.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Icon_v2.ico`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Logo.png` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Logo.svg` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_Logo_v1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_V1.svg` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_V1.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/CAMELS_v2.svg` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/CAMELS_v2.svg`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/camels - Kopie.png` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels - Kopie.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/camels_free.png` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/camels_free.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/graphics/legacy/plus_sign.png` & `nomad_camels-0.1.4/nomad_camels/graphics/legacy/plus_sign.png`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/addDeviceDialog.py` & `nomad_camels-0.1.4/nomad_camels/gui/addDeviceDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/device_installer.py` & `nomad_camels-0.1.4/nomad_camels/gui/device_installer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/enterTextDialog.py` & `nomad_camels-0.1.4/nomad_camels/gui/enterTextDialog.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/fit_definer.py` & `nomad_camels-0.1.4/nomad_camels/gui/fit_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/for_loop.py` & `nomad_camels-0.1.4/nomad_camels/gui/for_loop.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/general_protocol_settings.py` & `nomad_camels-0.1.4/nomad_camels/gui/general_protocol_settings.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/gradient_descent_step.py` & `nomad_camels-0.1.4/nomad_camels/gui/gradient_descent_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/instrument_config.py` & `nomad_camels-0.1.4/nomad_camels/gui/instrument_config.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/mainWindow_v2.py` & `nomad_camels-0.1.4/nomad_camels/gui/mainWindow_v2.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/pass_ask.py` & `nomad_camels-0.1.4/nomad_camels/gui/pass_ask.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/plot_definer.py` & `nomad_camels-0.1.4/nomad_camels/gui/plot_definer.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/plot_definer_2d.py` & `nomad_camels-0.1.4/nomad_camels/gui/plot_definer_2d.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/plot_options.py` & `nomad_camels-0.1.4/nomad_camels/gui/plot_options.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/protocol_view.py` & `nomad_camels-0.1.4/nomad_camels/gui/protocol_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/read_channels.py` & `nomad_camels-0.1.4/nomad_camels/gui/read_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/set_channels.py` & `nomad_camels-0.1.4/nomad_camels/gui/set_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/gui/settings_window.py` & `nomad_camels-0.1.4/nomad_camels/gui/settings_window.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/change_device_config.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/change_device_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,65 +3,57 @@
 
 from nomad_camels.main_classes.loop_step import Loop_Step, Loop_Step_Config
 from nomad_camels.main_classes.device_class import Device_Config_Sub
 
 from nomad_camels.utility import variables_handling
 
 class Change_DeviceConf(Loop_Step):
-    """ """
+    """
+    With this step, one can change the config-attributes of a device.
+
+    Attributes
+    ----------
+    device : str
+        The name of the device that has the config changed.
+    config_dict : dict
+        The dictionary with the new config-attributes of the device.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step, step_info, **kwargs)
         self.step_type = 'Change Device Config'
         if step_info is None:
             step_info = {}
         self.device = step_info['device'] if 'device' in step_info else ''
         self.config_dict = step_info['config_dict'] if 'config_dict' in step_info else {}
         self.settings_dict = step_info['settings_dict'] if 'settings_dict' in step_info else {}
 
     def update_used_devices(self):
-        """ """
+        """Includes self.device to the used devices."""
         self.used_devices = [self.device]
 
     def get_protocol_string(self, n_tabs=1):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """Creates an instance of `self.device` and uses `self.config_dict` to
+        get a complete config_dict from the instance.
+        The string consists of calling `dev.configure(config)`, where config is
+        the config_dict."""
         tabs = '\t' * n_tabs
         dev_name = self.device
         device = variables_handling.devices[dev_name]
         dev_type = device.name
         py_package = importlib.import_module(f'nomad_camels_driver_{dev_type}.{dev_type}')
         dev_instance = py_package.subclass()
         dev_instance.config = self.config_dict
         config_dict = dev_instance.get_config()
         protocol_string = super().get_protocol_string(n_tabs)
         protocol_string += f'{tabs}config = {config_dict}\n'
         protocol_string += f'{tabs}devs["{self.device}"].configure(config)\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """Includes the configured device in the short string."""
         short_string = super().get_protocol_short_string(n_tabs)
         short_string = f'{short_string[:-1]} - {self.device}\n'
         return short_string
 
 
 class Change_DeviceConf_Config(Loop_Step_Config):
     """ """
```

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/for_while_loops.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/for_while_loops.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 from nomad_camels.gui.for_loop import Ui_for_loop_config
 
 class While_Loop_Step(Loop_Step_Container):
     """A loopstep that adds a simple While Loop with a condition, that
     may be just written as python-code.
 
-    Parameters
-    ----------
-
-    Returns
-    -------
-
     Attributes
     ----------
     condition : str
-        The condition which is used for the loop
+        The condition which is used for the loop. It should be interpretable
+        python-code within the namespace of the protocol.
+    expected_iterations : int, default 1
+        The expected number of iterations, used for the steps time weight for
+        the progress bar. Ideally rather too large than to small (otherwise the
+        progress bar reaches 100% too early).
     """
     def __init__(self, name='', children=None, parent_step=None, step_info=None,
                  **kwargs):
         super().__init__(name, children, parent_step, step_info, **kwargs)
         self.step_type = 'While Loop'
         if step_info is None:
             step_info = {}
@@ -41,42 +40,34 @@
                 raise Exception('Variable already defined!')
         variables_handling.loop_step_variables.update(variables)
         super().update_variables()
 
     def get_protocol_string(self, n_tabs=1):
         """The string consists of declaring the count-variable. Then the
         while loop with the desired condition is started. After all the
-        children-steps, the count-variable increased by 1.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        children-steps, the count-variable increased by 1."""
         self.update_time_weight()
         tabs = '\t'*n_tabs
         count_var = f'{self.name.replace(" ", "_")}_Count'
         protocol_string = super().get_protocol_string(n_tabs)
         protocol_string += f'{tabs}{count_var} = 0\n'
         protocol_string += f'{tabs}while eva.eval("{self.condition}"):\n'
         protocol_string += f'{tabs}\tnamespace["{count_var}"] = {count_var}\n'
         protocol_string += self.get_children_strings(n_tabs+1)
         protocol_string += f'{tabs}\t{count_var} += 1\n'
         return protocol_string
 
     def update_time_weight(self):
-        """ """
+        """Multiplies the time_weight of the children with the expected
+        iterations + 5"""
         super().update_time_weight()
         self.time_weight *= self.expected_interations + 5
 
     def get_protocol_short_string(self, n_tabs=0):
+        """Adds the condition to the string"""
         tabs = '\t' * n_tabs
         short_string = f'{tabs}while {self.condition}:\n'
         for child in self.children:
             short_string += child.get_protocol_short_string(n_tabs+1)
         return short_string
 
 
@@ -128,20 +119,14 @@
             pass
 
 
 class For_Loop_Step(Loop_Step_Container):
     """Loop_Step representing a For Loop. It offers several ways of
     defining the sweep.
 
-    Parameters
-    ----------
-
-    Returns
-    -------
-
     Attributes
     ----------
     loop_type : str
         can be one of the following:
         - "start - stop" the loop goes from `min_val` to `max_val`
         - "start - min - max - stop" or "start - max - min - stop" goes from start over min/max, max/min to stop
         - "Value-List" the loop uses the values inside `val_list`
@@ -202,25 +187,16 @@
         for variable in variables:
             if variable in variables_handling.loop_step_variables:
                 raise Exception('Variable already defined!')
         variables_handling.loop_step_variables.update(variables)
         super().update_variables()
 
     def get_protocol_string(self, n_tabs=1):
-        """The loop is enumerating over the selected points.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """The loop is enumerating over the selected points. When using a range,
+        the get_range helper function is used."""
         tabs = '\t'*n_tabs
         if self.loop_type in ['start - stop', 'start - min - max - stop',
                               'start - max - min - stop']:
             enumerator = f'helper_functions.get_range(eva, "{self.start_val}", "{self.stop_val}", "{self.n_points}", "{self.min_val or np.nan}", "{self.max_val or np.nan}", "{self.loop_type}", "{self.sweep_mode}", "{self.include_end_points}")'
             # enumerator = get_space_string(self.start_val, self.stop_val,
             #                               self.n_points, self.min_val,
             #                               self.max_val, self.loop_type,
@@ -234,19 +210,21 @@
         protocol_string += f'{tabs}for {self.name.replace(" ", "_")}_Count, {self.name.replace(" ", "_")}_Value in enumerate({enumerator}):\n'
         protocol_string += f'{tabs}\tnamespace.update({{"{self.name.replace(" ", "_")}_Count": {self.name.replace(" ", "_")}_Count, "{self.name.replace(" ", "_")}_Value": {self.name.replace(" ", "_")}_Value}})\n'
         protocol_string += self.get_children_strings(n_tabs+1)
         self.update_time_weight()
         return protocol_string
 
     def update_time_weight(self):
-        """ """
+        """Multiplies the childrens time_weight (-1 for the step itself) by the
+        number of iterations and adds 1 (for the step itself)."""
         super().update_time_weight()
         self.time_weight = (self.time_weight - 1) * self.n_iterations + 1
 
     def get_protocol_short_string(self, n_tabs=0):
+        """Shows the type of loop and the range in the short string as well"""
         tabs = '\t' * n_tabs
         if self.loop_type == 'Value-List':
             vals = self.val_list
         elif self.loop_type in ['start - stop', 'start - min - max - stop',
                                 'start - max - min - stop']:
             vals = f'(start: {self.start_val}, stop: {self.stop_val}, '
             if 'max' in self.loop_type:
```

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/if_step.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/if_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,70 +8,45 @@
 from nomad_camels.ui_widgets.add_remove_table import AddRemoveTable
 
 
 class If_Loop_Step(Loop_Step_Container):
     """A loopstep providing an if-case selection with a variable number
     of `elif`.
 
-    Parameters
-    ----------
-
-    Returns
-    -------
-
     Attributes
     ----------
     condition : str
-        The condition which is used for the if-conditional
+        The condition which is used for the if-conditional (should be valid
+        python code)
     use_else : bool
         whether to add an `else`-case
     elifs : list of str
-        string-list of the conditions for a variable number of `elif`
+        string-list of the conditions for a variable number of `elif` cases
     """
     def __init__(self, name='', children=None, parent_step=None, step_info=None,
                  **kwargs):
         super().__init__(name, children, parent_step, step_info, **kwargs)
         self.step_type = 'If'
         self.has_children = False
         if step_info is None:
             step_info = {}
         self.condition = step_info['condition'] if 'condition' in step_info else '!'
         self.use_else = step_info['use_else'] if 'use_else' in step_info else False
         self.elifs = step_info['elifs'] if 'elifs' in step_info else []
         self.update_children()
 
     def append_to_model(self, item_model:QStandardItemModel, parent=None):
-        """Overwritten, so that nothing can be dropped into the main step.
-
-        Parameters
-        ----------
-        item_model:QStandardItemModel :
-            
-        parent :
-             (Default value = None)
-
-        Returns
-        -------
-
-        """
+        """Overwritten, so that nothing can be dropped into the main step."""
         item = super(If_Loop_Step, self).append_to_model(item_model, parent)
         item.setDropEnabled(False)
         return item
 
     def update_children(self):
         """Updates the if-substeps provided by this step, giving them
-        the names corresponding to the conditions.
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-
-        """
+        the names corresponding to the conditions."""
         if not self.children:
             self.children.append(If_Sub_Step(f'{self.name}_{self.condition}'))
         n_children = 1 + len(self.elifs) + (1 if self.use_else else 0)
         if self.use_else and not isinstance(self.children[-1], Else_Sub_Step):
             self.children.append(Else_Sub_Step(f'{self.name}_Else'))
         elif not self.use_else and isinstance(self.children[-1], Else_Sub_Step):
             self.children.pop()
@@ -96,50 +71,30 @@
                                          Elif_Sub_Step(f'{self.name}_{cond}'))
                 else:
                     self.children.append(Elif_Sub_Step(f'{self.name}_{cond}'))
         elif diff < 0:
             raise Exception('something went wrong with if-children!')
 
     def get_protocol_string(self, n_tabs=1):
-        """Putting together the children of all if-substeps.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
-        """
+        """Putting together the children of all if-substeps and the conditions"""
         tabs = '\t' * n_tabs
         protocol_string = super().get_protocol_string(n_tabs)
         protocol_string += f'{tabs}if eva.eval("{self.condition}"):\n'
         protocol_string += self.children[0].get_children_strings(n_tabs+1)
         for i, el in enumerate(self.elifs):
             child = self.children[i+1]
             protocol_string += f'{tabs}elif eva.eval("{el}"):\n'
             protocol_string += child.get_children_strings(n_tabs+1)
         if self.use_else:
             protocol_string += f'{tabs}else:\n'
             protocol_string += self.children[-1].get_children_strings(n_tabs+1)
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """Shows all the conditions and the steps' children"""
         tabs = '\t' * n_tabs
         short_string = f'{tabs}if {self.condition}:\n'
         for child in self.children[0].children:
             short_string += child.get_protocol_short_string(n_tabs+1)
         for i, el in enumerate(self.elifs):
             short_string += f'{tabs}else if {el}:\n'
             for child in self.children[i+1].children:
@@ -158,27 +113,16 @@
     """Simple sub-step that represents the if-condition."""
     def __init__(self, name='', children=None, parent_step=None, step_info=None,
                  **kwargs):
         super().__init__(name, children, parent_step, step_info, **kwargs)
         self.step_type = 'If_Sub'
 
     def append_to_model(self, item_model:QStandardItemModel, parent=None):
-        """Overwritten, so that nothing can be dropped into the main step.
-
-        Parameters
-        ----------
-        item_model:QStandardItemModel :
-            
-        parent :
-             (Default value = None)
-
-        Returns
-        -------
-
-        """
+        """Overwritten, so that nothing can be dropped into the main step. The
+        Sub-Step cannot be dragged out from the main step."""
         item = super().append_to_model(item_model, parent)
         item.setDragEnabled(False)
         item.setEnabled(False)
         return item
 
 class Elif_Sub_Step(If_Sub_Step):
     """Simple sub-step that represents an elif-condition."""
```

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/make_step_of_type.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/make_step_of_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""This module provides a way to produce all possible protocol steps from the UI"""
+
 from nomad_camels.main_classes.loop_step import Loop_Step
 from nomad_camels.loop_steps import for_while_loops, read_channels, set_channels,\
     wait_loop_step, if_step, prompt_loop_step, run_subprotocol, simple_sweep,\
     gradient_descent, change_device_config, nd_sweep, set_variables, set_value_popup
 
 from nomad_camels.utility import variables_handling
 
@@ -39,44 +41,46 @@
                 'Else_Sub': [if_step.Else_Sub_Step, if_step.Sub_Step_Config]}
 
 
 def get_device_steps():
     """Goes through all the devices and checks, whether they provide
     their own types of loop-steps.
 
-    Parameters
-    ----------
-
     Returns
     -------
-
+    device_steps
+        dictionary of the possible steps provided by the devices
     """
     device_steps = {}
     for devname, device in sorted(variables_handling.devices.items(), key=lambda x: x[0].lower()):
         device_steps.update(device.get_special_steps())
     return device_steps
 
 
 def make_step(step_type, step_info=None, children=None):
     """Checks whether the given `step_type` is supported, if yes, then a
-    step of that type with the given info and children will be created,
-    otherwise a new step is made.
+    step of that type with the given info and children will be created.
+    If there is no step_info, a new step is made.
 
     Parameters
     ----------
-    step_type :
-        
-    step_info :
-         (Default value = None)
-    children :
-         (Default value = None)
+    step_type : str
+        A string representing the type of the step. Should correspond to one of
+        the keys of `step_type_config` or a device specific step.
+    step_info : dict, None
+        (Default value = None)
+        The information for the step's configuration
+    children : list[Loop_Step], None
+        (Default value = None)
+        The produced step's children. Handed over to it's constructor.
 
     Returns
     -------
-
+    step
+        The produced step.
     """
     dev_steps = get_device_steps()
     if step_type in step_type_config:
         if step_info is None:
             name = step_type.replace(' ', '_')
         else:
             name = step_info['name']
@@ -96,20 +100,21 @@
     return Loop_Step(name='fail')
 
 def get_config(step:Loop_Step):
     """Returns the Loop_Step_Config belonging to the given step.
 
     Parameters
     ----------
-    step:Loop_Step :
-        
+    step : Loop_Step
+        The step for which the config-widget should be opened.
 
     Returns
     -------
-
+    step_config
+        The Loop_Step_Config corresponding to the given `step`.
     """
     step_type = step.step_type
     dev_steps = get_device_steps()
     if step_type in step_type_config:
         return step_type_config[step_type][1](loop_step=step)
     elif step_type in dev_steps:
         return dev_steps[step_type][1](loop_step=step)
```

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/nd_sweep.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/nd_sweep.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,50 +10,67 @@
 from nomad_camels.frontpanels.plot_definer import Plot_Button_Overview
 
 from nomad_camels.loop_steps.for_while_loops import For_Loop_Step_Config_Sub, For_Loop_Step
 
 
 
 class ND_Sweep(Loop_Step):
-    """ """
+    """
+    An n-dimensional sweep with the read values. Usefull for e.g. an xy-scan.
+
+    Attributes
+    ----------
+    sweep_channels : list[str]
+        From outer to inner sweep, the names of the channels that should be
+        sweeped through.
+    data_output : str
+        Whether the data is put into its own stream('sub-stream') or the primary
+        stream ('main-stream').
+    plots : list[Plot_Info]
+        List of the plots that should be created for the sweep.
+    read_channels : list[str]
+        List of the channels that should be read during the sweep.
+    sweep_values : list[Sweep_Step]
+        List of sub-steps containing the information about the sweeps.
+    """
     def __init__(self, name='', parent_step=None, step_info=None,
                  **kwargs):
         super().__init__(name=name, parent_step=parent_step, step_info=step_info,
                          **kwargs)
         step_info = step_info or {}
         self.step_type = 'ND Sweep'
         self.has_children = False
         self.sweep_channels = step_info['sweep_channels'] if 'sweep_channels' in step_info else []
         self.data_output = step_info['data_output'] if 'data_output' in step_info else 'sub-stream'
         self.plots = load_plots([], step_info['plots']) if 'plots' in step_info else []
         self.read_channels = step_info['read_channels'] if 'read_channels' in step_info else []
         self.sweep_values = step_info['sweep_values'] if 'sweep_values' in step_info else []
 
     def update_used_devices(self):
-        """ """
+        """Includes the devices from the read_channels and the sweep_channels"""
         self.used_devices = []
         for channel in self.read_channels:
             if channel in variables_handling.channels:
                 device = variables_handling.channels[channel].device
                 if device not in self.used_devices:
                     self.used_devices.append(device)
         for channel in self.sweep_channels:
             if channel in variables_handling.channels:
                 device = variables_handling.channels[channel].device
                 if device not in self.used_devices:
                     self.used_devices.append(device)
 
     def get_outer_string(self):
-        """ """
+        """Gives the string to create the plots of the sweeps"""
         if self.plots:
             return builder_helper_functions.plot_creator(self.plots, f'create_plots_{self.name}')[0]
         return ''
 
     def get_add_main_string(self):
-        """ """
+        """Calling the plot_creator from steps_add_main"""
         stream = f'"{self.name}"'
         if self.data_output == 'main stream':
             stream = '"primary"'
         add_main_string = ''
         if self.plots:
             add_main_string += builder_helper_functions.get_plot_add_string(self.name, stream)
         return add_main_string
```

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/prompt_loop_step.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/prompt_loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/read_channels.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/read_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/run_subprotocol.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/run_subprotocol.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/set_channels.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/set_channels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/set_value_popup.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/set_value_popup.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/set_variables.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/set_variables.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/simple_sweep.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/simple_sweep.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/loop_steps/wait_loop_step.py` & `nomad_camels-0.1.4/nomad_camels/loop_steps/wait_loop_step.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/device_class.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/device_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -599,15 +599,20 @@
 
         self.layout().addWidget(label_port, 0, 0)
         self.layout().addWidget(self.comboBox_port, 0, 1, 1, 4)
 
         label_baud = QLabel('Baud-Rate:')
         self.lineEdit_baud = QLineEdit('9600')
         self.layout().addWidget(label_baud, 1, 0)
-        self.layout().addWidget(self.lineEdit_baud, 1, 1, 1, 4)
+        self.layout().addWidget(self.lineEdit_baud, 1, 1)
+
+        label_timeout = QLabel('Timeout (ms):')
+        self.lineEdit_timeout = QLineEdit('2000')
+        self.layout().addWidget(label_timeout, 1, 2)
+        self.layout().addWidget(self.lineEdit_timeout, 1, 3)
 
         label_in_term = QLabel('In-Terminator:')
         self.lineEdit_in_term = QLineEdit('\\r\\n')
         self.layout().addWidget(label_in_term, 2, 0)
         self.layout().addWidget(self.lineEdit_in_term, 2, 1)
 
         label_out_term = QLabel('Out-Terminator:')
@@ -615,14 +620,15 @@
         self.layout().addWidget(label_out_term, 2, 2)
         self.layout().addWidget(self.lineEdit_out_term, 2, 3)
 
     def get_settings(self):
         """ """
         return {'resource_name': self.comboBox_port.currentText(),
                 'baud_rate': int(self.lineEdit_baud.text()),
+                'timeout': int(self.lineEdit_timeout.text()),
                 'read_termination': self.lineEdit_in_term.text().replace('\\r', '\r').replace('\\n', '\n'),
                 'write_termination': self.lineEdit_out_term.text().replace('\\r', '\r').replace('\\n', '\n')}
 
     def load_settings(self, settings_dict):
         """
 
         Parameters
@@ -636,14 +642,16 @@
         """
         if 'connection' in settings_dict:
             settings_dict = settings_dict['connection']
         if 'resource_name' in settings_dict and settings_dict['resource_name'] in self.ports:
             self.comboBox_port.setCurrentText(settings_dict['resource_name'])
         if 'baud_rate' in settings_dict:
             self.lineEdit_baud.setText(str(settings_dict['baud_rate']))
+        if 'timeout' in settings_dict:
+            self.lineEdit_timeout.setText(str(settings_dict['timeout']))
         if 'read_termination' in settings_dict:
             self.lineEdit_in_term.setText(settings_dict['read_termination'].replace('\r', '\\r').replace('\n', '\\n'))
         if 'write_termination' in settings_dict:
             self.lineEdit_out_term.setText(settings_dict['write_termination'].replace('\r', '\\r').replace('\n', '\\n'))
```

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/list_plot.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/list_plot.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/loop_step.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/loop_step.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,25 @@
 
 
 from nomad_camels.utility import treeView_functions, variables_handling
 
 
 
 class Loop_Step:
-    """Main Class for all Loop_Steps."""
+    """Main Class for all Loop_Steps.
+
+    Parameters
+    ----------
+    name : str
+        The custom name of the step.
+    parent_step : Loop_Step, default None
+        The step containing this step. If None, this step is in the outer layer.
+    step_info : dict, default None
+        Dictionary containing all the relevant information of the step.
+    """
     def __init__(self, name='', parent_step=None, step_info=None, **kwargs):
         self.step_type = 'Default'
         self.__save_dict__ = {}
         self.has_children = False
         self.children = []
         self.name = name
         self.full_name = f'{self.step_type} ({name})'
@@ -30,22 +40,19 @@
 
     def append_to_model(self, item_model, parent=None):
         """Ensures that the full_name of the loop_step is unique and
         updates name and full_name, then appends the step to the model.
 
         Parameters
         ----------
-        item_model :
-            
-        parent :
-             (Default value = None)
-
-        Returns
-        -------
-
+        item_model : QStandardItemModel
+            The item model that manages the view of the steps.
+        parent : QStandardItem
+            (Default value = None)
+            The parent of the step inside the item modle
         """
         if parent is None:
             parent = item_model
         if type(parent) is str:
             parent = item_model.itemFromIndex(treeView_functions.getItemIndex(item_model, parent))
         self.full_name = f'{self.step_type} ({self.name})'
         name = self.full_name
@@ -68,203 +75,160 @@
     def get_protocol_string(self, n_tabs=1):
         """Returns the string that is written into the protocol-file. To
         make use of the time_weight and status bar, it should start with
         printing, that the loop_step starts.
 
         Parameters
         ----------
-        n_tabs :
-             (Default value = 1)
+        n_tabs : int
+            (Default value = 1)
+            Number of tabs for indentation inside the script
 
         Returns
         -------
-
+        protocol_string : str
+            The string representing the step
         """
         tabs = '\t'*n_tabs
         desc = self.description.replace("\n", f"\n{tabs}")
         protocol_string = f'\n{tabs}"""{desc}"""\n'
         # protocol_string += f'{tabs}print("starting loop_step {self.full_name}")\n'
         protocol_string += f'{tabs}protocol_step_information["protocol_stepper_signal"].emit(protocol_step_information["protocol_step_counter"] / protocol_step_information["total_protocol_steps"] * 100)\n'
         protocol_string += f'{tabs}protocol_step_information["protocol_step_counter"] += 1\n'
         protocol_string += f'{tabs}yield from bps.checkpoint()\n'
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
         """
+        Gives a short overview of the step to quickly understand what the
+        protocol does.
 
         Parameters
         ----------
-        n_tabs :
-             (Default value = 0)
+        n_tabs : int
+            (Default value = 0)
+            Number of tabs for indentation inside the overview
 
         Returns
         -------
-
+        short_string : str
+            The string representing the step
         """
         tabs = '\t' * n_tabs
         short_string = f'{tabs}{self.step_type}\n'
         return short_string
 
 
     def get_outer_string(self):
-        """ """
+        """Returns the string for the protocol, where for example special plots
+        for the step are created."""
         return ''
 
     def get_add_main_string(self):
-        """ """
+        """Adds for example a call to the protocol function to the
+        steps_add_main function of the script."""
         return ''
 
     def update_variables(self):
         """Should update the variables_handling, if the loopstep
-        provides variables.
-
-        Parameters
-        ----------
-
-        Returns
-        -------
-
-        """
+        provides variables."""
         pass
 
     def update_used_devices(self):
         """Should update `used_devices` to include all necessary devices."""
         pass
 
     def update_time_weight(self):
-        """The time_weight of the children is included."""
+        """The number of calls for this step. It is used to set the scaling for
+        the progress bar of the protocol."""
         self.time_weight = 1
 
 
 class Loop_Step_Container(Loop_Step):
     """Parent Class for loop_steps that should contain further steps
     (like e.g. a for-loop).
 
     Parameters
     ----------
-
-    Returns
-    -------
-
-    Attributes
-    ----------
     children : list of Loop_Step
         A list of the children inside this step (in the order, they are
         to be executed)
     """
     def __init__(self, name='', children=None, parent_step=None, step_info=None, **kwargs):
         super().__init__(name, parent_step=parent_step, step_info=step_info, **kwargs)
         self.step_type = 'Container'
         self.has_children = True
         if children is None:
             children = []
         self.children = children
 
     def append_to_model(self, item_model:QStandardItemModel, parent=None):
         """Overwrites this function to additionally append all children
-        to the model.
-
-        Parameters
-        ----------
-        item_model:QStandardItemModel :
-            
-        parent :
-             (Default value = None)
-
-        Returns
-        -------
-
-        """
+        to the model."""
         item = super().append_to_model(item_model, parent)
         item.setDropEnabled(True)
         item.setEditable(False)
         for child in self.children:
             child.append_to_model(item_model, item)
         return item
 
     def add_child(self, child, position=-1):
         """Add a child-step at the specified position, default is -1,
         meaning to append at the end.
 
         Parameters
         ----------
-        child :
-            
-        position :
-             (Default value = -1)
-
-        Returns
-        -------
-
+        child : Loop_Step
+            The child to be added.
+        position : int
+            (Default value = -1)
+            The position, where to insert the child.
         """
         if position < 0:
             self.children.append(child)
         else:
             self.children.insert(position, child)
 
     def remove_child(self, child):
         """Removes the specified child from the children.
 
         Parameters
         ----------
-        child :
-            
-
-        Returns
-        -------
-
+        child : Loop_Step
+            Child step to be removed.
         """
         self.children.remove(child)
 
     def get_protocol_string(self, n_tabs=1):
         """Returns the string that is written into the protocol-file. To
         make use of the time_weight and status bar, it should start with
         printing, that the loop_step starts.
         Here it is overwritten to include the strings of the children.
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 1)
-
-        Returns
-        -------
-
         """
         protocol_string = super().get_protocol_string(n_tabs)
         # protocol_string += self.get_children_strings(n_tabs+1)
         self.update_time_weight()
         return protocol_string
 
     def get_protocol_short_string(self, n_tabs=0):
-        """
-
-        Parameters
-        ----------
-        n_tabs :
-             (Default value = 0)
-
-        Returns
-        -------
-
-        """
+        """This is overwritten to include the strings from the children"""
         short_string = super().get_protocol_short_string(n_tabs)
         for child in self.children:
             short_string += child.get_protocol_short_string(n_tabs+1)
         return short_string
 
     def get_outer_string(self):
-        """ """
+        """This is overwritten to include the strings from the children"""
         outer_string = ''
         for child in self.children:
             outer_string += child.get_outer_string()
         return outer_string
 
     def get_add_main_string(self):
-        """ """
+        """This is overwritten to include the strings from the children"""
         add_main_string = ''
         for child in self.children:
             add_main_string += child.get_add_main_string()
         return add_main_string
 
     def update_time_weight(self):
         """The time_weight of the children is included."""
@@ -275,20 +239,22 @@
 
 
     def get_children_strings(self, n_tabs=1):
         """Returns the protocol_strings of all the children.
 
         Parameters
         ----------
-        n_tabs :
-             (Default value = 1)
+        n_tabs : int
+            (Default value = 1)
+            Number of tabs for indentation inside the script
 
         Returns
         -------
-
+        child_string : str
+            The string of all children's protocol strings.
         """
         child_string = ''
         for child in self.children:
             child_string += child.get_protocol_string(n_tabs)
         return child_string
 
     def update_variables(self):
```

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/manual_control.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/manual_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/measurement_channel.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/measurement_channel.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/plot_2D.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/plot_2D.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/plot_widget.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/plot_widget.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/main_classes/protocol_class.py` & `nomad_camels-0.1.4/nomad_camels/main_classes/protocol_class.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/manual_controls/get_manual_controls.py` & `nomad_camels-0.1.4/nomad_camels/manual_controls/get_manual_controls.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/manual_controls/stage_control/stage_control.py` & `nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/manual_controls/stage_control/ui_stage_control.py` & `nomad_camels-0.1.4/nomad_camels/manual_controls/stage_control/ui_stage_control.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/tests/instrument_management_test.py` & `nomad_camels-0.1.4/nomad_camels/tests/instrument_management_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/tests/protocol_test.py` & `nomad_camels-0.1.4/nomad_camels/tests/protocol_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/tests/startup_test.py` & `nomad_camels-0.1.4/nomad_camels/tests/startup_test.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/tools/EPICS_driver_builder.py` & `nomad_camels-0.1.4/nomad_camels/tools/EPICS_driver_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 from pkg_resources import resource_filename
 
 
 class EPICS_Driver_Builder(QDialog):
     def __init__(self, parent=None):
         super().__init__(parent)
 
-        if os.path.isdir('graphics'):
+        try:
             self.setWindowIcon(QIcon(resource_filename('nomad_camels', 'graphics/camels_icon.png')))
-        else:
-            self.setWindowIcon(QIcon('../graphics/CAMELS.svg'))
+        except:
+            pass
         self.setWindowTitle('NOMAD-CAMELS - EPICS-driver-builder')
 
         label_name = QLabel('Instrument Name:')
         self.lineEdit_name = QLineEdit()
 
         label_in = QLabel('Input Channels')
         label_out = QLabel('Output Channels')
@@ -77,22 +77,25 @@
         def check_builtin(pv):
             if pv in vars(__builtins__):
                 raise Exception(f'PV-name "{pv}" resembles python builtin function or variable!\nDefine another name!\nYou may change the PV-name later in the code, see the documentation for more information.')
             try:
                 ast.parse(f'{pv} = None')
             except (ValueError, SyntaxError, TypeError):
                 raise Exception(f'PV-name "{pv}" resembles python builtin function or variable!\nDefine another name!\nYou may change the PV-name later in the code, see the documentation for more information.')
+        all_good = True
         for name in inputs['PV-Name']:
-            check_builtin(name)
+            all_good = all_good and variables_handling.check_variable_name(name, parent=self)
         for name in outputs['PV-Name']:
-            check_builtin(name)
+            all_good = all_good and variables_handling.check_variable_name(name, parent=self)
         for name in configs['PV-Name']:
-            check_builtin(name)
+            all_good = all_good and variables_handling.check_variable_name(name, parent=self)
         for name in configs_in['PV-Name']:
-            check_builtin(name)
+            all_good = all_good and variables_handling.check_variable_name(name, parent=self)
+        if not all_good:
+            raise Exception(f'Some PV-name resemble python builtin function or variable!\nDefine another name!\nYou may change the PV-name later in the code, see the documentation for more information.')
         directory = f'{path}/nomad_camels_driver_{dev_name}'
         sys.path.append(directory)
         fname = f'{directory}/{dev_name}.py'
         if os.path.isdir(directory) and os.path.isfile(fname):
             answer = QMessageBox.question(self, 'Instrument already exists!', f'Instrument type with name {dev_name} already exists.\nDo you want to overwrite the existing instrument driver?', buttons=QMessageBox.Yes | QMessageBox.Cancel, defaultButton=QMessageBox.Cancel)
             if answer != QMessageBox.Yes:
                 return
```

### Comparing `nomad_camels-0.1.3/nomad_camels/tools/VISA_builder.py` & `nomad_camels-0.1.4/nomad_camels/tools/VISA_builder.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/tools/VISA_driver_builder.py` & `nomad_camels-0.1.4/nomad_camels/tools/VISA_driver_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 class VISA_Driver_Builder(Ui_VISA_Device_Builder, QDialog):
     """ """
     def __init__(self, parent=None):
         super().__init__(parent=parent)
         self.setupUi(self)
 
-        if os.path.isdir('graphics'):
+        try:
             self.setWindowIcon(QIcon(resource_filename('nomad_camels', 'graphics/camels_icon.png')))
-        else:
-            self.setWindowIcon(QIcon('../graphics/CAMELS.svg'))
+        except:
+            pass
         self.setWindowTitle('NOMAD-CAMELS - VISA-driver-builder')
 
         label_in = QLabel('Input Channels')
         label_out = QLabel('Output Channels')
         label_config = QLabel('Config Channels')
         label_config_in = QLabel('Config Channels - Input Only')
         label_in.setStyleSheet("font-weight: bold")
```

### Comparing `nomad_camels-0.1.3/nomad_camels/tools/databroker_exporter.py` & `nomad_camels-0.1.4/nomad_camels/tools/databroker_exporter.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/ui_widgets/add_remove_table.py` & `nomad_camels-0.1.4/nomad_camels/ui_widgets/add_remove_table.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/ui_widgets/channels_check_table.py` & `nomad_camels-0.1.4/nomad_camels/ui_widgets/channels_check_table.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/ui_widgets/console_redirect.py` & `nomad_camels-0.1.4/nomad_camels/ui_widgets/console_redirect.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/ui_widgets/drag_drop_tree_view.py` & `nomad_camels-0.1.4/nomad_camels/ui_widgets/drag_drop_tree_view.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/ui_widgets/options_run_button.py` & `nomad_camels-0.1.4/nomad_camels/ui_widgets/options_run_button.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/ui_widgets/path_button_edit.py` & `nomad_camels-0.1.4/nomad_camels/ui_widgets/path_button_edit.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/ui_widgets/variable_tool_tip_box.py` & `nomad_camels-0.1.4/nomad_camels/ui_widgets/variable_tool_tip_box.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/databroker_export.py` & `nomad_camels-0.1.4/nomad_camels/utility/databroker_export.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/device_handling.py` & `nomad_camels-0.1.4/nomad_camels/utility/device_handling.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/exception_hook.py` & `nomad_camels-0.1.4/nomad_camels/utility/exception_hook.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/fit_variable_renaming.py` & `nomad_camels-0.1.4/nomad_camels/utility/fit_variable_renaming.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/load_save_functions.py` & `nomad_camels-0.1.4/nomad_camels/utility/load_save_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/load_save_helper_functions.py` & `nomad_camels-0.1.4/nomad_camels/utility/load_save_helper_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/number_formatting.py` & `nomad_camels-0.1.4/nomad_camels/utility/number_formatting.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/plot_placement.py` & `nomad_camels-0.1.4/nomad_camels/utility/plot_placement.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/qthreads.py` & `nomad_camels-0.1.4/nomad_camels/utility/qthreads.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/theme_changing.py` & `nomad_camels-0.1.4/nomad_camels/utility/theme_changing.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/treeView_functions.py` & `nomad_camels-0.1.4/nomad_camels/utility/treeView_functions.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/update_camels.py` & `nomad_camels-0.1.4/nomad_camels/utility/update_camels.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels/utility/variables_handling.py` & `nomad_camels-0.1.4/nomad_camels/utility/variables_handling.py`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/nomad_camels.egg-info/PKG-INFO` & `nomad_camels-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nomad-camels
-Version: 0.1.3
+Name: nomad_camels
+Version: 0.1.4
 Summary: CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics.
 Author-email: FAIRmat - HU Berlin <nomad-camels@fau.de>
 Project-URL: GitHub Page, https://github.com/FAU-LAP/NOMAD-CAMELS
 Project-URL: Documentation, https://fau-lap.github.io/NOMAD-CAMELS/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Requires-Python: >=3.9.6
@@ -24,7 +24,19 @@
 
 NOMAD-CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics. Here many experiments utilize a multitude of measurement devices used in dynamically changing setups. CAMELS will allow to define instrument control and measurement protocols using a graphical user interface (GUI). This provides a low entry threshold enabling the creation of new measurement protocols without programming knowledge or a deeper understanding of device communication. The GUI generates python code that interfaces with instruments and allows users to modify the code for specific applications and implementations of arbitrary devices if necessary. Even large-scale, distributed systems can be implemented. CAMELS is well suited to generate FAIR-compliant output data. Nexus standards, immediate NOMAD integration and hence a FAIRmat compliant data pipeline can be readily implemented.
 
 
 ## Documentation
 
 For more information and documentation visit [this page](https://fau-lap.github.io/NOMAD-CAMELS/).
+
+# Changelog
+
+
+## 0.1.4
+Added a timeout setting to all VISA instruments. 
+
+## 0.1.3
+First stable and working release
+
+## 0.1.0 to 0.1.2 
+&#9888; Broken releases due to minor bugs that were fixed in 0.1.3
```

### Comparing `nomad_camels-0.1.3/nomad_camels.egg-info/SOURCES.txt` & `nomad_camels-0.1.4/nomad_camels.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 nomad_camels/frontpanels/device_add_dialog.py
 nomad_camels/frontpanels/instrument_config.py
 nomad_camels/frontpanels/instrument_installer.py
 nomad_camels/frontpanels/manage_instruments.py
 nomad_camels/frontpanels/plot_definer.py
 nomad_camels/frontpanels/protocol_config.py
 nomad_camels/frontpanels/settings_window.py
-nomad_camels/frontpanels/taskSelector.py
 nomad_camels/frontpanels/helper_panels/__init__.py
 nomad_camels/frontpanels/helper_panels/button_move_scroll_area.py
 nomad_camels/frontpanels/helper_panels/enterTextDialog.py
 nomad_camels/frontpanels/helper_panels/pass_ask.py
 nomad_camels/graphics/CAMELS.ico
 nomad_camels/graphics/CAMELS_Icon.png
 nomad_camels/graphics/Camel Groan 2 - QuickSounds.com.mp3
@@ -63,15 +62,14 @@
 nomad_camels/gui/addDeviceDialog.py
 nomad_camels/gui/device_installer.py
 nomad_camels/gui/enterTextDialog.py
 nomad_camels/gui/fit_definer.py
 nomad_camels/gui/for_loop.py
 nomad_camels/gui/general_protocol_settings.py
 nomad_camels/gui/gradient_descent_step.py
-nomad_camels/gui/installer_window.py
 nomad_camels/gui/instrument_config.py
 nomad_camels/gui/mainWindow_v2.py
 nomad_camels/gui/pass_ask.py
 nomad_camels/gui/plot_definer.py
 nomad_camels/gui/plot_definer_2d.py
 nomad_camels/gui/plot_options.py
 nomad_camels/gui/protocol_view.py
@@ -90,15 +88,14 @@
 nomad_camels/loop_steps/run_subprotocol.py
 nomad_camels/loop_steps/set_channels.py
 nomad_camels/loop_steps/set_value_popup.py
 nomad_camels/loop_steps/set_variables.py
 nomad_camels/loop_steps/simple_sweep.py
 nomad_camels/loop_steps/wait_loop_step.py
 nomad_camels/main_classes/__init__.py
-nomad_camels/main_classes/camels_installer.py
 nomad_camels/main_classes/device_class.py
 nomad_camels/main_classes/list_plot.py
 nomad_camels/main_classes/loop_step.py
 nomad_camels/main_classes/manual_control.py
 nomad_camels/main_classes/measurement_channel.py
 nomad_camels/main_classes/plot_2D.py
 nomad_camels/main_classes/plot_widget.py
```

### Comparing `nomad_camels-0.1.3/nomad_camels.egg-info/requires.txt` & `nomad_camels-0.1.4/nomad_camels.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `nomad_camels-0.1.3/pyproject.toml` & `nomad_camels-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nomad_camels"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name="FAIRmat - HU Berlin", email="nomad-camels@fau.de" }
 ]
 description = "CAMELS is a configurable measurement software, targeted towards the requirements of experimental solid-state physics."
 readme = "README.md"
 requires-python = ">=3.9.6"
 classifiers = [
```

### Comparing `nomad_camels-0.1.3/requirements.txt` & `nomad_camels-0.1.4/requirements.txt`

 * *Files identical despite different names*

