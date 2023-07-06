# Comparing `tmp/python-ironicclient-5.2.0.tar.gz` & `tmp/python-ironicclient-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ironicclient-5.2.0.tar", last modified: Thu May 11 09:01:50 2023, max compression
+gzip compressed data, was "python-ironicclient-5.3.0.tar", last modified: Thu Jul  6 08:58:15 2023, max compression
```

## Comparing `python-ironicclient-5.2.0.tar` & `python-ironicclient-5.3.0.tar`

### file list

```diff
@@ -1,360 +1,362 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7126 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40110 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2592 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/api_v1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/doc/source/cli/osc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/cli/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/osc/v1/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/osc_plugin_cli.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/cli/standalone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/contributor/testing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/doc/source/user/create_command.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6037 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/apiclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13414 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13786 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/filecache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19500 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16410 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/exc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5009 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14167 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_chassis.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5486 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12397 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9423 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_driver.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    79576 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19378 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17413 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15268 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8613 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.070241 python-ironicclient-5.2.0/ironicclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18361 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8146 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3308 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4970 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7181 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5355 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8411 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_filecache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24336 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17668 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.074241 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7293 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/test_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.078241 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10097 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23761 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17983 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9451 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16550 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20048 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   140580 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29204 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28663 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31976 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38280 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11630 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/test_exc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/test_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.078241 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11950 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14520 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6549 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22786 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_create_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8960 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74840 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11355 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13737 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_resource_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10998 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_target.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.082241 python-ironicclient-5.2.0/ironicclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8839 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/allocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8245 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/chassis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5710 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13649 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/create_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/deploy_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50734 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/port.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/portgroup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17139 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/resource_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/volume_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/ironicclient/v1/volume_target.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.082241 python-ironicclient-5.2.0/playbooks/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/playbooks/functional/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.082241 python-ironicclient-5.2.0/python_ironicclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16585 2023-05-11 09:01:50.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8739 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-05-11 09:01:49.000000 python-ironicclient-5.2.0/python_ironicclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.066241 python-ironicclient-5.2.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/SHA1-hash-auth-token-f8dce46f854c002c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-allocation-owner-0c6daad4ebfea5e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-bios-registry-in-list-21974873f146aff7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-chassis_uuid-removal-possibility-5bc0bc3a7953eaa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-conductor-cli-233249ebc9d5a5f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-driver-cli-fields-selector-b0f527eb5f6fb2a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-environment-variable-to-specify-version-cache-timeout-dfa5f6d4af0ea1d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-events-support-53c461d28abf010b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-is-smartnic-port-attr-ed46d887aec276ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-json-option-0cf29be2a97e0212.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-network-data-node-attr-81dec9cecb7491b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-neutron-integration-fields-cee7596c49722de6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-no-retired-opt-403bb5e466e4facb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-boot-mode-08ac768649a2fc93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-boot-mode-set-9746b45aa3f80fe8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-description-support-6efd0882eaa0c788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-history-b9b9beeb0200f185.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-lessee-c36409eb0415f75d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-owner-c2dce5a6075ce2b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-node-resource-class-6040d1d6c734522c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-portgroups-to-create-command-6d685277f7af79df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-rescue-interface-to-node-and-driver-e3ff9b5df2628e5a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-rescue-unrescue-support-f78266514ca59346.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-vif-attach-detach-support-e680d64e4add0fa4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add_api_versions-a59e5b6899833c33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add_automated_clean_field-d2a0c824a4e90bf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/add_retired_field-6ec9f97c7c2f86ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/address-cross-distro-iso-tools-006711c9f150037a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allocation-api-5f13082a8b36d788.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allocation-backfill-4d4e51af2f787a72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allow-allocation-update-b4fb715045ab40a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/allow-client-to-request-list-of-versions-88f019cad76e6464.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-adds-node-create-args-a7ace744515e5943.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-update-baremetal-node-set-c1ac57de0d481efe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1712935-allow-os_baremetal_api_version_env_var_to_be_latest-28c8eed24f389673.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1724974-add-wanboot-to-supported-boot-devices.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/bug-1745099-allow-integer-portgroup-mode-6be4d3b35e216486.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/client-session-09e6ced1fbc6a9b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/conductor-group-9cfab3756aa108e4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/configdrive-7bd2b67830691b2e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/configdrive-json-b9d173dde111cf22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/continue-del-next-node-8827e67e1c41a0a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/debug-e9dd680d783fa4b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/deploy-templates-df354ce825b00430.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/deprecate-ironic-cli-686b7a238ddf3e25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/display-empty-string-for-chassis-uuid-if-it-is-empty-a5471c3aa740a27d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/driver-properties-for-osc-07a99d2d4e166436.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/drop-py-2-7-b0b950c0c2b6a667.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/endpoint-plus-version-4248f4f229dbc7dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/endpoint-strip-dea59ccb05628a35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/extend-vif-attach-commands-ef3a931413ddcee7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/feature-parity-osc-cli-7606eed15f1c124f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-negotiate-version-503-c3cb8d1d4901541a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-owner-feature-2f3f0163ff307727.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-python3-compatibility-993ace45fefcba34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/fix-token-with-vhosts-5d0a6d53e807fa5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/implicit-version-warning-d34b99727b50d519.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/implicit-version-warning-old-cli-fe34d423ae63544a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/index-error-no-endpoint-eb281187f80a9aa4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/instance-crash-dump-d845a31e72b5a9f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/ironic-create-files-fix-c31e40e566ff86b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/json-bytes-2f0085202d5e5796.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/keystone-token-auth-661a0c0d53c1b4de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/latest-baremetal-api-version-a20e3099e3b97a1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/latest-renegotiation-55daa01b3fc261be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/list-nodes-by-driver-b1e1e1018077089b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/logging-9c452e4869d80de9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/missing-session-cc11e62dc966b4e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/multinode-actions-9f682ad5172f032f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/negative-wrap-fix-4197e91b2ecfb722.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/network_data-c48b3878a5b04df5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/node-fault-adbe74fd600063ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/not-ignore-delete-failtures-0783d33a606ed6f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-baremetal-driver-raid-properties-159bd57058c0fc0e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-default-microver-172d6e69316e70c1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-instance-crash-dump-22634a57104561a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-max-microver-22-dc0d91a62f03a2e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-chassis-091d080684cdccf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-no-maintenance-ff1cef7cfbe60fb9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-option-driver-a2901ba6b4e1d3b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-provisionstate-cd98dbddaad93e96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-list-unassociated-60e46958a0abc3e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-power-on-off-c269980e3b9c79ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-rebuild-configdrive-8979d5b1373e8d5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-node-set-chassis-aae3413489b66b9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-9b5344aceb886cc1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-chassis-create-show-fix-ee276d707c5a5bdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-node-create-show-fix-283148c86fbccce2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-node-set-target-raid-config-5d538d6253902ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-set-unset-target-raid-config-9a1cecb5620eafda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-port-create-uuid-5da551b154540ef7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-soft-reboot-poweroff-121b8043567f54a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-versioned-endpoint-fix-08f6b7af2f47a5d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/osc-wait-option-for-provisioning-commands-b6f5b875d573c9c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/oslo-i18n-optional-ff28821441a0807c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/oslo.config-f67bf37ea35dd7fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/pass-interface-argument-deb92e3feb0bf051.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/port-physical-network-6ea8860d773e473c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/protected-72d7419245a4f6c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/provision-state-adopt-d07b838813cecfb1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/provision-state-wait-e7ff919ce8e13703.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/raid_CLI_support-7e816ccd0fb31d2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-endpoint-argument-fc0bd8099067e4ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-http-client-c969f583573251e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-keystone-args-925ac5f3607a89a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-ironic-command-5c9f7bc4946996e0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-llc-short-arg-89c7443acc6c54a4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/remove-states-field-0242960d121a09a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/reset-interface-bbd7a612242db399.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/reset-interfaces-bec227bf933fea59.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/retry-on-keystone-auth-retriable-failures-91c08b9f8bdab7f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/session-client-endpoint-override-20f1d822b4430afa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/session-create-092172964afdb71b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/show-required-arguments-in-help-commands-of-node-create-port-create-b213bb28bcc94743.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/soft-reboot-poweroff-e33d078a05db3894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/standalone-cli-f07834585909334a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/start-using-reno-ccd220efa2c7022a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/strip-prefix-when-paginating-6140465b1488828e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/switch-requests-8304d4465a8976b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/typerror-132801fe4541fdb4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/2023.1.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9019 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9750 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tools/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6953 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2737 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:01:50.098241 python-ironicclient-5.2.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/zuul.d/ironicclient-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-05-11 09:01:24.000000 python-ironicclient-5.2.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.039600 python-ironicclient-5.3.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7162 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40233 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-07-06 08:58:15.039600 python-ironicclient-5.3.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2592 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.999600 python-ironicclient-5.3.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.999600 python-ironicclient-5.3.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3380 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/api_v1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.999600 python-ironicclient-5.3.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/cli/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.995599 python-ironicclient-5.3.0/doc/source/cli/osc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.999600 python-ironicclient-5.3.0/doc/source/cli/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1096 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/cli/osc/v1/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/cli/osc_plugin_cli.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/cli/standalone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.999600 python-ironicclient-5.3.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1519 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/contributor/testing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.999600 python-ironicclient-5.3.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.999600 python-ironicclient-5.3.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/doc/source/user/create_command.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6037 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16928 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/apiclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13414 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13786 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3324 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/filecache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19500 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16410 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/exc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5009 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14167 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11134 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_chassis.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5486 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1398 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12397 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9423 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_driver.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    81857 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19378 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17413 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15268 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_volume_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8613 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17958 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.003600 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.007599 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18361 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8146 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3308 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7239 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1364 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9457 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4970 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3438 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3877 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5116 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.007599 python-ironicclient-5.3.0/ironicclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.007599 python-ironicclient-5.3.0/ironicclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.007599 python-ironicclient-5.3.0/ironicclient/tests/unit/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7181 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/apiclient/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5355 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9677 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8411 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_filecache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24336 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17668 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.011599 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7293 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/test_plugin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.011599 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10671 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23761 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17983 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9451 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1739 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16550 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20048 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   145108 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29204 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28663 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31976 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38280 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11630 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/test_exc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1393 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/test_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5060 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.015599 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11950 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14520 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6549 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22786 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_create_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9684 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8960 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76642 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11355 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13737 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_resource_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11601 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10998 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.015599 python-ironicclient-5.3.0/ironicclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8839 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/allocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8245 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/chassis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5710 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3713 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13649 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/create_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4538 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/deploy_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52074 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5979 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/port.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/portgroup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17139 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/resource_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4938 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/volume_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/ironicclient/v1/volume_target.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.995599 python-ironicclient-5.3.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.015599 python-ironicclient-5.3.0/playbooks/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/playbooks/functional/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.015599 python-ironicclient-5.3.0/python_ironicclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4232 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16705 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8824 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-07-06 08:58:14.000000 python-ironicclient-5.3.0/python_ironicclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:14.995599 python-ironicclient-5.3.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.035599 python-ironicclient-5.3.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/SHA1-hash-auth-token-f8dce46f854c002c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-allocation-owner-0c6daad4ebfea5e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-bios-registry-in-list-21974873f146aff7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-chassis_uuid-removal-possibility-5bc0bc3a7953eaa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-conductor-cli-233249ebc9d5a5f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-driver-cli-fields-selector-b0f527eb5f6fb2a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-environment-variable-to-specify-version-cache-timeout-dfa5f6d4af0ea1d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-events-support-53c461d28abf010b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-is-smartnic-port-attr-ed46d887aec276ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-json-option-0cf29be2a97e0212.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-network-data-node-attr-81dec9cecb7491b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-neutron-integration-fields-cee7596c49722de6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-no-retired-opt-403bb5e466e4facb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-boot-mode-08ac768649a2fc93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-boot-mode-set-9746b45aa3f80fe8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-description-support-6efd0882eaa0c788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-history-b9b9beeb0200f185.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-inventory-74e856c019cfa7e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-lessee-c36409eb0415f75d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-owner-c2dce5a6075ce2b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-node-resource-class-6040d1d6c734522c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-portgroups-to-create-command-6d685277f7af79df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-rescue-interface-to-node-and-driver-e3ff9b5df2628e5a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-rescue-unrescue-support-f78266514ca59346.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-vif-attach-detach-support-e680d64e4add0fa4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      710 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add_api_versions-a59e5b6899833c33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add_automated_clean_field-d2a0c824a4e90bf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/add_retired_field-6ec9f97c7c2f86ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/address-cross-distro-iso-tools-006711c9f150037a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/allocation-api-5f13082a8b36d788.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/allocation-backfill-4d4e51af2f787a72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/allow-allocation-update-b4fb715045ab40a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/allow-client-to-request-list-of-versions-88f019cad76e6464.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/bug-1524745-adds-node-create-args-a7ace744515e5943.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/bug-1524745-update-baremetal-node-set-c1ac57de0d481efe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/bug-1712935-allow-os_baremetal_api_version_env_var_to_be_latest-28c8eed24f389673.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/bug-1724974-add-wanboot-to-supported-boot-devices.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/bug-1745099-allow-integer-portgroup-mode-6be4d3b35e216486.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/client-session-09e6ced1fbc6a9b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/conductor-group-9cfab3756aa108e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/configdrive-7bd2b67830691b2e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/configdrive-json-b9d173dde111cf22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/continue-del-next-node-8827e67e1c41a0a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/debug-e9dd680d783fa4b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/deploy-templates-df354ce825b00430.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2705 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/deprecate-ironic-cli-686b7a238ddf3e25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/display-empty-string-for-chassis-uuid-if-it-is-empty-a5471c3aa740a27d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/driver-properties-for-osc-07a99d2d4e166436.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/drop-py-2-7-b0b950c0c2b6a667.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/endpoint-plus-version-4248f4f229dbc7dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/endpoint-strip-dea59ccb05628a35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/extend-vif-attach-commands-ef3a931413ddcee7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/feature-parity-osc-cli-7606eed15f1c124f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/fix-negotiate-version-503-c3cb8d1d4901541a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/fix-owner-feature-2f3f0163ff307727.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/fix-python3-compatibility-993ace45fefcba34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/fix-token-with-vhosts-5d0a6d53e807fa5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/implicit-version-warning-d34b99727b50d519.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/implicit-version-warning-old-cli-fe34d423ae63544a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/index-error-no-endpoint-eb281187f80a9aa4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/instance-crash-dump-d845a31e72b5a9f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/ironic-create-files-fix-c31e40e566ff86b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/json-bytes-2f0085202d5e5796.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/keystone-token-auth-661a0c0d53c1b4de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/latest-baremetal-api-version-a20e3099e3b97a1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1270 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/latest-renegotiation-55daa01b3fc261be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/list-nodes-by-driver-b1e1e1018077089b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/logging-9c452e4869d80de9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/missing-session-cc11e62dc966b4e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/multinode-actions-9f682ad5172f032f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/negative-wrap-fix-4197e91b2ecfb722.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/network_data-c48b3878a5b04df5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/node-fault-adbe74fd600063ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/node-shard-support-774ebfe6719fc7c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/not-ignore-delete-failtures-0783d33a606ed6f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-baremetal-driver-raid-properties-159bd57058c0fc0e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-default-microver-172d6e69316e70c1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-instance-crash-dump-22634a57104561a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-max-microver-22-dc0d91a62f03a2e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-list-chassis-091d080684cdccf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-list-no-maintenance-ff1cef7cfbe60fb9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-list-option-driver-a2901ba6b4e1d3b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-list-provisionstate-cd98dbddaad93e96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-list-unassociated-60e46958a0abc3e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-power-on-off-c269980e3b9c79ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-rebuild-configdrive-8979d5b1373e8d5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-node-set-chassis-aae3413489b66b9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-9b5344aceb886cc1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-chassis-create-show-fix-ee276d707c5a5bdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-node-create-show-fix-283148c86fbccce2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-node-set-target-raid-config-5d538d6253902ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-set-unset-target-raid-config-9a1cecb5620eafda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-port-create-uuid-5da551b154540ef7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-soft-reboot-poweroff-121b8043567f54a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-versioned-endpoint-fix-08f6b7af2f47a5d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/osc-wait-option-for-provisioning-commands-b6f5b875d573c9c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/oslo-i18n-optional-ff28821441a0807c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/oslo.config-f67bf37ea35dd7fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/pass-interface-argument-deb92e3feb0bf051.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/port-physical-network-6ea8860d773e473c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/protected-72d7419245a4f6c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/provision-state-adopt-d07b838813cecfb1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/provision-state-wait-e7ff919ce8e13703.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/raid_CLI_support-7e816ccd0fb31d2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/remove-deprecated-endpoint-argument-fc0bd8099067e4ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/remove-deprecated-http-client-c969f583573251e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/remove-deprecated-keystone-args-925ac5f3607a89a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/remove-ironic-command-5c9f7bc4946996e0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/remove-llc-short-arg-89c7443acc6c54a4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/remove-states-field-0242960d121a09a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/reset-interface-bbd7a612242db399.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/reset-interfaces-bec227bf933fea59.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/retry-on-keystone-auth-retriable-failures-91c08b9f8bdab7f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/session-client-endpoint-override-20f1d822b4430afa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/session-create-092172964afdb71b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/show-required-arguments-in-help-commands-of-node-create-port-create-b213bb28bcc94743.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/soft-reboot-poweroff-e33d078a05db3894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/standalone-cli-f07834585909334a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/start-using-reno-ccd220efa2c7022a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/strip-prefix-when-paginating-6140465b1488828e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/switch-requests-8304d4465a8976b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      668 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/typerror-132801fe4541fdb4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/version-overrides-4e9ba1266a238c6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/vif-attach-port-29a421b245e19f2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/wait-for-prov-last-error-5f49b1c488879775.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/notes/yaml-files-79cd8367d7a4c2f2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.039600 python-ironicclient-5.3.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.039600 python-ironicclient-5.3.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.039600 python-ironicclient-5.3.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9019 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9836 2023-07-06 08:58:15.043599 python-ironicclient-5.3.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.039600 python-ironicclient-5.3.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/tools/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6953 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2737 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:58:15.039600 python-ironicclient-5.3.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/zuul.d/ironicclient-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-07-06 08:56:12.000000 python-ironicclient-5.3.0/zuul.d/project.yaml
```

### Comparing `python-ironicclient-5.2.0/AUTHORS` & `python-ironicclient-5.3.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 LiuNanke <nanke.liu@easystack.cn>
 Lokesh S <lokesh.s@hp.com>
 Lucas Alvares Gomes <lucasagomes@gmail.com>
 Luong Anh Tuan <tuanla@vn.fujitsu.com>
 M V P Nitesh <m.nitesh@nectechnologies.in>
 Madhuri Kumari <madhuri.kumari@intel.com>
 Mahnoor Asghar <masghar.bese15seecs@seecs.edu.pk>
