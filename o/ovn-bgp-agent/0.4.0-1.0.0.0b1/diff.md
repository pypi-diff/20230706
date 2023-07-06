# Comparing `tmp/ovn-bgp-agent-0.4.0.tar.gz` & `tmp/ovn-bgp-agent-1.0.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovn-bgp-agent-0.4.0.tar", last modified: Tue May  9 07:52:19 2023, max compression
+gzip compressed data, was "ovn-bgp-agent-1.0.0.0b1.tar", last modified: Thu Jul  6 08:55:46 2023, max compression
```

## Comparing `ovn-bgp-agent-0.4.0.tar` & `ovn-bgp-agent-1.0.0.0b1.tar`

### file list

```diff
@@ -1,139 +1,150 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8049 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.031950 ovn-bgp-agent-0.4.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.031950 ovn-bgp-agent-0.4.0/doc/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105821 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/images/evpn_traffic_flow.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    97580 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/images/networking-bgpvpn_integration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.031950 ovn-bgp-agent-0.4.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2652 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25047 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/contributor/bgp_mode_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11445 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/contributor/bgp_mode_stretched_l2_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10242 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/contributor/bgp_supportability_matrix.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21038 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/contributor/evpn_mode_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.027950 ovn-bgp-agent-0.4.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/etc/ovn-bgp-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/etc/ovn-bgp-agent/rootwrap.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/etc/ovn-bgp-agent/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/cmd/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/driver_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18122 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52214 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36578 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19983 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/bgp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/driver_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4286 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/frr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19635 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/ovn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10797 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/ovs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12642 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/wire.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1676 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19173 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9108 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8637 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13943 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/ovs_vsctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/vtysh.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/test_ovn_bgp_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/cmd/test_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25492 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   104860 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34302 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40432 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3789 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29339 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17174 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.039950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47254 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22830 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19083 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16638 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/privileged/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3222 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2241 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/test_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31963 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/utils/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/ovn_bgp_agent/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27107 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent/utils/linux_net.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.035950 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4173 2023-05-09 07:52:19.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-05-09 07:52:18.000000 ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.031950 ovn-bgp-agent-0.4.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/releasenotes/notes/nb_driver-cc7098183fcedb0a.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-09 07:52:19.043950 ovn-bgp-agent-0.4.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2023-05-09 07:51:55.000000 ovn-bgp-agent-0.4.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      439 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9207 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.516907 ovn-bgp-agent-1.0.0.0b1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.516907 ovn-bgp-agent-1.0.0.0b1/doc/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105821 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/images/evpn_traffic_flow.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97580 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/images/networking-bgpvpn_integration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.516907 ovn-bgp-agent-1.0.0.0b1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2652 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.516907 ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25047 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/bgp_mode_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11445 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/bgp_mode_stretched_l2_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10242 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/bgp_supportability_matrix.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21038 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/evpn_mode_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.512906 ovn-bgp-agent-1.0.0.0b1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.516907 ovn-bgp-agent-1.0.0.0b1/etc/ovn-bgp-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/etc/ovn-bgp-agent/rootwrap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.516907 ovn-bgp-agent-1.0.0.0b1/etc/ovn-bgp-agent/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.516907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.520907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/cmd/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9481 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.520907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/driver_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.520907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18499 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52783 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36645 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20469 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.520907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/bgp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/driver_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4286 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/frr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20288 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/ovn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11321 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/ovs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12847 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/wire.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.520907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19572 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9060 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8838 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3291 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.520907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20624 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/ovs_vsctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/vtysh.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4301 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27574 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/privileged/test_linux_net.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5238 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/functional/utils/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/test_ovn_bgp_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/cmd/test_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25980 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105282 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34238 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41961 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3789 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30016 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17061 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.524908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48656 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22830 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19163 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4149 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/privileged/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3222 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2241 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/test_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/utils/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32522 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/utils/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1751 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/utils/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27428 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/utils/linux_net.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.520907 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1524 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4551 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2023-07-06 08:55:46.000000 ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.512906 ovn-bgp-agent-1.0.0.0b1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/releasenotes/notes/nb_driver-cc7098183fcedb0a.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      694 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1736 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 08:55:46.528908 ovn-bgp-agent-1.0.0.0b1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-07-06 08:55:19.000000 ovn-bgp-agent-1.0.0.0b1/zuul.d/project.yaml
```

### Comparing `ovn-bgp-agent-0.4.0/CONTRIBUTING.rst` & `ovn-bgp-agent-1.0.0.0b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ChangeLog` & `ovn-bgp-agent-1.0.0.0b1/ChangeLog`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,37 @@
 CHANGES
 =======
 
+1.0.0.0b1
+---------
+
+* [functional testing] enhance \_get\_device aux function
+* Ensure agent is protected again wrong/missing bridge mappings
+* Explicitly define the MAC address when creating the interface
+* Avoid vlan device leaking
+* Reshape code around ip neigh
+* CI: add periodic weekly and experimental queue
+* Config register\_opts for tests in base class
+* Minor code improvements around move from NDB to IPRoute
+* Ensure FIPs are exposed as part of cr-lrp binding events
+* Avoid usage of NDB linux\_net utils
+* Avoid usage of NDB in ovn\_bgp\_driver, and ovs and wire utils
+* Add new privileged rule methods implementations
+* Add more new privileged method implementations
+* Add new privileged method implementations
+* Retry get\_ovs\_patch\_port\_ofport if empty port
+* Ensure PortBindingChassis Events consider the port up status
+* Minor code improvements on priviledged linux\_net functions
+* [NB Driver] Ensure proper processing of LSP ports creation updates
+* Ensure watchers do not crash
+* Add more pyroute2 protection
+* Give more time for patch ports to be created
+* Publish docs at docs.openstack.org
+* Handle DatapathNotFound in l2 driver
+
 0.4.0
 -----
 
 * Use logical\_port instead of name for port binding (localnet) entries
 * Optimize the patch port ofport retrieval
 * Avoid race condition when adding ovs-flows
 * Ensure options are registered for unit testing
```

### Comparing `ovn-bgp-agent-0.4.0/LICENSE` & `ovn-bgp-agent-1.0.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/PKG-INFO` & `ovn-bgp-agent-1.0.0.0b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.2
 Name: ovn-bgp-agent
-Version: 0.4.0
+Version: 1.0.0.0b1
 Summary: The OVN BGP Agent allows to expose VMs/Containers/Networks through BGP on OVN
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =============
         OVN BGP Agent
         =============
         
         The OVN BGP Agent allows to expose VMs/Containers through BGP on OVN
         
         * Free software: Apache license
-        * Documentation: https://ovn-bgp-agent.readthedocs.io
+        * Documentation: https://docs.openstack.org/ovn-bgp-agent
         * Source: https://opendev.org/openstack/ovn-bgp-agent
         * Bugs: https://bugs.launchpad.net/ovn-bgp-agent
         
         Features
         --------
         
         * Expose VMs with FIPs or on Provider Networks through BGP on OVN
```

### Comparing `ovn-bgp-agent-0.4.0/doc/images/evpn_traffic_flow.png` & `ovn-bgp-agent-1.0.0.0b1/doc/images/evpn_traffic_flow.png`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/doc/images/networking-bgpvpn_integration.png` & `ovn-bgp-agent-1.0.0.0b1/doc/images/networking-bgpvpn_integration.png`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/doc/source/conf.py` & `ovn-bgp-agent-1.0.0.0b1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/doc/source/contributor/bgp_mode_design.rst` & `ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/bgp_mode_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/doc/source/contributor/bgp_mode_stretched_l2_design.rst` & `ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/bgp_mode_stretched_l2_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/doc/source/contributor/bgp_supportability_matrix.rst` & `ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/bgp_supportability_matrix.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/doc/source/contributor/evpn_mode_design.rst` & `ovn-bgp-agent-1.0.0.0b1/doc/source/contributor/evpn_mode_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/doc/source/index.rst` & `ovn-bgp-agent-1.0.0.0b1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/etc/ovn-bgp-agent/rootwrap.conf` & `ovn-bgp-agent-1.0.0.0b1/etc/ovn-bgp-agent/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters` & `ovn-bgp-agent-1.0.0.0b1/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/__init__.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/agent.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/cmd/agent.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/cmd/agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/config.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/config.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/constants.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/constants.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/driver_api.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/driver_api.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,16 @@
         for port in ports:
             if port.type not in [constants.OVN_VM_VIF_PORT_TYPE,
                                  constants.OVN_VIRTUAL_VIF_PORT_TYPE]:
                 continue
             self._ensure_port_exposed(port)
 
         # remove extra wiring leftovers
