# Comparing `tmp/opensesame-plugin-titta_eyetracking-0.3.0.tar.gz` & `tmp/opensesame-plugin-titta_eyetracking-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensesame-plugin-titta_eyetracking-0.3.0.tar", last modified: Wed Jul  5 21:35:54 2023, max compression
+gzip compressed data, was "opensesame-plugin-titta_eyetracking-0.4.0.tar", last modified: Thu Jul  6 19:21:59 2023, max compression
```

## Comparing `opensesame-plugin-titta_eyetracking-0.3.0.tar` & `opensesame-plugin-titta_eyetracking-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.198752 opensesame-plugin-titta_eyetracking-0.3.0/
--rw-r--r--   0 bob       (1000) bob       (1000)     3078 2023-07-04 21:15:23.000000 opensesame-plugin-titta_eyetracking-0.3.0/.gitignore
--rwxrwxr--   0 bob       (1000) bob       (1000)    14184 2023-06-02 07:45:26.000000 opensesame-plugin-titta_eyetracking-0.3.0/LICENSE.md
--rw-r--r--   0 bob       (1000) bob       (1000)      106 2022-10-27 05:29:28.000000 opensesame-plugin-titta_eyetracking-0.3.0/MANIFEST.in
--rw-r--r--   0 bob       (1000) bob       (1000)     2228 2023-07-05 21:35:54.198752 opensesame-plugin-titta_eyetracking-0.3.0/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     1576 2023-07-04 13:28:27.000000 opensesame-plugin-titta_eyetracking-0.3.0/README.md
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.196752 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugin_titta_eyetracking.egg-info/
--rw-r--r--   0 bob       (1000) bob       (1000)     2228 2023-07-05 21:35:53.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO
--rw-r--r--   0 bob       (1000) bob       (1000)     1734 2023-07-05 21:35:54.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-05 21:35:53.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugin_titta_eyetracking.egg-info/dependency_links.txt
--rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-05 21:35:53.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugin_titta_eyetracking.egg-info/top_level.txt
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.194752 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.196752 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/
--rw-r--r--   0 bob       (1000) bob       (1000)      256 2023-07-05 21:33:20.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/titta_calibrate.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1739 2023-07-05 21:20:34.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/titta_calibrate.png
--rw-r--r--   0 bob       (1000) bob       (1000)     2202 2023-07-05 19:15:55.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/titta_calibrate.py
--rw-r--r--   0 bob       (1000) bob       (1000)     3239 2023-07-05 21:20:14.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/titta_calibrate_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.197752 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/
--rw-r--r--   0 bob       (1000) bob       (1000)     2097 2023-07-05 21:33:20.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/titta_init.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1487 2023-07-05 21:21:26.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/titta_init.png
--rw-r--r--   0 bob       (1000) bob       (1000)     3022 2023-07-05 19:48:52.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/titta_init.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2289 2023-07-05 21:21:12.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/titta_init_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.197752 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/
--rw-r--r--   0 bob       (1000) bob       (1000)      381 2023-07-05 21:33:20.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/titta_send_message.md
--rw-r--r--   0 bob       (1000) bob       (1000)      805 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/titta_send_message.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1789 2023-07-05 19:15:21.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/titta_send_message.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1305 2023-06-29 21:34:52.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/titta_send_message_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.198752 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/
--rw-r--r--   0 bob       (1000) bob       (1000)      269 2023-07-05 21:33:20.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/titta_start_recording.md
--rw-r--r--   0 bob       (1000) bob       (1000)     1432 2023-07-05 21:27:48.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/titta_start_recording.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1913 2023-07-05 19:15:04.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/titta_start_recording.py
--rw-r--r--   0 bob       (1000) bob       (1000)     2156 2023-07-05 21:27:33.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/titta_start_recording_large.png
-drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-05 21:35:54.198752 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/
--rw-r--r--   0 bob       (1000) bob       (1000)      267 2023-07-05 21:33:20.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/info.yaml
--rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.md
--rw-r--r--   0 bob       (1000) bob       (1000)      804 2023-07-05 21:28:32.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.png
--rw-r--r--   0 bob       (1000) bob       (1000)     1976 2023-07-05 19:32:40.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.py
--rw-r--r--   0 bob       (1000) bob       (1000)     1304 2023-07-05 21:28:17.000000 opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png
--rw-r--r--   0 bob       (1000) bob       (1000)      121 2023-07-05 21:35:54.199752 opensesame-plugin-titta_eyetracking-0.3.0/setup.cfg
--rw-r--r--   0 bob       (1000) bob       (1000)     4097 2023-07-05 21:33:20.000000 opensesame-plugin-titta_eyetracking-0.3.0/setup.py
--rw-r--r--   0 bob       (1000) bob       (1000)      232 2023-07-04 21:24:56.000000 opensesame-plugin-titta_eyetracking-0.3.0/stdeb.cfg
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.406120 opensesame-plugin-titta_eyetracking-0.4.0/
+-rw-r--r--   0 bob       (1000) bob       (1000)     3078 2023-07-04 21:15:23.000000 opensesame-plugin-titta_eyetracking-0.4.0/.gitignore
+-rwxrwxr--   0 bob       (1000) bob       (1000)    14184 2023-07-06 18:44:08.000000 opensesame-plugin-titta_eyetracking-0.4.0/LICENSE.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      106 2022-10-27 05:29:28.000000 opensesame-plugin-titta_eyetracking-0.4.0/MANIFEST.in
+-rw-r--r--   0 bob       (1000) bob       (1000)     2454 2023-07-06 19:21:59.406120 opensesame-plugin-titta_eyetracking-0.4.0/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     1802 2023-07-06 19:15:47.000000 opensesame-plugin-titta_eyetracking-0.4.0/README.md
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.403120 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugin_titta_eyetracking.egg-info/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2454 2023-07-06 19:21:59.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO
+-rw-r--r--   0 bob       (1000) bob       (1000)     1734 2023-07-06 19:21:59.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-06 19:21:59.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugin_titta_eyetracking.egg-info/dependency_links.txt
+-rw-r--r--   0 bob       (1000) bob       (1000)        1 2023-07-06 19:21:59.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugin_titta_eyetracking.egg-info/top_level.txt
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.402120 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.404120 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/
+-rw-r--r--   0 bob       (1000) bob       (1000)      256 2023-07-06 19:18:33.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/titta_calibrate.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1739 2023-07-05 21:20:34.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/titta_calibrate.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     2220 2023-07-06 18:34:54.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/titta_calibrate.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     3239 2023-07-05 21:20:14.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/titta_calibrate_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.404120 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/
+-rw-r--r--   0 bob       (1000) bob       (1000)     2296 2023-07-06 19:18:33.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/titta_init.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1487 2023-07-05 21:21:26.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/titta_init.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     3210 2023-07-06 18:34:54.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/titta_init.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2289 2023-07-05 21:21:12.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/titta_init_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.405120 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/
+-rw-r--r--   0 bob       (1000) bob       (1000)      381 2023-07-06 19:18:33.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/titta_send_message.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      805 2023-06-29 21:35:35.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/titta_send_message.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1731 2023-07-06 18:34:54.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/titta_send_message.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1305 2023-06-29 21:34:52.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/titta_send_message_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.405120 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/
+-rw-r--r--   0 bob       (1000) bob       (1000)      269 2023-07-06 19:18:33.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/titta_start_recording.md
+-rw-r--r--   0 bob       (1000) bob       (1000)     1432 2023-07-05 21:27:48.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/titta_start_recording.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     1940 2023-07-06 18:34:54.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/titta_start_recording.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     2156 2023-07-05 21:27:33.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/titta_start_recording_large.png
+drwxr-xr-x   0 bob       (1000) bob       (1000)        0 2023-07-06 19:21:59.406120 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/
+-rw-r--r--   0 bob       (1000) bob       (1000)      267 2023-07-06 19:18:33.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/info.yaml
+-rw-r--r--   0 bob       (1000) bob       (1000)      120 2023-03-15 11:48:08.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.md
+-rw-r--r--   0 bob       (1000) bob       (1000)      804 2023-07-05 21:28:32.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.png
+-rw-r--r--   0 bob       (1000) bob       (1000)     2070 2023-07-06 18:34:54.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.py
+-rw-r--r--   0 bob       (1000) bob       (1000)     1304 2023-07-05 21:28:17.000000 opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png
+-rw-r--r--   0 bob       (1000) bob       (1000)      121 2023-07-06 19:21:59.406120 opensesame-plugin-titta_eyetracking-0.4.0/setup.cfg
+-rw-r--r--   0 bob       (1000) bob       (1000)     4095 2023-07-06 19:19:38.000000 opensesame-plugin-titta_eyetracking-0.4.0/setup.py
+-rw-r--r--   0 bob       (1000) bob       (1000)      232 2023-07-04 21:24:56.000000 opensesame-plugin-titta_eyetracking-0.4.0/stdeb.cfg
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/.gitignore` & `opensesame-plugin-titta_eyetracking-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/LICENSE.md` & `opensesame-plugin-titta_eyetracking-0.4.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 000001f0: 6620 6265 6e65 6669 7473 2074 6865 204c  f benefits the L
 00000200: 6963 656e 736f 7220 7265 6365 6976 6573  icensor receives
 00000210: 2066 726f 6d20 6d61 6b69 6e67 2074 6865   from making the
 00000220: 204c 6963 656e 7365 6420 4d61 7465 7269   Licensed Materi
 00000230: 616c 2061 7661 696c 6162 6c65 2075 6e64  al available und
 00000240: 6572 2074 6865 7365 2074 6572 6d73 2061  er these terms a
 00000250: 6e64 2063 6f6e 6469 7469 6f6e 732e 0a0a  nd conditions...