+Mahnoor Asghar <masghar@redhat.com>
 Marc Aubry <maubry@internap.com>
 Mario Villaplana <mario.villaplana@gmail.com>
 Mark Goddard <mark@stackhpc.com>
 Martin Geisler <martin@geisler.net>
 Mathieu Gagné <mgagne@iweb.com>
 Matt Keenan <matt.keenan@gmail.com>
 Maxime Belanger <mbelanger@iweb.com>
```

### Comparing `python-ironicclient-5.2.0/ChangeLog` & `python-ironicclient-5.3.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+5.3.0
+-----
+
+* Node sharding support
+* Add support for node inventory
+* Fix minor spelling errors and incorrect help text
+
 5.2.0
 -----
 
 * Update dependencies for pep8: to hacking v6
 * Accept configdrive as a JSON file
 * Update master for stable/2023.1
 * Allow several nodes for most node actions
```

### Comparing `python-ironicclient-5.2.0/LICENSE` & `python-ironicclient-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/PKG-INFO` & `python-ironicclient-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ironicclient
-Version: 5.2.0
+Version: 5.3.0
 Summary: OpenStack Bare Metal Provisioning API Client Library
 Home-page: https://docs.openstack.org/python-ironicclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================================
         Python bindings for the Ironic API
```

### Comparing `python-ironicclient-5.2.0/README.rst` & `python-ironicclient-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/api_v1.rst` & `python-ironicclient-5.3.0/doc/source/api_v1.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/cli/osc/v1/index.rst` & `python-ironicclient-5.3.0/doc/source/cli/osc/v1/index.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/cli/osc_plugin_cli.rst` & `python-ironicclient-5.3.0/doc/source/cli/osc_plugin_cli.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/cli/standalone.rst` & `python-ironicclient-5.3.0/doc/source/cli/standalone.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/conf.py` & `python-ironicclient-5.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/contributor/contributing.rst` & `python-ironicclient-5.3.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/contributor/testing.rst` & `python-ironicclient-5.3.0/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/index.rst` & `python-ironicclient-5.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/doc/source/user/create_command.rst` & `python-ironicclient-5.3.0/doc/source/user/create_command.rst`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/__init__.py` & `python-ironicclient-5.3.0/ironicclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/client.py` & `python-ironicclient-5.3.0/ironicclient/client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/common/apiclient/base.py` & `python-ironicclient-5.3.0/ironicclient/common/apiclient/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/common/apiclient/exceptions.py` & `python-ironicclient-5.3.0/ironicclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/common/base.py` & `python-ironicclient-5.3.0/ironicclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/common/filecache.py` & `python-ironicclient-5.3.0/ironicclient/common/filecache.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/common/http.py` & `python-ironicclient-5.3.0/ironicclient/common/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 # NOTE(deva): Record the latest version that this client was tested with.
 #             We still have a lot of work to do in the client to implement
 #             microversion support in the client properly! See
 #             http://specs.openstack.org/openstack/ironic-specs/specs/kilo/api-microversions.html # noqa
 #             for full details.
 DEFAULT_VER = '1.9'
-LAST_KNOWN_API_VERSION = 78
+LAST_KNOWN_API_VERSION = 82
 LATEST_VERSION = '1.{}'.format(LAST_KNOWN_API_VERSION)
 
 LOG = logging.getLogger(__name__)
 USER_AGENT = 'python-ironicclient'
 CHUNKSIZE = 1024 * 64  # 64kB
 
 _MAJOR_VERSION = 1
```

