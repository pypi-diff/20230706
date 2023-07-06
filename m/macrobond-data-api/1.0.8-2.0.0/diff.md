# Comparing `tmp/macrobond-data-api-1.0.8.tar.gz` & `tmp/macrobond-data-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-mj749aky/macrobond-data-api-1.0.8.tar", last modified: Mon Jul  3 11:42:48 2023, max compression
+gzip compressed data, was "/home/runner/work/macrobond-data-api/macrobond-data-api/dist/.tmp-c5j2b4ti/macrobond-data-api-2.0.0.tar", last modified: Thu Jul  6 13:35:34 2023, max compression
```

## Comparing `macrobond-data-api-1.0.8.tar` & `macrobond-data-api-2.0.0.tar`

### file list

```diff
@@ -1,148 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/_generated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/_get_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15973 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/_error_message_to_status_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/_fill_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/_fix_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/metadata_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/search_query.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series_with_revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/calendar_date_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/calendar_merge_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/metadata_attribute_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_missing_value_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_partial_periods_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_weekdays.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/enums/status_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/_parse_iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/_repr_html_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/format_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/get_all_vintage_series_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/get_entity_error.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/metadata_attribute_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/metadata_value_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/revision_history_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/revision_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/search_result_long.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/series_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/series_observation_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/series_with_vintages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/start_or_end_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/unified_series.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/values_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/common/types/vintage_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/util/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/util/save_credential_to_keyring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_metadata_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_split_in_to_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/_web_only_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/data_package_list_poller.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/subscription_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/data_pacakge_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/data_package_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/data_package_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/data_package_list_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/entity_info_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/entity_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/entity_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/feed_entities_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/http_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/metadata_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/problem_details_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/response_error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/revision_history_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/item_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/search_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/search_for_display_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/search_for_display_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/search_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/search_request_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_observation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_with_vintages_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/unified_series_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/unified_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/values_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/vintage_series_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/vintage_values_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/macrobond_data_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-03 11:42:48.000000 macrobond-data-api-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-03 11:41:11.000000 macrobond-data-api-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/_generated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/_get_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16229 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_error_message_to_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_fill_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_fix_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/metadata_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/search_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series_with_revisions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23175 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/calendar_date_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/calendar_merge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/metadata_attribute_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_missing_value_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_partial_periods_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_to_higher_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_to_lower_frequency_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_weekdays.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/enums/status_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/_parse_iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/_repr_html_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/format_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/get_all_vintage_series_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/get_entity_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/metadata_attribute_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/metadata_value_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/revision_history_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/revision_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/search_result_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/series_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/series_observation_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/series_with_vintages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/start_or_end_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/unified_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/values_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/common/types/vintage_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/util/save_credential_to_keyring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_metadata_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_split_in_to_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/_web_only_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/data_package_list_poller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/subscription_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/data_pacakge_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/data_package_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/data_package_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/data_package_list_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/entity_info_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/entity_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/feed_entities_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/http_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/metadata/metadata_value_information_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/metadata_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/problem_details_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/response_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/revision_history_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/item_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/search_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/search_for_display_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/search_for_display_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/search_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/search_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12233 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_observation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_location_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_with_revisions_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_with_times_of_change_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_with_vintages_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/unified_series_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/unified_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/values_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/vintage_series_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/vintage_values_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/macrobond_data_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-06 13:35:34.000000 macrobond-data-api-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-06 13:33:59.000000 macrobond-data-api-2.0.0/setup.py
```

### Comparing `macrobond-data-api-1.0.8/LICENSE` & `macrobond-data-api-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/PKG-INFO` & `macrobond-data-api-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 1.0.8
+Version: 2.0.0
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.8 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 2.0.0 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-1.0.8/README.md` & `macrobond-data-api-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/__init__.py` & `macrobond-data-api-2.0.0/macrobond_data_api/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/_generated.py` & `macrobond-data-api-2.0.0/macrobond_data_api/_generated.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/_get_api.py` & `macrobond-data-api-2.0.0/macrobond_data_api/_get_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_metadata.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_revision.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_revision.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,25 +150,25 @@
                 None,
             )
 
         values, dates = _remove_padding(series)
 
         if include_times_of_change:
             if series_with_revisions.HasRevisions:
