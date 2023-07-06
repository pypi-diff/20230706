# Comparing `tmp/ovsdbapp-2.3.0.tar.gz` & `tmp/ovsdbapp-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovsdbapp-2.3.0.tar", last modified: Thu Apr 27 15:14:39 2023, max compression
+gzip compressed data, was "ovsdbapp-2.4.0.tar", last modified: Thu Jul  6 08:47:18 2023, max compression
```

## Comparing `ovsdbapp-2.3.0.tar` & `ovsdbapp-2.4.0.tar`

### file list

```diff
@@ -1,194 +1,194 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.963996 ovsdbapp-2.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3072 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16765 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2023-04-27 15:14:39.963996 ovsdbapp-2.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2042 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/TESTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.939996 ovsdbapp-2.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.939996 ovsdbapp-2.3.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2670 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.939996 ovsdbapp-2.3.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.939996 ovsdbapp-2.3.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.939996 ovsdbapp-2.3.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.939996 ovsdbapp-2.3.0/ovsdbapp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/CHANGES
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.943996 ovsdbapp-2.3.0/ovsdbapp/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.943996 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9342 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14070 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/command.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.943996 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8119 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16687 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/idlutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.943996 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/rowview.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5256 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/transaction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/vlog.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.943996 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/windows/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6596 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.943996 ovsdbapp-2.3.0/ovsdbapp/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.947996 ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7885 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9755 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.947996 ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8593 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13455 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5614 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.947996 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.947996 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56958 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70612 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17281 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4464 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/hardware_vtep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/hardware_vtep/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15347 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.951996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.955996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.955996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105891 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.955996 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6575 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.955996 ovsdbapp-2.3.0/ovsdbapp/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.955996 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.955996 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.955996 ovsdbapp-2.3.0/ovsdbapp/tests/unit/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/schema/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.959996 ovsdbapp-2.3.0/ovsdbapp/tests/unit/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3026 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/test_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11660 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/ovsdbapp/venv.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.943996 ovsdbapp-2.3.0/ovsdbapp.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ovsdbapp.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5879 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ovsdbapp.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ovsdbapp.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ovsdbapp.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ovsdbapp.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ovsdbapp.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-04-27 15:14:39.000000 ovsdbapp-2.3.0/ovsdbapp.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.935996 ovsdbapp-2.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.959996 ovsdbapp-2.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/configure-ovsdb-manager-a29a148b241a125e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/drop-py27-support-c426980520444bfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/drop-python-3-6-and-3-7-8ae8ccf16e422fc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/ovn-support-allow-stateless-01aed5acdcd1c0d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/ovn-support-discard-nexthop-cdb1d35aceaf4b63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/ovn-support-hw-vtep-ca8b3ee7a74df3fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/ovn-support-ic-northbound-df557a866a1f411f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/provide-address-set-api-3cb387b9e571d4ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/provide-lb-hc-api-8ff13ccaf75f1eee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/provide-lrp-gateway-chassis-api-14e2948183f60cfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/provide-lrp-get-method-a33a99a7f86b827e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/notes/provide-lrp-networks-modifying-1af13589064c12c6.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.963996 ovsdbapp-2.3.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.963996 ovsdbapp-2.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7768 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2023-04-27 15:14:39.963996 ovsdbapp-2.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.963996 ovsdbapp-2.3.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1863 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1774 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/tools/debug_venv
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1735 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/tools/debug_venv.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      509 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/tools/setup-ovs.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2603 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-04-27 15:14:39.963996 ovsdbapp-2.3.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/zuul.d/ovsdbapp-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-04-27 15:14:09.000000 ovsdbapp-2.3.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3072 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3391 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16863 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2042 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/TESTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.663144 ovsdbapp-2.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.663144 ovsdbapp-2.4.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2670 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.663144 ovsdbapp-2.4.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.663144 ovsdbapp-2.4.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.663144 ovsdbapp-2.4.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/CHANGES
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9342 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14070 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/command.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8119 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16687 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/idlutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/rowview.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5256 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/transaction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/vlog.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/windows/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6596 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7885 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9755 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8593 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13455 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5614 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57192 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70758 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17299 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4464 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1668 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/hardware_vtep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/hardware_vtep/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15347 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.671144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   106126 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6575 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/unit/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/schema/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.675144 ovsdbapp-2.4.0/ovsdbapp/tests/unit/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3026 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11660 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/ovsdbapp/venv.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.667144 ovsdbapp-2.4.0/ovsdbapp.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ovsdbapp.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5879 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ovsdbapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ovsdbapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ovsdbapp.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ovsdbapp.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ovsdbapp.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-07-06 08:47:18.000000 ovsdbapp-2.4.0/ovsdbapp.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.663144 ovsdbapp-2.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/configure-ovsdb-manager-a29a148b241a125e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/drop-py27-support-c426980520444bfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/drop-python-3-6-and-3-7-8ae8ccf16e422fc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/ovn-support-allow-stateless-01aed5acdcd1c0d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/ovn-support-discard-nexthop-cdb1d35aceaf4b63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/ovn-support-hw-vtep-ca8b3ee7a74df3fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/ovn-support-ic-northbound-df557a866a1f411f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/provide-address-set-api-3cb387b9e571d4ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/provide-lb-hc-api-8ff13ccaf75f1eee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/provide-lrp-gateway-chassis-api-14e2948183f60cfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/provide-lrp-get-method-a33a99a7f86b827e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/notes/provide-lrp-networks-modifying-1af13589064c12c6.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7768 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      688 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1863 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1774 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/tools/debug_venv
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1735 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/tools/debug_venv.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      509 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/tools/setup-ovs.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2603 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:47:18.679144 ovsdbapp-2.4.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/zuul.d/ovsdbapp-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2023-07-06 08:46:52.000000 ovsdbapp-2.4.0/zuul.d/project.yaml
```

### Comparing `ovsdbapp-2.3.0/.pylintrc` & `ovsdbapp-2.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/AUTHORS` & `ovsdbapp-2.4.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/CONTRIBUTING.rst` & `ovsdbapp-2.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ChangeLog` & `ovsdbapp-2.4.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+2.4.0
+-----
+
+* Ensure LrpAddCommand may\_exits works without peers
+* Add support for ecmp routes
+
 2.3.0
 -----
 
 * Add support for manipulating BFD entries
 * Add if\_exists and \*\*kwargs columns to db\_set
 * Add 'no timeout' option to wait\_for\_change
 * Add Interface paramteres to \`\`OvsdbIdl.add\_port\`\` method
```