### Comparing `python-ironicclient-5.2.0/ironicclient/common/i18n.py` & `python-ironicclient-5.3.0/ironicclient/common/i18n.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/common/utils.py` & `python-ironicclient-5.3.0/ironicclient/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/exc.py` & `python-ironicclient-5.3.0/ironicclient/exc.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/plugin.py` & `python-ironicclient-5.3.0/ironicclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_allocation.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_chassis.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_conductor.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_create.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_deploy_template.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_driver.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_node.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #   under the License.
 #
 
 import argparse
 import itertools
 import json
 import logging
+import sys
 
 from osc_lib.command import command
 from osc_lib import utils as oscutils
 
 from ironicclient.common.i18n import _
 from ironicclient.common import utils
 from ironicclient import exc
@@ -518,27 +519,32 @@
             '--lessee',
             metavar='<lessee>',
             help=_('Lessee of the node.'))
         parser.add_argument(
             '--description',
             metavar='<description>',
             help=_("Description for the node."))
+        parser.add_argument(
+            '--shard',
+            metavar='<shard>',
+            help=_("Shard for the node."))
 
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
 
         field_list = ['automated_clean', 'chassis_uuid', 'driver',
                       'driver_info', 'properties', 'extra', 'uuid', 'name',
                       'conductor_group', 'owner', 'description', 'lessee',
-                      'resource_class'] + ['%s_interface' % iface
-                                           for iface in SUPPORTED_INTERFACES]
+                      'shard', 'resource_class'
+                      ] + ['%s_interface' % iface
+                           for iface in SUPPORTED_INTERFACES]
         fields = dict((k, v) for (k, v) in vars(parsed_args).items()
                       if k in field_list and not (v is None))
         fields = utils.args_array_to_dict(fields, 'driver_info')
         fields = utils.args_array_to_dict(fields, 'extra')
         if parsed_args.network_data:
             fields['network_data'] = utils.handle_json_arg(
                 parsed_args.network_data, 'static network configuration')