-00000260: 2323 2053 6563 7469 6f6e 2031 2096 2044  ## Section 1 . D
+00000260: 2323 2053 6563 7469 6f6e 2031 202d 2044  ## Section 1 - D
 00000270: 6566 696e 6974 696f 6e73 2e0a 0a61 2e20  efinitions...a. 
 00000280: 5f5f 4164 6170 7465 6420 4d61 7465 7269  __Adapted Materi
 00000290: 616c 5f5f 206d 6561 6e73 206d 6174 6572  al__ means mater
 000002a0: 6961 6c20 7375 626a 6563 7420 746f 2043  ial subject to C
 000002b0: 6f70 7972 6967 6874 2061 6e64 2053 696d  opyright and Sim
 000002c0: 696c 6172 2052 6967 6874 7320 7468 6174  ilar Rights that
 000002d0: 2069 7320 6465 7269 7665 6420 6672 6f6d   is derived from
@@ -221,15 +221,15 @@
 00000dc0: 206f 7220 656e 7469 7479 2065 7865 7263   or entity exerc
 00000dd0: 6973 696e 6720 7468 6520 4c69 6365 6e73  ising the Licens
 00000de0: 6564 2052 6967 6874 7320 756e 6465 7220  ed Rights under 
 00000df0: 7468 6973 2050 7562 6c69 6320 4c69 6365  this Public Lice
 00000e00: 6e73 652e 2059 6f75 7220 6861 7320 6120  nse. Your has a 
 00000e10: 636f 7272 6573 706f 6e64 696e 6720 6d65  corresponding me
 00000e20: 616e 696e 672e 0a0a 2323 2053 6563 7469  aning...## Secti
