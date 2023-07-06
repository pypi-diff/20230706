# Comparing `tmp/forecastmanager-0.0.5.tar.gz` & `tmp/forecastmanager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastmanager-0.0.5.tar", last modified: Wed Jul  5 13:33:54 2023, max compression
+gzip compressed data, was "forecastmanager-0.0.6.tar", last modified: Thu Jul  6 08:35:03 2023, max compression
```

## Comparing `forecastmanager-0.0.5.tar` & `forecastmanager-0.0.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.071714 forecastmanager-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-05 13:33:54.071714 forecastmanager-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.063714 forecastmanager-0.0.5/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.063714 forecastmanager-0.0.5/forecastmanager/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.067714 forecastmanager-0.0.5/forecastmanager/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/management/commands/generate_forecast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.067714 forecastmanager-0.0.5/forecastmanager/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/site_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.063714 forecastmanager-0.0.5/forecastmanager/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.063714 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.071714 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/clearsky.png
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/cloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/fair.png
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/fog.png
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightrain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightrainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsnow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/partlycloudy.png
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rain.png
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rainandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rainshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleet.png
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleetandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleetshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snow.png
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snowandthunder.png
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snowshowers.png
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.071714 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/js/
--rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/js/forecast_basemap.js
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/static/forecastmanager/js/helpers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.063714 forecastmanager-0.0.5/forecastmanager/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.071714 forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/create_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/forecast_base.html
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/load_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/query_forecast.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/forecastmanager/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 13:33:54.063714 forecastmanager-0.0.5/forecastmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-05 13:33:54.000000 forecastmanager-0.0.5/forecastmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-05 13:33:54.000000 forecastmanager-0.0.5/forecastmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 13:33:54.000000 forecastmanager-0.0.5/forecastmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-05 13:33:54.000000 forecastmanager-0.0.5/forecastmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 13:33:54.000000 forecastmanager-0.0.5/forecastmanager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 13:33:39.000000 forecastmanager-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-05 13:33:54.071714 forecastmanager-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.810488 forecastmanager-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 08:35:03.810488 forecastmanager-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.802487 forecastmanager-0.0.6/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.802487 forecastmanager-0.0.6/forecastmanager/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.802487 forecastmanager-0.0.6/forecastmanager/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/management/commands/generate_forecast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.806488 forecastmanager-0.0.6/forecastmanager/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/site_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.802487 forecastmanager-0.0.6/forecastmanager/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.802487 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.810488 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/clearsky.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/cloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/fair.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/fog.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11065 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11822 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightrain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightrainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightrainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsnow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsnowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/partlycloudy.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rain.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rainandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rainshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleet.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleetandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleetshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snowandthunder.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snowshowers.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.810488 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    38899 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/js/forecast_basemap.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/static/forecastmanager/js/helpers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.802487 forecastmanager-0.0.6/forecastmanager/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.810488 forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/create_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/forecast_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/load_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/query_forecast.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/forecastmanager/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:35:03.802487 forecastmanager-0.0.6/forecastmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 08:35:03.000000 forecastmanager-0.0.6/forecastmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-06 08:35:03.000000 forecastmanager-0.0.6/forecastmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:35:03.000000 forecastmanager-0.0.6/forecastmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 08:35:03.000000 forecastmanager-0.0.6/forecastmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-06 08:35:03.000000 forecastmanager-0.0.6/forecastmanager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 08:34:39.000000 forecastmanager-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-06 08:35:03.810488 forecastmanager-0.0.6/setup.cfg
```

### Comparing `forecastmanager-0.0.5/PKG-INFO` & `forecastmanager-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.5
+Version: 0.0.6
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.5/forecastmanager/blocks.py` & `forecastmanager-0.0.6/forecastmanager/blocks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/management/commands/generate_forecast.py` & `forecastmanager-0.0.6/forecastmanager/management/commands/generate_forecast.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/migrations/0001_initial.py` & `forecastmanager-0.0.6/forecastmanager/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/models.py` & `forecastmanager-0.0.6/forecastmanager/models.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/serializers.py` & `forecastmanager-0.0.6/forecastmanager/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,43 +16,43 @@
 
         return obj.coordinates
     
 
 class ForecastSerializer(serializers.ModelSerializer):
 
     city_detail =  serializers.SerializerMethodField()
-    condition_display = serializers.SerializerMethodField()
+    # condition_display = serializers.SerializerMethodField()
     list_serializer_class = serializers.ListSerializer
 
     class Meta:
         model = Forecast
-        fields =['id','forecast_date','max_temp','min_temp', 'condition_display', 'city', 'city_detail', 'condition']
+        fields =['id','forecast_date','max_temp','min_temp', 'city', 'city_detail', 'condition']
 
 
     @staticmethod
     def get_city_detail(obj):
         serializer = CitySerializer(obj.city)
         return serializer.data
     
-    def get_condition_display(self, obj):
-            return obj.get_condition_display()
+    # def get_condition_display(self, obj):
+    #         return obj.get_condition_display()
     
     def to_representation(self, instance):
         representation = super().to_representation(instance)
 
         forecast_feature = {
             "type": "Feature",
             "properties": {
                 'id': representation['id'],
                 'city_name': representation['city_detail']['name'],
                 'forecast_date': representation['forecast_date'],
                 'max_temp': representation['max_temp'],
                 'min_temp': representation['min_temp'],
-                'condition':representation['condition_display'],
-                'condition_icon': f'static/forecastmanager/img/{representation["condition"]}.png',
+                'condition':representation['condition'],
+                'condition_icon': f'{representation["condition"]}.png',
             },
             "geometry": {
                 "coordinates": representation['city_detail']['coordinates'],
                 "type": "Point"
             }
         }
