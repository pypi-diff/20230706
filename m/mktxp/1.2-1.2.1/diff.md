# Comparing `tmp/mktxp-1.2.tar.gz` & `tmp/mktxp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mktxp-1.2.tar", last modified: Wed Feb  8 07:31:55 2023, max compression
+gzip compressed data, was "mktxp-1.2.1.tar", last modified: Thu Jul  6 09:15:34 2023, max compression
```

## Comparing `mktxp-1.2.tar` & `mktxp-1.2.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.695648 mktxp-1.2/
--rw-r--r--   0 akpower    (501) staff       (20)      543 2023-02-08 07:31:34.000000 mktxp-1.2/LICENSE
--rw-r--r--   0 akpower    (501) staff       (20)    21103 2023-02-08 07:31:55.695499 mktxp-1.2/PKG-INFO
--rw-r--r--   0 akpower    (501) staff       (20)    20050 2023-02-08 07:31:34.000000 mktxp-1.2/README.md
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.685975 mktxp-1.2/mktxp/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/__init__.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.687201 mktxp-1.2/mktxp/cli/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/__init__.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.687424 mktxp-1.2/mktxp/cli/checks/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/checks/__init__.py
--rwxr-xr-x   0 akpower    (501) staff       (20)     1358 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/checks/chk_pv.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.687923 mktxp-1.2/mktxp/cli/config/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/config/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     1452 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/config/_mktxp.conf
--rwxr-xr-x   0 akpower    (501) staff       (20)    17329 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/config/config.py
--rw-r--r--   0 akpower    (501) staff       (20)     2616 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/config/mktxp.conf
--rwxr-xr-x   0 akpower    (501) staff       (20)     3777 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/dispatch.py
--rwxr-xr-x   0 akpower    (501) staff       (20)    11089 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/options.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.688499 mktxp-1.2/mktxp/cli/output/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/output/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2583 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/output/capsman_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2011 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/output/conn_stats_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2547 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/output/dhcp_out.py
--rw-r--r--   0 akpower    (501) staff       (20)     2815 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/cli/output/wifi_out.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.691273 mktxp-1.2/mktxp/collector/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     3100 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/bandwidth_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2804 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/base_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4886 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/capsman_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2039 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/connection_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3122 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/dhcp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4088 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/firewall_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2637 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/health_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1194 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/identity_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3554 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/interface_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1348 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/ipv6_neighbor_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1144 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/mktxp_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     3828 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/monitor_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1461 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/netwatch_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1272 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/package_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1310 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/poe_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2326 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/pool_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1448 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/public_ip_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4067 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/queue_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4020 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/resource_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     2888 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/route_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     1216 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/user_collector.py
--rw-r--r--   0 akpower    (501) staff       (20)     4659 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/collector/wlan_collector.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.693966 mktxp-1.2/mktxp/datasource/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     1897 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/base_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     4059 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/capsman_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3863 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/connection_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2670 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/dhcp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3508 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/firewall_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1880 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/health_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1321 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/identity_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3805 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/interface_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)      962 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/ipv6_neighbor_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1169 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/mktxp_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2102 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/netwatch_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1980 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/package_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     3150 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/poe_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1987 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/pool_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1211 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/public_ip_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2120 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/queue_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1306 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/route_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1340 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/routerboard_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1352 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/system_resource_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     1330 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/user_ds.py
--rw-r--r--   0 akpower    (501) staff       (20)     2551 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/datasource/wireless_ds.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.694697 mktxp-1.2/mktxp/flow/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     6060 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/collector_handler.py
--rw-r--r--   0 akpower    (501) staff       (20)     4189 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/collector_registry.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.695044 mktxp-1.2/mktxp/flow/processor/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/processor/__init__.py
--rw-r--r--   0 akpower    (501) staff       (20)     2719 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/processor/base_proc.py
--rw-r--r--   0 akpower    (501) staff       (20)     8070 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/processor/output.py
--rw-r--r--   0 akpower    (501) staff       (20)     5478 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/router_connection.py
--rw-r--r--   0 akpower    (501) staff       (20)     2392 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/router_entries_handler.py
--rw-r--r--   0 akpower    (501) staff       (20)     4496 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/flow/router_entry.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.695262 mktxp-1.2/mktxp/utils/
--rw-r--r--   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/utils/__init__.py
--rwxr-xr-x   0 akpower    (501) staff       (20)     9182 2023-02-08 07:31:34.000000 mktxp-1.2/mktxp/utils/utils.py
-drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-02-08 07:31:55.686831 mktxp-1.2/mktxp.egg-info/
--rw-r--r--   0 akpower    (501) staff       (20)    21103 2023-02-08 07:31:55.000000 mktxp-1.2/mktxp.egg-info/PKG-INFO
--rw-r--r--   0 akpower    (501) staff       (20)     2480 2023-02-08 07:31:55.000000 mktxp-1.2/mktxp.egg-info/SOURCES.txt
--rw-r--r--   0 akpower    (501) staff       (20)        1 2023-02-08 07:31:55.000000 mktxp-1.2/mktxp.egg-info/dependency_links.txt
--rw-r--r--   0 akpower    (501) staff       (20)       50 2023-02-08 07:31:55.000000 mktxp-1.2/mktxp.egg-info/entry_points.txt
--rw-r--r--   0 akpower    (501) staff       (20)      117 2023-02-08 07:31:55.000000 mktxp-1.2/mktxp.egg-info/requires.txt
--rw-r--r--   0 akpower    (501) staff       (20)        6 2023-02-08 07:31:55.000000 mktxp-1.2/mktxp.egg-info/top_level.txt
--rw-r--r--   0 akpower    (501) staff       (20)        1 2023-02-08 07:31:55.000000 mktxp-1.2/mktxp.egg-info/zip-safe
--rw-r--r--   0 akpower    (501) staff       (20)       38 2023-02-08 07:31:55.695691 mktxp-1.2/setup.cfg
--rwxr-xr-x   0 akpower    (501) staff       (20)     2535 2023-02-08 07:31:34.000000 mktxp-1.2/setup.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.319173 mktxp-1.2.1/
+-rw-r--r--   0 akpower    (501) staff       (20)      543 2023-06-11 16:02:43.000000 mktxp-1.2.1/LICENSE
+-rw-r--r--   0 akpower    (501) staff       (20)    21175 2023-07-06 09:15:34.319025 mktxp-1.2.1/PKG-INFO
+-rw-r--r--   0 akpower    (501) staff       (20)    20120 2023-06-30 09:18:00.000000 mktxp-1.2.1/README.md
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.307128 mktxp-1.2.1/mktxp/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/__init__.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.308449 mktxp-1.2.1/mktxp/cli/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/__init__.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.308906 mktxp-1.2.1/mktxp/cli/checks/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/checks/__init__.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)     1358 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/checks/chk_pv.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.309653 mktxp-1.2.1/mktxp/cli/config/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/config/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1456 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/config/_mktxp.conf
+-rwxr-xr-x   0 akpower    (501) staff       (20)    17442 2023-06-30 09:07:49.000000 mktxp-1.2.1/mktxp/cli/config/config.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2686 2023-06-30 09:07:49.000000 mktxp-1.2.1/mktxp/cli/config/mktxp.conf
+-rwxr-xr-x   0 akpower    (501) staff       (20)     3777 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/dispatch.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)    11095 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/options.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.310535 mktxp-1.2.1/mktxp/cli/output/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/output/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2583 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/output/capsman_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2011 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/output/conn_stats_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2547 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/output/dhcp_out.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2815 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/cli/output/wifi_out.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.314050 mktxp-1.2.1/mktxp/collector/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3100 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/bandwidth_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2804 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/base_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4931 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/capsman_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2039 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/connection_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3122 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/dhcp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4122 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/firewall_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2925 2023-07-01 10:16:09.000000 mktxp-1.2.1/mktxp/collector/health_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1194 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/identity_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3554 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/interface_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1348 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/ipv6_neighbor_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1144 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/mktxp_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3828 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/monitor_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1461 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/netwatch_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1272 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/package_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1310 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/poe_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2326 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/pool_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1448 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/public_ip_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4067 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/queue_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4686 2023-06-30 09:07:49.000000 mktxp-1.2.1/mktxp/collector/resource_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2888 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/route_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1216 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/user_collector.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4734 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/collector/wlan_collector.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.317200 mktxp-1.2.1/mktxp/datasource/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1897 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/base_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4059 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/capsman_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3863 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/connection_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2670 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/dhcp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3508 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/firewall_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1880 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/health_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1321 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/identity_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3805 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/interface_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)      962 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/ipv6_neighbor_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1169 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/mktxp_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2102 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/netwatch_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1980 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/package_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     3150 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/poe_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1987 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/pool_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1211 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/public_ip_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2120 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/queue_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1306 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/route_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1340 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/routerboard_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1352 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/system_resource_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     1330 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/user_ds.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2551 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/datasource/wireless_ds.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.318014 mktxp-1.2.1/mktxp/flow/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     6060 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/collector_handler.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4189 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/collector_registry.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.318408 mktxp-1.2.1/mktxp/flow/processor/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/processor/__init__.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2719 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/processor/base_proc.py
+-rw-r--r--   0 akpower    (501) staff       (20)     8160 2023-06-30 08:54:49.000000 mktxp-1.2.1/mktxp/flow/processor/output.py
+-rw-r--r--   0 akpower    (501) staff       (20)     5478 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/router_connection.py
+-rw-r--r--   0 akpower    (501) staff       (20)     2392 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/router_entries_handler.py
+-rw-r--r--   0 akpower    (501) staff       (20)     4496 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/flow/router_entry.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.318771 mktxp-1.2.1/mktxp/utils/
+-rw-r--r--   0 akpower    (501) staff       (20)        0 2023-06-11 16:02:43.000000 mktxp-1.2.1/mktxp/utils/__init__.py
+-rwxr-xr-x   0 akpower    (501) staff       (20)    11954 2023-06-30 09:07:49.000000 mktxp-1.2.1/mktxp/utils/utils.py
+drwxr-xr-x   0 akpower    (501) staff       (20)        0 2023-07-06 09:15:34.307982 mktxp-1.2.1/mktxp.egg-info/
+-rw-r--r--   0 akpower    (501) staff       (20)    21175 2023-07-06 09:15:34.000000 mktxp-1.2.1/mktxp.egg-info/PKG-INFO
+-rw-r--r--   0 akpower    (501) staff       (20)     2480 2023-07-06 09:15:34.000000 mktxp-1.2.1/mktxp.egg-info/SOURCES.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        1 2023-07-06 09:15:34.000000 mktxp-1.2.1/mktxp.egg-info/dependency_links.txt
+-rw-r--r--   0 akpower    (501) staff       (20)       50 2023-07-06 09:15:34.000000 mktxp-1.2.1/mktxp.egg-info/entry_points.txt
+-rw-r--r--   0 akpower    (501) staff       (20)      117 2023-07-06 09:15:34.000000 mktxp-1.2.1/mktxp.egg-info/requires.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        6 2023-07-06 09:15:34.000000 mktxp-1.2.1/mktxp.egg-info/top_level.txt
+-rw-r--r--   0 akpower    (501) staff       (20)        1 2023-07-06 09:15:34.000000 mktxp-1.2.1/mktxp.egg-info/zip-safe
+-rw-r--r--   0 akpower    (501) staff       (20)       38 2023-07-06 09:15:34.319216 mktxp-1.2.1/setup.cfg
+-rwxr-xr-x   0 akpower    (501) staff       (20)     2537 2023-07-06 09:12:58.000000 mktxp-1.2.1/setup.py
```

### Comparing `mktxp-1.2/LICENSE` & `mktxp-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/PKG-INFO` & `mktxp-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktxp
-Version: 1.2
+Version: 1.2.1
 Summary: Prometheus Exporter for Mikrotik RouterOS devices
 Home-page: https://github.com/akpw/mktxp
 Author: Arseniy Kuznetsov
 Author-email: k.arseniy@gmail.com
 License: GNU General Public License v2 (GPLv2)
 Keywords: Mikrotik RouterOS Prometheus Exporter
 Classifier: Development Status :: 4 - Beta