@@ -743,14 +749,32 @@
             help=_("Limit list to nodes with lessee "
                    "<lessee>"))
         parser.add_argument(
             '--description-contains',
             metavar='<description_contains>',
             help=_("Limit list to nodes with description contains "
                    "<description_contains>"))
+        sharded_group = parser.add_mutually_exclusive_group(required=False)
+        sharded_group.add_argument(
+            '--sharded',
+            dest='sharded',
+            help=_("List only nodes that are sharded."),
+            default=None,
+            action='store_true')
+        sharded_group.add_argument(
+            '--unsharded',
+            dest='sharded',
+            help=_("List only nodes that are not sharded."),
+            default=None,
+            action='store_false')
+        parser.add_argument(
+            '--shards',
+            nargs='+',
+            metavar='<shards>',
+            help=_("List only nodes that are in shards <shards>."))
         display_group = parser.add_mutually_exclusive_group(required=False)
         display_group.add_argument(
             '--long',
             default=False,
             help=_("Show detailed information about the nodes."),
             action='store_true')
         display_group.add_argument(
@@ -780,20 +804,22 @@
                 parsed_args.limit)
         params['limit'] = parsed_args.limit
         params['marker'] = parsed_args.marker
         if parsed_args.associated:
             params['associated'] = True
         if parsed_args.unassociated:
             params['associated'] = False
-        for field in ['maintenance', 'fault', 'conductor_group', 'retired']:
+
+        for field in ['maintenance', 'fault', 'conductor_group', 'retired',
+                      'sharded']:
             if getattr(parsed_args, field) is not None:
                 params[field] = getattr(parsed_args, field)
         for field in ['provision_state', 'driver', 'resource_class',
                       'chassis', 'conductor', 'owner', 'lessee',
-                      'description_contains']:
+                      'description_contains', 'shards']:
             if getattr(parsed_args, field):
                 params[field] = getattr(parsed_args, field)
         if parsed_args.long:
             params['detail'] = parsed_args.long
             columns = res_fields.NODE_DETAILED_RESOURCE.fields
             labels = res_fields.NODE_DETAILED_RESOURCE.labels
         elif parsed_args.fields:
@@ -876,17 +902,17 @@
     """Set provision state of baremetal node to 'manage'"""
 
     log = logging.getLogger(__name__ + ".ManageBaremetalNode")
     PROVISION_STATE = 'manage'
 
 
 class PassthruCallBaremetalNode(command.Command):
-    """Call a vendor passthu method for a node"""
+    """Call a vendor passthru method for a node"""
 
-    log = logging.getLogger(__name__ + ".PassthuCallBaremetalNode")
+    log = logging.getLogger(__name__ + ".PassthruCallBaremetalNode")
 
     def get_parser(self, prog_name):
         parser = super(PassthruCallBaremetalNode, self).get_parser(
             prog_name)
 
         parser.add_argument(
             'node',
@@ -1394,14 +1420,19 @@
             metavar='<lessee>',
             help=_('Set the lessee for the node')),
         parser.add_argument(
             "--description",
             metavar='<description>',
             help=_('Set the description for the node'),
         )
+        parser.add_argument(
+            "--shard",
+            metavar='<shard>',
+            help=_('Set the shard for the node'),
+        )
 
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         if parsed_args.name and len(parsed_args.nodes) > 1:
@@ -1424,15 +1455,15 @@
                 baremetal_client.node.set_target_raid_config(node, raid_config)
 
         properties = []
         for field in ['instance_uuid', 'name',
                       'chassis_uuid', 'driver', 'resource_class',
                       'conductor_group', 'protected', 'protected_reason',
                       'retired', 'retired_reason', 'owner', 'lessee',
-                      'description']:
+                      'description', 'shard']:
             value = getattr(parsed_args, field)
             if value:
                 properties.extend(utils.args_array_to_patch(
                     'add', ["%s=%s" % (field, value)]))
 
         if parsed_args.automated_clean is not None:
             properties.extend(utils.args_array_to_patch(
@@ -1740,14 +1771,19 @@
             help=_('Unset the lessee field of the node'),
         )
         parser.add_argument(
             "--description",
             action="store_true",
             help=_('Unset the description field of the node'),
         )
+        parser.add_argument(
+            "--shard",
+            action="store_true",
+            help=_('Unset the shard field of the node'),
+        )
 
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
@@ -1764,15 +1800,16 @@
                       'resource_class', 'conductor_group', 'automated_clean',
                       'bios_interface', 'boot_interface', 'console_interface',
                       'deploy_interface', 'inspect_interface',
                       'management_interface', 'network_interface',
                       'power_interface', 'raid_interface', 'rescue_interface',
                       'storage_interface', 'vendor_interface',
                       'protected', 'protected_reason', 'retired',
-                      'retired_reason', 'owner', 'lessee', 'description']:
+                      'retired_reason', 'owner', 'lessee', 'description',
+                      'shard', ]:
             if getattr(parsed_args, field):
                 properties.extend(utils.args_array_to_patch('remove', [field]))
 
         if parsed_args.property:
             properties.extend(utils.args_array_to_patch('remove',
                               ['properties/' + x
                                for x in parsed_args.property]))