### Comparing `ovsdbapp-2.3.0/LICENSE` & `ovsdbapp-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/PKG-INFO` & `ovsdbapp-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovsdbapp
-Version: 2.3.0
+Version: 2.4.0
 Summary: A library for creating OVSDB applications
 Home-page: https://pypi.org/project/ovsdbapp/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         ovsdbapp
```

### Comparing `ovsdbapp-2.3.0/README.rst` & `ovsdbapp-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/TESTING.rst` & `ovsdbapp-2.4.0/TESTING.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/doc/source/conf.py` & `ovsdbapp-2.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/__init__.py` & `ovsdbapp-2.4.0/ovsdbapp/__init__.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/api.py` & `ovsdbapp-2.4.0/ovsdbapp/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/__init__.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/__init__.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/command.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/command.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/connection.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/event.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/fixtures.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/idlutils.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/idlutils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/rowview.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/rowview.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/transaction.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/transaction.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/vlog.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/vlog.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/backend/ovs_idl/windows/utils.py` & `ovsdbapp-2.4.0/ovsdbapp/backend/ovs_idl/windows/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/constants.py` & `ovsdbapp-2.4.0/ovsdbapp/constants.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/event.py` & `ovsdbapp-2.4.0/ovsdbapp/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/exceptions.py` & `ovsdbapp-2.4.0/ovsdbapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/api.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/commands.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/hardware_vtep/impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/hardware_vtep/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/api.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/commands.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/helpers.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/helpers.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/open_vswitch/impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/open_vswitch/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/api.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/commands.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/api.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -731,15 +731,15 @@
         :param if_exists: If True, don't fail if the networks doesn't exist
         :type if_exists:  boolean
         :returns:         :class:`Command` with no result
         """
 
     @abc.abstractmethod
     def lr_route_add(self, router, prefix, nexthop, port=None,
-                     policy='dst-ip', may_exist=False):
+                     policy='dst-ip', may_exist=False, ecmp=False):
         """Add a route to 'router'
 
         :param router:    The name or uuid of the router
         :type router:     string or uuid.UUID
         :param prefix:    an IPv4/6 prefix for this route, e.g. 192.168.1.0/24
         :type prefix:     type string
         :parm nexthop:    The gateway to use for this route, which should be