-00000e30: 6f6e 2032 2096 2053 636f 7065 2e0a 0a61  on 2 . Scope...a
+00000e30: 6f6e 2032 202d 2053 636f 7065 2e0a 0a61  on 2 - Scope...a
 00000e40: 2e20 5f5f 5f4c 6963 656e 7365 2067 7261  . ___License gra
 00000e50: 6e74 2e5f 5f5f 0a0a 2020 2031 2e20 5375  nt.___..   1. Su
 00000e60: 626a 6563 7420 746f 2074 6865 2074 6572  bject to the ter
 00000e70: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
 00000e80: 7320 6f66 2074 6869 7320 5075 626c 6963  s of this Public
 00000e90: 204c 6963 656e 7365 2c20 7468 6520 4c69   License, the Li
 00000ea0: 6365 6e73 6f72 2068 6572 6562 7920 6772  censor hereby gr
@@ -309,15 +309,15 @@
 00001340: 5365 6374 696f 6e20 3228 6129 2834 2920  Section 2(a)(4) 
 00001350: 6e65 7665 7220 7072 6f64 7563 6573 2041  never produces A
 00001360: 6461 7074 6564 204d 6174 6572 6961 6c2e  dapted Material.
 00001370: 0a0a 2020 2035 2e20 5f5f 446f 776e 7374  ..   5. __Downst
 00001380: 7265 616d 2072 6563 6970 6965 6e74 732e  ream recipients.
 00001390: 5f5f 0a0a 2020 2020 2020 2041 2e20 5f5f  __..       A. __
 000013a0: 4f66 6665 7220 6672 6f6d 2074 6865 204c  Offer from the L
-000013b0: 6963 656e 736f 7220 9620 4c69 6365 6e73  icensor . Licens
+000013b0: 6963 656e 736f 7220 2d20 4c69 6365 6e73  icensor - Licens
 000013c0: 6564 204d 6174 6572 6961 6c2e 5f5f 2045  ed Material.__ E
 000013d0: 7665 7279 2072 6563 6970 6965 6e74 206f  very recipient o
 000013e0: 6620 7468 6520 4c69 6365 6e73 6564 204d  f the Licensed M
 000013f0: 6174 6572 6961 6c20 6175 746f 6d61 7469  aterial automati
 00001400: 6361 6c6c 7920 7265 6365 6976 6573 2061  cally receives a
 00001410: 6e20 6f66 6665 7220 6672 6f6d 2074 6865  n offer from the
 00001420: 204c 6963 656e 736f 7220 746f 2065 7865   Licensor to exe
@@ -414,15 +414,15 @@
 000019d0: 7279 206c 6963 656e 7369 6e67 2073 6368  ry licensing sch
 000019e0: 656d 652e 2049 6e20 616c 6c20 6f74 6865  eme. In all othe
 000019f0: 7220 6361 7365 7320 7468 6520 4c69 6365  r cases the Lice
 00001a00: 6e73 6f72 2065 7870 7265 7373 6c79 2072  nsor expressly r
 00001a10: 6573 6572 7665 7320 616e 7920 7269 6768  eserves any righ
 00001a20: 7420 746f 2063 6f6c 6c65 6374 2073 7563  t to collect suc
 00001a30: 6820 726f 7961 6c74 6965 732e 0a0a 2323  h royalties...##
-00001a40: 2053 6563 7469 6f6e 2033 2096 204c 6963   Section 3 . Lic
+00001a40: 2053 6563 7469 6f6e 2033 202d 204c 6963   Section 3 - Lic
 00001a50: 656e 7365 2043 6f6e 6469 7469 6f6e 732e  ense Conditions.
 00001a60: 0a0a 596f 7572 2065 7865 7263 6973 6520  ..Your exercise 
 00001a70: 6f66 2074 6865 204c 6963 656e 7365 6420  of the Licensed 
 00001a80: 5269 6768 7473 2069 7320 6578 7072 6573  Rights is expres
 00001a90: 736c 7920 6d61 6465 2073 7562 6a65 6374  sly made subject
 00001aa0: 2074 6f20 7468 6520 666f 6c6c 6f77 696e   to the followin
 00001ab0: 6720 636f 6e64 6974 696f 6e73 2e0a 0a61  g conditions...a
@@ -520,15 +520,15 @@
 00002070: 7320 4c69 6365 6e73 6520 596f 7520 6170  s License You ap
 00002080: 706c 7920 6d75 7374 206e 6f74 2070 7265  ply must not pre
 00002090: 7665 6e74 2072 6563 6970 6965 6e74 7320  vent recipients 
 000020a0: 6f66 2074 6865 2041 6461 7074 6564 204d  of the Adapted M
 000020b0: 6174 6572 6961 6c20 6672 6f6d 2063 6f6d  aterial from com
 000020c0: 706c 7969 6e67 2077 6974 6820 7468 6973  plying with this
 000020d0: 2050 7562 6c69 6320 4c69 6365 6e73 652e   Public License.