-        wire_utils.cleanup_wiring(self.ovn_bridge_mappings,
+        wire_utils.cleanup_wiring(self.nb_idl,
+                                  self.ovn_bridge_mappings,
                                   self.ovs_flows,
                                   self._exposed_ips,
                                   self.ovn_routing_tables,
                                   self.ovn_routing_tables_routes)
 
     def _ensure_port_exposed(self, port):
         port_fip = port.external_ids.get(constants.OVN_FIP_EXT_ID_KEY)
@@ -261,14 +262,17 @@
             return False
         localnet, bridge_device, bridge_vlan = self._get_ls_localnet_info(
             logical_switch)
         if not bridge_device:
             # This means it is not a provider network
             self.ovn_tenant_ls[logical_switch] = True
             return False
+        if bridge_device not in self.ovn_bridge_mappings.values():
+            # This node is not properly configured, no need to expose it
+            return False
         if not self.ovn_provider_ls.get(logical_switch):
             self.ovn_provider_ls[logical_switch] = {
                 'bridge_device': bridge_device,
                 'bridge_vlan': bridge_vlan,
                 'localnet': localnet}
         return self._expose_ip(ips, logical_switch, bridge_device, bridge_vlan,
                                port_type=row.type, cidr=row.external_ids.get(
@@ -372,14 +376,17 @@
 
     def _expose_fip(self, ip, logical_switch, row):
         localnet, bridge_device, bridge_vlan = self._get_ls_localnet_info(
             logical_switch)
         if not bridge_device:
             # This means it is not a provider network
             return False
+        if bridge_device not in self.ovn_bridge_mappings.values():
+            # This node is not properly configured, no need to expose it
+            return False
         if not self.ovn_provider_ls.get(logical_switch):
             self.ovn_provider_ls[logical_switch] = {
                 'bridge_device': bridge_device,
                 'bridge_vlan': bridge_vlan,
                 'localnet': localnet}
         tenant_logical_switch = row.external_ids.get(
             constants.OVN_LS_NAME_EXT_ID_KEY)
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import collections
 import ipaddress
-import pyroute2
 import threading
 
 from oslo_concurrency import lockutils
 from oslo_config import cfg
 from oslo_log import log as logging
 
 from ovn_bgp_agent import constants
@@ -26,14 +25,15 @@
 from ovn_bgp_agent.drivers.openstack.utils import bgp as bgp_utils
 from ovn_bgp_agent.drivers.openstack.utils import driver_utils
 from ovn_bgp_agent.drivers.openstack.utils import ovn
 from ovn_bgp_agent.drivers.openstack.utils import ovs
 from ovn_bgp_agent.drivers.openstack.utils import wire as wire_utils
 from ovn_bgp_agent.drivers.openstack.watchers import bgp_watcher as watcher
 from ovn_bgp_agent import exceptions as agent_exc
+from ovn_bgp_agent.utils import helpers
 from ovn_bgp_agent.utils import linux_net
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 # LOG.setLevel(logging.DEBUG)
 # logging.basicConfig(level=logging.DEBUG)
@@ -164,52 +164,55 @@
 
         LOG.debug("Configuring br-ex default rule and routing tables for "
                   "each provider network")
         # 1) Get bridge mappings: xxxx:br-ex,yyyy:br-ex2
         bridge_mappings = self.ovs_idl.get_ovn_bridge_mappings()
         # 2) Get macs for bridge mappings
         extra_routes = {}
-        with pyroute2.NDB() as ndb:
-            for bridge_index, bridge_mapping in enumerate(bridge_mappings, 1):
-                network = bridge_mapping.split(":")[0]
-                bridge = bridge_mapping.split(":")[1]
-                self.ovn_bridge_mappings[network] = bridge
-
-                if not extra_routes.get(bridge):
-                    extra_routes[bridge] = (
-                        linux_net.ensure_routing_table_for_bridge(
-                            self.ovn_routing_tables, bridge,
-                            CONF.bgp_vrf_table_id))
-                vlan_tags = self.sb_idl.get_network_vlan_tag_by_network_name(
-                    network)
-
-                for vlan_tag in vlan_tags:
-                    linux_net.ensure_vlan_device_for_network(bridge,
-                                                             vlan_tag)
-
-                linux_net.ensure_arp_ndp_enabled_for_bridge(bridge,
-                                                            bridge_index,
-                                                            vlan_tags)
-
-                if self.ovs_flows.get(bridge):
-                    continue
-                self.ovs_flows[bridge] = {
-                    'mac': ndb.interfaces[bridge]['address'],
-                    'in_port': set([])}
-                # 3) Get in_port for bridge mappings (br-ex, br-ex2)
-                self.ovs_flows[bridge]['in_port'] = (
-                    ovs.get_ovs_patch_ports_info(bridge))
-
-                # 4) Add/Remove flows for each bridge mappings
-                ovs.ensure_mac_tweak_flows(bridge,
-                                           self.ovs_flows[bridge]['mac'],
-                                           self.ovs_flows[bridge]['in_port'],
-                                           constants.OVS_RULE_COOKIE)
-                ovs.remove_extra_ovs_flows(self.ovs_flows, bridge,
-                                           constants.OVS_RULE_COOKIE)
+
+        for bridge_index, bridge_mapping in enumerate(bridge_mappings, 1):
+            network, bridge = helpers.parse_bridge_mapping(bridge_mapping)
+            if not network:
+                continue
+            self.ovn_bridge_mappings[network] = bridge
+
+            if not extra_routes.get(bridge):
+                extra_routes[bridge] = (
+                    linux_net.ensure_routing_table_for_bridge(
+                        self.ovn_routing_tables, bridge,
+                        CONF.bgp_vrf_table_id))
+            vlan_tags = self.sb_idl.get_network_vlan_tag_by_network_name(
+                network)
+
+            for vlan_tag in vlan_tags:
+                linux_net.ensure_vlan_device_for_network(bridge,
+                                                         vlan_tag)
+
+            linux_net.ensure_arp_ndp_enabled_for_bridge(bridge,
+                                                        bridge_index,
+                                                        vlan_tags)
+
+            if self.ovs_flows.get(bridge):
+                continue
+
+            mac = linux_net.get_interface_address(bridge)
+            self.ovs_flows[bridge] = {
+                'mac': mac,
+                'in_port': set([])}
+            # 3) Get in_port for bridge mappings (br-ex, br-ex2)
+            self.ovs_flows[bridge]['in_port'] = (
+                ovs.get_ovs_patch_ports_info(bridge))
+
+            # 4) Add/Remove flows for each bridge mappings
+            ovs.ensure_mac_tweak_flows(bridge,
+                                       self.ovs_flows[bridge]['mac'],
+                                       self.ovs_flows[bridge]['in_port'],
+                                       constants.OVS_RULE_COOKIE)
+            ovs.remove_extra_ovs_flows(self.ovs_flows, bridge,
+                                       constants.OVS_RULE_COOKIE)
 
         LOG.debug("Syncing current routes.")
         exposed_ips = linux_net.get_exposed_ips(CONF.bgp_nic)
         # get the rules pointing to ovn bridges
         ovn_ip_rules = linux_net.get_ovn_ip_rules(
             self.ovn_routing_tables.values())
 
@@ -253,14 +256,17 @@
         linux_net.delete_ip_rules(ovn_ip_rules)
 
         # remove all the extra rules not needed
         linux_net.delete_bridge_ip_routes(self.ovn_routing_tables,
                                           self.ovn_routing_tables_routes,
                                           extra_routes)
 
+        wire_utils.delete_vlan_devices_leftovers(self.sb_idl,
+                                                 self.ovn_bridge_mappings)
+
     def _ensure_cr_lrp_associated_ports_exposed(self, cr_lrp_port,
                                                 exposed_ips, ovn_ip_rules):
         ips, patch_port_row = self.sb_idl.get_cr_lrp_nat_addresses_info(
             cr_lrp_port, self.chassis, self.sb_idl)
         if not ips:
             return
         ips_adv = self._expose_ip(ips, patch_port_row,
@@ -318,16 +324,17 @@
 
     def _expose_provider_port(self, port_ips, provider_datapath,
                               bridge_device=None, bridge_vlan=None,
                               lladdr=None, proxy_cidrs=None):
         if not bridge_device and not bridge_vlan:
             bridge_device, bridge_vlan = self._get_bridge_for_datapath(
                 provider_datapath)
-            if not bridge_device:
-                return False
+        if (not bridge_device or
+                bridge_device not in self.ovn_bridge_mappings.values()):
+            return False
 
         localnet = self.ovn_provider_datapath.get(provider_datapath)
         if not localnet:
             try:
                 localnet = self.sb_idl.get_localnet_for_datapath(
                     provider_datapath)
                 if localnet:
@@ -903,14 +910,23 @@
         if not self._expose_provider_port(ips_without_mask, provider_datapath,
                                           bridge_device, bridge_vlan,
                                           lladdr=mac, proxy_cidrs=ips):
             LOG.debug("Failure adding BGP route for CR-LRP Port %s", ips)
             return False
         LOG.debug("Added BGP route for CR-LRP Port %s", ips)
 
+        # Expose FIPS
+        # This is needed in case the router get disabled and enabled
+        # In that case there may be FIPs already associated to VMs
+        fips, patch_port_row = self.sb_idl.get_cr_lrp_nat_addresses_info(
+            cr_lrp_port, self.chassis, self.sb_idl)
+        fips = [ip for ip in fips if ip not in ips_without_mask]
+        if fips:
+            self._expose_ip(fips, patch_port_row, associated_port=cr_lrp_port)
+
         # Check if there are networks attached to the router,
         # and if so, add the needed routes/rules
         lrp_ports = self.sb_idl.get_lrp_ports_for_router(router_datapath)
         for lrp in lrp_ports:
             self._process_lrp_port(lrp, cr_lrp_port)
 
         cr_lrp_provider_dp = self.ovn_local_cr_lrps[cr_lrp_port][
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers import driver_api
 from ovn_bgp_agent.drivers.openstack.utils import frr
 from ovn_bgp_agent.drivers.openstack.utils import ovn
 from ovn_bgp_agent.drivers.openstack.utils import ovs
 from ovn_bgp_agent.drivers.openstack.watchers import evpn_watcher as \
     watcher
+from ovn_bgp_agent.utils import helpers
 from ovn_bgp_agent.utils import linux_net
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 # LOG.setLevel(logging.DEBUG)
 # logging.basicConfig(level=logging.DEBUG)
@@ -123,16 +124,17 @@
         self._ovn_routing_tables_routes = collections.defaultdict()
         self._ovn_exposed_evpn_ips = collections.defaultdict()
 
         # 1) Get bridge mappings: xxxx:br-ex,yyyy:br-ex2
         bridge_mappings = self.ovs_idl.get_ovn_bridge_mappings()
         # 2) Get macs for bridge mappings
         for bridge_index, bridge_mapping in enumerate(bridge_mappings, 1):
-            network = bridge_mapping.split(":")[0]
-            bridge = bridge_mapping.split(":")[1]
+            network, bridge = helpers.parse_bridge_mapping(bridge_mapping)
+            if not network:
+                continue
             self.ovn_bridge_mappings[network] = bridge
 
             linux_net.ensure_arp_ndp_enabled_for_bridge(bridge, bridge_index)
 
         # TO DO
         # add missing routes/ips for fips/provider VMs
         ports = self.sb_idl.get_ports_on_chassis(self.chassis)
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from ovn_bgp_agent.drivers import driver_api
 from ovn_bgp_agent.drivers.openstack.utils import bgp as bgp_utils
 from ovn_bgp_agent.drivers.openstack.utils import driver_utils
 from ovn_bgp_agent.drivers.openstack.utils import frr
 from ovn_bgp_agent.drivers.openstack.utils import ovn
 from ovn_bgp_agent.drivers.openstack.utils import ovs
 from ovn_bgp_agent.drivers.openstack.watchers import bgp_watcher as watcher
+from ovn_bgp_agent import exceptions as agent_exc
 from ovn_bgp_agent.utils import linux_net
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 
 OVN_TABLES = ["Port_Binding", "Chassis", "Datapath_Binding"]
@@ -220,23 +221,33 @@
             # This address scope does not match => don't announce
             return False
 
         return True
 
     @lockutils.synchronized("bgp")
     def expose_subnet(self, ip, row):
-        cr_lrp = self.sb_idl.is_router_gateway_on_any_chassis(row.datapath)
+        try:
+            cr_lrp = self.sb_idl.is_router_gateway_on_any_chassis(row.datapath)
+        except agent_exc.DatapathNotFound:
+            LOG.debug("Port %s not being exposed as its datapath %s was "
+                      "removed", row.logical_port, row.datapath)
+            return
         if not cr_lrp:
             return
 
         self._ensure_network_exposed(row, cr_lrp.logical_port)
 
     @lockutils.synchronized("bgp")
     def update_subnet(self, old, row):
-        cr_lrp = self.sb_idl.is_router_gateway_on_any_chassis(row.datapath)
+        try:
+            cr_lrp = self.sb_idl.is_router_gateway_on_any_chassis(row.datapath)
+        except agent_exc.DatapathNotFound:
+            LOG.debug("Port %s not being updated as its datapath %s was "
+                      "removed", row.logical_port, row.datapath)
+            return
         if (not cr_lrp or not cr_lrp.mac or
                 len(cr_lrp.mac[0].strip().split(" ")) <= 1):
             return
 
         current_ips = row.mac[0].strip().split(" ")[1:]
         previous_ips = (
             old.mac[0].strip().split(" ")[1:]
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/bgp.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/bgp.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/driver_utils.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/driver_utils.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/frr.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/frr.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/ovn.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/ovn.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,23 @@
 
 
 class OvsdbNbOvnIdl(nb_impl_idl.OvnNbApiIdlImpl, Backend):
     def __init__(self, connection):
         super(OvsdbNbOvnIdl, self).__init__(connection)
         self.idl._session.reconnect.set_probe_interval(60000)
 
+    def get_network_vlan_tags(self):
+        tags = []
+        cmd = self.db_find_rows('Logical_Switch_Port', ('type', '=',
+                                constants.OVN_LOCALNET_VIF_PORT_TYPE))
+        for row in cmd.execute(check_error=True):
+            if row.tag:
+                tags.append(row.tag[0])
+        return tags
+
     def get_network_vlan_tag_by_network_name(self, network_name):
         tags = []
         cmd = self.db_find_rows('Logical_Switch_Port', ('type', '=',
                                 constants.OVN_LOCALNET_VIF_PORT_TYPE))
         for row in cmd.execute(check_error=True):
             if (row.tag and row.options and
                     row.options.get('network_name') == network_name):
@@ -336,14 +345,23 @@
         for row in self.get_ports_on_datapath(
                 datapath, constants.OVN_LOCALNET_VIF_PORT_TYPE):
             if (row.options and
                     row.options.get('network_name') in bridge_mappings):
                 return row.options.get('network_name'), row.tag
         return None, None
 
+    def get_network_vlan_tags(self):
+        tags = []
+        cmd = self.db_find_rows('Port_Binding', ('type', '=',
+                                constants.OVN_LOCALNET_VIF_PORT_TYPE))
+        for row in cmd.execute(check_error=True):
+            if row.tag:
+                tags.append(row.tag[0])
+        return tags
+
     def get_network_vlan_tag_by_network_name(self, network_name):
         tags = []
         cmd = self.db_find_rows('Port_Binding', ('type', '=',
                                 constants.OVN_LOCALNET_VIF_PORT_TYPE))
         for row in cmd.execute(check_error=True):
             if (row.tag and row.options and
                     row.options.get('network_name') == network_name):
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/ovs.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/ovs.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 # limitations under the License.
 
 from oslo_log import log as logging
 from ovs.db import idl
 from ovsdbapp.backend.ovs_idl import connection
 from ovsdbapp.backend.ovs_idl import idlutils
 from ovsdbapp.schema.open_vswitch import impl_idl as idl_ovs
-import pyroute2
+import tenacity
 
 from ovn_bgp_agent import constants
+from ovn_bgp_agent import exceptions as agent_exc
 import ovn_bgp_agent.privileged.ovs_vsctl
 from ovn_bgp_agent.utils import linux_net
 
 LOG = logging.getLogger(__name__)
 
 
 def _find_ovs_port(bridge):
@@ -58,18 +59,32 @@
     for ovs_port in ovs_ports.split("\n"):
         if ovs_port.startswith('patch-provnet-'):
             ovs_ofport = get_device_port_at_ovs(ovs_port)
             in_ports.append(ovs_ofport)
     return in_ports
 
 
+@tenacity.retry(
+    retry=tenacity.retry_if_exception_type(agent_exc.PatchPortNotFound),
+    wait=tenacity.wait_fixed(1),
+    stop=tenacity.stop_after_delay(5),
+    reraise=True)
 def get_ovs_patch_port_ofport(patch):
     patch_name = "patch-{}-to-br-int".format(patch)
-    ofport = ovn_bgp_agent.privileged.ovs_vsctl.ovs_cmd(
-        'ovs-vsctl', ['get', 'Interface', patch_name, 'ofport'])[0].rstrip()
+    try:
+        ofport = ovn_bgp_agent.privileged.ovs_vsctl.ovs_cmd(
+            'ovs-vsctl', ['get', 'Interface', patch_name, 'ofport']
+            )[0].rstrip()
+    except Exception:
+        raise agent_exc.PatchPortNotFound(localnet=patch)
+    if ofport == '[]':
+        # NOTE(ltomasbo): there is a chance the patch port interface was
+        # created but not yet added to ovs bridge, therefore it exists but
+        # has an empty ofport. We should retry in this case
+        raise agent_exc.PatchPortNotFound(localnet=patch)
     return ofport
 
 
 def ensure_mac_tweak_flows(bridge, mac, ports, cookie):
     cookie_id = "cookie={}/-1".format(cookie)
     current_flows = get_bridge_flows(bridge, cookie_id)
     flows_info = [flow.split("priority")[1].replace(" ", ",")
@@ -124,29 +139,27 @@
     if not ovs_port:
         return
     ovs_ofport = get_device_port_at_ovs(ovs_port)
     vrf_ofport = get_device_port_at_ovs(output_port)
 
     strip_vlan_opt = 'strip_vlan,' if strip_vlan else ''
     ip_version = linux_net.get_ip_version(net)
-    with pyroute2.NDB() as ndb:
-        if ip_version == constants.IP_VERSION_6:
-            flow = (
-                "cookie={},priority=1000,ipv6,in_port={},dl_src:{},"
-                "ipv6_src={} actions=mod_dl_dst:{},{}output={}".format(
-                    cookie, ovs_ofport, mac, net,
-                    ndb.interfaces[port_dst]['address'], strip_vlan_opt,
-                    vrf_ofport))
-        else:
-            flow = (
-                "cookie={},priority=1000,ip,in_port={},dl_src:{},nw_src={}"
-                "actions=mod_dl_dst:{},{}output={}".format(
-                    cookie, ovs_ofport, mac, net,
-                    ndb.interfaces[port_dst]['address'], strip_vlan_opt,
-                    vrf_ofport))
+    port_dst_mac = linux_net.get_interface_address(port_dst)
+    if ip_version == constants.IP_VERSION_6:
+        flow = (
+            "cookie={},priority=1000,ipv6,in_port={},dl_src:{},"
+            "ipv6_src={} actions=mod_dl_dst:{},{}output={}".format(
+                cookie, ovs_ofport, mac, net, port_dst_mac, strip_vlan_opt,
+                vrf_ofport))
+    else:
+        flow = (
+            "cookie={},priority=1000,ip,in_port={},dl_src:{},nw_src={}"
+            "actions=mod_dl_dst:{},{}output={}".format(
+                cookie, ovs_ofport, mac, net, port_dst_mac, strip_vlan_opt,
+                vrf_ofport))
     ovn_bgp_agent.privileged.ovs_vsctl.ovs_cmd(
         'ovs-ofctl', ['add-flow', bridge, flow])
 
 
 def remove_evpn_router_ovs_flows(bridge, cookie, mac):
     ovs_port = _find_ovs_port(bridge)
     if not ovs_port:
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/utils/wire.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/utils/wire.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import pyroute2
-
 from oslo_config import cfg
 from oslo_log import log as logging
-import tenacity
 
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack.utils import ovs
 from ovn_bgp_agent import exceptions as agent_exc
+from ovn_bgp_agent.utils import helpers
 from ovn_bgp_agent.utils import linux_net
 
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 
 
@@ -36,53 +34,52 @@
         raise NotImplementedError()
 
 
 def _ensure_base_wiring_config_underlay(idl, bridge_mappings, routing_tables):
     ovn_bridge_mappings = {}
     flows_info = {}
     for bridge_index, bridge_mapping in enumerate(bridge_mappings, 1):
-        network = bridge_mapping.split(":")[0]
-        bridge = bridge_mapping.split(":")[1]
+        network, bridge = helpers.parse_bridge_mapping(bridge_mapping)
+        if not network:
+            continue
         ovn_bridge_mappings[network] = bridge
 
         linux_net.ensure_routing_table_for_bridge(
             routing_tables, bridge, CONF.bgp_vrf_table_id)
         vlan_tags = idl.get_network_vlan_tag_by_network_name(network)
 
         for vlan_tag in vlan_tags:
             linux_net.ensure_vlan_device_for_network(bridge,
                                                      vlan_tag)
 
         linux_net.ensure_arp_ndp_enabled_for_bridge(bridge,
                                                     bridge_index,
                                                     vlan_tags)
         if not flows_info.get(bridge):
-            with pyroute2.NDB() as ndb:
-                flows_info[bridge] = {
-                    'mac': ndb.interfaces[bridge]['address'],
-                    'in_port': set([])}
+            mac = linux_net.get_interface_address(bridge)
+            flows_info[bridge] = {'mac': mac, 'in_port': set([])}
             flows_info[bridge]['in_port'] = ovs.get_ovs_patch_ports_info(
                 bridge)
-            ovs.ensure_mac_tweak_flows(bridge, flows_info[bridge]['mac'],
+            ovs.ensure_mac_tweak_flows(bridge, mac,
                                        flows_info[bridge]['in_port'],
                                        constants.OVS_RULE_COOKIE)
     return ovn_bridge_mappings, flows_info
 
 
-def cleanup_wiring(bridge_mappings, ovs_flows, exposed_ips, routing_tables,
-                   routing_tables_routes):
+def cleanup_wiring(idl, bridge_mappings, ovs_flows, exposed_ips,
+                   routing_tables, routing_tables_routes):
     if CONF.exposing_method == constants.EXPOSE_METHOD_UNDERLAY:
-        return _cleanup_wiring_underlay(bridge_mappings, ovs_flows,
+        return _cleanup_wiring_underlay(idl, bridge_mappings, ovs_flows,
                                         exposed_ips, routing_tables,
                                         routing_tables_routes)
     elif CONF.exposing_method == constants.EXPOSE_METHOD_OVN:
         raise NotImplementedError()
 
 
-def _cleanup_wiring_underlay(bridge_mappings, ovs_flows, exposed_ips,
+def _cleanup_wiring_underlay(idl, bridge_mappings, ovs_flows, exposed_ips,
                              routing_tables, routing_tables_routes):
     current_ips = linux_net.get_exposed_ips(CONF.bgp_nic)
     expected_ips = [ip for ip_dict in exposed_ips.values()
                     for ip in ip_dict.keys()]
 
     ips_to_delete = [ip for ip in current_ips if ip not in expected_ips]
     linux_net.delete_exposed_ips(ips_to_delete, CONF.bgp_nic)
@@ -108,14 +105,27 @@
             ovn_ip_rules.pop(ip_dst, None)
     linux_net.delete_ip_rules(ovn_ip_rules)
 
     # remove all the extra routes not needed
     linux_net.delete_bridge_ip_routes(routing_tables, routing_tables_routes,
                                       extra_routes)
 
+    # delete leaked vlan devices from previous vlan provider networks
+    delete_vlan_devices_leftovers(idl, bridge_mappings)
+
+
+def delete_vlan_devices_leftovers(idl, bridge_mappings):
+    vlan_tags = idl.get_network_vlan_tags()
+    ovs_devices = set(bridge_mappings.values())
+    for ovs_device in ovs_devices:
+        vlans = linux_net.get_bridge_vlans(ovs_device)
+        for vlan in vlans:
+            if vlan and vlan not in vlan_tags:
+                linux_net.delete_vlan_device_for_network(ovs_device, vlan)
+
 
 def wire_provider_port(routing_tables_routes, ovs_flows, port_ips,
                        bridge_device, bridge_vlan, localnet, routing_table,
                        proxy_cidrs, lladdr=None):
     if CONF.exposing_method == constants.EXPOSE_METHOD_UNDERLAY:
         return _wire_provider_port_underlay(routing_tables_routes, ovs_flows,
                                             port_ips, bridge_device,
@@ -135,24 +145,16 @@
                                               routing_table, proxy_cidrs,
                                               lladdr=lladdr)
     elif CONF.exposing_method == constants.EXPOSE_METHOD_OVN:
         # No need to wire anything
         return True
 
 
-@tenacity.retry(
-    retry=tenacity.retry_if_exception_type(agent_exc.PatchPortNotFound),
-    wait=tenacity.wait_fixed(0.5),
-    stop=tenacity.stop_after_delay(5),
-    reraise=True)
 def _ensure_updated_mac_tweak_flows(localnet, bridge_device, ovs_flows):
-    try:
-        ofport = ovs.get_ovs_patch_port_ofport(localnet)
-    except Exception:
-        raise agent_exc.PatchPortNotFound(localnet=localnet)
+    ofport = ovs.get_ovs_patch_port_ofport(localnet)
     if ofport not in ovs_flows[bridge_device]['in_port']:
         ovs_flows[bridge_device]['in_port'].append(ofport)
         ovs.ensure_mac_tweak_flows(bridge_device,
                                    ovs_flows[bridge_device]['mac'],
                                    [ofport],
                                    constants.OVS_RULE_COOKIE)
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,39 +8,52 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from oslo_log import log as logging
+
 from ovsdbapp.backend.ovs_idl import event as row_event
 
+LOG = logging.getLogger(__name__)
+
+
+class Event(row_event.RowEvent):
+    def run(self, *args, **kwargs):
+        try:
+            self._run(*args, **kwargs)
+        except Exception:
+            LOG.exception("Unexpected exception while running the event "
+                          "action")
+
 
-class PortBindingChassisEvent(row_event.RowEvent):
+class PortBindingChassisEvent(Event):
     def __init__(self, bgp_agent, events):
         self.agent = bgp_agent
         table = 'Port_Binding'
         super(PortBindingChassisEvent, self).__init__(
             events, table, None)
         self.event_name = self.__class__.__name__
 
     def _check_ip_associated(self, mac):
         return len(mac.strip().split(' ')) > 1
 
 
-class OVNLBMemberEvent(row_event.RowEvent):
+class OVNLBMemberEvent(Event):
     def __init__(self, bgp_agent, events):
         self.agent = bgp_agent
         table = 'Load_Balancer'
         super(OVNLBMemberEvent, self).__init__(
             events, table, None)
         self.event_name = self.__class__.__name__
 
 
-class LSPChassisEvent(row_event.RowEvent):
+class LSPChassisEvent(Event):
     def __init__(self, bgp_agent, events):
         self.agent = bgp_agent
         table = 'Logical_Switch_Port'
         super(LSPChassisEvent, self).__init__(
             events, table, None)
         self.event_name = self.__class__.__name__
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from oslo_concurrency import lockutils
 from oslo_config import cfg
 from oslo_log import log as logging
 
-from ovsdbapp.backend.ovs_idl import event as row_event
-
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack.watchers import base_watcher
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 _SYNC_STATE_LOCK = lockutils.ReaderWriterLock()
 
@@ -33,20 +31,29 @@
             bgp_agent, events)
 
     def match_fn(self, event, row, old):
         try:
             # single and dual-stack format
             if not self._check_ip_associated(row.mac[0]):
                 return False
-            return (row.chassis[0].name == self.agent.chassis and
-                    (not old.chassis or row.chassis != old.chassis))
+            if not bool(row.up[0]):
+                return False
+
+            if row.chassis[0].name != self.agent.chassis:
+                return False
+            if hasattr(old, 'chassis'):
+                if not old.chassis or row.chassis != old.chassis:
+                    return True
+            if hasattr(old, 'up'):
+                if not bool(old.up[0]):
+                    return True
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in constants.OVN_VIF_PORT_TYPES:
             return
         with _SYNC_STATE_LOCK.read_lock():
             ips = row.mac[0].split(' ')[1:]
             self.agent.expose_ip(ips, row)
 
 
@@ -57,23 +64,28 @@
             bgp_agent, events)
 
     def match_fn(self, event, row, old):
         try:
             # single and dual-stack format
             if not self._check_ip_associated(row.mac[0]):
                 return False
-            if event == self.ROW_UPDATE:
-                return (old.chassis[0].name == self.agent.chassis and
-                        (not row.chassis or row.chassis != old.chassis))
-            else:
+            if event == self.ROW_DELETE:
                 return row.chassis[0].name == self.agent.chassis
+
+            if hasattr(old, 'chassis'):
+                if (old.chassis[0].name == self.agent.chassis and
+                        (not row.chassis or row.chassis != old.chassis)):
+                    return True
+            if hasattr(old, 'up'):
+                if bool(old.up[0]) and not bool(row.up[0]):
+                    return True
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in constants.OVN_VIF_PORT_TYPES:
             return
         with _SYNC_STATE_LOCK.read_lock():
             ips = row.mac[0].split(' ')[1:]
             self.agent.withdraw_ip(ips, row)
 
 
@@ -87,15 +99,15 @@
         try:
             return (not row.chassis and
                     row.nat_addresses != old.nat_addresses and
                     not row.logical_port.startswith('lrp-'))
         except (AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_PATCH_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             # NOTE(ltomasbo): nat_addresses has the same format, where
             # different IPs can be present:
             # ["fa:16:3e:77:7f:9c 172.24.100.229 172.24.100.112
             #  is_chassis_resident(\"
@@ -125,15 +137,15 @@
         try:
             return (not row.chassis and
                     row.nat_addresses != old.nat_addresses and
                     not row.logical_port.startswith('lrp-'))
         except (AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_PATCH_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             # NOTE(ltomasbo): nat_addresses has the same format, where
             # different IPs can be present:
             # ["fa:16:3e:77:7f:9c 172.24.100.229 172.24.100.112
             #  is_chassis_resident(\"
@@ -167,15 +179,15 @@
                 return False
             return (not row.chassis and
                     row.logical_port.startswith('lrp-') and
                     "chassis-redirect-port" not in row.options.keys())
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_PATCH_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             ip_address = row.mac[0].split(' ')[1]
             self.agent.expose_subnet(ip_address, row)
 
 
@@ -202,15 +214,15 @@
                 row.logical_port.startswith("lrp-") and
                 "chassis-redirect-port" not in row.options.keys() and
                 old.mac != row.mac
             )
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_PATCH_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             self.agent.update_subnet(old, row)
 
 
 class SubnetRouterDetachedEvent(base_watcher.PortBindingChassisEvent):
@@ -226,15 +238,15 @@
                 return False
             return (not row.chassis and
                     row.logical_port.startswith('lrp-') and
                     "chassis-redirect-port" not in row.options.keys())
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_PATCH_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             ip_address = row.mac[0].split(' ')[1]
             self.agent.withdraw_subnet(ip_address, row)
 
 
@@ -256,15 +268,15 @@
             elif not self._check_ip_associated(row.mac[0]):
                 return False
             return (not old.chassis and row.chassis and
                     self.agent.ovn_local_lrps != [])
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in (constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE):
             return
         with _SYNC_STATE_LOCK.read_lock():
             if row.mac == ['unknown']:
                 # Handling the case for unknown MACs when configdrive is used
                 # instead of dhcp
@@ -296,15 +308,15 @@
                 return (old.chassis and not row.chassis and
                         self.agent.ovn_local_lrps != [])
             if event == self.ROW_DELETE:
                 return (self.agent.ovn_local_lrps != [])
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in (constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE):
             return
         if event == self.ROW_UPDATE:
             chassis = old.chassis
         else:
             chassis = row.chassis
@@ -333,15 +345,15 @@
             # it should not have mac, no chassis, and status down
             if not row.mac and not row.chassis and not row.up[0]:
                 return bool(self.agent.ovn_local_cr_lrps)
             return False
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_VM_VIF_PORT_TYPE:
             return
 
         with _SYNC_STATE_LOCK.read_lock():
             # This is depending on the external-id information added by
             # neutron, regarding the neutron:cidrs
             ext_n_cidr = row.external_ids.get(constants.OVN_CIDRS_EXT_ID_KEY)
@@ -361,15 +373,15 @@
         super(OVNLBMemberCreateEvent, self).__init__(
             bgp_agent, events)
 
     def match_fn(self, event, row, old):
         # Only process event if the local node has a cr-lrp ports associated
         return bool(self.agent.ovn_local_cr_lrps)
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         # Only process event if the local node has a cr-lrp port whose provider
         # datapath is included into the loadbalancer. This means the
         # loadbalancer has the VIP on a provider network
         # Also, the cr-lrp port needs to have subnet datapaths (LS) associated
         # to it that include the load balancer
         if not self.agent.ovn_local_cr_lrps:
             return
@@ -434,15 +446,15 @@
         super(OVNLBMemberDeleteEvent, self).__init__(
             bgp_agent, events)
 
     def match_fn(self, event, row, old):
         # Only process event if the local node has the lb exported
         return bool(self.agent.provider_ovn_lbs.get(row.name))
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         associated_cr_lrp_port = self.agent.provider_ovn_lbs[row.name].get(
             'gateway_port')
         if not associated_cr_lrp_port:
             # Something is wrong, not enough information to proceed
             return
         with _SYNC_STATE_LOCK.read_lock():
             # loadbalancer deleted. Withdraw the VIP through the cr-lrp
@@ -455,31 +467,31 @@
         events = (self.ROW_CREATE, self.ROW_DELETE,)
         super(LocalnetCreateDeleteEvent, self).__init__(
             bgp_agent, events)
 
     def match_fn(self, event, row, old):
         return row.type == constants.OVN_LOCALNET_VIF_PORT_TYPE
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         with _SYNC_STATE_LOCK.read_lock():
             self.agent.sync()
 
 
-class ChassisCreateEventBase(row_event.RowEvent):
+class ChassisCreateEventBase(base_watcher.Event):
     table = None
 
     def __init__(self, bgp_agent):
         self.agent = bgp_agent
         self.first_time = True
         events = (self.ROW_CREATE,)
         super(ChassisCreateEventBase, self).__init__(
             events, self.table, (('name', '=', self.agent.chassis),))
         self.event_name = self.__class__.__name__
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if self.first_time:
             self.first_time = False
         else:
             LOG.info("Connection to OVSDB established, doing a full sync")
             self.agent.sync()
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from oslo_concurrency import lockutils
 from oslo_log import log as logging
-from ovsdbapp.backend.ovs_idl import event as row_event
 
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack.watchers import base_watcher
 
 
 LOG = logging.getLogger(__name__)
 
@@ -39,15 +38,15 @@
             if not self._check_ip_associated(row.mac[0]):
                 return False
             return (row.chassis[0].name == self.agent.chassis and
                     not old.chassis)
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_CHASSISREDIRECT_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             self.agent.expose_ip(row, cr_lrp=True)
 
 
 class PortBindingChassisDeletedEvent(base_watcher.PortBindingChassisEvent):
@@ -67,15 +66,15 @@
                 return (old.chassis[0].name == self.agent.chassis and
                         not row.chassis)
             else:
                 return row.chassis[0].name == self.agent.chassis
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_CHASSISREDIRECT_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             self.agent.withdraw_ip(row, cr_lrp=True)
 
 
 class SubnetRouterAttachedEvent(base_watcher.PortBindingChassisEvent):
@@ -99,15 +98,15 @@
                 return (not row.chassis and
                         not row.logical_port.startswith('lrp-') and
                         row.external_ids[constants.OVN_EVPN_VNI_EXT_ID_KEY] and
                         row.external_ids[constants.OVN_EVPN_AS_EXT_ID_KEY])
         except (IndexError, AttributeError, KeyError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_PATCH_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             if row.nat_addresses:
                 self.agent.expose_ip(row)
             else:
                 self.agent.expose_subnet(row)
@@ -134,15 +133,15 @@
                 return (not row.chassis and
                         not row.logical_port.startswith('lrp-') and
                         row.external_ids[constants.OVN_EVPN_VNI_EXT_ID_KEY] and
                         row.external_ids[constants.OVN_EVPN_AS_EXT_ID_KEY])
         except (IndexError, AttributeError, KeyError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type != constants.OVN_PATCH_VIF_PORT_TYPE:
             return
         with _SYNC_STATE_LOCK.read_lock():
             if row.nat_addresses:
                 self.agent.withdraw_ip(row)
             else:
                 self.agent.withdraw_subnet(row)
@@ -160,15 +159,15 @@
             if not self._check_ip_associated(row.mac[0]):
                 return False
             return (not old.chassis and row.chassis and
                     self.agent.ovn_local_lrps != [])
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in (constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE):
             return
         with _SYNC_STATE_LOCK.read_lock():
             ips = row.mac[0].split(' ')[1:]
             self.agent.expose_remote_ip(ips, row)
 
@@ -188,15 +187,15 @@
                 return (old.chassis and not row.chassis and
                         self.agent.ovn_local_lrps != [])
             else:
                 return (self.agent.ovn_local_lrps != [])
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in (constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE):
             return
         with _SYNC_STATE_LOCK.read_lock():
             ips = row.mac[0].split(' ')[1:]
             self.agent.withdraw_remote_ip(ips, row)
 
@@ -206,31 +205,31 @@
         events = (self.ROW_CREATE, self.ROW_DELETE,)
         super(LocalnetCreateDeleteEvent, self).__init__(
             bgp_agent, events)
 
     def match_fn(self, event, row, old):
         return row.type == constants.OVN_LOCALNET_VIF_PORT_TYPE
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         with _SYNC_STATE_LOCK.read_lock():
             self.agent.sync()
 
 
-class ChassisCreateEventBase(row_event.RowEvent):
+class ChassisCreateEventBase(base_watcher.Event):
     table = None
 
     def __init__(self, bgp_agent):
         self.agent = bgp_agent
         self.first_time = True
         events = (self.ROW_CREATE,)
         super(ChassisCreateEventBase, self).__init__(
             events, self.table, (('name', '=', self.agent.chassis),))
         self.event_name = self.__class__.__name__
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if self.first_time:
             self.first_time = False
         else:
             LOG.info("Connection to OVSDB established, doing a full sync")
             self.agent.sync()
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,24 +34,28 @@
             # single and dual-stack format
             if not self._check_ip_associated(row.addresses[0]):
                 return False
 
             current_chassis = row.options.get(constants.OVN_REQUESTED_CHASSIS)
             if current_chassis != self.agent.chassis:
                 return False
-            if not row.up:
+            if not bool(row.up[0]):
                 return False
-            old_chassis = old.options.get(constants.OVN_REQUESTED_CHASSIS)
-            if (not old_chassis or current_chassis != old_chassis or
-                    not old.up):
-                return True
+
+            if hasattr(old, 'options'):
+                old_chassis = old.options.get(constants.OVN_REQUESTED_CHASSIS)
+                if not old_chassis or current_chassis != old_chassis:
+                    return True
+            if hasattr(old, 'up'):
+                if not bool(old.up[0]):
+                    return True
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in [constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE]:
             return
         with _SYNC_STATE_LOCK.read_lock():
             ips = row.addresses[0].split(' ')[1:]
             self.agent.expose_ip(ips, row)
 
@@ -78,22 +82,22 @@
                 old_chassis = old.options.get(constants.OVN_REQUESTED_CHASSIS)
                 if old_chassis != self.agent.chassis:
                     return False
                 if not current_chassis or current_chassis != old_chassis:
                     return True
 
             if hasattr(old, 'up'):
-                if not old.up:
+                if not bool(old.up[0]):
                     return False
-                if not row.up:
+                if not bool(row.up[0]):
                     return True
         except (IndexError, AttributeError):
             return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in [constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE]:
             return
         with _SYNC_STATE_LOCK.read_lock():
             ips = row.addresses[0].split(' ')[1:]
             self.agent.withdraw_ip(ips, row)
 
@@ -109,15 +113,15 @@
             # single and dual-stack format
             if not self._check_ip_associated(row.addresses[0]):
                 return False
 
             current_chassis = row.options.get(constants.OVN_REQUESTED_CHASSIS)
             current_port_fip = row.external_ids.get(
                 constants.OVN_FIP_EXT_ID_KEY)
-            if (current_chassis != self.agent.chassis or not row.up or
+            if (current_chassis != self.agent.chassis or not bool(row.up[0]) or
                     not current_port_fip):
                 return False
 
             if hasattr(old, 'options'):
                 # check chassis change
                 old_chassis = old.options.get(constants.OVN_REQUESTED_CHASSIS)
                 if not old_chassis or current_chassis != old_chassis:
@@ -126,21 +130,21 @@
                 # check fips addition
                 old_port_fip = old.external_ids.get(
                     constants.OVN_FIP_EXT_ID_KEY)
                 if not old_port_fip or current_port_fip != old_port_fip:
                     return True
             if hasattr(old, 'up'):
                 # check port status change
-                if not old.up:
+                if not bool(old.up[0]):
                     return True
         except (IndexError, AttributeError):
             return False
         return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in [constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE]:
             return
         external_ip, ls_name = self.agent.get_port_external_ip_and_ls(row.name)
         if not external_ip or not ls_name:
             return
 
@@ -160,16 +164,16 @@
             if not self._check_ip_associated(row.addresses[0]):
                 return False
 
             current_chassis = row.options.get(constants.OVN_REQUESTED_CHASSIS)
             current_port_fip = row.external_ids.get(
                 constants.OVN_FIP_EXT_ID_KEY)
             if event == self.ROW_DELETE:
-                if (current_chassis == self.agent.chassis and row.up and
-                        current_port_fip):
+                if (current_chassis == self.agent.chassis and
+                        bool(row.up[0]) and current_port_fip):
                     return True
                 return False
 
             if hasattr(old, 'options'):
                 # check chassis change
                 old_chassis = old.options.get(constants.OVN_REQUESTED_CHASSIS)
                 if (not old_chassis or old_chassis != self.agent.chassis):
@@ -186,23 +190,23 @@
                     constants.OVN_FIP_EXT_ID_KEY)
                 if not old_port_fip:
                     return False
                 if old_port_fip != current_port_fip:
                     return True
             if hasattr(old, 'up'):
                 # check port status change
-                if not old.up:
+                if not bool(old.up[0]):
                     return False
-                if not row.up and current_port_fip:
+                if not bool(row.up[0]) and current_port_fip:
                     return True
         except (IndexError, AttributeError):
             return False
         return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         if row.type not in [constants.OVN_VM_VIF_PORT_TYPE,
                             constants.OVN_VIRTUAL_VIF_PORT_TYPE]:
             return
         fip = row.external_ids.get(constants.OVN_FIP_EXT_ID_KEY)
         if not fip:
             fip = old.external_ids.get(constants.OVN_FIP_EXT_ID_KEY)
         if not fip:
@@ -218,10 +222,10 @@
             bgp_agent, events)
 
     def match_fn(self, event, row, old):
         if row.type == constants.OVN_LOCALNET_VIF_PORT_TYPE:
             return True
         return False
 
-    def run(self, event, row, old):
+    def _run(self, event, row, old):
         with _SYNC_STATE_LOCK.read_lock():
             self.agent.sync()
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/__init__.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/__init__.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/ovs_vsctl.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/ovs_vsctl.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/privileged/vtysh.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/privileged/vtysh.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/base.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/cmd/test_agent.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-# -*- coding: utf-8 -*-
-
-# Copyright 2010-2011 OpenStack Foundation
-# Copyright (c) 2013 Hewlett-Packard Development Company, L.P.
+# Copyright 2021 Red Hat, Inc.
 #
-# Licensed under the Apache License, Version 2.0 (the "License"); you may
-# not use this file except in compliance with the License. You may obtain
-# a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
-#      http://www.apache.org/licenses/LICENSE-2.0
+#   http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-# WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-# License for the specific language governing permissions and limitations
-# under the License.
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
-from unittest import mock
 
-from oslotest import base
+from unittest import mock
 
+from ovn_bgp_agent.tests import base as test_base
 
-class TestCase(base.BaseTestCase):
 
-    """Test case base class for all unit tests."""
+class TestAgentCmd(test_base.TestCase):
+    @mock.patch('ovn_bgp_agent.agent.start')
+    def test_start(self, m_start):
+        from ovn_bgp_agent.cmd import agent  # To make it import a mock.
+        agent.start()
 
-    def setUp(self):
-        super(TestCase, self).setUp()
-        self.addCleanup(mock.patch.stopall)
+        m_start.assert_called()
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/test_ovn_bgp_agent.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/test_ovn_bgp_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/cmd/test_agent.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/test_agent.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,33 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 from unittest import mock
 
+from ovn_bgp_agent import agent
 from ovn_bgp_agent.tests import base as test_base
 
 
-class TestAgentCmd(test_base.TestCase):
-    @mock.patch('ovn_bgp_agent.agent.start')
-    def test_start(self, m_start):
-        from ovn_bgp_agent.cmd import agent  # To make it import a mock.
+class TestAgent(test_base.TestCase):
+
+    @mock.patch('oslo_service.service.launch')
+    @mock.patch('ovn_bgp_agent.config.register_opts')
+    @mock.patch('ovn_bgp_agent.config.init')
+    @mock.patch('ovn_bgp_agent.config.setup_logging')
+    @mock.patch('ovn_bgp_agent.agent.BGPAgent')
+    def test_start(self, m_agent, m_setup_logging, m_config_init,
+                   m_register_opts, m_oslo_launch):
+        m_launcher = mock.Mock()
+        m_oslo_launch.return_value = m_launcher
+
         agent.start()
 
-        m_start.assert_called()
+        m_register_opts.assert_called()
+        m_config_init.assert_called()
+        m_setup_logging.assert_called()
+        m_agent.assert_called()
+        m_oslo_launch.assert_called()
+        m_launcher.wait.assert_called()
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from unittest import mock
 
 from oslo_config import cfg
 
-from ovn_bgp_agent import config
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack import nb_ovn_bgp_driver
 from ovn_bgp_agent.drivers.openstack.utils import bgp as bgp_utils
 from ovn_bgp_agent.drivers.openstack.utils import frr
 from ovn_bgp_agent.drivers.openstack.utils import ovn
 from ovn_bgp_agent.drivers.openstack.utils import ovs
 from ovn_bgp_agent.drivers.openstack.utils import wire as wire_utils
@@ -32,15 +31,14 @@
 CONF = cfg.CONF
 
 
 class TestNBOVNBGPDriver(test_base.TestCase):
 
     def setUp(self):
         super(TestNBOVNBGPDriver, self).setUp()
-        config.register_opts()
         self.bridge = 'fake-bridge'
         self.nb_bgp_driver = nb_ovn_bgp_driver.NBOVNBGPDriver()
         self.nb_bgp_driver._post_start_event = mock.Mock()
         self.nb_bgp_driver.nb_idl = mock.Mock()
         self.nb_idl = self.nb_bgp_driver.nb_idl
         self.nb_bgp_driver.chassis = 'fake-chassis'
         self.nb_bgp_driver.ovn_bridge_mappings = {'fake-network': self.bridge}
@@ -60,18 +58,14 @@
         self.nb_bgp_driver.ovn_routing_tables = self.ovn_routing_tables
         self.ovn_routing_tables_routes = mock.Mock()
         self.nb_bgp_driver.ovn_routing_tables_routes = (
             self.ovn_routing_tables_routes)
 
         self.conf_ovsdb_connection = 'tcp:127.0.0.1:6642'
 
-        # Mock pyroute2.NDB context manager object
-        self.mock_ndb = mock.patch.object(linux_net.pyroute2, 'NDB').start()
-        self.fake_ndb = self.mock_ndb().__enter__()
-
     @mock.patch.object(linux_net, 'ensure_vrf')
     @mock.patch.object(frr, 'vrf_leak')
     @mock.patch.object(linux_net, 'ensure_ovn_device')
     @mock.patch.object(linux_net, 'delete_routes_from_table')
     def test_start(self, mock_delete_routes_from_table,
                    mock_ensure_ovn_device, mock_vrf_leak, mock_ensure_vrf):
         CONF.set_override('clear_vrf_routes_on_startup', True)
@@ -110,31 +104,35 @@
             CONF.bgp_vrf, CONF.bgp_vrf_table_id)
         mock_vrf_leak.assert_called_once_with(
             CONF.bgp_vrf, CONF.bgp_AS, CONF.bgp_router_id,
             template=frr.LEAK_VRF_TEMPLATE)
         mock_ensure_ovn_dev.assert_called_once_with(
             CONF.bgp_nic, CONF.bgp_vrf)
 
+    @mock.patch.object(linux_net, 'delete_vlan_device_for_network')
+    @mock.patch.object(linux_net, 'get_bridge_vlans')
     @mock.patch.object(linux_net, 'get_extra_routing_table_for_bridge')
     @mock.patch.object(linux_net, 'delete_bridge_ip_routes')
     @mock.patch.object(linux_net, 'delete_ip_rules')
     @mock.patch.object(linux_net, 'delete_exposed_ips')
     @mock.patch.object(linux_net, 'get_ovn_ip_rules')
     @mock.patch.object(linux_net, 'get_exposed_ips')
     @mock.patch.object(ovs, 'remove_extra_ovs_flows')
     @mock.patch.object(ovs, 'ensure_mac_tweak_flows')
     @mock.patch.object(ovs, 'get_ovs_patch_ports_info')
+    @mock.patch.object(linux_net, 'get_interface_address')
     @mock.patch.object(linux_net, 'ensure_arp_ndp_enabled_for_bridge')
     @mock.patch.object(linux_net, 'ensure_vlan_device_for_network')
     @mock.patch.object(linux_net, 'ensure_routing_table_for_bridge')
     def test_sync(self, mock_routing_bridge, mock_ensure_vlan_network,
-                  mock_ensure_arp, mock_get_patch_ports, mock_ensure_mac,
-                  mock_remove_flows, mock_exposed_ips, mock_get_ip_rules,
-                  mock_del_exposed_ips, mock_del_ip_rules, mock_del_ip_routes,
-                  mock_get_extra_route):
+                  mock_ensure_arp, mock_nic_address, mock_get_patch_ports,
+                  mock_ensure_mac, mock_remove_flows, mock_exposed_ips,
+                  mock_get_ip_rules, mock_del_exposed_ips, mock_del_ip_rules,
+                  mock_del_ip_routes, mock_get_extra_route,
+                  mock_get_bridge_vlans, mock_delete_vlan_dev):
         self.mock_ovs_idl.get_ovn_bridge_mappings.return_value = [
             'net0:bridge0', 'net1:bridge1']
         self.nb_idl.get_network_vlan_tag_by_network_name.side_effect = (
             [10], [11])
         fake_ip_rules = 'fake-ip-rules'
         mock_get_ip_rules.return_value = fake_ip_rules
         ips = [self.ipv4, self.ipv6]
@@ -147,16 +145,20 @@
             'name': 'port-1',
             'type': constants.OVN_CHASSISREDIRECT_VIF_PORT_TYPE})
         self.nb_idl.get_active_ports_on_chassis.return_value = [
             port0, port1]
         mock_ensure_port_exposed = mock.patch.object(
             self.nb_bgp_driver, '_ensure_port_exposed').start()
         mock_routing_bridge.return_value = ['fake-route']
+        mock_nic_address.return_value = self.mac
         mock_get_patch_ports.return_value = [1, 2]
 
+        self.nb_idl.get_network_vlan_tags.return_value = [10, 11]
+        mock_get_bridge_vlans.side_effect = [[10, 12], [11]]
+
         self.nb_bgp_driver.sync()
 
         expected_calls = [mock.call({}, 'bridge0', CONF.bgp_vrf_table_id),
                           mock.call({}, 'bridge1', CONF.bgp_vrf_table_id)]
         mock_routing_bridge.assert_has_calls(expected_calls)
         expected_calls = [mock.call('bridge0', 10), mock.call('bridge1', 11)]
         mock_ensure_vlan_network.assert_has_calls(expected_calls)
@@ -177,14 +179,17 @@
         mock_get_ip_rules.assert_called_once()
         mock_ensure_port_exposed.assert_called_once_with(port0)
         mock_del_exposed_ips.assert_called_once_with(
             ips, CONF.bgp_nic)
         mock_del_ip_rules.assert_called_once_with(fake_ip_rules)
         mock_del_ip_routes.assert_called_once()
 
+        bridge = set(self.nb_bgp_driver.ovn_bridge_mappings.values()).pop()
+        mock_delete_vlan_dev.assert_called_once_with(bridge, 12)
+
     def test__ensure_port_exposed_fip(self):
         port0 = fakes.create_object({
             'name': 'port-0',
             'external_ids': {constants.OVN_FIP_EXT_ID_KEY: "fip"}})
 
         mock_get_port_external_ip_and_ls = mock.patch.object(
             self.nb_bgp_driver, 'get_port_external_ip_and_ls').start()
@@ -330,14 +335,15 @@
 
     def _test_expose_ip(self, ips, row):
         mock_expose_provider_port = mock.patch.object(
             self.nb_bgp_driver, '_expose_provider_port').start()
         mock_get_ls_localnet_info = mock.patch.object(
             self.nb_bgp_driver, '_get_ls_localnet_info').start()
         mock_get_ls_localnet_info.return_value = ('fake-localnet', 'br-ex', 10)
+        self.nb_bgp_driver.ovn_bridge_mappings = {'fake-localnet': 'br-ex'}
 
         cidr = row.external_ids.get(constants.OVN_CIDRS_EXT_ID_KEY)
         logical_switch = row.external_ids.get(constants.OVN_LS_NAME_EXT_ID_KEY)
 
         self.nb_bgp_driver.expose_ip(ips, row)
 
         if not logical_switch:
@@ -515,14 +521,15 @@
     def test_expose_fip(self):
         ip = '10.0.0.1'
         logical_switch = 'lswitch1'
         mock_get_ls_localnet_info = mock.patch.object(
             self.nb_bgp_driver, '_get_ls_localnet_info').start()
         mock_get_ls_localnet_info.return_value = ('fake-localnet', 'br-ex',
                                                   100)
+        self.nb_bgp_driver.ovn_bridge_mappings = {'fake-localnet': 'br-ex'}
         mock_expose_provider_port = mock.patch.object(
             self.nb_bgp_driver, '_expose_provider_port').start()
         row = fakes.create_object({
             'external_ids': {constants.OVN_LS_NAME_EXT_ID_KEY: 'test-ls'}})
 
         ret = self.nb_bgp_driver.expose_fip(ip, logical_switch, row)
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from unittest import mock
 
 from oslo_config import cfg
 
-from ovn_bgp_agent import config
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack import ovn_bgp_driver
 from ovn_bgp_agent.drivers.openstack.utils import bgp as bgp_utils
 from ovn_bgp_agent.drivers.openstack.utils import driver_utils
 from ovn_bgp_agent.drivers.openstack.utils import frr
 from ovn_bgp_agent.drivers.openstack.utils import ovn
 from ovn_bgp_agent.drivers.openstack.utils import ovs
@@ -34,15 +33,14 @@
 CONF = cfg.CONF
 
 
 class TestOVNBGPDriver(test_base.TestCase):
 
     def setUp(self):
         super(TestOVNBGPDriver, self).setUp()
-        config.register_opts()
         CONF.set_override('expose_tenant_networks', True)
         self.bridge = 'fake-bridge'
         self.bgp_driver = ovn_bgp_driver.OVNBGPDriver()
         self.bgp_driver._post_fork_event = mock.Mock()
         self.bgp_driver.sb_idl = mock.Mock()
         self.sb_idl = self.bgp_driver.sb_idl
         self.bgp_driver.chassis = 'fake-chassis'
@@ -71,20 +69,18 @@
                            'bridge_device': self.bridge,
                            'bridge_vlan': None},
             self.cr_lrp1: {'provider_datapath': 'fake-provider-dp2'}}
         self.bgp_driver.provider_ovn_lbs = {
             self.loadbalancer_vip_port: {'ips': [self.ipv4, self.ipv6],
                                          'gateway_port': self.cr_lrp0}}
 
-        # Mock pyroute2.NDB context manager object
-        self.mock_ndb = mock.patch.object(linux_net.pyroute2, 'NDB').start()
-        self.fake_ndb = self.mock_ndb().__enter__()
-
+    @mock.patch.object(linux_net, 'ensure_ovn_device')
+    @mock.patch.object(linux_net, 'ensure_vrf')
     @mock.patch.object(frr, 'vrf_leak')
-    def test_start(self, mock_vrf):
+    def test_start(self, mock_vrf, *args):
         self.bgp_driver.start()
 
         mock_vrf.assert_called_once_with(
             CONF.bgp_vrf, CONF.bgp_AS, CONF.bgp_router_id,
             template=frr.LEAK_VRF_TEMPLATE)
         # Assert connections were started
         self.mock_ovs_idl().start.assert_called_once_with(
@@ -102,30 +98,33 @@
             CONF.bgp_vrf, CONF.bgp_vrf_table_id)
         mock_vrf_leak.assert_called_once_with(
             CONF.bgp_vrf, CONF.bgp_AS, CONF.bgp_router_id,
             template=frr.LEAK_VRF_TEMPLATE)
         mock_ensure_ovn_dev.assert_called_once_with(
             CONF.bgp_nic, CONF.bgp_vrf)
 
+    @mock.patch.object(wire_utils, 'delete_vlan_devices_leftovers')
     @mock.patch.object(linux_net, 'delete_bridge_ip_routes')
     @mock.patch.object(linux_net, 'delete_ip_rules')
     @mock.patch.object(linux_net, 'delete_exposed_ips')
     @mock.patch.object(ovs, 'remove_extra_ovs_flows')
     @mock.patch.object(ovs, 'ensure_mac_tweak_flows')
     @mock.patch.object(ovs, 'get_ovs_patch_ports_info')
     @mock.patch.object(linux_net, 'get_ovn_ip_rules')
     @mock.patch.object(linux_net, 'get_exposed_ips')
+    @mock.patch.object(linux_net, 'get_interface_address')
     @mock.patch.object(linux_net, 'ensure_vlan_device_for_network')
     @mock.patch.object(linux_net, 'ensure_routing_table_for_bridge')
     @mock.patch.object(linux_net, 'ensure_arp_ndp_enabled_for_bridge')
     def test_sync(
             self, mock_ensure_arp, mock_routing_bridge,
-            mock_ensure_vlan_network, mock_exposed_ips, mock_get_ip_rules,
-            mock_get_patch_ports, mock_ensure_mac, mock_remove_flows,
-            mock_del_exposed_ips, mock_del_ip_rules, mock_del_ip_routes):
+            mock_ensure_vlan_network, mock_nic_address, mock_exposed_ips,
+            mock_get_ip_rules, mock_get_patch_ports, mock_ensure_mac,
+            mock_remove_flows, mock_del_exposed_ips, mock_del_ip_rules,
+            mock_del_ip_routes, mock_vlan_leftovers):
         self.mock_ovs_idl.get_ovn_bridge_mappings.return_value = [
             'net0:bridge0', 'net1:bridge1']
         self.sb_idl.get_network_vlan_tag_by_network_name.side_effect = (
             [10], [11])
         fake_ip_rules = 'fake-ip-rules'
         mock_get_ip_rules.return_value = fake_ip_rules
         ips = [self.ipv4, self.ipv6]
@@ -136,14 +135,15 @@
             'fake-cr-port0', 'fake-cr-port1']
 
         mock_ensure_port_exposed = mock.patch.object(
             self.bgp_driver, '_ensure_port_exposed').start()
         mock_ensure_cr_port_exposed = mock.patch.object(
             self.bgp_driver, '_ensure_cr_lrp_associated_ports_exposed').start()
         mock_routing_bridge.return_value = ['fake-route']
+        mock_nic_address.return_value = self.mac
         mock_get_patch_ports.return_value = [1, 2]
 
         self.bgp_driver.sync()
 
         expected_calls = [mock.call('bridge0', 1, [10]),
                           mock.call('bridge1', 2, [11])]
         mock_ensure_arp.assert_has_calls(expected_calls)
@@ -180,14 +180,16 @@
             ips, CONF.bgp_nic)
         mock_del_ip_rules.assert_called_once_with(fake_ip_rules)
         mock_del_ip_routes.assert_called_once_with(
             {}, mock.ANY,
             {'bridge0': ['fake-route'], 'bridge1': ['fake-route']})
 
         mock_get_ip_rules.assert_called_once_with(mock.ANY)
+        mock_vlan_leftovers.assert_called_once_with(
+            self.sb_idl, self.bgp_driver.ovn_bridge_mappings)
 
     @mock.patch.object(linux_net, 'get_ip_version')
     def test__ensure_cr_lrp_associated_ports_exposed(self, mock_ip_version):
         mock_expose_ip = mock.patch.object(
             self.bgp_driver, '_expose_ip').start()
         mock_ip_version.side_effect = (constants.IP_VERSION_4,
                                        constants.IP_VERSION_6)
@@ -1330,14 +1332,17 @@
         lrp2 = fakes.create_object({'logical_port': 'fake-lrp',
                                     'chassis': '',
                                     'options': {}})
         self.sb_idl.get_lrp_ports_for_router.return_value = [lrp0, lrp1, lrp2]
 
         self.sb_idl.get_port_datapath.return_value = 'fake-lrp-dp'
 
+        self.sb_idl.get_cr_lrp_nat_addresses_info.return_value = (
+            [], self.cr_lrp0)
+
         mock_process_lrp_port = mock.patch.object(
             self.bgp_driver, '_process_lrp_port').start()
 
         mock_ip_version.side_effect = (constants.IP_VERSION_4,
                                        constants.IP_VERSION_6)
         row = fakes.create_object({
             'type': constants.OVN_CHASSISREDIRECT_VIF_PORT_TYPE,
@@ -1814,19 +1819,22 @@
 
         dp_port0 = mock.Mock()
         self.sb_idl.get_lrp_ports_for_router.return_value = [dp_port0]
         ovn_lbs = {'fake-vip-port': 'fake-vip-ip'}
         self.sb_idl.get_provider_ovn_lbs_on_cr_lrp.return_value = (
             ovn_lbs)
 
+        ips_without_mask = [ip.split("/")[0] for ip in ips]
+        self.sb_idl.get_cr_lrp_nat_addresses_info.return_value = (
+            [ips_without_mask[0]], self.cr_lrp0)
+
         self.bgp_driver._expose_cr_lrp_port(
             ips, self.mac, self.bridge, None, router_datapath='fake-router-dp',
             provider_datapath='fake-provider-dp', cr_lrp_port=self.cr_lrp0)
 
-        ips_without_mask = [ip.split("/")[0] for ip in ips]
         mock_expose_provider_port.assert_called_once_with(
             ips_without_mask, 'fake-provider-dp', self.bridge, None,
             lladdr=self.mac, proxy_cidrs=ips)
         mock_process_lrp_port.assert_called_once_with(dp_port0, self.cr_lrp0)
         mock_expose_ovn_lb.assert_called_once_with(
             'fake-vip-ip', 'fake-vip-port', self.cr_lrp0)
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from unittest import mock
 
 from oslo_config import cfg
 
-from ovn_bgp_agent import config
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack import ovn_evpn_driver
 from ovn_bgp_agent.drivers.openstack.utils import frr
 from ovn_bgp_agent.drivers.openstack.utils import ovn
 from ovn_bgp_agent.drivers.openstack.utils import ovs
 from ovn_bgp_agent.tests import base as test_base
 from ovn_bgp_agent.tests.unit import fakes
@@ -30,15 +29,14 @@
 CONF = cfg.CONF
 
 
 class TestOVNEVPNDriver(test_base.TestCase):
 
     def setUp(self):
         super(TestOVNEVPNDriver, self).setUp()
-        config.register_opts()
         self.evpn_driver = ovn_evpn_driver.OVNEVPNDriver()
         self.mock_sbdb = mock.patch.object(ovn, 'OvnSbIdl').start()
         self.mock_ovs_idl = mock.patch.object(ovs, 'OvsIdl').start()
         self.evpn_driver.ovs_idl = self.mock_ovs_idl
         self.evpn_driver.sb_idl = mock.Mock()
         self.sb_idl = self.evpn_driver.sb_idl
         self.evpn_driver.chassis = 'fake-chassis'
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from unittest import mock
 
 from oslo_config import cfg
 
-from ovn_bgp_agent import config
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack import ovn_stretched_l2_bgp_driver
 from ovn_bgp_agent.drivers.openstack.utils import driver_utils
 from ovn_bgp_agent.drivers.openstack.utils import frr
 from ovn_bgp_agent.drivers.openstack.utils import ovn
 from ovn_bgp_agent.drivers.openstack.utils import ovs
+from ovn_bgp_agent import exceptions as agent_exc
 from ovn_bgp_agent.tests import base as test_base
 from ovn_bgp_agent.tests.unit import fakes
 from ovn_bgp_agent.utils import linux_net
 
 import ipaddress
 
 CONF = cfg.CONF
@@ -51,15 +51,14 @@
         self.table.remove(self.route)
         self.assertEqual(0, len(self.table))
 
 
 class TestOVNBGPStretchedL2Driver(test_base.TestCase):
     def setUp(self):
         super(TestOVNBGPStretchedL2Driver, self).setUp()
-        config.register_opts()
         CONF.set_override(
             "address_scopes",
             "11111111-1111-1111-1111-11111111,22222222-2222-2222-2222-22222222",  # NOQA E501
         )
         self.bgp_driver = ovn_stretched_l2_bgp_driver.OVNBGPStretchedL2Driver()
         self.bgp_driver._post_fork_event = mock.Mock()
         self.bgp_driver.sb_idl = mock.Mock()
@@ -132,18 +131,20 @@
             }
         )
 
         # Mock pyroute2.NDB context manager object
         self.mock_ndb = mock.patch.object(linux_net.pyroute2, "NDB").start()
         self.fake_ndb = self.mock_ndb().__enter__()
 
+    @mock.patch.object(linux_net, "ensure_vrf")
     @mock.patch.object(linux_net, "ensure_ovn_device")
     @mock.patch.object(linux_net, "delete_routes_from_table")
     @mock.patch.object(frr, "vrf_leak")
-    def test_start(self, mock_vrf, mock_delete_routes, mock_ensure_ovn_device):
+    def test_start(self, mock_vrf, mock_delete_routes, mock_ensure_ovn_device,
+                   *args):
         CONF.set_override("clear_vrf_routes_on_startup", True)
 
         self.bgp_driver.start()
 
         mock_vrf.assert_called_once_with(
             CONF.bgp_vrf,
             CONF.bgp_AS,
@@ -155,19 +156,20 @@
             CONF.ovsdb_connection
         )
         self.mock_sbdb().start.assert_called_once_with()
         mock_delete_routes.assert_called_once_with(CONF.bgp_vrf_table_id)
         mock_ensure_ovn_device.assert_called_once_with(
             CONF.bgp_nic, CONF.bgp_vrf)
 
+    @mock.patch.object(linux_net, "ensure_vrf")
     @mock.patch.object(linux_net, "ensure_ovn_device")
     @mock.patch.object(linux_net, "delete_routes_from_table")
     @mock.patch.object(frr, "vrf_leak")
     def test_start_clear_routes(
-        self, mock_vrf, mock_delete_routes, mock_ensure_ovn_device):
+        self, mock_vrf, mock_delete_routes, mock_ensure_ovn_device, *args):
         CONF.set_override("clear_vrf_routes_on_startup", False)
 
         self.bgp_driver.start()
 
         mock_vrf.assert_called_once_with(
             CONF.bgp_vrf,
             CONF.bgp_AS,
@@ -353,14 +355,31 @@
 
         self.sb_idl.is_router_gateway_on_any_chassis.assert_called_once_with(
             row.datapath
         )
 
         mock__ensure_network_exposed.assert_not_called()
 
+    def test_expose_subnet_no_datapath(self):
+        mock__ensure_network_exposed = mock.patch.object(
+            self.bgp_driver, "_ensure_network_exposed"
+        ).start()
+        row = mock.Mock()
+        row.datapath = "fake-dp"
+        self.sb_idl.is_router_gateway_on_any_chassis.side_effect = (
+            agent_exc.DatapathNotFound(datapath=row.datapath))
+
+        self.bgp_driver.expose_subnet(None, row)
+
+        self.sb_idl.is_router_gateway_on_any_chassis.assert_called_once_with(
+            row.datapath
+        )
+
+        mock__ensure_network_exposed.assert_not_called()
+
     def test_update_subnet(self):
         mock__update_network = mock.patch.object(
             self.bgp_driver, "_update_network"
         ).start()
         self.sb_idl.is_router_gateway_on_any_chassis.return_value = (
             self.cr_lrp0
         )
@@ -377,14 +396,39 @@
             row.datapath
         )
 
         mock__update_network.assert_called_once_with(
             row, self.cr_lrp0.logical_port, ["3.3.3.3/24"], ["1.1.1.1/24"]
         )
 
