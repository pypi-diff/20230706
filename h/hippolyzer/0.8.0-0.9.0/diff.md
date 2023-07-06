# Comparing `tmp/hippolyzer-0.8.0.tar.gz` & `tmp/hippolyzer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hippolyzer-0.8.0.tar", last modified: Tue Dec  7 07:21:11 2021, max compression
+gzip compressed data, was "hippolyzer-0.9.0.tar", last modified: Sat Mar 12 18:45:42 2022, max compression
```

## Comparing `hippolyzer-0.8.0.tar` & `hippolyzer-0.9.0.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.593200 hippolyzer-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11117 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (121)    18280 2021-12-07 07:21:11.593200 hippolyzer-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17205 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.573200 hippolyzer-0.8.0/hippolyzer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.577200 hippolyzer-0.8.0/hippolyzer/apps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/addon_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/filter_dialog.ui
--rw-r--r--   0 runner    (1001) docker     (121)     6993 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/message_builder.ui
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     7565 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)    38354 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/proxy_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)    10754 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/apps/proxy_mainwindow.ui
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.577200 hippolyzer-0.8.0/hippolyzer/lib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.581200 hippolyzer-0.8.0/hippolyzer/lib/base/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/anim_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.581200 hippolyzer-0.8.0/hippolyzer/lib/base/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/data/LICENSE-artwork.txt
--rw-r--r--   0 runner    (1001) docker     (121)   353273 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/data/avatar_lad.xml
--rw-r--r--   0 runner    (1001) docker     (121)    39717 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/data/avatar_skeleton.xml
--rw-r--r--   0 runner    (1001) docker     (121)   576578 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/data/static_data.db2
--rw-r--r--   0 runner    (1001) docker     (121)     9894 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/data/static_index.db2
--rw-r--r--   0 runner    (1001) docker     (121)     9901 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2654 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     9868 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/exc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4630 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10878 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/jp2_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6344 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/legacy_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     4806 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/llanim.py
--rw-r--r--   0 runner    (1001) docker     (121)     3187 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/llsd.py
--rw-r--r--   0 runner    (1001) docker     (121)    15442 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.585200 hippolyzer-0.8.0/hippolyzer/lib/base/message/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3205 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/circuit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.585200 hippolyzer-0.8.0/hippolyzer/lib/base/message/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16340 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/data/message.xml
--rw-r--r--   0 runner    (1001) docker     (121)   183971 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/data/message_template.msg
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/data_packer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/llsd_msg_serializer.py
--rw-r--r--   0 runner    (1001) docker     (121)    14839 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1945 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/message_dot_xml.py
--rw-r--r--   0 runner    (1001) docker     (121)     8969 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/message_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     5790 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3849 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/msgtypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/template.py
--rw-r--r--   0 runner    (1001) docker     (121)     4344 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/template_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     9373 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/template_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    11039 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/udpdeserializer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7754 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/message/udpserializer.py
--rw-r--r--   0 runner    (1001) docker     (121)    25024 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/multidict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/namevalue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.585200 hippolyzer-0.8.0/hippolyzer/lib/base/network/
--rw-r--r--   0 runner    (1001) docker     (121)      841 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7133 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/network/caps_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.585200 hippolyzer-0.8.0/hippolyzer/lib/base/network/data/
--rw-r--r--   0 runner    (1001) docker     (121)   810037 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/network/data/ca-bundle.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1640 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/network/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)    17802 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)    61663 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    54731 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5766 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/transfer_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4481 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/ui_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/vfs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5175 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/wearables.py
--rw-r--r--   0 runner    (1001) docker     (121)    11340 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/base/xfer_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.589200 hippolyzer-0.8.0/hippolyzer/lib/client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/client/namecache.py
--rw-r--r--   0 runner    (1001) docker     (121)    37946 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/client/object_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1331 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/client/state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.593200 hippolyzer-0.8.0/hippolyzer/lib/proxy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      881 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/addon_ctx.py
--rw-r--r--   0 runner    (1001) docker     (121)    10771 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22513 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/addons.py
--rw-r--r--   0 runner    (1001) docker     (121)      953 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/ca_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2958 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/caps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/caps_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     8365 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/circuit.py
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/http_asset_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)    17036 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/http_event_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/http_flow.py
--rw-r--r--   0 runner    (1001) docker     (121)    11263 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/http_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6670 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/lludp_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/message_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)    26928 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/message_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/namecache.py
--rw-r--r--   0 runner    (1001) docker     (121)     7595 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/object_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7729 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/region.py
--rw-r--r--   0 runner    (1001) docker     (121)     9515 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/sessions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     7669 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/socks_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3158 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/task_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)    38051 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/templates.py
--rw-r--r--   0 runner    (1001) docker     (121)     3287 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/viewer_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     8684 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/vocache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1896 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/hippolyzer/lib/proxy/webapp_cap_addon.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-07 07:21:11.577200 hippolyzer-0.8.0/hippolyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18280 2021-12-07 07:21:11.000000 hippolyzer-0.8.0/hippolyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2021-12-07 07:21:11.000000 hippolyzer-0.8.0/hippolyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 07:21:11.000000 hippolyzer-0.8.0/hippolyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-07 07:21:11.000000 hippolyzer-0.8.0/hippolyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-07 07:21:11.000000 hippolyzer-0.8.0/hippolyzer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-12-07 07:21:11.000000 hippolyzer-0.8.0/hippolyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-07 07:21:11.000000 hippolyzer-0.8.0/hippolyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-12-07 07:21:11.593200 hippolyzer-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2021-12-07 07:20:27.000000 hippolyzer-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.647532 hippolyzer-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11117 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (121)    18280 2022-03-12 18:45:42.647532 hippolyzer-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17205 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.631531 hippolyzer-0.9.0/hippolyzer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.635531 hippolyzer-0.9.0/hippolyzer/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/addon_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/filter_dialog.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     6993 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/message_builder.ui
+-rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7565 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38410 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/proxy_gui.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10754 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/apps/proxy_mainwindow.ui
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.635531 hippolyzer-0.9.0/hippolyzer/lib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.635531 hippolyzer-0.9.0/hippolyzer/lib/base/
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/anim_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.639531 hippolyzer-0.9.0/hippolyzer/lib/base/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/data/LICENSE-artwork.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   353273 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/data/avatar_lad.xml
+-rw-r--r--   0 runner    (1001) docker     (121)    39717 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/data/avatar_skeleton.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   576578 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/data/static_data.db2
+-rw-r--r--   0 runner    (1001) docker     (121)     9894 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/data/static_index.db2
+-rw-r--r--   0 runner    (1001) docker     (121)    10154 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2654 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9868 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/exc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10878 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/jp2_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6344 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/legacy_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/llanim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3187 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/llsd.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15442 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.639531 hippolyzer-0.9.0/hippolyzer/lib/base/message/
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5751 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/circuit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.639531 hippolyzer-0.9.0/hippolyzer/lib/base/message/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16340 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/data/message.xml
+-rw-r--r--   0 runner    (1001) docker     (121)   183971 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/data/message_template.msg
+-rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/data_packer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/llsd_msg_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14893 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1945 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/message_dot_xml.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9652 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/message_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5790 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3849 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/msgtypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5077 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/template.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4344 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/template_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9373 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/template_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11080 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/udpdeserializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7754 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/message/udpserializer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25024 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/multidict.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/namevalue.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.643531 hippolyzer-0.9.0/hippolyzer/lib/base/network/
+-rw-r--r--   0 runner    (1001) docker     (121)      841 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7133 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/network/caps_client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.643531 hippolyzer-0.9.0/hippolyzer/lib/base/network/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   810037 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/network/data/ca-bundle.crt
+-rw-r--r--   0 runner    (1001) docker     (121)     1640 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/network/transport.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17802 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61663 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54859 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/transfer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4481 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/ui_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/vfs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5175 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/wearables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11308 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/base/xfer_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.643531 hippolyzer-0.9.0/hippolyzer/lib/client/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/client/namecache.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37922 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/client/object_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1331 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/client/state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.647532 hippolyzer-0.9.0/hippolyzer/lib/proxy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      881 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/addon_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10747 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22513 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/addons.py
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/ca_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2958 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/caps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/caps_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8606 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/http_asset_repo.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17045 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/http_event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/http_flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11283 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/http_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7255 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/lludp_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6868 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/message_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29192 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/message_logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/namecache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7606 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/object_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7871 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/region.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9515 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7669 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/socks_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3158 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/task_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38051 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/templates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3350 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/transport.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/viewer_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8684 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/vocache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1896 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/hippolyzer/lib/proxy/webapp_cap_addon.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-12 18:45:42.631531 hippolyzer-0.9.0/hippolyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    18280 2022-03-12 18:45:42.000000 hippolyzer-0.9.0/hippolyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-03-12 18:45:42.000000 hippolyzer-0.9.0/hippolyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-12 18:45:42.000000 hippolyzer-0.9.0/hippolyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-03-12 18:45:42.000000 hippolyzer-0.9.0/hippolyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-12 18:45:42.000000 hippolyzer-0.9.0/hippolyzer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-03-12 18:45:42.000000 hippolyzer-0.9.0/hippolyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-12 18:45:42.000000 hippolyzer-0.9.0/hippolyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-03-12 18:45:42.647532 hippolyzer-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-03-12 18:44:43.000000 hippolyzer-0.9.0/setup.py
```

### Comparing `hippolyzer-0.8.0/LICENSE.txt` & `hippolyzer-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/NOTICE.md` & `hippolyzer-0.9.0/NOTICE.md`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/PKG-INFO` & `hippolyzer-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hippolyzer
-Version: 0.8.0
+Version: 0.9.0
 Summary: Analysis tools for SL-compatible virtual worlds
 Home-page: https://github.com/SaladDais/Hippolyzer/
 Author: Salad Dais
 Author-email: 83434023+SaladDais@users.noreply.github.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `hippolyzer-0.8.0/README.md` & `hippolyzer-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/apps/addon_dialog.ui` & `hippolyzer-0.9.0/hippolyzer/apps/addon_dialog.ui`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/apps/filter_dialog.ui` & `hippolyzer-0.9.0/hippolyzer/apps/filter_dialog.ui`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/apps/message_builder.ui` & `hippolyzer-0.9.0/hippolyzer/apps/message_builder.ui`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/apps/model.py` & `hippolyzer-0.9.0/hippolyzer/apps/model.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/apps/proxy.py` & `hippolyzer-0.9.0/hippolyzer/apps/proxy.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/apps/proxy_gui.py` & `hippolyzer-0.9.0/hippolyzer/apps/proxy_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 FILTER_DIALOG_UI_PATH = get_resource_filename("apps/filter_dialog.ui")
 
 
 def show_error_message(error_msg, parent=None):
     error_dialog = QtWidgets.QErrorMessage(parent=parent)
     # No obvious way to set this to plaintext, yuck...
     error_dialog.showMessage(html.escape(error_msg))
-    error_dialog.exec_()
+    error_dialog.exec()
     error_dialog.raise_()
 
 
 class GUISessionManager(SessionManager, QtCore.QObject):
     regionAdded = QtCore.Signal(ProxiedRegion)
     regionRemoved = QtCore.Signal(ProxiedRegion)
 
@@ -85,33 +85,33 @@
         for old_region in self.all_regions:
             if old_region not in new_regions:
                 self.regionRemoved.emit(old_region)  # type: ignore
 
         self.all_regions = new_regions
 
 
-class GUIInteractionManager(BaseInteractionManager, QtCore.QObject):
-    def __init__(self, parent):
+class GUIInteractionManager(BaseInteractionManager):
+    def __init__(self, parent: QtWidgets.QWidget):
         BaseInteractionManager.__init__(self)
-        QtCore.QObject.__init__(self, parent=parent)
+        self._parent = parent
 
     def main_window_handle(self) -> Any:
-        return self.parent()
+        return self._parent
 
     def _dialog_async_exec(self, dialog: QtWidgets.QDialog):
         future = asyncio.Future()
         dialog.finished.connect(lambda r: future.set_result(r))
         dialog.open()
         return future
 
     async def _file_dialog(
             self, caption: str, directory: str, filter_str: str, mode: QtWidgets.QFileDialog.FileMode,
             default_suffix: str = '',
     ) -> Tuple[bool, QtWidgets.QFileDialog]:
-        dialog = QtWidgets.QFileDialog(self.parent(), caption=caption, directory=directory, filter=filter_str)
+        dialog = QtWidgets.QFileDialog(self._parent, caption=caption, directory=directory, filter=filter_str)
         dialog.setFileMode(mode)
         if mode == QtWidgets.QFileDialog.FileMode.AnyFile:
             dialog.setAcceptMode(QtWidgets.QFileDialog.AcceptMode.AcceptSave)
         if default_suffix:
             dialog.setDefaultSuffix(default_suffix)
         res = await self._dialog_async_exec(dialog)
         return res, dialog
@@ -151,15 +151,15 @@
 
     async def confirm(self, title: str, caption: str) -> bool:
         msg = QtWidgets.QMessageBox(
             QtWidgets.QMessageBox.Icon.Question,
             title,
             caption,
             QtWidgets.QMessageBox.Ok | QtWidgets.QMessageBox.Cancel,
-            self.parent(),
+            self._parent,
         )
         fut = asyncio.Future()
         msg.finished.connect(lambda r: fut.set_result(r))
         msg.open()
         return (await fut) == QtWidgets.QMessageBox.Ok
 
 
@@ -319,15 +319,15 @@
 
     def setFilterDict(self, val: dict):
         self.settings.FILTERS = val
         self._populateFilterMenu()
 
     def _manageFilters(self):
         dialog = FilterDialog(self)
-        dialog.exec_()
+        dialog.exec()
 
     @nonFatalExceptions
     def setFilter(self, filter_str=None):
         if filter_str is None:
             filter_str = self.lineEditFilter.text()
         else:
             self.lineEditFilter.setText(filter_str)
@@ -356,29 +356,28 @@
         entry = self._selectedEntry
         if not entry:
             return
         req = entry.request(
             beautify=self.checkBeautify.isChecked(),
             replacements=buildReplacements(entry.session, entry.region),
         )
-        highlight_range = None
-        if isinstance(req, SpannedString):
-            match_result = self.model.filter.match(entry)
-            # Match result was a tuple indicating what matched
-            if isinstance(match_result, tuple):
-                highlight_range = req.spans.get(match_result)
-
         self.textRequest.setPlainText(req)
-        if highlight_range:
-            cursor = self.textRequest.textCursor()
-            cursor.setPosition(highlight_range[0], QtGui.QTextCursor.MoveAnchor)
-            cursor.setPosition(highlight_range[1], QtGui.QTextCursor.KeepAnchor)
-            highlight_format = QtGui.QTextBlockFormat()
-            highlight_format.setBackground(QtCore.Qt.yellow)
-            cursor.setBlockFormat(highlight_format)
+        # The string has a map of fields and their associated positions within the string,
+        # use that to highlight any individual fields the filter matched on.
+        if isinstance(req, SpannedString):
+            for field in self.model.filter.match(entry, short_circuit=False).fields:
+                field_span = req.spans.get(field)
+                if not field_span:
+                    continue
+                cursor = self.textRequest.textCursor()
+                cursor.setPosition(field_span[0], QtGui.QTextCursor.MoveAnchor)
+                cursor.setPosition(field_span[1], QtGui.QTextCursor.KeepAnchor)
+                highlight_format = QtGui.QTextBlockFormat()
+                highlight_format.setBackground(QtCore.Qt.yellow)
+                cursor.setBlockFormat(highlight_format)
 
         resp = entry.response(beautify=self.checkBeautify.isChecked())
         if resp:
             self.textResponse.show()
             self.textResponse.setPlainText(resp)
         else:
             self.textResponse.hide()
@@ -478,15 +477,15 @@
         self.sessionManager.settings.USE_VIEWER_OBJECT_CACHE = checked
 
     def _setRequestMissingObjects(self, checked: bool):
         self.sessionManager.settings.AUTOMATICALLY_REQUEST_MISSING_OBJECTS = checked
 
     def _manageAddons(self):
         dialog = AddonDialog(self)
-        dialog.exec_()
+        dialog.exec()
 
     def getAddonList(self) -> List[str]:
         return self.sessionManager.settings.ADDON_SCRIPTS
 
     def setAddonList(self, val: List[str]):
         self.sessionManager.settings.ADDON_SCRIPTS = val
 
@@ -708,15 +707,15 @@
                     self.llsdSerializer.serialize(msg),
                 )
         else:
             transport = None
             off_circuit = self.checkOffCircuit.isChecked()
             if off_circuit:
                 transport = SocketUDPTransport(socket.socket(socket.AF_INET, socket.SOCK_DGRAM))
-            region.circuit.send_message(msg, transport=transport)
+            region.circuit.send(msg, transport=transport)
             if off_circuit:
                 transport.close()
 
     def _sendEQMessage(self, session, region: Optional[ProxiedRegion], msg_text: str, _replacements: dict):
         if not session or not region:
             raise RuntimeError("Need a valid session and region to send EQ event")
         message_line, _, body = (x.strip() for x in msg_text.partition("\n"))
```