-000020e0: 0a0a 2323 2053 6563 7469 6f6e 2034 2096  ..## Section 4 .
+000020e0: 0a0a 2323 2053 6563 7469 6f6e 2034 202d  ..## Section 4 -
 000020f0: 2053 7569 2047 656e 6572 6973 2044 6174   Sui Generis Dat
 00002100: 6162 6173 6520 5269 6768 7473 2e0a 0a57  abase Rights...W
 00002110: 6865 7265 2074 6865 204c 6963 656e 7365  here the License
 00002120: 6420 5269 6768 7473 2069 6e63 6c75 6465  d Rights include
 00002130: 2053 7569 2047 656e 6572 6973 2044 6174   Sui Generis Dat
 00002140: 6162 6173 6520 5269 6768 7473 2074 6861  abase Rights tha
 00002150: 7420 6170 706c 7920 746f 2059 6f75 7220  t apply to Your 
@@ -577,15 +577,15 @@
 00002400: 626c 6967 6174 696f 6e73 2075 6e64 6572  bligations under
 00002410: 2074 6869 7320 5075 626c 6963 204c 6963   this Public Lic
 00002420: 656e 7365 2077 6865 7265 2074 6865 204c  ense where the L
 00002430: 6963 656e 7365 6420 5269 6768 7473 2069  icensed Rights i
 00002440: 6e63 6c75 6465 206f 7468 6572 2043 6f70  nclude other Cop
 00002450: 7972 6967 6874 2061 6e64 2053 696d 696c  yright and Simil
 00002460: 6172 2052 6967 6874 732e 0a0a 2323 2053  ar Rights...## S
-00002470: 6563 7469 6f6e 2035 2096 2044 6973 636c  ection 5 . Discl
+00002470: 6563 7469 6f6e 2035 202d 2044 6973 636c  ection 5 - Discl
 00002480: 6169 6d65 7220 6f66 2057 6172 7261 6e74  aimer of Warrant
 00002490: 6965 7320 616e 6420 4c69 6d69 7461 7469  ies and Limitati
 000024a0: 6f6e 206f 6620 4c69 6162 696c 6974 792e  on of Liability.
 000024b0: 0a0a 612e 205f 5f55 6e6c 6573 7320 6f74  ..a. __Unless ot
 000024c0: 6865 7277 6973 6520 7365 7061 7261 7465  herwise separate
 000024d0: 6c79 2075 6e64 6572 7461 6b65 6e20 6279  ly undertaken by
 000024e0: 2074 6865 204c 6963 656e 736f 722c 2074   the Licensor, t
@@ -670,15 +670,15 @@
 000029d0: 7468 6174 2c20 746f 2074 6865 2065 7874  that, to the ext
 000029e0: 656e 7420 706f 7373 6962 6c65 2c20 6d6f  ent possible, mo
 000029f0: 7374 2063 6c6f 7365 6c79 2061 7070 726f  st closely appro
 00002a00: 7869 6d61 7465 7320 616e 2061 6273 6f6c  ximates an absol
 00002a10: 7574 6520 6469 7363 6c61 696d 6572 2061  ute disclaimer a
 00002a20: 6e64 2077 6169 7665 7220 6f66 2061 6c6c  nd waiver of all
 00002a30: 206c 6961 6269 6c69 7479 2e0a 0a23 2320   liability...## 
-00002a40: 5365 6374 696f 6e20 3620 9620 5465 726d  Section 6 . Term
+00002a40: 5365 6374 696f 6e20 3620 2d20 5465 726d  Section 6 - Term
 00002a50: 2061 6e64 2054 6572 6d69 6e61 7469 6f6e   and Termination
 00002a60: 2e0a 0a61 2e20 5468 6973 2050 7562 6c69  ...a. This Publi
 00002a70: 6320 4c69 6365 6e73 6520 6170 706c 6965  c License applie
 00002a80: 7320 666f 7220 7468 6520 7465 726d 206f  s for the term o
 00002a90: 6620 7468 6520 436f 7079 7269 6768 7420  f the Copyright 
 00002aa0: 616e 6420 5369 6d69 6c61 7220 5269 6768  and Similar Righ
 00002ab0: 7473 206c 6963 656e 7365 6420 6865 7265  ts licensed here
@@ -733,15 +733,15 @@
 00002dc0: 6e6f 7420 7465 726d 696e 6174 6520 7468  not terminate th
 00002dd0: 6973 2050 7562 6c69 6320 4c69 6365 6e73  is Public Licens
 00002de0: 652e 0a0a 642e 2053 6563 7469 6f6e 7320  e...d. Sections 
 00002df0: 312c 2035 2c20 362c 2037 2c20 616e 6420  1, 5, 6, 7, and 
 00002e00: 3820 7375 7276 6976 6520 7465 726d 696e  8 survive termin
 00002e10: 6174 696f 6e20 6f66 2074 6869 7320 5075  ation of this Pu
 00002e20: 626c 6963 204c 6963 656e 7365 2e0a 0a23  blic License...#