```

### Comparing `forecastmanager-0.0.5/forecastmanager/site_settings.py` & `forecastmanager-0.0.6/forecastmanager/site_settings.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/clearsky.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/clearsky.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/cloudy.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/cloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/fair.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/fair.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/fog.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/fog.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrain.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrainshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavyrainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleet.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleetshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnow.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnowshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/heavysnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightrain.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightrain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightrainandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightrainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightrainshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightrainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsleet.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsleetshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsnow.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsnow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsnowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightsnowshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightsnowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightssleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/lightssnowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/partlycloudy.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/partlycloudy.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rain.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rain.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rainandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rainandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rainshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rainshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/rainshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleet.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleet.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleetandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleetandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleetshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleetshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/sleetshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snow.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snow.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snowandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snowandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snowshowers.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snowshowers.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/img/snowshowersandthunder.png`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/js/forecast_basemap.js` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/js/forecast_basemap.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/static/forecastmanager/js/helpers.js` & `forecastmanager-0.0.6/forecastmanager/static/forecastmanager/js/helpers.js`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/create_forecast.html` & `forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/create_forecast.html`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,14 @@
   document.addEventListener("DOMContentLoaded", function () {
 
     var weather_condition_ls = JSON.parse('{{weather_condition_ls|escapejs}}')
 
     var city_ls = JSON.parse('{{city_ls|escapejs}}')
 
     const container = document.querySelector('#createTable');
-    const BASE_URL = '{{request.get_full_path}}'
-
     
     const hot = new Handsontable(container, {
       width: '100%',
       rowHeaders: true,
       colHeaders: [
         'City',
         'Min Temp',
@@ -324,15 +322,15 @@
           };
           postData.push(row);
 
         }
 
         // Send the JSON data to a Django view via AJAX
         $.ajax({
-          url: `${BASE_URL}/api/forecasts/`,
+          url: `{% url 'forecast-list'%}`,
           type: 'POST',
           headers: {
             'X-CSRFToken': '{{ csrf_token }}',  // Replace with the actual CSRF token value
           },
           data: JSON.stringify(postData),
           contentType: 'application/json',
           success: function (response) {
```

### Comparing `forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/forecast_base.html` & `forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/forecast_base.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/load_forecast.html` & `forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/load_forecast.html`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     
    
     <script type="text/javascript">
     
 
         document.addEventListener("DOMContentLoaded", function() {
             
-        const BASE_URL = '{{request.get_full_path}}'
         // initialize map     
         var forecastMap = new maplibregl.Map({
             container:'forecast_map',
             style: basemap,
             center:[39.67458166409534,8.709054632756391],
             zoom:4.5
         })
@@ -146,33 +145,32 @@
                 easing: function (t) {
                     return t * (2 - t); // Cubic easing function
                   }
             })
 
         }
 
-        function setForecastData(forecast_date){
-
+        function setForecastData(forecast_date){    
             // Make an HTTP GET request to the API endpoint
-            fetch(`${BASE_URL}api/forecasts?forecast_date=${forecast_date}`)
+            fetch(`{% url 'forecast-list'%}?forecast_date=${forecast_date}`)
             .then(response => response.json())  // Parse the response as JSON
             .then(data => {
                 // Process the retrieved data
                 data.map(icon => {
     
     
                     let img = new Image()
 
                     img.onload = () => {
                         if (!forecastMap.hasImage(icon.properties.condition_icon)) {
                             return forecastMap.addImage(`${icon.properties.condition_icon}`, img)
                         }
 
                     }
-                    img.src = `${BASE_URL}${icon.properties.condition_icon}`
+                    img.src = `{% static 'forecastmanager/img/${icon.properties.condition_icon}' %}`
                     return img.src
     
                 })
                 // Access and use the data as needed                
                 populateMap({
                     type: "FeatureCollection",
                     features:data
```

### Comparing `forecastmanager-0.0.5/forecastmanager/templates/forecastmanager/query_forecast.html` & `forecastmanager-0.0.6/forecastmanager/templates/forecastmanager/query_forecast.html`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/views.py` & `forecastmanager-0.0.6/forecastmanager/views.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager/wagtail_hooks.py` & `forecastmanager-0.0.6/forecastmanager/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/forecastmanager.egg-info/PKG-INFO` & `forecastmanager-0.0.6/forecastmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastmanager
-Version: 0.0.5
+Version: 0.0.6
 Summary: Integration of Weather City Forecasts Manager in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/forecastmanager
 Author: Grace Amondi
 Author-email: miswa.grace@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `forecastmanager-0.0.5/forecastmanager.egg-info/SOURCES.txt` & `forecastmanager-0.0.6/forecastmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forecastmanager-0.0.5/setup.cfg` & `forecastmanager-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastmanager
-version = 0.0.5
+version = 0.0.6
 description = Integration of Weather City Forecasts Manager in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/forecastmanager
 author = Grace Amondi
 author_email = miswa.grace@gmail.com
 license = MIT
```