+    def test_update_subnet_no_datapath(self):
+        mock__update_network = mock.patch.object(
+            self.bgp_driver, "_update_network"
+        ).start()
+        self.sb_idl.is_router_gateway_on_any_chassis.return_value = (
+            self.cr_lrp0
+        )
+        old = mock.Mock()
+        old.mac = ["ff:ff:ff:ff:ff:01 1.1.1.1/24 2.2.2.2/24"]
+
+        row = mock.Mock()
+        row.datapath = "fake-dp"
+        row.mac = ["ff:ff:ff:ff:ff:01 2.2.2.2/24 3.3.3.3/24"]
+
+        self.sb_idl.is_router_gateway_on_any_chassis.side_effect = (
+            agent_exc.DatapathNotFound(datapath=row.datapath))
+
+        self.bgp_driver.update_subnet(old, row)
+
+        self.sb_idl.is_router_gateway_on_any_chassis.assert_called_once_with(
+            row.datapath
+        )
+
+        mock__update_network.assert_not_called()
+
     @mock.patch.object(linux_net, "get_exposed_routes_on_network")
     @mock.patch.object(linux_net, "del_ip_route")
     @mock.patch.object(linux_net, "add_ip_route")
     def test__update_network(
         self,
         mock_add_ip_route,
         mock_del_ip_route,
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from unittest import mock
 
 from oslo_config import cfg
 from ovs.stream import Stream
 from ovsdbapp.backend.ovs_idl import connection
 from ovsdbapp.backend.ovs_idl import idlutils
 
-from ovn_bgp_agent import config
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack.utils import ovn as ovn_utils
 from ovn_bgp_agent import exceptions
 from ovn_bgp_agent.tests import base as test_base
 from ovn_bgp_agent.tests.unit import fakes
 
 CONF = cfg.CONF
@@ -36,14 +35,27 @@
         super(TestOvsdbNbOvnIdl, self).setUp()
         self.nb_idl = ovn_utils.OvsdbNbOvnIdl(mock.Mock())
 
         # Monkey-patch parent class methods
         self.nb_idl.db_find_rows = mock.Mock()
         self.nb_idl.lookup = mock.Mock()
 
+    def test_get_network_vlan_tags(self):
+        tag = [123]
+        lsp = fakes.create_object({'name': 'port-0',
+                                   'tag': tag})
+        self.nb_idl.db_find_rows.return_value.execute.return_value = [
+            lsp]
+        ret = self.nb_idl.get_network_vlan_tags()
+
+        self.assertEqual(tag, ret)
+        self.nb_idl.db_find_rows.assert_called_once_with(
+            'Logical_Switch_Port',
+            ('type', '=', constants.OVN_LOCALNET_VIF_PORT_TYPE))
+
     def test_get_network_vlan_tag_by_network_name(self):
         network_name = 'net0'
         tag = [123]
         lsp = fakes.create_object({'name': 'port-0',
                                    'options': {'network_name': network_name},
                                    'tag': tag})
         self.nb_idl.db_find_rows.return_value.execute.return_value = [
@@ -319,14 +331,22 @@
 
     def test_get_network_name_and_tag(self):
         self._test_get_network_name_and_tag()
 
     def test_get_network_name_and_tag_not_in_bridge_mappings(self):
         self._test_get_network_name_and_tag(network_in_bridge_map=False)
 
+    def test_get_netweork_vlan_tags(self):
+        tag = [1001]
+        row = fakes.create_object({'tag': tag})
+        self.sb_idl.db_find_rows.return_value.execute.return_value = [row, ]
+
+        ret = self.sb_idl.get_network_vlan_tags()
+        self.assertEqual(tag, ret)
+
     def _test_get_network_vlan_tag_by_network_name(self, match=True):
         network = 'public' if match else 'spongebob'
         tag = [1001]
         row = fakes.create_object({
             'options': {'network_name': 'public'},
             'tag': tag})
         self.sb_idl.db_find_rows.return_value.execute.return_value = [row, ]
@@ -636,15 +656,14 @@
         self.assertEqual(lb2, ret)
 
 
 class TestOvnNbIdl(test_base.TestCase):
 
     def setUp(self):
         super(TestOvnNbIdl, self).setUp()
-        config.register_opts()
         mock.patch.object(idlutils, 'get_schema_helper').start()
         mock.patch.object(ovn_utils.OvnIdl, '__init__').start()
         self.nb_idl = ovn_utils.OvnNbIdl('tcp:127.0.0.1:6640')
 
     @mock.patch.object(Stream, 'ssl_set_ca_cert_file')
     @mock.patch.object(Stream, 'ssl_set_certificate_file')
     @mock.patch.object(Stream, 'ssl_set_private_key_file')
@@ -673,15 +692,14 @@
             ['fake-event0', 'fake-event1'])
 
 
 class TestOvnSbIdl(test_base.TestCase):
 
     def setUp(self):
         super(TestOvnSbIdl, self).setUp()
-        config.register_opts()
         mock.patch.object(idlutils, 'get_schema_helper').start()
         mock.patch.object(ovn_utils.OvnIdl, '__init__').start()
         self.sb_idl = ovn_utils.OvnSbIdl('tcp:127.0.0.1:6640')
 
     @mock.patch.object(Stream, 'ssl_set_ca_cert_file')
     @mock.patch.object(Stream, 'ssl_set_certificate_file')
     @mock.patch.object(Stream, 'ssl_set_private_key_file')
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,14 @@
 
         # Helper variables that are used across multiple methods
         self.bridge = 'br-fake'
         self.flows_info = {self.bridge: {'in_port': set()}}
         self.cookie = 'fake-cookie'
         self.cookie_id = 'cookie=%s/-1' % self.cookie
         self.mac = 'aa:bb:cc:dd:ee:ff'
-        self.fake_ndb = mock.Mock(interfaces={})
-        mock_ndb = mock.patch('pyroute2.NDB').start()
-        mock_ndb.return_value.__enter__.return_value = self.fake_ndb
 
     def _test_get_bridge_flows(self, has_filter=False):
         port_iface = '1'
         fake_flow_0 = '{},ip,in_port={}'.format(self.cookie_id, port_iface)
         fake_flow_1 = '{},ipv6,in_port={}'.format(self.cookie_id, port_iface)
         fake_filter = 'cookie=fake-cookie/-1' if has_filter else None
         flows = 'HEADER\n%s\n%s\n' % (fake_flow_0, fake_flow_1)
@@ -100,22 +97,23 @@
         expected_del_flow = ('%s,ip,in_port=%s' % (self.cookie_id,
                                                    extra_port_iface))
         self.mock_ovs_vsctl.ovs_cmd.assert_called_once_with(
             'ovs-ofctl', ['del-flows', self.bridge, expected_del_flow])
         mock_flows.assert_called_once_with(self.bridge, self.cookie_id)
 
     @mock.patch.object(ovs_utils, 'get_device_port_at_ovs')
+    @mock.patch.object(linux_net, 'get_interface_address')
     @mock.patch.object(linux_net, 'get_ip_version')
-    def _test_ensure_evpn_ovs_flow(self, mock_ip_version, mock_ofport,
-                                   ip_version, strip_vlan=False):
+    def _test_ensure_evpn_ovs_flow(self, mock_ip_version, mock_nic_address,
+                                   mock_ofport, ip_version, strip_vlan=False):
         address = '00:00:00:00:00:00'
         mock_ip_version.return_value = ip_version
+        mock_nic_address.return_value = address
         port = 'fake-port'
         port_dst = 'fake-port-dst'
-        self.fake_ndb.interfaces[port_dst] = {'address': address}
         ovs_port = constants.OVS_PATCH_PROVNET_PORT_PREFIX + 'fake-port'
         port_iface = '1'
         ovs_port_iface = '2'
         net = 'fake-net'
         self.mock_ovs_vsctl.ovs_cmd.side_effect = (
             ['%s\n%s\n' % (port, ovs_port)], None)
         mock_ofport.side_effect = (ovs_port_iface, port_iface)
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from unittest import mock
 
 from oslo_config import cfg
 
-from ovn_bgp_agent import config
 from ovn_bgp_agent import constants
 from ovn_bgp_agent.drivers.openstack.watchers import bgp_watcher
 from ovn_bgp_agent.tests import base as test_base
 from ovn_bgp_agent.tests import utils
 
 CONF = cfg.CONF
 
@@ -33,47 +32,67 @@
         self.chassis = '935f91fa-b8f8-47b9-8b1b-3a7a90ef7c26'
         self.agent = mock.Mock(chassis=self.chassis)
         self.event = bgp_watcher.PortBindingChassisCreatedEvent(self.agent)
 
     def test_match_fn(self):
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[ch],
-                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[True])
         old = utils.create_row(chassis=[])
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_not_single_or_dual_stack(self):
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[ch],
                                mac=['aa:bb:cc:dd:ee:ff'])
         old = utils.create_row(chassis=[])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_old_chassis_set(self):
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[ch],
-                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[True])
         old = utils.create_row(chassis=[ch])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_no_old_chassis(self):
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[ch],
-                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[True])
         old = utils.create_row(chassis=[])
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_different_old_chassis(self):
         ch = utils.create_row(name=self.chassis)
         ch_old = utils.create_row(name='old-chassis')
         row = utils.create_row(chassis=[ch],
-                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[True])
         old = utils.create_row(chassis=[ch_old])
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
+    def test_match_fn_no_up(self):
+        ch = utils.create_row(name=self.chassis)
+        row = utils.create_row(chassis=[ch],
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[False])
+        self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock))
+
+    def test_match_fn_no_old_up(self):
+        ch = utils.create_row(name=self.chassis)
+        row = utils.create_row(chassis=[ch],
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[True])
+        old = utils.create_row(chassis=[ch],
+                               up=[False])
+        self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
+
     def test_match_fn_index_error(self):
         row = utils.create_row(chassis=[],
                                mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
         old = utils.create_row(chassis=[])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_run(self):
@@ -102,19 +121,20 @@
     def setUp(self):
         super(TestPortBindingChassisDeletedEvent, self).setUp()
         self.chassis = '935f91fa-b8f8-47b9-8b1b-3a7a90ef7c26'
         self.agent = mock.Mock(chassis=self.chassis)
         self.event = bgp_watcher.PortBindingChassisDeletedEvent(self.agent)
 
     def test_match_fn(self):
+        event = self.event.ROW_DELETE
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[ch],
                                mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
         old = utils.create_row(chassis=[])
-        self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
+        self.assertTrue(self.event.match_fn(event, row, old))
 
     def test_match_fn_not_single_or_dual_stack(self):
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[ch],
                                mac=['aa:bb:cc:dd:ee:ff'])
         old = utils.create_row(chassis=[])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
