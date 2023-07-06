# Comparing `tmp/bemserver-ui-0.6.0.tar.gz` & `tmp/bemserver-ui-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bemserver-ui-0.6.0.tar", last modified: Wed Jul  5 08:22:06 2023, max compression
+gzip compressed data, was "bemserver-ui-0.6.1.tar", last modified: Thu Jul  6 06:52:07 2023, max compression
```

## Comparing `bemserver-ui-0.6.0.tar` & `bemserver-ui-0.6.1.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.215582 bemserver-ui-0.6.0/bemserver_ui/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.215582 bemserver-ui-0.6.0/bemserver_ui/common/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/time.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/common/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.219583 bemserver-ui-0.6.0/bemserver_ui/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/campaign_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/flask_es6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/jinja_custom_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/partners.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.219583 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-areas.json
--rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-full.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-regions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/completeness.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/services/weather_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/internal_api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-ico.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-min.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.ico
--rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.223583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/accordionList.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
--rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/dropZone.js
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/eventLevel.js
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/filterSelect.js
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/flash.js
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/itemsCount.js
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/modalConfirm.js
--rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/pagination.js
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/spinner.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
--rw-r--r--   0 runner    (1001) docker     (123)    33601 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/tree.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/userGroup/
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/flashTimer.js
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/formController.js
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/notifications.js
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/sidebar.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/array.js
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/dict.js
--rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/fetcher.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/flaskES6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/parser.js
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/time.js
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/uuid.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
--rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/weather.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/campaignScopes/
--rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/edit.js
--rw-r--r--   0 runner    (1001) docker     (123)    46089 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/list.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    66390 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/setup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/
--rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/weatherData/
--rw-r--r--   0 runner    (1001) docker     (123)    28668 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.227583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/structuralElements/
--rw-r--r--   0 runner    (1001) docker     (123)    33076 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
--rw-r--r--   0 runner    (1001) docker     (123)    36298 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
--rw-r--r--   0 runner    (1001) docker     (123)    25577 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    19413 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
--rw-r--r--   0 runner    (1001) docker     (123)    62819 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/list.js
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/static/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/app.css
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/dragndrop.css
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/main.css
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/signin.css
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/static/styles/tree.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_admin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_services.html
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/user_group_available.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/components/users/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_available.html
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_for_group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/campaign.html
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/structural_element_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/ts_selector.html
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/flash.html
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/macros/partners.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.231583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/about.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/degree_days.html
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/energy_consumption.html
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/weather.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/manage_groups.html
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/setup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.211583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/manage.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/weather_data/
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/weather_data/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/signin.html
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/skeleton.html
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/start.html
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/stats.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/create.html
--rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/explore.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/create.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/completeness.html
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/explore.html
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.235583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/list.html
--rw-r--r--   0 runner    (1001) docker     (123)    15694 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/semantic_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/upload.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage.html
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/create.html
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/edit.html
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/list.html
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/degree_days.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/energy_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/analysis/weather.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/campaign_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/campaigns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/events/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/events/categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/services/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/missing_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/outlier_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/services/weather_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/structural_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.239583 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/datastates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/timeseries/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/bemserver_ui/views/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.215582 bemserver-ui-0.6.0/bemserver_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 08:22:06.000000 bemserver-ui-0.6.0/bemserver_ui.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/requirements/install.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-05 08:22:06.247583 bemserver-ui-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-05 08:21:58.000000 bemserver-ui-0.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.302960 bemserver-ui-0.6.1/bemserver_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.306960 bemserver-ui-0.6.1/bemserver_ui/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/common/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/common/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/common/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.306960 bemserver-ui-0.6.1/bemserver_ui/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/campaign_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/flask_es6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/jinja_custom_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/partners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.310960 bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66289 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/timezones-areas.json
+-rw-r--r--   0 runner    (1001) docker     (123)   224723 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/timezones-full.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/timezones-regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/timezones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.310960 bemserver-ui-0.6.1/bemserver_ui/internal_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.310960 bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/completeness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.310960 bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.310960 bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/energy/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/energy/consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/energy/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.310960 bemserver-ui-0.6.1/bemserver_ui/internal_api/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/services/weather_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.314960 bemserver-ui-0.6.1/bemserver_ui/internal_api/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/internal_api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.298960 bemserver-ui-0.6.1/bemserver_ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.314960 bemserver-ui-0.6.1/bemserver_ui/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    16100 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver-ico.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8481 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver-min.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11477 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.314960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.314960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.314960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/accordionList.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/dropZone.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/eventLevel.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/filterSelect.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/flash.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/itemsCount.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/modalConfirm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15559 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/pagination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/spinner.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/time/
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/time/tzPicker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33601 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/timeseries/selector.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/tree.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/userGroup/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/flashTimer.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/formController.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/notifications.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/sidebar.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/array.js
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/dict.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12459 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/fetcher.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/flaskES6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/parser.js
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/time.js
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/uuid.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.298960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)    14470 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/analysis/weather.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/campaignScopes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11425 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)    39836 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/events/edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)    46089 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/events/list.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    66681 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/notifications/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/notifications/setup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.318960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/missingData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/missingData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/outlierData/
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/weatherData/
+-rw-r--r--   0 runner    (1001) docker     (123)    28668 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/structuralElements/
+-rw-r--r--   0 runner    (1001) docker     (123)    33076 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36298 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/delete.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25577 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19413 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62819 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/users/list.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/users/manageGroups.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/styles/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/styles/dragndrop.css
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/styles/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/styles/signin.css
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/static/styles/tree.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.302960 bemserver-ui-0.6.1/bemserver_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/templates/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.322960 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_admin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_analysis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_services.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/components/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/user_groups/group_for_campaign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/user_groups/user_group_available.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/components/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/users/user_available.html
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/components/users/user_for_group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/campaign.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/structural_element_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/ts_selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/macros/flash.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/macros/partners.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/about.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/pages/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/analysis/degree_days.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/analysis/energy_consumption.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/analysis/weather.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/manage_groups.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.326960 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/categories/
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/categories/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/categories/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/categories/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)    10620 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/notifications/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/notifications/setup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.302960 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/cleanup/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/cleanup/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/missing_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/missing_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/missing_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/outlier_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/outlier_data/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/outlier_data/manage.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/weather_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/weather_data/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/signin.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/skeleton.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/start.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/stats.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/explore.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/create.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/completeness.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/explore.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.330961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/datastates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/datastates/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/datastates/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/datastates/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.334961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/properties/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/properties/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/properties/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/semantic_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/upload.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.334961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/manage.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/manage_campaigns.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.334961 bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/create.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.334961 bemserver-ui-0.6.1/bemserver_ui/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/bemserver_ui/views/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/analysis/degree_days.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/analysis/energy_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/analysis/weather.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/campaign_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/campaigns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/bemserver_ui/views/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/events/categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/bemserver_ui/views/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/services/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/services/missing_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/services/outlier_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/services/weather_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/bemserver_ui/views/structural_elements/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/structural_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/structural_elements/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9617 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/structural_elements/structural_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/bemserver_ui/views/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/timeseries/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/timeseries/datastates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/timeseries/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12962 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/timeseries/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/bemserver_ui/views/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.306960 bemserver-ui-0.6.1/bemserver_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-06 06:52:07.000000 bemserver-ui-0.6.1/bemserver_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-07-06 06:52:07.000000 bemserver-ui-0.6.1/bemserver_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:52:07.000000 bemserver-ui-0.6.1/bemserver_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-06 06:52:07.000000 bemserver-ui-0.6.1/bemserver_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 06:52:07.000000 bemserver-ui-0.6.1/bemserver_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:52:07.338961 bemserver-ui-0.6.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/requirements/install.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-06 06:52:07.342961 bemserver-ui-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 06:51:59.000000 bemserver-ui-0.6.1/tox.ini
```

### Comparing `bemserver-ui-0.6.0/LICENSE` & `bemserver-ui-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/PKG-INFO` & `bemserver-ui-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.6.0
+Version: 0.6.1
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bemserver-ui-0.6.0/README.rst` & `bemserver-ui-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/__init__.py` & `bemserver-ui-0.6.1/bemserver_ui/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import flask
 
 from . import extensions
 from . import internal_api
 from . import views
 
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 
 def create_app(config_override=None):
     """Create application"""
     app = flask.Flask(__name__)
     app.config.from_object("bemserver_ui.settings.Config")
     app.config.from_envvar("BEMSERVER_UI_SETTINGS_FILE", silent=True)
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/common/time.py` & `bemserver-ui-0.6.1/bemserver_ui/common/time.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/common/tree.py` & `bemserver-ui-0.6.1/bemserver_ui/common/tree.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/__init__.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/api_client.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/auth.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/campaign_context.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/campaign_context.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/error_handlers.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/error_handlers.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/flask_es6.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/flask_es6.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/jinja_custom_filters.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/jinja_custom_filters.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/partners.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/partners.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/plugins.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/plugins.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/__init__.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-areas.json` & `bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/timezones-areas.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones-full.json` & `bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/timezones-full.json`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/extensions/timezones/timezones.py` & `bemserver-ui-0.6.1/bemserver_ui/extensions/timezones/timezones.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/__init__.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/completeness.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/completeness.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/degree_days.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/energy_consumption.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/energy_consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/analysis/weather.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/analysis/weather.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/campaign_scopes.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/campaigns.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/events.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/notifications.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/__init__.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/consumption.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/energy/consumption.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/energy/production.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/energy/production.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/semantics/weather.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/semantics/weather.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/cleanup.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/missing_data.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/outlier_data.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/services/weather_data.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/services/weather_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/structural_elements.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/data.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/timeseries/data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/timeseries/timeseries.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/user_groups.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/internal_api/users.py` & `bemserver-ui-0.6.1/bemserver_ui/internal_api/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/settings.py` & `bemserver-ui-0.6.1/bemserver_ui/settings.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-ico.svg` & `bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver-ico.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver-min.svg` & `bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver-min.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.ico` & `bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver.ico`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/images/bemserver.svg` & `bemserver-ui-0.6.1/bemserver_ui/static/images/bemserver.svg`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/app.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/app.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/accordionList.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/accordionList.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartCompleteness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartDegreeDays.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartEnergyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartExplore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/charts/tsChartWeather.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/dropZone.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/dropZone.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/eventLevel.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/eventLevel.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/filterSelect.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/filterSelect.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/flash.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/flash.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/itemsCount.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/itemsCount.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/modalConfirm.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/modalConfirm.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/pagination.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/pagination.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/spinner.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/spinner.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/structuralElements/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/time/datetimePicker.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/time/tzPicker.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/time/tzPicker.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/timeseries/bucketWidth.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/timeseries/selector.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/timeseries/selector.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/tree.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/tree.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/components/userGroup/userGroupItem.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/flashTimer.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/flashTimer.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/formController.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/formController.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/notifications.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/notifications.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/sidebar.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/sidebar.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/array.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/array.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/fetcher.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/fetcher.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/flaskES6.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/flaskES6.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/parser.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/parser.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/time.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/time.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/tools/uuid.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/tools/uuid.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/analysis/degreeDays.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/analysis/energyConsumption.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/analysis/weather.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/analysis/weather.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/campaignScopes/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/edit.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/events/edit.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/events/list.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/events/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/explore.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/notifications/explore.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -519,19 +519,19 @@
                 let notifIdPrefix = `notif-${notifId.toString()}`;
                 let notifRowElmt = document.getElementById(`${notifIdPrefix}-row`);
                 let notifTimestampElmt = document.getElementById(`${notifIdPrefix}-timestamp`);
 
                 notifRowElmt.notifData = data.data;
 
                 if (data.data.read) {
-                    notifRowElmt.classList.remove("bg-warning", "bg-opacity-10");
-                    notifTimestampElmt.classList.remove("border-start", "border-end-0", "border-5", "border-warning");
+                    notifRowElmt.classList.remove("table-warning");
+                    notifTimestampElmt.classList.remove("border-start", "border-end-0", "border-bottom-0", "border-top-0", "border-5", "border-warning", "text-warning-emphasis");
                 } else {
-                    notifRowElmt.classList.add("bg-warning", "bg-opacity-10");
-                    notifTimestampElmt.classList.add("border-start", "border-end-0", "border-5", "border-warning");
+                    notifRowElmt.classList.add("table-warning");
+                    notifTimestampElmt.classList.add("border-start", "border-end-0", "border-bottom-0", "border-top-0", "border-5", "border-warning", "text-warning-emphasis");
                 }
 
                 afterUpdateCallback?.();
             },
             (error) => {
                 let flashMsgElmt = new FlashMessage({
                     type: FlashMessageTypes.ERROR,
@@ -792,15 +792,15 @@
         timestampSortElmt.appendChild(timestampTextElmt);
 
         let timestampSortIconElmt = document.createElement("i");
         timestampSortIconElmt.classList.add("bi", "bi-sort-down");
         timestampSortElmt.appendChild(timestampSortIconElmt);
 
         let tableHeaderEventColElmt = document.createElement("th");
-        tableHeaderEventColElmt.classList.add("border-start", "border-4");
+        tableHeaderEventColElmt.classList.add("border-start", "border-top-0", "border-bottom-0", "border-end-0", "border-4");
         tableHeaderEventColElmt.setAttribute("scope", "col");
         tableHeaderEventColElmt.setAttribute("colspan", 6);
         tableHeaderElmt.appendChild(tableHeaderEventColElmt);
 
         let tableHeaderEventColContainerElmt = document.createElement("div");
         tableHeaderEventColContainerElmt.classList.add("d-flex", "justify-content-between", "gap-2");
         tableHeaderEventColElmt.appendChild(tableHeaderEventColContainerElmt);
@@ -820,15 +820,15 @@
         tableHeaderEventColContainerElmt.appendChild(markAllAsReadLinkElmt);
 
         let tableHeaderEventElmt = document.createElement("tr");
         tableHeaderEventElmt.classList.add("align-top");
         tableHeaderContainerElmt.appendChild(tableHeaderEventElmt);
 
         let tableHeaderEventTimestampColElmt = document.createElement("th");
-        tableHeaderEventTimestampColElmt.classList.add("border-start", "border-4");
+        tableHeaderEventTimestampColElmt.classList.add("border-start", "border-top-0", "border-bottom-0", "border-end-0", "border-4");
         tableHeaderEventTimestampColElmt.setAttribute("scope", "col");
         tableHeaderEventTimestampColElmt.innerText = "Timestamp";
         tableHeaderEventElmt.appendChild(tableHeaderEventTimestampColElmt);
 
         for (let eventCol of ["Source", "Level", "Category", "Campaign scope", "Description"]) {
             let tableHeaderEventInfoColElmt = document.createElement("th");
             tableHeaderEventInfoColElmt.innerText = eventCol;
@@ -881,37 +881,37 @@
     }
 
     #createNotifRowElement(notifData, campaignData, rowIndex) {
         let rowElmt = document.createElement("tr");
         rowElmt.id = `notif-${notifData.id.toString()}-row`;
         rowElmt.classList.add("align-middle");
         if (!notifData.read) {
-            rowElmt.classList.add("bg-warning", "bg-opacity-10");
+            rowElmt.classList.add("table-warning");
         }
         rowElmt.setAttribute("role", "button");
         rowElmt.setAttribute("data-bs-toggle", "modal");
         rowElmt.setAttribute("data-bs-target", "#notifInfoModal");
         rowElmt.setAttribute("data-index", rowIndex)
         rowElmt.notifData = notifData;
 
         let timestampElmt = document.createElement("th");
         timestampElmt.id = `notif-${notifData.id.toString()}-timestamp`;
         if (!notifData.read) {
-            timestampElmt.classList.add("border-start", "border-end-0", "border-5", "border-warning");
+            timestampElmt.classList.add("border-start", "border-end-0", "border-bottom-0", "border-top-0", "border-5", "border-warning", "text-warning-emphasis");
         }
         timestampElmt.setAttribute("scope", "row");
         timestampElmt.innerText = TimeDisplay.toLocaleString(new Date(notifData.timestamp), {
             timezone: campaignData.timezone
         });
         rowElmt.appendChild(timestampElmt);
 
         let eventRowElmt = this.#createEventRowElement(notifData.event, campaignData);
         for (let [cellIndex, eventCellElmt] of Object.entries(eventRowElmt.cells)) {
             if (cellIndex == 0) {
-                eventCellElmt.classList.add("border-start", "border-4");
+                eventCellElmt.classList.add("border-start", "border-end-0", "border-bottom-0", "border-top-0", "border-4");
             }
             rowElmt.appendChild(eventCellElmt);
         }
 
         return rowElmt;
     }
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/notifications/setup.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/notifications/setup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/cleanupManage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/list.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/missingData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/missingData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/outlierData/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/outlierData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/services/weatherData/manage.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/structuralElements/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/data/completeness.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/data/explore.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/delete.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/delete.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/list.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/manageStructuralElements.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/timeseries/semanticSetup.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/list.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/users/list.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/scripts/modules/views/users/manageGroups.js` & `bemserver-ui-0.6.1/bemserver_ui/static/scripts/modules/views/users/manageGroups.js`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/styles/app.css` & `bemserver-ui-0.6.1/bemserver_ui/static/styles/app.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/styles/signin.css` & `bemserver-ui-0.6.1/bemserver_ui/static/styles/signin.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/static/styles/tree.css` & `bemserver-ui-0.6.1/bemserver_ui/static/styles/tree.css`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/header.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/header.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_admin.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_admin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_analysis.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_analysis.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_context.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_campaign_selector.html`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         {{- mac_sidebar.render_nav_link("Campaigns", campaign_list_url, "Manage campaigns", ["bi", "bi-boxes"], extra_classes=["w-100"]) -}}
         {% endfilter %}
     </li>
     {% if g.campaign_ctxt.has_campaign or campaign %}
     <li id="campaignSelectedNavItem" class="nav-item d-flex justify-content-between align-items-center">
         {% filter indent(width=8, first=True) %}
         {% if g.campaign_ctxt.has_campaign %}
