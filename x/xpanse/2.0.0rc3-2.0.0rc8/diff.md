# Comparing `tmp/xpanse-2.0.0rc3.tar.gz` & `tmp/xpanse-2.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpanse-2.0.0rc3.tar", last modified: Tue May 30 19:38:20 2023, max compression
+gzip compressed data, was "xpanse-2.0.0rc8.tar", last modified: Wed Jul  5 14:44:34 2023, max compression
```

## Comparing `xpanse-2.0.0rc3.tar` & `xpanse-2.0.0rc8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/docs/_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/docs/_source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/_static/xpanse_banner.png
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/cover.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.asset_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.attack_surface_rules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.incident_management.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.api.tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/_source/xpanse.rst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/docs/requirements-docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.408517 xpanse-2.0.0rc3/examples/asset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/asset_management/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/asset_management/get_services_by_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/asset_management/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/examples/incident_management/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/incident_management/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/incident_management/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/incident_management/update_incidents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/examples/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/tags/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/tags/assign_and_remove_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/examples/tags/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/asset_management/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/assets_management_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/owned_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/asset_management/v1/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/incident_management/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/incident_management/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v1/incidents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/incident_management/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/incident_management/v2/alerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/tags/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse/api/tags/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/tags/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/api/tags/v1/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-30 19:37:39.000000 xpanse-2.0.0rc3/xpanse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:38:20.412516 xpanse-2.0.0rc3/xpanse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 19:38:20.000000 xpanse-2.0.0rc3/xpanse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/docs/_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/docs/_source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/_static/xpanse_banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/cover.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.asset_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.attack_surface_rules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.incident_management.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.api.tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/_source/xpanse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/docs/requirements-docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.261893 xpanse-2.0.0rc8/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/examples/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/asset_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/asset_management/get_services_by_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/asset_management/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/examples/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/incident_management/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/incident_management/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/incident_management/update_incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/examples/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/tags/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/tags/assign_and_remove_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/examples/tags/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.265893 xpanse-2.0.0rc8/xpanse/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/asset_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/assets_management_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/owned_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/asset_management/v1/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/incident_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/incident_management/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7612 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v1/incidents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/incident_management/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/incident_management/v2/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/tags/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse/api/tags/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/tags/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/api/tags/v1/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-05 14:44:02.000000 xpanse-2.0.0rc8/xpanse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 14:44:34.269893 xpanse-2.0.0rc8/xpanse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-05 14:44:34.000000 xpanse-2.0.0rc8/xpanse.egg-info/top_level.txt
```

### Comparing `xpanse-2.0.0rc3/LICENSE` & `xpanse-2.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/PKG-INFO` & `xpanse-2.0.0rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanse
-Version: 2.0.0rc3
+Version: 2.0.0rc8
 Summary: Python library is an interface to the Cortex Xpanse API.
 Home-page: UNKNOWN
 Author: Palo Alto Cortex Xpanse
 Author-email: xpanse-integrations@paloaltonetworks.com
 License: ISC
 Keywords: xpanse iom
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc3 Summary: Python library is
+Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc8 Summary: Python library is
 an interface to the Cortex Xpanse API. Home-page: UNKNOWN Author: Palo Alto
 Cortex Xpanse Author-email: xpanse-integrations@paloaltonetworks.com License:
 ISC Keywords: xpanse iom Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `xpanse-2.0.0rc3/README.md` & `xpanse-2.0.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/Makefile` & `xpanse-2.0.0rc8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/README.md` & `xpanse-2.0.0rc8/docs/README.md`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/_source/_static/xpanse_banner.png` & `xpanse-2.0.0rc8/docs/_source/_static/xpanse_banner.png`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/_source/conf.py` & `xpanse-2.0.0rc8/docs/_source/conf.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/_source/cover.rst` & `xpanse-2.0.0rc8/docs/_source/cover.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/_source/xpanse.api.asset_management.rst` & `xpanse-2.0.0rc8/docs/_source/xpanse.api.asset_management.rst`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .. automodule:: xpanse.api.asset_management.v1.assets
    :members:
    :undoc-members:
    :show-inheritance:
 
 xpanse.api.asset\_management.v1.owned\_ip\_ranges module