@@ -123,22 +143,34 @@
         event = self.event.ROW_UPDATE
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[],
                                mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
         old = utils.create_row(chassis=[ch])
         self.assertTrue(self.event.match_fn(event, row, old))
 
-    def test_match_fn_update_old_chassis_set(self):
+    def test_match_fn_update_old_chassis_set_up_false(self):
         event = self.event.ROW_UPDATE
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[ch],
-                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
-        old = utils.create_row(chassis=[ch])
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[True])
+        old = utils.create_row(chassis=[ch],
+                               up=[False])
         self.assertFalse(self.event.match_fn(event, row, old))
 
+    def test_match_fn_update_old_chassis_set_up_true(self):
+        event = self.event.ROW_UPDATE
+        ch = utils.create_row(name=self.chassis)
+        row = utils.create_row(chassis=[ch],
+                               mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'],
+                               up=[False])
+        old = utils.create_row(chassis=[ch],
+                               up=[True])
+        self.assertTrue(self.event.match_fn(event, row, old))
+
     def test_match_fn_update_no_chassis(self):
         event = self.event.ROW_UPDATE
         ch = utils.create_row(name=self.chassis)
         row = utils.create_row(chassis=[],
                                mac=['aa:bb:cc:dd:ee:ff 10.10.1.16'])
         old = utils.create_row(chassis=[ch])
         self.assertTrue(self.event.match_fn(event, row, old))