-        {{- mac_sidebar.render_nav_link(mac_camp.render_campaign_info(g.campaign_ctxt.name, g.campaign_ctxt.campaign.state, render_style="bullet") | indent(width=8), url_for("campaigns.view", id=g.campaign_ctxt.id), "Campaign info", [], extra_classes=["fw-bold", "text-center", "border", "border-5", "border-top-0", "border-bottom-0", "rounded-3", "app-campaign-selected", "shadow", "p-1", "w-100"]) -}}
+        {{- mac_sidebar.render_nav_link(mac_camp.render_campaign_info(g.campaign_ctxt.name, g.campaign_ctxt.campaign.state, render_style="bullet") | indent(width=8), url_for("campaigns.view", id=g.campaign_ctxt.id), g.campaign_ctxt.name, [], extra_classes=["fw-bold", "text-center", "border", "border-5", "border-top-0", "border-bottom-0", "rounded-3", "app-campaign-selected", "shadow", "p-1", "w-100"]) -}}
         {% elif campaign %}
-        {{- mac_sidebar.render_nav_link(mac_camp.render_campaign_info(campaign.name, campaign.state, render_style="bullet") | indent(width=8), url_for("campaigns.view", id=campaign.id), "Campaign info", [], extra_classes=["fw-bold", "text-center", "border", "border-5", "border-top-0", "border-bottom-0", "rounded-3", "app-campaign-selected", "shadow", "p-1", "w-100"]) -}}
+        {{- mac_sidebar.render_nav_link(mac_camp.render_campaign_info(campaign.name, campaign.state, render_style="bullet") | indent(width=8), url_for("campaigns.view", id=campaign.id), campaign.name, [], extra_classes=["fw-bold", "text-center", "border", "border-5", "border-top-0", "border-bottom-0", "rounded-3", "app-campaign-selected", "shadow", "p-1", "w-100"]) -}}
         {% endif %}
         {% endfilter %}
     </li>
     {% endif %}
 </ul>
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_dashboards.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_services.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_services.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/sidebar/sidebar_tsdata.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/user_groups/group_for_campaign.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/user_groups/group_for_campaign_scope.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/user_groups/user_group_available.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/user_groups/user_group_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_available.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/users/user_available.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/components/users/user_for_group.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/components/users/user_for_group.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/campaign.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/campaign.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/sidebar.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/sidebar.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/structural_element_selector.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/structural_element_selector.html`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             <span class="visually-hidden">Toggle select panel</span>
         </button>
         <div id="dropdownSearchPanel" class="dropdown-menu shadow w-100 p-4" aria-labelledby="dropdownSearchBtn">
             <div class="d-flex align-items-center gap-2 mb-2">
                 <input type="text" class="form-control form-control-sm" id="search" name="search" placeholder="Search..." aria-label="Search" aria-describedby="search" autofocus>
                 <a id="clearSearchBtn" role="button" class="link-danger text-decoration-none d-none invisible" title="Clear search filter"><i class="bi bi-x-circle"></i></a>
             </div>
-            <app-tree id="treeSelector" ignore-unselect="false" toolbar="{{ treeToolbar | tojson }}" {% if structural_element_types %} types={{ structural_element_types }}{% endif %}></app-tree>
+            <app-tree id="treeSelector" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted" ignore-unselect="false" toolbar="{{ treeToolbar | tojson }}"{% if structural_element_types %} types={{ structural_element_types }}{% endif %}></app-tree>
         </div>
     </div>
 </app-structural-element-selector>
 {% endmacro %}
 
 {% macro render_site_selector(html_element_id=none, title="Sites selection") %}
     {{- _render_structural_element_selector(html_element_id=html_element_id, title=title) }}
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/macros/components/ts_selector.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/macros/components/ts_selector.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/macros/flash.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/macros/flash.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/macros/partners.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/macros/partners.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/about.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/about.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/degree_days.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/analysis/degree_days.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                         </button>
                     </h2>
                     <div id="collapseParams" class="accordion-collapse collapse show" aria-labelledby="headingParams" data-bs-parent="#accordionParams">
                         <div class="accordion-body">
                             <div class="row row-cols-1 row-cols-xl-2 g-3 g-xl-4 mb-3">
                                 <div class="col">
                                     <h5 class="text-secondary"><i class="bi bi-buildings"></i> Sites</h5>
-                                    <app-tree id="sitesTree" toolbar="false"></app-tree>
+                                    <app-tree id="sitesTree" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted" toolbar="false"></app-tree>
                                 </div>
                                 <div class="col">
                                     <h5 class="text-secondary"><i class="bi bi-calendar4-range"></i> Period</h5>
                                     <div class="d-grid gap-2 mb-3">
                                         <select id="periodType" class="form-select form-select-sm" aria-label="Select a period" required>
                                             <option value="Month-Daily">Daily over 1 month</option>
                                             <option value="Year-Monthly" selected>Monthly over 1 year</option>
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/energy_consumption.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/analysis/energy_consumption.html`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,16 @@
                             <span class="fw-bold text-secondary"><i class="bi bi-easel"></i> Analysis parameters</span>
                         </button>
                     </h2>
                     <div id="collapseParams" class="accordion-collapse collapse show" aria-labelledby="headingParams" data-bs-parent="#accordionParams">
                         <div class="accordion-body">
                             <div class="row row-cols-1 row-cols-xl-2 g-3 g-xl-4">
                                 <div class="col">