-00002e30: 2320 5365 6374 696f 6e20 3720 9620 4f74  # Section 7 . Ot
+00002e30: 2320 5365 6374 696f 6e20 3720 2d20 4f74  # Section 7 - Ot
 00002e40: 6865 7220 5465 726d 7320 616e 6420 436f  her Terms and Co
 00002e50: 6e64 6974 696f 6e73 2e0a 0a61 2e20 5468  nditions...a. Th
 00002e60: 6520 4c69 6365 6e73 6f72 2073 6861 6c6c  e Licensor shall
 00002e70: 206e 6f74 2062 6520 626f 756e 6420 6279   not be bound by
 00002e80: 2061 6e79 2061 6464 6974 696f 6e61 6c20   any additional 
 00002e90: 6f72 2064 6966 6665 7265 6e74 2074 6572  or different ter
 00002ea0: 6d73 206f 7220 636f 6e64 6974 696f 6e73  ms or conditions
@@ -756,15 +756,15 @@
 00002f30: 6c20 6e6f 7420 7374 6174 6564 2068 6572  l not stated her
 00002f40: 6569 6e20 6172 6520 7365 7061 7261 7465  ein are separate
 00002f50: 2066 726f 6d20 616e 6420 696e 6465 7065   from and indepe
 00002f60: 6e64 656e 7420 6f66 2074 6865 2074 6572  ndent of the ter
 00002f70: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
 00002f80: 7320 6f66 2074 6869 7320 5075 626c 6963  s of this Public
 00002f90: 204c 6963 656e 7365 2e0a 0a23 2320 5365   License...## Se
-00002fa0: 6374 696f 6e20 3820 9620 496e 7465 7270  ction 8 . Interp
+00002fa0: 6374 696f 6e20 3820 2d20 496e 7465 7270  ction 8 - Interp
 00002fb0: 7265 7461 7469 6f6e 2e0a 0a61 2e20 466f  retation...a. Fo
 00002fc0: 7220 7468 6520 6176 6f69 6461 6e63 6520  r the avoidance 
 00002fd0: 6f66 2064 6f75 6274 2c20 7468 6973 2050  of doubt, this P
 00002fe0: 7562 6c69 6320 4c69 6365 6e73 6520 646f  ublic License do
 00002ff0: 6573 206e 6f74 2c20 616e 6420 7368 616c  es not, and shal
 00003000: 6c20 6e6f 7420 6265 2069 6e74 6572 7072  l not be interpr
 00003010: 6574 6564 2074 6f2c 2072 6564 7563 652c  eted to, reduce,
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/PKG-INFO` & `opensesame-plugin-titta_eyetracking-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-titta_eyetracking
-Version: 0.3.0
+Version: 0.4.0
 Summary: Titta Eye Tracking plugin for OpenSesame
 Home-page: https://github.com/dev-jam/opensesame-plugin-titta_eyetracking
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-OpenSesame Plug-in: Titta Eye Tracking
-==========
+# OpenSesame Plugin: Titta Eye Tracking
 
-*An OpenSesame plug-in for Titta Eye Tracking.*  
+*Copyright, 2023, Bob Rosbag, Diederick C. Niehorster & Marcus Nyström*
 
-Copyright, 2023, Bob Rosbag  
+## About
 
-
-## 1. About
---------
-
-This plug-in can be used to use Titta for Eye Tracking. 
+This plugin implements Titta in OpenSesame for Eye Tracking. 
 
 Titta is a toolbox for using eye trackers from Tobii Pro AB with Python, specifically offering integration with PsychoPy. A Matlab version that integrates with PsychToolbox is also available from https://github.com/dcnieho/Titta. For a similar toolbox for SMI eye trackers, please see www.github.com/marcus-nystrom/SMITE.
 
 Cite as: Niehorster, D.C., Andersson, R. & Nystrom, M. (2020). Titta: A toolbox for creating PsychToolbox and Psychopy experiments with Tobii eye trackers. Behavior Research Methods. doi: 10.3758/s13428-020-01358-8
 
 Please mention: Bob Rosbag as creator of this plugin
 
-For questions, bug reports or to check for updates on Titta, please visit https://github.com/marcus-nystrom/Titta.
+For questions, bug reports or to check for updates, please visit https://github.com/marcus-nystrom/Titta.
 
 To minimize the risk of missing samples, the current repository uses TittaPy (pip install TittaPy), a C++ wrapper around the Tobii SDK, to pull samples made available from the eye tracker.
 
 
-## 2. LICENSE
-----------
+IMPORTANT: This plugin needs PsychoPy as backend AND the dimensions and distance of the monitor have to be set in the PsychoPy monitor config file (for example ~/.psychopy3/testMonitor.json)
+
 
-The Titta Eye Tracking plug-in is distributed under the terms of the GNU General Public License 3.
-The full license should be included in the file COPYING, or can be obtained from
+## License
 
-- <http://www.gnu.org/licenses/gpl.txt>
+The Titta Eye Tracking plugin is distributed under the terms of the Creative Commons Attribution 4.0 International Public License
+The full license should be included in the file LICENSE.md
 
-This plug-in contains works of others.
-  
-  
-## 3. Documentation
-----------------
 
-Installation instructions and documentation on OpenSesame are available on the documentation website:
+## Known bugs
 
-- <http://osdoc.cogsci.nl/>
+- In dummy mode, when the experiment is finished, OpenSesame will not return to the GUI. The button with the cross and text: 'Forcibly kill the experiment' has to be used to end the session and get back to the GUI. This only happens when in dummy mode and the cause resides somewhere in the 'calibrate' command.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/README.md` & `opensesame-plugin-titta_eyetracking-0.4.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,31 @@
-OpenSesame Plug-in: Titta Eye Tracking
-==========
+# OpenSesame Plugin: Titta Eye Tracking
 