@@ -836,15 +868,14 @@
         self.agent.withdraw_ovn_lb.assert_not_called()
 
 
 class TestOVNLBMemberCreateEvent(test_base.TestCase):
 
     def setUp(self):
         super(TestOVNLBMemberCreateEvent, self).setUp()
-        config.register_opts()
         self.chassis = '935f91fa-b8f8-47b9-8b1b-3a7a90ef7c26'
         self.agent = mock.Mock(chassis=self.chassis)
         self.agent.ovn_local_cr_lrps = {
             'cr-lrp1': {'provider_datapath': 'dp1',
                         'subnets_datapath': {'lrp1': 's_dp1'},
                         'ovn_lbs': 'ovn-lb1'}}
         self.event = bgp_watcher.OVNLBMemberCreateEvent(self.agent)
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,60 +31,60 @@
         self.event = nb_bgp_watcher.LogicalSwitchPortProviderCreateEvent(
             self.agent)
 
     def test_match_fn(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         old = utils.create_row(options={}, up=True)
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_exception(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_not_up(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_invalid_address(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac '],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_wrong_chassis(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': 'fake_chassis'},
-                               up=True)
-        old = utils.create_row(options={}, up=True)
+                               up=[True])
+        old = utils.create_row(options={}, up=[True])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_run(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         self.event.run(mock.Mock(), row, mock.Mock())
         self.agent.expose_ip.assert_called_once_with(['192.168.0.1'], row)
 
     def test_run_wrong_type(self):
         row = utils.create_row(
             type=constants.OVN_CHASSISREDIRECT_VIF_PORT_TYPE,
             addresses=['mac 192.168.0.1'],
             options={'requested-chassis': self.chassis},
-            up=True)
+            up=[True])
         self.event.run(mock.Mock(), row, mock.Mock())
         self.agent.expose_ip.assert_not_called()
 
 
 class TestLogicalSwitchPortProviderDeleteEvent(test_base.TestCase):
 
     def setUp(self):
@@ -95,71 +95,71 @@
             self.agent)
 
     def test_match_fn_delete(self):
         event = self.event.ROW_DELETE
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         self.assertTrue(self.event.match_fn(event, row, mock.Mock()))
 
     def test_match_fn_update(self):
         event = self.event.ROW_UPDATE
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=False)
+                               up=[False])
         old = utils.create_row(options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         self.assertTrue(self.event.match_fn(event, row, old))
 
     def test_match_fn_exception(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_not_up(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=False)
+                               up=[False])
         old = utils.create_row(options={'requested-chassis': self.chassis},
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_invalid_address(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac '],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_wrong_chassis(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         old = utils.create_row(options={'requested-chassis': 'other_chassis'})
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_run(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         self.event.run(mock.Mock(), row, mock.Mock())
         self.agent.withdraw_ip.assert_called_once_with(['192.168.0.1'], row)
 
     def test_run_wrong_type(self):
         row = utils.create_row(
             type=constants.OVN_CHASSISREDIRECT_VIF_PORT_TYPE,
             addresses=['mac 192.168.0.1'],
             options={'requested-chassis': self.chassis},
-            up=True)
+            up=[True])
         self.event.run(mock.Mock(), row, mock.Mock())
         self.agent.withdraw_ip.assert_not_called()
 
 
 class TestLogicalSwitchPortFIPCreateEvent(test_base.TestCase):
 
     def setUp(self):
@@ -171,83 +171,83 @@
 
     def test_match_fn_chassis_change(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
-        old = utils.create_row(options={}, up=True)
+                               up=[True])
+        old = utils.create_row(options={}, up=[True])
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_status_change(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         old = utils.create_row(options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=False)
+                               up=[False])
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_fip_addition(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         old = utils.create_row(options={'requested-chassis': self.chassis},
                                external_ids={},
-                               up=True)
+                               up=[True])
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_no_fip(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={},
-                               up=True)
+                               up=[True])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_wrong_chassis(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': 'wrong_chassis'},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_port_down(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_wrong_address(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac '],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_exception(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_run(self):
         external_ip = '10.0.0.10'
         ls_name = 'neutron-net-id'
         self.agent.get_port_external_ip_and_ls.return_value = (external_ip,
                                                                ls_name)
@@ -286,88 +286,88 @@
     def test_match_fn_delete(self):
         event = self.event.ROW_DELETE
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         self.assertTrue(self.event.match_fn(event, row, mock.Mock()))
 
     def test_match_fn_update(self):
         event = self.event.ROW_UPDATE
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=False)
-        old = utils.create_row(up=True)
+                               up=[False])
+        old = utils.create_row(up=[True])
         self.assertTrue(self.event.match_fn(event, row, old))
 
     def test_match_fn_exception(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_not_up(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=False)
+                               up=[False])
         old = utils.create_row(options={'requested-chassis': self.chassis},
-                               up=False)
+                               up=[False])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_invalid_address(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac '],
                                options={'requested-chassis': self.chassis},
-                               up=True)
+                               up=[True])
         self.assertFalse(self.event.match_fn(mock.Mock(), row, mock.Mock()))
 
     def test_match_fn_wrong_chassis(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         old = utils.create_row(options={'requested-chassis': 'other_chassis'})
         self.assertFalse(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_chassis_update(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': 'other_chassis'},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         old = utils.create_row(options={'requested-chassis': self.chassis})
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_match_fn_fip_update(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                addresses=['mac 192.168.0.1'],
                                options={'requested-chassis': self.chassis},
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'new-fip-ip'},
-                               up=True)
+                               up=[True])
         old = utils.create_row(
             external_ids={constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'})
         self.assertTrue(self.event.match_fn(mock.Mock(), row, old))
 
     def test_run(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                external_ids={
                                    constants.OVN_FIP_EXT_ID_KEY: 'fip-ip'},
-                               up=True)
+                               up=[True])
         self.event.run(mock.Mock(), row, mock.Mock())
         self.agent.withdraw_fip.assert_called_once_with('fip-ip', row)
 
     def test_run_no_fip(self):
         row = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
                                external_ids={})
         old = utils.create_row(type=constants.OVN_VM_VIF_PORT_TYPE,
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/fakes.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/tests/unit/utils/test_linux_net.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/tests/unit/utils/test_linux_net.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,22 +21,35 @@
 from unittest import mock
 
 from ovn_bgp_agent import exceptions as agent_exc
 from ovn_bgp_agent.tests import base as test_base
 from ovn_bgp_agent.utils import linux_net
 
 
+class IPRouteDict(dict):
+    def get_attr(self, attr_name):
+        for attr in self['attrs']:
+            if attr[0] == attr_name:
+                return attr[1]
+        return
+
+
 class TestLinuxNet(test_base.TestCase):
 
     def setUp(self):
         super(TestLinuxNet, self).setUp()
         # Mock pyroute2.NDB context manager object
         self.mock_ndb = mock.patch.object(linux_net.pyroute2, 'NDB').start()
         self.fake_ndb = self.mock_ndb().__enter__()
 
+        # Mock pyroute2.IPRoute context manager object
+        self.mock_ipr = mock.patch.object(linux_net.pyroute2,
+                                          'IPRoute').start()
+        self.fake_ipr = self.mock_ipr().__enter__()
+
         # Helper variables used accross many tests
         self.ip = '10.10.1.16'
         self.ipv6 = '2002::1234:abcd:ffff:c0a8:101'
         self.dev = 'ethfake'
         self.mac = 'aa:bb:cc:dd:ee:ff'
         self.bridge = 'br-fake'
         self.table_id = 100
@@ -48,27 +61,47 @@
         self.assertEqual(4, linux_net.get_ip_version(self.ip))
 
     def test_get_ip_version_v6(self):
         self.assertEqual(6, linux_net.get_ip_version('%s/64' % self.ipv6))
         self.assertEqual(6, linux_net.get_ip_version(self.ipv6))
 
     def test_get_interfaces(self):
-        iface0 = mock.Mock(ifname='ethfake0')
-        iface1 = mock.Mock(ifname='ethfake1')
-        iface2 = mock.Mock(ifname='ethfake2')
-        self.fake_ndb.interfaces = [iface0, iface1, iface2]
+        iface0 = IPRouteDict({'attrs': [('IFLA_IFNAME', 'ethfake0')]})
+        iface1 = IPRouteDict({'attrs': [('IFLA_IFNAME', 'ethfake1')]})
+        iface2 = IPRouteDict({'attrs': [('IFLA_IFNAME', 'ethfake2')]})
+        self.fake_ipr.get_links.return_value = [iface0, iface1, iface2]
 
         ret = linux_net.get_interfaces(filter_out='ethfake1')
         self.assertEqual(['ethfake0', 'ethfake2'], ret)
 
     def test_get_interface_index(self):
-        self.fake_ndb.interfaces = {'fake-nic': {'index': 7}}
+        self.fake_ipr.link_lookup.return_value = [7]
         ret = linux_net.get_interface_index('fake-nic')
         self.assertEqual(7, ret)
 
+    def test_get_interface_index_error(self):
+        self.fake_ipr.link_lookup.return_value = ''
+        self.assertRaises(agent_exc.NetworkInterfaceNotFound,
+                          linux_net.get_interface_index, 'fake-nic')
+
+    def test_get_interface_address(self):
+        device_idx = 7
+        self.fake_ipr.link_lookup.return_value = [device_idx]
+        fake_link = mock.MagicMock()
+        fake_link.get_attr.return_value = self.mac
+        self.fake_ipr.get_links.return_value = [fake_link]
+
+        ret = linux_net.get_interface_address('fake-nic')
+        self.assertEqual(self.mac, ret)
+
+    def test_get_interface_address_index_error(self):
+        self.fake_ipr.link_lookup.return_value = ''
+        self.assertRaises(agent_exc.NetworkInterfaceNotFound,
+                          linux_net.get_interface_address, 'fake-nic')
+
     @mock.patch('ovn_bgp_agent.privileged.linux_net.ensure_vrf')
     def test_ensure_vrf(self, mock_ensure_vrf):
         linux_net.ensure_vrf('fake-vrf', 10)
         mock_ensure_vrf.assert_called_once_with('fake-vrf', 10)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.ensure_bridge')
     def test_ensure_bridge(self, mock_ensure_bridge):
@@ -81,32 +114,14 @@
         mock_ensure_vxlan.assert_called_once_with('fake-vxlan', 11, self.ip, 7)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.ensure_veth')
     def test_ensure_veth(self, mock_ensure_veth):
         linux_net.ensure_veth('fake-veth', 'fake-veth-peer')
         mock_ensure_veth.assert_called_once_with('fake-veth', 'fake-veth-peer')
 
-    def test_set_master_for_device(self):
-        dev = mock.MagicMock()
-        self.fake_ndb.interfaces = {
-            'fake-dev': dev, 'fake-master': {'index': 5}}
-        linux_net.set_master_for_device('fake-dev', 'fake-master')
-
-        dev.__enter__().set.assert_called_once_with('master', 5)
-
-    def test_set_master_for_device_already_set(self):
-        dev = mock.MagicMock()
-        dev.get.return_value = 5
-
-        self.fake_ndb.interfaces = {
-            'fake-dev': dev, 'fake-master': {'index': 5}}
-        linux_net.set_master_for_device('fake-dev', 'fake-master')
-        # Both values were the same, assert set() is not called
-        self.assertFalse(dev.__enter__().set.called)
-
     @mock.patch('ovn_bgp_agent.privileged.linux_net.ensure_dummy_device')
     def test_ensure_dummy_device(self, mock_ensure_dummy_device):
         linux_net.ensure_dummy_device('fake-dev')
         mock_ensure_dummy_device.assert_called_once_with('fake-dev')
 
     @mock.patch.object(linux_net, 'ensure_dummy_device')
     @mock.patch.object(linux_net, 'set_master_for_device')
@@ -186,58 +201,53 @@
     @mock.patch('ovn_bgp_agent.privileged.linux_net.set_kernel_flag')
     def test_enable_proxy_arp(self, mock_flag):
         linux_net.enable_proxy_arp(self.dev)
         expected_flag = 'net.ipv4.conf.%s.proxy_arp' % self.dev
         mock_flag.assert_called_once_with(expected_flag, 1)
 
     def test_get_exposed_ips(self):
-        ip0 = mock.Mock(address=self.ip, prefixlen=32)
-        ip1 = mock.Mock(address=self.ipv6, prefixlen=128)
-        ip2 = mock.Mock(address='10.10.1.18', prefixlen=24)
-        ip3 = mock.Mock(address='2001:0DB8:0000:000b::', prefixlen=64)
-        iface = mock.Mock()
-        iface.ipaddr.summary.return_value = [ip0, ip1, ip2, ip3]
-        self.fake_ndb.interfaces = {self.dev: iface}
+        ip0 = IPRouteDict({'prefixlen': 32,
+                           'attrs': [('IFA_ADDRESS', self.ip)]})
+        ip1 = IPRouteDict({'prefixlen': 128,
+                           'attrs': [('IFA_ADDRESS', self.ipv6)]})
+        ip2 = IPRouteDict({'prefixlen': 24,
+                           'attrs': [('IFA_ADDRESS', '10.10.1.18')]})
+        ip3 = IPRouteDict(
+            {'prefixlen': 64,
+             'attrs': [('IFA_ADDRESS', '2001:0DB8:0000:000b::')]})
+        self.fake_ipr.get_addr.return_value = [ip0, ip1, ip2, ip3]
 
         ips = linux_net.get_exposed_ips(self.dev)
 
         expected_ips = [self.ip, self.ipv6]
         self.assertEqual(expected_ips, ips)
 
     def test_get_nic_ip(self):
-        ip0 = mock.Mock(address='10.10.1.16')
-        ip1 = mock.Mock(address='10.10.1.17')
-        iface = mock.Mock()
-        iface.ipaddr.summary.return_value = [ip0, ip1]
-        self.fake_ndb.interfaces = {self.dev: iface}
+        ip0 = IPRouteDict({'attrs': [('IFA_ADDRESS', '10.10.1.16')]})
+        ip1 = IPRouteDict({'attrs': [('IFA_ADDRESS', '10.10.1.17')]})
+        self.fake_ipr.get_addr.return_value = [ip0, ip1]
 
         ips = linux_net.get_nic_ip(self.dev)
 
         expected_ips = ['10.10.1.16', '10.10.1.17']
         self.assertEqual(expected_ips, ips)
 
-    def test_get_nic_ip_prefixlen(self):
-        ip = mock.Mock(address=self.ip, prefixlen=32)
-        iface = mock.Mock()
-        iface.ipaddr.summary.return_value.filter.return_value = [ip]
-        self.fake_ndb.interfaces = {self.dev: iface}
-
-        linux_net.get_nic_ip(self.dev, prefixlen_filter=32)
-        iface.ipaddr.summary.return_value.filter.assert_called_once_with(
-            prefixlen=32)
-
     def test_get_exposed_ips_on_network(self):
-        ip0 = mock.Mock(address=self.ip, prefixlen=32)
-        ip1 = mock.Mock(address='10.10.1.17', prefixlen=128)
-        ip2 = mock.Mock(address=self.ipv6, prefixlen=128)
-        ip3 = mock.Mock(
-            address='2001:db8:3333:4444:5555:6666:7777:8888', prefixlen=128)
-        iface = mock.Mock()
-        iface.ipaddr.summary.return_value = [ip0, ip1, ip2, ip3]
-        self.fake_ndb.interfaces = {self.dev: iface}
+        ip0 = IPRouteDict({'prefixlen': 32,
+                           'attrs': [('IFA_ADDRESS', self.ip)]})
+        ip1 = IPRouteDict({'prefixlen': 128,
+                           'attrs': [('IFA_ADDRESS', '10.10.1.17')]})
+        ip2 = IPRouteDict({'prefixlen': 128,
+                           'attrs': [('IFA_ADDRESS', self.ipv6)]})
+        ip3 = IPRouteDict({
+            'prefixlen': 128,
+            'attrs': [('IFA_ADDRESS', '2001:db8:3333:4444:5555:6666:7777:8888')
+                      ]})
+
+        self.fake_ipr.get_addr.return_value = [ip0, ip1, ip2, ip3]
 
         network_ips = [ipaddress.ip_address(self.ip),
                        ipaddress.ip_address(self.ipv6)]
         ret = linux_net.get_exposed_ips_on_network(self.dev, network_ips)
 
         self.assertEqual([self.ip, self.ipv6], ret)
 
@@ -298,71 +308,86 @@
         ret = linux_net.get_exposed_routes_on_network(
             [self.table_id], self.network_v6
         )
 
         self.assertEqual([route1], ret)
 
     def test_get_ovn_ip_rules(self):
-        rule0 = mock.Mock(table=7, dst=10, dst_len=128, family='fake')
-        rule1 = mock.Mock(table=7, dst=11, dst_len=32, family='fake')
-        rule2 = mock.Mock(table=9, dst=5, dst_len=24, family='fake')
-        rule3 = mock.Mock(table=10, dst=6, dst_len=128, family='fake')
-        self.fake_ndb.rules.dump.return_value = [rule0, rule1, rule2, rule3]
+        rule0 = IPRouteDict({'dst_len': 128, 'family': 10,
+                             'attrs': [('FRA_TABLE', 7),
+                                       ('FRA_DST', 10)]})
+        rule1 = IPRouteDict({'dst_len': 32, 'family': 2,
+                             'attrs': [('FRA_TABLE', 7),
+                                       ('FRA_DST', 11)]})
+        rule2 = IPRouteDict({'dst_len': 24, 'family': 2,
+                             'attrs': [('FRA_TABLE', 9),
+                                       ('FRA_DST', 5)]})
+        rule3 = IPRouteDict({'dst_len': 128, 'family': 10,
+                             'attrs': [('FRA_TABLE', 10),
+                                       ('FRA_DST', 6)]})
+        self.fake_ipr.get_rules.side_effect = [[rule1, rule2], [rule0, rule3]]
 
         ret = linux_net.get_ovn_ip_rules([7, 10])
-        expected_ret = {'10/128': {'table': 7, 'family': 'fake'},
-                        '11/32': {'table': 7, 'family': 'fake'},
-                        '6/128': {'table': 10, 'family': 'fake'}}
+        expected_ret = {'10/128': {'table': 7, 'family': 10},
+                        '11/32': {'table': 7, 'family': 2},
+                        '6/128': {'table': 10, 'family': 10}}
         self.assertEqual(expected_ret, ret)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.delete_exposed_ips')
     def test_delete_exposed_ips(self, mock_delete_exposed_ips):
         linux_net.delete_exposed_ips([self.ip], self.dev)
         mock_delete_exposed_ips.assert_called_once_with([self.ip], self.dev)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.delete_ip_rules')
     def test_delete_ip_rules(self, mock_delete_ip_rules):
         ip_rules = {'10/128': {'table': 7, 'family': 'fake'},
                     '6/128': {'table': 10, 'family': 'fake'}}
         linux_net.delete_ip_rules(ip_rules)
         mock_delete_ip_rules.assert_called_once_with(ip_rules)
 
-    def _test_delete_bridge_ip_routes(self, mock_route_delete, is_vlan=False,
-                                      has_gateway=False):
+    @mock.patch.object(linux_net, 'get_interface_index')
+    def _test_delete_bridge_ip_routes(self, mock_route_delete, mock_get_index,
+                                      is_vlan=False, has_gateway=False):
         gateway = '1.1.1.1'
         oif = 11
         vlan = 30 if is_vlan else None
-        vlan_dev = '%s.%s' % (self.bridge, vlan) if is_vlan else None
-        self.fake_ndb.interfaces = {self.bridge: {'index': oif}}
-        if is_vlan:
-            self.fake_ndb.interfaces.update({vlan_dev: {'index': oif}})
+        mock_get_index.return_value = oif
 
         route = {'route': {'dst': self.ip,
                            'dst_len': 32,
                            'table': 20},
                  'vlan': vlan}
         if has_gateway:
             route['route']['gateway'] = gateway
 
         routing_tables = {self.bridge: 20}
         routing_tables_routes = {self.bridge: [route]}
         # extra_route0 matches with the route
-        extra_route0 = {'dst': self.ip, 'dst_len': 32,
-                        'family': AF_INET, 'oif': oif,
-                        'gateway': gateway, 'table': 20}
+        extra_route0 = IPRouteDict({
+            'dst_len': 32, 'family': AF_INET, 'table': 20,
+            'attrs': [('RTA_DST', self.ip),
+                      ('RTA_OIF', oif),
+                      ('RTA_GATEWAY', gateway)]})
         # extra_route1 does not match with route and should be removed
-        extra_route1 = copy.deepcopy(extra_route0)
-        extra_route1['dst'] = '10.10.1.17'
+        extra_route1 = IPRouteDict({
+            'dst_len': 32, 'family': AF_INET, 'table': 20,
+            'attrs': [('RTA_DST', '10.10.1.17'),
+                      ('RTA_OIF', oif),
+                      ('RTA_GATEWAY', gateway)]})
         extra_routes = {self.bridge: [extra_route0, extra_route1]}
 
         linux_net.delete_bridge_ip_routes(
             routing_tables, routing_tables_routes, extra_routes)
 
         # Assert extra_route1 has been removed
-        mock_route_delete.assert_called_once_with(extra_route1)
+        expected_route = {'dst': '10.10.1.17', 'dst_len': 32,
+                          'family': AF_INET, 'oif': oif,
+                          'gateway': gateway, 'table': 20}
+
+        mock_route_delete.assert_called_once_with(expected_route)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_delete')
     def test_delete_bridge_ip_routes(self, mock_route_delete):
         self._test_delete_bridge_ip_routes(mock_route_delete)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_delete')
     def test_delete_bridge_ip_routes_vlan(self, mock_route_delete):
@@ -370,53 +395,55 @@
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_delete')
     def test_delete_bridge_ip_routes_gateway(self, mock_route_delete):
         self._test_delete_bridge_ip_routes(mock_route_delete, has_gateway=True)
 
     @mock.patch('ovn_bgp_agent.utils.linux_net.delete_ip_routes')
     def test_delete_routes_from_table(self, mock_delete_ip_routes):
-        route0 = mock.MagicMock(scope=1, proto=11)
-        route1 = mock.MagicMock(scope=2, proto=22)
-        route2 = mock.MagicMock(scope=254, proto=186)
-        self.fake_ndb.routes.dump().filter.return_value = [
+        route0 = {'scope': 1, 'proto': 11}
+        route1 = {'scope': 2, 'proto': 22}
+        route2 = {'scope': 254, 'proto': 186}
+        self.fake_ipr.get_routes.return_value = [
             route0, route1, route2]
 
-        self.fake_ndb.routes.__getitem__.side_effect = (
-            route0, route1)
-
         linux_net.delete_routes_from_table('fake-table')
 
         mock_delete_ip_routes.assert_called_once_with([route0, route1])
 
     def test_get_routes_on_tables(self):
-        route0 = mock.MagicMock(table=10, dst='10.10.10.10', proto=10)
+        route0 = IPRouteDict({
+            'proto': 10, 'table': 10,
+            'attrs': [('RTA_DST', '10.10.10.10')]})
         # Route1 has proto 186, should be ignored
-        route1 = mock.MagicMock(table=11, dst='11.11.11.11', proto=186)
-        route2 = mock.MagicMock(table=11, dst='12.12.12.12', proto=12)
-        # Route3 is not in the table list, should be ignored
-        route3 = mock.MagicMock(table=99, dst='14.14.14.14', proto=14)
-        # Route4 is in the list but dst is empty
-        route4 = mock.MagicMock(table=22, dst='', proto=10)
-        self.fake_ndb.routes.dump.return_value = [
-            route0, route1, route2, route3, route4]
+        route1 = IPRouteDict({
+            'proto': 186, 'table': 11,
+            'attrs': [('RTA_DST', '11.11.11.11')]})
+        route2 = IPRouteDict({
+            'proto': 12, 'table': 11,
+            'attrs': [('RTA_DST', '12.12.12.12')]})
+        # Route3 is in the list but dst is empty
+        route3 = IPRouteDict({
+            'proto': 10, 'table': 22,
+            'attrs': [('RTA_DST', '')]})
+        self.fake_ipr.get_routes.side_effect = [
+            [route0], [route1, route2], [route3]]
 
         ret = linux_net.get_routes_on_tables([10, 11, 22])
 
         self.assertEqual([route0, route2], ret)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_delete')
     def test_delete_ip_routes(self, mock_route_delete):
         route0 = mock.MagicMock(
             table=10, dst='10.10.10.10', proto=10, dst_len=128,
             oif='ethout', family='fake', gateway='1.1.1.1')
         route1 = mock.MagicMock(
             table=11, dst='11.11.11.11', proto=11, dst_len=64,
             oif='ethout', family='fake', gateway='2.2.2.2')
         routes = [route0, route1]
-        self.fake_ndb.routes.__getitem__.side_effect = routes
 
         linux_net.delete_ip_routes(routes)
 
         mock_route_delete.has_calls([mock.call(route0), mock.call(route1)])
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.add_ndp_proxy')
     def test_add_ndp_proxy(self, mock_ndp_proxy):
@@ -427,17 +454,14 @@
     def test_del_ndp_proxy(self, mock_ndp_proxy):
         linux_net.del_ndp_proxy(self.ip, self.dev, vlan=10)
         mock_ndp_proxy.assert_called_once_with(self.ip, self.dev, 10)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_delete')
     @mock.patch('ovn_bgp_agent.privileged.linux_net.add_ip_to_dev')
     def test_add_ips_to_dev(self, mock_add_ip_to_dev, mock_route_delete):
-        iface = mock.MagicMock(index=7)
-        self.fake_ndb.interfaces = {self.dev: iface}
-
         ips = [self.ip, self.ipv6]
         linux_net.add_ips_to_dev(
             self.dev, ips, clear_local_route_at_table=123)
 
         # Assert called for each ip
         calls = [mock.call(self.ip, self.dev),
                  mock.call(self.ipv6, self.dev)]
@@ -448,17 +472,14 @@
               'oif': 7}
         calls = [mock.call(r1),
                  mock.call(r2)]
         mock_route_delete.has_calls(calls)
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.del_ip_from_dev')
     def test_del_ips_from_dev(self, mock_del_ip_from_dev):
-        iface = mock.MagicMock()
-        self.fake_ndb.interfaces = {self.dev: iface}
-
         ips = [self.ip, self.ipv6]
         linux_net.del_ips_from_dev(self.dev, ips)
 
         calls = [mock.call(self.ip, self.dev),
                  mock.call(self.ipv6, self.dev)]
         mock_del_ip_from_dev.has_calls(calls)
 
@@ -492,42 +513,33 @@
     def test_add_ip_nei(self, mock_add_ip_nei):
         linux_net.add_ip_nei(self.ip, self.mac, self.dev)
         mock_add_ip_nei.assert_called_once_with(self.ip, self.mac, self.dev)
 
     @mock.patch.object(linux_net, 'del_ip_nei')
     @mock.patch('ovn_bgp_agent.privileged.linux_net.rule_delete')
     def test_del_ip_rule(self, mock_rule_delete, mock_del_ip_nei):
-        rule = mock.MagicMock()
-        self.fake_ndb.rules.__getitem__.return_value = rule
-
         linux_net.del_ip_rule(self.ip, 7, dev=self.dev, lladdr=self.mac)
 
         expected_args = {'dst': self.ip, 'table': 7, 'dst_len': 32}
         mock_rule_delete.assert_called_once_with(expected_args)
         mock_del_ip_nei.assert_called_once_with(self.ip, self.mac, self.dev)
 
     @mock.patch.object(linux_net, 'del_ip_nei')
     @mock.patch('ovn_bgp_agent.privileged.linux_net.rule_delete')
     def test_del_ip_rule_ipv6(self, mock_rule_delete, mock_del_ip_nei):
-        rule = mock.MagicMock()
-        self.fake_ndb.rules.__getitem__.return_value = rule
-
         linux_net.del_ip_rule(self.ipv6, 7, dev=self.dev, lladdr=self.mac)
 
         expected_args = {'dst': self.ipv6, 'table': 7,
                          'dst_len': 128, 'family': AF_INET6}
         mock_rule_delete.assert_called_once_with(expected_args)
         mock_del_ip_nei.assert_called_once_with(self.ipv6, self.mac, self.dev)
 
     @mock.patch.object(linux_net, 'del_ip_nei')
     @mock.patch('ovn_bgp_agent.privileged.linux_net.rule_delete')
     def test_del_ip_rule_invalid_ip(self, mock_rule_delete, mock_del_ip_nei):
-        rule = mock.MagicMock()
-        self.fake_ndb.rules.__getitem__.return_value = rule
-
         self.assertRaises(agent_exc.InvalidPortIP,
                           linux_net.del_ip_rule, '10.10.1.6/30/128', 7)
 
         mock_rule_delete.assert_not_called()
         mock_del_ip_nei.assert_not_called()
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.del_ip_nei')
@@ -549,15 +561,14 @@
                                   'dst_len': 32,
                                   'oif': mock.ANY,
                                   'proto': 3,
                                   'scope': 253,
                                   'table': 7},
                         'vlan': None}]}
         self.assertEqual(expected_routes, routes)
