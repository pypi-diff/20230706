# Comparing `tmp/zigpy-0.56.1.tar.gz` & `tmp/zigpy-0.56.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-0.56.1.tar", last modified: Thu Jun 22 21:09:27 2023, max compression
+gzip compressed data, was "zigpy-0.56.2.tar", last modified: Thu Jul  6 21:30:46 2023, max compression
```

## Comparing `zigpy-0.56.1.tar` & `zigpy-0.56.2.tar`

### file list

```diff
@@ -1,85 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 21:09:23.000000 zigpy-0.56.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-22 21:09:23.000000 zigpy-0.56.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-22 21:09:27.416668 zigpy-0.56.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-22 21:09:23.000000 zigpy-0.56.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-22 21:09:27.420668 zigpy-0.56.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-22 21:09:23.000000 zigpy-0.56.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.408668 zigpy-0.56.1/zigpy/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/appdb_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v0.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v1.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v12.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v2.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v4.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v5.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v6.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v8.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v9.sql
--rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/backups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/ota/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/zgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/zha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/zll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/quirks/
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/quirks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/quirks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/types/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/zcl/
--rw-r--r--   0 runner    (1001) docker     (123)    35495 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/zcl/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/closures.py
--rw-r--r--   0 runner    (1001) docker     (123)    90858 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/hvac.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/manufacturer_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16606 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/zdo/
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zdo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.408668 zigpy-0.56.1/zigpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.084423 zigpy-0.56.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-06 21:30:35.000000 zigpy-0.56.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-06 21:30:35.000000 zigpy-0.56.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-06 21:30:46.084423 zigpy-0.56.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-06 21:30:35.000000 zigpy-0.56.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-06 21:30:35.000000 zigpy-0.56.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:30:46.084423 zigpy-0.56.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-06 21:30:35.000000 zigpy-0.56.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.072422 zigpy-0.56.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_app_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_appdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15944 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_appdb_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_appdb_pysqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43780 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11948 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16848 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19107 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_ota_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35673 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_quirks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_quirks_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23058 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_topology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22446 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37037 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23451 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zcl_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24602 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zcl_foundation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zdo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14523 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zdo_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-07-06 21:30:35.000000 zigpy-0.56.2/tests/test_zigbee_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.076422 zigpy-0.56.2/zigpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45445 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/appdb_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v0.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v12.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v4.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v5.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v6.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v8.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/appdb_schemas/schema_v9.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/backups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/ota/
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26170 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/ota/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/zgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/zha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/profiles/zll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/quirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/quirks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/quirks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23918 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.080423 zigpy-0.56.2/zigpy/zcl/
+-rw-r--r--   0 runner    (1001) docker     (123)    35495 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.084423 zigpy-0.56.2/zigpy/zcl/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90858 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/manufacturer_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16606 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/clusters/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zcl/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.084423 zigpy-0.56.2/zigpy/zdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-07-06 21:30:35.000000 zigpy-0.56.2/zigpy/zdo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:30:46.076422 zigpy-0.56.2/zigpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7949 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 21:30:46.000000 zigpy-0.56.2/zigpy.egg-info/top_level.txt
```

### Comparing `zigpy-0.56.1/COPYING` & `zigpy-0.56.2/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/LICENSE` & `zigpy-0.56.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/PKG-INFO` & `zigpy-0.56.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.56.1
-Summary: Library implementing a ZigBee stack
-Home-page: https://github.com/zigpy/zigpy
-Author: Russell Cloran
-Author-email: rcloran@gmail.com
+Version: 0.56.2
+Summary: Library implementing a Zigbee stack
+Author-email: Russell Cloran <rcloran@gmail.com>
 License: GPL-3.0