-*An OpenSesame plug-in for Titta Eye Tracking.*  
+*Copyright, 2023, Bob Rosbag, Diederick C. Niehorster & Marcus Nyström*
 
-Copyright, 2023, Bob Rosbag  
+## About
 
-
-## 1. About
---------
-
-This plug-in can be used to use Titta for Eye Tracking. 
+This plugin implements Titta in OpenSesame for Eye Tracking. 
 
 Titta is a toolbox for using eye trackers from Tobii Pro AB with Python, specifically offering integration with PsychoPy. A Matlab version that integrates with PsychToolbox is also available from https://github.com/dcnieho/Titta. For a similar toolbox for SMI eye trackers, please see www.github.com/marcus-nystrom/SMITE.
 
 Cite as: Niehorster, D.C., Andersson, R. & Nystrom, M. (2020). Titta: A toolbox for creating PsychToolbox and Psychopy experiments with Tobii eye trackers. Behavior Research Methods. doi: 10.3758/s13428-020-01358-8
 
 Please mention: Bob Rosbag as creator of this plugin
 
-For questions, bug reports or to check for updates on Titta, please visit https://github.com/marcus-nystrom/Titta.
+For questions, bug reports or to check for updates, please visit https://github.com/marcus-nystrom/Titta.
 
 To minimize the risk of missing samples, the current repository uses TittaPy (pip install TittaPy), a C++ wrapper around the Tobii SDK, to pull samples made available from the eye tracker.
 
 
-## 2. LICENSE
-----------
+IMPORTANT: This plugin needs PsychoPy as backend AND the dimensions and distance of the monitor have to be set in the PsychoPy monitor config file (for example ~/.psychopy3/testMonitor.json)
+
 
-The Titta Eye Tracking plug-in is distributed under the terms of the GNU General Public License 3.
-The full license should be included in the file COPYING, or can be obtained from
+## License
 
-- <http://www.gnu.org/licenses/gpl.txt>
+The Titta Eye Tracking plugin is distributed under the terms of the Creative Commons Attribution 4.0 International Public License
+The full license should be included in the file LICENSE.md
 
-This plug-in contains works of others.
-  
-  
-## 3. Documentation
-----------------
 
-Installation instructions and documentation on OpenSesame are available on the documentation website:
+## Known bugs
 
-- <http://osdoc.cogsci.nl/>
+- In dummy mode, when the experiment is finished, OpenSesame will not return to the GUI. The button with the cross and text: 'Forcibly kill the experiment' has to be used to end the session and get back to the GUI. This only happens when in dummy mode and the cause resides somewhere in the 'calibrate' command.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugin_titta_eyetracking.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 Metadata-Version: 2.1
 Name: opensesame-plugin-titta-eyetracking
-Version: 0.3.0
+Version: 0.4.0
 Summary: Titta Eye Tracking plugin for OpenSesame
 Home-page: https://github.com/dev-jam/opensesame-plugin-titta_eyetracking
 Author: Bob Rosbag
 Author-email: debian@bobrosbag.nl
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Environment :: MacOS X
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-OpenSesame Plug-in: Titta Eye Tracking
-==========
+# OpenSesame Plugin: Titta Eye Tracking
 
-*An OpenSesame plug-in for Titta Eye Tracking.*  
+*Copyright, 2023, Bob Rosbag, Diederick C. Niehorster & Marcus Nyström*
 
-Copyright, 2023, Bob Rosbag  
+## About
 
-
-## 1. About
---------
-
-This plug-in can be used to use Titta for Eye Tracking. 
+This plugin implements Titta in OpenSesame for Eye Tracking. 
 
 Titta is a toolbox for using eye trackers from Tobii Pro AB with Python, specifically offering integration with PsychoPy. A Matlab version that integrates with PsychToolbox is also available from https://github.com/dcnieho/Titta. For a similar toolbox for SMI eye trackers, please see www.github.com/marcus-nystrom/SMITE.
 
 Cite as: Niehorster, D.C., Andersson, R. & Nystrom, M. (2020). Titta: A toolbox for creating PsychToolbox and Psychopy experiments with Tobii eye trackers. Behavior Research Methods. doi: 10.3758/s13428-020-01358-8
 
 Please mention: Bob Rosbag as creator of this plugin
 
-For questions, bug reports or to check for updates on Titta, please visit https://github.com/marcus-nystrom/Titta.
+For questions, bug reports or to check for updates, please visit https://github.com/marcus-nystrom/Titta.
 
 To minimize the risk of missing samples, the current repository uses TittaPy (pip install TittaPy), a C++ wrapper around the Tobii SDK, to pull samples made available from the eye tracker.
 
 
-## 2. LICENSE
-----------
+IMPORTANT: This plugin needs PsychoPy as backend AND the dimensions and distance of the monitor have to be set in the PsychoPy monitor config file (for example ~/.psychopy3/testMonitor.json)
+
 
-The Titta Eye Tracking plug-in is distributed under the terms of the GNU General Public License 3.
-The full license should be included in the file COPYING, or can be obtained from
+## License
 
-- <http://www.gnu.org/licenses/gpl.txt>
+The Titta Eye Tracking plugin is distributed under the terms of the Creative Commons Attribution 4.0 International Public License
+The full license should be included in the file LICENSE.md
 
-This plug-in contains works of others.
-  
-  
-## 3. Documentation
-----------------
 