@@ -750,14 +750,18 @@
                           sent out this port. Otherwise OVN infers the output
                           port based on nexthop.
         :type port:       string
         :param policy:    the policy used to make routing decisions
         :type policy:     string, 'dst-ip' or 'src-ip'
         :param may_exist: If True, don't fail if the route already exists
         :type may_exist:  boolean
+        :param ecmp:      Enable ECMP support. If True adding routes with
+                          same IP prefix is allowed as long as the nexthop is
+                          different
+        :type ecmp:       boolean
         returns:          :class:`Command` with RowView result
         """
 
     @abc.abstractmethod
     def lr_route_del(self, router, prefix=None, if_exists=False):
         """Remove routes from 'router'
```

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/commands.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,15 +849,15 @@
 class LrpAddCommand(cmd.BaseCommand):
     def __init__(self, api, router, port, mac, networks,
                  peer=None, may_exist=False, **columns):
         self.mac = str(netaddr.EUI(mac, dialect=netaddr.mac_unix_expanded))
         self.networks = [str(netaddr.IPNetwork(net)) for net in networks]
         self.router = router
         self.port = port
-        self.peer = peer
+        self.peer = peer if peer else []
         self.may_exist = may_exist
         self.columns = columns
         super().__init__(api)
 
     def run_idl(self, txn):
         lr = self.api.lookup('Logical_Router', self.router)
         try:
@@ -1135,30 +1135,33 @@
 
 class BFDGetCommand(cmd.BaseGetRowCommand):
     table = 'BFD'
 
 
 class LrRouteAddCommand(cmd.BaseCommand):
     def __init__(self, api, router, prefix, nexthop, port=None,
-                 policy='dst-ip', may_exist=False):
+                 policy='dst-ip', may_exist=False, ecmp=False):
         prefix = str(netaddr.IPNetwork(prefix))
         if nexthop != const.ROUTE_DISCARD:
             nexthop = str(netaddr.IPAddress(nexthop))
         super().__init__(api)
         self.router = router
         self.prefix = prefix
         self.nexthop = nexthop
         self.port = port
         self.policy = policy
+        self.ecmp = ecmp
         self.may_exist = may_exist
 
     def run_idl(self, txn):
         lr = self.api.lookup('Logical_Router', self.router)
         for route in lr.static_routes:
             if self.prefix == route.ip_prefix:
+                if self.ecmp and self.nexthop != route.nexthop:
+                    continue
                 if not self.may_exist:
                     msg = "Route %s already exists on router %s" % (
                         self.prefix, self.router)
                     raise RuntimeError(msg)
                 route.nexthop = self.nexthop
                 route.policy = self.policy
                 if self.port:
```

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_northbound/impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_northbound/impl_idl.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,17 +232,17 @@
     def lrp_add_networks(self, port, networks, may_exist=False):
         return cmd.LrpAddNetworksCommand(self, port, networks, may_exist)
 
     def lrp_del_networks(self, port, networks, if_exists=False):
         return cmd.LrpDelNetworksCommand(self, port, networks, if_exists)
 
     def lr_route_add(self, router, prefix, nexthop, port=None,
-                     policy='dst-ip', may_exist=False):
+                     policy='dst-ip', may_exist=False, ecmp=False):
         return cmd.LrRouteAddCommand(self, router, prefix, nexthop, port,
-                                     policy, may_exist)
+                                     policy, may_exist, ecmp)
 
     def lr_route_del(self, router, prefix=None, if_exists=False):
         return cmd.LrRouteDelCommand(self, router, prefix, if_exists)
 
     def lr_route_list(self, router):
         return cmd.LrRouteListCommand(self, router)
```

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/api.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/commands.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/schema/ovn_southbound/impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/schema/ovn_southbound/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/base.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/base.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/base.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/fixtures.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py`

 * *Files 0% similar despite different names*