### Comparing `hippolyzer-0.8.0/hippolyzer/apps/proxy_mainwindow.ui` & `hippolyzer-0.9.0/hippolyzer/apps/proxy_mainwindow.ui`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/__init__.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/__init__.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/anim_utils.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/anim_utils.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/data/LICENSE-artwork.txt` & `hippolyzer-0.9.0/hippolyzer/lib/base/data/LICENSE-artwork.txt`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/data/avatar_lad.xml` & `hippolyzer-0.9.0/hippolyzer/lib/base/data/avatar_lad.xml`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/data/avatar_skeleton.xml` & `hippolyzer-0.9.0/hippolyzer/lib/base/data/avatar_skeleton.xml`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/data/static_data.db2` & `hippolyzer-0.9.0/hippolyzer/lib/base/data/static_data.db2`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/data/static_index.db2` & `hippolyzer-0.9.0/hippolyzer/lib/base/data/static_index.db2`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/datatypes.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/datatypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,29 +269,35 @@
 
 
 class JankStringyBytes(bytes):
     """
     Treat bytes as UTF8 if used in string context
 
     Sinful, but necessary evil for now since templates don't specify what's
-    binary and what's a string.
+    binary and what's a string. There are also certain fields where the value
+    may be either binary _or_ a string, depending on the context.
     """
     __slots__ = ()
 
     def __str__(self):
         return self.rstrip(b"\x00").decode("utf8", errors="replace")
 
     def __eq__(self, other):
         if isinstance(other, str):
             return str(self) == other
         return super().__eq__(other)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