-                values_metadata = _fill_values_metadata_from_series(series, True)
+                values_metadata = _fill_values_metadata_from_series(series, self, True)
             else:
                 values_metadata = [{}] * len(values)
         else:
             values_metadata = None
 
         return VintageSeries(
             series_name,
             "",
             StatusCode.OK,
-            _fill_metadata_from_entity(series),
+            _fill_metadata_from_entity(series, self),
             values_metadata,
             values,
             _datetime_to_datetime_timezone(dates),
             None,
         )
 
     series = [to_obj(x) for x in series_names]
@@ -218,22 +218,28 @@
             )
 
         values = [None if isnan(x) else x for x in series.Values]  # type: ignore
         dates = _datetime_to_datetime_timezone(series.DatesAtStartOfPeriod)
 
         if include_times_of_change:
             if series_with_revisions.HasRevisions:
-                values_metadata = _fill_values_metadata_from_series(series)
+                values_metadata = _fill_values_metadata_from_series(series, self)
             else:
                 values_metadata = [{}] * len(values)
         else:
             values_metadata = None
 
         return Series(
-            series_name, None, StatusCode.OK, _fill_metadata_from_entity(series), values_metadata, values, dates
+            series_name,
+            None,
+            StatusCode.OK,
+            _fill_metadata_from_entity(series, self),
+            values_metadata,
+            values,
+            dates,
         )
 
     series = [to_obj(x) for x in series_names]
 
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
 
@@ -249,15 +255,15 @@
 
         values, dates = _remove_padding(com_series)
 
         return VintageSeries(
             name,
             None,
             StatusCode.OK,
-            _fill_metadata_from_entity(com_series),
+            _fill_metadata_from_entity(com_series, self),
             None,
             values,
             _datetime_to_datetime_timezone(dates),
             None,
         )
 
     series_with_revisions = self.database.FetchOneSeriesWithRevisions(series_name)
@@ -272,15 +278,22 @@
     if not series_with_revisions.HasRevisions:
         series = complete_history[0]
         values = [None if isnan(x) else x for x in series.Values]  # type: ignore
         dates = _datetime_to_datetime_timezone(series.DatesAtStartOfPeriod)
         return GetAllVintageSeriesResult(
             [
                 VintageSeries(
-                    series_name, None, StatusCode.OK, _fill_metadata_from_entity(series), None, values, dates, None
+                    series_name,
+                    None,
+                    StatusCode.OK,
+                    _fill_metadata_from_entity(series, self),
+                    None,
+                    values,
+                    dates,
+                    None,
                 )
             ],
             series_name,
         )
 
     return GetAllVintageSeriesResult([to_obj(x, series_name) for x in complete_history], series_name)
 
@@ -371,15 +384,15 @@
         if series_with_revisions.IsError:
             if series_with_revisions.ErrorMessage == "Not found":
                 yield SeriesWithVintages("Not found", StatusCode.NOT_FOUND, None, [])
                 continue
             raise Exception(series_with_revisions.ErrorMessage)
 
         head = series_with_revisions.Head
-        metadata = _fill_metadata_from_entity(head)
+        metadata = _fill_metadata_from_entity(head, self)
         last_modified_time = metadata["LastModifiedTimeStamp"]
 
         if (
             request.if_modified_since
             and last_modified_time
             and _less_than_or_equal_with_margin(last_modified_time, request.if_modified_since)
         ):
```

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_search.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 if TYPE_CHECKING:  # pragma: no cover
     from .com_api import ComApi
 
     from macrobond_data_api.common.types import SearchFilter
 
     from .com_types import SearchQuery
 
-    from .com_types import Entity as ComEntity
-
 
 def entity_search_multi_filter(
     self: "ComApi",
     *filters: "SearchFilter",
     include_discontinued: bool = False,
     no_metadata: bool = False  # pylint: disable=unused-argument
 ) -> SearchResult:
@@ -51,8 +49,8 @@
             query.AddAttributeFilter(attribute, False)
 
         query.IncludeDiscontinued = include_discontinued
 
         querys.append(query)
 
     result = self.database.Search(querys)
-    return SearchResult([_fill_metadata_from_entity(x) for x in result.Entities], result.IsTruncated)
+    return SearchResult([_fill_metadata_from_entity(x, self) for x in result.Entities], result.IsTruncated)
```

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/_com_api_series.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/_com_api_series.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,55 +28,55 @@
     from .com_types import Series as ComSeries, Entity as ComEntity
 
 
 def _datetime_to_datetime(dates: Sequence[datetime]) -> List[datetime]:
     return [datetime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond) for x in dates]
 
 