@@ -114,15 +114,17 @@
     capsman_clients = True          # CAPsMAN clients metrics    
 
     user = True                     # Active Users metrics
     queue = True                    # Queues metrics
     
     remote_dhcp_entry = None        # An MKTXP entry for remote DHCP info resolution (capsman/wireless)
 
-    use_comments_over_names = True  # when available, forces using comments over the interfaces names 
+    use_comments_over_names = True  # when available, forces using comments over the interfaces names
+
+    check_for_updates = False       # check for available ROS updates
 ```
 
 Most options are easy to understand at first glance, and some are described in more details [later](https://github.com/akpw/mktxp#advanced-features).
 
 
 #### Local install
 If you have a local MKTXP installation, you can edit the configuration file with your default system editor directly from mktxp:
@@ -236,16 +238,16 @@
     port = 49090                    
     socket_timeout = 2
     
     initial_delay_on_failure = 120
     max_delay_on_failure = 900
     delay_inc_div = 5
 
-    bandwidth = True                # Turns metrics bandwidth metrics collection on / off    
-    bandwidth_test_interval = 420   # Interval for colllecting bandwidth metrics
+    bandwidth = False               # Turns metrics bandwidth metrics collection on / off    
+    bandwidth_test_interval = 600   # Interval for colllecting bandwidth metrics
     minimal_collect_interval = 5    # Minimal metric collection interval
 
     verbose_mode = False            # Set it on for troubleshooting
 
     fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
     max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
```