@@ -2173,15 +2210,15 @@
             'node',
             metavar='<node>',
             help=_("Name or UUID of the node.")
         )
         parser.add_argument(
             '--long',
             default=False,
-            help=_("Show detailed information about the BIOS settings."),
+            help=_("Show detailed information about the node history events."),
             action='store_true')
         return parser
 
     def take_action(self, parsed_args):
         self.log.debug("take_action(%s)", parsed_args)
 
         baremetal_client = self.app.client_manager.baremetal
@@ -2229,7 +2266,37 @@
 
         data = baremetal_client.node.get_history_event(
             parsed_args.node,
             parsed_args.event)
         data.pop('links')
 
         return self.dict2columns(data)
+
+
+class NodeInventorySave(command.Command):
+    """Get hardware inventory of a node (in JSON format) or save it to file."""
+
+    log = logging.getLogger(__name__ + ".NodeInventorySave")
+
+    def get_parser(self, prog_name):
+        parser = super(NodeInventorySave, self).get_parser(prog_name)
+        parser.add_argument(
+            "node",
+            metavar="<node>",
+            help=_("Name or UUID of the node"))
+        parser.add_argument("--file",
+                            metavar="<filename>",
+                            help="Save inspection data to file with name "
+                            "(default: stdout).")
+        return parser
+
+    def take_action(self, parsed_args):
+        self.log.debug("take_action(%s)", parsed_args)
+
+        baremetal_client = self.app.client_manager.baremetal
+        inventory = baremetal_client.node.get_inventory(parsed_args.node)
+
+        if parsed_args.file:
+            with open(parsed_args.file, 'w') as fp:
+                json.dump(inventory, fp)
+        else:
+            json.dump(inventory, sys.stdout)
```

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_port.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_portgroup.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_connector.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/osc/v1/baremetal_volume_target.py` & `python-ironicclient-5.3.0/ironicclient/osc/v1/baremetal_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/shell.py` & `python-ironicclient-5.3.0/ironicclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/base.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/base.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_chassis_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_conductor_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_deploy_template_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_driver_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_create_negative.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_negative.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_power_states.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_node_provision_states.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_port_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/osc/v1/test_baremetal_portgroup_basic.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/functional/utils.py` & `python-ironicclient-5.3.0/ironicclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_base.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/common/apiclient/test_base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/common/apiclient/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_base.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_base.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_filecache.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_filecache.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_http.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_http.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/common/test_utils.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/fakes.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/fakes.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/test_plugin.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/fakes.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,14 +237,31 @@
         'event': 'meow',
         'event_type': 'purring',
         'conductor': 'lap-conductor',
         'user': '0191',
         'links': {'href': 'url', 'rel': 'self'},
     }
 ]
+NODE_INVENTORY = [
+    {
+        'inventory':
+        {
+            'memory': {'physical_mb': 3072},
+            'cpu': {'count': 1,
+                    'model_name': 'qemu64',
+                    'architecture': 'x86_64'},
+            'disks': [{'name': 'testvm2.qcow2',
+                       'size': 11811160064}],
+            'interfaces': [{'mac_address': '52:54:00:11:2d:26'}],
+            'system_vendor': {'product_name': 'testvm2',
+                              'manufacturer': 'Sushy Emulator'},
+            'boot': {'current_boot_mode': 'uefi'}
+        }
+    }
+]
 
 
 class TestBaremetal(utils.TestCommand):
 
     def setUp(self):
         super(TestBaremetal, self).setUp()
```

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_create.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 #   distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 #
 
 import copy
+import io
 import json
+import sys
 from unittest import mock
 
 from osc_lib.tests import utils as oscutils
 
 from ironicclient.common import utils as commonutils
 from ironicclient import exc
 from ironicclient.osc.v1 import baremetal_node
@@ -725,14 +727,19 @@
                                 {'description': 'there is no spoon'})
 
     def test_baremetal_create_with_lessee(self):
         self.check_with_options(['--lessee', 'lessee 1'],
                                 [('lessee', 'lessee 1')],
                                 {'lessee': 'lessee 1'})
 