------------------------------------------------------------
+--------------------------------------------------------
 
 .. automodule:: xpanse.api.asset_management.v1.owned_ip_ranges
    :members:
    :undoc-members:
    :show-inheritance:
 
 xpanse.api.asset\_management.v1.services module
```

### Comparing `xpanse-2.0.0rc3/docs/_source/xpanse.api.incident_management.rst` & `xpanse-2.0.0rc8/docs/_source/xpanse.api.incident_management.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/_source/xpanse.api.rst` & `xpanse-2.0.0rc8/docs/_source/xpanse.api.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/_source/xpanse.rst` & `xpanse-2.0.0rc8/docs/_source/xpanse.rst`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/docs/requirements-docs.txt` & `xpanse-2.0.0rc8/docs/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/examples/asset_management/get_services_by_asset.py` & `xpanse-2.0.0rc8/examples/asset_management/get_services_by_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     ]
 
     # Paginate the chunk sizes
     details = []
     for chunk in id_chunks:
         detail = get_details(chunk)
         status_code = detail.response.status_code
-        if status_code >= 400:
+        if status_code >= 300:
             raise UnexpectedResponseError(f"Unexpected status code {status_code}.")
         details += detail.data
 
     return details
 
 
 if __name__ == "__main__":
```

### Comparing `xpanse-2.0.0rc3/examples/incident_management/update_incidents.py` & `xpanse-2.0.0rc8/examples/incident_management/update_incidents.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,19 +95,22 @@
     # Update data
     update_data = {
         **({STATUS: status} if status else {}),
         **({SEVERITY: severity} if severity else {}),
     }
 
     # Run bulk update
-    update_results = client.incidents.update(
-        incident_ids=incidents_to_update, update_data=update_data
-    )
-    status_code = update_results.response.status_code
-    if status_code >= 400:
-        raise UnexpectedResponseError(f"Unexpected status code {status_code}.")
+    for incident_id in incidents_to_update:
+        update_results = client.incidents.update(
+            incident_id=incident_id, update_data=update_data
+        )
+        status_code = update_results.response.status_code
+        if status_code >= 300:
+            raise UnexpectedResponseError(f"Unexpected status code {status_code}.")
 
-    print(f"Update {'succeeded' if update_results.data else 'failed'}.")
+        print(
+            f"Update for incident_id={incident_id} {'succeeded' if update_results.data else 'failed'}."
+        )
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `xpanse-2.0.0rc3/examples/tags/assign_and_remove_tags.py` & `xpanse-2.0.0rc8/examples/tags/assign_and_remove_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,25 +71,25 @@
     ]
 
     # Assign Tags
     assign_tags = client.tags.assign(
         data_type=TaggableDataType[data_type], tags=tags, filters=filters
     )
     status_code = assign_tags.response.status_code
-    if status_code >= 400:
+    if status_code >= 300:
         raise UnexpectedResponseError(f"Unexpected status code {status_code}.")
 
     print(f"Assigned tags: {assign_tags.data}")
 
     # Remove Tags
     remove_tags = client.tags.remove(
         data_type=TaggableDataType[data_type], tags=tags, filters=filters
     )
     status_code = remove_tags.response.status_code
-    if status_code >= 400:
+    if status_code >= 300:
         raise UnexpectedResponseError(f"Unexpected status code {status_code}.")
 
     print(f"Remove tags: {remove_tags.data}")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `xpanse-2.0.0rc3/setup.py` & `xpanse-2.0.0rc8/setup.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/api/asset_management/__init__.py` & `xpanse-2.0.0rc8/xpanse/api/asset_management/__init__.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/api/asset_management/assets_management_base.py` & `xpanse-2.0.0rc8/xpanse/api/asset_management/assets_management_base.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/api/asset_management/v1/assets.py` & `xpanse-2.0.0rc8/xpanse/api/asset_management/v1/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     LIST_ENDPOINT = (
         f"{AssetsManagementBaseEndpoint.ENDPOINT}/get_assets_internet_exposure/"
     )
     GET_ENDPOINT = (
         f"{AssetsManagementBaseEndpoint.ENDPOINT}/get_asset_internet_exposure/"
     )
 