-Installation instructions and documentation on OpenSesame are available on the documentation website:
+## Known bugs
 
-- <http://osdoc.cogsci.nl/>
+- In dummy mode, when the experiment is finished, OpenSesame will not return to the GUI. The button with the cross and text: 'Forcibly kill the experiment' has to be used to end the session and get back to the GUI. This only happens when in dummy mode and the cause resides somewhere in the 'calibrate' command.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugin_titta_eyetracking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/titta_calibrate.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/titta_calibrate.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/titta_calibrate.py` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/titta_calibrate.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,17 @@
         item.prepare(self)
         self._check_init()
 
     def run(self):
         """The run phase of the plug-in goes here."""
         from titta import helpers_tobii
         self.fixation_point = helpers_tobii.MyDot2(self.experiment.window)
-        
+
         self._show_message('Starting calibration')
+        self.set_item_onset()
         #  Calibrate
         if self.experiment.titta_bimonocular_calibration == 'yes':
             self.experiment.tracker.calibrate(self.experiment.window, eye='left', calibration_number='first')
             self.experiment.tracker.calibrate(self.experiment.window, eye='right', calibration_number='second')
         elif self.experiment.titta_bimonocular_calibration == 'no':
             self.experiment.tracker.calibrate(self.experiment.window)
 
@@ -51,11 +52,11 @@
         debug.msg(message)
         if self.verbose == u'yes':
             print(message)
 
 
 class qttitta_calibrate(titta_calibrate, qtautoplugin):
     """This class handles the GUI aspect of the plug-in."""
-    
+
     def __init__(self, name, experiment, script=None):
         titta_calibrate.__init__(self, name, experiment, script)
         qtautoplugin.__init__(self, __file__)
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_calibrate/titta_calibrate_large.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_calibrate/titta_calibrate_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/info.yaml` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/info.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 description: Titta Eye Tracking Init.
-version: 0.3.0
+version: 0.4.0
 author: "Bob Rosbag"
 url: "http://osdoc.cogsci.nl/"
 category: "Titta Eye Tracking"
 date: "2023"
 controls:
 -
     type: "checkbox"
@@ -49,15 +49,16 @@
     type: "line_edit"
     var: "ncalibration_targets"
     label: "Number of calibration targets"
     name: "line_edit_widget_ncal"
     tooltip: "An example line_edit widget"
 -
     type: "text"
-    label: "\n\n\nTitta is a toolbox for using eye trackers from Tobii Pro AB with Python, specifically offering integration with PsychoPy. \n\n\
+    label: "\n\nIMPORTANT: This plugin needs PsychoPy as backend AND the dimensions and distance of the monitor have to be set in the PsychoPy monitor config file (for example ~/.psychopy3/testMonitor.json)\n\n\n\
+    Titta is a toolbox for using eye trackers from Tobii Pro AB with Python, specifically offering integration with PsychoPy.\n\n\
     Cite as:\n\nNiehorster, D.C., Andersson, R. & Nystrom, M. (2020). Titta: A toolbox for creating PsychToolbox and Psychopy experiments with Tobii eye trackers. Behavior Research Methods. doi: 10.3758/s13428-020-01358-8\n\n\
     Please mention: Bob Rosbag as creator of this plugin\n\n
     For questions, bug reports or to check for updates on Titta, please visit https://github.com/marcus-nystrom/Titta.\n\n\
     To minimize the risk of missing samples, the current repository uses TittaPy (pip install TittaPy), a C++ wrapper around the Tobii SDK, to pull samples made available from the eye tracker."
 -
     type: "text"
-    label: "Version 0.3.0"
+    label: "Version 0.4.0"
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/titta_init.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/titta_init.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/titta_init.py` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/titta_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,46 +25,53 @@
         self.var.ncalibration_targets = '3'
 
     def prepare(self):
         """The preparation phase of the plug-in goes here."""
         # Call the parent constructor.
         item.prepare(self)
         self._init_var()
-        
+        self._check_init()
+
         try:
             from titta import Titta
         except:
             print('Could not import titta')
-        
+
         if self.experiment.canvas_backend != 'psycho':
             raise osexception(
                     u'Titta only supports PsychoPy as backend')
-        
-        self.file_name = 'subject-' + str(self.experiment.subject_nr) + '_TOBII_output.hd5'
-        
+
+        self.file_name = 'subject-' + str(self.experiment.subject_nr) + '_TOBII_output'
+
         if self.experiment.experiment_path:
             self.fname = self.experiment.experiment_path + os.sep + self.file_name
         else:
             self.fname = self.file_name
-        
+
         print('Data will be stored in: %s' % self.fname)
-        
+
         self.settings = Titta.get_defaults(self.var.tracker)
         self.settings.FILENAME = self.fname
         self.settings.N_CAL_TARGETS = self.var.ncalibration_targets
         self.settings.DEBUG = False
-        
+
         # %% Connect to eye tracker and calibrate
         self._show_message('Initialising Eye Tracker')
+        self.set_item_onset()
         self.experiment.tracker = Titta.Connect(self.settings)
         if self.var.dummy_mode == 'yes':
              self._show_message('Dummy mode activated')
              self.experiment.tracker.set_dummy_mode()
         self.experiment.tracker.init()
 
+    def _check_init(self):
+        if hasattr(self.experiment, 'tracker'):
+            raise osexception(
+                'You should have only one instance of `titta_init` in your experiment')
+
     def run(self):
         """The run phase of the plug-in goes here."""
         pass
 
     def _init_var(self):
         self.dummy_mode = self.var.dummy_mode
         self.verbose = self.var.verbose
@@ -76,11 +83,11 @@
         debug.msg(message)
         if self.verbose == u'yes':
             print(message)
 
 
 class qttitta_init(titta_init, qtautoplugin):
     """This class handles the GUI aspect of the plug-in."""
-    
+
     def __init__(self, name, experiment, script=None):
         titta_init.__init__(self, name, experiment, script)
         qtautoplugin.__init__(self, __file__)
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_init/titta_init_large.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_init/titta_init_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/titta_send_message.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/titta_send_message.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/titta_send_message.py` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/titta_send_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """The preparation phase of the plug-in goes here."""
         # Call the parent constructor.
         item.prepare(self)
         self._check_init()
 
     def run(self):
         """The run phase of the plug-in goes here."""