### Comparing `mktxp-1.2/README.md` & `mktxp-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,17 @@
     capsman_clients = True          # CAPsMAN clients metrics    
 
     user = True                     # Active Users metrics
     queue = True                    # Queues metrics
     
     remote_dhcp_entry = None        # An MKTXP entry for remote DHCP info resolution (capsman/wireless)
 
-    use_comments_over_names = True  # when available, forces using comments over the interfaces names 
+    use_comments_over_names = True  # when available, forces using comments over the interfaces names
+
+    check_for_updates = False       # check for available ROS updates
 ```
 
 Most options are easy to understand at first glance, and some are described in more details [later](https://github.com/akpw/mktxp#advanced-features).
 
 
 #### Local install
 If you have a local MKTXP installation, you can edit the configuration file with your default system editor directly from mktxp:
@@ -210,16 +212,16 @@
     port = 49090                    
     socket_timeout = 2
     
     initial_delay_on_failure = 120
     max_delay_on_failure = 900
     delay_inc_div = 5
 
-    bandwidth = True                # Turns metrics bandwidth metrics collection on / off    
-    bandwidth_test_interval = 420   # Interval for colllecting bandwidth metrics
+    bandwidth = False               # Turns metrics bandwidth metrics collection on / off    
+    bandwidth_test_interval = 600   # Interval for colllecting bandwidth metrics
     minimal_collect_interval = 5    # Minimal metric collection interval
 
     verbose_mode = False            # Set it on for troubleshooting
 
     fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
     max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
```

### Comparing `mktxp-1.2/mktxp/cli/checks/chk_pv.py` & `mktxp-1.2.1/mktxp/cli/checks/chk_pv.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/cli/config/_mktxp.conf` & `mktxp-1.2.1/mktxp/cli/config/_mktxp.conf`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     port = 49090
     socket_timeout = 2
     
     initial_delay_on_failure = 120
     max_delay_on_failure = 900
     delay_inc_div = 5
 
-    bandwidth = True                # Turns metrics bandwidth metrics collection on / off    
-    bandwidth_test_interval = 420   # Interval for colllecting bandwidth metrics
-    minimal_collect_interval = 5    # Minimal metric collection interval
+    bandwidth = False                # Turns metrics bandwidth metrics collection on / off    
+    bandwidth_test_interval = 600    # Interval for colllecting bandwidth metrics
+    minimal_collect_interval = 5     # Minimal metric collection interval
 
-    verbose_mode = False            # Set it on for troubleshooting
+    verbose_mode = False             # Set it on for troubleshooting
 
     fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
     max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
     total_max_scrape_duration = 30      # Max overall duration of all metrics collection (parallel fetch only)
```

### Comparing `mktxp-1.2/mktxp/cli/config/config.py` & `mktxp-1.2.1/mktxp/cli/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     FE_PUBLIC_IP_KEY = 'public_ip'
     FE_NETWATCH_KEY = 'netwatch'
 
     FE_USER_KEY = 'user'
     FE_QUEUE_KEY = 'queue'
     FE_REMOTE_DHCP_ENTRY = 'remote_dhcp_entry'
 
+    FE_CHECK_FOR_UPDATES = 'check_for_updates'
+
     MKTXP_SOCKET_TIMEOUT = 'socket_timeout'
     MKTXP_INITIAL_DELAY = 'initial_delay_on_failure'
     MKTXP_MAX_DELAY = 'max_delay_on_failure'
     MKTXP_INC_DIV = 'delay_inc_div'
     MKTXP_BANDWIDTH_KEY = 'bandwidth'
     MKTXP_BANDWIDTH_TEST_INTERVAL = 'bandwidth_test_interval'
     MKTXP_VERBOSE_MODE = 'verbose_mode'
@@ -123,25 +125,25 @@
     DEFAULT_MKTXP_MIN_COLLECT_INTERVAL = 5
     DEFAULT_MKTXP_FETCH_IN_PARALLEL = False
     DEFAULT_MKTXP_MAX_WORKER_THREADS = 5
     DEFAULT_MKTXP_MAX_SCRAPE_DURATION = 10
     DEFAULT_MKTXP_TOTAL_MAX_SCRAPE_DURATION = 30
 
 