+    LIST_DATA_KEY = "assets_internet_exposure"
+
     def list(
         self,
         asset_types: Optional[Set[AssetType]] = None,
         request_data: Optional[RequestData] = None,
         **kwargs: Any,
     ) -> XpanseResultIterator:
         """
```

### Comparing `xpanse-2.0.0rc3/xpanse/api/asset_management/v1/owned_ip_ranges.py` & `xpanse-2.0.0rc8/xpanse/api/asset_management/v1/owned_ip_ranges.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 class OwnedIpRangesEndpoint(AssetsManagementBaseEndpoint):
     """
     Part of the Public API for handling Owned IP Ranges.
     See: https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-All-External-IP-Address-Ranges
     See: https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-External-IP-Address-Range
     """
 
+    LIST_DATA_KEY = "external_ip_address_ranges"
+
     LIST_ENDPOINT = (
         f"{AssetsManagementBaseEndpoint.ENDPOINT}/get_external_ip_address_ranges/"
     )
     GET_ENDPOINT = (
         f"{AssetsManagementBaseEndpoint.ENDPOINT}/get_external_ip_address_range/"
     )
```

### Comparing `xpanse-2.0.0rc3/xpanse/api/asset_management/v1/services.py` & `xpanse-2.0.0rc8/xpanse/api/asset_management/v1/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     See: https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-All-External-Services
     See: https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-External-Service
     """
 
     LIST_ENDPOINT = f"{AssetsManagementBaseEndpoint.ENDPOINT}/get_external_services/"
     GET_ENDPOINT = f"{AssetsManagementBaseEndpoint.ENDPOINT}/get_external_service/"
 
+    LIST_DATA_KEY = "external_services"
+
     def list(
         self, request_data: Optional[RequestData] = None, **kwargs: Any
     ) -> XpanseResultIterator:
         """
         This endpoint will return a paginated list of Services.
 
         Args:
```

### Comparing `xpanse-2.0.0rc3/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py` & `xpanse-2.0.0rc8/xpanse/api/attack_surface_rules/v1/attack_surface_rules.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/api/incident_management/__init__.py` & `xpanse-2.0.0rc8/xpanse/api/incident_management/__init__.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/api/incident_management/v1/incidents.py` & `xpanse-2.0.0rc8/xpanse/api/incident_management/v1/incidents.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,43 +140,43 @@
             >>>     count = incidents.data
         """
         return super(IncidentsEndpoint, self)._count(
             self.LIST_ENDPOINT, request_data=request_data, **kwargs
         )
 
     def update(
-        self, incident_ids: List[str], update_data: Any, **kwargs: Any
+        self, incident_id: str, update_data: Any, **kwargs: Any
     ) -> XpanseResponse:
         """
         This endpoint will update a set of Incidents' data.
 
         Args:
-            incident_ids (List[str]):
-                The list of Incident ids to modify with your request data.
+            incident_id (str):
+                The Incident id to modify with your request data.
             update_data (Any):
-                The data with which to update the set of Incidents.
+                The data with which to update the Incident.
             **kwargs:
                 Any extraneous parameters you would like to include when executing your
                 request with the Requests.request module. Note: By default, all payload data
                 is sent under the "json" keyword for your request.
 
         Returns:
             :obj:`XpanseResponse`:
                 An object containing the raw requests.Response and parsed data results.
                 The raw response can be accessed with `<xpanse_reponse>.response` attribute.
                 The parsed results can be accessed with the `<xpanse_response>.data` attribute.
 
         Examples:
             >>> # Update Incidents with new assignee:
-            >>> incidents =  client.incidents.update(incident_ids=["id1", "id2"],
+            >>> incidents =  client.incidents.update(incident_id="id1",
             >>>                                      update_data={"assigned_user_mail": "new@mail.com"})
             >>> if incidents.response.status_code < 300:
             >>>     results = incidents.data
 
         """
         extra_request_data = {
-            "incident_id_list": incident_ids,
+            "incident_id": incident_id,
             "update_data": update_data,
         }
         kwargs = build_request_payload(extra_request_data=extra_request_data, **kwargs)
         response = self._api.post(self.UPDATE_ENDPOINT, **kwargs)
         return XpanseResponse(response)