-def _create_entity(com_entity: "ComEntity", name: str) -> Entity:
+def _create_entity(com_entity: "ComEntity", name: str, api: "ComApi") -> Entity:
     if com_entity.IsError:
         return Entity(name, com_entity.ErrorMessage, _error_message_to_status_code(com_entity), None)
-    return Entity(name, None, StatusCode.OK, _fill_metadata_from_entity(com_entity))
+    return Entity(name, None, StatusCode.OK, _fill_metadata_from_entity(com_entity, api))
 
 
-def _create_series(com_series: "ComSeries", name: str) -> Series:
+def _create_series(com_series: "ComSeries", name: str, api: "ComApi") -> Series:
     if com_series.IsError:
         return Series(name, com_series.ErrorMessage, _error_message_to_status_code(com_series), None, None, None, None)
     return Series(
         name,
         None,
         StatusCode.OK,
-        _fill_metadata_from_entity(com_series),
+        _fill_metadata_from_entity(com_series, api),
         None,
         [None if isnan(x) else x for x in com_series.Values],
         _datetime_to_datetime(com_series.DatesAtStartOfPeriod),
     )
 
 
 def get_one_series(self: "ComApi", series_name: str, raise_error: bool = None) -> Series:
     return self.get_series([series_name], raise_error=raise_error)[0]
 
 
 def get_series(self: "ComApi", series_names: Sequence[str], raise_error: Optional[bool] = None) -> Sequence[Series]:
     series_names = tuple(series_names)
     com_series = self.database.FetchSeries(series_names)
-    series = [_create_series(x, y) for x, y in zip(com_series, series_names)]
+    series = [_create_series(x, y, self) for x, y in zip(com_series, series_names)]
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(series_names, series)])
     return _ReprHtmlSequence(series)
 
 
 def get_one_entity(self: "ComApi", entity_name: str, raise_error: bool = None) -> Entity:
     return self.get_entities([entity_name], raise_error=raise_error)[0]
 
 
 def get_entities(self: "ComApi", entity_names: Sequence[str], raise_error: bool = None) -> Sequence[Entity]:
     entity_names = tuple(entity_names)
     com_entitys = self.database.FetchEntities(entity_names)