-                                    <h5 class="text-secondary"><i class="bi bi-buildings"></i> Sites and buildings</h5>
-                                    <app-tree id="sitesTree"></app-tree>
+                                    <h5 class="text-secondary"><i class="bi bi-buildings"></i> Sites</h5>
+                                    <app-tree id="sitesTree" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted"></app-tree>
                                 </div>
                                 <div class="col">
                                     <h5 class="text-secondary"><i class="bi bi-calendar4-range"></i> Period</h5>
                                     <div class="d-grid gap-2">
                                         <select id="periodType" class="form-select" aria-label="Select a period" required>
                                             <option value="Month-Hourly">Hourly consumption over 1 month</option>
                                             <option value="Month-Daily" selected>Daily consumption over 1 month</option>
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/analysis/weather.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/analysis/weather.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                         </button>
                     </h2>
                     <div id="collapseParams" class="accordion-collapse collapse show" aria-labelledby="headingParams" data-bs-parent="#accordionParams">
                         <div class="accordion-body">
                             <div class="row row-cols-1 row-cols-xl-2 g-3 g-xl-4 mb-2">
                                 <div class="col">
                                     <h5 class="text-secondary"><i class="bi bi-buildings"></i> Sites</h5>
-                                    <app-tree id="sitesTree" toolbar="false"></app-tree>
+                                    <app-tree id="sitesTree" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted" toolbar="false"></app-tree>
                                 </div>
                                 <div class="col">
                                     <h5 class="text-secondary"><i class="bi bi-calendar4-range"></i> Period</h5>
                                     <div class="d-grid gap-2">
                                         <select id="periodType" class="form-select" aria-label="Select a period" required>
                                             <option value="Last-Day" selected>Last 24 hours</option>
                                             <option value="Last-Week">Last 7 days</option>
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/base.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/base.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaign_scopes/view.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaign_scopes/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/manage_groups.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/manage_groups.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/campaigns/view.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/campaigns/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/categories/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/categories/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/categories/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/categories/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/events/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/events/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/explore.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/notifications/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/notifications/setup.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/notifications/setup.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/cleanup/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/cleanup/manage.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/cleanup/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/missing_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/missing_data/manage.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/missing_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/outlier_data/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/outlier_data/manage.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/outlier_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/services/weather_data/manage.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/services/weather_data/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/signin.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/signin.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/skeleton.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/skeleton.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/start.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/start.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/stats.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/stats.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/explore.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/explore.html`

 * *Files 6% similar despite different names*

```diff
@@ -48,18 +48,18 @@
                 </li>
                 <li class="nav-item" role="presentation">
                     <button class="nav-link{% if tab == 'zones' %} active{% endif %}" id="zones-tab" data-bs-toggle="tab" data-bs-target="#zones-tabcontent" type="button" role="tab" aria-controls="zones-tabcontent" aria-selected="{% if tab == 'zones' %}true{% else %}false{% endif %}"><i class="bi bi-bullseye me-1"></i>Zones</button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white" id="tabSitesContent">
                 <div class="tab-pane fade{% if tab == 'sites' %} show active{% endif %} p-3" id="sites-tabcontent" role="tabpanel" aria-labelledby="sites-tab">