+    def __contains__(self, item):
+        if isinstance(item, str):
+            return item in str(self)
+        return item in bytes(self)
+
 
 class RawBytes(bytes):
     __slots__ = ()
     pass
 
 
 _T = TypeVar("_T")
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/events.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/events.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/exc.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/exc.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/helpers.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/helpers.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/inventory.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/inventory.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/jp2_utils.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/jp2_utils.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/legacy_schema.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/legacy_schema.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/llanim.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/llanim.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/llsd.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/llsd.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/mesh.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/mesh.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/__init__.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/__init__.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/data/__init__.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/data/message.xml` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/data/message.xml`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/data/message_template.msg` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/data/message_template.msg`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/data_packer.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/data_packer.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/llsd_msg_serializer.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/llsd_msg_serializer.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/message.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         else:
             super().__setitem__(item, val)
 
 
 class Message:
     __slots__ = ("name", "send_flags", "packet_id", "acks", "body_boundaries", "queued",
                  "offset", "raw_extra", "raw_body", "deserializer", "_blocks", "finalized",
-                 "direction", "meta", "injected", "dropped", "sender")
+                 "direction", "meta", "synthetic", "dropped", "sender")
 
     def __init__(self, name, *args, packet_id=None, flags=0, acks=None, direction=None):
         # TODO: Do this on a timer or something.
         maybe_reload_templates()
 
         self.name = name
         self.send_flags = flags
@@ -209,15 +209,15 @@
         # should be set once a packet is sent / dropped to prevent accidental
         # re-sending or re-dropping
         self.finalized = False
         # Whether message is owned by the queue or should be sent immediately
         self.queued: bool = False
         self._blocks: BLOCK_DICT = {}
         self.meta = {}
-        self.injected = False
+        self.synthetic = packet_id is None
         self.dropped = False
         self.sender: Optional[ADDR_TUPLE] = None
 
         self.add_blocks(args)
 
     def add_blocks(self, block_list):
         # can have a list of blocks if it is multiple or variable
@@ -308,15 +308,15 @@
                 dict_blocks.append(new_vars)
 
         if extended:
             base_repr.update({
                 "packet_id": self.packet_id,
                 "meta": self.meta.copy(),
                 "dropped": self.dropped,
-                "injected": self.injected,
+                "synthetic": self.synthetic,
                 "direction": self.direction.name,
                 "send_flags": int(self.send_flags),
                 "extra": self.extra,
                 "acks": self.acks,
             })
 
         return base_repr
@@ -330,15 +330,15 @@
                 msg.add_block(Block(block_type, **block))
 
         if 'packet_id' in dict_val:
             # extended format
             msg.packet_id = dict_val['packet_id']
             msg.meta = dict_val['meta']
             msg.dropped = dict_val['dropped']
-            msg.injected = dict_val['injected']
+            msg.synthetic = dict_val['synthetic']
             msg.direction = Direction[dict_val['direction']]
             msg.send_flags = dict_val['send_flags']
             msg.extra = dict_val['extra']
             msg.acks = dict_val['acks']
         return msg
 
     def invalidate_caches(self):
@@ -382,14 +382,15 @@
 
         # Original was dropped so let's make sure we have clean acks and packet id
         message_copy.acks = tuple()
         message_copy.send_flags &= ~PacketFlags.ACK
         message_copy.packet_id = None
         message_copy.dropped = False
         message_copy.finalized = False
+        message_copy.queued = False
         return message_copy
 
     def to_summary(self):
         string = ""
         for block_name, block_list in self.blocks.items():
             for block in block_list:
                 for var_name, val in block.items():
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/message_dot_xml.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/message_dot_xml.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/message_formatting.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/message_formatting.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,17 +58,24 @@
         while lines:
             line = lines.pop(0)
             # Ignore comment / blank lines
             if re.match(r"^\s*(#.*)?$", line):
                 continue
 
             if first_line:
-                direction, message_name = line.split(" ", 1)
+                first_split = [x for x in line.split(" ") if x]
+                direction, message_name = first_split[:2]
+                options = [x.strip("[]") for x in first_split[2:]]
                 msg = Message(message_name)
                 msg.direction = Direction[direction.upper()]
+                for option in options:
+                    if option in PacketFlags.__members__:
+                        msg.send_flags |= PacketFlags[option]
+                    elif re.match(r"^\d+$", option):
+                        msg.send_flags |= int(option)
                 first_line = False
                 continue
 
             if line.startswith("["):
                 cur_block = Block(re.search(r"\w+", line).group(0))
                 msg.add_block(cur_block)
             else:
@@ -133,17 +140,25 @@
         replacements = replacements or {}
         maybe_reload_templates()
         spans: SpanDict = {}
         string = ""
         if msg.direction is not None:
             string += f'{msg.direction.name} '
         string += msg.name
+        flags = msg.send_flags
+        for poss_flag in iter(PacketFlags):
+            if flags & poss_flag:
+                flags &= ~poss_flag
+                string += f" [{poss_flag.name}]"
+        # Make sure flags with unknown meanings don't get lost
+        if flags:
+            string += f" [{int(flags)}]"
         if msg.packet_id is not None:
-            string += f'\n# {msg.packet_id}: {PacketFlags(msg.send_flags)!r}'
-            string += f'{", DROPPED" if msg.dropped else ""}{", INJECTED" if msg.injected else ""}'
+            string += f'\n# ID: {msg.packet_id}'
+            string += f'{", DROPPED" if msg.dropped else ""}{", SYNTHETIC" if msg.synthetic else ""}'
         if msg.extra:
             string += f'\n# EXTRA: {msg.extra!r}'
         string += '\n\n'
 
         for block_name, block_list in msg.blocks.items():
             block_suffix = ""
             if template and template.get_block(block_name).block_type == MsgBlockType.MBT_VARIABLE:
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/message_handler.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/message_handler.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/msgtypes.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/msgtypes.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/template.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/template.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/template_dict.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/template_dict.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/template_parser.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/template_parser.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/udpdeserializer.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/udpdeserializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class UDPMessageDeserializer:
     DEFAULT_TEMPLATE = DEFAULT_TEMPLATE_DICT
 
     def __init__(self, settings=None):
         self.settings = settings or Settings()
         self.template_dict = self.DEFAULT_TEMPLATE
 
-    def deserialize(self, msg_buff: bytes):
+    def deserialize(self, msg_buff: bytes) -> Message:
         msg = self._parse_message_header(msg_buff)
         if not self.settings.ENABLE_DEFERRED_PACKET_PARSING:
             try:
                 self.parse_message_body(msg)
             except exc.DataPackingError as error:
                 raise exc.MessageDeserializationError(msg.name, error)
         return msg
@@ -81,14 +81,15 @@
         msg_size = len(data)
         if PacketLayout.PACKET_ID_LENGTH >= msg_size:
             raise exc.MessageDeserializationError("packet length", "packet header too short")
 
         reader = se.BufferReader("!", data)
 
         msg: Message = Message("Placeholder")
