# Comparing `tmp/nsz-4.2.1.tar.gz` & `tmp/nsz-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsz-4.2.1.tar", last modified: Tue Dec 13 22:57:05 2022, max compression
+gzip compressed data, was "nsz-4.3.0.tar", last modified: Thu Jul  6 13:50:01 2023, max compression
```

## Comparing `nsz-4.2.1.tar` & `nsz-4.3.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.704721 nsz-4.2.1/
--rw-rw-rw-   0        0        0    14887 2022-12-13 22:57:05.703710 nsz-4.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    12518 2022-12-08 21:10:34.000000 nsz-4.2.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.584693 nsz-4.2.1/nsz/
--rw-rw-rw-   0        0        0    10290 2022-12-08 19:50:26.000000 nsz-4.2.1/nsz/BlockCompressor.py
--rw-rw-rw-   0        0        0     2302 2020-09-04 20:34:54.000000 nsz-4.2.1/nsz/BlockDecompressorReader.py
--rw-rw-rw-   0        0        0     2833 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/ExtractTitlekeys.py
--rw-rw-rw-   0        0        0     6804 2022-12-08 20:07:11.000000 nsz-4.2.1/nsz/FileExistingChecks.py
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.620709 nsz-4.2.1/nsz/Fs/
--rw-rw-rw-   0        0        0     5552 2020-09-05 17:02:35.000000 nsz-4.2.1/nsz/Fs/BaseFs.py
--rw-rw-rw-   0        0        0     7491 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Bktr.py
--rw-rw-rw-   0        0        0     2142 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Cnmt.py
--rw-rw-rw-   0        0        0    14879 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/File.py
--rw-rw-rw-   0        0        0     4699 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Hfs0.py
--rw-rw-rw-   0        0        0     1395 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Ivfc.py
--rw-rw-rw-   0        0        0    18339 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Nacp.py
--rw-rw-rw-   0        0        0     8911 2020-09-05 18:10:42.000000 nsz-4.2.1/nsz/Fs/Nca.py
--rw-rw-rw-   0        0        0    13186 2022-10-03 17:43:34.000000 nsz-4.2.1/nsz/Fs/Nsp.py
--rw-rw-rw-   0        0        0     5725 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Pfs0.py
--rw-rw-rw-   0        0        0     1783 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Rom.py
--rw-rw-rw-   0        0        0     6278 2022-10-03 17:43:34.000000 nsz-4.2.1/nsz/Fs/Ticket.py
--rw-rw-rw-   0        0        0      552 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/Type.py
--rw-rw-rw-   0        0        0     9553 2020-09-02 00:56:55.000000 nsz-4.2.1/nsz/Fs/Xci.py
--rw-rw-rw-   0        0        0      908 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Fs/__init__.py
--rw-rw-rw-   0        0        0      743 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/Header.py
--rw-rw-rw-   0        0        0     3942 2022-12-08 20:07:11.000000 nsz-4.2.1/nsz/IndependentNczDecompressor.py
--rw-rw-rw-   0        0        0     9430 2022-12-08 20:07:11.000000 nsz-4.2.1/nsz/NszDecompressor.py
--rw-rw-rw-   0        0        0     6160 2022-12-08 19:26:15.000000 nsz-4.2.1/nsz/ParseArguments.py
--rw-rw-rw-   0        0        0     1532 2022-12-08 20:07:11.000000 nsz-4.2.1/nsz/PathTools.py
--rw-rw-rw-   0        0        0      366 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/SectionFs.py
--rw-rw-rw-   0        0        0     7051 2022-12-08 20:07:54.000000 nsz-4.2.1/nsz/SolidCompressor.py
--rw-rw-rw-   0        0        0      428 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/ThreadSafeCounter.py
--rw-rw-rw-   0        0        0    11220 2022-12-08 21:18:51.000000 nsz-4.2.1/nsz/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.647698 nsz-4.2.1/nsz/gui/
--rw-rw-rw-   0        0        0      940 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/AboutDialog.py
--rw-rw-rw-   0        0        0     1478 2020-08-30 22:49:38.000000 nsz-4.2.1/nsz/gui/DraggableScrollbar.py
--rw-rw-rw-   0        0        0     1602 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/FileDialogs.py
--rw-rw-rw-   0        0        0     5767 2020-12-24 23:45:55.000000 nsz-4.2.1/nsz/gui/GameList.py
--rw-rw-rw-   0        0        0      159 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/GuiPath.py
--rw-rw-rw-   0        0        0     2685 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/Hyperlink.py
--rw-rw-rw-   0        0        0     1650 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/KivyOnTop.py
--rw-rw-rw-   0        0        0     5815 2022-12-13 22:47:08.000000 nsz-4.2.1/nsz/gui/NSZ_GUI.py
--rw-rw-rw-   0        0        0     2862 2022-12-13 22:45:55.000000 nsz-4.2.1/nsz/gui/RootWidget.py
--rw-rw-rw-   0        0        0     1360 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/SettingScrollOptions.py
--rw-rw-rw-   0        0        0     1434 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/ShaderWidget.py
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.658701 nsz-4.2.1/nsz/gui/fonts/
--rw-rw-rw-   0        0        0  1754936 2020-08-31 22:31:18.000000 nsz-4.2.1/nsz/gui/fonts/MPLUS1p-Medium.ttf
--rw-rw-rw-   0        0        0     4393 2020-08-31 22:31:18.000000 nsz-4.2.1/nsz/gui/fonts/OFL.txt
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.665700 nsz-4.2.1/nsz/gui/json/
--rw-rw-rw-   0        0        0     1621 2022-12-13 22:23:43.000000 nsz-4.2.1/nsz/gui/json/settings_advanced.json
--rw-rw-rw-   0        0        0     1607 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/json/settings_basic.json
--rw-rw-rw-   0        0        0      616 2020-08-31 22:31:18.000000 nsz-4.2.1/nsz/gui/json/settings_tools.json
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.680715 nsz-4.2.1/nsz/gui/layout/
--rw-rw-rw-   0        0        0     1763 2020-08-31 22:31:18.000000 nsz-4.2.1/nsz/gui/layout/AboutDialog.kv
--rw-rw-rw-   0        0        0      113 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/layout/GUI.kv
--rw-rw-rw-   0        0        0     2583 2020-08-31 22:31:18.000000 nsz-4.2.1/nsz/gui/layout/GameList.kv
--rw-rw-rw-   0        0        0      352 2020-08-31 22:31:18.000000 nsz-4.2.1/nsz/gui/layout/Hyperlink.kv
--rw-rw-rw-   0        0        0     1263 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/layout/OpenFileDialog.kv
--rw-rw-rw-   0        0        0     2365 2020-08-31 22:31:18.000000 nsz-4.2.1/nsz/gui/layout/RootWidget.kv
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.682716 nsz-4.2.1/nsz/gui/shaders/
--rw-rw-rw-   0        0        0      599 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/gui/shaders/plasma.shader
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.684704 nsz-4.2.1/nsz/gui/txt/
--rw-rw-rw-   0        0        0     1566 2022-12-08 21:14:11.000000 nsz-4.2.1/nsz/gui/txt/license.txt
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.693718 nsz-4.2.1/nsz/nut/
--rw-rw-rw-   0        0        0     1066 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/nut/Hex.py
--rw-rw-rw-   0        0        0     5757 2022-10-16 22:59:27.000000 nsz-4.2.1/nsz/nut/Keys.py
--rw-rw-rw-   0        0        0      621 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/nut/Print.py
--rw-rw-rw-   0        0        0     1417 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/nut/Titles.py
--rw-rw-rw-   0        0        0    25572 2020-08-11 01:14:07.000000 nsz-4.2.1/nsz/nut/aes128.py
--rw-rw-rw-   0        0        0     3957 2021-06-26 23:57:40.000000 nsz-4.2.1/nsz/undupe.py
-drwxrwxrwx   0        0        0        0 2022-12-13 22:57:05.701709 nsz-4.2.1/nsz.egg-info/
--rw-rw-rw-   0        0        0     1281 2022-12-13 22:57:05.000000 nsz-4.2.1/nsz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      594 2022-10-03 17:43:34.000000 nsz-4.2.1/nsz.py
--rw-rw-rw-   0        0        0       42 2022-12-13 22:57:05.705711 nsz-4.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1197 2022-12-13 22:51:44.000000 nsz-4.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.938816 nsz-4.3.0/
+-rw-rw-rw-   0        0        0     1400 2020-08-11 01:14:07.000000 nsz-4.3.0/LICENSE
+-rw-rw-rw-   0        0        0    14352 2023-07-06 13:50:01.937806 nsz-4.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13770 2023-07-06 12:07:20.000000 nsz-4.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.831800 nsz-4.3.0/nsz/
+-rw-rw-rw-   0        0        0    10343 2023-06-22 23:31:37.000000 nsz-4.3.0/nsz/BlockCompressor.py
+-rw-rw-rw-   0        0        0     2302 2020-09-04 20:34:54.000000 nsz-4.3.0/nsz/BlockDecompressorReader.py
+-rw-rw-rw-   0        0        0     2833 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/ExtractTitlekeys.py
+-rw-rw-rw-   0        0        0     6804 2022-12-08 20:07:11.000000 nsz-4.3.0/nsz/FileExistingChecks.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.869791 nsz-4.3.0/nsz/Fs/
+-rw-rw-rw-   0        0        0     5552 2020-09-05 17:02:35.000000 nsz-4.3.0/nsz/Fs/BaseFs.py
+-rw-rw-rw-   0        0        0     7491 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Bktr.py
+-rw-rw-rw-   0        0        0     2142 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Cnmt.py
+-rw-rw-rw-   0        0        0    14879 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/File.py
+-rw-rw-rw-   0        0        0     4699 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Hfs0.py
+-rw-rw-rw-   0        0        0     1395 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Ivfc.py
+-rw-rw-rw-   0        0        0    18339 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Nacp.py
+-rw-rw-rw-   0        0        0     8911 2020-09-05 18:10:42.000000 nsz-4.3.0/nsz/Fs/Nca.py
+-rw-rw-rw-   0        0        0    13186 2022-10-03 17:43:34.000000 nsz-4.3.0/nsz/Fs/Nsp.py
+-rw-rw-rw-   0        0        0     7167 2023-07-05 16:25:07.000000 nsz-4.3.0/nsz/Fs/Pfs0.py
+-rw-rw-rw-   0        0        0     1783 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Rom.py
+-rw-rw-rw-   0        0        0     6443 2023-07-05 22:08:01.000000 nsz-4.3.0/nsz/Fs/Ticket.py
+-rw-rw-rw-   0        0        0      552 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/Type.py
+-rw-rw-rw-   0        0        0     9553 2020-09-02 00:56:55.000000 nsz-4.3.0/nsz/Fs/Xci.py
+-rw-rw-rw-   0        0        0      908 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Fs/__init__.py
+-rw-rw-rw-   0        0        0      743 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/Header.py
+-rw-rw-rw-   0        0        0     3942 2022-12-08 20:07:11.000000 nsz-4.3.0/nsz/IndependentNczDecompressor.py
+-rw-rw-rw-   0        0        0    11010 2023-07-06 11:32:26.000000 nsz-4.3.0/nsz/NszDecompressor.py
+-rw-rw-rw-   0        0        0     6900 2023-07-06 11:45:03.000000 nsz-4.3.0/nsz/ParseArguments.py
+-rw-rw-rw-   0        0        0     1532 2022-12-08 20:07:11.000000 nsz-4.3.0/nsz/PathTools.py
+-rw-rw-rw-   0        0        0      366 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/SectionFs.py
+-rw-rw-rw-   0        0        0     7184 2023-06-22 23:31:37.000000 nsz-4.3.0/nsz/SolidCompressor.py
+-rw-rw-rw-   0        0        0      428 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/ThreadSafeCounter.py
+-rw-rw-rw-   0        0        0    12142 2023-07-06 12:27:31.000000 nsz-4.3.0/nsz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.890814 nsz-4.3.0/nsz/gui/
+-rw-rw-rw-   0        0        0      940 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/AboutDialog.py
+-rw-rw-rw-   0        0        0     1478 2020-08-30 22:49:38.000000 nsz-4.3.0/nsz/gui/DraggableScrollbar.py
+-rw-rw-rw-   0        0        0     1602 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/FileDialogs.py
+-rw-rw-rw-   0        0        0     5767 2020-12-24 23:45:55.000000 nsz-4.3.0/nsz/gui/GameList.py
+-rw-rw-rw-   0        0        0      159 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/GuiPath.py
+-rw-rw-rw-   0        0        0     2685 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/Hyperlink.py
+-rw-rw-rw-   0        0        0     1650 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/KivyOnTop.py
+-rw-rw-rw-   0        0        0     6291 2023-07-06 12:04:52.000000 nsz-4.3.0/nsz/gui/NSZ_GUI.py
+-rw-rw-rw-   0        0        0     2862 2023-04-11 08:37:41.000000 nsz-4.3.0/nsz/gui/RootWidget.py
+-rw-rw-rw-   0        0        0     1360 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/SettingScrollOptions.py
+-rw-rw-rw-   0        0        0     1434 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/ShaderWidget.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.897798 nsz-4.3.0/nsz/gui/fonts/
+-rw-rw-rw-   0        0        0  1754936 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/fonts/MPLUS1p-Medium.ttf
+-rw-rw-rw-   0        0        0     4393 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/fonts/OFL.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.905801 nsz-4.3.0/nsz/gui/json/
+-rw-rw-rw-   0        0        0     1859 2023-07-06 11:58:43.000000 nsz-4.3.0/nsz/gui/json/settings_advanced.json
+-rw-rw-rw-   0        0        0     2112 2023-07-06 11:58:59.000000 nsz-4.3.0/nsz/gui/json/settings_basic.json
+-rw-rw-rw-   0        0        0      616 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/json/settings_tools.json
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.917801 nsz-4.3.0/nsz/gui/layout/
+-rw-rw-rw-   0        0        0     1763 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/AboutDialog.kv
+-rw-rw-rw-   0        0        0      113 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/layout/GUI.kv
+-rw-rw-rw-   0        0        0     2583 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/GameList.kv
+-rw-rw-rw-   0        0        0      352 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/Hyperlink.kv
+-rw-rw-rw-   0        0        0     1263 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/layout/OpenFileDialog.kv
+-rw-rw-rw-   0        0        0     2365 2020-08-31 22:31:18.000000 nsz-4.3.0/nsz/gui/layout/RootWidget.kv
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.919813 nsz-4.3.0/nsz/gui/shaders/
+-rw-rw-rw-   0        0        0      599 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/gui/shaders/plasma.shader
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.921803 nsz-4.3.0/nsz/gui/txt/
+-rw-rw-rw-   0        0        0     1574 2023-07-06 10:16:02.000000 nsz-4.3.0/nsz/gui/txt/license.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.930807 nsz-4.3.0/nsz/nut/
+-rw-rw-rw-   0        0        0     1066 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/Hex.py
+-rw-rw-rw-   0        0        0     6092 2023-07-06 13:10:18.000000 nsz-4.3.0/nsz/nut/Keys.py
+-rw-rw-rw-   0        0        0      621 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/Print.py
+-rw-rw-rw-   0        0        0     1417 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/Titles.py
+-rw-rw-rw-   0        0        0    25572 2020-08-11 01:14:07.000000 nsz-4.3.0/nsz/nut/aes128.py
+-rw-rw-rw-   0        0        0     3957 2021-06-26 23:57:40.000000 nsz-4.3.0/nsz/undupe.py
+drwxrwxrwx   0        0        0        0 2023-07-06 13:50:01.935815 nsz-4.3.0/nsz.egg-info/
+-rw-rw-rw-   0        0        0     1289 2023-07-06 13:50:01.000000 nsz-4.3.0/nsz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      594 2022-10-03 17:43:34.000000 nsz-4.3.0/nsz.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 13:50:01.938816 nsz-4.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2023-07-06 10:41:21.000000 nsz-4.3.0/setup.py
```

### Comparing `nsz-4.2.1/PKG-INFO` & `nsz-4.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,239 +1,256 @@
 Metadata-Version: 2.1
 Name: nsz