+    def test_baremetal_create_with_shard(self):
+        self.check_with_options(['--shard', 'myshard'],
+                                [('shard', 'myshard')],
+                                {'shard': 'myshard'})
+
 
 class TestBaremetalDelete(TestBaremetal):
     def setUp(self):
         super(TestBaremetalDelete, self).setUp()
 
         self.baremetal_mock.node.get.return_value = (
             baremetal_fakes.FakeBaremetalResource(
@@ -1398,15 +1405,15 @@
         ]
         verifylist = [
             ('fields', [['uuid', 'name'], ['extra']])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
-        self.cmd.take_action(parsed_args)
+        self.cmd.take_action(parsed_args=parsed_args)
 
         # Set expected values
         kwargs = {
             'marker': None,
             'limit': None,
             'detail': False,
             'fields': ('uuid', 'name', 'extra')
@@ -1424,14 +1431,77 @@
             ('fields', [['uuid', 'invalid']])
         ]
 
         self.assertRaises(oscutils.ParserException,
                           self.check_parser,
                           self.cmd, arglist, verifylist)
 
+    def test_baremetal_list_by_shards(self):
+        arglist = ['--shards', 'myshard1', 'myshard2']
+        verifylist = [
+            ('shards', ['myshard1', 'myshard2'])
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        kwargs = {
+            'marker': None,
+            'limit': None,
+            'shards': ['myshard1', 'myshard2'],
+        }
+
+        self.baremetal_mock.node.list.assert_called_with(
+            **kwargs
+        )
+
+    def test_baremetal_list_sharded(self):
+        arglist = ['--sharded']
+        verifylist = [('sharded', True)]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        kwargs = {
+            'marker': None,
+            'limit': None,
+            'sharded': True,
+        }
+
+        self.baremetal_mock.node.list.assert_called_with(
+            **kwargs
+        )
+
+    def test_baremetal_list_unsharded(self):
+        arglist = ['--unsharded']
+        verifylist = [('sharded', False)]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        kwargs = {
+            'marker': None,
+            'limit': None,
+            'sharded': False,
+        }
+
+        self.baremetal_mock.node.list.assert_called_with(
+            **kwargs
+        )
+
+    def test_baremetal_list_sharded_unsharded_fail(self):
+        arglist = ['--sharded', '--unsharded']
+        verifylist = [('sharded', True), ('sharded', False)]
+
+        self.assertRaises(oscutils.ParserException, self.check_parser,
+                          self.cmd, arglist, verifylist)
+
 
 class TestBaremetalMaintenanceSet(TestBaremetal):
     def setUp(self):
         super(TestBaremetalMaintenanceSet, self).setUp()
 
         # Get the command object to test
         self.cmd = baremetal_node.MaintenanceSetBaremetalNode(self.app, None)
@@ -3127,14 +3197,34 @@
         self.baremetal_mock.node.update.assert_called_once_with(
             'node_uuid', [{'op': 'add',
                            'path': '/lessee',
                            'value': 'lessee 1'}],
             reset_interfaces=None
         )
 
+    def test_baremetal_set_shard(self):
+        arglist = [
+            'node_uuid',
+            '--shard', 'myshard',
+        ]
+        verifylist = [
+            ('nodes', ['node_uuid']),
+            ('shard', 'myshard')
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.update.assert_called_once_with(
+            'node_uuid', [{'op': 'add',
+                           'path': '/shard',
+                           'value': 'myshard'}],
+            reset_interfaces=None
+        )
+
     @mock.patch.object(commonutils, 'get_from_stdin', autospec=True)
     @mock.patch.object(commonutils, 'handle_json_or_file_arg', autospec=True)
     def test_baremetal_set_network_data(self, mock_handle, mock_stdin):
         self.cmd.log = mock.Mock(autospec=True)
         network_data_string = '{"a": ["b"]}'
         expected_network_data = {'a': ['b']}
         mock_handle.return_value = expected_network_data.copy()
@@ -3769,14 +3859,33 @@
         self.cmd.take_action(parsed_args)
 
         self.baremetal_mock.node.update.assert_called_once_with(
             'node_uuid',
             [{'path': '/lessee', 'op': 'remove'}]
         )
 
+    def test_baremetal_unset_shard(self):
+        arglist = [
+            'node_uuid',
+            '--shard',
+        ]
+        verifylist = [
+            ('nodes', ['node_uuid']),
+            ('shard', True)
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.update.assert_called_once_with(
+            'node_uuid',
+            [{'path': '/shard', 'op': 'remove'}]
+        )
+
     def test_baremetal_unset_network_data(self):
         arglist = [
             'node_uuid',
             '--network-data',
         ]
         verifylist = [
             ('nodes', ['node_uuid']),
@@ -4298,7 +4407,44 @@
         expected_columns = ('conductor', 'created_at', 'event', 'event_type',
                             'severity', 'user', 'uuid')
         expected_data = ('lap-conductor', 'time', 'meow', 'purring', 'info',
                          '0191', 'abcdef1')
 
         self.assertEqual(expected_columns, columns)
         self.assertEqual(expected_data, tuple(data))
+
+
+class TestNodeInventorySave(TestBaremetal):
+    def setUp(self):
+        super(TestNodeInventorySave, self).setUp()
+
+        self.baremetal_mock.node.get_inventory.return_value = (
+            baremetal_fakes.NODE_INVENTORY[0])
+
+        # Get the command object to test
+        self.cmd = baremetal_node.NodeInventorySave(self.app, None)
+
+    def test_baremetal_node_inventory_save(self):
+        arglist = ['node_uuid']
+        verifylist = [('node', 'node_uuid')]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        buf = io.StringIO()
+        with mock.patch.object(sys, 'stdout', buf):
+            self.cmd.take_action(parsed_args)
+
+        self.baremetal_mock.node.get_inventory.assert_called_once_with(
+            'node_uuid')
+
+        expected_data = {'memory': {'physical_mb': 3072},
+                         'cpu': {'count': 1,
+                                 'model_name': 'qemu64',
+                                 'architecture': 'x86_64'},
+                         'disks': [{'name': 'testvm2.qcow2',
+                                    'size': 11811160064}],
+                         'interfaces': [{'mac_address': '52:54:00:11:2d:26'}],
+                         'system_vendor': {'product_name': 'testvm2',
+                                           'manufacturer': 'Sushy Emulator'},
+                         'boot': {'current_boot_mode': 'uefi'}}
+        inventory = json.loads(buf.getvalue())
+        self.assertEqual(expected_data, inventory['inventory'])
```

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/osc/v1/test_baremetal_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/test_client.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/test_exc.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/test_exc.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/test_import.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/test_import.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/utils.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_allocation.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_chassis.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_client.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_conductor.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_create_resources.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_create_resources.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_deploy_template.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_driver.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_events.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_events.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_node.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,16 @@
          'driver_info': {'user': 'foo', 'password': 'bar'},
          'properties': {'num_cpu': 4},
          'network_data': {},
          'resource_class': 'bar',
          'extra': {},
          'owner': '33333333-2222-1111-0000-111111111111',
          'retired': True,
-         'lessee': '77777777-8888-5555-2222-999999999999'}
+         'lessee': '77777777-8888-5555-2222-999999999999',
+         'shard': 'myshard'}
 PORT = {'uuid': '11111111-2222-3333-4444-555555555555',
         'node_uuid': '66666666-7777-8888-9999-000000000000',
         'address': 'AA:AA:AA:AA:AA:AA',
         'extra': {}}
 PORTGROUP = {'uuid': '11111111-2222-3333-4444-555555555555',
              'name': 'Portgroup',
              'node_uuid': '66666666-7777-8888-9999-000000000000',
@@ -104,14 +105,21 @@
 NODE_VENDOR_PASSTHRU_METHOD = {"heartbeat": {"attach": "false",
                                              "http_methods": ["POST"],
                                              "description": "",
                                              "async": "true"}}
 
 VIFS = {'vifs': [{'id': 'aaa-aaa'}]}
 TRAITS = {'traits': ['CUSTOM_FOO', 'CUSTOM_BAR']}
+INVENTORY = {'inventory': [{'memory': {'physical_mb': '3072'},
+                            'cpu': {'count': 1, 'architecture': 'x86_64',
+                                    'model_name': 'qemu64'},
+                            'disks': [{'name': 'testvm2.qcow2',
+                                       'size': 11811160064}],
+                            'interfaces':
+                            [{'mac_address': '52:54:00:c7:02:45'}]}]}
 
 CREATE_NODE = copy.deepcopy(NODE1)
 del CREATE_NODE['uuid']
 del CREATE_NODE['maintenance']
 del CREATE_NODE['provision_state']
 
 UPDATED_NODE = copy.deepcopy(NODE1)
@@ -256,14 +264,28 @@
     '/v1/nodes/?conductor=fake-conductor':
     {
         'GET': (
             {},
             {"nodes": [NODE2]},
         )
     },
+    '/v1/nodes/?sharded=False':
+    {
+        'GET': (
+            {},
+            {"nodes": [NODE1]},
+        )
+    },
+    '/v1/nodes/?shard=myshard':
+    {
+        'GET': (
+            {},
+            {"nodes": [NODE2]}
+        )
+    },
     '/v1/nodes/detail?instance_uuid=%s' % NODE2['instance_uuid']:
     {
         'GET': (
             {},
             {"nodes": [NODE2]},
         )
     },
@@ -539,14 +561,21 @@
             {},
             None,
         ),
         'DELETE': (
             {},
             None,
         ),
+    },
+    '/v1/nodes/%s/inventory' % NODE1['uuid']:
+    {
+        'GET': (
+            {},
+            INVENTORY,
+        ),
     }
 }
 
 fake_responses_pagination = {
     '/v1/nodes':
     {
         'GET': (
@@ -965,14 +994,32 @@
         expect = [
             ('GET', '/v1/nodes/?conductor=fake-conductor', {}, None),
         ]
         self.assertEqual(expect, self.api.calls)
         self.assertThat(nodes, HasLength(1))
         self.assertEqual(NODE2['uuid'], getattr(nodes[0], 'uuid'))
 
+    def test_node_list_not_sharded(self):
+        nodes = self.mgr.list(sharded=False)
+        expect = [
+            ('GET', '/v1/nodes/?sharded=False', {}, None),
+        ]
+        self.assertEqual(expect, self.api.calls)
+        self.assertThat(nodes, HasLength(1))
+        self.assertEqual(NODE1['uuid'], getattr(nodes[0], 'uuid'))
+
+    def test_node_list_by_shard(self):
+        nodes = self.mgr.list(shards=["myshard"])
+        expect = [
+            ('GET', '/v1/nodes/?shard=myshard', {}, None),
+        ]
+        self.assertEqual(expect, self.api.calls)
+        self.assertThat(nodes, HasLength(1))
+        self.assertEqual(NODE2['uuid'], getattr(nodes[0], 'uuid'))
+
     def test_node_list_detail(self):
         nodes = self.mgr.list(detail=True)
         expect = [
             ('GET', '/v1/nodes/detail', {}, None),
         ]
         self.assertEqual(expect, self.api.calls)
         self.assertEqual(2, len(nodes))
@@ -2144,7 +2191,15 @@
         resp = self.mgr.remove_trait(NODE1['uuid'], trait)
         expect = [
             ('DELETE', '/v1/nodes/%s/traits/%s' % (NODE1['uuid'], trait),
                 {}, None),
         ]
         self.assertEqual(expect, self.api.calls)
         self.assertIsNone(resp)
+
+    def test_node_get_inventory(self):
+        inventory = self.mgr.get_inventory(NODE1['uuid'])
+        expect = [
+            ('GET', '/v1/nodes/%s/inventory' % NODE1['uuid'], {}, None),
+        ]
+        self.assertEqual(expect, self.api.calls)
+        self.assertEqual(INVENTORY, inventory)
```

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_port.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_portgroup.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_resource_fields.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_connector.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/tests/unit/v1/test_volume_target.py` & `python-ironicclient-5.3.0/ironicclient/tests/unit/v1/test_volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/allocation.py` & `python-ironicclient-5.3.0/ironicclient/v1/allocation.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/chassis.py` & `python-ironicclient-5.3.0/ironicclient/v1/chassis.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/client.py` & `python-ironicclient-5.3.0/ironicclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/conductor.py` & `python-ironicclient-5.3.0/ironicclient/v1/conductor.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/create_resources.py` & `python-ironicclient-5.3.0/ironicclient/v1/create_resources.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/deploy_template.py` & `python-ironicclient-5.3.0/ironicclient/v1/deploy_template.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/driver.py` & `python-ironicclient-5.3.0/ironicclient/v1/driver.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/events.py` & `python-ironicclient-5.3.0/ironicclient/v1/events.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/node.py` & `python-ironicclient-5.3.0/ironicclient/v1/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     def list(self, associated=None, maintenance=None, marker=None,
              limit=None, detail=False, sort_key=None, sort_dir=None,
              fields=None, provision_state=None, driver=None,
              resource_class=None, chassis=None, fault=None,
              os_ironic_api_version=None, conductor_group=None,
              conductor=None, owner=None, retired=None, lessee=None,
-             global_request_id=None):
+             shards=None, sharded=None, global_request_id=None):
         """Retrieve a list of nodes.
 
         :param associated: Optional. Either a Boolean or a string
                            representation of a Boolean that indicates whether
                            to return a list of associated (True or "True") or
                            unassociated (False or "False") nodes.
         :param maintenance: Optional. Either a Boolean or a string
@@ -122,17 +122,22 @@
             value (in form "req-<UUID>") to use for the request.
 
         :param conductor_group: Optional. String value to get only nodes
                                 with the given conductor group set.
         :param conductor: Optional. String value to get only nodes
                           mapped to the given conductor.
         :param owner: Optional. String value to get only nodes
-                          mapped to a specific owner.
+                      mapped to a specific owner.
         :param lessee: Optional. String value to get only nodes
-                          mapped to a specific lessee.
+                       mapped to a specific lessee.
+        :param shards: Optional. A list with a specified set of shards
+                      to limit node returns to.
+        :param sharded: Optional. Boolean value, when true get only nodes
+                        with a non-null node.shard value, when false get only
+                        nodes with a null node.shard value. None is a noop.
 
         :returns: A list of nodes.
 
         """
         if limit is not None:
             limit = int(limit)
 
@@ -162,14 +167,18 @@
             filters.append('conductor_group=%s' % conductor_group)
         if conductor is not None:
             filters.append('conductor=%s' % conductor)
         if owner is not None:
             filters.append('owner=%s' % owner)
         if lessee is not None:
             filters.append('lessee=%s' % lessee)
+        if sharded is not None:
+            filters.append('sharded=%s' % sharded)
+        if shards is not None:
+            filters.append('shard=%s' % ','.join(shards))
 
         path = ''
         if detail:
             path += 'detail'
         if filters:
             path += '?' + '&'.join(filters)
         header_values = {"os_ironic_api_version": os_ironic_api_version,
@@ -1081,21 +1090,40 @@
                           node_ident,
                           event,
                           os_ironic_api_version=None,
                           global_request_id=None):
         """Get a single event record for a node.
 
         Provides the ability to request, and return
-        a node's single vent hisotyr entry.
+        a node's single event history entry.
 
         :param node_ident: The name or UUID of the node.
         :param event: The UUID of the event entry as listed
                       in the node event history list.
         :param os_ironic_api_version: String version (e.g. "1.35") to use for
             the request.  If not specified, the client's default is used.
         :param global_request_id: String containing global request ID header
             value (in form "req-<UUID>") to use for the request.
         """
         path = "%s/history/%s" % (node_ident, event)
         return self._get_as_dict(
             path, os_ironic_api_version=os_ironic_api_version,
             global_request_id=global_request_id)
+
+    def get_inventory(self,
+                      node_ident,
+                      os_ironic_api_version=None,
+                      global_request_id=None):
+        """Get the hardware inventory of the node.
+
+        Requires API version 1.81.
+
+        :param node_ident: The name or UUID of the node.
+        :param os_ironic_api_version: String version (e.g. "1.81") to use for
+            the request.  If not specified, the client's default is used.
+        :param global_request_id: String containing global request ID header
+            value (in form "req-<UUID>") to use for the request.
+        """
+        path = "%s/inventory" % node_ident
+        return self._get_as_dict(
+            path, os_ironic_api_version=os_ironic_api_version,
+            global_request_id=global_request_id)
```

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/port.py` & `python-ironicclient-5.3.0/ironicclient/v1/port.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/portgroup.py` & `python-ironicclient-5.3.0/ironicclient/v1/portgroup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/resource_fields.py` & `python-ironicclient-5.3.0/ironicclient/v1/resource_fields.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/utils.py` & `python-ironicclient-5.3.0/ironicclient/v1/utils.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/volume_connector.py` & `python-ironicclient-5.3.0/ironicclient/v1/volume_connector.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/ironicclient/v1/volume_target.py` & `python-ironicclient-5.3.0/ironicclient/v1/volume_target.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/playbooks/functional/run.yaml` & `python-ironicclient-5.3.0/playbooks/functional/run.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/python_ironicclient.egg-info/PKG-INFO` & `python-ironicclient-5.3.0/python_ironicclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ironicclient
-Version: 5.2.0
+Version: 5.3.0
 Summary: OpenStack Bare Metal Provisioning API Client Library
 Home-page: https://docs.openstack.org/python-ironicclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================================
         Python bindings for the Ironic API
```

### Comparing `python-ironicclient-5.2.0/python_ironicclient.egg-info/SOURCES.txt` & `python-ironicclient-5.3.0/python_ironicclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
 releasenotes/notes/add-network-data-node-attr-81dec9cecb7491b9.yaml
 releasenotes/notes/add-neutron-integration-fields-cee7596c49722de6.yaml
 releasenotes/notes/add-no-retired-opt-403bb5e466e4facb.yaml
 releasenotes/notes/add-node-boot-mode-08ac768649a2fc93.yaml
 releasenotes/notes/add-node-boot-mode-set-9746b45aa3f80fe8.yaml
 releasenotes/notes/add-node-description-support-6efd0882eaa0c788.yaml
 releasenotes/notes/add-node-history-b9b9beeb0200f185.yaml
+releasenotes/notes/add-node-inventory-74e856c019cfa7e2.yaml
 releasenotes/notes/add-node-lessee-c36409eb0415f75d.yaml
 releasenotes/notes/add-node-owner-c2dce5a6075ce2b7.yaml
 releasenotes/notes/add-node-resource-class-6040d1d6c734522c.yaml
 releasenotes/notes/add-pecan-exc-construction-a776408f7ae110dc.yaml
 releasenotes/notes/add-port-internal-info-74a03ebd8b0a3dfc.yaml
 releasenotes/notes/add-portgroup-mode-properties-0a3023cf905adaef.yaml
 releasenotes/notes/add-portgroups-support-c3cf3826093ee815.yaml
@@ -232,14 +233,15 @@
 releasenotes/notes/network_data-c48b3878a5b04df5.yaml
 releasenotes/notes/no-automated-clean-0e437581ded44eb3.yaml
 releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml
 releasenotes/notes/no-resource-attributeerror-d0cb327abab7dcc0.yaml
 releasenotes/notes/node-deploy-step-061e8925dfee3918.yaml
 releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml
 releasenotes/notes/node-fault-adbe74fd600063ee.yaml
+releasenotes/notes/node-shard-support-774ebfe6719fc7c2.yaml
 releasenotes/notes/not-ignore-delete-failtures-0783d33a606ed6f1.yaml
 releasenotes/notes/osc-baremetal-driver-raid-properties-159bd57058c0fc0e.yaml
 releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml
 releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml
 releasenotes/notes/osc-default-microver-172d6e69316e70c1.yaml
 releasenotes/notes/osc-instance-crash-dump-22634a57104561a5.yaml
 releasenotes/notes/osc-max-microver-22-dc0d91a62f03a2e6.yaml
```

### Comparing `python-ironicclient-5.2.0/python_ironicclient.egg-info/entry_points.txt` & `python-ironicclient-5.3.0/python_ironicclient.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 baremetal_node_create = ironicclient.osc.v1.baremetal_node:CreateBaremetalNode
 baremetal_node_delete = ironicclient.osc.v1.baremetal_node:DeleteBaremetalNode
 baremetal_node_deploy = ironicclient.osc.v1.baremetal_node:DeployBaremetalNode
 baremetal_node_history_get = ironicclient.osc.v1.baremetal_node:NodeHistoryEventGet
 baremetal_node_history_list = ironicclient.osc.v1.baremetal_node:NodeHistoryList
 baremetal_node_inject_nmi = ironicclient.osc.v1.baremetal_node:InjectNmiBaremetalNode
 baremetal_node_inspect = ironicclient.osc.v1.baremetal_node:InspectBaremetalNode
+baremetal_node_inventory_save = ironicclient.osc.v1.baremetal_node:NodeInventorySave
 baremetal_node_list = ironicclient.osc.v1.baremetal_node:ListBaremetalNode
 baremetal_node_maintenance_set = ironicclient.osc.v1.baremetal_node:MaintenanceSetBaremetalNode
 baremetal_node_maintenance_unset = ironicclient.osc.v1.baremetal_node:MaintenanceUnsetBaremetalNode
 baremetal_node_manage = ironicclient.osc.v1.baremetal_node:ManageBaremetalNode
 baremetal_node_passthru_call = ironicclient.osc.v1.baremetal_node:PassthruCallBaremetalNode
 baremetal_node_passthru_list = ironicclient.osc.v1.baremetal_node:PassthruListBaremetalNode
 baremetal_node_power_off = ironicclient.osc.v1.baremetal_node:PowerOffBaremetalNode
```

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/accept-valid_interfaces-3b8f5e3e362e04cd.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/add-create-command-3df5efbbecc33276.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/add-deploy-steps-arg-0b127e29c8cf976d.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/add-volume-connector-api-873090474d5e41b8.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/add-volume-connector-cli-873090474d5e41b9.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/add-volume-target-api-e062303f4b3b40ef.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/add-volume-target-cli-e062303f4b3b40f0.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/allow-api-user-to-use-latest-6b80e9f584eaaa4e.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/bug-1524745-extend-driver-list-and-driver-show-800d96393aa17342.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/deprecate-http-client-8d664e5ec50ec403.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/ironic-cli-version-a5cdec73d585444d.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/latest-default-41fdcc49701c4d70.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/manual-clean-09f6b49df7d2513f.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/no-osc-requirement-411f25fd10f18caa.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/node-driver-support-storage-interface-e93fc8d4de5d24d6.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/osc-baremetal-node-bios-setting-list-b062b31d0d4de337.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/osc-commands-1-7-d531960472a11ac2.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-f87e0fbb472261dd.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/osc-plugin-ff0d897d8441a9e1.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/osc-port-set-llc-pxeenabled-21fd8ea1982af17e.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/prelude-2-0-release-ee44150902d3d399.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/remove-deprecated-osc-cmd-6dc980299d2fbde4.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/support-passing-global-request-id-4b96beb31ec906cb.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml` & `python-ironicclient-5.3.0/releasenotes/notes/traits-support-8864f6816abecdb2.yaml`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/releasenotes/source/conf.py` & `python-ironicclient-5.3.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/requirements.txt` & `python-ironicclient-5.3.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/setup.cfg` & `python-ironicclient-5.3.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 	baremetal_node_console_show = ironicclient.osc.v1.baremetal_node:ConsoleShowBaremetalNode
 	baremetal_node_create = ironicclient.osc.v1.baremetal_node:CreateBaremetalNode
 	baremetal_node_delete = ironicclient.osc.v1.baremetal_node:DeleteBaremetalNode
 	baremetal_node_deploy = ironicclient.osc.v1.baremetal_node:DeployBaremetalNode
 	baremetal_node_history_list = ironicclient.osc.v1.baremetal_node:NodeHistoryList
 	baremetal_node_history_get = ironicclient.osc.v1.baremetal_node:NodeHistoryEventGet
 	baremetal_node_inspect = ironicclient.osc.v1.baremetal_node:InspectBaremetalNode
+	baremetal_node_inventory_save = ironicclient.osc.v1.baremetal_node:NodeInventorySave
 	baremetal_node_list = ironicclient.osc.v1.baremetal_node:ListBaremetalNode
 	baremetal_node_maintenance_set = ironicclient.osc.v1.baremetal_node:MaintenanceSetBaremetalNode
 	baremetal_node_maintenance_unset = ironicclient.osc.v1.baremetal_node:MaintenanceUnsetBaremetalNode
 	baremetal_node_manage = ironicclient.osc.v1.baremetal_node:ManageBaremetalNode
 	baremetal_node_passthru_call = ironicclient.osc.v1.baremetal_node:PassthruCallBaremetalNode
 	baremetal_node_passthru_list = ironicclient.osc.v1.baremetal_node:PassthruListBaremetalNode
 	baremetal_node_power_off = ironicclient.osc.v1.baremetal_node:PowerOffBaremetalNode
```

### Comparing `python-ironicclient-5.2.0/setup.py` & `python-ironicclient-5.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/tools/install_venv_common.py` & `python-ironicclient-5.3.0/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/tox.ini` & `python-ironicclient-5.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `python-ironicclient-5.2.0/zuul.d/ironicclient-jobs.yaml` & `python-ironicclient-5.3.0/zuul.d/ironicclient-jobs.yaml`

 * *Files identical despite different names*