-        #self._show_message('Sending message to Eye Tracker: %s' % self.var.message)
+        self.set_item_onset()
         self.experiment.tracker.send_message(self.var.message)
 
     def _check_init(self):
         if hasattr(self.experiment, "titta_dummy_mode"):
             self.dummy_mode = self.experiment.titta_dummy_mode
             self.verbose = self.experiment.titta_verbose
         else:
@@ -43,11 +43,11 @@
         debug.msg(message)
         if self.verbose == u'yes':
             print(message)
 
 
 class qttitta_send_message(titta_send_message, qtautoplugin):
     """This class handles the GUI aspect of the plug-in."""
-    
+
     def __init__(self, name, experiment, script=None):
         titta_send_message.__init__(self, name, experiment, script)
-        qtautoplugin.__init__(self, __file__)
+        qtautoplugin.__init__(self, __file__)
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_send_message/titta_send_message_large.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_send_message/titta_send_message_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/titta_start_recording.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/titta_start_recording.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/titta_start_recording.py` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/titta_start_recording.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         """The preparation phase of the plug-in goes here."""
         # Call the parent constructor.
         item.prepare(self)
         self._check_init()
 
     def run(self):
         """The run phase of the plug-in goes here."""
+        self.set_item_onset()
         self.experiment.tracker.start_recording(gaze=True,
                                 time_sync=True,
                                 eye_image=False,
                                 notifications=True,
                                 external_signal=True,
                                 positioning=True)
 
@@ -48,11 +49,11 @@
         debug.msg(message)
         if self.verbose == u'yes':
             print(message)
 
 
 class qttitta_start_recording(titta_start_recording, qtautoplugin):
     """This class handles the GUI aspect of the plug-in."""
-    
+
     def __init__(self, name, experiment, script=None):
         titta_start_recording.__init__(self, name, experiment, script)
-        qtautoplugin.__init__(self, __file__)
+        qtautoplugin.__init__(self, __file__)
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_start_recording/titta_start_recording_large.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_start_recording/titta_start_recording_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.py` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/titta_stop_recording.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,21 +24,23 @@
         """The preparation phase of the plug-in goes here."""
         # Call the parent constructor.
         item.prepare(self)
         self._check_init()
 
     def run(self):
         """The run phase of the plug-in goes here."""
+        # Stop streams (if available). Normally only gaze stream is stopped
+        self.set_item_onset()
         self.experiment.tracker.stop_recording(gaze=True,
                                time_sync=True,
                                eye_image=False,
                                notifications=True,
                                external_signal=True,
                                positioning=True)
-        
+
         # Save data
         self.experiment.tracker.save_data()
 
     def _check_init(self):
         if hasattr(self.experiment, "titta_dummy_mode"):
             self.dummy_mode = self.experiment.titta_dummy_mode
             self.verbose = self.experiment.titta_verbose
@@ -51,11 +53,11 @@
         debug.msg(message)
         if self.verbose == u'yes':
             print(message)
 
 
 class qttitta_stop_recording(titta_stop_recording, qtautoplugin):
     """This class handles the GUI aspect of the plug-in."""
-    
+
     def __init__(self, name, experiment, script=None):
         titta_stop_recording.__init__(self, name, experiment, script)
         qtautoplugin.__init__(self, __file__)
```

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png` & `opensesame-plugin-titta_eyetracking-0.4.0/opensesame_plugins/titta_stop_recording/titta_stop_recording_large.png`

 * *Files identical despite different names*

### Comparing `opensesame-plugin-titta_eyetracking-0.3.0/setup.py` & `opensesame-plugin-titta_eyetracking-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
 Author: Bob Rosbag
 2022
 
-This plug-in is free software: you can redistribute it and/or modify
+This plugin is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This software is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with this plug-in.  If not, see <http://www.gnu.org/licenses/>.
+along with this plugin.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 import os
 from setuptools import setup
 
 
 def get_readme():
@@ -29,15 +29,15 @@
         with open('README.md') as fd:
             return fd.read()
     return 'No readme information'
 
 
 setup(
     name='opensesame-plugin-titta_eyetracking',
-    version='0.3.0',
+    version='0.4.0',
     description='Titta Eye Tracking plugin for OpenSesame',
     long_description=get_readme(),
     long_description_content_type='text/markdown',
     author='Bob Rosbag',
     author_email='debian@bobrosbag.nl',
     url='https://github.com/dev-jam/opensesame-plugin-titta_eyetracking',
     # Classifiers used by PyPi if you upload the plugin there
```

