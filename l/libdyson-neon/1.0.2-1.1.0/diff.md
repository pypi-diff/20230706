# Comparing `tmp/libdyson-neon-1.0.2.tar.gz` & `tmp/libdyson-neon-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdyson-neon-1.0.2.tar", last modified: Fri May  5 16:00:04 2023, max compression
+gzip compressed data, was "libdyson-neon-1.1.0.tar", last modified: Thu Jul  6 04:03:44 2023, max compression
```

## Comparing `libdyson-neon-1.0.2.tar` & `libdyson-neon-1.1.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/libdyson/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/libdyson/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/cloud_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_hot_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_vacuum_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/libdyson_neon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/test_bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/test_cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/test_dyson_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/mocked_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_fan_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_heating_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool_missing_env_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_purifier_humidify_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_vacuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:03:44.212032 libdyson-neon-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 04:03:44.212032 libdyson-neon-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:03:44.208032 libdyson-neon-1.1.0/libdyson/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:03:44.208032 libdyson-neon-1.1.0/libdyson/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/cloud/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/cloud/cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/cloud/cloud_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/cloud/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/cloud/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14714 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_pure_hot_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/dyson_vacuum_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/libdyson/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:03:44.208032 libdyson-neon-1.1.0/libdyson_neon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 04:03:44.000000 libdyson-neon-1.1.0/libdyson_neon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-07-06 04:03:44.000000 libdyson-neon-1.1.0/libdyson_neon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:03:44.000000 libdyson-neon-1.1.0/libdyson_neon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 04:03:44.000000 libdyson-neon-1.1.0/libdyson_neon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-06 04:03:44.000000 libdyson-neon-1.1.0/libdyson_neon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-06 04:03:44.212032 libdyson-neon-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:03:44.212032 libdyson-neon-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:03:44.212032 libdyson-neon-1.1.0/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/cloud/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/cloud/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/cloud/test_bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/cloud/test_cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/cloud/test_dyson_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/mocked_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_fan_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_heating_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_pure_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_pure_cool_missing_env_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_purifier_humidify_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-06 04:03:33.000000 libdyson-neon-1.1.0/tests/test_vacuum.py
```

### Comparing `libdyson-neon-1.0.2/LICENSE` & `libdyson-neon-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/PKG-INFO` & `libdyson-neon-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-1.0.2/libdyson/__init__.py` & `libdyson-neon-1.1.0/libdyson/__init__.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/cloud/account.py` & `libdyson-neon-1.1.0/libdyson/cloud/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import pathlib
 from typing import Callable, List, Optional
 
 import requests
 from requests.auth import AuthBase, HTTPBasicAuth
 