-                    <app-tree id="sitesTree"></app-tree>
+                    <app-tree id="sitesTree" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted"></app-tree>
                 </div>
                 <div class="tab-pane fade{% if tab == 'zones' %} show active{% endif %} p-3" id="zones-tabcontent" role="tabpanel" aria-labelledby="zones-tab">
-                    <app-tree id="zonesTree" toolbar="false"></app-tree>
+                    <app-tree id="zonesTree" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted" toolbar="false"></app-tree>
                 </div>
             </div>
         </div>
         <div class="col">
             <div id="alertInfoData" class="alert alert-info" role="alert">
                 <i class="bi bi-info-square float-start me-2"></i>
                 <span>Select a <span class="fw-bold">site/building/storey/space or zone</span> in the tree to explore its data.</span>
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/properties/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/structural_elements/upload.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/structural_elements/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/completeness.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/completeness.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/delete.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/delete.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/explore.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/explore.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/data/upload.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/data/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/datastates/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/datastates/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/datastates/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/datastates/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/manage_structural_elements.html`

 * *Files 4% similar despite different names*

```diff
@@ -35,26 +35,26 @@
             <div class="alert alert-info alert-dismissible fade show" role="alert">
                 <i class="bi bi-info-square float-start me-2"></i>
                 <span>Open a timeseries accordion panel to <span class="fw-bold fst-italic">drag and drop</span> locations over it.</span>
                 <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
             </div>
             <ul class="nav nav-tabs app-tabs" id="tabSites" role="tablist">
                 <li class="nav-item" role="presentation">