-        self.assertFalse(self.fake_ndb.routes.create.called)
         mock_route_create.assert_not_called()
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_create')
     def test_add_ip_route_ipv6(self, mock_route_create):
         routes = {}
         linux_net.add_ip_route(routes, self.ipv6, 7, self.dev)
         expected_routes = {
@@ -598,22 +609,23 @@
                                   'proto': 3,
                                   'scope': 253,
                                   'table': 7},
                         'vlan': 10}]}
         self.assertEqual(expected_routes, routes)
         mock_route_create.assert_not_called()
 
+    @mock.patch.object(linux_net, 'get_interface_index')
     @mock.patch.object(linux_net, 'ensure_vlan_device_for_network')
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_create')
     def test_add_ip_route_vlan_keyerror(self, mock_route_create,
-                                        mock_ensure_vlan_device):
+                                        mock_ensure_vlan_device,
+                                        mock_get_index):
         routes = {}
         oif = '5'
-        self.fake_ndb.interfaces.__getitem__.side_effect = (
-            KeyError('No index'), {'index': oif})
+        mock_get_index.side_effect = [agent_exc.NetworkInterfaceNotFound, oif]
         linux_net.add_ip_route(routes, self.ip, 7, self.dev, vlan=10)
         expected_routes = {
             self.dev: [{'route': {'dst': self.ip,
                                   'dst_len': 32,
                                   'oif': oif,
                                   'proto': 3,
                                   'scope': 253,
@@ -635,16 +647,16 @@
                                   'scope': 253,
                                   'table': 7},
                         'vlan': None}]}
         self.assertEqual(expected_routes, routes)
         mock_route_create.assert_not_called()
 
     @mock.patch('ovn_bgp_agent.privileged.linux_net.route_create')