-from libdyson.exceptions import (
+from ..exceptions import (
     DysonAuthRequired,
     DysonInvalidAccountStatus,
     DysonInvalidAuth,
     DysonLoginFailure,
     DysonNetworkError,
     DysonOTPTooFrequently,
     DysonServerError,
```

### Comparing `libdyson-neon-1.0.2/libdyson/cloud/cloud_360_eye.py` & `libdyson-neon-1.1.0/libdyson/cloud/cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/cloud/device_info.py` & `libdyson-neon-1.1.0/libdyson/cloud/device_info.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/cloud/regions.py` & `libdyson-neon-1.1.0/libdyson/cloud/regions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/cloud/utils.py` & `libdyson-neon-1.1.0/libdyson/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/const.py` & `libdyson-neon-1.1.0/libdyson/const.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/discovery.py` & `libdyson-neon-1.1.0/libdyson/discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_360_eye.py` & `libdyson-neon-1.1.0/libdyson/dyson_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_360_heurist.py` & `libdyson-neon-1.1.0/libdyson/dyson_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_device.py` & `libdyson-neon-1.1.0/libdyson/dyson_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,21 +253,21 @@
 
     @property
     def warning_code(self) -> str:
         """Return warning code."""
         return self._get_field_value(self._status, "wacd")
 
     @property
-    def formaldehyde(self) -> Optional[int]:
+    def formaldehyde(self) -> Optional[float]:
         """Return formaldehyde reading."""
-        val = self._get_environmental_field_value("hcho")
+        val = self._get_environmental_field_value("hchr", divisor=1000)
         if val is None:
             return None
 
-        return int(val)
+        return float(val)
 
     @property
     def humidity(self) -> int:
         """Return humidity in percentage."""
         return self._get_environmental_field_value("hact")
 
     @property
```

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_pure_cool.py` & `libdyson-neon-1.1.0/libdyson/dyson_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_pure_cool_link.py` & `libdyson-neon-1.1.0/libdyson/dyson_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_pure_hot_cool_link.py` & `libdyson-neon-1.1.0/libdyson/dyson_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_pure_humidify_cool.py` & `libdyson-neon-1.1.0/libdyson/dyson_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/dyson_vacuum_device.py` & `libdyson-neon-1.1.0/libdyson/dyson_vacuum_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/exceptions.py` & `libdyson-neon-1.1.0/libdyson/exceptions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson/utils.py` & `libdyson-neon-1.1.0/libdyson/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/libdyson_neon.egg-info/PKG-INFO` & `libdyson-neon-1.1.0/libdyson_neon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 1.0.2
+Version: 1.1.0
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-1.0.2/libdyson_neon.egg-info/SOURCES.txt` & `libdyson-neon-1.1.0/libdyson_neon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/pyproject.toml` & `libdyson-neon-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/setup.cfg` & `libdyson-neon-1.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libdyson-neon
-version = 1.0.2
+version = 1.1.0
 author = The libdyson Working Group
 author_email = dotvezz@gmail.com
 license = MIT License
 license_file = LICENSE
 platforms = any
 description = A Python library for Dyson devices.
 long_description = file: README.md
```

### Comparing `libdyson-neon-1.0.2/tests/cloud/mocked_requests.py` & `libdyson-neon-1.1.0/tests/cloud/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/cloud/test_bearer_auth.py` & `libdyson-neon-1.1.0/tests/cloud/test_bearer_auth.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/cloud/test_cloud_360_eye.py` & `libdyson-neon-1.1.0/tests/cloud/test_cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/cloud/test_dyson_account.py` & `libdyson-neon-1.1.0/tests/cloud/test_dyson_account.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/cloud/utils.py` & `libdyson-neon-1.1.0/tests/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/conftest.py` & `libdyson-neon-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/mocked_mqtt.py` & `libdyson-neon-1.1.0/tests/mocked_mqtt.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_360_eye.py` & `libdyson-neon-1.1.0/tests/test_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_360_heurist.py` & `libdyson-neon-1.1.0/tests/test_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_device.py` & `libdyson-neon-1.1.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_discovery.py` & `libdyson-neon-1.1.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_fan_device.py` & `libdyson-neon-1.1.0/tests/test_fan_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_heating_device.py` & `libdyson-neon-1.1.0/tests/test_heating_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_init.py` & `libdyson-neon-1.1.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_pure_cool.py` & `libdyson-neon-1.1.0/tests/test_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_pure_cool_formaldehyde.py` & `libdyson-neon-1.1.0/tests/test_pure_cool_formaldehyde.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,8 +62,8 @@
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
     assert device.volatile_organic_compounds == 0.4
     assert device.nitrogen_dioxide == 1.1
-    assert device.formaldehyde == 1
+    assert device.formaldehyde == 0.002
```

### Comparing `libdyson-neon-1.0.2/tests/test_pure_cool_link.py` & `libdyson-neon-1.1.0/tests/test_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_pure_cool_missing_env_data.py` & `libdyson-neon-1.1.0/tests/test_pure_cool_missing_env_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             "pm10": "0005",
             "va10": "0004",
             "noxl": "0011",
             "p25r": "0010",
             "p10r": "0009",
             "sltm": "OFF",
             "hcho": "NONE",
-            "hchr": "0002",
+            "hchr": "NONE",
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
     assert device.volatile_organic_compounds == .4
     assert device.nitrogen_dioxide == 1.1
@@ -88,15 +88,14 @@
             "pm25": "0009",
             "pm10": "0005",
             "va10": "0004",
             "noxl": "0011",
             "p25r": "0010",
             "p10r": "0009",
             "sltm": "OFF",
-            "hchr": "0002",
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
     assert device.volatile_organic_compounds == .4
     assert device.nitrogen_dioxide == 1.1
```

### Comparing `libdyson-neon-1.0.2/tests/test_pure_hot_cool_link.py` & `libdyson-neon-1.1.0/tests/test_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_pure_humidify_cool.py` & `libdyson-neon-1.1.0/tests/test_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_purifier_humidify_cool_formaldehyde.py` & `libdyson-neon-1.1.0/tests/test_purifier_humidify_cool_formaldehyde.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,8 +62,8 @@
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
     assert device.volatile_organic_compounds == .4
     assert device.nitrogen_dioxide == 1.1
-    assert device.formaldehyde == 1
+    assert device.formaldehyde == 0.002
```

### Comparing `libdyson-neon-1.0.2/tests/test_utils.py` & `libdyson-neon-1.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.2/tests/test_vacuum.py` & `libdyson-neon-1.1.0/tests/test_vacuum.py`

 * *Files identical despite different names*