-                    <button class="nav-link active" id="sites-tab" data-bs-toggle="tab" data-bs-target="#sites-tabcontent" type="button" role="tab" aria-controls="sites-tabcontent" aria-selected="true"><i class="bi bi-buildings"></i> Sites / Buildings...</button>
+                    <button class="nav-link active" id="sites-tab" data-bs-toggle="tab" data-bs-target="#sites-tabcontent" type="button" role="tab" aria-controls="sites-tabcontent" aria-selected="true"><i class="bi bi-buildings"></i> Sites</button>
                 </li>
                 <li class="nav-item" role="presentation">
                     <button class="nav-link" id="zones-tab" data-bs-toggle="tab" data-bs-target="#zones-tabcontent" type="button" role="tab" aria-controls="zones-tabcontent" aria-selected="false"><i class="bi bi-bullseye"></i> Zones</button>
                 </li>
             </ul>
             <div class="tab-content app-tab-content overflow-auto border border-top-0 bg-white" id="tabSitesContent">
                 <div class="tab-pane fade show active p-3" id="sites-tabcontent" role="tabpanel" aria-labelledby="sites-tab">
-                    <app-tree id="sitesTree"></app-tree>
+                    <app-tree id="sitesTree" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted"></app-tree>
                 </div>
                 <div class="tab-pane fade p-3" id="zones-tabcontent" role="tabpanel" aria-labelledby="zones-tab">