-Version: 4.2.1
+Version: 4.3.0
 Summary: NSZ - Homebrew compatible NSP/XCI compressor/decompressor
 Home-page: https://github.com/nicoboss/nsz
 Author: Nico Bosshard
 Author-email: nico@bosshome.ch
 Maintainer: Nico Bosshard
 Maintainer-email: nico@bosshome.ch
-License: UNKNOWN
-Description: # NSZ
-        A compression/decompresson script (with optional GUI) that allows user to compress/decompress Nintendo Switch ROMs loselessly, thanks to [zstd](https://github.com/facebook/zstd) compression algorithm. The compressed file can be installed directly with supported NSW Homebrew Title Installers.
-        
-        ## Installation:
-        There are several ways the install the script. You can find details on installation for all of them below.\
-        \
-        **You need to have a hactool compatible keys file in a suitable directory to use the script**.\
-        The keys file must be located as `prod.keys` file in `%USERPROFILE%/.switch/`(Windows)/`$HOME/.switch/`(UNIX) or `keys.txt` in the working directory.\
-        \
-        It can be dumped with [Lockpick_RCM](https://github.com/shchmue/Lockpick_RCM/releases).
-        
-        ### Windows Builds
-        You can also use the Windows binaries. They do not require any external libraries to be installed and can be run without installing anything. You can find the binaries in the [release](https://github.com/nicoboss/nsz/releases/) page.
-        
-        **Methods listed below requires you to have Python 3.6+ and pip3 installed.**
-        
-        ### PIP Package
-        Use the following command to install the console-only version:\
-        `pip3 install --upgrade nsz`
-        
-        Use the following command to install the GUI version:\
-        `pip3 install --upgrade nsz[gui]`
-        
-        ### Running from source
-        The tool can also be run by cloning the repository, installing the requirements and then executing nsz using `python3 nsz.py`
-        
-        Use the following command to install the console-only versions requirements:\
-        `pip3 install -r requirements.txt`
-        
-        Use the following command to install the GUI versions requirements:\
-        `pip3 install -r requirements-gui.txt`
-        
-        ## Usage
-        ```
-        nsz --help
-        usage: nsz.py [-h] [-C] [-D] [-l LEVEL] [-L] [-B] [-S] [-s BS] [-V] [-p] [-P]
-                      [-t THREADS] [-m MULTI] [-o [OUTPUT]] [-w] [-r] [--rm-source]
-                      [-i] [--depth DEPTH] [-x] [--extractregex EXTRACTREGEX]
-                      [--titlekeys] [--undupe] [--undupe-dryrun] [--undupe-rename]
-                      [--undupe-hardlink] [--undupe-prioritylist UNDUPE_PRIORITYLIST]
-                      [--undupe-whitelist UNDUPE_WHITELIST]
-                      [--undupe-blacklist UNDUPE_BLACKLIST] [--undupe-old-versions]
-                      [-c CREATE]
-                      [file ...]
-        
-        positional arguments:
-          file
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -C                    Compress NSP/XCI
-          -D                    Decompress NSZ/XCZ/NCZ
-          -l LEVEL, --level LEVEL
-                                Compression Level: Trade-off between compression speed
-                                and compression ratio. Default: 18, Max: 22
-          -L, --long            Enables zStandard long distance mode for even better
-                                compression
-          -B, --block           Use block compression option. This mode allows highly
-                                multi-threaded compression/decompression with random
-                                read access allowing compressed games to be played
-                                without decompression in the future however this comes
-                                with a slightly lower compression ratio cost. This is
-                                the default option for XCZ.
-          -S, --solid           Use solid compression option. Slightly higher
-                                compression ratio but won't allow for random read
-                                access. File compressed this way will never be
-                                mountable (have to be installed or decompressed first
-                                to run). This is the default option for NSZ.
-          -s BS, --bs BS        Block Size for random read access 2^x while x between
-                                14 and 32. Default: 20 => 1 MB
-          -V, --verify          Verifies files after compression raising an unhandled
-                                exception on hash mismatch and verify existing NSP and
-                                NSZ files when given as parameter
-          -p, --parseCnmt       Extract TitleId/Version from Cnmt if this information
-                                cannot be obtained from the filename. Required for
-                                skipping/overwriting existing files and --rm-old-
-                                version to work properly if some not every file is
-                                named properly. Supported filenames:
-                                *TitleID*[vVersion]*
-          -P, --alwaysParseCnmt
-                                Always extract TitleId/Version from Cnmt and never
-                                trust filenames
-          -t THREADS, --threads THREADS
-                                Number of threads to compress with. Numbers < 1
-                                corresponds to the number of logical CPU cores for
-                                block compression and 3 for solid compression
-          -m MULTI, --multi MULTI
-                                Executes multiple compression tasks in parallel. Take
-                                a look at available RAM especially if compression
-                                level is over 18.
-          -o [OUTPUT], --output [OUTPUT]
-                                Directory to save the output NSZ files
-          -w, --overwrite       Continues even if there already is a file with the
-                                same name or title id inside the output directory
-          -r, --rm-old-version  Removes older versions if found
-          --rm-source           Deletes source file/s after compressing/decompressing.
-                                It's recommended to only use this in combination with
-                                --verify
-          -i, --info            Show info about title or file
-          --depth DEPTH         Max depth for file info and extraction
-          -x, --extract         Extract a NSP/XCI/NSZ/XCZ/NSPZ
-          --extractregex EXTRACTREGEX
-                                Regex specifying which files inside the container
-                                should be extracted. Example: "^.*\.(cert|tik)$"
-          --titlekeys           Extracts titlekeys from your NSP/NSZ files and adds
-                                missing keys to ./titlekeys.txt and JSON files inside
-                                ./titledb/ (obtainable from
-                                https://github.com/blawar/titledb). Titlekeys can be
-                                used to unlock updates using NUT OG (OG fork
-                                obtainable from https://github.com/plato79/nut). There
-                                is currently no publicly known way of optioning NSX
-                                files. To MitM: Apply disable_ca_verification &
-                                disable_browser_ca_verification patches, use your
-                                device's nx_tls_client_cert.pfx (Password: switch,
-                                Install to OS and import for Fiddler or import into
-                                Charles/OWASP ZAP). Use it for aauth-
-                                lp1.ndas.srv.nintendo.net:443, dauth-
-                                lp1.ndas.srv.nintendo.net:443 and
-                                app-b01-lp1.npns.srv.nintendo.net:443. Try with your
-                                WiiU first as there you won't get banned if you mess
-                                up.
-          --undupe              Deleted all duplicates (games with same ID and
-                                Version). The Files folder will get parsed in order so
-                                the later in the argument list the more likely the
-                                file is to be deleted
-          --undupe-dryrun       Shows what files would get deleted using --undupe
-          --undupe-rename       Renames files to minimal standard:
-                                [TitleId][vVersion].nsz
-          --undupe-hardlink     Hardlinks files to minimal standard:
-                                [TitleId][vVersion].nsz
-          --undupe-prioritylist UNDUPE_PRIORITYLIST
-                                Regex specifying which dublicates delegtion should be
-                                prioritized before following the normal deletion
-                                order. Example: "^.*\.(nsp|xci)$"
-          --undupe-whitelist UNDUPE_WHITELIST
-                                Regex specifying which dublicates should under no
-                                circumstances be deleted. Example: "^.*\.(nsz|xcz)$"
-          --undupe-blacklist UNDUPE_BLACKLIST
-                                Regex specifying which files should always be deleted
-                                - even if they are not even a dublicate! Be careful!
-                                Example: "^.*\.(nsp|xci)$"
-          --undupe-old-versions
-                                Removes every old version as long there is a newer one
-                                of the same titleID.
-          -c CREATE, --create CREATE
-                                Inverse of --extract. Repacks files/folders to an NSP.
-                                Example: --create out.nsp .\in
-        ```
-        
-        ## Few Usage Examples
-        * To compress all files in a folder: `nsz -C /path/to/folder/with/roms/`
-        * To compress all files in a folder and verifying integrity of compressed files: `nsz --verify -C /path/to/folder/with/roms/`
-        * To compress all files in a folder with 8 threads and outputting resulting files to a new directory: `nsz --threads 8 --output /path/to/out/dir/ -C /path/to/folder/with/roms/`
-        * To compress all files in a folder with level 22 compression level: `nsz --level 22 -C /path/to/folder/with/roms/`
-        * To decompress all files in a folder: `nsz -D /path/to/folder/with/roms/`
-        
-        To view all the possible flags and a description on what each flag, check the [Usage](https://github.com/nicoboss/nsz#usage) section.
-        
-        ## File Format Details
-        
-        ### NSZ
-        NSZ files are functionally identical to NSP files. Their sole purpose to alert the user that it contains compressed NCZ files. NCZ files can be mixed with NCA files in the same container.
-        
-        As an alternative to this tool NSC_Builder also supports compressing NSP to NSZ, and decompressing NSZ to NSP. NSC_Builder can be downloaded at https://github.com/julesontheroad/NSC_BUILDER
-        
-        ### XCZ
-        XCZ files are functionally identical to XCI files. Their sole purpose to alert the user that it contains compressed NCZ files. NCZ files can be mixed with NCA files in the same container.
-        
-        ### NCZ
-        These are compressed NCA files. The NCA's are decrypted, and then compressed using zStandard.
-        
-        The first 0x4000 bytes of an NCZ file is exactly the same as the original NCA (and still encrypted). This applies even if the first section doesn't start at 0x4000.
-        
-        At 0x4000, there is the variable sized NCZ Header. It contains a list of sections which tell the decompressor how to re-encrypt the NCA data after decompression. It can also contain an optional block compression header allowing random read access.
-        
-        All of the information in the header can be derived from the original NCA + Ticket, however it is provided pre-parsed to make decompression as easy as possible for third parties.
-        
-        Directly after the NCZ header, the zStandard stream begins and ends at EOF. The stream is decompressed to offset 0x4000. If block compression is used the stream is splitted into independent blocks and can be decompressed as shown in https://github.com/nicoboss/nsz/blob/master/nsz/BlockDecompressorReader.py. CompressedBlockSizeList[blockID] must not exceed decompressedBlockSize. If smaller the block must be decompressed. If equal the block is stored in plain text.
-        
-        ```python
-        class Section:
-        	def __init__(self, f):
-        		self.magic = f.read(8) # b'NCZSECTN'
-        		self.offset = f.readInt64()
-        		self.size = f.readInt64()
-        		self.cryptoType = f.readInt64()
-        		f.readInt64() # padding
-        		self.cryptoKey = f.read(16)
-        		self.cryptoCounter = f.read(16)
-        
-        class Block:
-        	def __init__(self, f):
-        		self.magic = f.read(8) # b'NCZBLOCK'
-        		self.version = f.readInt8()
-        		self.type = f.readInt8()
-        		self.unused = f.readInt8()
-        		self.blockSizeExponent = f.readInt8()
-        		self.numberOfBlocks = f.readInt32()
-        		self.decompressedSize = f.readInt64()
-        		self.compressedBlockSizeList = []
-        		for i in range(self.numberOfBlocks):
-        			self.compressedBlockSizeList.append(f.readInt32())
-        
-        nspf.seek(0x4000)
-        sectionCount = nspf.readInt64()
-        for i in range(sectionCount):
-        	sections.append(Section(nspf))
-        
-        if blockCompression:
-        	BlockHeader = Block(nspf)
-        ```
-        
-        ## References
-        NSZ pip package: https://pypi.org/project/nsz/  
-        Forum thread: https://gbatemp.net/threads/nsz-homebrew-compatible-nsp-xci-compressor-decompressor.550556/
-        
-        ## Credits
-        SciresM for his hardware crypto functions; the blazing install speeds (50 MB/sec +) achieved here would not be possible without this.
-        
-        Thanks to our contributors: nicoboss, blawar, plato79, eXhumer, Taorni, teknoraver, anthonyu, gabest11, KWottrich, maki-chan, thatch, 2weak2live, pR0Ps, 16BitWonder
-        
 Keywords: nsz,xcz,ncz,nsp,xci,nca,Switch
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: gui
+License-File: LICENSE
+
+# NSZ
+A compression/decompresson script (with optional GUI) that allows user to compress/decompress Nintendo Switch ROMs loselessly, thanks to [zstd](https://github.com/facebook/zstd) compression algorithm. The compressed file can be installed directly with supported NSW Homebrew Title Installers.
+
+## Legal
+- This project does NOT incorporate any copyrighted material such as cryptographic keys. All keys must be provided by the user.
+- This project does NOT circumvent any technological protection measures. The NSZ file format purposely keeps all technological protection measures in place by not decrypting the most crucial parts.
+- This project shall only be used for legally purchased games.
+- This project is MIT licensed. Check [LICENSE](https://github.com/nicoboss/nsz/blob/master/LICENSE) for more information.
+
+## Installation:
+There are several ways the install the script. You can find details on installation for all of them below.\
+\
+**You need to have a hactool compatible keys file in a suitable directory to use the script**.\
+The keys file must be located as `prod.keys` file in `%USERPROFILE%/.switch/`(Windows)/`$HOME/.switch/`(UNIX) or `keys.txt` in the working directory.\
+\
+It can be dumped using Lockpick_RCM.
+
+### Windows Builds
+You can also use the Windows binaries. They do not require any external libraries to be installed and can be run without installing anything. You can find the binaries in the [release](https://github.com/nicoboss/nsz/releases/) page.
+
+**Methods listed below requires you to have Python 3.6+ and pip3 installed.**
+
+### PIP Package
+Use the following command to install the console-only version:\
+`pip3 install --upgrade nsz`
+
+Use the following command to install the GUI version:\
+`pip3 install --upgrade nsz[gui]`
+
+### Running from source
+The tool can also be run by cloning the repository, installing the requirements and then executing nsz using `python3 nsz.py`
+
+Use the following command to install the console-only versions requirements:\
+`pip3 install -r requirements.txt`
+
+Use the following command to install the GUI versions requirements:\
+`pip3 install -r requirements-gui.txt`
+
+## Usage
+```
+nsz.py --help
+usage: nsz.py [-h] [-C] [-D] [-l LEVEL] [-L] [-B] [-S] [-s BS] [-V] [-Q] [-K]
+              [-R] [-p] [-P] [-t THREADS] [-m MULTI] [-o [OUTPUT]] [-w] [-r]
+              [--rm-source] [-i] [--depth DEPTH] [-x]
+              [--extractregex EXTRACTREGEX] [--titlekeys] [--undupe]
+              [--undupe-dryrun] [--undupe-rename] [--undupe-hardlink]
+              [--undupe-prioritylist UNDUPE_PRIORITYLIST]
+              [--undupe-whitelist UNDUPE_WHITELIST]
+              [--undupe-blacklist UNDUPE_BLACKLIST] [--undupe-old-versions]
+              [-c CREATE]
+              [file ...]
+
+positional arguments:
+  file
+
+options:
+  -h, --help            show this help message and exit
+  -C                    Compress NSP/XCI
+  -D                    Decompress NSZ/XCZ/NCZ
+  -l LEVEL, --level LEVEL
+                        Compression Level: Trade-off between compression speed
+                        and compression ratio. Default: 18, Max: 22
+  -L, --long            Enables zStandard long distance mode for even better
+                        compression
+  -B, --block           Use block compression option. This mode allows highly
+                        multi-threaded compression/decompression with random
+                        read access allowing compressed games to be played
+                        without decompression in the future however this comes
+                        with a slightly lower compression ratio cost. This is
+                        the default option for XCZ.
+  -S, --solid           Use solid compression option. Slightly higher
+                        compression ratio but won't allow for random read
+                        access. File compressed this way will never be
+                        mountable (have to be installed or decompressed first
+                        to run). This is the default option for NSZ.
+  -s BS, --bs BS        Block Size for random read access 2^x while x between
+                        14 and 32. Default: 20 => 1 MB
+  -V, --verify          Verifies files after compression raising an unhandled
+                        exception on hash mismatch and verify existing NSP and
+                        NSZ files when given as parameter. Requires --keep-
+                        delta when used during compression.
+  -Q, --quick-verify    Same as --verify but skips the expensive and mostly
+                        useless PFS0 hash verification and only verifies NCA
+                        hashes. Does not require --keep-delta when used during
+                        compression.
+  -K, --keep-delta      Keep all useless delta fragments (NDV0) during
+                        compression so the NSP (PFS0) can be recreated bit-
+                        identical during decompression
+  -R, --remove-padding  Remove the padding between the PFS0 header and the
+                        first file so the NSP matches the nxdumptool/no-intro
+                        standard
+  -p, --parseCnmt       Extract TitleId/Version from Cnmt if this information
+                        cannot be obtained from the filename. Required for
+                        skipping/overwriting existing files and --rm-old-
+                        version to work properly if some not every file is
+                        named properly. Supported filenames:
+                        *TitleID*[vVersion]*
+  -P, --alwaysParseCnmt
+                        Always extract TitleId/Version from Cnmt and never
+                        trust filenames
+  -t THREADS, --threads THREADS
+                        Number of threads to compress with. Numbers < 1
+                        corresponds to the number of logical CPU cores for
+                        block compression and 3 for solid compression
+  -m MULTI, --multi MULTI
+                        Executes multiple compression tasks in parallel. Take
+                        a look at available RAM especially if compression
+                        level is over 18.
+  -o [OUTPUT], --output [OUTPUT]
+                        Directory to save the output NSZ files
+  -w, --overwrite       Continues even if there already is a file with the
+                        same name or title id inside the output directory
+  -r, --rm-old-version  Removes older versions if found
+  --rm-source           Deletes source file/s after compressing/decompressing.
+                        It's recommended to only use this in combination with
+                        --verify
+  -i, --info            Show info about title or file
+  --depth DEPTH         Max depth for file info and extraction
+  -x, --extract         Extract a NSP/XCI/NSZ/XCZ/NSPZ
+  --extractregex EXTRACTREGEX
+                        Regex specifying which files inside the container
+                        should be extracted. Example: "^.*\.(cert|tik)$"
+  --titlekeys           Extracts titlekeys from your NSP/NSZ files and adds
+                        missing keys to ./titlekeys.txt and JSON files inside
+                        ./titledb/ (obtainable from
+                        https://github.com/blawar/titledb). Titlekeys can be
+                        used to unlock updates using NUT OG (OG fork
+                        obtainable from https://github.com/plato79/nut). There
+                        is currently no publicly known way of optioning NSX
+                        files. To MitM: Apply disable_ca_verification &
+                        disable_browser_ca_verification patches, use your
+                        device's nx_tls_client_cert.pfx (Password: switch,
+                        Install to OS and import for Fiddler or import into
+                        Charles/OWASP ZAP). Use it for aauth-
+                        lp1.ndas.srv.nintendo.net:443, dauth-
+                        lp1.ndas.srv.nintendo.net:443 and
+                        app-b01-lp1.npns.srv.nintendo.net:443. Try with your
+                        WiiU first as there you won't get banned if you mess
+                        up.
+  --undupe              Deleted all duplicates (games with same ID and
+                        Version). The Files folder will get parsed in order so
+                        the later in the argument list the more likely the
+                        file is to be deleted
+  --undupe-dryrun       Shows what files would get deleted using --undupe
+  --undupe-rename       Renames files to minimal standard:
+                        [TitleId][vVersion].nsz
+  --undupe-hardlink     Hardlinks files to minimal standard:
+                        [TitleId][vVersion].nsz
+  --undupe-prioritylist UNDUPE_PRIORITYLIST
+                        Regex specifying which dublicate deletion should be
+                        prioritized before following the normal deletion
+                        order. Example: "^.*\.(nsp|xci)$"
+  --undupe-whitelist UNDUPE_WHITELIST
+                        Regex specifying which dublicates should under no
+                        circumstances be deleted. Example: "^.*\.(nsz|xcz)$"
+  --undupe-blacklist UNDUPE_BLACKLIST
+                        Regex specifying which files should always be deleted
+                        - even if they are not even a dublicate! Be careful!
+                        Example: "^.*\.(nsp|xci)$"
+  --undupe-old-versions
+                        Removes every old version as long there is a newer one
+                        of the same titleID.
+  -c CREATE, --create CREATE
+                        Inverse of --extract. Repacks files/folders to an NSP.
+                        Example: --create out.nsp .\in
+```
+
+## Few Usage Examples
+* To compress all files in a folder: `nsz -C /path/to/folder/with/roms/`
+* To compress all files in a folder and verifying integrity of compressed files: `nsz --verify -C /path/to/folder/with/roms/`
+* To compress all files in a folder with 8 threads and outputting resulting files to a new directory: `nsz --threads 8 --output /path/to/out/dir/ -C /path/to/folder/with/roms/`
+* To compress all files in a folder with level 22 compression level: `nsz --level 22 -C /path/to/folder/with/roms/`
+* To decompress all files in a folder: `nsz -D /path/to/folder/with/roms/`
+
+To view all the possible flags and a description on what each flag, check the [Usage](https://github.com/nicoboss/nsz#usage) section.
+
+## File Format Details
+
+### NSZ
+NSZ files are functionally identical to NSP files. Their sole purpose to alert the user that it contains compressed NCZ files. NCZ files can be mixed with NCA files in the same container.
+
+As an alternative to this tool NSC_Builder also supports compressing NSP to NSZ, and decompressing NSZ to NSP. NSC_Builder can be downloaded at https://github.com/julesontheroad/NSC_BUILDER
+
+### XCZ
+XCZ files are functionally identical to XCI files. Their sole purpose to alert the user that it contains compressed NCZ files. NCZ files can be mixed with NCA files in the same container.
+
+### NCZ
+These are compressed NCA files. The NCA's are decrypted, and then compressed using zStandard.
+
+The first 0x4000 bytes of an NCZ file is exactly the same as the original NCA (and still encrypted). This applies even if the first section doesn't start at 0x4000.
+
+At 0x4000, there is the variable sized NCZ Header. It contains a list of sections which tell the decompressor how to re-encrypt the NCA data after decompression. It can also contain an optional block compression header allowing random read access.
+
+All of the information in the header can be derived from the original NCA + Ticket, however it is provided pre-parsed to make decompression as easy as possible for third parties.
+
+Directly after the NCZ header, the zStandard stream begins and ends at EOF. The stream is decompressed to offset 0x4000. If block compression is used the stream is splitted into independent blocks and can be decompressed as shown in https://github.com/nicoboss/nsz/blob/master/nsz/BlockDecompressorReader.py. CompressedBlockSizeList[blockID] must not exceed decompressedBlockSize. If smaller the block must be decompressed. If equal the block is stored in plain text.
+
+```python
+class Section:
+	def __init__(self, f):
+		self.magic = f.read(8) # b'NCZSECTN'
+		self.offset = f.readInt64()
+		self.size = f.readInt64()
+		self.cryptoType = f.readInt64()
+		f.readInt64() # padding
+		self.cryptoKey = f.read(16)
+		self.cryptoCounter = f.read(16)
+
+class Block:
+	def __init__(self, f):
+		self.magic = f.read(8) # b'NCZBLOCK'
+		self.version = f.readInt8()
+		self.type = f.readInt8()
+		self.unused = f.readInt8()
+		self.blockSizeExponent = f.readInt8()
+		self.numberOfBlocks = f.readInt32()
+		self.decompressedSize = f.readInt64()
+		self.compressedBlockSizeList = []
+		for i in range(self.numberOfBlocks):
+			self.compressedBlockSizeList.append(f.readInt32())
+
+nspf.seek(0x4000)
+sectionCount = nspf.readInt64()
+for i in range(sectionCount):
+	sections.append(Section(nspf))
+
+if blockCompression:
+	BlockHeader = Block(nspf)
+```
+
+## References
+NSZ pip package: https://pypi.org/project/nsz/  
+Forum thread: https://gbatemp.net/threads/nsz-homebrew-compatible-nsp-xci-compressor-decompressor.550556/
+
+## Credits
+SciresM for his hardware crypto functions; the blazing install speeds (50 MB/sec +) achieved here would not be possible without this.
+
+Thanks to our contributors: nicoboss, blawar, plato79, eXhumer, Taorni, teknoraver, anthonyu, gabest11, KWottrich, maki-chan, thatch, 2weak2live, pR0Ps, 16BitWonder, drizzt
```

### Comparing `nsz-4.2.1/README.md` & `nsz-4.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # NSZ
 A compression/decompresson script (with optional GUI) that allows user to compress/decompress Nintendo Switch ROMs loselessly, thanks to [zstd](https://github.com/facebook/zstd) compression algorithm. The compressed file can be installed directly with supported NSW Homebrew Title Installers.
 
+## Legal
+- This project does NOT incorporate any copyrighted material such as cryptographic keys. All keys must be provided by the user.
+- This project does NOT circumvent any technological protection measures. The NSZ file format purposely keeps all technological protection measures in place by not decrypting the most crucial parts.
+- This project shall only be used for legally purchased games.
+- This project is MIT licensed. Check [LICENSE](https://github.com/nicoboss/nsz/blob/master/LICENSE) for more information.
+
 ## Installation:
 There are several ways the install the script. You can find details on installation for all of them below.\
 \
 **You need to have a hactool compatible keys file in a suitable directory to use the script**.\
 The keys file must be located as `prod.keys` file in `%USERPROFILE%/.switch/`(Windows)/`$HOME/.switch/`(UNIX) or `keys.txt` in the working directory.\
 \
-It can be dumped with [Lockpick_RCM](https://github.com/shchmue/Lockpick_RCM/releases).
+It can be dumped using Lockpick_RCM.
 
 ### Windows Builds
 You can also use the Windows binaries. They do not require any external libraries to be installed and can be run without installing anything. You can find the binaries in the [release](https://github.com/nicoboss/nsz/releases/) page.
 
 **Methods listed below requires you to have Python 3.6+ and pip3 installed.**
 
 ### PIP Package
@@ -28,29 +34,30 @@
 `pip3 install -r requirements.txt`
 
 Use the following command to install the GUI versions requirements:\
 `pip3 install -r requirements-gui.txt`
 
 ## Usage
 ```
-nsz --help
-usage: nsz.py [-h] [-C] [-D] [-l LEVEL] [-L] [-B] [-S] [-s BS] [-V] [-p] [-P]
-              [-t THREADS] [-m MULTI] [-o [OUTPUT]] [-w] [-r] [--rm-source]
-              [-i] [--depth DEPTH] [-x] [--extractregex EXTRACTREGEX]
-              [--titlekeys] [--undupe] [--undupe-dryrun] [--undupe-rename]
-              [--undupe-hardlink] [--undupe-prioritylist UNDUPE_PRIORITYLIST]
+nsz.py --help
+usage: nsz.py [-h] [-C] [-D] [-l LEVEL] [-L] [-B] [-S] [-s BS] [-V] [-Q] [-K]
+              [-R] [-p] [-P] [-t THREADS] [-m MULTI] [-o [OUTPUT]] [-w] [-r]
+              [--rm-source] [-i] [--depth DEPTH] [-x]
+              [--extractregex EXTRACTREGEX] [--titlekeys] [--undupe]
+              [--undupe-dryrun] [--undupe-rename] [--undupe-hardlink]
+              [--undupe-prioritylist UNDUPE_PRIORITYLIST]
               [--undupe-whitelist UNDUPE_WHITELIST]
               [--undupe-blacklist UNDUPE_BLACKLIST] [--undupe-old-versions]
               [-c CREATE]
               [file ...]
 
 positional arguments:
   file
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -C                    Compress NSP/XCI
   -D                    Decompress NSZ/XCZ/NCZ
   -l LEVEL, --level LEVEL
                         Compression Level: Trade-off between compression speed
                         and compression ratio. Default: 18, Max: 22
   -L, --long            Enables zStandard long distance mode for even better
@@ -66,15 +73,26 @@
                         access. File compressed this way will never be
                         mountable (have to be installed or decompressed first
                         to run). This is the default option for NSZ.
   -s BS, --bs BS        Block Size for random read access 2^x while x between
                         14 and 32. Default: 20 => 1 MB
   -V, --verify          Verifies files after compression raising an unhandled
                         exception on hash mismatch and verify existing NSP and
-                        NSZ files when given as parameter
+                        NSZ files when given as parameter. Requires --keep-
+                        delta when used during compression.
+  -Q, --quick-verify    Same as --verify but skips the expensive and mostly
+                        useless PFS0 hash verification and only verifies NCA
+                        hashes. Does not require --keep-delta when used during
+                        compression.
+  -K, --keep-delta      Keep all useless delta fragments (NDV0) during
+                        compression so the NSP (PFS0) can be recreated bit-
+                        identical during decompression
+  -R, --remove-padding  Remove the padding between the PFS0 header and the
+                        first file so the NSP matches the nxdumptool/no-intro
+                        standard
   -p, --parseCnmt       Extract TitleId/Version from Cnmt if this information
                         cannot be obtained from the filename. Required for
                         skipping/overwriting existing files and --rm-old-
                         version to work properly if some not every file is
                         named properly. Supported filenames:
                         *TitleID*[vVersion]*
   -P, --alwaysParseCnmt
@@ -125,15 +143,15 @@
                         file is to be deleted
   --undupe-dryrun       Shows what files would get deleted using --undupe
   --undupe-rename       Renames files to minimal standard:
                         [TitleId][vVersion].nsz
   --undupe-hardlink     Hardlinks files to minimal standard:
                         [TitleId][vVersion].nsz
   --undupe-prioritylist UNDUPE_PRIORITYLIST
-                        Regex specifying which dublicates delegtion should be
+                        Regex specifying which dublicate deletion should be
                         prioritized before following the normal deletion
                         order. Example: "^.*\.(nsp|xci)$"
   --undupe-whitelist UNDUPE_WHITELIST
                         Regex specifying which dublicates should under no
                         circumstances be deleted. Example: "^.*\.(nsz|xcz)$"
   --undupe-blacklist UNDUPE_BLACKLIST
                         Regex specifying which files should always be deleted
@@ -213,8 +231,8 @@
 ## References
 NSZ pip package: https://pypi.org/project/nsz/  
 Forum thread: https://gbatemp.net/threads/nsz-homebrew-compatible-nsp-xci-compressor-decompressor.550556/
 
 ## Credits
 SciresM for his hardware crypto functions; the blazing install speeds (50 MB/sec +) achieved here would not be possible without this.
 
-Thanks to our contributors: nicoboss, blawar, plato79, eXhumer, Taorni, teknoraver, anthonyu, gabest11, KWottrich, maki-chan, thatch, 2weak2live, pR0Ps, 16BitWonder
+Thanks to our contributors: nicoboss, blawar, plato79, eXhumer, Taorni, teknoraver, anthonyu, gabest11, KWottrich, maki-chan, thatch, 2weak2live, pR0Ps, 16BitWonder, drizzt
```

### Comparing `nsz-4.2.1/nsz/BlockCompressor.py` & `nsz-4.3.0/nsz/BlockCompressor.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 def compressBlockTask(in_queue, out_list, readyForWork, pleaseKillYourself, blockSize):
 	while True:
 		readyForWork.increment()
 		item = in_queue.get()
 		#readyForWork.decrement() # https://github.com/nicoboss/nsz/issues/80
 		if pleaseKillYourself.value() > 0:
 			break
-		buffer, compressionLevel, useLongDistanceMode, compressedblockSizeList, chunkRelativeBlockID = item # compressedblockSizeList IS UNUSED VARIABLE
+		buffer, compressionLevel, useLongDistanceMode, chunkRelativeBlockID = item
 		if buffer == 0:
 			return
 		if compressionLevel == 0 and len(buffer) == blockSize: # https://github.com/nicoboss/nsz/issues/79
 			out_list[chunkRelativeBlockID] = buffer
 		else:
 			params = ZstdCompressionParameters.from_level(compressionLevel, enable_ldm=useLongDistanceMode)
 			compressed = ZstdCompressor(compression_params=params).compress(buffer)
 			out_list[chunkRelativeBlockID] = compressed if len(compressed) < len(buffer) else buffer
 
-def blockCompress(filePath, compressionLevel, useLongDistanceMode, blockSizeExponent, outputDir, threads):
+def blockCompress(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, blockSizeExponent, outputDir, threads):
 	if filePath.suffix == '.nsp':
-		return blockCompressNsp(filePath, compressionLevel, useLongDistanceMode, blockSizeExponent, outputDir, threads)
+		return blockCompressNsp(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, blockSizeExponent, outputDir, threads)
 	elif filePath.suffix == '.xci':
-		return blockCompressXci(filePath, compressionLevel, useLongDistanceMode, blockSizeExponent, outputDir, threads)
+		return blockCompressXci(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, blockSizeExponent, outputDir, threads)
 
-def blockCompressContainer(readContainer, writeContainer, compressionLevel, useLongDistanceMode, blockSizeExponent, threads):
+def blockCompressContainer(readContainer, writeContainer, compressionLevel, keepDelta, useLongDistanceMode, blockSizeExponent, threads):
 	CHUNK_SZ = 0x100000
 	UNCOMPRESSABLE_HEADER_SIZE = 0x4000
 	if blockSizeExponent < 14 or blockSizeExponent > 32:
 		raise ValueError("Block size must be between 14 and 32")
 	blockSize = 2**blockSizeExponent
 	manager = Manager()
 	results = manager.list()
@@ -53,20 +53,18 @@
 	
 	for i in range(threads):
 		p = Process(target=compressBlockTask, args=(work, results, readyForWork, pleaseKillYourself, blockSize))
 		p.start()
 		pool.append(p)
 
 	for nspf in readContainer:
-		if isinstance(nspf, Nca.Nca) and nspf.header.contentType == Type.Content.DATA:
-			Print.info('[SKIPPED]    Delta fragment {0}'.format(nspf._path))
-			continue
-		if nspf._path.endswith('.cnmt.xml'):
-			Print.info('[SKIPPED]    Content meta {0}'.format(nspf._path))
-			continue
+		if not keepDelta:
+			if isinstance(nspf, Nca.Nca) and nspf.header.contentType == Type.Content.DATA:
+				Print.info('[SKIPPED]    Delta fragment {0}'.format(nspf._path))
+				continue
 		if isinstance(nspf, Nca.Nca) and (nspf.header.contentType == Type.Content.PROGRAM or nspf.header.contentType == Type.Content.PUBLICDATA) and nspf.size > UNCOMPRESSABLE_HEADER_SIZE:
 			if isNcaPacked(nspf):
 				
 				offsetFirstSection = sortedFs(nspf)[0].offset
 				newFileName = nspf._path[0:-1] + 'z'
 				f = writeContainer.add(newFileName, nspf.size)
 				startPos = f.tell()
@@ -150,15 +148,15 @@
 							f.write(results[i])
 							results[i] = b""
 
 						if len(buffer) == 0:
 							break
 						chunkRelativeBlockID = 0
 						startChunkBlockID = blockID
-					work.put([buffer, compressionLevel, useLongDistanceMode,compressedblockSizeList, chunkRelativeBlockID])
+					work.put([buffer, compressionLevel, useLongDistanceMode, chunkRelativeBlockID])
 					readyForWork.decrement()
 					blockID += 1
 					chunkRelativeBlockID += 1
 					decompressedBytes += len(buffer)
 					if decompressedBytes - decompressedBytesOld > 10485760: #Refresh every 10 MB
 						decompressedBytesOld = decompressedBytes
 						bar.count = decompressedBytes//1048576
@@ -199,47 +197,47 @@
 		work.put(None)
 		readyForWork.decrement()
 
 	while readyForWork.value() > 0:
 		sleep(0.02)
 
 
-def blockCompressNsp(filePath, compressionLevel, useLongDistanceMode, blockSizeExponent, outputDir, threads):
+def blockCompressNsp(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, blockSizeExponent, outputDir, threads):
 	filePath = filePath.resolve()
 	container = factory(filePath)
 	container.open(str(filePath), 'rb')
 	nszPath = outputDir.joinpath(filePath.stem + '.nsz')
 
 	Print.info(f'Block compressing (level {compressionLevel}{" ldm" if useLongDistanceMode else ""}) {filePath} -> {nszPath}')
 	
 	try:
-		with Pfs0.Pfs0Stream(str(nszPath)) as nsp:
-			blockCompressContainer(container, nsp, compressionLevel, useLongDistanceMode, blockSizeExponent, threads)
+		with Pfs0.Pfs0Stream(container.getHeaderSize() if removePadding else container.getFirstFileOffset(), str(nszPath)) as nsp:
+			blockCompressContainer(container, nsp, compressionLevel, keepDelta, useLongDistanceMode, blockSizeExponent, threads)
 	except BaseException as ex:
 		if not ex is KeyboardInterrupt:
 			Print.error(format_exc())
 		if nszPath.is_file():
 			nszPath.unlink()
 
 	container.close()
 	return nszPath
 	
-def blockCompressXci(filePath, compressionLevel, useLongDistanceMode, blockSizeExponent, outputDir, threads):
+def blockCompressXci(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, blockSizeExponent, outputDir, threads):
 	filePath = filePath.resolve()
 	container = factory(filePath)
 	container.open(str(filePath), 'rb')
 	secureIn = container.hfs0['secure']
 	xczPath = outputDir.joinpath(filePath.stem + '.xcz')
 
 	Print.info(f'Block compressing (level {compressionLevel}{" ldm" if useLongDistanceMode else ""}) {filePath} -> {xczPath}')
 	
 	try:
 		with Xci.XciStream(str(xczPath), originalXciPath = filePath) as xci: # need filepath to copy XCI container settings
 			with Hfs0.Hfs0Stream(xci.hfs0.add('secure', 0), xci.f.tell()) as secureOut:
-				blockCompressContainer(secureIn, secureOut, compressionLevel, useLongDistanceMode, blockSizeExponent, threads)
+				blockCompressContainer(secureIn, secureOut, compressionLevel, keepDelta, useLongDistanceMode, blockSizeExponent, threads)
 			
 			xci.hfs0.resize('secure', secureOut.actualSize)
 	except BaseException as ex:
 		if not ex is KeyboardInterrupt:
 			Print.error(format_exc())
 		if xczPath.is_file():
 			xczPath.unlink()
```

### Comparing `nsz-4.2.1/nsz/BlockDecompressorReader.py` & `nsz-4.3.0/nsz/BlockDecompressorReader.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/ExtractTitlekeys.py` & `nsz-4.3.0/nsz/ExtractTitlekeys.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/FileExistingChecks.py` & `nsz-4.3.0/nsz/FileExistingChecks.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/BaseFs.py` & `nsz-4.3.0/nsz/Fs/BaseFs.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Bktr.py` & `nsz-4.3.0/nsz/Fs/Bktr.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Cnmt.py` & `nsz-4.3.0/nsz/Fs/Cnmt.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/File.py` & `nsz-4.3.0/nsz/Fs/File.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Hfs0.py` & `nsz-4.3.0/nsz/Fs/Hfs0.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Ivfc.py` & `nsz-4.3.0/nsz/Fs/Ivfc.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Nacp.py` & `nsz-4.3.0/nsz/Fs/Nacp.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Nca.py` & `nsz-4.3.0/nsz/Fs/Nca.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Nsp.py` & `nsz-4.3.0/nsz/Fs/Nsp.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Pfs0.py` & `nsz-4.3.0/nsz/Fs/Pfs0.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from nsz.nut import Print
 from nsz.Fs.BaseFs import BaseFs
 from nsz.nut import Titles
 
 MEDIA_SIZE = 0x200
 
 class Pfs0Stream(BaseFile):
-	def __init__(self, path, mode = 'wb'):
+	def __init__(self, headerSize, path, mode = 'wb'):
 		os.makedirs(os.path.dirname(path), exist_ok = True)
 		super(Pfs0Stream, self).__init__(path, mode)
-		self.headerSize = 0x8000
+		self.headerSize = headerSize
 		self.files = []
 		
 		self.actualSize = 0
 
 		self.f.seek(self.headerSize)
 
 	def __enter__(self):
@@ -57,18 +57,27 @@
 		return False
 
 	def close(self):
 		if self.isOpen():
 			self.seek(0)
 			self.write(self.getHeader())
 			super(Pfs0Stream, self).close()
+			
+	def getHeaderSize(self):
+		stringTable = '\x00'.join(file['name'] for file in self.files)
+		headerSize = 0x10 + len(self.files) * 0x18 + len(stringTable)
+		remainder = 0x10 - headerSize % 0x10
+		headerSize += remainder
+		return headerSize
+
+	def getFirstFileOffset(self):
+		return self.files[0].offset
 
 	def getHeader(self):
 		stringTable = '\x00'.join(file['name'] for file in self.files)
-		
 		headerSize = 0x10 + len(self.files) * 0x18 + len(stringTable)
 		remainder = 0x10 - headerSize % 0x10
 		headerSize += remainder
 	
 		h = b''
 		h += b'PFS0'
 		h += len(self.files).to_bytes(4, byteorder='little')
@@ -85,53 +94,101 @@
 			
 			stringOffset += len(f['name']) + 1
 			
 		h += stringTable.encode()
 		h += remainder * b'\x00'
 		
 		return h
+
+
+class Pfs0VerifyStream():
+	def __init__(self, headerSize, mode = 'wb'):
+		self.files = []
+		self.binhash = sha256()
+		self.pos = headerSize
+
+	def __enter__(self):
+		return self
 		
-class Pfs0(BaseFs):
-	def __init__(self, buffer, path = None, mode = None, cryptoType = -1, cryptoKey = -1, cryptoCounter = -1):
-		super(Pfs0, self).__init__(buffer, path, mode, cryptoType, cryptoKey, cryptoCounter)
-		
-		if buffer:
-			self.size = int.from_bytes(buffer[0x48:0x50], byteorder='little', signed=False)
-			self.sectionStart = int.from_bytes(buffer[0x40:0x48], byteorder='little', signed=False)
-			#self.offset += sectionStart
-			#self.size -= sectionStart
-		
-	def getHeader(self):
-		stringTable = '\x00'.join(file.name for file in self.files)
+	def __exit__(self, type, value, traceback):
+		pass
 		
+	def write(self, value, size = None):
+		self.binhash.update(value)
+		self.pos += len(value)
+
+	def tell(self):
+		return self.pos
+
+	def add(self, name, size, pleaseNoPrint = None):
+		Print.info('[ADDING]     {0} {1} bytes to NSP'.format(name, size), pleaseNoPrint)
+		self.files.append({'name': name, 'size': size, 'offset': self.pos})
+		return self
+
+	def resize(self, name, size):
+		for i in self.files:
+			if i['name'] == name:
+				i['size'] = size
+				return True
+		return False
+
+	def close(self):
+		pass
+	
+	def getHash(self):
+		hexHash = self.binhash.hexdigest()
+		return hexHash
+
+	def getHeaderHash(self):
+		stringTable = '\x00'.join(file['name'] for file in self.files)
 		headerSize = 0x10 + len(self.files) * 0x18 + len(stringTable)
 		remainder = 0x10 - headerSize % 0x10
 		headerSize += remainder
 	
 		h = b''
 		h += b'PFS0'
 		h += len(self.files).to_bytes(4, byteorder='little')
 		h += (len(stringTable)+remainder).to_bytes(4, byteorder='little')
 		h += b'\x00\x00\x00\x00'
 		
 		stringOffset = 0
 		
-		for f in range(len(self.files)):
-			h += f.offset.to_bytes(8, byteorder='little')
-			h += f.size.to_bytes(8, byteorder='little')
+		for f in self.files:
+			h += (f['offset'] - headerSize).to_bytes(8, byteorder='little')
+			h += f['size'].to_bytes(8, byteorder='little')
 			h += stringOffset.to_bytes(4, byteorder='little')
 			h += b'\x00\x00\x00\x00'
 			
-			stringOffset += len(f.name) + 1
+			stringOffset += len(f['name']) + 1
 			
 		h += stringTable.encode()
 		h += remainder * b'\x00'
 		
-		return h
+		headerBinhash = sha256()
+		headerBinhash.update(h)
+		headerHexHash = headerBinhash.hexdigest()
+		return headerHexHash
+
+
+class Pfs0(BaseFs):
+	def __init__(self, buffer, path = None, mode = None, cryptoType = -1, cryptoKey = -1, cryptoCounter = -1):
+		super(Pfs0, self).__init__(buffer, path, mode, cryptoType, cryptoKey, cryptoCounter)
 		
+		if buffer:
+			self.size = int.from_bytes(buffer[0x48:0x50], byteorder='little', signed=False)
+			self.sectionStart = int.from_bytes(buffer[0x40:0x48], byteorder='little', signed=False)
+			#self.offset += sectionStart
+			#self.size -= sectionStart
+
+	def getHeaderSize(self):
+		return self._headerSize;
+
+	def getFirstFileOffset(self):
+		return self.files[0].offset
+
 	def open(self, path = None, mode = 'rb', cryptoType = -1, cryptoKey = -1, cryptoCounter = -1):
 		r = super(Pfs0, self).open(path, mode, cryptoType, cryptoKey, cryptoCounter)
 		self.rewind()
 		#self.setupCrypto()
 		#Print.info('cryptoType = ' + hex(self.cryptoType))
 		#Print.info('titleKey = ' + (self.cryptoKey.hex()))
 		#Print.info('cryptoCounter = ' + (self.cryptoCounter.hex()))
@@ -145,15 +202,15 @@
 		stringTableSize = self.readInt32()
 		self.readInt32() # junk data
 
 		self.seek(0x10 + fileCount * 0x18)
 		stringTable = self.read(stringTableSize)
 		stringEndOffset = stringTableSize
 		
-		headerSize = 0x10 + 0x18 * fileCount + stringTableSize
+		self._headerSize = 0x10 + 0x18 * fileCount + stringTableSize
 		self.files = []
 
 		for i in range(fileCount):
 			i = fileCount - i - 1
 			self.seek(0x10 + i * 0x18)
 
 			offset = self.readInt64()
@@ -166,15 +223,15 @@
 
 			f = Fs.factory(Path(name))
 
 			f._path = name
 			f.offset = offset
 			f.size = size
 			
-			self.files.append(self.partition(offset + headerSize, f.size, f, autoOpen = False))
+			self.files.append(self.partition(offset + self._headerSize, f.size, f, autoOpen = False))
 
 		ticket = None
 
 
 		try:
 			ticket = self.ticket()
 			ticket.open(None, None)
```

### Comparing `nsz-4.2.1/nsz/Fs/Rom.py` & `nsz-4.3.0/nsz/Fs/Rom.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Ticket.py` & `nsz-4.3.0/nsz/Fs/Ticket.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,18 +204,21 @@
 		titleKey = format(self.getTitleKeyBlock(), 'X').zfill(32)
 		masterKeyRevision = self.getMasterKeyRevision()
 
 		Print.info('\n%sTicket\n' % (tabs))
 		super(Ticket, self).printInfo(maxDepth, indent)
 		Print.info(tabs + 'signatureType = ' + str(self.signatureType))
 		Print.info(tabs + 'keyType = ' + str(self.keyType))
-		Print.info(tabs + 'masterKeyRev = ' + str(masterKeyRevision))
+		Print.info(tabs + 'masterKeyRev = ' + str(masterKeyRevision) + " (master_key_{0:02x})".format(masterKeyRevision - 1))
 		Print.info(tabs + 'ticketId = ' + str(self.ticketId))
 		Print.info(tabs + 'deviceId = ' + str(self.deviceId))
 		Print.info(tabs + 'rightsId = ' + rightsId)
 		Print.info(tabs + 'accountId = ' + str(self.accountId))
 		Print.info(tabs + 'titleId = ' + titleId)
 		Print.info(tabs + 'titleKey = ' + titleKey)
-		Print.info(tabs + 'titleKeyDec = ' + str(hx(Keys.decryptTitleKey((self.getTitleKey()), masterKeyRevision))))
+		try:
+			Print.info(tabs + 'titleKeyDec = ' + str(hx(Keys.decryptTitleKey((self.getTitleKey()), masterKeyRevision - 1))))
+		except:
+			Print.info(tabs + 'titleKeyDec = An error occurred while obtaining titleKeyDec')
```

### Comparing `nsz-4.2.1/nsz/Fs/Type.py` & `nsz-4.3.0/nsz/Fs/Type.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/Xci.py` & `nsz-4.3.0/nsz/Fs/Xci.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Fs/__init__.py` & `nsz-4.3.0/nsz/Fs/__init__.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/Header.py` & `nsz-4.3.0/nsz/Header.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/IndependentNczDecompressor.py` & `nsz-4.3.0/nsz/IndependentNczDecompressor.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/NszDecompressor.py` & `nsz-4.3.0/nsz/NszDecompressor.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from nsz.PathTools import *
 from nsz import Header, BlockDecompressorReader, FileExistingChecks
 import enlighten
 
 class VerificationException(Exception):
 	pass
 
-def decompress(filePath, outputDir, statusReportInfo, pleaseNoPrint = None):
+def decompress(filePath, outputDir, removePadding, statusReportInfo, pleaseNoPrint = None):
 	if isNspNsz(filePath):
-		__decompressNsz(filePath, outputDir, True, False, statusReportInfo, pleaseNoPrint)
+		__decompressNsz(filePath, outputDir, removePadding, True, False, False, statusReportInfo, None, pleaseNoPrint)
 	elif isXciXcz(filePath):
-		__decompressXcz(filePath, outputDir, True, False, statusReportInfo, pleaseNoPrint)
+		__decompressXcz(filePath, outputDir, removePadding, True, False, False, statusReportInfo, None, pleaseNoPrint)
 	elif isCompressedGameFile(filePath):
 		filePathNca = changeExtension(filePath, '.nca')
 		outPath = filePathNca if outputDir == None else str(Path(outputDir).joinpath(Path(filePathNca).name))
 		Print.info('Decompressing %s -> %s' % (filePath, outPath), pleaseNoPrint)
 		try:
 			inFile = factory(filePath)
 			inFile.open(str(filePath), 'rb')
@@ -37,31 +37,25 @@
 				Path(outPath).unlink()
 		finally:
 			inFile.close()
 	else:
 		raise NotImplementedError("Can't decompress {0} as that file format isn't implemented!".format(filePath))
 
 
-def verify(filePath, raiseVerificationException, statusReportInfo, pleaseNoPrint):
+def verify(filePath, removePadding, raiseVerificationException, raisePfs0Exception, originalFilePath, statusReportInfo, pleaseNoPrint):
 	if isNspNsz(filePath):
-		__decompressNsz(filePath, None, False, raiseVerificationException, statusReportInfo, pleaseNoPrint)
+		__decompressNsz(filePath, None, removePadding, False, raiseVerificationException, raisePfs0Exception, originalFilePath, statusReportInfo, pleaseNoPrint)
 	elif isXciXcz(filePath):
-		__decompressXcz(filePath, None, False, raiseVerificationException, statusReportInfo, pleaseNoPrint)
+		__decompressXcz(filePath, None, removePadding, False, raiseVerificationException, raisePfs0Exception, originalFilePath, statusReportInfo, pleaseNoPrint)
 
 
-def __decompressContainer(readContainer, writeContainer, fileHashes, write, raiseVerificationException, statusReportInfo, pleaseNoPrint):
+def __decompressContainer(readContainer, writeContainer, fileHashes, write, raiseVerificationException, raisePfs0Exception, statusReportInfo, pleaseNoPrint):
 	for nspf in readContainer:
 		CHUNK_SZ = 0x100000
 		f = None
-		if isinstance(nspf, Nca.Nca) and nspf.header.contentType == Type.Content.DATA:
-			Print.info('[SKIPPED]    Delta fragment', pleaseNoPrint)
-			continue
-		if nspf._path.endswith('.cnmt.xml'):
-			Print.info('[SKIPPED]    Content meta {0}'.format(nspf._path), pleaseNoPrint)
-			continue
 		if not nspf._path.endswith('.ncz'):
 			verifyFile = nspf._path.endswith('.nca') and not nspf._path.endswith('.cnmt.nca')
 			if write:
 				f = writeContainer.add(nspf._path, nspf.size, pleaseNoPrint)
 			hash = sha256()
 			nspf.seek(0)
 			while not nspf.eof():
@@ -189,46 +183,68 @@
 	if f != None:
 		end = f.tell()
 		written = (end - start)
 		return (written, hexHash)
 	return (0, hexHash)
 
 
-def __decompressNsz(filePath, outputDir, write, raiseVerificationException, statusReportInfo, pleaseNoPrint):
+def __decompressNsz(filePath, outputDir, removePadding, write, raiseVerificationException, raisePfs0Exception, originalFilePath, statusReportInfo, pleaseNoPrint):
 	fileHashes = FileExistingChecks.ExtractHashes(filePath)
 	container = factory(filePath)
 	container.open(str(filePath), 'rb')
 	
 	try:
 		if write:
 			filePathNsp = changeExtension(filePath, '.nsp')
 			outPath = filePathNsp if outputDir == None else str(Path(outputDir).joinpath(Path(filePathNsp).name))
 			Print.info('Decompressing %s -> %s' % (filePath, outPath), pleaseNoPrint)
-			with Pfs0.Pfs0Stream(outPath) as nsp:
-				__decompressContainer(container, nsp, fileHashes, write, raiseVerificationException, statusReportInfo, pleaseNoPrint)
+			with Pfs0.Pfs0Stream(container.getHeaderSize() if removePadding else container.getFirstFileOffset(), outPath) as nsp:
+				__decompressContainer(container, nsp, fileHashes, True, raiseVerificationException, raisePfs0Exception, statusReportInfo, pleaseNoPrint)
 		else:
-			__decompressContainer(container, None, fileHashes, write, raiseVerificationException, statusReportInfo, pleaseNoPrint)
+			with Pfs0.Pfs0VerifyStream(container.getHeaderSize() if removePadding else container.getFirstFileOffset()) as nsp:
+				__decompressContainer(container, nsp, fileHashes, True, raiseVerificationException, raisePfs0Exception, statusReportInfo, pleaseNoPrint)
+				Print.info("[PFS0 HEAD]  " + nsp.getHeaderHash())
+				Print.info("[PFS0 DATA]  " + nsp.getHash())
+				if originalFilePath != None: 
+					originalContainer = factory(originalFilePath)
+					originalContainer.open(str(originalFilePath), 'rb')
+					with Pfs0.Pfs0VerifyStream(originalContainer.getHeaderSize() if removePadding else originalContainer.getFirstFileOffset()) as originalNsp:
+						__decompressContainer(originalContainer, originalNsp, fileHashes, True, raiseVerificationException, raisePfs0Exception, statusReportInfo, pleaseNoPrint)
+						Print.info("[PFS0 HEAD]  " + originalNsp.getHeaderHash())
+						Print.info("[PFS0 DATA]  " + originalNsp.getHash())
+						if nsp.getHeaderHash() == originalNsp.getHeaderHash():
+							Print.info("[VERIFIED]   PFS0 Header")
+						else:
+							Print.info("[MISSMATCH]  PFS0 Header") 
+							if raisePfs0Exception:
+								raise VerificationException("Verification detected PFS0 hader hash mismatch!")
+						if nsp.getHash() == originalNsp.getHash():
+							Print.info("[VERIFIED]   PFS0 Data")
+						else:
+							Print.info("[MISSMATCH]  PFS0 Data")
+							if raisePfs0Exception:
+								raise VerificationException("Verification detected PFS0 data hash mismatch!")
 	except BaseException:
 		raise
 	finally:
 		container.close()
 
 
-def __decompressXcz(filePath, outputDir, write, raiseVerificationException, statusReportInfo, pleaseNoPrint):
+def __decompressXcz(filePath, outputDir, removePadding, write, raiseVerificationException, raisePfs0Exception, originalFilePath, statusReportInfo, pleaseNoPrint):
 	fileHashes = FileExistingChecks.ExtractHashes(filePath)
 	container = factory(filePath)
 	container.open(str(filePath), 'rb')
 	secureIn = container.hfs0['secure']
 	
 	if write:
 		filePathXci = changeExtension(filePath, '.xci')
 		outPath = filePathXci if outputDir == None else str(Path(outputDir).joinpath(Path(filePathXci).name))
 		Print.info('Decompressing %s -> %s' % (filePath, outPath), pleaseNoPrint)
 		with Xci.XciStream(outPath, originalXciPath = filePath) as xci: # need filepath to copy XCI container settings
 			with Hfs0.Hfs0Stream(xci.hfs0.add('secure', 0, pleaseNoPrint), xci.f.tell()) as secureOut:
-				__decompressContainer(secureIn, secureOut, fileHashes, write, raiseVerificationException, statusReportInfo, pleaseNoPrint)
+				__decompressContainer(secureIn, secureOut, fileHashes, write, raiseVerificationException, raisePfs0Exception, statusReportInfo, pleaseNoPrint)
 				xci.hfs0.resize('secure', secureOut.actualSize)
 	else:
-		__decompressContainer(secureIn, None, fileHashes, write, raiseVerificationException, statusReportInfo, pleaseNoPrint)
+		__decompressContainer(secureIn, None, fileHashes, write, raiseVerificationException, raisePfs0Exception, statusReportInfo, pleaseNoPrint)
 
 	container.close()
```

### Comparing `nsz-4.2.1/nsz/ParseArguments.py` & `nsz-4.3.0/nsz/ParseArguments.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 		parser.add_argument('-C', action="store_true", help='Compress NSP/XCI')
 		parser.add_argument('-D', action="store_true", help='Decompress NSZ/XCZ/NCZ')
 		parser.add_argument('-l', '--level', type=int, default=18, help='Compression Level: Trade-off between compression speed and compression ratio. Default: 18, Max: 22')
 		parser.add_argument('-L', '--long', action="store_true", default=False, help='Enables zStandard long distance mode for even better compression')
 		parser.add_argument('-B', '--block', action="store_true", default=False, help="Use block compression option. This mode allows highly multi-threaded compression/decompression with random read access allowing compressed games to be played without decompression in the future however this comes with a slightly lower compression ratio cost. This is the default option for XCZ.")
 		parser.add_argument('-S', '--solid', action="store_true", default=False, help="Use solid compression option. Slightly higher compression ratio but won't allow for random read access. File compressed this way will never be mountable (have to be installed or decompressed first to run). This is the default option for NSZ.")
 		parser.add_argument('-s', '--bs', type=int, default=20, help='Block Size for random read access 2^x while x between 14 and 32. Default: 20 => 1 MB')
-		parser.add_argument('-V', '--verify', action="store_true", default=False, help='Verifies files after compression raising an unhandled exception on hash mismatch and verify existing NSP and NSZ files when given as parameter')
+		parser.add_argument('-V', '--verify', action="store_true", default=False, help='Verifies files after compression raising an unhandled exception on hash mismatch and verify existing NSP and NSZ files when given as parameter. Requires --keep-delta when used during compression.')
+		parser.add_argument('-Q', '--quick-verify', action="store_true", default=False, help='Same as --verify but skips the expensive and mostly useless PFS0 hash verification and only verifies NCA hashes. Does not require --keep-delta when used during compression.')
+		parser.add_argument('-K', '--keep-delta', action="store_true", default=False, help='Keep all useless delta fragments (NDV0) during compression so the NSP (PFS0) can be recreated bit-identical during decompression')
+		parser.add_argument('-R', '--remove-padding', action="store_true", default=False, help='Remove the padding between the PFS0 header and the first file so the NSP matches the nxdumptool/no-intro standard')
 		parser.add_argument('-p', '--parseCnmt', action="store_true", default=False, help='Extract TitleId/Version from Cnmt if this information cannot be obtained from the filename. Required for skipping/overwriting existing files and --rm-old-version to work properly if some not every file is named properly. Supported filenames: *TitleID*[vVersion]*')
 		parser.add_argument('-P', '--alwaysParseCnmt', action="store_true", default=False, help='Always extract TitleId/Version from Cnmt and never trust filenames')
 		parser.add_argument('-t', '--threads', type=int, default=-1, help='Number of threads to compress with. Numbers < 1 corresponds to the number of logical CPU cores for block compression and 3 for solid compression')
 		parser.add_argument('-m', '--multi', type=int, default=4, help='Executes multiple compression tasks in parallel. Take a look at available RAM especially if compression level is over 18.')
 		parser.add_argument('-o', '--output', nargs='?', help='Directory to save the output NSZ files')
 		parser.add_argument('-w', '--overwrite', action="store_true", default=False, help='Continues even if there already is a file with the same name or title id inside the output directory')
 		parser.add_argument('-r', '--rm-old-version', action="store_true", default=False, help='Removes older versions if found')
@@ -26,15 +29,15 @@
 		parser.add_argument('-x', '--extract', action="store_true", help='Extract a NSP/XCI/NSZ/XCZ/NSPZ')
 		parser.add_argument('--extractregex', type=str, default="", help='Regex specifying which files inside the container should be extracted. Example: "^.*\.(cert|tik)$"')
 		parser.add_argument('--titlekeys', action='store_true', default=False, help="Extracts titlekeys from your NSP/NSZ files and adds missing keys to ./titlekeys.txt and JSON files inside ./titledb/ (obtainable from https://github.com/blawar/titledb). Titlekeys can be used to unlock updates using NUT OG (OG fork obtainable from https://github.com/plato79/nut). There is currently no publicly known way of optioning NSX files. To MitM: Apply disable_ca_verification & disable_browser_ca_verification patches, use your device's nx_tls_client_cert.pfx (Password: switch, Install to OS and import for Fiddler or import into Charles/OWASP ZAP). Use it for aauth-lp1.ndas.srv.nintendo.net:443, dauth-lp1.ndas.srv.nintendo.net:443 and app-b01-lp1.npns.srv.nintendo.net:443. Try with your WiiU first as there you won't get banned if you mess up.")
 		parser.add_argument('--undupe', action='store_true', help="Deleted all duplicates (games with same ID and Version). The Files folder will get parsed in order so the later in the argument list the more likely the file is to be deleted")
 		parser.add_argument('--undupe-dryrun' , action='store_true', help="Shows what files would get deleted using --undupe")
 		parser.add_argument('--undupe-rename' , action='store_true', help="Renames files to minimal standard: [TitleId][vVersion].nsz")
 		parser.add_argument('--undupe-hardlink' , action='store_true', help="Hardlinks files to minimal standard: [TitleId][vVersion].nsz")
-		parser.add_argument('--undupe-prioritylist', type=str, default="", help='Regex specifying which dublicates delegtion should be prioritized before following the normal deletion order. Example: "^.*\.(nsp|xci)$"')
+		parser.add_argument('--undupe-prioritylist', type=str, default="", help='Regex specifying which dublicate deletion should be prioritized before following the normal deletion order. Example: "^.*\.(nsp|xci)$"')
 		parser.add_argument('--undupe-whitelist', type=str, default="", help='Regex specifying which dublicates should under no circumstances be deleted. Example: "^.*\.(nsz|xcz)$"')
 		parser.add_argument('--undupe-blacklist', type=str, default="", help='Regex specifying which files should always be deleted - even if they are not even a dublicate! Be careful! Example: "^.*\.(nsp|xci)$"')
 		parser.add_argument('--undupe-old-versions',action="store_true", default=False, help='Removes every old version as long there is a newer one of the same titleID.')
 		parser.add_argument('-c', '--create', help='Inverse of --extract. Repacks files/folders to an NSP. Example: --create out.nsp .\in')
 	
 		args = parser.parse_args()
 		return args
```

### Comparing `nsz-4.2.1/nsz/PathTools.py` & `nsz-4.3.0/nsz/PathTools.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/SolidCompressor.py` & `nsz-4.3.0/nsz/SolidCompressor.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,26 @@
 from zstandard import FLUSH_FRAME, COMPRESSOBJ_FLUSH_FINISH, ZstdCompressionParameters, ZstdCompressor
 from nsz.PathTools import *
 
 UNCOMPRESSABLE_HEADER_SIZE = 0x4000
 CHUNK_SZ = 0x1000000
 
 
-def solidCompress(filePath, compressionLevel, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint):
+def solidCompress(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint):
 	if filePath.suffix == '.nsp':
-		return solidCompressNsp(filePath, compressionLevel, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint)
+		return solidCompressNsp(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint)
 	elif filePath.suffix == '.xci':
-		return solidCompressXci(filePath, compressionLevel, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint)
+		return solidCompressXci(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint)
 		
-def processContainer(readContainer, writeContainer, compressionLevel, useLongDistanceMode, threads, statusReport, id, pleaseNoPrint):
+def processContainer(readContainer, writeContainer, compressionLevel, keepDelta, useLongDistanceMode, threads, statusReport, id, pleaseNoPrint):
 	for nspf in readContainer:
-		if isinstance(nspf, Nca.Nca) and nspf.header.contentType == Type.Content.DATA:
-			Print.info('[SKIPPED]    Delta fragment {0}'.format(nspf._path), pleaseNoPrint)
-			continue
-		if nspf._path.endswith('.cnmt.xml'):
-			Print.info('[SKIPPED]    Content meta {0}'.format(nspf._path), pleaseNoPrint)
-			continue
+		if not keepDelta:
+			if isinstance(nspf, Nca.Nca) and nspf.header.contentType == Type.Content.DATA:
+				Print.info('[SKIPPED]    Delta fragment {0}'.format(nspf._path), pleaseNoPrint)
+				continue
 		if isinstance(nspf, Nca.Nca) and (nspf.header.contentType == Type.Content.PROGRAM or nspf.header.contentType == Type.Content.PUBLICDATA) and nspf.size > UNCOMPRESSABLE_HEADER_SIZE:
 			if isNcaPacked(nspf):
 				
 				offsetFirstSection = sortedFs(nspf)[0].offset
 				newFileName = nspf._path[0:-1] + 'z'
 		
 				with writeContainer.add(newFileName, nspf.size, pleaseNoPrint) as f:
@@ -118,47 +116,47 @@
 		with writeContainer.add(nspf._path, nspf.size, pleaseNoPrint) as f:
 			nspf.seek(0)
 			while not nspf.eof():
 				buffer = nspf.read(CHUNK_SZ)
 				f.write(buffer)
 
 
-def solidCompressNsp(filePath, compressionLevel, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint):
+def solidCompressNsp(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint):
 	filePath = filePath.resolve()
 	container = factory(filePath)
 	container.open(str(filePath), 'rb')
 	nszPath = outputDir.joinpath(filePath.stem + '.nsz')
 
 	Print.info(f'Solid compressing (level {compressionLevel}{" ldm" if useLongDistanceMode else ""}) {filePath} -> {nszPath}', pleaseNoPrint)
 	
 	try:
-		with Pfs0.Pfs0Stream(str(nszPath)) as nsp:
-			processContainer(container, nsp, compressionLevel, useLongDistanceMode,threads, statusReport, id, pleaseNoPrint)
+		with Pfs0.Pfs0Stream(container.getHeaderSize() if removePadding else container.getFirstFileOffset(), str(nszPath)) as nsp:
+			processContainer(container, nsp, compressionLevel, keepDelta, useLongDistanceMode, threads, statusReport, id, pleaseNoPrint)
 	except BaseException as ex:
 		if not ex is KeyboardInterrupt:
 			Print.error(format_exc())
 		if nszPath.is_file():
 			nszPath.unlink()
 
 	container.close()
 	return nszPath
 	
-def solidCompressXci(filePath, compressionLevel, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint):
+def solidCompressXci(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, outputDir, threads, statusReport, id, pleaseNoPrint):
 	filePath = filePath.resolve()
 	container = factory(filePath)
 	container.open(str(filePath), 'rb')
 	secureIn = container.hfs0['secure']
 	xczPath = outputDir.joinpath(filePath.stem + '.xcz')
 
 	Print.info(f'Solid compressing (level {compressionLevel}{" ldm" if useLongDistanceMode else ""}) {filePath} -> {xczPath}', pleaseNoPrint)
 	
 	try:
 		with Xci.XciStream(str(xczPath), originalXciPath = filePath) as xci: # need filepath to copy XCI container settings
 			with Hfs0.Hfs0Stream(xci.hfs0.add('secure', 0, pleaseNoPrint), xci.f.tell()) as secureOut:
-				processContainer(secureIn, secureOut, compressionLevel, useLongDistanceMode, threads, statusReport, id, pleaseNoPrint)
+				processContainer(secureIn, secureOut, compressionLevel, keepDelta, useLongDistanceMode, threads, statusReport, id, pleaseNoPrint)
 			
 			xci.hfs0.resize('secure', secureOut.actualSize)
 	except BaseException as ex:
 		if not ex is KeyboardInterrupt:
 			Print.error(format_exc())
 		if xczPath.is_file():
 			xczPath.unlink()
```

### Comparing `nsz-4.2.1/nsz/__init__.py` & `nsz-4.3.0/nsz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 	while True:
 		readyForWork.increment()
 		item = in_queue.get()
 		readyForWork.decrement()
 		if pleaseKillYourself.value() > 0:
 			break
 		try:
-			filePath, compressionLevel, useLongDistanceMode, outputDir, threadsToUse, verifyArg = item
-			outFile = solidCompress(filePath, compressionLevel, useLongDistanceMode, outputDir, threadsToUse, statusReport, id, pleaseNoPrint)
+			filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, outputDir, threadsToUse, verifyArg, quickVerify = item
+			outFile = solidCompress(filePath, compressionLevel, keepDelta, removePadding, useLongDistanceMode, outputDir, threadsToUse, statusReport, id, pleaseNoPrint)
 			if verifyArg:
 				Print.info("[VERIFY NSZ] {0}".format(outFile))
 				try:
-					verify(outFile, True, [statusReport, id], pleaseNoPrint)
+					verify(outFile, removePadding, True, keepDelta, None if quickVerify else filePath, [statusReport, id], pleaseNoPrint)
 				except VerificationException:
 					Print.error("[BAD VERIFY] {0}".format(outFile))
 					Print.error("[DELETE NSZ] {0}".format(outFile))
 					remove(outFile)
 		except KeyboardInterrupt:
 			Print.info('Keyboard exception')
 		except BaseException as e:
@@ -49,29 +49,29 @@
 			raise
 
 def compress(filePath, outputDir, args, work, amountOfTastkQueued):
 	compressionLevel = 18 if args.level is None else args.level
 	
 	if filePath.suffix == ".xci" and not args.solid or args.block:
 		threadsToUseForBlockCompression = args.threads if args.threads > 0 else cpu_count()
-		outFile = blockCompress(filePath, compressionLevel, args.long, args.bs, outputDir, threadsToUseForBlockCompression)
+		outFile = blockCompress(filePath, compressionLevel, args.keep_delta, args.remove_padding, args.long, args.bs, outputDir, threadsToUseForBlockCompression)
 		if args.verify:
 			Print.info("[VERIFY NSZ] {0}".format(outFile))
-			verify(outFile, True)
+			verify(outFile, args.remove_padding, True, args.keep_delta, None if args.quick_verify else filePath)
 	else:
 		threadsToUseForSolidCompression = args.threads if args.threads > 0 else 3
-		work.put([filePath, compressionLevel, args.long, outputDir, threadsToUseForSolidCompression, args.verify])
+		work.put([filePath, compressionLevel, args.keep_delta, args.remove_padding, args.long, outputDir, threadsToUseForSolidCompression, args.verify, args.quick_verify])
 		amountOfTastkQueued.increment()
 
 
-def decompress(filePath, outputDir, statusReportInfo = None):
-	NszDecompress(filePath, outputDir, statusReportInfo)
+def decompress(filePath, outputDir, removePadding, statusReportInfo = None):
+	NszDecompress(filePath, outputDir, removePadding, statusReportInfo)
 
-def verify(filePath, raiseVerificationException, statusReportInfo = None, pleaseNoPrint = None):
-	NszVerify(filePath, raiseVerificationException, statusReportInfo, pleaseNoPrint)
+def verify(filePath, removePadding, raiseVerificationException, raisePfs0Exception, originalFilePath = None, statusReportInfo = None, pleaseNoPrint = None):
+	NszVerify(filePath, removePadding, raiseVerificationException, raisePfs0Exception, originalFilePath, statusReportInfo, pleaseNoPrint)
 
 err = []
 
 def main():
 	global err
 	try:
 		if len(argv) > 1:
@@ -82,26 +82,29 @@
 			except ImportError:
 				Print.error("Failed to import the GUI - is it installed?")
 				return
 			args = GUI().run()
 			if args == None:
 				Print.info("Done!")
 				return
+
+		if args.quick_verify:
+			args.verify = True
 		
 		if args.output:
 			argOutFolderToPharse = args.output
 			if not argOutFolderToPharse.endswith('/') and not argOutFolderToPharse.endswith('\\'):
 				argOutFolderToPharse += "/"
 			if not Path(argOutFolderToPharse).is_dir():
 				Print.error('Error: Output directory "{0}" does not exist!'.format(args.output))
 				return
 		argOutFolder = Path(argOutFolderToPharse).resolve() if args.output else None
 		
 		Print.info('')
-		Print.info('             NSZ v4.2   ,;:;;,')
+		Print.info('             NSZ v4.3   ,;:;;,')
 		Print.info('                       ;;;;;')
 		Print.info('               .=\',    ;:;;:,')
 		Print.info('              /_\', "=. \';:;:;')
 		Print.info('              @=:__,  \,;:;:\'')
 		Print.info('                _(\.=  ;:;;\'')
 		Print.info('               `"_(  _/="`')
 		Print.info('                `"\'')
@@ -144,14 +147,17 @@
 		if args.create:
 			Print.info('Creating "{0}"'.format(args.create))
 			nsp = Nsp.Nsp(None, None)
 			nsp.path = args.create
 			nsp.pack(args.file)
 
 		if args.C:
+			if args.verify and not args.quick_verify and not args.keep_delta:
+				Print.info("Warning: --verify requires --keep-delta when used during compression or it will detect removed NDV0 fragments as errors. For compatibility reasons --quick-verify will be automatically used instead to match the command line argument behavior prior to NSZ v4.3.0.")
+				args.quick_verify = True
 			sourceFileToDelete = []
 			for f_str in args.file:
 				for filePath in expandFiles(Path(f_str)):
 					if not isUncompressedGame(filePath):
 						continue
 					try:
 						outFolder = argOutFolder if argOutFolder else filePath.parent.absolute()
@@ -238,15 +244,15 @@
 								continue
 						elif filePath.suffix == '.ncz':
 							outFile = Path(changeExtension(outFolder.joinpath(filePath.name), ".nca"))
 							if not args.overwrite and outFile.is_file():
 								Print.info('{0} with the same file name already exists in the output directory.\n'\
 								'If you want to overwrite it use the -w parameter!'.format(outFile.name))
 								continue
-						decompress(filePath, outFolder)
+						decompress(filePath, outFolder, args.remove_padding)
 						if args.rm_source:
 							delete_source_file(filePath, outFolder)
 					except KeyboardInterrupt:
 						raise
 					except BaseException as e:
 						Print.error('Error while decompressing file: {0}'.format(filePath))
 						err.append({"filename":filePath, "error":format_exc()})
@@ -264,15 +270,15 @@
 
 		if args.verify and not args.C and not args.D:
 			for f_str in args.file:
 				for filePath in expandFiles(Path(f_str)):
 					try:
 						if isGame(filePath):
 							Print.info("[VERIFY {0}] {1}".format(getExtensionName(filePath), filePath.name))
-							verify(filePath, True)
+							verify(filePath, args.remove_padding, True, True)
 					except KeyboardInterrupt:
 						raise
 					except BaseException as e:
 						Print.error('Error while verifying file: {0}'.format(filePath))
 						err.append({"filename":filePath,"error":format_exc()})
 						print_exc()
```

### Comparing `nsz-4.2.1/nsz/gui/AboutDialog.py` & `nsz-4.3.0/nsz/gui/AboutDialog.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/DraggableScrollbar.py` & `nsz-4.3.0/nsz/gui/DraggableScrollbar.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/FileDialogs.py` & `nsz-4.3.0/nsz/gui/FileDialogs.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/GameList.py` & `nsz-4.3.0/nsz/gui/GameList.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/Hyperlink.py` & `nsz-4.3.0/nsz/gui/Hyperlink.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/KivyOnTop.py` & `nsz-4.3.0/nsz/gui/KivyOnTop.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/NSZ_GUI.py` & `nsz-4.3.0/nsz/gui/NSZ_GUI.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		#to take effect." caused by checking if booth variables are set after setting
 		#one of them without offering any way of setting booth at the same time
 		Logger.setLevel(logging.ERROR)
 		Window.minimum_width = 800
 		Window.minimum_height = 600
 		Logger.setLevel(realLevl)
 		Builder.load_file(getGuiPath('layout/GUI.kv'))
-		self.title = 'NSZ GUI 4.2'
+		self.title = 'NSZ GUI 4.3'
 		self.icon = getGuiPath('nsZip.png')
 		root = FloatLayout()
 		with open(getGuiPath('shaders/plasma.shader')) as stream:
 			plasma_shader = stream.read()
 			root.add_widget(ShaderWidget(fs=plasma_shader))
 		gameList = GameList()
 		self.rootWidget = RootWidget(gameList)
@@ -60,19 +60,21 @@
 	def build_config(self, config):
 		config.setdefaults(
 		'Settings', {
 			'level': '[Lv. 18] Great (default)',
 			'block': 0,
 			'solid': 0,
 			'bs': "1 MB (default)",
-			'verify': 1,
+			'verify_options': "Quick (NCA hashes)",
+			'keepDelta': 0,
 		})
 		config.setdefaults('Advanced', {
 			'threads': -1,
 			'multi': 4,
+			'removePadding': 0,
 			'ldm': 0,
 			'parseCnmt': 0,
 			'overwrite': 0,
 			'rm_old_version': 0,
 			'rm_source': 0,
 		})
 		config.setdefaults('Tools', {
@@ -136,20 +138,27 @@
 		self.create = True if rootWidget.create is True else None
 		self.level = level_scrolloptions.get(config.get('Settings', 'level'), 18)
 		self.block = True if int(config.get('Settings', 'block')) == 1 else None
 		self.solid = True if int(config.get('Settings', 'solid')) == 1 else None
 		self.bs = bs_scrolloptions.get(config.get('Settings', 'bs'), 20)
 		if rootWidget.verify is True \
 		or ((rootWidget.C is True or rootWidget.D is True) \
-		and int(config.get('Settings', 'verify')) == 1):
+		and config.get('Settings', 'verify_options') == "Full (NCA & PFS0 hashes)"):
 			self.verify = True
 		else:
 			self.verify = None
+		if ((rootWidget.C is True or rootWidget.D is True) \
+		and config.get('Settings', 'verify_options') == "Quick (NCA hashes)"):
+			self.quick_verify = True
+		else:
+			self.quick_verify = None
+		self.keep_delta = True if int(config.get('Settings', 'keepDelta')) == 1 else False
 		self.threads = int(config.get('Advanced', 'threads'))
 		self.multi = int(config.get('Advanced', 'multi'))
+		self.remove_padding = True if int(config.get('Advanced', 'removePadding')) == 1 else False
 		self.long = True if int(config.get('Advanced', 'ldm')) == 1 else False
 		self.parseCnmt = True if int(config.get('Advanced', 'parseCnmt')) == 1 else None
 		self.overwrite = True if int(config.get('Advanced', 'overwrite')) == 1 else None
 		self.rm_old_version = True if int(config.get('Advanced', 'rm_old_version')) == 1 else None
 		self.rm_source = True if int(config.get('Advanced', 'rm_source')) == 1 else None
 		self.depth = int(config.get('Tools', 'depth'))
 		self.extractregex = str(config.get('Tools', 'extractregex'))
```

### Comparing `nsz-4.2.1/nsz/gui/RootWidget.py` & `nsz-4.3.0/nsz/gui/RootWidget.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/SettingScrollOptions.py` & `nsz-4.3.0/nsz/gui/SettingScrollOptions.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/ShaderWidget.py` & `nsz-4.3.0/nsz/gui/ShaderWidget.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/fonts/MPLUS1p-Medium.ttf` & `nsz-4.3.0/nsz/gui/fonts/MPLUS1p-Medium.ttf`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/fonts/OFL.txt` & `nsz-4.3.0/nsz/gui/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/json/settings_advanced.json` & `nsz-4.3.0/nsz/gui/json/settings_advanced.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {'insert': "[(2, OrderedDict([('type', 'bool'), ('title', 'Remove Padding'), ('desc', 'Remove the "*

 * *           'padding between the PFS0 header and the first file so the NSP matches the '*

 * *           "nxdumptool/no-intro standard'), ('section', 'Advanced'), ('key', 'removePadding')]))]"}*

```diff
@@ -10,14 +10,21 @@
         "desc": "Executes multiple compression tasks in parallel. Take a look at available RAM especially if compression level is over 18.",
         "key": "multi",
         "section": "Advanced",
         "title": "Multitasking",
         "type": "numeric"
     },
     {
+        "desc": "Remove the padding between the PFS0 header and the first file so the NSP matches the nxdumptool/no-intro standard",
+        "key": "removePadding",
+        "section": "Advanced",
+        "title": "Remove Padding",
+        "type": "bool"
+    },
+    {
         "desc": "Enables zStandard long distance mode for even better compression",
         "key": "ldm",
         "section": "Advanced",
         "title": "Long Distance Mode",
         "type": "bool"
     },
     {
```

### Comparing `nsz-4.2.1/nsz/gui/json/settings_basic.json` & `nsz-4.3.0/nsz/gui/json/settings_basic.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7833333333333333%*

 * *Differences: {'5': "{'title': 'Keep Delta Fragments', 'desc': 'Keep all useless delta fragments (NDV0) during "*

 * *      "compression so the NSP (PFS0) can be recreated bit-identical during decompression', 'key': "*

 * *      "'keepDelta'}",*

 * * 'insert': "[(4, OrderedDict([('type', 'scrolloptions'), ('title', 'Verify'), ('desc', 'Verifies "*

 * *           'files after compression raising an unhandled exception on hash mismatch and verify '*

 * *           'existing NSP and NSZ files when given as parameter. Quick skips the expensive and ' […]*

```diff
@@ -43,14 +43,26 @@
             "16 MB"
         ],
         "section": "Settings",
         "title": "Block Size",
         "type": "scrolloptions"
     },
     {
-        "desc": "Verifies files after compression raising an unhandled exception on hash mismatch and verify existing NSP and NSZ files when given as parameter",
-        "key": "verify",
+        "desc": "Verifies files after compression raising an unhandled exception on hash mismatch and verify existing NSP and NSZ files when given as parameter. Quick skips the expensive and mostly useless PFS0 hash verification and only verifies NCA hashes. Full requires --keep-delta when used for compression.",
+        "key": "verify_options",
+        "options": [
+            "None",
+            "Quick (NCA hashes)",
+            "Full (NCA & PFS0 hashes)"
+        ],
         "section": "Settings",
         "title": "Verify",
+        "type": "scrolloptions"
+    },
+    {
+        "desc": "Keep all useless delta fragments (NDV0) during compression so the NSP (PFS0) can be recreated bit-identical during decompression",
+        "key": "keepDelta",
+        "section": "Settings",
+        "title": "Keep Delta Fragments",
         "type": "bool"
     }
 ]
```

### Comparing `nsz-4.2.1/nsz/gui/json/settings_tools.json` & `nsz-4.3.0/nsz/gui/json/settings_tools.json`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/layout/AboutDialog.kv` & `nsz-4.3.0/nsz/gui/layout/AboutDialog.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/layout/GameList.kv` & `nsz-4.3.0/nsz/gui/layout/GameList.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/layout/OpenFileDialog.kv` & `nsz-4.3.0/nsz/gui/layout/OpenFileDialog.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/layout/RootWidget.kv` & `nsz-4.3.0/nsz/gui/layout/RootWidget.kv`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/shaders/plasma.shader` & `nsz-4.3.0/nsz/gui/shaders/plasma.shader`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/gui/txt/license.txt` & `nsz-4.3.0/nsz/gui/txt/license.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
 Copyright (c) 2019 Nico Bosshard and Blake Warner
-Thanks to our contributors: nicoboss, blawar, plato79, eXhumer, Taorni, teknoraver, anthonyu, gabest11, KWottrich, maki-chan, thatch, 2weak2live, pR0Ps, 16BitWonder
+Thanks to our contributors: nicoboss, blawar, plato79, eXhumer, Taorni, teknoraver, anthonyu, gabest11, KWottrich, maki-chan, thatch, 2weak2live, pR0Ps, 16BitWonder, drizzt
 
 Some code inside NSZ originates from NUT. Blake Warner, as the author of NUT,
 permits to license all NUT code used in NSZ to the following MIT license.
 This permission isn't bound to this project so that NUT code inside NSZ can
 be used and sublicensed like any other MIT licensed code.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nsz-4.2.1/nsz/nut/Hex.py` & `nsz-4.3.0/nsz/nut/Hex.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/nut/Keys.py` & `nsz-4.3.0/nsz/nut/Keys.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,16 @@
 	'master_key_07': 1146095808,
 	'master_key_08': 1605958034,
 	'master_key_09': 3456782962,
 	'master_key_0a': 2012895168,
 	'master_key_0b': 3813624150,
 	'master_key_0c': 3881579466,
 	'master_key_0d': 723654444,
-	'master_key_0e': 2690905064
+	'master_key_0e': 2690905064,
+	'master_key_0f': 4082108335
 }
 
 def getMasterKeyIndex(i):
 	if i > 0:
 		return i-1
 	else:
 		return 0
@@ -96,20 +97,22 @@
 	kek = generateKek(getKey('key_area_key_application_source'), getMasterKey(keyGeneration), aes_kek_generation_source, aes_key_generation_source)
 
 	crypto = aes128.AESECB(kek)
 	return crypto.decrypt(wrappedKey)
 
 def getKey(key):
 	if key not in keys:
-		raise IOError('{0} missing from {1}'.format(key, loadedKeysFile))
+		Print.error('{0} missing from {1}! This will lead to corrupted output.'.format(key, loadedKeysFile))
+		raise IOError('{0} missing from {1}! This will lead to corrupted output.'.format(key, loadedKeysFile))
 	foundKey = uhx(keys[key])
 	foundKeyChecksum = crc32(foundKey)
 	if key in crc32_checksum:
 		if crc32_checksum[key] != foundKeyChecksum:
-			raise IOError('{0} from {1} is invalid (crc32 missmatch)'.format(key, loadedKeysFile))
+			Print.error('{0} from {1} is invalid (crc32 missmatch)! This will lead to corrupted output.'.format(key, loadedKeysFile))
+			raise IOError('{0} from {1} is invalid (crc32 missmatch)! This will lead to corrupted output.'.format(key, loadedKeysFile))
 	elif current_process().name == 'MainProcess':
 		Print.info('Unconfirmed: crc32({0}) = {1}'.format(key, foundKeyChecksum))
 	return foundKey
 
 def getMasterKey(masterKeyIndex):
 	return getKey('master_key_{0:02x}'.format(masterKeyIndex))
```

### Comparing `nsz-4.2.1/nsz/nut/Print.py` & `nsz-4.3.0/nsz/nut/Print.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/nut/Titles.py` & `nsz-4.3.0/nsz/nut/Titles.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/nut/aes128.py` & `nsz-4.3.0/nsz/nut/aes128.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz/undupe.py` & `nsz-4.3.0/nsz/undupe.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/nsz.egg-info/SOURCES.txt` & `nsz-4.3.0/nsz.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 nsz.py
 setup.py
 nsz/BlockCompressor.py
 nsz/BlockDecompressorReader.py
 nsz/ExtractTitlekeys.py
 nsz/FileExistingChecks.py
```

### Comparing `nsz-4.2.1/nsz.py` & `nsz-4.3.0/nsz.py`

 * *Files identical despite different names*

### Comparing `nsz-4.2.1/setup.py` & `nsz-4.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='nsz',
-	version='4.2.1',
+	version='4.3.0',
 	script="nsz.py",
 	author="Nico Bosshard",
 	author_email="nico@bosshome.ch",
 	maintainer="Nico Bosshard",
 	maintainer_email="nico@bosshome.ch",
 	description="NSZ - Homebrew compatible NSP/XCI compressor/decompressor",
 	long_description=long_description,
```