```diff
@@ -952,21 +952,21 @@
 
     def test_lr_list(self):
         lrs = {self._lr_add() for _ in range(3)}
         lr_set = set(self.api.lr_list().execute(check_error=True))
         self.assertTrue(lrs.issubset(lr_set), "%s vs %s" % (lrs, lr_set))
 
     def _lr_add_route(self, router=None, prefix=None, nexthop=None, port=None,
-                      **kwargs):
+                      ecmp=False, **kwargs):
         lr = self._lr_add(router or utils.get_rand_device_name(),
                           may_exist=True)
         prefix = prefix or '192.0.2.0/25'
         nexthop = nexthop or '192.0.2.254'
         port = port or "port_name"
-        sr = self.api.lr_route_add(lr.uuid, prefix, nexthop, port,
+        sr = self.api.lr_route_add(lr.uuid, prefix, nexthop, port, ecmp=ecmp,
                                    **kwargs).execute(check_error=True)
         self.assertIn(sr, lr.static_routes)
         self.assertEqual(prefix, sr.ip_prefix)
         self.assertEqual(nexthop, sr.nexthop)
         self.assertIn(port, sr.output_port)
         sr.router = lr
         return sr
@@ -988,14 +988,20 @@
         self.assertRaises(RuntimeError, self._lr_add_route, router=router_name)
 
     def test_lr_route_add_may_exist(self):
         router_name = utils.get_rand_device_name()
         self._lr_add_route(router_name)
         self._lr_add_route(router_name, may_exist=True)
 
+    def test_lr_route_add_exists_ecmp(self):
+        router_name = utils.get_rand_device_name()
+        self._lr_add_route(router_name)
+        self._lr_add_route(router=router_name, nexthop='192.0.3.254',
+                           ecmp=True)
+
     def test_lr_route_add_discard(self):
         self._lr_add_route(nexthop=const.ROUTE_DISCARD)
         self.assertRaises(netaddr.AddrFormatError, self._lr_add_route,
                           prefix='not-discard')
 
     def test_lr_route_del(self):
         prefix = "192.0.2.0/25"
@@ -1374,15 +1380,15 @@
 
     def test_lrp_get_name(self):
         self._test_lrp_get('name')
 
     def test_lrp_add(self):
         self._lrp_add(None, 'de:ad:be:ef:4d:ad', ['192.0.2.0/24'])
 
-    def test_lpr_add_peer(self):
+    def test_lrp_add_peer(self):
         lrp = self._lrp_add(None, 'de:ad:be:ef:4d:ad', ['192.0.2.0/24'],
                             peer='fake_peer')
         self.assertIn('fake_peer', lrp.peer)
 
     def test_lpr_add_multiple_networks(self):
         networks = ['192.0.2.0/24', '192.2.1.0/24']
         self._lrp_add(None, 'de:ad:be:ef:4d:ad', networks)
@@ -1405,15 +1411,15 @@
         self._lrp_add(*args)
         self.assertRaises(RuntimeError, self._lrp_add, *args)
 
     def test_lrp_add_may_exist(self):
         name = utils.get_rand_device_name()
         args = (name, 'de:ad:be:ef:4d:ad', ['192.0.2.0/24'])
         self._lrp_add(*args)
-        self.assertRaises(RuntimeError, self._lrp_add, *args, may_exist=True)
+        self._lrp_add(*args, may_exist=True)
 
     def test_lrp_add_may_exist_different_router(self):
         name = utils.get_rand_device_name()
         args = (name, 'de:ad:be:ef:4d:ad', ['192.0.2.0/24'])
         lr2 = self.useFixture(fixtures.LogicalRouterFixture(self.api)).obj
         self._lrp_add(*args)
         cmd = self.api.lrp_add(lr2.uuid, *args, may_exist=True)
```

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/test_api.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/test_event.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/test_event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/unit/test_utils.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/tests/utils.py` & `ovsdbapp-2.4.0/ovsdbapp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/utils.py` & `ovsdbapp-2.4.0/ovsdbapp/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp/venv.py` & `ovsdbapp-2.4.0/ovsdbapp/venv.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/ovsdbapp.egg-info/PKG-INFO` & `ovsdbapp-2.4.0/ovsdbapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovsdbapp
-Version: 2.3.0
+Version: 2.4.0
 Summary: A library for creating OVSDB applications
 Home-page: https://pypi.org/project/ovsdbapp/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         ovsdbapp
```

### Comparing `ovsdbapp-2.3.0/ovsdbapp.egg-info/SOURCES.txt` & `ovsdbapp-2.4.0/ovsdbapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/releasenotes/source/conf.py` & `ovsdbapp-2.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/requirements.txt` & `ovsdbapp-2.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/setup.cfg` & `ovsdbapp-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/setup.py` & `ovsdbapp-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/tools/coding-checks.sh` & `ovsdbapp-2.4.0/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/tools/debug_venv` & `ovsdbapp-2.4.0/tools/debug_venv`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/tools/debug_venv.py` & `ovsdbapp-2.4.0/tools/debug_venv.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.3.0/tox.ini` & `ovsdbapp-2.4.0/tox.ini`

 * *Files identical despite different names*