-                    <app-tree id="zonesTree" toolbar="false"></app-tree>
+                    <app-tree id="zonesTree" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted" toolbar="false"></app-tree>
                 </div>
             </div>
 
         </div>
     </div>
 </div>
 {% endblock main_content %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends "pages/base.html" %} {% set title = "Timeseries" %} {% set subtitle
 = "Manage locations" %} {% block main_content %} {{ super() -}}
 Search [search              ]
 ** Locations available **
  Open a timeseries accordion panel to drag and drop locations over it.
-    *  Sites / Buildings...
+    *  Sites
     *  Zones
 {% endblock main_content %} {% block body_scripts %} {{ super() -}} {% filter
 indent(width=8, first=True) %}
  {% endfilter %} {% endblock body_scripts %}
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/properties/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/properties/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/properties/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/properties/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/semantic_setup.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/semantic_setup.html`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 {% endblock main_toolbar %}
 
 {% block main_content %}
 {{ super() -}}
 <div class="container-fluid">
     <div class="row mb-3">
         <div class="col">
-            <h5 class="text-secondary"><i class="bi bi-buildings"></i> Sites and buildings</h5>
-            <app-tree id="sitesTree" class="bg-light"></app-tree>
+            <h5 class="text-secondary"><i class="bi bi-buildings"></i> Sites</h5>
+            <app-tree id="sitesTree" class="bg-light" icon="bi,bi-dash-square-dotted" icon-collapsed="bi,bi-plus-square" icon-expanded="bi,bi-dash-square-dotted"></app-tree>
         </div>
     </div>
     <div class="row">
         <div class="col">
             <h5 class="text-secondary"><i class="bi bi-clock-history"></i> Timeseries semantic setup</h5>
             <ul class="nav nav-tabs app-tabs" role="tablist">
                 <li class="nav-item" role="presentation">
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 "pages/base.html" %} {% set title = "Timeseries" %} {% set subtitle = "Semantic
 setup" %} {% if not tab %} {% set tab = "weather" %} {% endif %} {% set
 is_editable = signed_user.is_admin %} {% block main_toolbar %} {{ super() -}}
 {% filter indent(width=20, first=True) %}
  Back_to_timeseries
  {% endfilter %} {% endblock main_toolbar %} {% block main_content %} {{ super
 () -}}
- Sites and buildings
+ Sites
  Timeseries semantic setup
     * Weather
     * Weather forecast
     * Energy production
     * Energy consumption
  Help
 Select a site in the tree to see its weather parameters setup.
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/timeseries/upload.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/timeseries/upload.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/manage.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/manage_campaign_scopes.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/manage_campaigns.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/manage_campaigns.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/user_groups/view.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/user_groups/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/create.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/create.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/edit.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/edit.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/list.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/list.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/templates/pages/users/view.html` & `bemserver-ui-0.6.1/bemserver_ui/templates/pages/users/view.html`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/__init__.py` & `bemserver-ui-0.6.1/bemserver_ui/views/__init__.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/analysis/degree_days.py` & `bemserver-ui-0.6.1/bemserver_ui/views/analysis/degree_days.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/auth.py` & `bemserver-ui-0.6.1/bemserver_ui/views/auth.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/campaign_scopes.py` & `bemserver-ui-0.6.1/bemserver_ui/views/campaign_scopes.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/campaigns.py` & `bemserver-ui-0.6.1/bemserver_ui/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/events/categories.py` & `bemserver-ui-0.6.1/bemserver_ui/views/events/categories.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/events/events.py` & `bemserver-ui-0.6.1/bemserver_ui/views/events/events.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/main.py` & `bemserver-ui-0.6.1/bemserver_ui/views/main.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/notifications.py` & `bemserver-ui-0.6.1/bemserver_ui/views/notifications.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/services/cleanup.py` & `bemserver-ui-0.6.1/bemserver_ui/views/services/cleanup.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/services/missing_data.py` & `bemserver-ui-0.6.1/bemserver_ui/views/services/missing_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/services/outlier_data.py` & `bemserver-ui-0.6.1/bemserver_ui/views/services/outlier_data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/properties.py` & `bemserver-ui-0.6.1/bemserver_ui/views/structural_elements/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/structural_elements/structural_elements.py` & `bemserver-ui-0.6.1/bemserver_ui/views/structural_elements/structural_elements.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/data.py` & `bemserver-ui-0.6.1/bemserver_ui/views/timeseries/data.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/datastates.py` & `bemserver-ui-0.6.1/bemserver_ui/views/timeseries/datastates.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/properties.py` & `bemserver-ui-0.6.1/bemserver_ui/views/timeseries/properties.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/timeseries/timeseries.py` & `bemserver-ui-0.6.1/bemserver_ui/views/timeseries/timeseries.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/user_groups.py` & `bemserver-ui-0.6.1/bemserver_ui/views/user_groups.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui/views/users.py` & `bemserver-ui-0.6.1/bemserver_ui/views/users.py`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/bemserver_ui.egg-info/PKG-INFO` & `bemserver-ui-0.6.1/bemserver_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bemserver-ui
-Version: 0.6.0
+Version: 0.6.1
 Summary: BEMServer web interface
 Home-page: https://github.com/BEMServer/bemserver-ui
 Author: NOBATEK/INEF4
 Author-email: dfrederique@nobatek.inef4.com
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bemserver-ui-0.6.0/bemserver_ui.egg-info/SOURCES.txt` & `bemserver-ui-0.6.1/bemserver_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/requirements/dev.txt` & `bemserver-ui-0.6.1/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/requirements/install.txt` & `bemserver-ui-0.6.1/requirements/install.txt`

 * *Files identical despite different names*

### Comparing `bemserver-ui-0.6.0/setup.py` & `bemserver-ui-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Get the long description from the README file
 with open("README.rst", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="bemserver-ui",
-    version="0.6.0",
+    version="0.6.1",
     description="BEMServer web interface",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/BEMServer/bemserver-ui",
     author="NOBATEK/INEF4",
     author_email="dfrederique@nobatek.inef4.com",
     license="AGPLv3+",
```

