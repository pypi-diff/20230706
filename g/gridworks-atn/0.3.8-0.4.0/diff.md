# Comparing `tmp/gridworks_atn-0.3.8.tar.gz` & `tmp/gridworks_atn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_atn-0.3.8.tar", max compression
+gzip compressed data, was "gridworks_atn-0.4.0.tar", max compression
```

## Comparing `gridworks_atn-0.3.8.tar` & `gridworks_atn-0.4.0.tar`

### file list

```diff
@@ -1,243 +1,259 @@
--rw-r--r--   0        0        0     1065 2023-06-27 19:18:29.214349 gridworks_atn-0.3.8/LICENSE
--rw-r--r--   0        0        0     3002 2023-06-27 19:18:29.218349 gridworks_atn-0.3.8/README.md
--rw-r--r--   0        0        0     2157 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      681 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/__init__.py
--rw-r--r--   0        0        0      226 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/__main__.py
--rw-r--r--   0        0        0    13844 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/api_types.py
--rw-r--r--   0        0        0    23400 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/atn_actor_base.py
--rw-r--r--   0        0        0     3538 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/atn_utils.py
--rw-r--r--   0        0        0     4521 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/config.py
--rw-r--r--   0        0        0       43 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/conversion_factors.py
--rw-r--r--   0        0        0     6148 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/.DS_Store
--rw-r--r--   0        0        0      935 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/__init__.py
--rw-r--r--   0        0        0      577 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/d_edge.py
--rw-r--r--   0        0        0     7812 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/d_graph.py
--rw-r--r--   0        0        0     1508 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/d_node.py
--rw-r--r--   0        0        0     8684 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/hack_price_method.py
--rw-r--r--   0        0        0     4082 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_location.py
--rw-r--r--   0        0        0     2104 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_source.py
--rw-r--r--   0        0        0    14466 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/demo_methods.py
--rw-r--r--   0        0        0      276 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_discoverer.py
--rw-r--r--   0        0        0    11883 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_ta_owner.py
--rw-r--r--   0        0        0    10994 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_validator.py
--rw-r--r--   0        0        0     1171 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dev_utils/make_plants.py
--rw-r--r--   0        0        0    11409 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract.py
--rw-r--r--   0        0        0    12463 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/application.json
--rw-r--r--   0        0        0     5229 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/approval.teal
--rw-r--r--   0        0        0       40 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/clear.teal
--rw-r--r--   0        0        0     3937 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/contract.json
--rw-r--r--   0        0        0     2069 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/enums/__init__.py
--rw-r--r--   0        0        0     2677 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/enums/distribution_tariff.py
--rw-r--r--   0        0        0      614 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/energy_supply_type.py
--rw-r--r--   0        0        0     1308 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_price_method.py
--rw-r--r--   0        0        0      415 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_recognized_p_node_alias.py
--rw-r--r--   0        0        0      590 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_weather_method.py
--rw-r--r--   0        0        0      132 2023-06-27 19:18:29.230349 gridworks_atn-0.3.8/src/gwatn/enums/hack_weather_source.py
--rw-r--r--   0        0        0      947 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/enums/recognized_irradiance_type.py
--rw-r--r--   0        0        0      570 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/enums/recognized_temperature_unit.py
--rw-r--r--   0        0        0      122 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/errors.py
--rw-r--r--   0        0        0        0 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/py.typed
--rw-r--r--   0        0        0     7945 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.json
--rw-r--r--   0        0        0    12518 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.py
--rw-r--r--   0        0        0      834 2023-06-27 19:18:29.234349 gridworks_atn-0.3.8/src/gwatn/scada_codec.py
--rw-r--r--   0        0        0     3677 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/simple_atn_actor.py
--rw-r--r--   0        0        0        0 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/__init__.py
--rw-r--r--   0        0        0    20114 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/atn.py
--rw-r--r--   0        0        0       98 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/dev_atn_params_data.csv
--rw-r--r--   0        0        0     7337 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/dev_io.py
--rw-r--r--   0        0        0      867 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/edge.py
--rw-r--r--   0        0        0     7536 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo.py
--rw-r--r--   0        0        0    18355 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo_output.py
--rw-r--r--   0        0        0     1508 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/make_dev_input_data.py
--rw-r--r--   0        0        0      841 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/node.py
--rw-r--r--   0        0        0     2549 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/strategy_utils.py
--rw-r--r--   0        0        0    20114 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/atn.py
--rw-r--r--   0        0        0     8663 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/dev_io.py
--rw-r--r--   0        0        0      867 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/edge.py
--rw-r--r--   0        0        0     7536 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/flo.py
--rw-r--r--   0        0        0    18355 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/flo_output.py
--rw-r--r--   0        0        0     9363 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/flo_utils.py
--rw-r--r--   0        0        0     1824 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/make_dev_input_data.py
--rw-r--r--   0        0        0      841 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/node.py
--rw-r--r--   0        0        0        0 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/output_data/__init__.py
--rw-r--r--   0        0        0    26363 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/simple_scada_sim.py
--rw-r--r--   0        0        0     3717 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/strategy_utils.py
--rw-r--r--   0        0        0    11673 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/tea.py
--rw-r--r--   0        0        0     3152 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/tea_config.py
--rw-r--r--   0        0        0    21042 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/tea_output.py
--rw-r--r--   0        0        0     3169 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/ta_daemon_rest_api.py
--rw-r--r--   0        0        0      460 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/ta_validator_rest_api.py
--rw-r--r--   0        0        0    51741 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/two_channel_actor_base.py
--rw-r--r--   0        0        0    13733 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/__init__.py
--rw-r--r--   0        0        0     7868 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/accepted_bid.py
--rw-r--r--   0        0        0    20222 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/atn_bid.py
--rw-r--r--   0        0        0     4288 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/atn_params.py
--rw-r--r--   0        0        0    22525 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/atn_params_brickstorageheater.py
--rw-r--r--   0        0        0     8144 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/atn_params_report.py
--rw-r--r--   0        0        0    19280 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/atn_params_simpleresistivehydronic.py
--rw-r--r--   0        0        0     8321 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/basegnode_scada_create.py
--rw-r--r--   0        0        0     1067 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/data_channel.py
--rw-r--r--   0        0        0     9885 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/discoverycert_algo_create.py
--rw-r--r--   0        0        0     8092 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/dispatch_contract_confirmed.py
--rw-r--r--   0        0        0     3235 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0.py
--rw-r--r--   0        0        0      555 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3959 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3338 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0      555 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3959 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3658 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     1690 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     4905 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7648 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/flo_params.py
--rw-r--r--   0        0        0    22633 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/flo_params_brickstorageheater.py
--rw-r--r--   0        0        0     8827 2023-06-27 19:18:29.238349 gridworks_atn-0.3.8/src/gwatn/types/flo_params_report.py
--rw-r--r--   0        0        0    16757 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/flo_params_simpleresistivehydronic.py
--rw-r--r--   0        0        0     3885 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py
--rw-r--r--   0        0        0      600 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4184 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5457 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py
--rw-r--r--   0        0        0      620 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7905 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5419 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0      625 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7913 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5176 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py
--rw-r--r--   0        0        0      649 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py
--rw-r--r--   0        0        0     8053 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3885 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py
--rw-r--r--   0        0        0      593 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4203 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5392 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py
--rw-r--r--   0        0        0      613 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7891 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3909 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py
--rw-r--r--   0        0        0      609 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4212 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7507 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py
--rw-r--r--   0        0        0     1453 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py
--rw-r--r--   0        0        0    12856 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7530 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py
--rw-r--r--   0        0        0     1453 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0    11873 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3980 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py
--rw-r--r--   0        0        0      611 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4060 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4083 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py
--rw-r--r--   0        0        0      627 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4430 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3879 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py
--rw-r--r--   0        0        0      595 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py
--rw-r--r--   0        0        0     4196 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5398 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py
--rw-r--r--   0        0        0      615 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py
--rw-r--r--   0        0        0     7901 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py
--rw-r--r--   0        0        0     8206 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0    14769 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_property_format.py
--rw-r--r--   0        0        0      194 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_test_dummy.py
--rw-r--r--   0        0        0      781 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_type_base.py
--rw-r--r--   0        0        0      990 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/hack_utils.py
--rw-r--r--   0        0        0     9155 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/heartbeat_b.py
--rw-r--r--   0        0        0     6154 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_create.py
--rw-r--r--   0        0        0     7610 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_optin.py
--rw-r--r--   0        0        0     8932 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_transfer.py
--rw-r--r--   0        0        0     7959 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/join_dispatch_contract.py
--rw-r--r--   0        0        0    12429 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/latest_price.py
--rw-r--r--   0        0        0     5028 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/market_slot.py
--rw-r--r--   0        0        0    17161 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/market_type_gt.py
--rw-r--r--   0        0        0     5294 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_algo_optin.py
--rw-r--r--   0        0        0     5196 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_send.py
--rw-r--r--   0        0        0     5024 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/old_tadeed_algo_return.py
--rw-r--r--   0        0        0     8461 2023-06-27 19:18:29.242349 gridworks_atn-0.3.8/src/gwatn/types/price_quantity.py
--rw-r--r--   0        0        0     2492 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/price_quantity_unitless.py
--rw-r--r--   0        0        0    13837 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py
--rw-r--r--   0        0        0    13162 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py
--rw-r--r--   0        0        0    14105 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py
--rw-r--r--   0        0        0     5624 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py
--rw-r--r--   0        0        0      558 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py
--rw-r--r--   0        0        0     8026 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5026 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py
--rw-r--r--   0        0        0      594 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py
--rw-r--r--   0        0        0     7236 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5890 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py
--rw-r--r--   0        0        0      578 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7750 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7618 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py
--rw-r--r--   0        0        0    13827 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py
--rw-r--r--   0        0        0     7319 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0    12667 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py
--rw-r--r--   0        0        0     8872 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0    10345 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py
--rw-r--r--   0        0        0    14435 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py
--rw-r--r--   0        0        0     4044 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py
--rw-r--r--   0        0        0      589 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3804 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5402 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py
--rw-r--r--   0        0        0      561 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py
--rw-r--r--   0        0        0     7263 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4044 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py
--rw-r--r--   0        0        0      589 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py
--rw-r--r--   0        0        0     3804 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5661 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py
--rw-r--r--   0        0        0      597 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py
--rw-r--r--   0        0        0     7829 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3535 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py
--rw-r--r--   0        0        0      653 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py
--rw-r--r--   0        0        0     3064 2023-06-27 19:18:29.246349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4184 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0      586 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     3863 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5892 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py
--rw-r--r--   0        0        0      581 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7746 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3707 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py
--rw-r--r--   0        0        0      581 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py
--rw-r--r--   0        0        0     3547 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py
--rw-r--r--   0        0        0    13926 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py
--rw-r--r--   0        0        0    14182 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py
--rw-r--r--   0        0        0     5617 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py
--rw-r--r--   0        0        0      544 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py
--rw-r--r--   0        0        0     8022 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5864 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py
--rw-r--r--   0        0        0      573 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py
--rw-r--r--   0        0        0     7746 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     5004 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/scada_cert_transfer.py
--rw-r--r--   0        0        0     3682 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data.py
--rw-r--r--   0        0        0     4166 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data_bsh.py
--rw-r--r--   0        0        0     6534 2023-06-27 19:18:48.906515 gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_report.py
--rw-r--r--   0        0        0     6774 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
--rw-r--r--   0        0        0     3220 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/sla_enter.py
--rw-r--r--   0        0        0     4101 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/tadeed_specs_hack.py
--rw-r--r--   0        0        0     5734 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_create.py
--rw-r--r--   0        0        0     6371 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_transfer.py
--rw-r--r--   0        0        0     5242 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/terminalasset_certify_hack.py
--rw-r--r--   0        0        0    30475 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py
--rw-r--r--   0        0        0    29247 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     8474 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py
--rw-r--r--   0        0        0     1920 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py
--rw-r--r--   0        0        0    13416 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3535 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py
--rw-r--r--   0        0        0      686 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py
--rw-r--r--   0        0        0     3076 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py
--rw-r--r--   0        0        0     7834 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py
--rw-r--r--   0        0        0      829 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py
--rw-r--r--   0        0        0    12801 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py
--rw-r--r--   0        0        0     8628 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py
--rw-r--r--   0        0        0     1153 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py
--rw-r--r--   0        0        0    12807 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3671 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py
--rw-r--r--   0        0        0      572 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py
--rw-r--r--   0        0        0     3547 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py
--rw-r--r--   0        0        0    14909 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py
--rw-r--r--   0        0        0    11616 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py
--rw-r--r--   0        0        0     4544 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py
--rw-r--r--   0        0        0      631 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py
--rw-r--r--   0        0        0     6001 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py
--rw-r--r--   0        0        0    12321 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py
--rw-r--r--   0        0        0     6939 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py
--rw-r--r--   0        0        0      642 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py
--rw-r--r--   0        0        0    10751 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     4677 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py
--rw-r--r--   0        0        0      610 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py
--rw-r--r--   0        0        0     6741 2023-06-27 19:18:29.250349 gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py
--rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-06 21:43:41.123624 gridworks_atn-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3002 2023-07-06 21:43:41.123624 gridworks_atn-0.4.0/README.md
+-rw-r--r--   0        0        0     2156 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      681 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/__init__.py
+-rw-r--r--   0        0        0      226 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/__main__.py
+-rw-r--r--   0        0        0    14041 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/api_types.py
+-rw-r--r--   0        0        0    23400 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/atn_actor_base.py
+-rw-r--r--   0        0        0     3538 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/atn_utils.py
+-rw-r--r--   0        0        0     4521 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/config.py
+-rw-r--r--   0        0        0       43 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/conversion_factors.py
+-rw-r--r--   0        0        0     6148 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/data_classes/.DS_Store
+-rw-r--r--   0        0        0      935 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/data_classes/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/data_classes/d_edge.py
+-rw-r--r--   0        0        0     9629 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/data_classes/d_graph.py
+-rw-r--r--   0        0        0     1508 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/data_classes/d_node.py
+-rw-r--r--   0        0        0     8684 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/data_classes/hack_price_method.py
+-rw-r--r--   0        0        0     4082 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/data_classes/hack_weather_location.py
+-rw-r--r--   0        0        0     2104 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/data_classes/hack_weather_source.py
+-rw-r--r--   0        0        0    14466 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/demo_methods.py
+-rw-r--r--   0        0        0      276 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/dev_utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/dev_utils/dev_discoverer.py
+-rw-r--r--   0        0        0    11883 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/dev_utils/dev_ta_owner.py
+-rw-r--r--   0        0        0    10994 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/dev_utils/dev_validator.py
+-rw-r--r--   0        0        0     1171 2023-07-06 21:43:41.135624 gridworks_atn-0.4.0/src/gwatn/dev_utils/make_plants.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/actual_data/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/actual_data/init_actual_prices_db.py
+-rw-r--r--   0        0        0     4912 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/actual_data/update_actual_price_db.py
+-rw-r--r--   0        0        0      704 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/basic_eprt_handler.py
+-rw-r--r--   0        0        0    13455 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/distp_sync_100_handler.py
+-rw-r--r--   0        0        0     9164 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/eprt_forecast_sync_100_handler.py
+-rw-r--r--   0        0        0    12341 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/eprt_sync_100_handler.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/caiso/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/ercot/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/gw/__init__.py
+-rw-r--r--   0        0        0     3748 2023-07-06 21:43:59.115853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/init_ps_db.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/isone/__init__.py
+-rw-r--r--   0        0        0     1480 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/isone/distp__w.isone.stetson__2022__168__gw.me.versant.a1.res.ets__5311504b.csv
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/miso/__init__.py
+-rw-r--r--   0        0        0    12116 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/forecast_data/update_forecast_price_db.py
+-rw-r--r--   0        0        0     1075 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/input_handler.py
+-rw-r--r--   0        0        0    11667 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/dev_utils/price/regp_sync_100_handler.py
+-rw-r--r--   0        0        0    11409 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/dispatch_contract.py
+-rw-r--r--   0        0        0    12463 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/dispatch_contract_artifacts/application.json
+-rw-r--r--   0        0        0     5229 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/dispatch_contract_artifacts/approval.teal
+-rw-r--r--   0        0        0       40 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/dispatch_contract_artifacts/clear.teal
+-rw-r--r--   0        0        0     3937 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/dispatch_contract_artifacts/contract.json
+-rw-r--r--   0        0        0     2411 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/enums/__init__.py
+-rw-r--r--   0        0        0     3032 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/enums/distribution_tariff.py
+-rw-r--r--   0        0        0      614 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/enums/energy_supply_type.py
+-rw-r--r--   0        0        0     1308 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/enums/hack_price_method.py
+-rw-r--r--   0        0        0      415 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/enums/hack_recognized_p_node_alias.py
+-rw-r--r--   0        0        0      590 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/enums/hack_weather_method.py
+-rw-r--r--   0        0        0      132 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/enums/hack_weather_source.py
+-rw-r--r--   0        0        0      947 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/enums/recognized_irradiance_type.py
+-rw-r--r--   0        0        0      570 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/enums/recognized_temperature_unit.py
+-rw-r--r--   0        0        0      122 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/errors.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/py.typed
+-rw-r--r--   0        0        0     7945 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/python_ta_daemon.json
+-rw-r--r--   0        0        0    12518 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/python_ta_daemon.py
+-rw-r--r--   0        0        0      834 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/scada_codec.py
+-rw-r--r--   0        0        0     3677 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/simple_atn_actor.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/__init__.py
+-rw-r--r--   0        0        0    20108 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/atn.py
+-rw-r--r--   0        0        0       98 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/dev_atn_params_data.csv
+-rw-r--r--   0        0        0     7337 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/dev_io.py
+-rw-r--r--   0        0        0      867 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/edge.py
+-rw-r--r--   0        0        0     7534 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/flo.py
+-rw-r--r--   0        0        0    18349 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/flo_output.py
+-rw-r--r--   0        0        0     1508 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/make_dev_input_data.py
+-rw-r--r--   0        0        0      841 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/node.py
+-rw-r--r--   0        0        0     2549 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/strategy_utils.py
+-rw-r--r--   0        0        0    19970 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/atn.py
+-rw-r--r--   0        0        0     8709 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/dev_io.py
+-rw-r--r--   0        0        0      984 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/edge.py
+-rw-r--r--   0        0        0    11210 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/flo.py
+-rw-r--r--   0        0        0    17459 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/flo_output.py
+-rw-r--r--   0        0        0     9037 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/flo_utils.py
+-rw-r--r--   0        0        0     1828 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/make_dev_input_data.py
+-rw-r--r--   0        0        0      785 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/node.py
+-rw-r--r--   0        0        0        0 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/output_data/__init__.py
+-rw-r--r--   0        0        0    26307 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/simple_scada_sim.py
+-rw-r--r--   0        0        0     3300 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/strategy_utils.py
+-rw-r--r--   0        0        0     3169 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/ta_daemon_rest_api.py
+-rw-r--r--   0        0        0      460 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/ta_validator_rest_api.py
+-rw-r--r--   0        0        0    51741 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/two_channel_actor_base.py
+-rw-r--r--   0        0        0    13965 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/types/__init__.py
+-rw-r--r--   0        0        0     7868 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/types/accepted_bid.py
+-rw-r--r--   0        0        0    20222 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/types/atn_bid.py
+-rw-r--r--   0        0        0     2842 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/types/atn_outside_temp_regr_coeffs.py
+-rw-r--r--   0        0        0     4288 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/types/atn_params.py
+-rw-r--r--   0        0        0    22525 2023-07-06 21:43:41.139624 gridworks_atn-0.4.0/src/gwatn/types/atn_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8144 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/atn_params_report.py
+-rw-r--r--   0        0        0    20143 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/types/atn_params_simpleresistivehydronic.py
+-rw-r--r--   0        0        0     8321 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/basegnode_scada_create.py
+-rw-r--r--   0        0        0     1067 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/data_channel.py
+-rw-r--r--   0        0        0     9885 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/discoverycert_algo_create.py
+-rw-r--r--   0        0        0     8092 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/dispatch_contract_confirmed.py
+-rw-r--r--   0        0        0     3235 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/epda/gt_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3338 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      555 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3959 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3658 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1690 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     4905 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7648 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/flo_params.py
+-rw-r--r--   0        0        0    22633 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/flo_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8827 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/flo_params_report.py
+-rw-r--r--   0        0        0    26527 2023-07-06 21:43:59.119853 gridworks_atn-0.4.0/src/gwatn/types/flo_params_simpleresistivehydronic.py
+-rw-r--r--   0        0        0     3885 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py
+-rw-r--r--   0        0        0      600 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4184 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5457 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      620 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7905 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5419 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      625 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7913 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5176 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0      649 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     8053 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3885 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py
+-rw-r--r--   0        0        0      593 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4203 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5392 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      613 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7891 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3909 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      609 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4212 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7507 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    12856 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7530 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py
+-rw-r--r--   0        0        0     1453 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0    11873 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3980 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py
+-rw-r--r--   0        0        0      611 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4060 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4083 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py
+-rw-r--r--   0        0        0      627 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4430 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3879 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py
+-rw-r--r--   0        0        0      595 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     4196 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5398 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py
+-rw-r--r--   0        0        0      615 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py
+-rw-r--r--   0        0        0     7901 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8206 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0    14769 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/hack_property_format.py
+-rw-r--r--   0        0        0      194 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/hack_test_dummy.py
+-rw-r--r--   0        0        0      781 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/hack_type_base.py
+-rw-r--r--   0        0        0      990 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/hack_utils.py
+-rw-r--r--   0        0        0     9155 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/heartbeat_b.py
+-rw-r--r--   0        0        0     6154 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/initial_tadeed_algo_create.py
+-rw-r--r--   0        0        0     7610 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/initial_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     8932 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/initial_tadeed_algo_transfer.py
+-rw-r--r--   0        0        0     7959 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/join_dispatch_contract.py
+-rw-r--r--   0        0        0    12429 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/latest_price.py
+-rw-r--r--   0        0        0     5028 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/market_slot.py
+-rw-r--r--   0        0        0    17161 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/market_type_gt.py
+-rw-r--r--   0        0        0     5294 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/new_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     5196 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/new_tadeed_send.py
+-rw-r--r--   0        0        0     5024 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/old_tadeed_algo_return.py
+-rw-r--r--   0        0        0     8461 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/price_quantity.py
+-rw-r--r--   0        0        0     2492 2023-07-06 21:43:41.143624 gridworks_atn-0.4.0/src/gwatn/types/price_quantity_unitless.py
+-rw-r--r--   0        0        0    13837 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py
+-rw-r--r--   0        0        0    13162 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0    14105 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5624 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py
+-rw-r--r--   0        0        0      558 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8026 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5026 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py
+-rw-r--r--   0        0        0      594 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py
+-rw-r--r--   0        0        0     7236 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5890 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py
+-rw-r--r--   0        0        0      578 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7750 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7618 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0    13827 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py
+-rw-r--r--   0        0        0     7319 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0    12667 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0     8872 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0    10345 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py
+-rw-r--r--   0        0        0    14435 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0     4044 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5402 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py
+-rw-r--r--   0        0        0      561 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py
+-rw-r--r--   0        0        0     7263 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4044 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py
+-rw-r--r--   0        0        0      589 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py
+-rw-r--r--   0        0        0     3804 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5661 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py
+-rw-r--r--   0        0        0      597 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0     7829 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      653 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3064 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4184 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0      586 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     3863 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5892 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3707 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py
+-rw-r--r--   0        0        0      581 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    13926 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py
+-rw-r--r--   0        0        0    14182 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0     5617 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py
+-rw-r--r--   0        0        0      544 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py
+-rw-r--r--   0        0        0     8022 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5864 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py
+-rw-r--r--   0        0        0      573 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0     7746 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     5004 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/scada_cert_transfer.py
+-rw-r--r--   0        0        0     3682 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/simplesim_driver_data.py
+-rw-r--r--   0        0        0     4166 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/simplesim_driver_data_bsh.py
+-rw-r--r--   0        0        0     6534 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/simplesim_driver_report.py
+-rw-r--r--   0        0        0     6774 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
+-rw-r--r--   0        0        0     3220 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/sla_enter.py
+-rw-r--r--   0        0        0     4101 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/tadeed_specs_hack.py
+-rw-r--r--   0        0        0     5734 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/tavalidatorcert_algo_create.py
+-rw-r--r--   0        0        0     6371 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/tavalidatorcert_algo_transfer.py
+-rw-r--r--   0        0        0     5242 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/terminalasset_certify_hack.py
+-rw-r--r--   0        0        0    30475 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0    29247 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     8474 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py
+-rw-r--r--   0        0        0     1920 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py
+-rw-r--r--   0        0        0    13416 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3535 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py
+-rw-r--r--   0        0        0      686 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py
+-rw-r--r--   0        0        0     3076 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     7834 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py
+-rw-r--r--   0        0        0      829 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py
+-rw-r--r--   0        0        0    12801 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     8628 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py
+-rw-r--r--   0        0        0     1153 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py
+-rw-r--r--   0        0        0    12807 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3671 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py
+-rw-r--r--   0        0        0      572 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py
+-rw-r--r--   0        0        0     3547 2023-07-06 21:43:41.147624 gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    14909 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py
+-rw-r--r--   0        0        0    11616 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0     4544 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py
+-rw-r--r--   0        0        0      631 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py
+-rw-r--r--   0        0        0     6001 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py
+-rw-r--r--   0        0        0    12321 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0     6939 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py
+-rw-r--r--   0        0        0      642 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py
+-rw-r--r--   0        0        0    10751 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     4677 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py
+-rw-r--r--   0        0        0      610 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py
+-rw-r--r--   0        0        0     6741 2023-07-06 21:43:41.151624 gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py
+-rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.4.0/PKG-INFO
```

### Comparing `gridworks_atn-0.3.8/LICENSE` & `gridworks_atn-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/README.md` & `gridworks_atn-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/pyproject.toml` & `gridworks_atn-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-atn"
-version = "0.3.8"
+version = "0.4.0"
 description = "Gridworks Atn Spaceheat"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "None"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-atn"
 repository = "https://github.com/thegridelectric/gridworks-atn"
 documentation = "https://gridworks-atn.readthedocs.io"