-    def test_add_ip_route_keyerror(self, mock_route_create):
-        self.fake_ndb.routes.__getitem__.side_effect = KeyError('Nite Expo')
+    def test_add_ip_route_no_route(self, mock_route_create):
+        self.fake_ipr.route.return_value = ()
         routes = {}
         linux_net.add_ip_route(routes, self.ip, 7, self.dev)
         expected_routes = {
             self.dev: [{'route': {'dst': self.ip,
                                   'dst_len': 32,
                                   'oif': mock.ANY,
                                   'proto': 3,
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent/utils/linux_net.py` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent/utils/linux_net.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,28 +39,46 @@
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def get_interfaces(filter_out=[]):
-    with pyroute2.NDB() as ndb:
-        return [iface.ifname for iface in ndb.interfaces
-                if iface.ifname not in filter_out]
+    with pyroute2.IPRoute() as ipr:
+        return [iface.get_attr('IFLA_IFNAME') for iface in ipr.get_links()
+                if iface.get_attr('IFLA_IFNAME') not in filter_out]
 
 
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def get_interface_index(nic):
-    with pyroute2.NDB() as ndb:
-        return ndb.interfaces[nic]['index']
+    try:
+        with pyroute2.IPRoute() as ipr:
+            return ipr.link_lookup(ifname=nic)[0]
+    except IndexError:
+        raise agent_exc.NetworkInterfaceNotFound(device=nic)
+
+
+@tenacity.retry(
+    retry=tenacity.retry_if_exception_type(
+        netlink_exceptions.NetlinkDumpInterrupted),
+    wait=tenacity.wait_exponential(multiplier=0.02, max=1),
+    stop=tenacity.stop_after_delay(8),
+    reraise=True)
+def get_interface_address(nic):
+    try:
+        with pyroute2.IPRoute() as ipr:
+            idx = ipr.link_lookup(ifname=nic)[0]
+            return ipr.get_links(idx)[0].get_attr('IFLA_ADDRESS')
+    except IndexError:
+        raise agent_exc.NetworkInterfaceNotFound(device=nic)
 
 
 def ensure_vrf(vrf_name, vrf_table):
     ovn_bgp_agent.privileged.linux_net.ensure_vrf(vrf_name, vrf_table)
 
 
 def ensure_bridge(bridge_name):
@@ -95,21 +113,25 @@
 
 def ensure_arp_ndp_enabled_for_bridge(bridge, offset, vlan_tag=None):
     ipv4 = constants.ARP_IPV4_PREFIX + str(int(offset / 256)) + "." + str(
         offset % 256)
     ipv6 = constants.NDP_IPV6_PREFIX + "%x" % offset
     try:
         ovn_bgp_agent.privileged.linux_net.add_ip_to_dev(ipv4, bridge)
+    except agent_exc.IpAddressAlreadyExists:
+        LOG.debug("IP %s already added on bridge %s", ipv4, bridge)
     except KeyError as e:
         if "object exists" not in str(e):
             LOG.error("Unable to add IP on bridge %s to enable arp/ndp. "
                       "Exception: %s", bridge, e)
             raise
     try:
         ovn_bgp_agent.privileged.linux_net.add_ip_to_dev(ipv6, bridge)
+    except agent_exc.IpAddressAlreadyExists:
+        LOG.debug("IP %s already added on bridge %s", ipv6, bridge)
     except KeyError as e:
         if "object exists" not in str(e):
             LOG.error("Unable to add IP on bridge %s to enable arp/ndp. "
                       "Exception: %s", bridge, e)
             raise
 
     if not vlan_tag:
@@ -162,154 +184,149 @@
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def _ensure_routing_table_routes(ovn_routing_tables, bridge):
     # add default route on that table if it does not exist
     extra_routes = []
+    bridge_idx = get_interface_index(bridge)
 
-    with pyroute2.NDB() as ndb:
+    with pyroute2.IPRoute() as ip:
         table_route_dsts = set(
             [
-                (r.dst, r.dst_len)
-                for r in ndb.routes.summary().filter(
-                    table=ovn_routing_tables[bridge]
-                )
+                (r.get_attr('RTA_DST'), r['dst_len'])
+                for r in ip.get_routes(table=ovn_routing_tables[bridge])
             ]
         )
 
         if not table_route_dsts:
-            r1 = {'dst': 'default', 'oif': ndb.interfaces[bridge]['index'],
+            r1 = {'dst': 'default', 'oif': bridge_idx,
                   'table': ovn_routing_tables[bridge], 'scope': 253,
                   'proto': 3}
             ovn_bgp_agent.privileged.linux_net.route_create(r1)
 
-            r2 = {'dst': 'default', 'oif': ndb.interfaces[bridge]['index'],
+            r2 = {'dst': 'default', 'oif': bridge_idx,
                   'table': ovn_routing_tables[bridge], 'family': AF_INET6,
                   'proto': 3}
             ovn_bgp_agent.privileged.linux_net.route_create(r2)
         else:
             route_missing = True
             route6_missing = True
             for (dst, dst_len) in table_route_dsts:
                 if not dst:  # default route
                     try:
-                        route = ndb.routes[
-                            {'table': ovn_routing_tables[bridge],
-                             'dst': '',
-                             'family': AF_INET}]
-                        if (bridge ==
-                                ndb.interfaces[{'index': route['oif']}][
-                                    'ifname']):
+                        route = [
+                            r for r in ip.get_routes(
+                                table=ovn_routing_tables[bridge],
+                                family=AF_INET)
+                            if not r.get_attr('RTA_DST')][0]
+                        if bridge_idx == route.get_attr('RTA_OIF'):
                             route_missing = False
                         else:
                             extra_routes.append(route)
-                    except KeyError:
+                    except IndexError:
                         pass  # no ipv4 default rule
                     try:
-                        route_6 = ndb.routes[
-                            {'table': ovn_routing_tables[bridge],
-                             'dst': '',
-                             'family': AF_INET6}]
-                        if (bridge ==
-                                ndb.interfaces[{'index': route_6['oif']}][
-                                    'ifname']):
+                        route_6 = [
+                            r for r in ip.get_routes(
+                                table=ovn_routing_tables[bridge],
+                                family=AF_INET6)
+                            if not r.get_attr('RTA_DST')][0]
+                        if bridge_idx == route_6.get_attr('RTA_OIF'):
                             route6_missing = False
                         else:
                             extra_routes.append(route_6)
-                    except KeyError:
+                    except IndexError:
                         pass  # no ipv6 default rule
                 else:
                     if get_ip_version(dst) == constants.IP_VERSION_6:
                         extra_routes.append(
-                            ndb.routes[{'table': ovn_routing_tables[bridge],
-                                        'dst': dst,
-                                        'dst_len': dst_len,
-                                        'family': AF_INET6}]
-                        )
+                            ip.get_routes(
+                                table=ovn_routing_tables[bridge],
+                                dst=dst,
+                                dst_len=dst_len,
+                                family=AF_INET6)[0])
                     else:
                         extra_routes.append(
-                            ndb.routes[{'table': ovn_routing_tables[bridge],
-                                        'dst': dst,
-                                        'dst_len': dst_len,
-                                        'family': AF_INET}]
-                        )
+                            ip.get_routes(
+                                table=ovn_routing_tables[bridge],
+                                dst=dst,
+                                dst_len=dst_len,
+                                family=AF_INET)[0])
 
             if route_missing:
-                r = {'dst': 'default', 'oif': ndb.interfaces[bridge]['index'],
+                r = {'dst': 'default', 'oif': bridge_idx,
                      'table': ovn_routing_tables[bridge], 'scope': 253,
                      'proto': 3}
                 ovn_bgp_agent.privileged.linux_net.route_create(r)
             if route6_missing:
-                r = {'dst': 'default', 'oif': ndb.interfaces[bridge]['index'],
+                r = {'dst': 'default', 'oif': bridge_idx,
                      'table': ovn_routing_tables[bridge], 'family': AF_INET6,
                      'proto': 3}
                 ovn_bgp_agent.privileged.linux_net.route_create(r)
     return extra_routes
 
 
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def get_extra_routing_table_for_bridge(ovn_routing_tables, bridge):
     extra_routes = []
-
-    with pyroute2.NDB() as ndb:
+    bridge_idx = get_interface_index(bridge)
+    with pyroute2.IPRoute() as ip:
         table_route_dsts = set(
             [
-                (r.dst, r.dst_len)
-                for r in ndb.routes.summary().filter(
-                    table=ovn_routing_tables[bridge]
-                )
+                (r.get_attr('RTA_DST'), r['dst_len'])
+                for r in ip.get_routes(table=ovn_routing_tables[bridge])
             ]
         )
 
         if not table_route_dsts:
             return extra_routes
 
         for (dst, dst_len) in table_route_dsts:
             if not dst:  # default route
                 try:
-                    route = ndb.routes[
-                        {'table': ovn_routing_tables[bridge],
-                         'dst': '',
-                         'family': AF_INET}]
-                    if (bridge != ndb.interfaces[{'index': route['oif']}][
-                            'ifname']):
+                    route = [
+                        r for r in ip.get_routes(
+                            table=ovn_routing_tables[bridge],
+                            family=AF_INET)
+                        if not r.get_attr('RTA_DST')][0]
+                    if bridge_idx != route.get_attr('RTA_OIF'):
                         extra_routes.append(route)
-                except KeyError:
-                    pass  # no ipv4 default rule
+                except IndexError:
+                    pass  # no IPv4 default rule
                 try:
-                    route_6 = ndb.routes[
-                        {'table': ovn_routing_tables[bridge],
-                         'dst': '',
-                         'family': AF_INET6}]
-                    if (bridge != ndb.interfaces[{'index': route_6['oif']}][
-                            'ifname']):
+                    route_6 = [
+                        r for r in ip.get_routes(
+                            table=ovn_routing_tables[bridge],
+                            family=AF_INET6)
+                        if not r.get_attr('RTA_DST')][0]
+                    if bridge_idx != route_6.get_attr('RTA_OIF'):
                         extra_routes.append(route_6)
-                except KeyError:
-                    pass  # no ipv6 default rule
+                except IndexError:
+                    pass  # no IPv6 default rule
             else:
                 if get_ip_version(dst) == constants.IP_VERSION_6:
                     extra_routes.append(
-                        ndb.routes[{'table': ovn_routing_tables[bridge],
-                                    'dst': dst,
-                                    'dst_len': dst_len,
-                                    'family': AF_INET6}]
-                    )
+                        ip.get_routes(
+                            table=ovn_routing_tables[bridge],
+                            dst=dst,
+                            dst_len=dst_len,
+                            family=AF_INET6)[0])
                 else:
                     extra_routes.append(
-                        ndb.routes[{'table': ovn_routing_tables[bridge],
-                                    'dst': dst,
-                                    'dst_len': dst_len,
-                                    'family': AF_INET}]
-                    )
+                        ip.get_routes(
+                            table=ovn_routing_tables[bridge],
+                            dst=dst,
+                            dst_len=dst_len,
+                            family=AF_INET)[0])
     return extra_routes
 
 
 def ensure_vlan_device_for_network(bridge, vlan_tag):
     ovn_bgp_agent.privileged.linux_net.ensure_vlan_device_for_network(bridge,
                                                                       vlan_tag)
     device = "{}/{}".format(bridge, vlan_tag)
@@ -318,14 +335,18 @@
 
 
 def delete_vlan_device_for_network(bridge, vlan_tag):
     vlan_device_name = '{}.{}'.format(bridge, vlan_tag)
     delete_device(vlan_device_name)
 
 
+def get_bridge_vlans(bridge):
+    return ovn_bgp_agent.privileged.linux_net.get_bridge_vlans(bridge)
+
+
 def enable_proxy_ndp(device):
     flag = "net.ipv6.conf.{}.proxy_ndp".format(device)
     ovn_bgp_agent.privileged.linux_net.set_kernel_flag(flag, 1)
 
 
 def enable_proxy_arp(device):
     flag = "net.ipv4.conf.{}.proxy_arp".format(device)
@@ -335,61 +356,52 @@
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def get_exposed_ips(nic):
-    exposed_ips = []
-    with pyroute2.NDB() as ndb:
-        exposed_ips = [ip.address
-                       for ip in ndb.interfaces[nic].ipaddr.summary()
-                       if ip.prefixlen == 32 or ip.prefixlen == 128]
-    return exposed_ips
+    nic_idx = get_interface_index(nic)
+    try:
+        with pyroute2.IPRoute() as ipr:
+            return [ip.get_attr('IFA_ADDRESS')
+                    for ip in ipr.get_addr(index=nic_idx)
+                    if ip['prefixlen'] in (32, 128)]
+    except pyroute2.netlink.exceptions.NetlinkError:
+        # Nic does not exist
+        LOG.debug("NIC %s does not yet exist, so it does not have exposed IPs",
+                  nic)
+        return []
 
 
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def get_nic_ip(nic, prefixlen_filter=None):
-    exposed_ips = []
-    with pyroute2.NDB() as ndb:
+    nic_idx = get_interface_index(nic)
+    with pyroute2.IPRoute() as ipr:
         if prefixlen_filter:
-            exposed_ips = [ip.address
-                           for ip in ndb.interfaces[nic].ipaddr.summary(
-                               ).filter(prefixlen=prefixlen_filter)]
+            return [
+                ip.get_attr('IFA_ADDRESS')
+                for ip in ipr.get_addr(index=nic_idx,
+                                       prefixlen=prefixlen_filter)
+            ]
         else:
-            exposed_ips = [ip.address
-                           for ip in ndb.interfaces[nic].ipaddr.summary()]
-
-    return exposed_ips
+            return [
+                ip.get_attr('IFA_ADDRESS')
+                for ip in ipr.get_addr(index=nic_idx)
+            ]
 
 
-@tenacity.retry(
-    retry=tenacity.retry_if_exception_type(
-        netlink_exceptions.NetlinkDumpInterrupted),
-    wait=tenacity.wait_exponential(multiplier=0.02, max=1),
-    stop=tenacity.stop_after_delay(8),
-    reraise=True)
 def get_exposed_ips_on_network(nic, network):
-    exposed_ips = []
-    with pyroute2.NDB() as ndb:
-        try:
-            exposed_ips = [ip.address
-                           for ip in ndb.interfaces[nic].ipaddr.summary()
-                           if ((ip.prefixlen == 32 or ip.prefixlen == 128) and
-                               ipaddress.ip_address(ip.address) in network)]
-        except KeyError:
-            # Nic does not exists
-            LOG.debug("Nic %s does not yet exists, so it does not have "
-                      "exposed IPs", nic)
-    return exposed_ips
+    exposed_ips = get_exposed_ips(nic)
+    return [ip for ip in exposed_ips if ipaddress.ip_address(ip) in network]
 
 
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
@@ -410,22 +422,25 @@
 
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
-def get_ovn_ip_rules(routing_table):
-    # get the rules pointing to ovn bridges
+def get_ovn_ip_rules(routing_tables):
     ovn_ip_rules = {}
-    with pyroute2.NDB() as ndb:
-        rules_info = [(rule.table,
-                       "{}/{}".format(rule.dst, rule.dst_len),
-                       rule.family) for rule in ndb.rules.dump()
-                      if rule.table in routing_table]
+    with pyroute2.IPRoute() as ipr:
+        rules_info = [
+            (rule.get_attr('FRA_TABLE'),
+             "{}/{}".format(rule.get_attr('FRA_DST'), rule['dst_len']),
+             rule['family'])
+            for rule in (
+                ipr.get_rules(family=AF_INET) + ipr.get_rules(family=AF_INET6))
+            if rule.get_attr('FRA_TABLE') in routing_tables
+        ]
         for table, dst, family in rules_info:
             ovn_ip_rules[dst] = {'table': table, 'family': family}
     return ovn_ip_rules
 
 
 def delete_exposed_ips(ips, nic):
     ovn_bgp_agent.privileged.linux_net.delete_exposed_ips(ips, nic)
@@ -433,47 +448,48 @@
 
 def delete_ip_rules(ip_rules):
     ovn_bgp_agent.privileged.linux_net.delete_ip_rules(ip_rules)
 
 
 def delete_bridge_ip_routes(routing_tables, routing_tables_routes,
                             extra_routes):
-    with pyroute2.NDB() as ndb:
-        for device, routes_info in routing_tables_routes.items():
-            if not extra_routes.get(device):
-                continue
-            for route_info in routes_info:
-                oif = ndb.interfaces[device]['index']
-                if route_info['vlan']:
-                    vlan_device_name = '{}.{}'.format(device,
-                                                      route_info['vlan'])
-                    oif = ndb.interfaces[vlan_device_name]['index']
-                if 'gateway' in route_info['route'].keys():  # subnet route
-                    possible_matchings = [
-                        r for r in extra_routes[device]
-                        if (r['dst'] == route_info['route']['dst'] and
-                            r['dst_len'] == route_info['route']['dst_len'] and
-                            r['gateway'] == route_info['route']['gateway'])]
-                else:  # cr-lrp
-                    possible_matchings = [
-                        r for r in extra_routes[device]
-                        if (r['dst'] == route_info['route']['dst'] and
-                            r['dst_len'] == route_info['route']['dst_len'] and
-                            r['oif'] == oif)]
-                for r in possible_matchings:
-                    extra_routes[device].remove(r)
+    for device, routes_info in routing_tables_routes.items():
+        if not extra_routes.get(device):
+            continue
+        for route_info in routes_info:
+            oif = get_interface_index(device)
+            if route_info['vlan']:
+                vlan_device_name = '{}.{}'.format(device,
+                                                  route_info['vlan'])
+                oif = get_interface_index(vlan_device_name)
+            if 'gateway' in route_info['route'].keys():  # subnet route
+                possible_matchings = [
+                    r for r in extra_routes[device]
+                    if (r.get_attr('RTA_DST') == route_info['route']['dst'] and
+                        r['dst_len'] == route_info['route']['dst_len'] and
+                        r.get_attr('RTA_GATEWAY') == route_info['route'][
+                            'gateway'])]
+            else:  # cr-lrp
+                possible_matchings = [
+                    r for r in extra_routes[device]
+                    if (r.get_attr('RTA_DST') == route_info['route']['dst'] and
+                        r['dst_len'] == route_info['route']['dst_len'] and
+                        r.get_attr('RTA_OIF') == oif)]
+            for r in possible_matchings:
+                extra_routes[device].remove(r)
 
     for bridge, routes in extra_routes.items():
         for route in routes:
-            r_info = {'dst': route['dst'],
+            r_info = {'dst': route.get_attr('RTA_DST'),
                       'dst_len': route['dst_len'],
                       'family': route['family'],
-                      'oif': route['oif'],
-                      'gateway': route['gateway'],
+                      'oif': route.get_attr('RTA_OIF'),
                       'table': routing_tables[bridge]}
+            if route.get_attr('RTA_GATEWAY'):
+                r_info['gateway'] = route.get_attr('RTA_GATEWAY')
             ovn_bgp_agent.privileged.linux_net.route_delete(r_info)
 
 
 def delete_routes_from_table(table):
     table_routes = _get_table_routes(table)
     delete_ip_routes(table_routes)
 
@@ -481,31 +497,37 @@
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def _get_table_routes(table):
-    with pyroute2.NDB() as ndb:
-        # FIXME: problem in pyroute2 removing routes with local (254) scope
-        return [r for r in ndb.routes.dump().filter(table=table)
-                if r.scope != 254 and r.proto != 186]
+    with pyroute2.IPRoute() as ipr:
+        return [
+            r for r in ipr.get_routes(table=table)
+            if r['scope'] != 254 and r['proto'] != 186
+        ]
 
 
 @tenacity.retry(
     retry=tenacity.retry_if_exception_type(
         netlink_exceptions.NetlinkDumpInterrupted),
     wait=tenacity.wait_exponential(multiplier=0.02, max=1),
     stop=tenacity.stop_after_delay(8),
     reraise=True)
 def get_routes_on_tables(table_ids):
-    with pyroute2.NDB() as ndb:
-        # NOTE: skip bgp routes (proto 186)
-        return [r for r in ndb.routes.dump()
-                if r.table in table_ids and r.dst != '' and r.proto != 186]
+    routes = []
+    with pyroute2.IPRoute() as ipr:
+        for table_id in table_ids:
+            table_routes = [
+                r for r in ipr.get_routes(table=table_id)
+                if r.get_attr('RTA_DST') and r['proto'] != 186
+            ]
+            routes.extend(table_routes)
+    return routes
 
 
 def delete_ip_routes(routes):
     for route in routes:
         r_info = {'dst': route['dst'],
                   'dst_len': route['dst_len'],
                   'family': route['family'],
@@ -524,31 +546,28 @@
 
 
 def add_ips_to_dev(nic, ips, clear_local_route_at_table=False):
     already_added_ips = []
     for ip in ips:
         try:
             ovn_bgp_agent.privileged.linux_net.add_ip_to_dev(ip, nic)
-        except KeyError:
-            # NDB raises KeyError: 'object exists'
-            # if the ip is already added
+        except agent_exc.IpAddressAlreadyExists:
             already_added_ips.append(ip)
 
     if clear_local_route_at_table:
         for ip in ips:
             if ip in already_added_ips:
                 continue
-            with pyroute2.NDB() as ndb:
-                oif = ndb.interfaces[nic]['index']
-                route = {'table': clear_local_route_at_table,
-                         'proto': 2,
-                         'scope': 254,
-                         'dst': ip,
-                         'oif': oif}
-                ovn_bgp_agent.privileged.linux_net.route_delete(route)
+            oif = get_interface_index(nic)
+            route = {'table': clear_local_route_at_table,
+                     'proto': 2,
+                     'scope': 254,
+                     'dst': ip,
+                     'oif': oif}
+            ovn_bgp_agent.privileged.linux_net.route_delete(route)
 
 
 def del_ips_from_dev(nic, ips):
     for ip in ips:
         ovn_bgp_agent.privileged.linux_net.del_ip_from_dev(ip, nic)
 
 
@@ -577,16 +596,14 @@
 def add_ip_nei(ip, lladdr, dev):
     """Add ip neighbor permament entry
 
     param ip: IP of the neighbor to add an entry for
     param lladdr: link layer address of the neighbor to associate to that IP
     param dev: the interface to which the neighbor is attached
     """
-    # FIXME: There is no support for creating neighbours in NDB
-    # So we are using iproute here
     ovn_bgp_agent.privileged.linux_net.add_ip_nei(ip, lladdr, dev)
 
 
 def del_ip_rule(ip, table, dev=None, lladdr=None):
     ip_version = get_ip_version(ip)
     ip_info = ip.split("/")
 
@@ -611,23 +628,27 @@
 def del_ip_nei(ip, lladdr, dev):
     """Del ip neighbor permament entry
 
     param ip: IP of the neighbor to delete the entry
     param lladdr: link layer address of the neighbor to disassociate
     param dev: the interface to which the neighbor is attached
     """
-    # FIXME: There is no support for deleting neighbours in NDB
-    # So we are using iproute here
     ovn_bgp_agent.privileged.linux_net.del_ip_nei(ip, lladdr, dev)
 
 
 def add_unreachable_route(vrf_name):
     ovn_bgp_agent.privileged.linux_net.add_unreachable_route(vrf_name)
 
 
+@tenacity.retry(
+    retry=tenacity.retry_if_exception_type(
+        netlink_exceptions.NetlinkDumpInterrupted),
+    wait=tenacity.wait_exponential(multiplier=0.02, max=1),
+    stop=tenacity.stop_after_delay(8),
+    reraise=True)
 def add_ip_route(ovn_routing_tables_routes, ip_address, route_table, dev,
                  vlan=None, mask=None, via=None):
     net_ip = ip_address
     if not mask:  # default /32 or /128
         if get_ip_version(ip_address) == constants.IP_VERSION_6:
             mask = 128
         else:
@@ -637,48 +658,46 @@
         if get_ip_version(ip_address) == constants.IP_VERSION_6:
             net_ip = '{}'.format(ipaddress.IPv6Network(
                 ip, strict=False).network_address)
         else:
             net_ip = '{}'.format(ipaddress.IPv4Network(
                 ip, strict=False).network_address)
 
-    with pyroute2.NDB() as ndb:
-        if vlan:
-            oif_name = '{}.{}'.format(dev, vlan)
-            try:
-                oif = ndb.interfaces[oif_name]['index']
-            except KeyError:
-                # Most provider network was recently created an
-                # there has not been a sync since then, therefore
-                # the vlan device has not yet been created
-                # Trying to create the device and retrying
-                ensure_vlan_device_for_network(dev, vlan)
-                oif = ndb.interfaces[oif_name]['index']
-        else:
-            oif = ndb.interfaces[dev]['index']
+    if vlan:
+        oif_name = '{}.{}'.format(dev, vlan)
+        try:
+            oif = get_interface_index(oif_name)
+        except agent_exc.NetworkInterfaceNotFound:
+            # Most provider network was recently created an
+            # there has not been a sync since then, therefore
+            # the vlan device has not yet been created
+            # Trying to create the device and retrying
+            ensure_vlan_device_for_network(dev, vlan)
+            oif = get_interface_index(oif_name)
+    else:
+        oif = get_interface_index(dev)
 
     route = {'dst': net_ip, 'dst_len': int(mask), 'oif': oif,
              'table': int(route_table), 'proto': 3}
     if via:
         route['gateway'] = via
         route['scope'] = 0
     else:
         route['scope'] = 253
     if get_ip_version(net_ip) == constants.IP_VERSION_6:
         route['family'] = AF_INET6
         del route['scope']
 
-    with pyroute2.NDB() as ndb:
-        try:
-            with ndb.routes[route]:
-                LOG.debug("Route already existing: %s", route)
-        except KeyError:
+    with pyroute2.IPRoute() as ipr:
+        if not ipr.route('show', **route):
             LOG.debug("Creating route at table %s: %s", route_table, route)
             ovn_bgp_agent.privileged.linux_net.route_create(route)
             LOG.debug("Route created at table %s: %s", route_table, route)
+        else:
+            LOG.debug("Route already existing: %s", route)
     route_info = {'vlan': vlan, 'route': route}
     ovn_routing_tables_routes.setdefault(dev, []).append(route_info)
 
 
 def del_ip_route(ovn_routing_tables_routes, ip_address, route_table, dev,
                  vlan=None, mask=None, via=None):
     net_ip = ip_address
@@ -692,26 +711,25 @@
         if get_ip_version(ip_address) == constants.IP_VERSION_6:
             net_ip = '{}'.format(ipaddress.IPv6Network(
                 ip, strict=False).network_address)
         else:
             net_ip = '{}'.format(ipaddress.IPv4Network(
                 ip, strict=False).network_address)
 
-    with pyroute2.NDB() as ndb:
-        try:
-            if vlan:
-                oif_name = '{}.{}'.format(dev, vlan)
-                oif = ndb.interfaces[oif_name]['index']
-            else:
-                oif = ndb.interfaces[dev]['index']
-        except KeyError:
-            LOG.debug("Device %s does not exists, so the associated "
-                      "routes should have been automatically deleted.", dev)
-            ovn_routing_tables_routes.pop(dev, None)
-            return
+    try:
+        if vlan:
+            oif_name = '{}.{}'.format(dev, vlan)
+            oif = get_interface_index(oif_name)
+        else:
+            oif = get_interface_index(dev)
+    except agent_exc.NetworkInterfaceNotFound:
+        LOG.debug("Device %s does not exists, so the associated "
+                  "routes should have been automatically deleted.", dev)
+        ovn_routing_tables_routes.pop(dev, None)
+        return
 
     route = {'dst': net_ip, 'dst_len': int(mask), 'oif': oif,
              'table': int(route_table), 'proto': 3}
     if via:
         route['gateway'] = via
         route['scope'] = 0
     else:
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/PKG-INFO` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.2
 Name: ovn-bgp-agent
-Version: 0.4.0
+Version: 1.0.0.0b1
 Summary: The OVN BGP Agent allows to expose VMs/Containers/Networks through BGP on OVN
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =============
         OVN BGP Agent
         =============
         
         The OVN BGP Agent allows to expose VMs/Containers through BGP on OVN
         
         * Free software: Apache license
-        * Documentation: https://ovn-bgp-agent.readthedocs.io
+        * Documentation: https://docs.openstack.org/ovn-bgp-agent
         * Source: https://opendev.org/openstack/ovn-bgp-agent
         * Bugs: https://bugs.launchpad.net/ovn-bgp-agent
         
         Features
         --------
         
         * Expose VMs with FIPs or on Provider Networks through BGP on OVN
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/SOURCES.txt` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,20 @@
 ovn_bgp_agent/privileged/linux_net.py
 ovn_bgp_agent/privileged/ovs_vsctl.py
 ovn_bgp_agent/privileged/vtysh.py
 ovn_bgp_agent/tests/__init__.py
 ovn_bgp_agent/tests/base.py
 ovn_bgp_agent/tests/test_ovn_bgp_agent.py
 ovn_bgp_agent/tests/utils.py
+ovn_bgp_agent/tests/functional/__init__.py
+ovn_bgp_agent/tests/functional/base.py
+ovn_bgp_agent/tests/functional/privileged/__init__.py
+ovn_bgp_agent/tests/functional/privileged/test_linux_net.py
+ovn_bgp_agent/tests/functional/utils/__init__.py
+ovn_bgp_agent/tests/functional/utils/test_linux_net.py
 ovn_bgp_agent/tests/unit/__init__.py
 ovn_bgp_agent/tests/unit/fakes.py
 ovn_bgp_agent/tests/unit/test_agent.py
 ovn_bgp_agent/tests/unit/cmd/__init__.py
 ovn_bgp_agent/tests/unit/cmd/test_agent.py
 ovn_bgp_agent/tests/unit/drivers/__init__.py
 ovn_bgp_agent/tests/unit/drivers/openstack/__init__.py
@@ -89,16 +95,18 @@
 ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py
 ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py
 ovn_bgp_agent/tests/unit/privileged/__init__.py
 ovn_bgp_agent/tests/unit/privileged/test_linux_net.py
 ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py
 ovn_bgp_agent/tests/unit/privileged/test_vtysh.py
 ovn_bgp_agent/tests/unit/utils/__init__.py
+ovn_bgp_agent/tests/unit/utils/test_helpers.py
 ovn_bgp_agent/tests/unit/utils/test_linux_net.py
 ovn_bgp_agent/utils/__init__.py
+ovn_bgp_agent/utils/helpers.py
 ovn_bgp_agent/utils/linux_net.py
 releasenotes/notes/.placeholder
 releasenotes/notes/nb_driver-cc7098183fcedb0a.yaml
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/_static/.placeholder
```

### Comparing `ovn-bgp-agent-0.4.0/ovn_bgp_agent.egg-info/entry_points.txt` & `ovn-bgp-agent-1.0.0.0b1/ovn_bgp_agent.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/releasenotes/source/conf.py` & `ovn-bgp-agent-1.0.0.0b1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/requirements.txt` & `ovn-bgp-agent-1.0.0.0b1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/setup.cfg` & `ovn-bgp-agent-1.0.0.0b1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/setup.py` & `ovn-bgp-agent-1.0.0.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-0.4.0/tox.ini` & `ovn-bgp-agent-1.0.0.0b1/tox.ini`

 * *Files 26% similar despite different names*

```diff
@@ -5,42 +5,50 @@
 ignore_basepython_conflict = true
 
 
 [testenv]
 basepython = python3
 usedevelop = True
 setenv =
+   VIRTUAL_ENV={envdir}
    PYTHONWARNINGS=default::DeprecationWarning
    OS_STDOUT_CAPTURE=1
    OS_STDERR_CAPTURE=1
    OS_TEST_TIMEOUT=60
 deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/test-requirements.txt
-commands = stestr run {posargs}
+commands = stestr run --exclude-regex ".tests.functional" {posargs}
 
 [testenv:lower-constraints]
 deps = -c{toxinidir}/lower-constraints.txt
        -r{toxinidir}/test-requirements.txt
 
 [testenv:pep8]
 commands = flake8 {posargs}
 
 [testenv:venv]
 commands = {posargs}
 
+[testenv:functional]
+envdir = {toxworkdir}/functional
+setenv =
+  {[testenv]setenv}
+commands =
+  stestr run --exclude-regex ".tests.unit" {posargs}
+
 [testenv:cover]
 setenv =
     VIRTUAL_ENV={envdir}
     PYTHON=coverage run --source ovn_bgp_agent --parallel-mode
 commands =
-    stestr run {posargs}
+    stestr run --exclude-regex ".tests.functional" {posargs}
     coverage combine
     coverage html -d cover --omit='*tests*'
     coverage xml -o cover/coverage.xml --omit='*tests*'
-    coverage report --fail-under=92 --skip-covered --omit='*tests*'
+    coverage report --fail-under=85 --skip-covered --omit='*tests*'
 
 [testenv:docs]
 deps = -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:releasenotes]
 deps = {[testenv:docs]deps}
```