```

### Comparing `xpanse-2.0.0rc3/xpanse/api/incident_management/v2/alerts.py` & `xpanse-2.0.0rc8/xpanse/api/incident_management/v2/alerts.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class AlertsEndpoint(XpanseEndpoint):
     """
     Part of the Public API for handling Alerts Multi-Events v2.
     See: https://docs-cortex.paloaltonetworks.com/r/Cortex-XPANSE/Cortex-Xpanse-API-Reference/Get-Alerts-Multi-Events
     """
 
     ENDPOINT = f"{V2_PREFIX}/alerts/get_alerts_multi_events/"
-    DATA_KEY = "data"
+    DATA_KEY = "alerts"
 
     def list(
         self, request_data: Optional[RequestData] = None, **kwargs: Any
     ) -> XpanseResultIterator:
         """
         This endpoint will return a paginated list of Alerts.
```

### Comparing `xpanse-2.0.0rc3/xpanse/api/tags/v1/tags.py` & `xpanse-2.0.0rc8/xpanse/api/tags/v1/tags.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/client.py` & `xpanse-2.0.0rc8/xpanse/client.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/const.py` & `xpanse-2.0.0rc8/xpanse/const.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/endpoint.py` & `xpanse-2.0.0rc8/xpanse/endpoint.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/error.py` & `xpanse-2.0.0rc8/xpanse/error.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/iterator.py` & `xpanse-2.0.0rc8/xpanse/iterator.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/response.py` & `xpanse-2.0.0rc8/xpanse/response.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/types.py` & `xpanse-2.0.0rc8/xpanse/types.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse/utils.py` & `xpanse-2.0.0rc8/xpanse/utils.py`

 * *Files identical despite different names*

### Comparing `xpanse-2.0.0rc3/xpanse.egg-info/PKG-INFO` & `xpanse-2.0.0rc8/xpanse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpanse
-Version: 2.0.0rc3
+Version: 2.0.0rc8
 Summary: Python library is an interface to the Cortex Xpanse API.
 Home-page: UNKNOWN
 Author: Palo Alto Cortex Xpanse
 Author-email: xpanse-integrations@paloaltonetworks.com
 License: ISC
 Keywords: xpanse iom
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc3 Summary: Python library is
+Metadata-Version: 2.1 Name: xpanse Version: 2.0.0rc8 Summary: Python library is
 an interface to the Cortex Xpanse API. Home-page: UNKNOWN Author: Palo Alto
 Cortex Xpanse Author-email: xpanse-integrations@paloaltonetworks.com License:
 ISC Keywords: xpanse iom Platform: UNKNOWN Classifier: Development Status :: 5
 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development Classifier: Topic :: Software Development ::
 Libraries Classifier: Topic :: Software Development :: Libraries :: Application
 Frameworks Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `xpanse-2.0.0rc3/xpanse.egg-info/SOURCES.txt` & `xpanse-2.0.0rc8/xpanse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