@@ -24,15 +24,14 @@
 numpy = "^1.23.4"
 #gridworks-proactor = "0.2.2"
 #gridworks = { path = "../gridworks"}
 gridworks-proactor = "^0.2.2"
 gridworks-ps = "^0.0.1"
 
 
-
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
 flake8-bandit = ">=2.1.2"
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/__init__.py` & `gridworks_atn-0.4.0/src/gwatn/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/api_types.py` & `gridworks_atn-0.4.0/src/gwatn/api_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ List of all the types used"""
 from typing import Dict
 from typing import List
 from typing import no_type_check
 
 from gwatn.types import AcceptedBid_Maker
 from gwatn.types import AtnBid_Maker
+from gwatn.types import AtnOutsideTempRegrCoeffs_Maker
 from gwatn.types import AtnParams_Maker
 from gwatn.types import AtnParamsBrickstorageheater_Maker
 from gwatn.types import AtnParamsReport_Maker
 from gwatn.types import AtnParamsSimpleresistivehydronic_Maker
 from gwatn.types import BaseGNodeGt_Maker
 from gwatn.types import BasegnodeScadaCreate_Maker
 from gwatn.types import ComponentAttributeClassGt_Maker
@@ -86,14 +87,15 @@
 
 
 @no_type_check
 def type_makers() -> List[HeartbeatA_Maker]:
     return [
         AcceptedBid_Maker,
         AtnBid_Maker,
+        AtnOutsideTempRegrCoeffs_Maker,
         AtnParams_Maker,
         AtnParamsBrickstorageheater_Maker,
         AtnParamsReport_Maker,
         AtnParamsSimpleresistivehydronic_Maker,
         BaseGNodeGt_Maker,
         BasegnodeScadaCreate_Maker,
         ComponentAttributeClassGt_Maker,
@@ -177,14 +179,15 @@
     Returns:
         Dict[str, str]: Keys are TypeNames, values are versions
     """
 
     v: Dict[str, str] = {
         "accepted.bid": "000",
         "atn.bid": "001",
+        "atn.outside.temp.regr.coeffs": "000",
         "atn.params": "000",
         "atn.params.brickstorageheater": "000",
         "atn.params.report": "000",
         "atn.params.simpleresistivehydronic": "000",
         "base.g.node.gt": "002",
         "basegnode.scada.create": "000",
         "component.attribute.class.gt": "000",
@@ -266,14 +269,15 @@
     Returns:
         Dict[str, str]: Keys are versioned TypeNames, values are type status
     """
 
     v: Dict[str, str] = {
         "accepted.bid.000": "Active",
         "atn.bid.001": "Active",
+        "atn.outside.temp.regr.coeffs.000": "Pending",
         "atn.params.000": "Active",
         "atn.params.brickstorageheater.000": "Active",
         "atn.params.report.000": "Active",
         "atn.params.simpleresistivehydronic.000": "Pending",
         "base.g.node.gt.002": "Active",
         "basegnode.scada.create.000": "Active",
         "component.attribute.class.gt.000": "Active",
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/atn_actor_base.py` & `gridworks_atn-0.4.0/src/gwatn/atn_actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/atn_utils.py` & `gridworks_atn-0.4.0/src/gwatn/atn_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/config.py` & `gridworks_atn-0.4.0/src/gwatn/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/.DS_Store` & `gridworks_atn-0.4.0/src/gwatn/data_classes/.DS_Store`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/__init__.py` & `gridworks_atn-0.4.0/src/gwatn/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/d_edge.py` & `gridworks_atn-0.4.0/src/gwatn/data_classes/d_edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/d_graph.py` & `gridworks_atn-0.4.0/src/gwatn/data_classes/d_graph.py`

 * *Files 18% similar despite different names*

```diff
@@ -39,29 +39,72 @@
         starting_store_idx: int,
         home_city: str,
         currency_unit: RecognizedCurrencyUnit,
         max_storage: float,
         max_power_in: float,
         wh_exponent: int = 3,
     ):
+        """
+
+        Args:
+            d_graph_id:
+            graph_strategy_alias:
+            flo_start_unix_time_s:
+            slice_duration_hrs:
+            timezone_string:
+            default_storage_steps:
+            starting_store_idx:
+            home_city:
+            currency_unit:
+            max_storage:
+            max_power_in:
+            wh_exponent:
+
+        """
         self.graph_strategy_alias = graph_strategy_alias
         self.starting_store_idx = starting_store_idx
-        self.edges: Dict[
-            DNode, List[DEdge]
-        ] = (
-            {}
-        )  # a dictionary that takes nodes to lists of edges connecting that node to nodes in the next time slice
-        self.best_edge: Dict[
-            DNode, DEdge
-        ] = {}  # a dictionary that takes node to its best edge in the dijsktra path
-        self.node: Dict[
-            int, Dict[int, DNode]
-        ] = (
-            {}
-        )  # self.node[jj][kk] is the node with time slice index jj and energy index kk
+
+        self.node: Dict[int, Dict[int, DNode]] = {}
+        """
+        self.node is a dictionary representing the nodes in the graph.
+
+        The dictionary structure is as follows:
+        - The outer dictionary's keys represent the time slice index (jj).
+        - The inner dictionary's keys represent the energy index (kk).
+        - The corresponding value is the node with the given time slice index (jj) and energy index (kk).
+
+        Example usage: self.node[jj][kk] returns the node with time slice index jj and energy index kk.
+        """
+
+        self.edge: Dict[int, Dict[int, Dict[int, DEdge]]] = {}
+        """
+        self.edge is a dictionary representing the edges in the graph. Each edge is an object
+        determined by its starting timeslice index (start_ts_idx), its starting store index
+        (start_idx) and its ending store index (end_idx)
+
+        The dictionary structure as follows:
+        - The first key represents the starting timeslice index
+        - The second key represents the starting store index
+        - The third key represents the final store index
+
+        Example usage: self.edge[ts_idx][start_idx][end_idx] returns the edge starting at the node
+        with time slice index start_ts_idx and store index start_idx, and ending with the node
+        with time slice index start_ts_idx + 1 and store end_idx.
+        """
+
+        self.best_edge: Dict[DNode, DEdge] = {}
+        """
+        self.best_edge[node] is the optimal edge choice going forward from node.
+
+        That is, its a dictionary mapping each node to the best next edge on the least-cost path
+        going forward to the end of the graph from that node. This dictionary is filled out in the
+        `solve_dijkstra` method, as the key step in using Dijkstra's algorithm, which solves
+        for the least-cost path not only for the starting node but for all nodes in the graph.
+        """
+
         self.slice_duration_hrs = slice_duration_hrs
         self.time_slices: int = len(self.slice_duration_hrs)
         self.default_storage_steps = default_storage_steps
         self.storage_steps: Dict[int, int] = {}
         self.set_storage_steps_per_time_slice()
         self.flo_start_unix_time_s: int = flo_start_unix_time_s
         self.timezone_string: str = timezone_string
@@ -118,15 +161,15 @@
         self.set_final_slice_benefits()
         last_bad_slice_found = False
         for mm in range(1, self.time_slices + 1):
             # start from the last time slice and work to the front
             ts_idx = self.time_slices - mm
             bad_slice = True
             for node in self.node[ts_idx].values():
-                edges = self.edges[node]
+                edges = list(self.edge[ts_idx][node.store_idx].values())
                 # options gives a list of edge choices along with the cost of the path
                 # from the node assuming that this edge is chosen, and that from that point
                 # on the optimal path is chosen.
 
                 # The path cost is the sum of the local cost at the current node, the
                 # edge cost of the edge choice, and the path cost of the node in the next
                 # time slice.
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/d_node.py` & `gridworks_atn-0.4.0/src/gwatn/data_classes/d_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/hack_price_method.py` & `gridworks_atn-0.4.0/src/gwatn/data_classes/hack_price_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_location.py` & `gridworks_atn-0.4.0/src/gwatn/data_classes/hack_weather_location.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/data_classes/hack_weather_source.py` & `gridworks_atn-0.4.0/src/gwatn/data_classes/hack_weather_source.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/demo_methods.py` & `gridworks_atn-0.4.0/src/gwatn/demo_methods.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_discoverer.py` & `gridworks_atn-0.4.0/src/gwatn/dev_utils/dev_discoverer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_ta_owner.py` & `gridworks_atn-0.4.0/src/gwatn/dev_utils/dev_ta_owner.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dev_utils/dev_validator.py` & `gridworks_atn-0.4.0/src/gwatn/dev_utils/dev_validator.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dev_utils/make_plants.py` & `gridworks_atn-0.4.0/src/gwatn/dev_utils/make_plants.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dispatch_contract.py` & `gridworks_atn-0.4.0/src/gwatn/dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/application.json` & `gridworks_atn-0.4.0/src/gwatn/dispatch_contract_artifacts/application.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/approval.teal` & `gridworks_atn-0.4.0/src/gwatn/dispatch_contract_artifacts/approval.teal`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/dispatch_contract_artifacts/contract.json` & `gridworks_atn-0.4.0/src/gwatn/dispatch_contract_artifacts/contract.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/enums/__init__.py` & `gridworks_atn-0.4.0/src/gwatn/enums/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 from gwproto.enums.role import Role
 from gwproto.enums.telemetry_name import TelemetryName
 from gwproto.enums.unit import Unit
 
 # From gwatn
 from gwatn.enums.distribution_tariff import DistributionTariff
 from gwatn.enums.energy_supply_type import EnergySupplyType
+
+# hacks
+from gwatn.enums.hack_price_method import PriceMethod
+from gwatn.enums.hack_recognized_p_node_alias import RecognizedPNodeAlias
+from gwatn.enums.hack_weather_method import WeatherMethod
+from gwatn.enums.hack_weather_source import WeatherSource
 from gwatn.enums.recognized_irradiance_type import RecognizedIrradianceType
 from gwatn.enums.recognized_temperature_unit import RecognizedTemperatureUnit
 
 
 __all__ = [
     "ActorClass",
     "AlgoCertType",
@@ -52,8 +58,12 @@
     "RecognizedTemperatureUnit",
     "Role",
     "StrategyName",
     "SupervisorContainerStatus",
     "TelemetryName",
     "Unit",
     "UniverseType",
+    "PriceMethod",
+    "RecognizedPNodeAlias",
+    "WeatherMethod",
+    "WeatherSource",
 ]
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/enums/distribution_tariff.py` & `gridworks_atn-0.4.0/src/gwatn/enums/distribution_tariff.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 class DistributionTariff(StrEnum):
     """
     Name of distribution tariff of local network company/utility
 
     Choices and descriptions:
 
       * Unknown:
-      * VersantA1StorageHeatTariff: Versant is a utility serving customers in Maine, and in particular serves much of the area behind the Keene Rd Constraint in the [GridWorks Millinocket Demo](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html#background). Alternately known as the "Home Eco Rate With Bonus Meter, Time-of-Use". Look for rate A1 in Versant [rate schedules](https://www.versantpower.com/residential/rates/rates-schedules/); details are also available [here](https://drive.google.com/drive/u/0/folders/1mhIeNj2JWVyIJrQnSHmBDOkBpNnRRVKB). More: Service under this rate will be available to residential customers with thermal energy storage devices, electric battery storage devices, and/or vehicle chargers who agree to install a second metered point of delivery. The customer will be subject to inspections to ensure that the thermal storage device, electric battery storage device, and electric vehicle charger(s) are sized appropriately for residential use. If the thermal storage device, electric battery storage device, and electric vehicle charger(s) do not pass Company inspection, then the service will be denied. Service will be single-phase, alternating current, 60 hertz, at one standard secondary distribution voltage. Customers taking service under this rate schedule are responsible for paying both Distribution Service and Stranded Cost.. [More Info](https://github.com/thegridelectric/gridworks-ps/blob/dev/input_data/electricity_prices/isone/distp__w.isone.stetson__2020__gw.me.versant.a1.res.ets.csv).
+      * VersantA1StorageHeatTariff: Versant is a utility serving customers in Maine, and in particular serves much of the area behind the Keene Rd Constraint in the [GridWorks Millinocket Demo](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html#background). Alternately known as the 'Home Eco Rate With Bonus Meter, Time-of-Use.' Look for rate A1 in Versant [rate schedules](https://www.versantpower.com/residential/rates/rates-schedules/); details are also available [here](https://drive.google.com/drive/u/0/folders/1mhIeNj2JWVyIJrQnSHmBDOkBpNnRRVKB). More: Service under this rate will be available to residential customers with thermal energy storage devices, electric battery storage devices, and/or vehicle chargers who agree to install a second metered point of delivery. The customer will be subject to inspections to ensure that the thermal storage device, electric battery storage device, and electric vehicle charger(s) are sized appropriately for residential use. If the thermal storage device, electric battery storage device, and electric vehicle charger(s) do not pass Company inspection, then the service will be denied. Service will be single-phase, alternating current, 60 hertz, at one standard secondary distribution voltage. Customers taking service under this rate schedule are responsible for paying both Distribution Service and Stranded Cost. See attached csv for instantiation of this rate as an 8760.. [More Info](https://github.com/thegridelectric/gridworks-ps/blob/dev/input_data/electricity_prices/isone/distp__w.isone.stetson__2022__gw.me.versant.a1.res.ets.csv).
       * VersantATariff: Versant is a utility serving customers in Maine, and in particular serves much of the area behind the Keene Rd Constraint in the [GridWorks Millinocket Demo](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html#background). The A Tariff is their standard residential tariff. Look for rate A in Versant [rate schedules](https://www.versantpower.com/residential/rates/rates-schedules/)
-      * VersantA20HeatTariff:
+      * VersantA20HeatTariff: Versant is a utility serving customers in Maine, and in particular serves much of the area behind the Keene Rd Constraint in the [GridWorks Millinocket Demo](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html#background). This is an alternative tariff available for electric heat.
     """
 
     Unknown = auto()
     VersantA1StorageHeatTariff = auto()
     VersantATariff = auto()
     VersantA20HeatTariff = auto()
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/enums/energy_supply_type.py` & `gridworks_atn-0.4.0/src/gwatn/enums/energy_supply_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/enums/hack_price_method.py` & `gridworks_atn-0.4.0/src/gwatn/enums/hack_price_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/enums/hack_weather_method.py` & `gridworks_atn-0.4.0/src/gwatn/enums/hack_weather_method.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/enums/recognized_irradiance_type.py` & `gridworks_atn-0.4.0/src/gwatn/enums/recognized_irradiance_type.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/enums/recognized_temperature_unit.py` & `gridworks_atn-0.4.0/src/gwatn/enums/recognized_temperature_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.json` & `gridworks_atn-0.4.0/src/gwatn/python_ta_daemon.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/python_ta_daemon.py` & `gridworks_atn-0.4.0/src/gwatn/python_ta_daemon.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/scada_codec.py` & `gridworks_atn-0.4.0/src/gwatn/scada_codec.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/simple_atn_actor.py` & `gridworks_atn-0.4.0/src/gwatn/simple_atn_actor.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/atn.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/atn.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
             LOGGER.exception("Error in update_power_levels")
         payload = Snapshot_Maker(
             from_g_node_alias=self.alias,
             from_g_node_instance_id=self.g_node_instance_id,
             power_watts=self._power_watts,
             store_kwh=int(self.store_kwh),
             max_store_kwh=int(
-                strategy_utils.get_max_store_kwh_th(
+                strategy_utils.get_max_energy_kwh(
                     max_brick_temp_c=self.atn_params.MaxBrickTempC,
                     c=self.atn_params.C,
                     room_temp_f=self.atn_params.RoomTempF,
                 )
             ),
             about_terminal_asset_alias=self.alias + ".ta",
         ).tuple
@@ -315,15 +315,15 @@
         try:
             store_idx = flo.node[0][flo.starting_store_idx].best_next_idx
         except:
             raise Exception(f"Flo node did not have best_node_idx!")
         # self.store_kwh = ...
         self.store_kwh = (
             store_idx
-            * strategy_utils.get_max_store_kwh_th(
+            * strategy_utils.get_max_energy_kwh(
                 max_brick_temp_c=self.atn_params.MaxBrickTempC,
                 c=self.atn_params.C,
                 room_temp_f=self.atn_params.RoomTempF,
             )
             / self.atn_params.StorageSteps
         )
         # LOGGER.info(
@@ -500,13 +500,13 @@
     # TerminalAsset properties
     #################
 
     def store_idx(self) -> int:
         return round(
             self.atn_params.StorageSteps
             * self.store_kwh
-            / strategy_utils.get_max_store_kwh_th(
+            / strategy_utils.get_max_energy_kwh(
                 max_brick_temp_c=self.atn_params.MaxBrickTempC,
                 c=self.atn_params.C,
                 room_temp_f=self.atn_params.RoomTempF,
             )
         )
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/dev_io.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/dev_io.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/edge.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/flo.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if self.params.IsRegulating:
             self.reg_price_per_mwh = np.array(self.params.RegulationPrice)
         else:
             self.reg_price_per_mwh = np.array(
                 [0] * len(self.params.RealtimeElectricityPrice)
             )
 
-        self.max_energy_kwh_th = strategy_utils.get_max_store_kwh_th(self.params)
+        self.max_energy_kwh_th = strategy_utils.get_max_energy_kwh(self.params)
 
         self.currency_unit = self.params.CurrencyUnit
         self.temp_unit = self.params.TempUnit
         DGraph.__init__(
             self,
             d_graph_id=d_graph_id,
             graph_strategy_alias="SpaceHeat__HeatPumpWithBoostStore__Flo",
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/flo_output.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/flo_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,18 +432,18 @@
     w.write("D7", "MaxStoreTempF", bold)
     w.write("E7", flo.params.MaxStoreTempF)
 
     w.write("D8", "ZeroPotentialEnergyWaterTempF", bold)
     w.write("E8", flo.params.ZeroPotentialEnergyWaterTempF)
 
     w.write("D9", "TotalStorageKwh", derived_format_bold)
-    w.write("E9", round(flo.max_energy_kwh_th, 1), derived_format)
+    w.write("E9", round(flo.max_energy_kwh, 1), derived_format)
 
     w.write("D10", "TotalStorage BTU", derived_format_bold)
-    w.write("E10", round(cf.BTU_PER_KWH * flo.max_energy_kwh_th), derived_format)
+    w.write("E10", round(cf.BTU_PER_KWH * flo.max_energy_kwh), derived_format)
 
     w.write("D12", "EmitterPumpFeedbackModel", bold)
     w.write("E12", flo.params.EmitterPumpFeedbackModel.value)
 
     w.write("D13", "MixingValveFeedbackModel", bold)
     w.write("E13", flo.params.MixingValveFeedbackModel.value)
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/make_dev_input_data.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/make_dev_input_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/node.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/brick_storage_heater/strategy_utils.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/brick_storage_heater/strategy_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/atn.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/atn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-""" BrickStorageHeater AtomicTNode Strategy.
+""" SimpleResistiveHydronic AtomicTNode Strategy.
 
- This is a heating and bidding strategy for a thermal storage heater that is
- designed to heat part or all of a single room. The storage medium is ceramic
- bricks and the heating source is resistive elements embedded in those bricks.
-
- This kind of heater is often called a Night Storage Heater in the UK, and
- is often also referred to (ambigiously, since there are other kinds) as
- an Electric Thermal Storage (ETS) heater.
+ This is a heating and bidding strategy for a simple resistive hydronic heating
+ system: one or more 120 gallon domestic hot water tanks heated with resistive
+ elements and providing hot water to a hydronic heating system.
+
+ [schematic](https://gridworks-atn.readthedocs.io/en/latest/simple-resistive-hydronic.html)
  """
 import functools
 import logging
 import math
 import random
 import time
 import uuid
@@ -24,31 +22,31 @@
 import requests
 from algosdk import encoding
 from algosdk.future import transaction
 from algosdk.v2client.algod import AlgodClient
 from gridworks.algo_utils import BasicAccount
 from gridworks.data_classes.market_type import Rt60Gate30B
 from gridworks.utils import RestfulResponse
+from satn.strategies.simple_resistive_hydronic import Edge__BrickStorageHeater as Edge
 
 import gwatn.atn_utils as atn_utils
 import gwatn.brick_storage_heater.dev_io as dev_io
 import gwatn.brick_storage_heater.strategy_utils as strategy_utils
 import gwatn.config as config
 from gwatn.atn_actor_base import AtnActorBase
-from gwatn.brick_storage_heater.edge import Edge__BrickStorageHeater as Edge
 from gwatn.brick_storage_heater.flo import Flo__BrickStorageHeater as Flo
 from gwatn.brick_storage_heater.strategy_utils import SlotStuff
 from gwatn.enums import GNodeRole
 from gwatn.enums import MessageCategory
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
 from gwatn.types import AcceptedBid_Maker
 from gwatn.types import AtnParams
-from gwatn.types import AtnParamsBrickstorageheater
 from gwatn.types import AtnParamsReport_Maker
+from gwatn.types import AtnParamsSimpleresistivehydronic
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import LatestPrice
 from gwatn.types import MarketSlot
 from gwatn.types import MarketTypeGt
 from gwatn.types import MarketTypeGt_Maker
 from gwatn.types import PriceQuantityUnitless
@@ -62,26 +60,25 @@
     "-35s %(lineno) -5d: %(message)s"
 )
 LOGGER = logging.getLogger(__name__)
 
 LOGGER.setLevel(logging.WARNING)
 
 
-class Atn__BrickStorageHeater(AtnActorBase):
-    """AtomicTNode HeatPumpWithBoostStore strategy for thermal storage heat pump
-    space heating system"""
+class Atn__SimpleResistiveHydronic(AtnActorBase):
+    """AtomicTNode SimpleResistiveHydronic strategy"""
 
     def __init__(
         self,
         settings: config.AtnSettings = config.AtnSettings(
             _env_file=dotenv.find_dotenv()
         ),
     ):
         super().__init__(settings)
-        LOGGER.info("Initializing HeatPumpWithBoostStore Atn")
+        LOGGER.info("Initializing SimpleResistiveHydronic Atn")
         self.algo_acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
         self.algo_client: AlgodClient = AlgodClient(
             settings.algo_api_secrets.algod_token.get_secret_value(),
             settings.public.algod_address,
         )
         if self.universe_type == UniverseType.Dev:
             self.atn_params: AtnParamsBrickstorageheater = (
@@ -243,15 +240,15 @@
             LOGGER.exception("Error in update_power_levels")
         payload = Snapshot_Maker(
             from_g_node_alias=self.alias,
             from_g_node_instance_id=self.g_node_instance_id,
             power_watts=self._power_watts,
             store_kwh=int(self.store_kwh),
             max_store_kwh=int(
-                strategy_utils.get_max_store_kwh_th(
+                strategy_utils.get_max_energy_kwh(
                     max_brick_temp_c=self.atn_params.MaxBrickTempC,
                     c=self.atn_params.C,
                     room_temp_f=self.atn_params.RoomTempF,
                 )
             ),
             about_terminal_asset_alias=self.alias + ".ta",
         ).tuple
@@ -315,15 +312,15 @@
         try:
             store_idx = flo.node[0][flo.starting_store_idx].best_next_idx
         except:
             raise Exception(f"Flo node did not have best_node_idx!")
         # self.store_kwh = ...
         self.store_kwh = (
             store_idx
-            * strategy_utils.get_max_store_kwh_th(
+            * strategy_utils.get_max_energy_kwh(
                 max_brick_temp_c=self.atn_params.MaxBrickTempC,
                 c=self.atn_params.C,
                 room_temp_f=self.atn_params.RoomTempF,
             )
             / self.atn_params.StorageSteps
         )
         # LOGGER.info(
@@ -500,13 +497,13 @@
     # TerminalAsset properties
     #################
 
     def store_idx(self) -> int:
         return round(
             self.atn_params.StorageSteps
             * self.store_kwh
-            / strategy_utils.get_max_store_kwh_th(
+            / strategy_utils.get_max_energy_kwh(
                 max_brick_temp_c=self.atn_params.MaxBrickTempC,
                 c=self.atn_params.C,
                 room_temp_f=self.atn_params.RoomTempF,
             )
         )
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/dev_io.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/dev_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 import os
 import typing
 import uuid
 from typing import List
 from typing import Optional
 
 import pendulum
-import satn.strategies.heatpumpwithbooststore.strategy_utils as strategy_utils
 from pydantic import BaseModel
-from satn.strategies.heatpumpwithbooststore.strategy_utils import SlotStuff
-from satn.types import AtnParamsHeatpumpwithbooststore as AtnParams
-from satn.types import AtnParamsHeatpumpwithbooststore_Maker as AtnParams_Maker
-from satn.types import FloParamsHeatpumpwithbooststore as FloParams
 
 import gwatn.atn_utils as atn_utils
+import gwatn.strategies.simple_resistive_hydronic.strategy_utils as strategy_utils
+from gwatn.strategies.simple_resistive_hydronic.strategy_utils import SlotStuff
 from gwatn.types import AtnBid
 from gwatn.types import AtnParamsReport_Maker
+from gwatn.types import AtnParamsSimpleresistivehydronic as AtnParams
+from gwatn.types import AtnParamsSimpleresistivehydronic_Maker as AtnParams_Maker
+from gwatn.types import FloParamsSimpleresistivehydronic as FloParams
 from gwatn.types import MarketSlot
 from gwatn.types.ps_distprices_gnode.csv_distp_sync.csv_distp_sync_1_0_0 import (
     Csv_Distp_Sync_1_0_0,
 )
 from gwatn.types.ps_electricityprices_gnode.csv_eprt_sync.csv_eprt_sync_1_0_0 import (
     Csv_Eprt_Sync_1_0_0,
 )
@@ -36,16 +36,16 @@
 )
 LOGGER = logging.getLogger(__name__)
 
 LOGGER.setLevel(logging.WARNING)
 DATA_DIR = "input_data"
 EVENTSTORE_DIR = f"{DATA_DIR}/eventstore"
 
-ELEC_PRICE_FILE = "input_data/electricity_prices/isone/eprt__w.isone.stetson__2020.csv"
-DIST_PRICE_FILE = "input_data/electricity_prices/isone/distp__w.isone.stetson__2020__gw.me.versant.a1.res.ets.csv"
+ELEC_PRICE_FILE = "../gridworks-ps/input_data/electricity_prices/isone/eprt__w.isone.stetson__2020.csv"
+DIST_PRICE_FILE = "../gridworks-ps/input_data/electricity_prices/isone/distp__w.isone.stetson__2020__gw.me.versant.a1.res.ets.csv"
 WEATHER_PRICE_FILE = (
     "input_data/weather/us/me/temp__ws.us.me.millinocketairport__2020.csv"
 )
 HEAT_PROFILE_FILE = "input_data/dev_heat_profile_data.csv"
 
 
 class FileNameMeta(BaseModel):
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/edge.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/edge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-""" Heatpumpwithbooststore Flo Edge Class Definition """
+""" SimpleResistiveHydronic Flo Edge Class Definition """
 from typing import Optional
 from typing import no_type_check
 
 from gwatn.data_classes.d_edge import DEdge
 
 
 SIG_FIGS_FOR_OUTPUT = 6
 
 
-class Edge__BrickStorageHeater(DEdge):
+class Edge_SimpleResistiveHydronic(DEdge):
     def __init__(
         self,
         start_ts_idx: int,
         start_idx: int,
         end_idx: int,
         avg_kw: Optional[float] = None,
         cost: Optional[float] = None,
@@ -25,9 +25,11 @@
             cost=cost,
         )
         self.avg_kw = avg_kw
 
     def __repr__(self) -> str:
         rep = f"DEdge => Time Slice Idx: {self.start_ts_idx}, StartIdx: {self.start_idx}, EndIdx: {self.end_idx}"
         if self.cost is not None:
-            rep += f" Cost => {self.cost}"
+            rep += f", Cost => ${round(self.cost, 3)}"
+        if self.avg_kw is not None:
+            rep += f", Avg Power => {round(self.avg_kw, 2)} kW"
         return rep
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/flo_output.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/flo_output.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 import time
 
 import gridworks.conversion_factors as cf
 import pendulum
 import xlsxwriter
 
-import gwatn.brick_storage_heater.strategy_utils as strategy_utils
-from gwatn.brick_storage_heater.edge import Edge__BrickStorageHeater as Edge
-from gwatn.brick_storage_heater.flo import Flo__BrickStorageHeater as Flo
-from gwatn.brick_storage_heater.node import Node_BrickStorageHeater as Node
 from gwatn.enums import RecognizedCurrencyUnit
+from gwatn.strategies.simple_resistive_hydronic.edge import (
+    Edge_SimpleResistiveHydronic as Edge,
+)
+from gwatn.strategies.simple_resistive_hydronic.flo import (
+    Flo_SimpleResistiveHydronic as Flo,
+)
+from gwatn.strategies.simple_resistive_hydronic.node import (
+    Node_SimpleResistiveHydronic as Node,
+)
 from gwatn.types import AtnParamsBrickstorageheater as AtnParams
 
 
 OUTPUT_FOLDER = "output_data"
 
 ON_PEAK_DIST_PRICE_PER_MWH_CUTOFF = 100
 SHOULDER_PEAK_DIST_PRICE_PER_MWH_CUTOFF = 50
@@ -118,45 +123,35 @@
     w.write(7, 0, "Outside Temp F", header_format)
     w.write(
         7,
         1,
         round(sum(flo.params.OutsideTempF) / len(flo.params.OutsideTempF), 2),
         bold_format,
     )
-    w.write(8, 0, "COP", header_format)
-    avg_cop = sum(flo.cop.values()) / len(flo.cop)
-    w.write(8, 1, round(avg_cop, 2), bold_format)
-    w.write(9, 0, "House Power Required AvgKw", header_format)
+
+    w.write(9, 0, "Power Lost From House AvgKw", header_format)
     w.write(
         9,
         1,
-        round(sum(flo.params.PowerRequiredByHouseFromSystemAvgKwList), 2),
+        round(sum(flo.params.PowerLostFromHouseKwList), 2),
         bold_format,
     )
     w.write(10, 0, "Required Source Water Temp F", header_format)
-    avg_swt = round((sum(swt_list) / len(swt_list)), 0)
-    w.write(10, 1, avg_swt, bold_format)
-    w.write(11, 0, "Max HeatPump kWh thermal", header_format)
-    avg_max_thermal_hp_kwh = round(
-        (sum(flo.max_thermal_hp_kwh.values()) / len(flo.max_thermal_hp_kwh)), 2
-    )
-    w.write(11, 1, avg_max_thermal_hp_kwh, bold_format)
+    swt = flo.params.RequiredSourceWaterTempF
+    w.write(10, 1, swt, bold_format)
 
     w.write(12, 0, "Outputs", header_format)
 
     for jj in range(flo.time_slices):
         hours_since_start = sum(flo.slice_duration_hrs[0:jj])
         local_time = local_start.add(hours=hours_since_start)
         w.write(2, jj + 2, local_time.strftime("%m/%d"))
         w.write(3, jj + 2, local_time.strftime("%H:%M"))
         w.write(4, jj + 2, flo.RealtimeElectricityPrice[jj], currency_format)
-        if flo.params.IsRegulating:
-            w.write(5, jj + 2, flo.reg_price_per_mwh[jj], currency_format)
-        else:
-            w.write(5, jj + 2, "", gray_filler_format)
+        w.write(5, jj + 2, "", gray_filler_format)
         dp = flo.DistributionPrice[jj]
         LIGHT_GREEN_HEX = "#bbe3a6"
         LIGHT_RED_HEX = "#ff6363"
         if dp > ON_PEAK_DIST_PRICE_PER_MWH_CUTOFF:
             if flo.params.CurrencyUnit == RecognizedCurrencyUnit.USD:
                 dist_format = workbook.add_format(
                     {"bg_color": LIGHT_RED_HEX, "num_format": "$#,##0.00"}
@@ -191,15 +186,15 @@
                 )
         w.write(6, jj + 2, flo.DistributionPrice[jj], dist_format)
         w.write(7, jj + 2, flo.params.OutsideTempF[jj])
         w.write(8, jj + 2, flo.cop[jj])
         w.write(
             9, jj + 2, round(flo.params.PowerRequiredByHouseFromSystemAvgKwList[jj], 2)
         )
-        w.write(10, jj + 2, round(swt_list[jj], 0))
+        w.write(10, jj + 2, round(swt, 0))
         w.write(11, jj + 2, round(flo.max_thermal_hp_kwh[jj], 2))
 
         w.write(12, jj + 2, "", gray_filler_format)
 
     node: Node = flo.node[0][starting_store_idx]
     w.write(OPT_PATH_STATE_VAR_ROW, 0, "Store Temp (F)", header_format)
     w.write(OPT_PATH_STATE_VAR_ROW + 1, 0, "HeatPump kWh thermal", header_format)
@@ -212,21 +207,20 @@
     opt_heatpump_electricity_used_kwh = []
     opt_boost_electricity_used_kwh = []
     opt_energy_cost_dollars = []
 
     best_idx = starting_store_idx
     dist_cost = []
     min_dist_price_per_mwh = min(flo.DistributionPrice)
-
+    slice_duration = flo.params.Slice
     for jj in range(flo.time_slices):
         edge: Edge = flo.best_edge[node]
         store_temp_f.append(node.store_avg_water_temp_f)
-        hp_kwh = edge.hp_electricity_avg_kw
+        kwh = edge.avg_kw
         boost_kwh = edge.boost_electricity_used_avg_kw
-        opt_heatpump_electricity_used_kwh.append(hp_kwh)
         opt_boost_electricity_used_kwh.append(boost_kwh)
         opt_energy_cost_dollars.append(edge.cost)
         hours_since_start = sum(flo.slice_duration_hrs[0:jj])
 
         w.write(OPT_PATH_STATE_VAR_ROW, jj + 2, round(node.store_avg_water_temp_f, 2))
         w.write(
             OPT_PATH_STATE_VAR_ROW + 1,
@@ -342,15 +336,15 @@
     atn_params: AtnParams,
     workbook: xlsxwriter.workbook.Workbook,
 ):
     bold = workbook.add_format({"bold": True})
     w = workbook.add_worksheet("Params")
     derived_format_bold = workbook.add_format({"bold": True, "font_color": "green"})
     derived_format = workbook.add_format({"font_color": "green"})
-    swt_list = flo_utils.get_source_water_temp_f_list(flo.params)
+
     w.set_column("A:A", 31)
     w.set_column("D:D", 31)
     w.set_column("G:G", 31)
     w.write("A1", "Key Parameters", bold)
 
     t = flo.params.OutsideTempF
     w.write("A4", "This Run ColdestTempF ", derived_format_bold)
@@ -432,18 +426,18 @@
     w.write("D7", "MaxStoreTempF", bold)
     w.write("E7", flo.params.MaxStoreTempF)
 
     w.write("D8", "ZeroPotentialEnergyWaterTempF", bold)
     w.write("E8", flo.params.ZeroPotentialEnergyWaterTempF)
 
     w.write("D9", "TotalStorageKwh", derived_format_bold)
-    w.write("E9", round(flo.max_energy_kwh_th, 1), derived_format)
+    w.write("E9", round(flo.max_energy_kwh, 1), derived_format)
 
     w.write("D10", "TotalStorage BTU", derived_format_bold)
-    w.write("E10", round(cf.BTU_PER_KWH * flo.max_energy_kwh_th), derived_format)
+    w.write("E10", round(cf.BTU_PER_KWH * flo.max_energy_kwh), derived_format)
 
     w.write("D12", "EmitterPumpFeedbackModel", bold)
     w.write("E12", flo.params.EmitterPumpFeedbackModel.value)
 
     w.write("D13", "MixingValveFeedbackModel", bold)
     w.write("E13", flo.params.MixingValveFeedbackModel.value)
 
@@ -479,13 +473,7 @@
     w.write("A29", "WeatherUid", bold)
     w.write("B29", flo.params.WeatherUid)
     w.write("A31", "RtElecPriceUid", bold)
     w.write("B31", flo.params.RtElecPriceUid)
 
     w.write("A33", "DistPriceUid", bold)
     w.write("B33", flo.params.DistPriceUid)
-
-    if flo.params.IsRegulating:
-        w.write("A34", "LocalRegulationFile", bold)
-        w.write("B34", regp_sync_100_handler.csv_file_by_uid(flo.params.RegPriceUid))
-        w.write("A35", "RegPriceUid", bold)
-        w.write("B35", flo.params.RegPriceUid)
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/make_dev_input_data.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/make_dev_input_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import csv
 import json
 
 import pendulum
-from satn.types import AtnParamsHeatpumpwithbooststore as AtnParams
-from satn.types import AtnParamsHeatpumpwithbooststore_Maker as AtnParams_Maker
 
 from gwatn.types import AtnParamsReport_Maker
+from gwatn.types import AtnParamsSimpleresistivehydronic as AtnParams
+from gwatn.types import AtnParamsSimpleresistivehydronic_Maker as AtnParams_Maker
 
 
 params_file = "input_data/atn_params_data.csv"
 params = []
 with open(params_file) as csv_file:
     reader = csv.reader(csv_file)
     for row in reader:
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/simple_scada_sim.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/simple_scada_sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 from gwatn.types import GwCertId_Maker
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import HeartbeatB
 from gwatn.types import HeartbeatB_Maker
 from gwatn.types import JoinDispatchContract_Maker
 from gwatn.types import ScadaCertTransfer_Maker
-from gwatn.types import SimScadaDriverReportBsh as SimScadaDriverReport
-from gwatn.types import SimScadaDriverReportBsh_Maker as SimScadaDriverReport_Maker
+from gwatn.types import SimplesimDriverReport
+from gwatn.types import SimplesimDriverReport_Maker
 from gwatn.types import SimTimestep
 from gwatn.types import SimTimestep_Maker
 from gwatn.types import SnapshotBrickstorageheater as Snapshot
 
 
 DISPATCH_CONTRACT_REPORTING_ALGOS = 5
 
@@ -191,15 +191,15 @@
                 LOGGER.info(
                     f"Ignoring HeartbeatB from GNode with role {from_role}; expects AtomicTNode"
                 )
             try:
                 self.heartbeat_from_atn(ping=payload)
             except:
                 LOGGER.exception("Error in heartbeat_from_atn")
-        elif payload.TypeName == SimScadaDriverReport_Maker.type_name:
+        elif payload.TypeName == SimplesimDriverReport_Maker.type_name:
             try:
                 self.sim_scada_driver_report_received(payload)
             except:
                 LOGGER.exception("Error in sim_scada_driver_report_received")
         elif payload.TypeName == SimTimestep_Maker.type_name:
             if from_role != GNodeRole.TimeCoordinator:
                 LOGGER.info(
@@ -533,15 +533,15 @@
         self.dc_client.opt_in()
         LOGGER.info(f"Dispatch Contract {self.dc_app_id} is live")
 
     #########################################################
     # Make the below into abstractmethods if pulling out base class
     #########################################################
 
-    def sim_scada_driver_report_received(self, payload: SimScadaDriverReport) -> None:
+    def simplesim_driver_report_received(self, payload: SimplesimDriverReport) -> None:
         """This gets received right before the top of the hour, from our
         best simulation of the TerminalAsset (which is happening in the
         AtomicTNode)."""
         if payload.FromGNodeInstanceId != self.atn_gni_id:
             LOGGER.info(f"Igoring {payload} - incorrect GNodeInstanceId")
         self.power_watts = payload.PowerWatts
         self.store_kwh = payload.StoreKwh
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/strategies/simple_resistive_hydronic/strategy_utils.py` & `gridworks_atn-0.4.0/src/gwatn/strategies/simple_resistive_hydronic/strategy_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Optional
 
-import gridworks.conversion_factors as cf  # TODO change to from gwatn import conversion_factors as cf
 import numpy as np
 from pydantic import BaseModel
-from satn.strategies.heatpumpwithbooststore.flo import (
-    Flo__HeatpumpWithBoostStore as Flo,
-)
-from satn.types import AtnParamsHeatpumpwithbooststore as AtnParams
-from satn.types import FloParamsHeatpumpwithbooststore as FloParams
 
 from gwatn import atn_utils
+from gwatn import conversion_factors as cf
+from gwatn.strategies.simple_resistive_hydronic.flo import (
+    Flo_SimpleResistiveHydronic as Flo,
+)
 from gwatn.types import AtnBid
+from gwatn.types import AtnParamsSimpleresistivehydronic as AtnParams
+from gwatn.types import FloParamsSimpleresistivehydronic as FloParams
 from gwatn.types import MarketSlot
 
 
 #################################
 # Bidding related
 #################################
 
@@ -87,27 +87,14 @@
 
 
 ##########################################
 # Flo prep (uses AtnParams as variable)
 ##########################################
 
 
-def get_k(
-    system_max_heat_output_delta_temp_f: int,
-    system_max_heat_output_gpm: float,
-    system_max_heat_output_swt_f: int,
-    room_temp_f: int,
-) -> float:
-    dt = system_max_heat_output_delta_temp_f
-    gpm = system_max_heat_output_gpm
-    swt = system_max_heat_output_swt_f
-    rt = room_temp_f
-    return float(gpm * np.log(1 - dt / (swt - rt)))
-
-
 def get_system_max_heat_output_kw_avg(
     system_max_heat_output_gpm: float, system_max_heat_output_delta_temp_f: float
 ) -> float:
     """What is the max heat that the system put out?  ASSUMES that the hydronic
     fluid is water.
 
     Args:
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/ta_daemon_rest_api.py` & `gridworks_atn-0.4.0/src/gwatn/ta_daemon_rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/two_channel_actor_base.py` & `gridworks_atn-0.4.0/src/gwatn/two_channel_actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/__init__.py` & `gridworks_atn-0.4.0/src/gwatn/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 )
 
 # From gwatn
 from gwatn.types.accepted_bid import AcceptedBid
 from gwatn.types.accepted_bid import AcceptedBid_Maker
 from gwatn.types.atn_bid import AtnBid
 from gwatn.types.atn_bid import AtnBid_Maker
+from gwatn.types.atn_outside_temp_regr_coeffs import AtnOutsideTempRegrCoeffs
+from gwatn.types.atn_outside_temp_regr_coeffs import AtnOutsideTempRegrCoeffs_Maker
 from gwatn.types.atn_params import AtnParams
 from gwatn.types.atn_params import AtnParams_Maker
 from gwatn.types.atn_params_brickstorageheater import AtnParamsBrickstorageheater
 from gwatn.types.atn_params_brickstorageheater import AtnParamsBrickstorageheater_Maker
 from gwatn.types.atn_params_report import AtnParamsReport
 from gwatn.types.atn_params_report import AtnParamsReport_Maker
 from gwatn.types.atn_params_simpleresistivehydronic import (
@@ -176,14 +178,16 @@
 
 
 __all__ = [
     "AcceptedBid",
     "AcceptedBid_Maker",
     "AtnBid",
     "AtnBid_Maker",
+    "AtnOutsideTempRegrCoeffs",
+    "AtnOutsideTempRegrCoeffs_Maker",
     "AtnParams",
     "AtnParams_Maker",
     "AtnParamsBrickstorageheater",
     "AtnParamsBrickstorageheater_Maker",
     "AtnParamsReport",
     "AtnParamsReport_Maker",
     "AtnParamsSimpleresistivehydronic",
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/accepted_bid.py` & `gridworks_atn-0.4.0/src/gwatn/types/accepted_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/atn_bid.py` & `gridworks_atn-0.4.0/src/gwatn/types/atn_bid.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/atn_params.py` & `gridworks_atn-0.4.0/src/gwatn/types/atn_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/atn_params_brickstorageheater.py` & `gridworks_atn-0.4.0/src/gwatn/types/atn_params_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/atn_params_report.py` & `gridworks_atn-0.4.0/src/gwatn/types/atn_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/atn_params_simpleresistivehydronic.py` & `gridworks_atn-0.4.0/src/gwatn/types/atn_params_simpleresistivehydronic.py`

 * *Files 16% similar despite different names*

```diff
@@ -272,16 +272,16 @@
         title="EnergyType",
         default=EnergySupplyType.RealtimeLocalLmp,
     )
     StandardOfferPriceDollarsPerMwh: int = Field(
         title="StandardOfferPriceDollarsPerMwh",
         default=110,
     )
-    DistributionTariffDollarsPerMwh: int = Field(
-        title="DistributionTariffDollarsPerMwh",
+    FlatDistributionTariffDollarsPerMwh: int = Field(
+        title="FlatDistributionTariffDollarsPerMwh",
         default=113,
     )
     StoreSizeGallons: int = Field(
         title="StoreSizeGallons",
         default=240,
     )
     MaxStoreTempF: int = Field(
@@ -292,20 +292,20 @@
         title="ElementMaxPowerKw",
         default=9.5,
     )
     RequiredSourceWaterTempF: int = Field(
         title="RequiredSourceWaterTempF",
         default=120,
     )
-    FixedPumpGpm: float = Field(
-        title="FixedPumpGpm",
+    CirculatorPumpGpm: float = Field(
+        title="CirculatorPumpGpm",
         default=5.5,
     )
-    ReturnWaterFixedDeltaT: int = Field(
-        title="ReturnWaterFixedDeltaT",
+    ReturnWaterDeltaTempF: int = Field(
+        title="ReturnWaterDeltaTempF",
         default=20,
     )
     AnnualHvacKwhTh: int = Field(
         title="AnnualHvacKwhTh",
         default=25000,
     )
     AmbientPowerInKw: float = Field(
@@ -316,14 +316,22 @@
         title="HouseWorstCaseTempF",
         default=-7,
     )
     RoomTempF: int = Field(
         title="RoomTempF",
         default=68,
     )
+    StorePassiveLossRatio: float = Field(
+        title="StorePassiveLossRatio",
+        default=0.005,
+    )
+    AmbientTempStoreF: int = Field(
+        title="AmbientTempStoreF",
+        default=65,
+    )
     TypeName: Literal[
         "atn.params.simpleresistivehydronic"
     ] = "atn.params.simpleresistivehydronic"
     Version: str = "000"
 
     @validator("GNodeAlias")
     def _check_g_node_alias(cls, v: str) -> str:
@@ -383,48 +391,52 @@
         storage_steps: int,
         flo_slices: int,
         slice_duration_minutes: int,
         currency_unit: RecognizedCurrencyUnit,
         tariff: DistributionTariff,
         energy_type: EnergySupplyType,
         standard_offer_price_dollars_per_mwh: int,
-        distribution_tariff_dollars_per_mwh: int,
+        flat_distribution_tariff_dollars_per_mwh: int,
         store_size_gallons: int,
         max_store_temp_f: int,
         element_max_power_kw: float,
         required_source_water_temp_f: int,
-        fixed_pump_gpm: float,
-        return_water_fixed_delta_t: int,
+        circulator_pump_gpm: float,
+        return_water_delta_temp_f: int,
         annual_hvac_kwh_th: int,
         ambient_power_in_kw: float,
         house_worst_case_temp_f: int,
         room_temp_f: int,
+        store_passive_loss_ratio: float,
+        ambient_temp_store_f: int,
     ):
         self.tuple = AtnParamsSimpleresistivehydronic(
             GNodeAlias=g_node_alias,
             HomeCity=home_city,
             TimezoneString=timezone_string,
             StorageSteps=storage_steps,
             FloSlices=flo_slices,
             SliceDurationMinutes=slice_duration_minutes,
             CurrencyUnit=currency_unit,
             Tariff=tariff,
             EnergyType=energy_type,
             StandardOfferPriceDollarsPerMwh=standard_offer_price_dollars_per_mwh,
-            DistributionTariffDollarsPerMwh=distribution_tariff_dollars_per_mwh,
+            FlatDistributionTariffDollarsPerMwh=flat_distribution_tariff_dollars_per_mwh,
             StoreSizeGallons=store_size_gallons,
             MaxStoreTempF=max_store_temp_f,
             ElementMaxPowerKw=element_max_power_kw,
             RequiredSourceWaterTempF=required_source_water_temp_f,
-            FixedPumpGpm=fixed_pump_gpm,
-            ReturnWaterFixedDeltaT=return_water_fixed_delta_t,
+            CirculatorPumpGpm=circulator_pump_gpm,
+            ReturnWaterDeltaTempF=return_water_delta_temp_f,
             AnnualHvacKwhTh=annual_hvac_kwh_th,
             AmbientPowerInKw=ambient_power_in_kw,
             HouseWorstCaseTempF=house_worst_case_temp_f,
             RoomTempF=room_temp_f,
+            StorePassiveLossRatio=store_passive_loss_ratio,
+            AmbientTempStoreF=ambient_temp_store_f,
             #
         )
 
     @classmethod
     def tuple_to_type(cls, tuple: AtnParamsSimpleresistivehydronic) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
@@ -482,57 +494,65 @@
             d2["EnergyType"] = EnergySupplyTypeMap.type_to_local(
                 d2["EnergyTypeGtEnumSymbol"]
             )
         else:
             d2["EnergyType"] = EnergySupplyType.default()
         if "StandardOfferPriceDollarsPerMwh" not in d2.keys():
             raise SchemaError(f"dict {d2} missing StandardOfferPriceDollarsPerMwh")
-        if "DistributionTariffDollarsPerMwh" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing DistributionTariffDollarsPerMwh")
+        if "FlatDistributionTariffDollarsPerMwh" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FlatDistributionTariffDollarsPerMwh")
         if "StoreSizeGallons" not in d2.keys():
             raise SchemaError(f"dict {d2} missing StoreSizeGallons")
         if "MaxStoreTempF" not in d2.keys():
             raise SchemaError(f"dict {d2} missing MaxStoreTempF")
         if "ElementMaxPowerKw" not in d2.keys():
             raise SchemaError(f"dict {d2} missing ElementMaxPowerKw")
         if "RequiredSourceWaterTempF" not in d2.keys():
             raise SchemaError(f"dict {d2} missing RequiredSourceWaterTempF")
-        if "FixedPumpGpm" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FixedPumpGpm")
-        if "ReturnWaterFixedDeltaT" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing ReturnWaterFixedDeltaT")
+        if "CirculatorPumpGpm" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing CirculatorPumpGpm")
+        if "ReturnWaterDeltaTempF" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing ReturnWaterDeltaTempF")
         if "AnnualHvacKwhTh" not in d2.keys():
             raise SchemaError(f"dict {d2} missing AnnualHvacKwhTh")
         if "AmbientPowerInKw" not in d2.keys():
             raise SchemaError(f"dict {d2} missing AmbientPowerInKw")
         if "HouseWorstCaseTempF" not in d2.keys():
             raise SchemaError(f"dict {d2} missing HouseWorstCaseTempF")
         if "RoomTempF" not in d2.keys():
             raise SchemaError(f"dict {d2} missing RoomTempF")
+        if "StorePassiveLossRatio" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StorePassiveLossRatio")
+        if "AmbientTempStoreF" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing AmbientTempStoreF")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
         return AtnParamsSimpleresistivehydronic(
             GNodeAlias=d2["GNodeAlias"],
             HomeCity=d2["HomeCity"],
             TimezoneString=d2["TimezoneString"],
             StorageSteps=d2["StorageSteps"],
             FloSlices=d2["FloSlices"],
             SliceDurationMinutes=d2["SliceDurationMinutes"],
             CurrencyUnit=d2["CurrencyUnit"],
             Tariff=d2["Tariff"],
             EnergyType=d2["EnergyType"],
             StandardOfferPriceDollarsPerMwh=d2["StandardOfferPriceDollarsPerMwh"],
-            DistributionTariffDollarsPerMwh=d2["DistributionTariffDollarsPerMwh"],
+            FlatDistributionTariffDollarsPerMwh=d2[
+                "FlatDistributionTariffDollarsPerMwh"
+            ],
             StoreSizeGallons=d2["StoreSizeGallons"],
             MaxStoreTempF=d2["MaxStoreTempF"],
             ElementMaxPowerKw=d2["ElementMaxPowerKw"],
             RequiredSourceWaterTempF=d2["RequiredSourceWaterTempF"],
-            FixedPumpGpm=d2["FixedPumpGpm"],
-            ReturnWaterFixedDeltaT=d2["ReturnWaterFixedDeltaT"],
+            CirculatorPumpGpm=d2["CirculatorPumpGpm"],
+            ReturnWaterDeltaTempF=d2["ReturnWaterDeltaTempF"],
             AnnualHvacKwhTh=d2["AnnualHvacKwhTh"],
             AmbientPowerInKw=d2["AmbientPowerInKw"],
             HouseWorstCaseTempF=d2["HouseWorstCaseTempF"],
             RoomTempF=d2["RoomTempF"],
+            StorePassiveLossRatio=d2["StorePassiveLossRatio"],
+            AmbientTempStoreF=d2["AmbientTempStoreF"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/basegnode_scada_create.py` & `gridworks_atn-0.4.0/src/gwatn/types/basegnode_scada_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/data_channel.py` & `gridworks_atn-0.4.0/src/gwatn/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/discoverycert_algo_create.py` & `gridworks_atn-0.4.0/src/gwatn/types/discoverycert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/dispatch_contract_confirmed.py` & `gridworks_atn-0.4.0/src/gwatn/types/dispatch_contract_confirmed.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/epda/gt_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/epda/gt_epda_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/eprt/gt_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/flo_params.py` & `gridworks_atn-0.4.0/src/gwatn/types/flo_params.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/flo_params_brickstorageheater.py` & `gridworks_atn-0.4.0/src/gwatn/types/flo_params_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/flo_params_report.py` & `gridworks_atn-0.4.0/src/gwatn/types/flo_params_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/flo_params_simpleresistivehydronic.py` & `gridworks_atn-0.4.0/src/gwatn/types/market_type_gt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,80 @@
-"""Type flo.params.simpleresistivehydronic, version 000"""
+"""Type market.type.gt, version 000"""
 import json
 from enum import auto
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 
 from fastapi_utils.enums import StrEnum
 from gridworks.errors import SchemaError
 from gridworks.message import as_enum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
+from gwatn.data_classes import MarketType
+from gwatn.enums import MarketPriceUnit
+from gwatn.enums import MarketQuantityUnit
+from gwatn.enums import MarketTypeName
 from gwatn.enums import RecognizedCurrencyUnit
 
 
+class MarketPriceUnit000SchemaEnum:
+    enum_name: str = "market.price.unit.000"
+    symbols: List[str] = [
+        "00000000",
+    ]
+
+    @classmethod
+    def is_symbol(cls, candidate: str) -> bool:
+        if candidate in cls.symbols:
+            return True
+        return False
+
+
+class MarketPriceUnit000(StrEnum):
+    USDPerMWh = auto()
+
+    @classmethod
+    def default(cls) -> "MarketPriceUnit000":
+        return cls.USDPerMWh
+
+    @classmethod
+    def values(cls) -> List[str]:
+        return [elt.value for elt in cls]
+
+
+class MarketPriceUnitMap:
+    @classmethod
+    def type_to_local(cls, symbol: str) -> MarketPriceUnit:
+        if not MarketPriceUnit000SchemaEnum.is_symbol(symbol):
+            raise SchemaError(f"{symbol} must belong to MarketPriceUnit000 symbols")
+        versioned_enum = cls.type_to_versioned_enum_dict[symbol]
+        return as_enum(versioned_enum, MarketPriceUnit, MarketPriceUnit.default())
+
+    @classmethod
+    def local_to_type(cls, market_price_unit: MarketPriceUnit) -> str:
+        if not isinstance(market_price_unit, MarketPriceUnit):
+            raise SchemaError(f"{market_price_unit} must be of type {MarketPriceUnit}")
+        versioned_enum = as_enum(
+            market_price_unit, MarketPriceUnit000, MarketPriceUnit000.default()
+        )
+        return cls.versioned_enum_to_type_dict[versioned_enum]
+
+    type_to_versioned_enum_dict: Dict[str, MarketPriceUnit000] = {
+        "00000000": MarketPriceUnit000.USDPerMWh,
+    }
+
+    versioned_enum_to_type_dict: Dict[MarketPriceUnit000, str] = {
+        MarketPriceUnit000.USDPerMWh: "00000000",
+    }
+
+
 class RecognizedCurrencyUnit000SchemaEnum:
     enum_name: str = "recognized.currency.unit.000"
     symbols: List[str] = [
         "00000000",
         "e57c5143",
         "f7b38fc5",
     ]
@@ -79,223 +134,214 @@
     versioned_enum_to_type_dict: Dict[RecognizedCurrencyUnit000, str] = {
         RecognizedCurrencyUnit000.UNKNOWN: "00000000",
         RecognizedCurrencyUnit000.USD: "e57c5143",
         RecognizedCurrencyUnit000.GBP: "f7b38fc5",
     }
 
 
-def check_is_uuid_canonical_textual(v: str) -> None:
-    """
-    UuidCanonicalTextual format:  A string of hex words separated by hyphens
-    of length 8-4-4-4-12.
+class MarketTypeName000SchemaEnum:
+    enum_name: str = "market.type.name.000"
+    symbols: List[str] = [
+        "00000000",
+        "d20b81e4",
+        "b36cbfb4",
+        "94a3fe9b",
+        "5f335bdb",
+        "01a84101",
+        "e997ccfb",
+        "618f9c0a",
+    ]
 
-    Raises:
-        ValueError: if not UuidCanonicalTextual format
-    """
-    try:
-        x = v.split("-")
-    except AttributeError as e:
-        raise ValueError(f"Failed to split on -: {e}")
-    if len(x) != 5:
-        raise ValueError(f"{v} split by '-' did not have 5 words")
-    for hex_word in x:
-        try:
-            int(hex_word, 16)
-        except ValueError:
-            raise ValueError(f"Words of {v} are not all hex")
-    if len(x[0]) != 8:
-        raise ValueError(f"{v} word lengths not 8-4-4-4-12")
-    if len(x[1]) != 4:
-        raise ValueError(f"{v} word lengths not 8-4-4-4-12")
-    if len(x[2]) != 4:
-        raise ValueError(f"{v} word lengths not 8-4-4-4-12")
-    if len(x[3]) != 4:
-        raise ValueError(f"{v} word lengths not 8-4-4-4-12")
-    if len(x[4]) != 12:
-        raise ValueError(f"{v} word lengths not 8-4-4-4-12")
+    @classmethod
+    def is_symbol(cls, candidate: str) -> bool:
+        if candidate in cls.symbols:
+            return True
+        return False
 
 
-def check_is_left_right_dot(v: str) -> None:
-    """
-    LeftRightDot format: Lowercase alphanumeric words separated by periods,
-    most significant word (on the left) starting with an alphabet character.
+class MarketTypeName000(StrEnum):
+    unknown = auto()
+    rt5gate5 = auto()
+    rt60gate5 = auto()
+    da60 = auto()
+    rt60gate30 = auto()
+    rt15gate5 = auto()
+    rt30gate5 = auto()
+    rt60gate30b = auto()
 
-    Raises:
-        ValueError: if not LeftRightDot format
-    """
-    from typing import List
+    @classmethod
+    def default(cls) -> "MarketTypeName000":
+        return cls.unknown
 
-    try:
-        x: List[str] = v.split(".")
-    except:
-        raise ValueError(f"Failed to seperate {v} into words with split'.'")
-    first_word = x[0]
-    first_char = first_word[0]
-    if not first_char.isalpha():
-        raise ValueError(f"Most significant word of {v} must start with alphabet char.")
-    for word in x:
-        if not word.isalnum():
-            raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
-    if not v.islower():
-        raise ValueError(f"All characters of {v} must be lowercase.")
+    @classmethod
+    def values(cls) -> List[str]:
+        return [elt.value for elt in cls]
 
 
-class FloParamsSimpleresistivehydronic(BaseModel):
-    """ """
+class MarketTypeNameMap:
+    @classmethod
+    def type_to_local(cls, symbol: str) -> MarketTypeName:
+        if not MarketTypeName000SchemaEnum.is_symbol(symbol):
+            raise SchemaError(f"{symbol} must belong to MarketTypeName000 symbols")
+        versioned_enum = cls.type_to_versioned_enum_dict[symbol]
+        return as_enum(versioned_enum, MarketTypeName, MarketTypeName.default())
 
-    GNodeAlias: str = Field(
-        title="GNodeAlias",
-    )
-    FloParamsUid: str = Field(
-        title="FloParamsUid",
-    )
-    HomeCity: str = Field(
-        title="HomeCity",
-        default="MILLINOCKET_ME",
-    )
-    TimezoneString: str = Field(
-        title="TimezoneString",
-        default="US/Eastern",
-    )
-    StartYearUtc: int = Field(
-        title="StartYearUtc",
-        default=2020,
-    )
-    StartMonthUtc: int = Field(
-        title="StartMonthUtc",
-        default=1,
-    )
-    StartDayUtc: int = Field(
-        title="StartDayUtc",
-        default=1,
-    )
-    StartHourUtc: int = Field(
-        title="StartHourUtc",
-        default=0,
-    )
-    StartMinuteUtc: int = Field(
-        title="StartMinuteUtc",
-        default=0,
-    )
-    StoreSizeGallons: int = Field(
-        title="StoreSizeGallons",
-        default=240,
-    )
-    MaxStoreTempF: int = Field(
-        title="MaxStoreTempF",
-        default=190,
-    )
-    ElementMaxPowerKw: float = Field(
-        title="ElementMaxPowerKw",
-        default=9.5,
-    )
-    RequiredSourceWaterTempF: int = Field(
-        title="RequiredSourceWaterTempF",
-        default=120,
-    )
-    FixedPumpGpm: float = Field(
-        title="FixedPumpGpm",
-        default=4.5,
-    )
-    ReturnWaterFixedDeltaT: int = Field(
-        title="ReturnWaterFixedDeltaT",
-        default=20,
-    )
-    SliceDurationMinutes: List[int] = Field(
-        title="SliceDurationMinutes",
-        default=[60],
-    )
-    PowerLostFromHouseKwList: List[float] = Field(
-        title="PowerLostFromHouseKwList",
-        default=[3.42],
-    )
-    OutsideTempF: List[float] = Field(
-        title="OutsideTempF",
-        default=[-5.1],
-    )
-    DistributionPrice: List[float] = Field(
-        title="DistributionPrice",
-        default=[40.0],
+    @classmethod
+    def local_to_type(cls, market_type_name: MarketTypeName) -> str:
+        if not isinstance(market_type_name, MarketTypeName):
+            raise SchemaError(f"{market_type_name} must be of type {MarketTypeName}")
+        versioned_enum = as_enum(
+            market_type_name, MarketTypeName000, MarketTypeName000.default()
+        )
+        return cls.versioned_enum_to_type_dict[versioned_enum]
+
+    type_to_versioned_enum_dict: Dict[str, MarketTypeName000] = {
+        "00000000": MarketTypeName000.unknown,
+        "d20b81e4": MarketTypeName000.rt5gate5,
+        "b36cbfb4": MarketTypeName000.rt60gate5,
+        "94a3fe9b": MarketTypeName000.da60,
+        "5f335bdb": MarketTypeName000.rt60gate30,
+        "01a84101": MarketTypeName000.rt15gate5,
+        "e997ccfb": MarketTypeName000.rt30gate5,
+        "618f9c0a": MarketTypeName000.rt60gate30b,
+    }
+
+    versioned_enum_to_type_dict: Dict[MarketTypeName000, str] = {
+        MarketTypeName000.unknown: "00000000",
+        MarketTypeName000.rt5gate5: "d20b81e4",
+        MarketTypeName000.rt60gate5: "b36cbfb4",
+        MarketTypeName000.da60: "94a3fe9b",
+        MarketTypeName000.rt60gate30: "5f335bdb",
+        MarketTypeName000.rt15gate5: "01a84101",
+        MarketTypeName000.rt30gate5: "e997ccfb",
+        MarketTypeName000.rt60gate30b: "618f9c0a",
+    }
+
+
+class MarketQuantityUnit000SchemaEnum:
+    enum_name: str = "market.quantity.unit.000"
+    symbols: List[str] = [
+        "00000000",
+        "c272f3b3",
+    ]
+
+    @classmethod
+    def is_symbol(cls, candidate: str) -> bool:
+        if candidate in cls.symbols:
+            return True
+        return False
+
+
+class MarketQuantityUnit000(StrEnum):
+    AvgMW = auto()
+    AvgkW = auto()
+
+    @classmethod
+    def default(cls) -> "MarketQuantityUnit000":
+        return cls.AvgMW
+
+    @classmethod
+    def values(cls) -> List[str]:
+        return [elt.value for elt in cls]
+
+
+class MarketQuantityUnitMap:
+    @classmethod
+    def type_to_local(cls, symbol: str) -> MarketQuantityUnit:
+        if not MarketQuantityUnit000SchemaEnum.is_symbol(symbol):
+            raise SchemaError(f"{symbol} must belong to MarketQuantityUnit000 symbols")
+        versioned_enum = cls.type_to_versioned_enum_dict[symbol]
+        return as_enum(versioned_enum, MarketQuantityUnit, MarketQuantityUnit.default())
+
+    @classmethod
+    def local_to_type(cls, market_quantity_unit: MarketQuantityUnit) -> str:
+        if not isinstance(market_quantity_unit, MarketQuantityUnit):
+            raise SchemaError(
+                f"{market_quantity_unit} must be of type {MarketQuantityUnit}"
+            )
+        versioned_enum = as_enum(
+            market_quantity_unit, MarketQuantityUnit000, MarketQuantityUnit000.default()
+        )
+        return cls.versioned_enum_to_type_dict[versioned_enum]
+
+    type_to_versioned_enum_dict: Dict[str, MarketQuantityUnit000] = {
+        "00000000": MarketQuantityUnit000.AvgMW,
+        "c272f3b3": MarketQuantityUnit000.AvgkW,
+    }
+
+    versioned_enum_to_type_dict: Dict[MarketQuantityUnit000, str] = {
+        MarketQuantityUnit000.AvgMW: "00000000",
+        MarketQuantityUnit000.AvgkW: "c272f3b3",
+    }
+
+
+class MarketTypeGt(BaseModel):
+    """Used by MarketMakers to simultaneously run several different types of Markets.
+
+        A [MarketMaker](https://gridworks.readthedocs.io/en/latest/market-maker.html) GNode can run several types of Markets. For example, it can run an
+    hourly real-time market and also an ancillary services market for Regulation. This is captured
+    by the concept of MarketType.
+        [More info](https://gridworks.readthedocs.io/en/latest/market-type.html).
+    """
+
+    Name: MarketTypeName = Field(
+        title="Name of the MarketType",
     )
-    RealtimeElectricityPrice: List[float] = Field(
-        title="RealtimeElectricityPrice",
-        default=[10.35],
+    DurationMinutes: int = Field(
+        title="Duration of MarketSlots, in minutes",
     )
-    RtElecPriceUid: str = Field(
-        title="RtElecPriceUid",
+    GateClosingSeconds: int = Field(
+        title="Seconds before the start of a MarketSlot after which bids are not accepted",
     )
-    WeatherUid: str = Field(
-        title="WeatherUid",
+    PriceUnit: MarketPriceUnit = Field(
+        title="Price Unit for market (e.g. USD Per MWh)",
     )
-    DistPriceUid: str = Field(
-        title="DistPriceUid",
+    QuantityUnit: MarketQuantityUnit = Field(
+        title="Quantity Unit for market (e.g. AvgMW)",
     )
     CurrencyUnit: RecognizedCurrencyUnit = Field(
-        title="CurrencyUnit",
-        default=RecognizedCurrencyUnit.USD,
+        title="Currency Unit for market (e.g. USD)",
     )
-    TypeName: Literal[
-        "flo.params.simpleresistivehydronic"
-    ] = "flo.params.simpleresistivehydronic"
+    PriceMax: int = Field(
+        title="PMax, required for defining bids",
+    )
+    TypeName: Literal["market.type.gt"] = "market.type.gt"
     Version: str = "000"
 
-    @validator("GNodeAlias")
-    def _check_g_node_alias(cls, v: str) -> str:
-        try:
-            check_is_left_right_dot(v)
-        except ValueError as e:
-            raise ValueError(f"GNodeAlias failed LeftRightDot format validation: {e}")
-        return v
-
-    @validator("FloParamsUid")
-    def _check_flo_params_uid(cls, v: str) -> str:
-        try:
-            check_is_uuid_canonical_textual(v)
-        except ValueError as e:
-            raise ValueError(
-                f"FloParamsUid failed UuidCanonicalTextual format validation: {e}"
-            )
-        return v
-
-    @validator("RtElecPriceUid")
-    def _check_rt_elec_price_uid(cls, v: str) -> str:
-        try:
-            check_is_uuid_canonical_textual(v)
-        except ValueError as e:
-            raise ValueError(
-                f"RtElecPriceUid failed UuidCanonicalTextual format validation: {e}"
-            )
-        return v
-
-    @validator("WeatherUid")
-    def _check_weather_uid(cls, v: str) -> str:
-        try:
-            check_is_uuid_canonical_textual(v)
-        except ValueError as e:
-            raise ValueError(
-                f"WeatherUid failed UuidCanonicalTextual format validation: {e}"
-            )
-        return v
-
-    @validator("DistPriceUid")
-    def _check_dist_price_uid(cls, v: str) -> str:
-        try:
-            check_is_uuid_canonical_textual(v)
-        except ValueError as e:
-            raise ValueError(
-                f"DistPriceUid failed UuidCanonicalTextual format validation: {e}"
-            )
-        return v
+    @validator("Name")
+    def _check_name(cls, v: MarketTypeName) -> MarketTypeName:
+        return as_enum(v, MarketTypeName, MarketTypeName.unknown)
+
+    @validator("PriceUnit")
+    def _check_price_unit(cls, v: MarketPriceUnit) -> MarketPriceUnit:
+        return as_enum(v, MarketPriceUnit, MarketPriceUnit.USDPerMWh)
+
+    @validator("QuantityUnit")
+    def _check_quantity_unit(cls, v: MarketQuantityUnit) -> MarketQuantityUnit:
+        return as_enum(v, MarketQuantityUnit, MarketQuantityUnit.AvgMW)
 
     @validator("CurrencyUnit")
     def _check_currency_unit(cls, v: RecognizedCurrencyUnit) -> RecognizedCurrencyUnit:
         return as_enum(v, RecognizedCurrencyUnit, RecognizedCurrencyUnit.UNKNOWN)
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
+        del d["Name"]
+        Name = as_enum(self.Name, MarketTypeName, MarketTypeName.default())
+        d["NameGtEnumSymbol"] = MarketTypeNameMap.local_to_type(Name)
+        del d["PriceUnit"]
+        PriceUnit = as_enum(self.PriceUnit, MarketPriceUnit, MarketPriceUnit.default())
+        d["PriceUnitGtEnumSymbol"] = MarketPriceUnitMap.local_to_type(PriceUnit)
+        del d["QuantityUnit"]
+        QuantityUnit = as_enum(
+            self.QuantityUnit, MarketQuantityUnit, MarketQuantityUnit.default()
+        )
+        d["QuantityUnitGtEnumSymbol"] = MarketQuantityUnitMap.local_to_type(
+            QuantityUnit
+        )
         del d["CurrencyUnit"]
         CurrencyUnit = as_enum(
             self.CurrencyUnit, RecognizedCurrencyUnit, RecognizedCurrencyUnit.default()
         )
         d["CurrencyUnitGtEnumSymbol"] = RecognizedCurrencyUnitMap.local_to_type(
             CurrencyUnit
         )
@@ -304,177 +350,150 @@
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
     def __hash__(self):
         return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
 
-class FloParamsSimpleresistivehydronic_Maker:
-    type_name = "flo.params.simpleresistivehydronic"
+class MarketTypeGt_Maker:
+    type_name = "market.type.gt"
     version = "000"
 
     def __init__(
         self,
-        g_node_alias: str,
-        flo_params_uid: str,
-        home_city: str,
-        timezone_string: str,
-        start_year_utc: int,
-        start_month_utc: int,
-        start_day_utc: int,
-        start_hour_utc: int,
-        start_minute_utc: int,
-        store_size_gallons: int,
-        max_store_temp_f: int,
-        element_max_power_kw: float,
-        required_source_water_temp_f: int,
-        fixed_pump_gpm: float,
-        return_water_fixed_delta_t: int,
-        slice_duration_minutes: List[int],
-        power_lost_from_house_kw_list: List[float],
-        outside_temp_f: List[float],
-        distribution_price: List[float],
-        realtime_electricity_price: List[float],
-        rt_elec_price_uid: str,
-        weather_uid: str,
-        dist_price_uid: str,
+        name: MarketTypeName,
+        duration_minutes: int,
+        gate_closing_seconds: int,
+        price_unit: MarketPriceUnit,
+        quantity_unit: MarketQuantityUnit,
         currency_unit: RecognizedCurrencyUnit,
+        price_max: int,
     ):
-        self.tuple = FloParamsSimpleresistivehydronic(
-            GNodeAlias=g_node_alias,
-            FloParamsUid=flo_params_uid,
-            HomeCity=home_city,
-            TimezoneString=timezone_string,
-            StartYearUtc=start_year_utc,
-            StartMonthUtc=start_month_utc,
-            StartDayUtc=start_day_utc,
-            StartHourUtc=start_hour_utc,
-            StartMinuteUtc=start_minute_utc,
-            StoreSizeGallons=store_size_gallons,
-            MaxStoreTempF=max_store_temp_f,
-            ElementMaxPowerKw=element_max_power_kw,
-            RequiredSourceWaterTempF=required_source_water_temp_f,
-            FixedPumpGpm=fixed_pump_gpm,
-            ReturnWaterFixedDeltaT=return_water_fixed_delta_t,
-            SliceDurationMinutes=slice_duration_minutes,
-            PowerLostFromHouseKwList=power_lost_from_house_kw_list,
-            OutsideTempF=outside_temp_f,
-            DistributionPrice=distribution_price,
-            RealtimeElectricityPrice=realtime_electricity_price,
-            RtElecPriceUid=rt_elec_price_uid,
-            WeatherUid=weather_uid,
-            DistPriceUid=dist_price_uid,
+        self.tuple = MarketTypeGt(
+            Name=name,
+            DurationMinutes=duration_minutes,
+            GateClosingSeconds=gate_closing_seconds,
+            PriceUnit=price_unit,
+            QuantityUnit=quantity_unit,
             CurrencyUnit=currency_unit,
+            PriceMax=price_max,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: FloParamsSimpleresistivehydronic) -> str:
+    def tuple_to_type(cls, tuple: MarketTypeGt) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> FloParamsSimpleresistivehydronic:
+    def type_to_tuple(cls, t: str) -> MarketTypeGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> FloParamsSimpleresistivehydronic:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> MarketTypeGt:
         d2 = dict(d)
-        if "GNodeAlias" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing GNodeAlias")
-        if "FloParamsUid" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FloParamsUid")
-        if "HomeCity" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing HomeCity")
-        if "TimezoneString" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing TimezoneString")
-        if "StartYearUtc" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StartYearUtc")
-        if "StartMonthUtc" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StartMonthUtc")
-        if "StartDayUtc" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StartDayUtc")
-        if "StartHourUtc" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StartHourUtc")
-        if "StartMinuteUtc" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StartMinuteUtc")
-        if "StoreSizeGallons" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StoreSizeGallons")
-        if "MaxStoreTempF" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing MaxStoreTempF")
-        if "ElementMaxPowerKw" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing ElementMaxPowerKw")
-        if "RequiredSourceWaterTempF" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing RequiredSourceWaterTempF")
-        if "FixedPumpGpm" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FixedPumpGpm")
-        if "ReturnWaterFixedDeltaT" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing ReturnWaterFixedDeltaT")
-        if "SliceDurationMinutes" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing SliceDurationMinutes")
-        if "PowerLostFromHouseKwList" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing PowerLostFromHouseKwList")
-        if "OutsideTempF" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing OutsideTempF")
-        if "DistributionPrice" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing DistributionPrice")
-        if "RealtimeElectricityPrice" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing RealtimeElectricityPrice")
-        if "RtElecPriceUid" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing RtElecPriceUid")
-        if "WeatherUid" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing WeatherUid")
-        if "DistPriceUid" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing DistPriceUid")
+        if "NameGtEnumSymbol" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing NameGtEnumSymbol")
+        if d2["NameGtEnumSymbol"] in MarketTypeName000SchemaEnum.symbols:
+            d2["Name"] = MarketTypeNameMap.type_to_local(d2["NameGtEnumSymbol"])
+        else:
+            d2["Name"] = MarketTypeName.default()
+        if "DurationMinutes" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing DurationMinutes")
+        if "GateClosingSeconds" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing GateClosingSeconds")
+        if "PriceUnitGtEnumSymbol" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing PriceUnitGtEnumSymbol")
+        if d2["PriceUnitGtEnumSymbol"] in MarketPriceUnit000SchemaEnum.symbols:
+            d2["PriceUnit"] = MarketPriceUnitMap.type_to_local(
+                d2["PriceUnitGtEnumSymbol"]
+            )
+        else:
+            d2["PriceUnit"] = MarketPriceUnit.default()
+        if "QuantityUnitGtEnumSymbol" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing QuantityUnitGtEnumSymbol")
+        if d2["QuantityUnitGtEnumSymbol"] in MarketQuantityUnit000SchemaEnum.symbols:
+            d2["QuantityUnit"] = MarketQuantityUnitMap.type_to_local(
+                d2["QuantityUnitGtEnumSymbol"]
+            )
+        else:
+            d2["QuantityUnit"] = MarketQuantityUnit.default()
         if "CurrencyUnitGtEnumSymbol" not in d2.keys():
             raise SchemaError(f"dict {d2} missing CurrencyUnitGtEnumSymbol")
         if (
             d2["CurrencyUnitGtEnumSymbol"]
             in RecognizedCurrencyUnit000SchemaEnum.symbols
         ):
             d2["CurrencyUnit"] = RecognizedCurrencyUnitMap.type_to_local(
                 d2["CurrencyUnitGtEnumSymbol"]
             )
         else:
             d2["CurrencyUnit"] = RecognizedCurrencyUnit.default()
+        if "PriceMax" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing PriceMax")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return FloParamsSimpleresistivehydronic(
-            GNodeAlias=d2["GNodeAlias"],
-            FloParamsUid=d2["FloParamsUid"],
-            HomeCity=d2["HomeCity"],
-            TimezoneString=d2["TimezoneString"],
-            StartYearUtc=d2["StartYearUtc"],
-            StartMonthUtc=d2["StartMonthUtc"],
-            StartDayUtc=d2["StartDayUtc"],
-            StartHourUtc=d2["StartHourUtc"],
-            StartMinuteUtc=d2["StartMinuteUtc"],
-            StoreSizeGallons=d2["StoreSizeGallons"],
-            MaxStoreTempF=d2["MaxStoreTempF"],
-            ElementMaxPowerKw=d2["ElementMaxPowerKw"],
-            RequiredSourceWaterTempF=d2["RequiredSourceWaterTempF"],
-            FixedPumpGpm=d2["FixedPumpGpm"],
-            ReturnWaterFixedDeltaT=d2["ReturnWaterFixedDeltaT"],
-            SliceDurationMinutes=d2["SliceDurationMinutes"],
-            PowerLostFromHouseKwList=d2["PowerLostFromHouseKwList"],
-            OutsideTempF=d2["OutsideTempF"],
-            DistributionPrice=d2["DistributionPrice"],
-            RealtimeElectricityPrice=d2["RealtimeElectricityPrice"],
-            RtElecPriceUid=d2["RtElecPriceUid"],
-            WeatherUid=d2["WeatherUid"],
-            DistPriceUid=d2["DistPriceUid"],
+        return MarketTypeGt(
+            Name=d2["Name"],
+            DurationMinutes=d2["DurationMinutes"],
+            GateClosingSeconds=d2["GateClosingSeconds"],
+            PriceUnit=d2["PriceUnit"],
+            QuantityUnit=d2["QuantityUnit"],
             CurrencyUnit=d2["CurrencyUnit"],
+            PriceMax=d2["PriceMax"],
             TypeName=d2["TypeName"],
             Version="000",
         )
+
+    @classmethod
+    def tuple_to_dc(cls, t: MarketTypeGt) -> MarketType:
+        if t.Name in MarketType.by_id.keys():
+            dc = MarketType.by_id[t.Name]
+        else:
+            dc = MarketType(
+                name=t.Name,
+                duration_minutes=t.DurationMinutes,
+                gate_closing_seconds=t.GateClosingSeconds,
+                price_unit=t.PriceUnit,
+                quantity_unit=t.QuantityUnit,
+                currency_unit=t.CurrencyUnit,
+                price_max=t.PriceMax,
+            )
+
+        return dc
+
+    @classmethod
+    def dc_to_tuple(cls, dc: MarketType) -> MarketTypeGt:
+        t = MarketTypeGt_Maker(
+            name=dc.name,
+            duration_minutes=dc.duration_minutes,
+            gate_closing_seconds=dc.gate_closing_seconds,
+            price_unit=dc.price_unit,
+            quantity_unit=dc.quantity_unit,
+            currency_unit=dc.currency_unit,
+            price_max=dc.price_max,
+        ).tuple
+        return t
+
+    @classmethod
+    def type_to_dc(cls, t: str) -> MarketType:
+        return cls.tuple_to_dc(cls.type_to_tuple(t))
+
+    @classmethod
+    def dc_to_type(cls, dc: MarketType) -> str:
+        return cls.dc_to_tuple(dc).as_type()
+
+    @classmethod
+    def dict_to_dc(cls, d: dict[Any, str]) -> MarketType:
+        return cls.tuple_to_dc(cls.dict_to_tuple(d))
```

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_req/r_gnode_distp_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_distprequest_ps/r_gnode_distp_sync_req/r_gnode_distp_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_get_eprt_forecast_sync/r_get_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_forecast_cron_req/r_gnode_eprt_forecast_cron_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_req/r_gnode_eprt_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_sync_req/r_gnode_eprt_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_eprequest_ps/r_gnode_eprt_uid_req/r_gnode_eprt_uid_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_cron_req/r_gnode_weather_forecast_cron_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_forecast_sync_req/r_gnode_weather_forecast_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_req/r_gnode_weather_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_forecastrequest_ws/r_gnode_weather_uid_req/r_gnode_weather_uid_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_req/r_gnode_regp_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/gnode_regprequest_ps/r_gnode_regp_sync_req/r_gnode_regp_sync_req_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/gt_dispatch_boolean.py` & `gridworks_atn-0.4.0/src/gwatn/types/gt_dispatch_boolean.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/hack_property_format.py` & `gridworks_atn-0.4.0/src/gwatn/types/hack_property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/hack_type_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/hack_type_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/hack_utils.py` & `gridworks_atn-0.4.0/src/gwatn/types/hack_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/heartbeat_b.py` & `gridworks_atn-0.4.0/src/gwatn/types/heartbeat_b.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_create.py` & `gridworks_atn-0.4.0/src/gwatn/types/initial_tadeed_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_optin.py` & `gridworks_atn-0.4.0/src/gwatn/types/initial_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/initial_tadeed_algo_transfer.py` & `gridworks_atn-0.4.0/src/gwatn/types/initial_tadeed_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/join_dispatch_contract.py` & `gridworks_atn-0.4.0/src/gwatn/types/join_dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/latest_price.py` & `gridworks_atn-0.4.0/src/gwatn/types/latest_price.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/market_slot.py` & `gridworks_atn-0.4.0/src/gwatn/types/market_slot.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_algo_optin.py` & `gridworks_atn-0.4.0/src/gwatn/types/new_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/new_tadeed_send.py` & `gridworks_atn-0.4.0/src/gwatn/types/new_tadeed_send.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/old_tadeed_algo_return.py` & `gridworks_atn-0.4.0/src/gwatn/types/old_tadeed_algo_return.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/price_quantity.py` & `gridworks_atn-0.4.0/src/gwatn/types/price_quantity.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/price_quantity_unitless.py` & `gridworks_atn-0.4.0/src/gwatn/types/price_quantity_unitless.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/csv_distp/csv_distp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/csv_distp_oneprice/csv_distp_oneprice_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/csv_distp_sync/csv_distp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp/r_distp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_oneprice/r_distp_oneprice_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_distprices_gnode/r_distp_sync/r_distp_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_epda_actual/csv_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt/csv_eprt_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_actual/csv_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast/csv_eprt_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync/csv_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_forecast_sync_table/csv_eprt_forecast_sync_table_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/csv_eprt_sync/csv_eprt_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_epda_actual/r_epda_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt/r_eprt_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_actual/r_eprt_actual_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast/r_eprt_forecast_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_cron_response/r_eprt_forecast_cron_response_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_forecast_sync/r_eprt_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_eprt_sync/r_eprt_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_electricityprices_gnode/r_ps_penpal/r_ps_penpal_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/csv_regp/csv_regp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/csv_regp_sync/csv_regp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp/r_regp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ps_regprices_gnode/r_regp_sync/r_regp_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/scada_cert_transfer.py` & `gridworks_atn-0.4.0/src/gwatn/types/scada_cert_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data.py` & `gridworks_atn-0.4.0/src/gwatn/types/simplesim_driver_data.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_data_bsh.py` & `gridworks_atn-0.4.0/src/gwatn/types/simplesim_driver_data_bsh.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/simplesim_driver_report.py` & `gridworks_atn-0.4.0/src/gwatn/types/simplesim_driver_report.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/simplesim_snapshot_brickstorageheater.py` & `gridworks_atn-0.4.0/src/gwatn/types/simplesim_snapshot_brickstorageheater.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/sla_enter.py` & `gridworks_atn-0.4.0/src/gwatn/types/sla_enter.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/tadeed_specs_hack.py` & `gridworks_atn-0.4.0/src/gwatn/types/tadeed_specs_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_create.py` & `gridworks_atn-0.4.0/src/gwatn/types/tavalidatorcert_algo_create.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/tavalidatorcert_algo_transfer.py` & `gridworks_atn-0.4.0/src/gwatn/types/tavalidatorcert_algo_transfer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/terminalasset_certify_hack.py` & `gridworks_atn-0.4.0/src/gwatn/types/terminalasset_certify_hack.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_raw/csv_weather_forecast_raw_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/csv_weather_forecast_sync/csv_weather_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast/r_weather_forecast_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_cron_response/r_weather_forecast_cron_response_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_raw/r_weather_forecast_raw_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_weather_forecast_sync/r_weather_forecast_sync_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_forecast_gnode/r_ws_penpal/r_ws_penpal_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_sync/csv_irradiance_poa_sync_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/csv_irradiance_poa_template/csv_irradiance_poa_template_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_irradiances_gnode/r_irradiance_poa_template/r_irradiance_poa_template_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/csv_weather_tmy_temp/csv_weather_tmy_temp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_solarandtemp/r_weather_tmy_solarandtemp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py` & `gridworks_atn-0.4.0/src/gwatn/types/ws_typicalmodeledyear_gnode/r_weather_tmy_temp/r_weather_tmy_temp_1_0_0_payload_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.3.8/PKG-INFO` & `gridworks_atn-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks-atn
-Version: 0.3.8
+Version: 0.4.0
 Summary: Gridworks Atn Spaceheat
 Home-page: https://github.com/thegridelectric/gridworks-atn
 License: None
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