+        msg.synthetic = False
         msg.send_flags = reader.read(se.U8)
         msg.packet_id = reader.read(se.U32)
 
         # ACK_FLAG - means the incoming packet is ACKing some old packets of ours
         if msg.has_acks:
             # Last byte in the message is the number of acks
             msg_size -= 1
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/message/udpserializer.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/message/udpserializer.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/multidict.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/multidict.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/multiprocessing_utils.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/namevalue.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/namevalue.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/network/__init__.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/network/__init__.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/network/caps_client.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/network/caps_client.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/network/data/ca-bundle.crt` & `hippolyzer-0.9.0/hippolyzer/lib/base/network/data/ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/network/transport.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/network/transport.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/objects.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/objects.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/serialization.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/serialization.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/settings.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/settings.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/templates.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1596,14 +1596,15 @@
     VOCACHE_IS_EMPTY = 0x2  # the cache file is empty, no need to send cache probes.
     SUPPORTS_SELF_APPEARANCE = 0x4  # inbound AvatarAppearance for self is ok
 
 
 @se.flag_field_serializer("TeleportStart", "Info", "TeleportFlags")
 @se.flag_field_serializer("TeleportProgress", "Info", "TeleportFlags")
 @se.flag_field_serializer("TeleportFinish", "Info", "TeleportFlags")
+@se.flag_field_serializer("TeleportLocal", "Info", "TeleportFlags")
 @se.flag_field_serializer("TeleportLureRequest", "Info", "TeleportFlags")
 class TeleportFlags(IntFlag):
     SET_HOME_TO_TARGET = 1 << 0  # newbie leaving prelude (starter area)
     SET_LAST_TO_TARGET = 1 << 1
     VIA_LURE = 1 << 2
     VIA_LANDMARK = 1 << 3
     VIA_LOCATION = 1 << 4
@@ -1614,14 +1615,16 @@
     GODLIKE = 1 << 9
     NINE_ONE_ONE = 1 << 10  # What is this?
     DISABLE_CANCEL = 1 << 11  # Used for llTeleportAgentHome()
     VIA_REGION_ID = 1 << 12
     IS_FLYING = 1 << 13
     SHOW_RESET_HOME = 1 << 14
     FORCE_REDIRECT = 1 << 15
+    VIA_GLOBAL_COORDS = 1 << 16
+    WITHIN_REGION = 1 << 17
 
 
 @se.http_serializer("RenderMaterials")
 class RenderMaterialsSerializer(se.BaseHTTPSerializer):
     @classmethod
     def deserialize_resp_body(cls, method: str, body: bytes):
         deser = llsd.unzip_llsd(llsd.parse_xml(body)["Zipped"])
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/transfer_manager.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/transfer_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         params_dict = dataclasses.asdict(params)
         # Fill in any missing AgentID or SessionID attrs if the params type has them
         if params_dict.get("AgentID", dataclasses.MISSING) is None:
             params.AgentID = self._agent_id
         if params_dict.get("SessionID", dataclasses.MISSING) is None:
             params.SessionID = self._session_id
 
