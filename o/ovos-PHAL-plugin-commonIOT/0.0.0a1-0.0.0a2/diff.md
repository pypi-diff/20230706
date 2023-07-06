# Comparing `tmp/ovos-PHAL-plugin-commonIOT-0.0.0a1.tar.gz` & `tmp/ovos-PHAL-plugin-commonIOT-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-commonIOT-0.0.0a1.tar", last modified: Wed Jul  5 23:34:37 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-commonIOT-0.0.0a2.tar", last modified: Wed Jul  5 23:47:34 2023, max compression
```

## Comparing `ovos-PHAL-plugin-commonIOT-0.0.0a1.tar` & `ovos-PHAL-plugin-commonIOT-0.0.0a2.tar`

### file list

```diff
@@ -1,64 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.024965 ovos-PHAL-plugin-commonIOT-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 23:34:37.024965 ovos-PHAL-plugin-commonIOT-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.020965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/device_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.016965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.016965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.020965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/device.not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.action.not.available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.current.brightness.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.current.color.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.status.not.available.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/no_area.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/no_device_class.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/no_entity.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.020965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/entities/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/entities/color.entity
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.024965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.decrease.brightness.intent
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.get.brightness.intent
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.get.color.intent
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.increase.brightness.intent
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.set.brightness.intent
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.set.color.intent
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.get.volume.intent
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.mute.intent
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.set.volume.intent
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.unmute.intent
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.volume.down.intent
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.volume.up.intent
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/reboot.intent
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/sleep.intent
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/turn.off.intent
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/turn.on.intent
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/tv.get.active.app.intent
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/tv.set.active.app.intent
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/tv.set.channel.intent
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/wakeup.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.024965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/close.voc
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/color.voc
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/max.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/min.voc
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/open.voc
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/temperature.voc
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/temperature_unit.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/turn.voc
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/tv.voc
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/window.voc
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 23:34:32.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/vui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:34:37.020965 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 23:34:36.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-05 23:34:36.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:34:36.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-05 23:34:36.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 23:34:36.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 23:34:36.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:34:36.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:34:37.024965 ovos-PHAL-plugin-commonIOT-0.0.0a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2768 2023-07-05 23:34:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.840129 ovos-PHAL-plugin-commonIOT-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 23:47:34.840129 ovos-PHAL-plugin-commonIOT-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.828129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/device_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.828129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.828129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.832129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/device.not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.action.not.available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.current.brightness.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.current.color.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/lights.status.not.available.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/no_area.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/no_device_class.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/dialogs/no_entity.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.832129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/entities/color.entity
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.836129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.decrease.brightness.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.get.brightness.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.get.color.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.increase.brightness.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.set.brightness.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/lights.set.color.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.get.volume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.mute.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.set.volume.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.unmute.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.volume.down.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/mediaplayer.volume.up.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/reboot.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/sleep.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/turn.off.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/turn.on.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/tv.get.active.app.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/tv.set.active.app.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/tv.set.channel.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/intents/wakeup.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.836129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/close.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/color.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/max.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/min.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/open.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/temperature.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/temperature_unit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/turn.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/tv.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/window.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.836129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/opm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/opm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/opm/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/opm/lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/opm/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/opm/players.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 23:47:29.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/vui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:47:34.832129 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-05 23:47:34.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-05 23:47:34.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:47:34.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-05 23:47:34.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 23:47:34.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 23:47:34.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:47:34.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:47:34.840129 ovos-PHAL-plugin-commonIOT-0.0.0a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2768 2023-07-05 23:47:25.000000 ovos-PHAL-plugin-commonIOT-0.0.0a2/setup.py
```

### Comparing `ovos-PHAL-plugin-commonIOT-0.0.0a1/PKG-INFO` & `ovos-PHAL-plugin-commonIOT-0.0.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-commonIOT
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-commonIOT
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/device_manager.py` & `ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/device_manager.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT/plugin.py` & `ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT/plugin.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/PKG-INFO` & `ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-commonIOT
-Version: 0.0.0a1
+Version: 0.0.0a2
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-commonIOT
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-commonIOT-0.0.0a1/ovos_PHAL_plugin_commonIOT.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-commonIOT-0.0.0a2/ovos_PHAL_plugin_commonIOT.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,8 +46,13 @@
 ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/max.voc
 ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/min.voc
 ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/open.voc
 ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/temperature.voc
 ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/temperature_unit.voc
 ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/turn.voc
 ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/tv.voc
-ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/window.voc
+ovos_PHAL_plugin_commonIOT/locale/en-us/vocab/window.voc
+ovos_PHAL_plugin_commonIOT/opm/__init__.py
+ovos_PHAL_plugin_commonIOT/opm/base.py
+ovos_PHAL_plugin_commonIOT/opm/lights.py
+ovos_PHAL_plugin_commonIOT/opm/misc.py
+ovos_PHAL_plugin_commonIOT/opm/players.py
```

### Comparing `ovos-PHAL-plugin-commonIOT-0.0.0a1/setup.py` & `ovos-PHAL-plugin-commonIOT-0.0.0a2/setup.py`

 * *Files identical despite different names*