-    BOOLEAN_KEYS_NO = {ENABLED_KEY, SSL_KEY, NO_SSL_CERTIFICATE,
+    BOOLEAN_KEYS_NO = {ENABLED_KEY, SSL_KEY, NO_SSL_CERTIFICATE, FE_CHECK_FOR_UPDATES,
                        SSL_CERTIFICATE_VERIFY, FE_IPV6_FIREWALL_KEY, FE_IPV6_NEIGHBOR_KEY, FE_CONNECTION_STATS_KEY}
 
     # Feature keys enabled by default
     BOOLEAN_KEYS_YES = {FE_DHCP_KEY, FE_PACKAGE_KEY, FE_DHCP_LEASE_KEY, FE_DHCP_POOL_KEY, FE_IP_CONNECTIONS_KEY, FE_INTERFACE_KEY, FE_FIREWALL_KEY,
                         FE_MONITOR_KEY, FE_ROUTE_KEY, MKTXP_USE_COMMENTS_OVER_NAMES,
                         FE_WIRELESS_KEY, FE_WIRELESS_CLIENTS_KEY, FE_CAPSMAN_KEY, FE_CAPSMAN_CLIENTS_KEY, FE_POE_KEY,
                         FE_NETWATCH_KEY, FE_PUBLIC_IP_KEY, FE_USER_KEY, FE_QUEUE_KEY}
 
-    SYSTEM_BOOLEAN_KEYS_YES = {MKTXP_BANDWIDTH_KEY}
-    SYSTEM_BOOLEAN_KEYS_NO = {MKTXP_VERBOSE_MODE, MKTXP_FETCH_IN_PARALLEL}
+    SYSTEM_BOOLEAN_KEYS_YES = set()
+    SYSTEM_BOOLEAN_KEYS_NO = {MKTXP_BANDWIDTH_KEY, MKTXP_VERBOSE_MODE, MKTXP_FETCH_IN_PARALLEL}
 
     STR_KEYS = (HOST_KEY, USER_KEY, PASSWD_KEY, FE_REMOTE_DHCP_ENTRY)
     INT_KEYS =  ()
     MKTXP_INT_KEYS = (PORT_KEY, MKTXP_SOCKET_TIMEOUT, MKTXP_INITIAL_DELAY, MKTXP_MAX_DELAY,
                       MKTXP_INC_DIV, MKTXP_BANDWIDTH_TEST_INTERVAL, MKTXP_MIN_COLLECT_INTERVAL,
                       MKTXP_MAX_WORKER_THREADS, MKTXP_MAX_SCRAPE_DURATION, MKTXP_TOTAL_MAX_SCRAPE_DURATION)
 
@@ -153,15 +155,15 @@
     MKTXPConfigEntry = namedtuple('MKTXPConfigEntry', [MKTXPConfigKeys.ENABLED_KEY, MKTXPConfigKeys.HOST_KEY, MKTXPConfigKeys.PORT_KEY,
                                                        MKTXPConfigKeys.USER_KEY, MKTXPConfigKeys.PASSWD_KEY,
                                                        MKTXPConfigKeys.SSL_KEY, MKTXPConfigKeys.NO_SSL_CERTIFICATE, MKTXPConfigKeys.SSL_CERTIFICATE_VERIFY,
                                                        MKTXPConfigKeys.FE_DHCP_KEY, MKTXPConfigKeys.FE_PACKAGE_KEY, MKTXPConfigKeys.FE_DHCP_LEASE_KEY, MKTXPConfigKeys.FE_DHCP_POOL_KEY, MKTXPConfigKeys.FE_INTERFACE_KEY,
                                                        MKTXPConfigKeys.FE_FIREWALL_KEY, MKTXPConfigKeys.FE_MONITOR_KEY, MKTXPConfigKeys.FE_ROUTE_KEY, MKTXPConfigKeys.FE_WIRELESS_KEY, MKTXPConfigKeys.FE_WIRELESS_CLIENTS_KEY,
                                                        MKTXPConfigKeys.FE_IP_CONNECTIONS_KEY, MKTXPConfigKeys.FE_CONNECTION_STATS_KEY, MKTXPConfigKeys.FE_CAPSMAN_KEY, MKTXPConfigKeys.FE_CAPSMAN_CLIENTS_KEY, MKTXPConfigKeys.FE_POE_KEY, MKTXPConfigKeys.FE_NETWATCH_KEY,
                                                        MKTXPConfigKeys.MKTXP_USE_COMMENTS_OVER_NAMES, MKTXPConfigKeys.FE_PUBLIC_IP_KEY, MKTXPConfigKeys.FE_IPV6_FIREWALL_KEY, MKTXPConfigKeys.FE_IPV6_NEIGHBOR_KEY,
-                                                       MKTXPConfigKeys.FE_USER_KEY, MKTXPConfigKeys.FE_QUEUE_KEY, MKTXPConfigKeys.FE_REMOTE_DHCP_ENTRY
+                                                       MKTXPConfigKeys.FE_USER_KEY, MKTXPConfigKeys.FE_QUEUE_KEY, MKTXPConfigKeys.FE_REMOTE_DHCP_ENTRY, MKTXPConfigKeys.FE_CHECK_FOR_UPDATES
                                                        ])
     MKTXPSystemEntry = namedtuple('MKTXPSystemEntry', [MKTXPConfigKeys.PORT_KEY, MKTXPConfigKeys.MKTXP_SOCKET_TIMEOUT,
                                                        MKTXPConfigKeys.MKTXP_INITIAL_DELAY, MKTXPConfigKeys.MKTXP_MAX_DELAY,
                                                        MKTXPConfigKeys.MKTXP_INC_DIV, MKTXPConfigKeys.MKTXP_BANDWIDTH_KEY,
                                                        MKTXPConfigKeys.MKTXP_VERBOSE_MODE, MKTXPConfigKeys.MKTXP_BANDWIDTH_TEST_INTERVAL,
                                                        MKTXPConfigKeys.MKTXP_MIN_COLLECT_INTERVAL, MKTXPConfigKeys.MKTXP_FETCH_IN_PARALLEL,
                                                        MKTXPConfigKeys.MKTXP_MAX_WORKER_THREADS, MKTXPConfigKeys.MKTXP_MAX_SCRAPE_DURATION,
```

### Comparing `mktxp-1.2/mktxp/cli/config/mktxp.conf` & `mktxp-1.2.1/mktxp/cli/config/mktxp.conf`

 * *Files 2% similar despite different names*

```diff
@@ -49,8 +49,10 @@
     capsman_clients = True          # CAPsMAN clients metrics    
 
     user = True                     # Active Users metrics
     queue = True                    # Queues metrics
     
     remote_dhcp_entry = None        # An MKTXP entry for remote DHCP info resolution (capsman/wireless)
 
-    use_comments_over_names = True  # when available, forces using comments over the interfaces names 
+    use_comments_over_names = True  # when available, forces using comments over the interfaces names
+
+    check_for_updates = False       # check for available ROS updates
```

### Comparing `mktxp-1.2/mktxp/cli/dispatch.py` & `mktxp-1.2.1/mktxp/cli/dispatch.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/cli/options.py` & `mktxp-1.2.1/mktxp/cli/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         else:
             return path_arg
 
     @staticmethod
     def _add_entry_name(parser, registered_only = False, required = True, help = 'MKTXP Entry name'):
         parser.add_argument('-en', '--entry-name', dest = 'entry_name',
             type = str,
-            metavar = config_handler.registered_entries() if registered_only else None,
+            metavar = list(config_handler.registered_entries()) if registered_only else None,
             required = required,
             choices = UniquePartialMatchList(config_handler.registered_entries())if registered_only else None,
             help = help)
 
     @staticmethod
     def _add_entry_groups(parser):
         required_args_group = parser.add_argument_group('Required Arguments')
```

### Comparing `mktxp-1.2/mktxp/cli/output/capsman_out.py` & `mktxp-1.2.1/mktxp/cli/output/capsman_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/cli/output/conn_stats_out.py` & `mktxp-1.2.1/mktxp/cli/output/conn_stats_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/cli/output/dhcp_out.py` & `mktxp-1.2.1/mktxp/cli/output/dhcp_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/cli/output/wifi_out.py` & `mktxp-1.2.1/mktxp/cli/output/wifi_out.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/bandwidth_collector.py` & `mktxp-1.2.1/mktxp/collector/bandwidth_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/base_collector.py` & `mktxp-1.2.1/mktxp/collector/base_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/capsman_collector.py` & `mktxp-1.2.1/mktxp/collector/capsman_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,21 @@
             # the client info metrics
             if router_entry.config_entry.capsman_clients:
 
                 # translate / trim / augment registration records
                 for registration_record in registration_records:
                     BaseOutputProcessor.augment_record(router_entry, registration_record)
                     
-                tx_byte_metrics = BaseCollector.counter_collector('capsman_clients_tx_bytes', 'Number of sent packet bytes', registration_records, 'tx_bytes', ['dhcp_name'])
+                tx_byte_metrics = BaseCollector.counter_collector('capsman_clients_tx_bytes', 'Number of sent packet bytes', registration_records, 'tx_bytes', ['dhcp_name', 'mac_address'])
                 yield tx_byte_metrics
 
-                rx_byte_metrics = BaseCollector.counter_collector('capsman_clients_rx_bytes', 'Number of received packet bytes', registration_records, 'rx_bytes', ['dhcp_name'])
+                rx_byte_metrics = BaseCollector.counter_collector('capsman_clients_rx_bytes', 'Number of received packet bytes', registration_records, 'rx_bytes', ['dhcp_name', 'mac_address'])
                 yield rx_byte_metrics
 
-                signal_strength_metrics = BaseCollector.gauge_collector('capsman_clients_signal_strength', 'Client devices signal strength', registration_records, 'rx_signal', ['dhcp_name'])
+                signal_strength_metrics = BaseCollector.gauge_collector('capsman_clients_signal_strength', 'Client devices signal strength', registration_records, 'rx_signal', ['dhcp_name', 'mac_address'])
                 yield signal_strength_metrics
 
                 registration_metrics = BaseCollector.info_collector('capsman_clients_devices', 'Registered client devices info', 
                                         registration_records, ['dhcp_name', 'dhcp_address', 'rx_signal', 'ssid', 'tx_rate', 'rx_rate', 'interface', 'mac_address', 'uptime'])
                 yield registration_metrics
```

### Comparing `mktxp-1.2/mktxp/collector/connection_collector.py` & `mktxp-1.2.1/mktxp/collector/connection_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/dhcp_collector.py` & `mktxp-1.2.1/mktxp/collector/dhcp_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/firewall_collector.py` & `mktxp-1.2.1/mktxp/collector/firewall_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,12 +53,12 @@
                 metrics_records_ipv6 = [FirewallCollector.metric_record(router_entry, record) for record in firewall_raw_records_ipv6]     
                 firewall_raw_metrics_ipv6 = BaseCollector.counter_collector('firewall_raw_ipv6', 'Total amount of bytes matched by raw firewall rules (IPv6)', metrics_records_ipv6, 'bytes', ['name', 'log'])
                 yield firewall_raw_metrics_ipv6
 
     # Helpers
     @staticmethod
     def metric_record(router_entry, firewall_record):
-        name = f"| {firewall_record['chain']} | {firewall_record['action']} | {firewall_record['comment']}"
-        bytes = firewall_record['bytes']
+        name = f"| {firewall_record.get('chain', ' ')} | {firewall_record.get('action', ' ')} | {firewall_record.get('comment', ' ')}"
+        bytes = firewall_record.get('bytes', 0)
         return {MKTXPConfigKeys.ROUTERBOARD_NAME: router_entry.router_id[MKTXPConfigKeys.ROUTERBOARD_NAME],
                 MKTXPConfigKeys.ROUTERBOARD_ADDRESS: router_entry.router_id[MKTXPConfigKeys.ROUTERBOARD_ADDRESS],
                 'name': name, 'log': firewall_record['log'], 'bytes': bytes}
```

### Comparing `mktxp-1.2/mktxp/collector/health_collector.py` & `mktxp-1.2.1/mktxp/collector/health_collector.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 class HealthCollector(BaseCollector):
     ''' System Health Metrics collector
     '''    
     @staticmethod
     def collect(router_entry):
-        health_labels = ['voltage', 'temperature', 'cpu_temperature', 'fan1_speed', 'fan2_speed', 'power_consumption']
+        health_labels = ['voltage', 'temperature', 'cpu_temperature', 'switch_temperature', 'fan1_speed', 'fan2_speed', 'power_consumption']
         health_records = HealthMetricsDataSource.metric_records(router_entry, metric_labels = health_labels)   
         if health_records:
             for record in health_records:
 
                 if 'voltage' in record:
                     voltage_metrics = BaseCollector.gauge_collector('system_routerboard_voltage', 'Supplied routerboard voltage', [record, ], 'voltage')
                     yield voltage_metrics
@@ -33,14 +33,17 @@
                 if 'temperature' in record:
                     temperature_metrics = BaseCollector.gauge_collector('system_routerboard_temperature', 'Routerboard current temperature', [record, ], 'temperature')
                     yield temperature_metrics
 
                 if 'cpu_temperature' in record:
                     cpu_temperature_metrics = BaseCollector.gauge_collector('system_cpu_temperature', 'CPU current temperature', [record, ], 'cpu_temperature')
                     yield cpu_temperature_metrics
+                elif 'switch_temperature' in record:
+                    cpu_temperature_metrics = BaseCollector.gauge_collector('system_cpu_temperature', 'CPU current temperature', [record, ], 'switch_temperature')
+                    yield cpu_temperature_metrics
 
                 if 'fan1_speed' in record:
                     fan_one_speed_metrics = BaseCollector.gauge_collector('system_fan_one_speed', 'System fan 1 current speed', [record, ], 'fan1_speed')
                     yield fan_one_speed_metrics
 
                 if 'fan2_speed' in record:
                     fan_two_speed_metrics = BaseCollector.gauge_collector('system_fan_two_speed', 'System fan 2 current speed', [record, ], 'fan2_speed')
```

### Comparing `mktxp-1.2/mktxp/collector/identity_collector.py` & `mktxp-1.2.1/mktxp/collector/identity_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/interface_collector.py` & `mktxp-1.2.1/mktxp/collector/interface_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/ipv6_neighbor_collector.py` & `mktxp-1.2.1/mktxp/collector/ipv6_neighbor_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/mktxp_collector.py` & `mktxp-1.2.1/mktxp/collector/mktxp_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/monitor_collector.py` & `mktxp-1.2.1/mktxp/collector/monitor_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/netwatch_collector.py` & `mktxp-1.2.1/mktxp/collector/netwatch_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/package_collector.py` & `mktxp-1.2.1/mktxp/collector/package_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/poe_collector.py` & `mktxp-1.2.1/mktxp/collector/poe_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/pool_collector.py` & `mktxp-1.2.1/mktxp/collector/pool_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/public_ip_collector.py` & `mktxp-1.2.1/mktxp/collector/public_ip_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/queue_collector.py` & `mktxp-1.2.1/mktxp/collector/queue_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/resource_collector.py` & `mktxp-1.2.1/mktxp/collector/resource_collector.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
 
 from mktxp.collector.base_collector import BaseCollector
 from mktxp.flow.processor.output import BaseOutputProcessor
 from mktxp.datasource.system_resource_ds import SystemResourceMetricsDataSource
+from mktxp.utils.utils import check_for_updates
 
 
 class SystemResourceCollector(BaseCollector):
     ''' System Resource Metrics collector
     '''        
     @staticmethod
     def collect(router_entry):
@@ -57,14 +58,24 @@
 
             cpu_count_metrics = BaseCollector.gauge_collector('system_cpu_count', 'Number of CPUs present on the system', resource_records, 'cpu_count', ['version', 'board_name', 'cpu', 'architecture_name'])
             yield cpu_count_metrics
 
             cpu_frequency_metrics = BaseCollector.gauge_collector('system_cpu_frequency', 'Current CPU frequency', resource_records, 'cpu_frequency', ['version', 'board_name', 'cpu', 'architecture_name'])
             yield cpu_frequency_metrics
 
+            # Check for updates
+            if router_entry.config_entry.check_for_updates:
+                for record in resource_records:
+                    cur_version, newest_version = check_for_updates(record['version'])
+                    record['newest_version'] = str(newest_version)
+                    record['update_available'] = cur_version < newest_version
+
+                update_available_metrics = BaseCollector.gauge_collector('system_update_available', 'Is there a newer version available', resource_records, 'update_available', ['newest_version',])
+                yield update_available_metrics
+
 
     # Helpers
     @staticmethod
     def _translated_values(translated_field, value):
         return {
                 'uptime': lambda value: BaseOutputProcessor.parse_timedelta_seconds(value)
                 }[translated_field](value)
```

### Comparing `mktxp-1.2/mktxp/collector/route_collector.py` & `mktxp-1.2.1/mktxp/collector/route_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/user_collector.py` & `mktxp-1.2.1/mktxp/collector/user_collector.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/collector/wlan_collector.py` & `mktxp-1.2.1/mktxp/collector/wlan_collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,27 +50,27 @@
         if router_entry.config_entry.wireless_clients:
             registration_labels = ['interface', 'ssid', 'mac_address', 'tx_rate', 'rx_rate', 'uptime', 'bytes', 'signal_to_noise', 'tx_ccq', 'signal_strength', 'signal']
             registration_records = WirelessMetricsDataSource.metric_records(router_entry, metric_labels = registration_labels)
             if registration_records:
                 for registration_record in registration_records:
                     BaseOutputProcessor.augment_record(router_entry, registration_record)
 
-                tx_byte_metrics = BaseCollector.counter_collector('wlan_clients_tx_bytes', 'Number of sent packet bytes', registration_records, 'tx_bytes', ['dhcp_name'])
+                tx_byte_metrics = BaseCollector.counter_collector('wlan_clients_tx_bytes', 'Number of sent packet bytes', registration_records, 'tx_bytes', ['dhcp_name', 'mac_address'])
                 yield tx_byte_metrics
 
-                rx_byte_metrics = BaseCollector.counter_collector('wlan_clients_rx_bytes', 'Number of received packet bytes', registration_records, 'rx_bytes', ['dhcp_name'])
+                rx_byte_metrics = BaseCollector.counter_collector('wlan_clients_rx_bytes', 'Number of received packet bytes', registration_records, 'rx_bytes', ['dhcp_name', 'mac_address'])
                 yield rx_byte_metrics
 
-                signal_strength_metrics = BaseCollector.gauge_collector('wlan_clients_signal_strength', 'Average strength of the client signal recevied by AP', registration_records, 'signal_strength', ['dhcp_name'])
+                signal_strength_metrics = BaseCollector.gauge_collector('wlan_clients_signal_strength', 'Average strength of the client signal recevied by AP', registration_records, 'signal_strength', ['dhcp_name', 'mac_address'])
                 yield signal_strength_metrics
 
-                signal_to_noise_metrics = BaseCollector.gauge_collector('wlan_clients_signal_to_noise', 'Client devices signal to noise ratio', registration_records, 'signal_to_noise', ['dhcp_name'])
+                signal_to_noise_metrics = BaseCollector.gauge_collector('wlan_clients_signal_to_noise', 'Client devices signal to noise ratio', registration_records, 'signal_to_noise', ['dhcp_name', 'mac_address'])
                 yield signal_to_noise_metrics
 
-                tx_ccq_metrics = BaseCollector.gauge_collector('wlan_clients_tx_ccq', 'Client Connection Quality (CCQ) for transmit', registration_records, 'tx_ccq', ['dhcp_name'])
+                tx_ccq_metrics = BaseCollector.gauge_collector('wlan_clients_tx_ccq', 'Client Connection Quality (CCQ) for transmit', registration_records, 'tx_ccq', ['dhcp_name', 'mac_address'])
                 yield tx_ccq_metrics
 
                 registration_metrics = BaseCollector.info_collector('wlan_clients_devices', 'Client devices info', 
                                         registration_records, ['dhcp_name', 'dhcp_address', 'rx_signal', 'ssid', 'tx_rate', 'rx_rate', 'interface', 'mac_address', 'uptime'])
                 yield registration_metrics
```

### Comparing `mktxp-1.2/mktxp/datasource/base_ds.py` & `mktxp-1.2.1/mktxp/datasource/base_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/capsman_ds.py` & `mktxp-1.2.1/mktxp/datasource/capsman_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/connection_ds.py` & `mktxp-1.2.1/mktxp/datasource/connection_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/dhcp_ds.py` & `mktxp-1.2.1/mktxp/datasource/dhcp_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/firewall_ds.py` & `mktxp-1.2.1/mktxp/datasource/firewall_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/health_ds.py` & `mktxp-1.2.1/mktxp/datasource/health_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/identity_ds.py` & `mktxp-1.2.1/mktxp/datasource/identity_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/interface_ds.py` & `mktxp-1.2.1/mktxp/datasource/interface_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/ipv6_neighbor_ds.py` & `mktxp-1.2.1/mktxp/datasource/ipv6_neighbor_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/mktxp_ds.py` & `mktxp-1.2.1/mktxp/datasource/mktxp_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/netwatch_ds.py` & `mktxp-1.2.1/mktxp/datasource/netwatch_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/package_ds.py` & `mktxp-1.2.1/mktxp/datasource/package_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/poe_ds.py` & `mktxp-1.2.1/mktxp/datasource/poe_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/pool_ds.py` & `mktxp-1.2.1/mktxp/datasource/pool_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/public_ip_ds.py` & `mktxp-1.2.1/mktxp/datasource/public_ip_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/queue_ds.py` & `mktxp-1.2.1/mktxp/datasource/queue_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/route_ds.py` & `mktxp-1.2.1/mktxp/datasource/route_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/routerboard_ds.py` & `mktxp-1.2.1/mktxp/datasource/routerboard_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/system_resource_ds.py` & `mktxp-1.2.1/mktxp/datasource/system_resource_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/user_ds.py` & `mktxp-1.2.1/mktxp/datasource/user_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/datasource/wireless_ds.py` & `mktxp-1.2.1/mktxp/datasource/wireless_ds.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/flow/collector_handler.py` & `mktxp-1.2.1/mktxp/flow/collector_handler.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/flow/collector_registry.py` & `mktxp-1.2.1/mktxp/flow/collector_registry.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/flow/processor/base_proc.py` & `mktxp-1.2.1/mktxp/flow/processor/base_proc.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/flow/processor/output.py` & `mktxp-1.2.1/mktxp/flow/processor/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,18 @@
             wifi_rates_rgx = re.compile(r'(\d*(?:\.\d*)?)([GgMmKk]bps?)')
             config_handler.re_compiled['wifi_rates_rgx'] = wifi_rates_rgx
         rc = wifi_rates_rgx.search(rate)
         return f'{int(float(rc[1]))} {rc[2]}' if rc and len(rc.groups()) == 2 else rate
 
     @staticmethod
     def parse_bitrates(rate):
-        rate = int(rate)
+        try:
+            rate = int(rate)
+        except:
+            return BaseOutputProcessor.parse_rates(rate)
         power = floor(log(rate, 1000))
         return f"{int(rate / 1000 ** power)} {['bps', 'Kbps', 'Mbps', 'Gbps'][int(power)]}"
 
     @staticmethod
     def parse_timedelta(time):
         duration_interval_rgx = config_handler.re_compiled.get('duration_interval_rgx')
         if not duration_interval_rgx:
```

### Comparing `mktxp-1.2/mktxp/flow/router_connection.py` & `mktxp-1.2.1/mktxp/flow/router_connection.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/flow/router_entries_handler.py` & `mktxp-1.2.1/mktxp/flow/router_entries_handler.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/flow/router_entry.py` & `mktxp-1.2.1/mktxp/flow/router_entry.py`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/mktxp/utils/utils.py` & `mktxp-1.2.1/mktxp/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,22 +7,26 @@
 ## of the License, or (at your option) any later version.
 ##
 ## This program is distributed in the hope that it will be useful,
 ## but WITHOUT ANY WARRANTY; without even the implied warranty of
 ## MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 ## GNU General Public License for more details.
 
-
+from functools import lru_cache
 import os, sys, shlex, tempfile, shutil, re
-import subprocess, hashlib
+import subprocess, hashlib, urllib
+import time
 from timeit import default_timer
 from collections.abc import Iterable
+import xml.etree.ElementTree as ET
 from contextlib import contextmanager
 from multiprocessing import Process, Event
 from datetime import timedelta
+from pkg_resources import packaging
+
 
 
 ''' Utilities / Helpers
 '''
 @contextmanager
 def temp_dir(quiet = True):
     ''' Temp dir context manager
@@ -266,7 +270,80 @@
         self.start = default_timer()
         return self
 
     def __exit__(self, *args):
         self.time = default_timer() - self.start
 
 
+# mapping of channels to RSS feeds
+CHANNEL_RSS_FEED_MAPPING = {
+    'development': 'https://mikrotik.com/development.rss',
+    'long-term': 'https://mikrotik.com/bugfix.rss',
+    'stable': 'https://mikrotik.com/current.rss',
+    'testing': 'https://mikrotik.com/candidate.rss',
+}
+
+
+def get_ttl_hash(seconds=3600):
+    """Return the same value withing `seconds` time period"""
+    return round(time.time() / seconds)
+
+
+@lru_cache(maxsize=5)
+def get_available_updates(channel, ttl_hash=get_ttl_hash()):
+    """Check the RSS feed for available updates for a given update channel.
+    This method fetches the RSS feed and returns all version from the parsed XML.
+    Version numbers are parsed into version.Version instances (part of setuptools)."""
+    del ttl_hash
+    rss_feed = CHANNEL_RSS_FEED_MAPPING[channel]
+
+    print(f'Fetching available ROS releases from {rss_feed}')
+    versions = []
+    with urllib.request.urlopen(rss_feed) as response:
+        result = response.read()
+        root = ET.fromstring(result)
+        channel = root[0]
+
+        for child in channel:
+            # iterate over all updates
+            if child.tag == 'item':
+                title, _, _, _, _, _ = child
+                # extract and parse the version number from title
+                version_text = re.findall(r'[\d+\.]+', title.text)[0]
+                version_number = packaging.version.parse(version_text)
+                versions.append(version_number)
+    return versions
+
+
+def parse_ros_version(string):
+    """Parse the version returned from the /system/resource command.
+    Returns a tuple: (<version>, <channel>).
+
+    >>> parse_ros_version('1.2.3 (stable)')
+    1.2.3, stable
+    """
+    version, channel = re.findall(r'([\d\.]+).*?([\w]+)', string)[0]
+    return packaging.version.parse(version), channel
+
+def check_for_updates(cur_version):
+    """Try to check if there is a newer version available.
+    If anything goes wrong, it returns the same version.
+    Returns a tuple: (<current version>, <newest version>)"""
+    error = False
+    try:
+        cur_version, channel = parse_ros_version(cur_version)
+        available_versions = get_available_updates(channel)
+        newest_version = sorted(available_versions)[-1]
+    except KeyError:
+        print(f'unknown update channel {channel}')
+        error = True
+    except urllib.error.HTTPError as err:
+        print(f'update feed returned: {str(err)}')
+        error = True
+    except Exception as err:
+        print(f'could not check for updates, because: {str(err)}')
+        error = True
+
+    if error:
+        return cur_version, cur_version
+
+    return cur_version, newest_version
```

### Comparing `mktxp-1.2/mktxp.egg-info/PKG-INFO` & `mktxp-1.2.1/mktxp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mktxp
-Version: 1.2
+Version: 1.2.1
 Summary: Prometheus Exporter for Mikrotik RouterOS devices
 Home-page: https://github.com/akpw/mktxp
 Author: Arseniy Kuznetsov
 Author-email: k.arseniy@gmail.com
 License: GNU General Public License v2 (GPLv2)
 Keywords: Mikrotik RouterOS Prometheus Exporter
 Classifier: Development Status :: 4 - Beta
@@ -114,15 +114,17 @@
     capsman_clients = True          # CAPsMAN clients metrics    
 
     user = True                     # Active Users metrics
     queue = True                    # Queues metrics
     
     remote_dhcp_entry = None        # An MKTXP entry for remote DHCP info resolution (capsman/wireless)
 
-    use_comments_over_names = True  # when available, forces using comments over the interfaces names 
+    use_comments_over_names = True  # when available, forces using comments over the interfaces names
+
+    check_for_updates = False       # check for available ROS updates
 ```
 
 Most options are easy to understand at first glance, and some are described in more details [later](https://github.com/akpw/mktxp#advanced-features).
 
 
 #### Local install
 If you have a local MKTXP installation, you can edit the configuration file with your default system editor directly from mktxp:
@@ -236,16 +238,16 @@
     port = 49090                    
     socket_timeout = 2
     
     initial_delay_on_failure = 120
     max_delay_on_failure = 900
     delay_inc_div = 5
 
-    bandwidth = True                # Turns metrics bandwidth metrics collection on / off    
-    bandwidth_test_interval = 420   # Interval for colllecting bandwidth metrics
+    bandwidth = False               # Turns metrics bandwidth metrics collection on / off    
+    bandwidth_test_interval = 600   # Interval for colllecting bandwidth metrics
     minimal_collect_interval = 5    # Minimal metric collection interval
 
     verbose_mode = False            # Set it on for troubleshooting
 
     fetch_routers_in_parallel = False   # Set to True if you want to fetch multiple routers parallel
     max_worker_threads = 5              # Max number of worker threads that can fetch routers (parallel fetch only)
     max_scrape_duration = 10            # Max duration of individual routers' metrics collection (parallel fetch only)
```

### Comparing `mktxp-1.2/mktxp.egg-info/SOURCES.txt` & `mktxp-1.2.1/mktxp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mktxp-1.2/setup.py` & `mktxp-1.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # read the README.md contents
 pkg_dir = path.abspath(path.dirname(__file__))
 with open(path.join(pkg_dir, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='mktxp',
-    version='1.2',
+    version='1.2.1',
 
     url='https://github.com/akpw/mktxp',
 
     author='Arseniy Kuznetsov',
     author_email='k.arseniy@gmail.com',
 
     long_description=long_description,
```