-Platform: UNKNOWN
+Project-URL: repository, https://github.com/zigpy/zigpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 License-File: COPYING
 
 # zigpy
 
 [![Build](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)
 [![Coverage Status](https://codecov.io/gh/zigpy/zigpy/branch/dev/graph/badge.svg)](https://codecov.io/gh/zigpy/zigpy)
@@ -75,9 +74,7 @@
 - https://pypi.org/project/zigpy/
   - https://pypi.org/project/bellows/
   - https://pypi.org/project/zigpy-cc/
   - https://pypi.org/project/zigpy-deconz/
   - https://pypi.org/project/zigpy-xbee/
   - https://pypi.org/project/zigpy-zigate/
   - https://pypi.org/project/zigpy-znp/
-
-
```

### Comparing `zigpy-0.56.1/README.md` & `zigpy-0.56.2/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb.py` & `zigpy-0.56.2/zigpy/appdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
         self._application.backups.backups.clear()
 
         async with self.execute(
             f"SELECT * FROM network_backups{DB_V} ORDER BY id"
         ) as cursor:
             backups = []
 
-            async for id_, backup_json in cursor:
+            async for _id, backup_json in cursor:
                 backup = zigpy.backups.NetworkBackup.from_dict(json.loads(backup_json))
                 backups.append(backup)
 
         backups.sort(key=lambda b: b.backup_time)
 
         for backup in backups:
             self._application.backups.add_backup(backup, suppress_event=True)
@@ -918,17 +918,15 @@
                         elif errors == "warn":
                             LOGGER.warning(
                                 "Failed to migrate row %s%s: %s", old_table, row, e
                             )
                         elif errors == "ignore":
                             pass
                         else:
-                            raise ValueError(
-                                f"Invalid value for `errors`: {errors!r}"
-                            )  # noqa
+                            raise ValueError(f"Invalid value for `errors`: {errors!r}")
 
     async def _migrate_to_v4(self):
         """Schema v4 expanded the node descriptor and neighbor table columns"""
         # The `node_descriptors` table was added in v1
         if await self._table_exists("node_descriptors"):
             async with self.execute("SELECT * FROM node_descriptors") as cur:
                 async for dev_ieee, value in cur:
```

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v0.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v0.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v1.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v1.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v10.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v10.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v11.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v11.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v12.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v12.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v2.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v2.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v3.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v3.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v4.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v4.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v5.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v5.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v6.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v6.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v7.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v7.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v8.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v8.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/appdb_schemas/schema_v9.sql` & `zigpy-0.56.2/zigpy/appdb_schemas/schema_v9.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/application.py` & `zigpy-0.56.2/zigpy/application.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/backups.py` & `zigpy-0.56.2/zigpy/backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/config/__init__.py` & `zigpy-0.56.2/zigpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/config/defaults.py` & `zigpy-0.56.2/zigpy/config/defaults.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/config/validators.py` & `zigpy-0.56.2/zigpy/config/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/const.py` & `zigpy-0.56.2/zigpy/const.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/device.py` & `zigpy-0.56.2/zigpy/device.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/endpoint.py` & `zigpy-0.56.2/zigpy/endpoint.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/exceptions.py` & `zigpy-0.56.2/zigpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/group.py` & `zigpy-0.56.2/zigpy/group.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/listeners.py` & `zigpy-0.56.2/zigpy/listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/ota/__init__.py` & `zigpy-0.56.2/zigpy/ota/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/ota/image.py` & `zigpy-0.56.2/zigpy/ota/image.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/ota/provider.py` & `zigpy-0.56.2/zigpy/ota/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,15 +577,15 @@
 
     async def refresh_firmware_list(self) -> None:
         if self._ota_dir is None:
             return None
 
         self._cache.clear()
         loop = asyncio.get_event_loop()
-        for root, dirs, files in os.walk(self._ota_dir):
+        for root, _dirs, files in os.walk(self._ota_dir):
             for file in files:
                 if file in SKIP_OTA_FILES:
                     continue
                 file_name = os.path.join(root, file)
                 img = await loop.run_in_executor(None, FileImage.scan_image, file_name)
                 if img is None:
                     continue
@@ -691,15 +691,15 @@
                             rsp.reason,
                         )
                         return
                     fw_lst = await rsp.json()
         self.debug("Finished downloading firmware update list")
         self._cache.clear()
 
-        for model, firmwares in fw_lst.items():
+        for _model, firmwares in fw_lst.items():
             for firmware in firmwares:
                 img = INOVELLIImage.from_json(firmware)
 
                 # Only replace the previously-cached image if its version is smaller
                 if (
                     img.key in self._cache
                     and self._cache[img.key].version > img.version
```

### Comparing `zigpy-0.56.1/zigpy/ota/validators.py` & `zigpy-0.56.2/zigpy/ota/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/profiles/zgp.py` & `zigpy-0.56.2/zigpy/profiles/zgp.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/profiles/zha.py` & `zigpy-0.56.2/zigpy/profiles/zha.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/profiles/zll.py` & `zigpy-0.56.2/zigpy/profiles/zll.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/quirks/__init__.py` & `zigpy-0.56.2/zigpy/quirks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             setattr(self, attr, getattr(replaces, attr))
 
         set_device_attr("status")
         set_device_attr(SIG_NODE_DESC)
         set_device_attr(SIG_MANUFACTURER)
         set_device_attr(SIG_MODEL)
         set_device_attr(SIG_SKIP_CONFIG)
-        for endpoint_id, endpoint in self.replacement.get(SIG_ENDPOINTS, {}).items():
+        for endpoint_id, _endpoint in self.replacement.get(SIG_ENDPOINTS, {}).items():
             self.add_endpoint(endpoint_id, replace_device=replaces)
 
     def add_endpoint(
         self, endpoint_id: int, replace_device: zigpy.device.Device | None = None
     ) -> zigpy.endpoint.Endpoint:
         if endpoint_id not in self.replacement.get(SIG_ENDPOINTS, {}):
             return super().add_endpoint(endpoint_id)
```

### Comparing `zigpy-0.56.1/zigpy/quirks/registry.py` & `zigpy-0.56.2/zigpy/quirks/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,53 +96,45 @@
                     "Fail because endpoint list mismatch: %s %s",
                     set(sig.keys()),
                     dev_ep,
                 )
                 continue
 
             if not all(
-                [
-                    device[eid].profile_id
-                    == sig[eid].get(SIG_EP_PROFILE, device[eid].profile_id)
-                    for eid in sig
-                ]
+                device[eid].profile_id
+                == sig[eid].get(SIG_EP_PROFILE, device[eid].profile_id)
+                for eid in sig
             ):
                 _LOGGER.debug(
                     "Fail because profile_id mismatch on at least one endpoint"
                 )
                 continue
 
             if not all(
-                [
-                    device[eid].device_type
-                    == sig[eid].get(SIG_EP_TYPE, device[eid].device_type)
-                    for eid in sig
-                ]
+                device[eid].device_type
+                == sig[eid].get(SIG_EP_TYPE, device[eid].device_type)
+                for eid in sig
             ):
                 _LOGGER.debug(
                     "Fail because device_type mismatch on at least one endpoint"
                 )
                 continue
 
             if not all(
-                [
-                    self._match(device[eid].in_clusters, ep.get(SIG_EP_INPUT, []))
-                    for eid, ep in sig.items()
-                ]
+                self._match(device[eid].in_clusters, ep.get(SIG_EP_INPUT, []))
+                for eid, ep in sig.items()
             ):
                 _LOGGER.debug(
                     "Fail because input cluster mismatch on at least one endpoint"
                 )
                 continue
 
             if not all(
-                [
-                    self._match(device[eid].out_clusters, ep.get(SIG_EP_OUTPUT, []))
-                    for eid, ep in sig.items()
-                ]
+                self._match(device[eid].out_clusters, ep.get(SIG_EP_OUTPUT, []))
+                for eid, ep in sig.items()
             ):
                 _LOGGER.debug(
                     "Fail because output cluster mismatch on at least one endpoint"
                 )
                 continue
 
             _LOGGER.debug(
```

### Comparing `zigpy-0.56.1/zigpy/serial.py` & `zigpy-0.56.2/zigpy/serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/state.py` & `zigpy-0.56.2/zigpy/state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/topology.py` & `zigpy-0.56.2/zigpy/topology.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/types/basic.py` & `zigpy-0.56.2/zigpy/types/basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 class SerializableBytes:
     """A container object for raw bytes that enforces `serialize()` will be called."""
 
     def __init__(self, value: bytes = b"") -> None:
         if isinstance(value, type(self)):
             value = value.value
         elif not isinstance(value, (bytes, bytearray)):
-            raise ValueError(f"Object is not bytes: {value!r}")
+            raise ValueError(f"Object is not bytes: {value!r}")  # noqa: TRY004
 
         self.value = value
 
     def __eq__(self, other: typing.Any) -> bool:
         if not isinstance(other, type(self)):
             return NotImplemented
 
@@ -702,15 +702,15 @@
 
     def __new__(metaclass, name, bases, namespaces, **kwargs):
         cls_kwarg_attrs = namespaces.get("_getitem_kwargs", {})
 
         def __init_subclass__(cls, **kwargs):
             filtered_kwargs = kwargs.copy()
 
-            for name, value in kwargs.items():
+            for name, _value in kwargs.items():
                 if name in cls_kwarg_attrs:
                     setattr(cls, f"_{name}", filtered_kwargs.pop(name))
 
             super().__init_subclass__(**filtered_kwargs)
 
         if "__init_subclass__" not in namespaces:
             namespaces["__init_subclass__"] = __init_subclass__
@@ -817,15 +817,15 @@
         )
 
     @classmethod
     def deserialize(cls: type[T], data: bytes) -> tuple[T, bytes]:
         assert cls._item_type is not None
         length, data = cls._length_type.deserialize(data)
         r = cls()
-        for i in range(length):
+        for _i in range(length):
             item, data = cls._item_type.deserialize(data)
             r.append(item)
         return r, data
 
 
 class FixedList(list, metaclass=KwargTypeMeta):
     _item_type = None
@@ -843,15 +843,15 @@
 
         return b"".join([self._item_type(i).serialize() for i in self])
 
     @classmethod
     def deserialize(cls: type[T], data: bytes) -> tuple[T, bytes]:
         assert cls._item_type is not None
         r = cls()
-        for i in range(cls._length):
+        for _i in range(cls._length):
             item, data = cls._item_type.deserialize(data)
             r.append(item)
         return r, data
 
 
 class CharacterString(str):
     _prefix_length = 1
```

### Comparing `zigpy-0.56.1/zigpy/types/named.py` & `zigpy-0.56.2/zigpy/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/types/struct.py` & `zigpy-0.56.2/zigpy/types/struct.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/typing.py` & `zigpy-0.56.2/zigpy/typing.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/util.py` & `zigpy-0.56.2/zigpy/util.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/__init__.py` & `zigpy-0.56.2/zigpy/zcl/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/__init__.py` & `zigpy-0.56.2/zigpy/zcl/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/closures.py` & `zigpy-0.56.2/zigpy/zcl/clusters/closures.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/general.py` & `zigpy-0.56.2/zigpy/zcl/clusters/general.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/homeautomation.py` & `zigpy-0.56.2/zigpy/zcl/clusters/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/hvac.py` & `zigpy-0.56.2/zigpy/zcl/clusters/hvac.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/lighting.py` & `zigpy-0.56.2/zigpy/zcl/clusters/lighting.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/lightlink.py` & `zigpy-0.56.2/zigpy/zcl/clusters/lightlink.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/measurement.py` & `zigpy-0.56.2/zigpy/zcl/clusters/measurement.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/protocol.py` & `zigpy-0.56.2/zigpy/zcl/clusters/protocol.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/security.py` & `zigpy-0.56.2/zigpy/zcl/clusters/security.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,15 +495,15 @@
         cluster_revision: Final = foundation.ZCL_CLUSTER_REVISION_ATTR
         reporting_status: Final = foundation.ZCL_REPORTING_STATUS_ATTR
 
     class ServerCommandDefs(BaseCommandDefs):
         start_warning: Final = ZCLCommandDef(
             id=0x00,
             schema={
-                "warning": Warning,
+                "warning": WarningType,
                 "warning_duration": t.uint16_t,
                 "strobe_duty_cycle": t.uint8_t,
                 "stobe_level": StrobeLevel,
             },
             direction=False,
         )
         squawk: Final = ZCLCommandDef(
```

### Comparing `zigpy-0.56.1/zigpy/zcl/clusters/smartenergy.py` & `zigpy-0.56.2/zigpy/zcl/clusters/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zcl/foundation.py` & `zigpy-0.56.2/zigpy/zcl/foundation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zdo/__init__.py` & `zigpy-0.56.2/zigpy/zdo/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy/zdo/types.py` & `zigpy-0.56.2/zigpy/zdo/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.1/zigpy.egg-info/PKG-INFO` & `zigpy-0.56.2/zigpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.56.1
-Summary: Library implementing a ZigBee stack
-Home-page: https://github.com/zigpy/zigpy
-Author: Russell Cloran
-Author-email: rcloran@gmail.com
+Version: 0.56.2
+Summary: Library implementing a Zigbee stack
+Author-email: Russell Cloran <rcloran@gmail.com>
 License: GPL-3.0
-Platform: UNKNOWN
+Project-URL: repository, https://github.com/zigpy/zigpy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: testing
 License-File: LICENSE
 License-File: COPYING
 
 # zigpy
 
 [![Build](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)](https://github.com/zigpy/zigpy/workflows/CI/badge.svg?branch=dev)
 [![Coverage Status](https://codecov.io/gh/zigpy/zigpy/branch/dev/graph/badge.svg)](https://codecov.io/gh/zigpy/zigpy)
@@ -75,9 +74,7 @@
 - https://pypi.org/project/zigpy/
   - https://pypi.org/project/bellows/
   - https://pypi.org/project/zigpy-cc/
   - https://pypi.org/project/zigpy-deconz/
   - https://pypi.org/project/zigpy-xbee/
   - https://pypi.org/project/zigpy-zigate/
   - https://pypi.org/project/zigpy-znp/
-
-
```

### Comparing `zigpy-0.56.1/zigpy.egg-info/SOURCES.txt` & `zigpy-0.56.2/zigpy.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,39 @@
 COPYING
 LICENSE
 README.md
-setup.cfg
+pyproject.toml
 setup.py
+tests/test_app_state.py
+tests/test_appdb.py
+tests/test_appdb_migration.py
+tests/test_appdb_pysqlite.py
+tests/test_application.py
+tests/test_backups.py
+tests/test_config.py
+tests/test_device.py
+tests/test_endpoint.py
+tests/test_group.py
+tests/test_listeners.py
+tests/test_ota.py
+tests/test_ota_image.py
+tests/test_ota_provider.py
+tests/test_ota_validators.py
+tests/test_quirks.py
+tests/test_quirks_registry.py
+tests/test_serial.py
+tests/test_struct.py
+tests/test_topology.py
+tests/test_types.py
+tests/test_zcl.py
+tests/test_zcl_clusters.py
+tests/test_zcl_foundation.py
+tests/test_zdo.py
+tests/test_zdo_types.py
+tests/test_zigbee_util.py
 zigpy/__init__.py
 zigpy/appdb.py
 zigpy/application.py
 zigpy/backups.py
 zigpy/const.py
 zigpy/device.py
 zigpy/endpoint.py
```