-    entitys = [_create_entity(x, y) for x, y in zip(com_entitys, entity_names)]
+    entitys = [_create_entity(x, y, self) for x, y in zip(com_entitys, entity_names)]
     if self.raise_error if raise_error is None else raise_error:
         GetEntitiesError._raise_if([(x, y.error_message) for x, y in zip(entity_names, entitys)])
     return _ReprHtmlSequence(entitys)
 
 
 def get_many_series(
     self: "ComApi", series: Sequence[Union[str, Tuple[str, Optional[datetime]]]], include_not_modified: bool = False
@@ -160,15 +160,15 @@
     def to_obj(name: str, com_one_series: "ComSeries") -> UnifiedSeries:
         if com_one_series.IsError:
             return UnifiedSeries(name, com_one_series.ErrorMessage, {}, [])
 
         return UnifiedSeries(
             name,
             "",
-            _fill_metadata_from_entity(com_one_series),
+            _fill_metadata_from_entity(com_one_series, self),
             [None if isnan(x) else x for x in com_one_series.Values],
         )
 
     ret = UnifiedSeriesList([to_obj(request.AddedSeries[x].Name, y) for x, y in enumerate(com_series)], dates)
 
     if self.raise_error if raise_error is None else raise_error:
         errors = [EntityErrorInfo(x, y) for x, y in ret.get_errors().items()]
```

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/_fill_metadata.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/_fill_metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import Any, TYPE_CHECKING, Sequence, Dict
+from typing import Any, TYPE_CHECKING, Sequence
 from datetime import datetime, timezone
 
+from ._metadata import _Metadata
 
 try:
     from pywintypes import TimeType
 except ImportError as ex:
     ...
 
 if TYPE_CHECKING:  # pragma: no cover
+    from .com_api import ComApi
     from .com_types import Entity as ComEntity
     from .com_types import Series as ComSeries
     from .com_types import Metadata as ComMetadata
-    from macrobond_data_api.common.types.metadata import Metadata
     from macrobond_data_api.common.types.values_metadata import ValuesMetadata
 
 
 def _get_val(name: str, values: Sequence[Any]) -> Any:
     if isinstance(values[0], TimeType):
         if name in ("OriginalStartDate", "OriginalEndDate"):
             datetime_ = values[0]
@@ -54,24 +55,29 @@
         values = [
             datetime(x.year, x.month, x.day, x.hour, x.minute, x.second, x.microsecond, timezone.utc) for x in values
         ]
         return values[0] if len(values) == 1 else values
     return values[0] if len(values) == 1 else list(values)
 
 
-def _fill_metadata_from_metadata(com_metadata: "ComMetadata", add_empty_revision_time_stamp: bool = False) -> Dict:
-    metadata = {x: _get_val(x, com_metadata.GetValues(x)) for x, _ in com_metadata.ListNames()}
+def _fill_metadata_from_metadata(
+    com_metadata: "ComMetadata", api: "ComApi", add_empty_revision_time_stamp: bool = False
+) -> _Metadata:
+    metadata = _Metadata(
+        {x: _get_val(x, com_metadata.GetValues(x)) for x, _ in com_metadata.ListNames()}, api._metadata_type_directory
+    )
     if add_empty_revision_time_stamp and "RevisionTimeStamp" not in metadata:
         metadata["RevisionTimeStamp"] = None
     return metadata
 
 
-def _fill_metadata_from_entity(com_entity: "ComEntity") -> "Metadata":
-    ret = _fill_metadata_from_metadata(com_entity.Metadata)
-    ret.setdefault("FullDescription", com_entity.Title)
+def _fill_metadata_from_entity(com_entity: "ComEntity", api: "ComApi") -> _Metadata:
+    ret = _fill_metadata_from_metadata(com_entity.Metadata, api)
+    if "FullDescription" not in ret:
+        ret["FullDescription"] = com_entity.Title
     return ret
 
 
 def _fill_values_metadata_from_series(
-    com_series: "ComSeries", add_empty_revision_time_stamp: bool = False
+    com_series: "ComSeries", api: "ComApi", add_empty_revision_time_stamp: bool = False
 ) -> "ValuesMetadata":
-    return [_fill_metadata_from_metadata(x, add_empty_revision_time_stamp) for x in com_series.ValuesMetadata]
+    return [_fill_metadata_from_metadata(x, api, add_empty_revision_time_stamp) for x in com_series.ValuesMetadata]
```

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_api.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import TYPE_CHECKING, Optional
 
 from macrobond_data_api.common import Api
 
+from ._metadata_directory import _MetadataTypeDirectory
+
 from ._com_api_metadata import (
     metadata_get_attribute_information,
     metadata_get_value_information,
     metadata_list_values,
 )
 
 from ._com_api_revision import (
@@ -42,14 +44,15 @@
 
 class ComApi(Api):
     _connection: Optional["Connection"]
 
     def __init__(self, connection: "Connection") -> None:
         super().__init__()
         self._connection = connection
+        self._metadata_type_directory = _MetadataTypeDirectory(connection)
 
     @property
     def connection(self) -> "Connection":
         if self._connection is None:
             raise ValueError("ComApi is not open")
         return self._connection
```

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_client.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,10 +147,11 @@
         """
         free all resources used by the Macrobond API.
         Opening and closing sessions can be slow,
         so it is usually not a good idea to open and close them for each request
         """
         self.has_closed = True
         if self.__api:
+            self.__api._metadata_type_directory.close()
             self.__api.connection.Close()
             self.__api._connection = None
             self.__api = None
```

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/connection.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/connection.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/database.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/database.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/entity.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/metadata.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/metadata_information.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/metadata_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/search_query.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/search_query.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series_expression.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series_expression.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series_request.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/com/com_types/series_with_revisions.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/com_types/series_with_revisions.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/api.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/client.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/enums/__init__.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/enums/metadata_attribute_type.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/enums/metadata_attribute_type.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_frequency.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_frequency.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_partial_periods_method.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_partial_periods_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_to_higher_frequency_method.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_to_higher_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_to_lower_frequency_method.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_to_lower_frequency_method.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/enums/series_weekdays.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/enums/series_weekdays.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/__init__.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/_parse_iso8601.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/_parse_iso8601.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/_repr_html_sequence.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/_repr_html_sequence.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/entity.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/entity.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/get_all_vintage_series_result.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/get_all_vintage_series_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/get_entity_error.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/get_entity_error.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/metadata_attribute_information.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/metadata_attribute_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/metadata_value_information.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/metadata_value_information.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/revision_history_request.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/revision_info.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/revision_info.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/search_filter.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/search_result.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/search_result.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/search_result_long.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/search_result_long.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/series.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/series_entry.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/series_entry.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/series_observation_history.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/series_observation_history.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/series_with_vintages.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/series_with_vintages.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/start_or_end_point.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/start_or_end_point.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/unified_series.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/unified_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/common/types/vintage_series.py` & `macrobond-data-api-2.0.0/macrobond_data_api/common/types/vintage_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/util/save_credential_to_keyring.py` & `macrobond-data-api-2.0.0/macrobond_data_api/util/save_credential_to_keyring.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/_metadata.py` & `macrobond-data-api-2.0.0/macrobond_data_api/com/_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/_metadata_directory.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/_metadata_directory.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_metadata.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_metadata.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_revision.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_revision.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_search.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_search.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/_web_api_series.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/_web_api_series.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/_web_only_api.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/_web_only_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/data_package_list_poller.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/data_package_list_poller.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/session.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/session.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/subscription_list.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/subscription_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_api.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_api.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_client.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_client.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/__init__.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/__init__.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/data_package_body.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/data_package_body.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/data_package_list.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/data_package_list.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/data_package_list_state.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/data_package_list_state.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/entity_info_for_display_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/entity_info_for_display_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/feed_entities_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/feed_entities_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/http_exception.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/http_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/metadata/metadata_attribute_information_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/metadata_methods.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/metadata_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/problem_details_exception.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/problem_details_exception.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/response_error_code.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/response_error_code.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/revision_history_request.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/revision_history_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/item_listing_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/item_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search/search_filter.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search/search_filter.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/search_methods.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/search_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_methods.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_observation_history_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_observation_history_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_listing_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree/series_tree_node_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_tree_methods.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_tree_methods.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_with_revisions_info_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_with_revisions_info_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/series_with_vintages_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/series_with_vintages_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/status_response.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/status_response.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api/web/web_types/unified_series_request.py` & `macrobond-data-api-2.0.0/macrobond_data_api/web/web_types/unified_series_request.py`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api.egg-info/PKG-INFO` & `macrobond-data-api-2.0.0/macrobond_data_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrobond-data-api
-Version: 1.0.8
+Version: 2.0.0
 Summary: Exposes a common API in Python for the Macrobond Web and Client Data APIs
 Home-page: https://github.com/macrobond/macrobond-data-api
 Author: Macrobond Financial
 Author-email: support@macrobond.com
 Project-URL: Documentation, https://macrobond.github.io/macrobond-data-api
 Project-URL: Source, https://github.com/macrobond/macrobond-data-api
 Project-URL: Tracker, https://github.com/macrobond/macrobond-data-api/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: macrobond-data-api Version: 1.0.8 Summary: Exposes
+Metadata-Version: 2.1 Name: macrobond-data-api Version: 2.0.0 Summary: Exposes
 a common API in Python for the Macrobond Web and Client Data APIs Home-page:
 https://github.com/macrobond/macrobond-data-api Author: Macrobond Financial
 Author-email: support@macrobond.com Project-URL: Documentation, https://
 macrobond.github.io/macrobond-data-api Project-URL: Source, https://github.com/
 macrobond/macrobond-data-api Project-URL: Tracker, https://github.com/
 macrobond/macrobond-data-api/issues Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 :: Only Classifier:
```

### Comparing `macrobond-data-api-1.0.8/macrobond_data_api.egg-info/SOURCES.txt` & `macrobond-data-api-2.0.0/macrobond_data_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 macrobond_data_api/com/_com_api_metadata.py
 macrobond_data_api/com/_com_api_revision.py
 macrobond_data_api/com/_com_api_search.py
 macrobond_data_api/com/_com_api_series.py
 macrobond_data_api/com/_error_message_to_status_code.py
 macrobond_data_api/com/_fill_metadata.py
 macrobond_data_api/com/_fix_datetime.py
+macrobond_data_api/com/_metadata.py
+macrobond_data_api/com/_metadata_directory.py
 macrobond_data_api/com/com_api.py
 macrobond_data_api/com/com_client.py
 macrobond_data_api/com/com_types/__init__.py
 macrobond_data_api/com/com_types/connection.py
 macrobond_data_api/com/com_types/database.py
 macrobond_data_api/com/com_types/entity.py
 macrobond_data_api/com/com_types/metadata.py
```

### Comparing `macrobond-data-api-1.0.8/setup.cfg` & `macrobond-data-api-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `macrobond-data-api-1.0.8/setup.py` & `macrobond-data-api-2.0.0/setup.py`

 * *Files identical despite different names*