-        self._connection_holder.circuit.send_message(Message(
+        self._connection_holder.circuit.send(Message(
             'TransferRequest',
             Block(
                 'TransferInfo',
                 TransferID=transfer_id,
                 ChannelType=channel_type,
                 SourceType=source_type,
                 Priority=priority,
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/ui_helpers.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/ui_helpers.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/vfs.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/vfs.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/wearables.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/wearables.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/base/xfer_manager.py` & `hippolyzer-0.9.0/hippolyzer/lib/base/xfer_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             vfile_type: Optional[Union[AssetType, int]] = None,
             use_big_packets: bool = False,
             delete_on_completion: bool = True,
             turbo: bool = False,
             direction: Direction = Direction.OUT,
     ) -> Xfer:
         xfer_id = xfer_id if xfer_id is not None else random.getrandbits(64)
-        self._connection_holder.circuit.send_message(Message(
+        self._connection_holder.circuit.send(Message(
             'RequestXfer',
             Block(
                 'XferID',
                 ID=xfer_id,
                 Filename=file_name or b'',
                 FilePath=file_path or XferFilePath.NONE,
                 DeleteOnCompletion=delete_on_completion,
@@ -170,15 +170,15 @@
         to_ack = (packet_id.PacketID,)
         if xfer.turbo:
             # ACK the next few packets we expect to be sent, if we haven't already
             ack_max = packet_id.PacketID + ACK_AHEAD_MAX
             to_ack = range(xfer.next_ackable, ack_max)
             xfer.next_ackable = ack_max
         for ack_id in to_ack:
-            self._connection_holder.circuit.send_message(Message(
+            self._connection_holder.circuit.send(Message(
                 "ConfirmXferPacket",
                 Block("XferID", ID=xfer.xfer_id, Packet=ack_id),
                 direction=xfer.direction,
             ))
 
         xfer.chunks[packet_id.PacketID] = packet_data
         # We may be waiting on other packets so we can't end immediately.
@@ -212,15 +212,15 @@
         xfer = None
         inline_data = b''
         if upload_strategy == UploadStrategy.XFER:
             xfer = Xfer(data=data)
         else:
             inline_data = data
 
-        self._connection_holder.circuit.send_message(Message(
+        self._connection_holder.circuit.send(Message(
             "AssetUploadRequest",
             Block(
                 "AssetBlock",
                 TransactionID=transaction_id,
                 Type=asset_type,
                 Tempfile=temp_file,
                 StoreLocal=store_local,
@@ -268,15 +268,15 @@
 
         packet_id = 0
         # TODO: No resend yet. If it's lost, it's lost.
         while xfer.chunks:
             chunk = xfer.chunks.pop(packet_id)
             # EOF if there are no chunks left
             packet_val = XferPacket(PacketID=packet_id, IsEOF=not bool(xfer.chunks))
-            self._connection_holder.circuit.send_message(Message(
+            self._connection_holder.circuit.send(Message(
                 "SendXferPacket",
                 Block("XferID", ID=xfer.xfer_id, Packet_=packet_val),
                 Block("DataPacket", Data=chunk),
                 # Send this towards the sender of the RequestXfer
                 direction=~request_msg.direction,
             ))
             # Don't care about the value, just want to know it was confirmed.
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/client/namecache.py` & `hippolyzer-0.9.0/hippolyzer/lib/client/namecache.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/client/object_manager.py` & `hippolyzer-0.9.0/hippolyzer/lib/client/object_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,16 +112,16 @@
         session = self._region.session()
         while ids_to_req:
             blocks = [
                 Block("AgentData", AgentID=session.agent_id, SessionID=session.id),
                 *[Block("ObjectData", ObjectLocalID=x) for x in ids_to_req[:255]],
             ]
             # Selecting causes ObjectProperties to be sent
-            self._region.circuit.send_message(Message("ObjectSelect", blocks))
-            self._region.circuit.send_message(Message("ObjectDeselect", blocks))
+            self._region.circuit.send(Message("ObjectSelect", blocks))
+            self._region.circuit.send(Message("ObjectDeselect", blocks))
             ids_to_req = ids_to_req[255:]
 
         futures = []
         for local_id in local_ids:
             if local_id in unselected_ids:
                 # Need to wait until we get our reply
                 fut = self.state.register_future(local_id, UpdateType.PROPERTIES)
@@ -146,15 +146,15 @@
         elif isinstance(local_ids, set):
             local_ids = tuple(local_ids)
 
         session = self._region.session()
 
         ids_to_req = local_ids
         while ids_to_req:
-            self._region.circuit.send_message(Message(
+            self._region.circuit.send(Message(
                 "RequestMultipleObjects",
                 Block("AgentData", AgentID=session.agent_id, SessionID=session.id),
                 *[Block("ObjectData", CacheMissType=0, ID=x) for x in ids_to_req[:255]],
             ))
             ids_to_req = ids_to_req[255:]
 
         futures = []
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/client/state.py` & `hippolyzer-0.9.0/hippolyzer/lib/client/state.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/addon_ctx.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/addon_ctx.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/addon_utils.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/addon_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,25 +69,25 @@
             Audible=True,
             Position=Vector3(),
             Message=text,
         ),
         direction=Direction.IN,
     )
     if session:
-        session.main_region.circuit.send_message(message)
+        session.main_region.circuit.send(message)
     else:
         for session in AddonManager.SESSION_MANAGER.sessions:
-            session.main_region.circuit.send_message(copy.copy(message))
+            session.main_region.circuit.send(copy.copy(message))
 
 
 def send_chat(message: Union[bytes, str], channel=0, chat_type=ChatType.NORMAL, session=None):
     session = session or addon_ctx.session.get(None) or None
     if not session:
         raise RuntimeError("Tried to send chat without session")
-    session.main_region.circuit.send_message(Message(
+    session.main_region.circuit.send(Message(
         "ChatFromViewer",
         Block(
             "AgentData",
             AgentID=session.agent_id,
             SessionID=session.id,
         ),
         Block(
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/addons.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/addons.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/ca_utils.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/ca_utils.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/caps.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/caps.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/caps_client.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/caps_client.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/circuit.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/circuit.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,64 +21,63 @@
 
     def _send_prepared_message(self, message: Message, transport=None):
         try:
             serialized = self.serializer.serialize(message)
         except:
             logging.exception(f"Failed to serialize: {message.to_dict()!r}")
             raise
-        if self.logging_hook and message.injected:
+        if self.logging_hook and message.synthetic:
             self.logging_hook(message)
         return self.send_datagram(serialized, message.direction, transport=transport)
 
     def _get_injections(self, direction: Direction):
         if direction == Direction.OUT:
             return self.out_injections, self.in_injections
         return self.in_injections, self.out_injections
 
-    def prepare_message(self, message: Message, direction=None):
+    def prepare_message(self, message: Message):
         if message.finalized:
             raise RuntimeError(f"Trying to re-send finalized {message!r}")
         if message.queued:
             # This is due to be dropped, nothing should be sending the original
             raise RuntimeError(f"Trying to send original of queued {message!r}")
-        direction = direction or getattr(message, 'direction')
-        fwd_injections, reverse_injections = self._get_injections(direction)
+        fwd_injections, reverse_injections = self._get_injections(message.direction)
+
+        message.finalized = True
 
         # Injected, let's gen an ID
         if message.packet_id is None:
             message.packet_id = fwd_injections.gen_injectable_id()
-            message.injected = True
-        else:
+            message.synthetic = True
+        # This message wasn't injected by the proxy so we need to rewrite packet IDs
+        # to account for IDs the real creator of the packet couldn't have known about.
+        elif not message.synthetic:
             # was_dropped needs the unmodified packet ID
             if fwd_injections.was_dropped(message.packet_id) and message.name != "PacketAck":
                 logging.warning("Attempting to re-send previously dropped %s:%s, did we ack?" %
                                 (message.packet_id, message.name))
             message.packet_id = fwd_injections.get_effective_id(message.packet_id)
             fwd_injections.track_seen(message.packet_id)
-
-        message.finalized = True
-
-        if not message.injected:
-            # This message wasn't injected by the proxy so we need to rewrite packet IDs
-            # to account for IDs the other parties couldn't have known about.
             message.acks = tuple(
                 reverse_injections.get_original_id(x) for x in message.acks
                 if not reverse_injections.was_injected(x)
             )
 
             if message.name == "PacketAck":
-                if not self._rewrite_packet_ack(message, reverse_injections):
-                    logging.debug(f"Dropping {direction} ack for injected packets!")
+                if not self._rewrite_packet_ack(message, reverse_injections) and not message.acks:
+                    logging.debug(f"Dropping {message.direction} ack for injected packets!")
                     # Let caller know this shouldn't be sent at all, it's strictly ACKs for
                     # injected packets.
                     return False
             elif message.name == "StartPingCheck":
                 self._rewrite_start_ping_check(message, fwd_injections)
 
-        if not message.acks:
+        if message.acks:
+            message.send_flags |= PacketFlags.ACK
+        else:
             message.send_flags &= ~PacketFlags.ACK
         return True
 
     def _rewrite_packet_ack(self, message: Message, reverse_injections):
         new_blocks = []
         for block in message["Packets"]:
             packet_id = block["ID"]
@@ -96,39 +95,42 @@
         return True
 
     def _rewrite_start_ping_check(self, message: Message, fwd_injections):
         orig_id = message["PingID"]["OldestUnacked"]
         new_id = fwd_injections.get_effective_id(orig_id)
         if orig_id != new_id:
             logging.debug("Rewrote oldest unacked %s -> %s" % (orig_id, new_id))
+        # Get a list of unacked IDs for the direction this StartPingCheck is heading
+        fwd_unacked = (a for (d, a) in self.unacked_reliable.keys() if d == message.direction)
+        # Use the proxy's oldest unacked ID if it's older than the client's
+        new_id = min((new_id, *fwd_unacked))
         message["PingID"]["OldestUnacked"] = new_id
 
-    def drop_message(self, message: Message, orig_direction=None):
+    def drop_message(self, message: Message):
         if message.finalized:
             raise RuntimeError(f"Trying to drop finalized {message!r}")
         if message.packet_id is None:
             return
-        orig_direction = orig_direction or message.direction
-        fwd_injections, reverse_injections = self._get_injections(orig_direction)
+        fwd_injections, reverse_injections = self._get_injections(message.direction)
 
         fwd_injections.mark_dropped(message.packet_id)
         message.dropped = True
         message.finalized = True
 
         # Was sent reliably, tell the other end that we saw it and to shut up.
         if message.reliable:
-            self.send_acks([message.packet_id], ~orig_direction)
+            self.send_acks([message.packet_id], ~message.direction)
 
         # This packet had acks for the other end, send them in a separate PacketAck
         effective_acks = tuple(
             reverse_injections.get_original_id(x) for x in message.acks
             if not reverse_injections.was_injected(x)
         )
         if effective_acks:
-            self.send_acks(effective_acks, orig_direction, packet_id=message.packet_id)
+            self.send_acks(effective_acks, message.direction, packet_id=message.packet_id)
 
 
 class InjectionTracker:
     # TODO: WARNING! DOESN'T DEAL WITH PACKET ID WRAPAROUND WHATSOEVER!
     #  Circuits that last for hundreds of hours can be expected to break.
     #  Maybe just kill circuit when that happens to prevent silent wonkiness.
     def __init__(self, last_seen_id=0, maxlen=10000):
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/commands.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/commands.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/http_asset_repo.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/http_asset_repo.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/http_event_manager.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/http_event_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
                     eq_manager.cache_last_poll_response(req_ack_id, parsed_eq_resp)
                 flow.response.content = llsd.format_xml(parsed_eq_resp)
             elif cap_data.cap_name in self.UPLOAD_CREATING_CAPS:
                 if not region:
                     return
                 parsed = llsd.parse_xml(flow.response.content)
                 if "uploader" in parsed:
-                    region.register_temporary_cap(cap_data.cap_name + "Uploader", parsed["uploader"])
+                    region.register_cap(cap_data.cap_name + "Uploader", parsed["uploader"], CapType.TEMPORARY)
         except:
             logging.exception("OOPS, blew up in HTTP proxy!")
 
     def _handle_login_flow(self, flow: HippoHTTPFlow):
         resp = xmlrpc.client.loads(flow.response.content)[0][0]  # type: ignore
         sess = self.session_manager.create_session(resp)
         AddonManager.handle_session_init(sess)
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/http_flow.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/http_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.resumed = False
         self.taken = False
         self.callback_queue = weakref.ref(callback_queue) if callback_queue else None
         meta = self.flow.metadata
         meta.setdefault("can_stream", True)
         meta.setdefault("response_injected", False)
         meta.setdefault("request_injected", False)
-        meta.setdefault("cap_data", None)
+        meta.setdefault("cap_data", CapData())
         meta.setdefault("from_browser", False)
 
     @property
     def request(self) -> mitmproxy.http.Request:
         return self.flow.request
 
     @property
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/http_proxy.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/http_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,49 +171,49 @@
         flow.intercept()
         self.intercepted_flows[flow.id] = flow
         self.from_proxy_queue.put((event_type, flow.get_state()), True)
 
     def responseheaders(self, flow: HTTPFlow):
         # The response was injected earlier in an earlier handler,
         # we don't want to touch this anymore.
-        if flow.metadata["response_injected"]:
+        if flow.metadata.get("response_injected"):
             return
 
         # Someone fucked up and put a mimetype in Content-Encoding.
         # I'm assuming this means "identity" because it makes no sense otherwise
         # and will break many clients' (and our) content decoding.
         if flow.response.headers.get("Content-Encoding") == "binary/octet-stream":
             flow.response.headers["X-Broken-Content-Encoding"] = "binary/octet-stream"
             flow.response.headers["Content-Encoding"] = "identity"
 
     def response(self, flow: HTTPFlow):
         cap_data: typing.Optional[SerializedCapData] = flow.metadata.get("cap_data")
-        if flow.metadata["response_injected"] and cap_data and cap_data.asset_server_cap:
+        if flow.metadata.get("response_injected") and cap_data and cap_data.asset_server_cap:
             # Don't bother intercepting asset server requests where we injected a response.
             # We don't want to log them and they don't need any more processing by user hooks.
             return
         self._queue_flow_interception("response", flow)
 
 
 class SLMITMAddon(IPCInterceptionAddon):
     def responseheaders(self, flow: HTTPFlow):
         super().responseheaders(flow)
-        cap_data: typing.Optional[SerializedCapData] = flow.metadata["cap_data_ser"]
+        cap_data: typing.Optional[SerializedCapData] = flow.metadata.get("cap_data_ser")
 
         # Request came from the proxy itself, don't touch it.
-        if flow.metadata["request_injected"]:
+        if flow.metadata.get("request_injected"):
             return
 
         # This is an asset server response that we're not interested in intercepting.
         # Let it stream through and don't try to buffer up the whole response body.
         if cap_data and cap_data.asset_server_cap:
             # Can't stream if we injected our own response or we were asked not to stream
             if not flow.metadata["response_injected"] and flow.metadata["can_stream"]:
                 flow.response.stream = True
-        elif not cap_data and not flow.metadata["from_browser"]:
+        elif not cap_data and not flow.metadata.get("from_browser"):
             object_name = flow.response.headers.get("X-SecondLife-Object-Name", "")
             # Meh. Add some fake Cap data for this so it can be matched on.
             if object_name.startswith("#Firestorm LSL Bridge"):
                 flow.metadata["cap_data_ser"] = SerializedCapData(cap_name="FirestormBridge")
 
 
 class SLMITMMaster(mitmproxy.master.Master):
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/lludp_proxy.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/lludp_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 import weakref
 from typing import Optional, Tuple
 
 from hippolyzer.lib.base.message.message_dot_xml import MessageDotXML
 from hippolyzer.lib.base.message.udpdeserializer import UDPMessageDeserializer
 from hippolyzer.lib.base.message.udpserializer import UDPMessageSerializer
@@ -31,14 +32,25 @@
         self.session_manager: SessionManager = session_manager
         self.serializer = UDPMessageSerializer()
         self.deserializer = UDPMessageDeserializer(
             settings=self.session_manager.settings,
         )
         self.message_xml = MessageDotXML()
         self.session: Optional[Session] = None
+        self.resend_task = asyncio.get_event_loop().create_task(self.attempt_resends())
+
+    async def attempt_resends(self):
+        while True:
+            await asyncio.sleep(0.1)
+            if self.session is None:
+                continue
+            for region in self.session.regions:
+                if not region.circuit or not region.circuit.is_alive:
+                    continue
+                region.circuit.resend_unacked()
 
     def _ensure_message_allowed(self, msg: Message):
         if not self.message_xml.validate_udp_msg(msg.name):
             LOG.warning(
                 f"Received {msg.name!r} over UDP, when it should come over the event queue. Discarding."
             )
             raise PermissionError(f"UDPBanned message {msg.name}")
@@ -95,14 +107,17 @@
                 return
 
         region = self.session.region_by_circuit_addr(packet.far_addr)
         if not region:
             LOG.error("No circuit for %r, dropping packet!" % (packet.far_addr,))
             return
 
+        # Process any ACKs for messages we injected first
+        region.circuit.collect_acks(message)
+
         if message.name == "AgentMovementComplete":
             self.session.main_region = region
             if region.handle is None:
                 region.handle = message["Data"]["RegionHandle"]
             LOG.info(f"Setting main region to {region!r}, had circuit addr {packet.far_addr!r}")
             AddonManager.handle_region_changed(self.session, region)
         if message.name == "RegionHandshake":
@@ -144,15 +159,16 @@
         if message.name in ("CloseCircuit", "DisableSimulator"):
             region.mark_dead()
         elif message.name == "RegionHandshake":
             region.name = str(message["RegionInfo"][0]["SimName"])
 
         # Send the message if it wasn't explicitly dropped or sent before
         if not message.finalized:
-            region.circuit.send_message(message)
+            region.circuit.send(message)
 
     def close(self):
         super().close()
         if self.session:
             AddonManager.handle_session_closed(self.session)
             self.session_manager.close_session(self.session)
         self.session = None
+        self.resend_task.cancel()
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/message_filter.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/message_filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import ast
 import typing
 
 from arpeggio import Optional, ZeroOrMore, EOF, \
-    ParserPython, PTNodeVisitor, visit_parse_tree, RegExMatch
+    ParserPython, PTNodeVisitor, visit_parse_tree, RegExMatch, OneOrMore
 
 
 def literal():
     return [
         # Nightmare. str or bytes literal.
         # https://stackoverflow.com/questions/14366401/#comment79795017_14366904
         RegExMatch(r'''b?(\"\"\"|\'\'\'|\"|\')((?<!\\)(\\\\)*\\\1|.)*?\1'''),
@@ -22,15 +22,17 @@
         RegExMatch(r'\(\s*\d+(\.\d+)?\s*,\s*\d+(\.\d+)?\s*,\s*\d+(\.\d+)?\s*\)'),
         # vector4 (tuple)
         RegExMatch(r'\(\s*\d+(\.\d+)?\s*,\s*\d+(\.\d+)?\s*,\s*\d+(\.\d+)?\s*,\s*\d+(\.\d+)?\s*\)'),
     ]
 
 
 def identifier():
-    return RegExMatch(r'[a-zA-Z*]([a-zA-Z0-9_*]+)?')
+    # Identifiers are allowed to have "-". It's not a special character
+    # in our grammar, and we expect them to show up some places, like header names.
+    return RegExMatch(r'[a-zA-Z*]([a-zA-Z0-9_*-]+)?')
 
 
 def field_specifier():
     return identifier, ZeroOrMore('.', identifier)
 
 
 def unary_field_specifier():
@@ -38,15 +40,15 @@
 
 
 def unary_expression():
     return Optional(["!"]), [unary_field_specifier, ("(", expression, ")")]
 
 
 def meta_field_specifier():
-    return "Meta", ".", identifier
+    return "Meta", OneOrMore(".", identifier)
 
 
 def enum_field_specifier():
     return identifier, ".", identifier
 
 
 def compare_val():
@@ -65,20 +67,25 @@
     return term, ZeroOrMore(["||", "&&"], expression)
 
 
 def message_filter():
     return expression, EOF
 
 
-MATCH_RESULT = typing.Union[bool, typing.Tuple]
+class MatchResult(typing.NamedTuple):
+    result: bool
+    fields: typing.List[typing.Tuple]
+
+    def __bool__(self):
+        return self.result
 
 
 class BaseFilterNode(abc.ABC):
     @abc.abstractmethod
-    def match(self, msg) -> MATCH_RESULT:
+    def match(self, msg, short_circuit=True) -> MatchResult:
         raise NotImplementedError()
 
     @property
     @abc.abstractmethod
     def children(self):
         raise NotImplementedError()
 
@@ -100,43 +107,61 @@
 
     @property
     def children(self):
         return self.left_node, self.right_node
 
 
 class UnaryNotFilterNode(UnaryFilterNode):
-    def match(self, msg) -> MATCH_RESULT:
-        return not self.node.match(msg)
+    def match(self, msg, short_circuit=True) -> MatchResult:
+        # Should we pass fields up here? Maybe not.
+        return MatchResult(not self.node.match(msg, short_circuit), [])
 
 
 class OrFilterNode(BinaryFilterNode):
-    def match(self, msg) -> MATCH_RESULT:
-        return self.left_node.match(msg) or self.right_node.match(msg)
+    def match(self, msg, short_circuit=True) -> MatchResult:
+        left_match = self.left_node.match(msg, short_circuit)
+        if left_match and short_circuit:
+            return MatchResult(True, left_match.fields)
+
+        right_match = self.right_node.match(msg, short_circuit)
+        if right_match and short_circuit:
+            return MatchResult(True, right_match.fields)
+
+        if left_match or right_match:
+            # Fine since fields should be empty when result=False
+            return MatchResult(True, left_match.fields + right_match.fields)
+        return MatchResult(False, [])
 
 
 class AndFilterNode(BinaryFilterNode):
-    def match(self, msg) -> MATCH_RESULT:
-        return self.left_node.match(msg) and self.right_node.match(msg)
+    def match(self, msg, short_circuit=True) -> MatchResult:
+        left_match = self.left_node.match(msg, short_circuit)
+        if not left_match:
+            return MatchResult(False, [])
+        right_match = self.right_node.match(msg, short_circuit)
+        if not right_match:
+            return MatchResult(False, [])
+        return MatchResult(True, left_match.fields + right_match.fields)
 
 
 class MessageFilterNode(BaseFilterNode):
     def __init__(self, selector: typing.Sequence[str], operator: typing.Optional[str], value: typing.Optional):
         self.selector = selector
         self.operator = operator
         self.value = value
 
-    def match(self, msg) -> MATCH_RESULT:
-        return msg.matches(self)
+    def match(self, msg, short_circuit=True) -> MatchResult:
+        return msg.matches(self, short_circuit)
 
     @property
     def children(self):
         return self.selector, self.operator, self.value
 
 
-class MetaFieldSpecifier(str):
+class MetaFieldSpecifier(tuple):
     pass
 
 
 class EnumFieldSpecifier(typing.NamedTuple):
     enum_name: str
     field_name: str
 
@@ -154,15 +179,15 @@
     def visit_field_specifier(self, _node, children):
         return children
 
     def visit_literal(self, node, _children):
         return LiteralValue(ast.literal_eval(node.value))
 
     def visit_meta_field_specifier(self, _node, children):
-        return MetaFieldSpecifier(children[0])
+        return MetaFieldSpecifier(children)
 
     def visit_enum_field_specifier(self, _node, children):
         return EnumFieldSpecifier(*children)
 
     def visit_unary_field_specifier(self, _node, children):
         # Looks like a bare field specifier with no operator
         return MessageFilterNode(tuple(children), None, None)
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/message_logger.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/message_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from hippolyzer.lib.base import serialization as se, llsd
 from hippolyzer.lib.base.message.message import Message
 from hippolyzer.lib.base.datatypes import TaggedUnion, UUID, TupleCoord
 from hippolyzer.lib.base.helpers import bytes_escape
 from hippolyzer.lib.base.message.message_formatting import HumanMessageSerializer
 from hippolyzer.lib.proxy.message_filter import MetaFieldSpecifier, compile_filter, BaseFilterNode, MessageFilterNode, \
-    EnumFieldSpecifier
+    EnumFieldSpecifier, MatchResult
 from hippolyzer.lib.proxy.http_flow import HippoHTTPFlow
 from hippolyzer.lib.proxy.caps import CapType, SerializedCapData
 
 if typing.TYPE_CHECKING:
     from hippolyzer.lib.proxy.region import ProxiedRegion
     from hippolyzer.lib.proxy.sessions import Session
 
@@ -231,15 +231,15 @@
     def _current_selected_full(self):
         selected_local = self._current_selected_local()
         if selected_local is None or self.region is None:
             return None
         obj = self.region.objects.lookup_localid(selected_local)
         return obj and obj.FullID
 
-    def _get_meta(self, name: str):
+    def _get_meta(self, name: str) -> typing.Any:
         # Slight difference in semantics. Filters are meant to return the same
         # thing no matter when they're run, so SelectedLocal and friends resolve
         # to the selected items _at the time the message was logged_. To handle
         # the case where we want to match on the selected object at the time the
         # filter is evaluated, we resolve these here.
         if name == "CurrentSelectedLocal":
             return self._current_selected_local()
@@ -304,15 +304,17 @@
             return True
         if fnmatch.fnmatchcase(self.type, pattern):
             return True
         return False
 
     def _val_matches(self, operator, val, expected):
         if isinstance(expected, MetaFieldSpecifier):
-            expected = self._get_meta(str(expected))
+            if len(expected) != 1:
+                raise ValueError(f"Can only support single-level Meta specifiers, not {expected!r}")
+            expected = self._get_meta(str(expected[0]))
             if not isinstance(expected, (int, float, bytes, str, type(None), tuple)):
                 if callable(expected):
                     expected = expected()
                 else:
                     expected = str(expected)
         elif isinstance(expected, EnumFieldSpecifier):
             # Local import so we get a fresh copy of the templates module
@@ -358,20 +360,26 @@
 
     def _base_matches(self, matcher: "MessageFilterNode") -> typing.Optional[bool]:
         if len(matcher.selector) == 1:
             # Comparison operators would make no sense here
             if matcher.value or matcher.operator:
                 return False
             return self._packet_root_matches(matcher.selector[0])
-        if len(matcher.selector) == 2 and matcher.selector[0] == "Meta":
-            return self._val_matches(matcher.operator, self._get_meta(matcher.selector[1]), matcher.value)
+        if matcher.selector[0] == "Meta":
+            if len(matcher.selector) == 2:
+                return self._val_matches(matcher.operator, self._get_meta(matcher.selector[1]), matcher.value)
+            elif len(matcher.selector) == 3:
+                meta_dict = self._get_meta(matcher.selector[1])
+                if not meta_dict or not hasattr(meta_dict, 'get'):
+                    return False
+                return self._val_matches(matcher.operator, meta_dict.get(matcher.selector[2]), matcher.value)
         return None
 
-    def matches(self, matcher: "MessageFilterNode"):
-        return self._base_matches(matcher) or False
+    def matches(self, matcher: "MessageFilterNode", short_circuit=True) -> "MatchResult":
+        return MatchResult(self._base_matches(matcher) or False, [])
 
     @property
     def seq(self):
         return ""
 
     @property
     def method(self):
@@ -384,27 +392,35 @@
     @staticmethod
     def _format_llsd(parsed):
         xmlified = llsd.format_pretty_xml(parsed)
         # dedent <key> by 1 for easier visual scanning
         xmlified = re.sub(rb" <key>", b"<key>", xmlified)
         return xmlified.decode("utf8", errors="replace")
 
+    @staticmethod
+    def _format_xml(content):
+        beautified = minidom.parseString(content).toprettyxml(indent="  ")
+        # kill blank lines. will break cdata sections. meh.
+        beautified = re.sub(r'\n\s*\n', '\n', beautified, flags=re.MULTILINE)
+        return re.sub(r'<([\w]+)>\s*</\1>', r'<\1></\1>',
+                      beautified, flags=re.MULTILINE)
+
 
 class HTTPMessageLogEntry(AbstractMessageLogEntry):
     __slots__ = ["flow"]
 
     def __init__(self, flow: HippoHTTPFlow):
         self.flow: HippoHTTPFlow = flow
         cap_data = self.flow.cap_data
         region = cap_data and cap_data.region
         session = cap_data and cap_data.session
 
         super().__init__(region, session)
         # This was a request the proxy made through itself
-        self.meta["Injected"] = flow.request_injected
+        self.meta["Synthetic"] = flow.request_injected
 
     @property
     def type(self):
         return "HTTP"
 
     @property
     def name(self):
@@ -472,21 +488,25 @@
                     else:
                         beautified = self._format_llsd(beautified)
                         headers["X-Hippo-Beautify"] = "1"
 
                 if not beautified:
                     content_type = self._guess_content_type(message)
                     if content_type.startswith("application/llsd"):
-                        beautified = self._format_llsd(llsd.parse(message.content))
+                        try:
+                            beautified = self._format_llsd(llsd.parse(message.content))
+                        except llsd.LLSDParseError:
+                            # Sometimes LL sends plain XML with a Content-Type of application/llsd+xml.
+                            # Try to detect that case and work around it
+                            if content_type == "application/llsd+xml" and message.content.startswith(b'<'):
+                                beautified = self._format_xml(message.content)
+                            else:
+                                raise
                     elif any(content_type.startswith(x) for x in ("application/xml", "text/xml")):
-                        beautified = minidom.parseString(message.content).toprettyxml(indent="  ")
-                        # kill blank lines. will break cdata sections. meh.
-                        beautified = re.sub(r'\n\s*\n', '\n', beautified, flags=re.MULTILINE)
-                        beautified = re.sub(r'<([\w]+)>\s*</\1>', r'<\1></\1>',
-                                            beautified, flags=re.MULTILINE)
+                        beautified = self._format_xml(message.content)
             except:
                 LOG.exception("Failed to beautify message")
 
         message_body = beautified or message.content
         if isinstance(message_body, bytes):
             try:
                 decoded = message.text
@@ -537,14 +557,28 @@
             return "application/llsd+xml"
         if message.content.startswith(rb'<llsd>'):
             return "application/llsd+xml"
         if message.content.startswith(rb'<?xml '):
             return "application/xml"
         return content_type
 
+    def _get_meta(self, name: str) -> typing.Any:
+        lower_name = name.lower()
+        if lower_name == "url":
+            return self.flow.request.url
+        elif lower_name == "reqheaders":
+            return self.flow.request.headers
+        elif lower_name == "respheaders":
+            return self.flow.response.headers
+        elif lower_name == "host":
+            return self.flow.request.host.lower()
+        elif lower_name == "status":
+            return self.flow.response.status_code
+        return super()._get_meta(name)
+
     def to_dict(self):
         val = super().to_dict()
         val['flow'] = self.flow.get_state()
         cap_data = val['flow'].get('metadata', {}).get('cap_data_ser')
         if cap_data is not None:
             # Have to convert this from a namedtuple to a dict to make
             # it importable
@@ -609,15 +643,15 @@
         self._name = message.name
         self._direction = message.direction
         self._frozen_message: typing.Optional[bytes] = None
         self._seq = message.packet_id
         super().__init__(region, session)
 
     _MESSAGE_META_ATTRS = {
-        "Injected", "Dropped", "Extra", "Resent", "Zerocoded", "Acks", "Reliable",
+        "Synthetic", "Dropped", "Extra", "Resent", "Zerocoded", "Acks", "Reliable",
     }
 
     def _get_meta(self, name: str):
         # These may change between when the message is logged and when we
         # actually filter on it, since logging happens before addons.
         msg = self.message
         if name in self._MESSAGE_META_ATTRS:
@@ -667,62 +701,69 @@
         if self._message:
             self._direction = self._message.direction
         return self._direction.name if self._direction is not None else ""
 
     def request(self, beautify=False, replacements=None):
         return HumanMessageSerializer.to_human_string(self.message, replacements, beautify)
 
-    def matches(self, matcher):
+    def matches(self, matcher, short_circuit=True) -> "MatchResult":
         base_matched = self._base_matches(matcher)
         if base_matched is not None:
-            return base_matched
+            return MatchResult(base_matched, [])
 
         if not self._packet_root_matches(matcher.selector[0]):
-            return False
+            return MatchResult(False, [])
 
         message = self.message
 
         selector_len = len(matcher.selector)
         # name, block_name, var_name(, subfield_name)?
         if selector_len not in (3, 4):
-            return False
+            return MatchResult(False, [])
+        found_field_keys = []
         for block_name in message.blocks:
             if not fnmatch.fnmatchcase(block_name, matcher.selector[1]):
                 continue
             for block_num, block in enumerate(message[block_name]):
                 for var_name in block.vars.keys():
                     if not fnmatch.fnmatchcase(var_name, matcher.selector[2]):
                         continue
                     # So we know where the match happened
-                    span_key = (message.name, block_name, block_num, var_name)
+                    field_key = (message.name, block_name, block_num, var_name)
                     if selector_len == 3:
                         # We're just matching on the var existing, not having any particular value
                         if matcher.value is None:
-                            return span_key
-                        if self._val_matches(matcher.operator, block[var_name], matcher.value):
-                            return span_key
+                            found_field_keys.append(field_key)
+                        elif self._val_matches(matcher.operator, block[var_name], matcher.value):
+                            found_field_keys.append(field_key)
                     # Need to invoke a special unpacker
                     elif selector_len == 4:
                         try:
                             deserialized = block.deserialize_var(var_name)
                         except KeyError:
                             continue
                         # Discard the tag if this is a tagged union, we only want the value
                         if isinstance(deserialized, TaggedUnion):
                             deserialized = deserialized.value
                         if not isinstance(deserialized, dict):
-                            return False
+                            continue
                         for key in deserialized.keys():
                             if fnmatch.fnmatchcase(str(key), matcher.selector[3]):
                                 if matcher.value is None:
-                                    return span_key
-                                if self._val_matches(matcher.operator, deserialized[key], matcher.value):
-                                    return span_key
-
-        return False
+                                    # Short-circuiting checking individual subfields is fine since
+                                    # we only highlight fields anyway.
+                                    found_field_keys.append(field_key)
+                                    break
+                                elif self._val_matches(matcher.operator, deserialized[key], matcher.value):
+                                    found_field_keys.append(field_key)
+                                    break
+
+                    if short_circuit and found_field_keys:
+                        return MatchResult(True, found_field_keys)
+        return MatchResult(bool(found_field_keys), found_field_keys)
 
     @property
     def summary(self):
         if self._summary is None:
             self._summary = self.message.to_summary()[:500]
         return self._summary
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/namecache.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/namecache.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/object_manager.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/object_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,17 +126,17 @@
     def _run_object_update_hooks(self, obj: Object, updated_props: Set[str], update_type: UpdateType):
         super()._run_object_update_hooks(obj, updated_props, update_type)
         region = self._session.region_by_handle(obj.RegionHandle)
         if self._settings.ALLOW_AUTO_REQUEST_OBJECTS:
             if obj.PCode == PCode.AVATAR and "ParentID" in updated_props:
                 if obj.ParentID and not region.objects.lookup_localid(obj.ParentID):
                     # If an avatar just sat on an object we don't know about, add it to the queued
-                    # cache misses and request if if the viewer doesn't. This should happen
-                    # regardless of the auto-request object setting because otherwise we have no way
-                    # to get a sitting agent's true region location, even if it's ourself.
+                    # cache misses and request it if the viewer doesn't. This should happen
+                    # regardless of the auto-request missing objects setting because otherwise we
+                    # have no way to get a sitting agent's true region location, even if it's ourselves.
                     region.objects.queued_cache_misses.add(obj.ParentID)
                     region.objects.request_missed_cached_objects_soon()
         AddonManager.handle_object_updated(self._session, region, obj, updated_props)
 
     def _run_kill_object_hooks(self, obj: Object):
         super()._run_kill_object_hooks(obj)
         region = self._session.region_by_handle(obj.RegionHandle)
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/region.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/region.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,40 +106,39 @@
             self._caps_url_lookup[cap_url] = (cap_type, name)
 
     def register_wrapper_cap(self, name: str):
         """
         Wrap an existing, non-unique cap with a unique URL
 
         caps like ViewerAsset may be the same globally and wouldn't let us infer
-        which session / region the request was related to without a wrapper
+        which session / region the request was related to without a wrapper URL
+        that we inject into the seed response sent to the viewer.
         """
         parsed = list(urllib.parse.urlsplit(self.caps[name][1]))
         seed_id = self.caps["Seed"][1].split("/")[-1].encode("utf8")
         # Give it a unique domain tied to the current Seed URI
         parsed[1] = f"{name.lower()}-{hashlib.sha256(seed_id).hexdigest()[:16]}.hippo-proxy.localhost"
         # Force the URL to HTTP, we're going to handle the request ourselves so it doesn't need
         # to be secure. This should save on expensive TLS context setup for each req.
         parsed[0] = "http"
         wrapper_url = urllib.parse.urlunsplit(parsed)
-        self.caps.add(name + "ProxyWrapper", (CapType.WRAPPER, wrapper_url))
-        self._recalc_caps()
+        # Register it with "ProxyWrapper" appended so we don't shadow the real cap URL
+        # in our own view of the caps
+        self.register_cap(name + "ProxyWrapper", wrapper_url, CapType.WRAPPER)
         return wrapper_url
 
     def register_proxy_cap(self, name: str):
-        """
-        Register a cap to be completely handled by the proxy
-        """
+        """Register a cap to be completely handled by the proxy"""
         cap_url = f"http://{uuid.uuid4()!s}.caps.hippo-proxy.localhost"
-        self.caps.add(name, (CapType.PROXY_ONLY, cap_url))
-        self._recalc_caps()
+        self.register_cap(name, cap_url, CapType.PROXY_ONLY)
         return cap_url
 
-    def register_temporary_cap(self, name: str, cap_url: str):
+    def register_cap(self, name: str, cap_url: str, cap_type: CapType = CapType.NORMAL):
         """Register a Cap that only has meaning the first time it's used"""
-        self.caps.add(name, (CapType.TEMPORARY, cap_url))
+        self.caps.add(name, (cap_type, cap_url))
         self._recalc_caps()
 
     def resolve_cap(self, url: str, consume=True) -> Optional[Tuple[str, str, CapType]]:
         for cap_url in self._caps_url_lookup.keys():
             if url.startswith(cap_url):
                 cap_type, name = self._caps_url_lookup[cap_url]
                 if cap_type == CapType.TEMPORARY and consume:
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/sessions.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/sessions.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/settings.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/settings.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/socks_proxy.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/socks_proxy.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/task_scheduler.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/templates.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/templates.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/test_utils.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         self.transport = MockTransport()
         self.protocol = InterceptingLLUDPProxyProtocol(
             self.client_addr, self.session_manager)
         self.protocol.transport = self.transport
         self.serializer = UDPMessageSerializer()
         self.session.objects.track_region_objects(123)
 
+    def tearDown(self) -> None:
+        self.protocol.close()
+
     async def _wait_drained(self):
         await asyncio.sleep(0.001)
 
     def _setup_default_circuit(self):
         self._setup_region_circuit(self.session.regions[-1])
         self.session.main_region = self.session.regions[-1]
```

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/transport.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/transport.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/viewer_settings.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/viewer_settings.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/vocache.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/vocache.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer/lib/proxy/webapp_cap_addon.py` & `hippolyzer-0.9.0/hippolyzer/lib/proxy/webapp_cap_addon.py`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/hippolyzer.egg-info/PKG-INFO` & `hippolyzer-0.9.0/hippolyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hippolyzer
-Version: 0.8.0
+Version: 0.9.0
 Summary: Analysis tools for SL-compatible virtual worlds
 Home-page: https://github.com/SaladDais/Hippolyzer/
 Author: Salad Dais
 Author-email: 83434023+SaladDais@users.noreply.github.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `hippolyzer-0.8.0/hippolyzer.egg-info/SOURCES.txt` & `hippolyzer-0.9.0/hippolyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hippolyzer-0.8.0/setup.py` & `hippolyzer-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from os import path
 
 from setuptools import setup, find_packages
 
 here = path.abspath(path.dirname(__file__))
 
-version = '0.8.0'
+version = '0.9.0'
 
 with open(path.join(here, 'README.md')) as readme_fh:
     readme = readme_fh.read()
 
 setup(
     name='hippolyzer',
     version=version,
```

