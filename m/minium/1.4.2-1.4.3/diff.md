# Comparing `tmp/minium-1.4.2.tar.gz` & `tmp/minium-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minium-1.4.2.tar", last modified: Fri Jun 30 02:36:03 2023, max compression
+gzip compressed data, was "dist/minium-1.4.3.tar", last modified: Thu Jul  6 02:50:01 2023, max compression
```

## Comparing `minium-1.4.2.tar` & `minium-1.4.3.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.707526 minium-1.4.2/
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-30 02:36:03.707526 minium-1.4.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.659526 minium-1.4.2/minium/
--rw-r--r--   0 root         (0) root         (0)      948 2023-04-27 02:49:43.000000 minium-1.4.2/minium/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/
--rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18577 2023-06-28 02:27:06.000000 minium-1.4.2/minium/framework/assertbase.py
--rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.4.2/minium/framework/casedump.py
--rw-r--r--   0 root         (0) root         (0)     7714 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/caseinspect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/css/
--rw-r--r--   0 root         (0) root         (0)      437 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/css/app.87891bf0.css
--rw-r--r--   0 root         (0) root         (0)   240799 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/css/chunk-vendors.52eeca6f.css
--rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/dist/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/fonts/
--rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/dist/fonts/element-icons.535877f5.woff
--rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/dist/fonts/element-icons.732389de.ttf
--rw-r--r--   0 root         (0) root         (0)      847 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.667526 minium-1.4.2/minium/framework/dist/js/
--rw-r--r--   0 root         (0) root         (0)    17537 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/js/app.544bedf4.js
--rw-r--r--   0 root         (0) root         (0)  1346000 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/dist/js/chunk-vendors.22ed339a.js
--rw-r--r--   0 root         (0) root         (0)     3447 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/errorReport.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.671526 minium-1.4.2/minium/framework/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.671526 minium-1.4.2/minium/framework/libs/tgit/
--rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/libs/tgit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/libs/tgit/auth.py
--rw-r--r--   0 root         (0) root         (0)    97167 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/libs/tgit/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.675526 minium-1.4.2/minium/framework/libs/unittest/
--rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.4.2/minium/framework/libs/unittest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22297 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/libs/unittest/case.py
--rw-r--r--   0 root         (0) root         (0)     5629 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/libs/unittest/suite.py
--rw-r--r--   0 root         (0) root         (0)    20015 2023-06-29 15:00:02.000000 minium-1.4.2/minium/framework/loader.py
--rw-r--r--   0 root         (0) root         (0)     9938 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/logcolor.py
--rw-r--r--   0 root         (0) root         (0)     7244 2023-04-27 02:49:43.000000 minium-1.4.2/minium/framework/miniconfig.py
--rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/miniddt.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.4.2/minium/framework/minidoctor.py
--rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/minilimit.py
--rw-r--r--   0 root         (0) root         (0)      832 2022-09-14 13:08:12.000000 minium-1.4.2/minium/framework/miniprogram.py
--rw-r--r--   0 root         (0) root         (0)     6617 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/miniresult.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/minisuite.py
--rw-r--r--   0 root         (0) root         (0)    29964 2023-06-21 12:00:44.000000 minium-1.4.2/minium/framework/minitest.py
--rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.4.2/minium/framework/report.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-05-09 06:36:06.000000 minium-1.4.2/minium/framework/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.675526 minium-1.4.2/minium/framework/tools/
--rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.4.2/minium/framework/tools/report_issue.py
--rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.4.2/minium/framework/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.675526 minium-1.4.2/minium/miniprogram/
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.4.2/minium/miniprogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.679526 minium-1.4.2/minium/miniprogram/base_driver/
--rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/base_driver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49814 2023-06-28 06:28:59.000000 minium-1.4.2/minium/miniprogram/base_driver/app.py
--rw-r--r--   0 root         (0) root         (0)     3929 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/callback.py
--rw-r--r--   0 root         (0) root         (0)    29048 2023-06-29 15:00:02.000000 minium-1.4.2/minium/miniprogram/base_driver/connection.py
--rw-r--r--   0 root         (0) root         (0)    46351 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/element.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-27 02:49:43.000000 minium-1.4.2/minium/miniprogram/base_driver/minium.py
--rw-r--r--   0 root         (0) root         (0)     5959 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/minium_log.py
--rw-r--r--   0 root         (0) root         (0)     8998 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/minium_object.py
--rw-r--r--   0 root         (0) root         (0)    23516 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/base_driver/page.py
--rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/base_driver/prefixer.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-30 02:36:01.000000 minium-1.4.2/minium/miniprogram/base_driver/version.json
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-27 02:49:44.000000 minium-1.4.2/minium/miniprogram/base_driver/version.py
--rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/base_driver/waiter.py
--rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.4.2/minium/miniprogram/qq_minium.py
--rw-r--r--   0 root         (0) root         (0)    39106 2023-06-21 12:00:44.000000 minium-1.4.2/minium/miniprogram/wx_minium.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.679526 minium-1.4.2/minium/native/
--rw-r--r--   0 root         (0) root         (0)     3218 2022-12-19 02:27:07.000000 minium-1.4.2/minium/native/__init__.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.679526 minium-1.4.2/minium/native/lib/
--rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.683526 minium-1.4.2/minium/native/lib/android_base/
--rw-r--r--   0 root         (0) root         (0)     1012 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/android_base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.683526 minium-1.4.2/minium/native/lib/at/
--rw-r--r--   0 root         (0) root         (0)     4087 2022-09-14 13:08:12.000000 minium-1.4.2/minium/native/lib/at/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1755 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/apkapi.py
--rw-r--r--   0 root         (0) root         (0)     5609 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/atproxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.687526 minium-1.4.2/minium/native/lib/at/bin/
--rw-r--r--   0 root         (0) root         (0)  3566862 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/bin/AtServer.apk
--rw-r--r--   0 root         (0) root         (0)    95449 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/bin/AtStub.jar
--rw-r--r--   0 root         (0) root         (0)     3222 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/command_line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.691526 minium-1.4.2/minium/native/lib/at/core/
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      951 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/accesshelper.py
--rw-r--r--   0 root         (0) root         (0)    47016 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/lib/at/core/adbwrap.py
--rw-r--r--   0 root         (0) root         (0)    10763 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/basedriver.py
--rw-r--r--   0 root         (0) root         (0)    15919 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/case_repair_adapter.py
--rw-r--r--   0 root         (0) root         (0)      624 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/config.py
--rw-r--r--   0 root         (0) root         (0)    31731 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/element.py
--rw-r--r--   0 root         (0) root         (0)      669 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18740 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/javadriver.py
--rw-r--r--   0 root         (0) root         (0)     3620 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/resguard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.695526 minium-1.4.2/minium/native/lib/at/core/stf/
--rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/stf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/stf/mincap.py
--rw-r--r--   0 root         (0) root         (0)     5507 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/stf/minitouch.py
--rw-r--r--   0 root         (0) root         (0)    11600 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/uidevice.py
--rw-r--r--   0 root         (0) root         (0)    17965 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/uixml.py
--rw-r--r--   0 root         (0) root         (0)     2711 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/core/websocketcli.py
--rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/eventmonitor.py
--rw-r--r--   0 root         (0) root         (0)     1087 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/hook.py
--rw-r--r--   0 root         (0) root         (0)     8495 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/jlogcat.py
--rw-r--r--   0 root         (0) root         (0)    36015 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/keycode.py
--rw-r--r--   0 root         (0) root         (0)     9492 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/perfcollector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.695526 minium-1.4.2/minium/native/lib/at/tests/
--rw-r--r--   0 root         (0) root         (0)      690 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/AtEvent.py
--rw-r--r--   0 root         (0) root         (0)      326 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/AtSocket.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/adbtest.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/airtesttest.py
--rw-r--r--   0 root         (0) root         (0)    10434 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/atdevicetest.py
--rw-r--r--   0 root         (0) root         (0)      474 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/attestbase.py
--rw-r--r--   0 root         (0) root         (0)     1022 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/drivertest.py
--rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/elementtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/tests/images/
--rw-r--r--   0 root         (0) root         (0)     7525 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/images/1.jpg
--rw-r--r--   0 root         (0) root         (0)     4388 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/images/2.jpg
--rw-r--r--   0 root         (0) root         (0)    80712 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/images/image.jpg
--rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/javadrivertest.py
--rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/minicap_test.py
--rw-r--r--   0 root         (0) root         (0)      375 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/minitest.py
--rw-r--r--   0 root         (0) root         (0)      843 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/minitouch_test.py
--rw-r--r--   0 root         (0) root         (0)      792 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/u2test.py
--rw-r--r--   0 root         (0) root         (0)     1797 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/uixmltest.py
--rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/vs_test.py
--rw-r--r--   0 root         (0) root         (0)      989 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/tests/webdrivertest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/utils/
--rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4896 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/apkinfo.py
--rw-r--r--   0 root         (0) root         (0)   105609 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/axmlparser.py
--rw-r--r--   0 root         (0) root         (0)    27360 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/axmlparser3.py
--rw-r--r--   0 root         (0) root         (0)      526 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/commonhelper.py
--rw-r--r--   0 root         (0) root         (0)     8332 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)      257 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/magic.py
--rw-r--r--   0 root         (0) root         (0)     2457 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/nbsp.py
--rw-r--r--   0 root         (0) root         (0)     1435 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/utils/threadhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/vision/
--rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)      394 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/vision/template_match.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/webdriver/
--rw-r--r--   0 root         (0) root         (0)       72 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15310 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/driver.py
--rw-r--r--   0 root         (0) root         (0)      425 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/error.py
--rw-r--r--   0 root         (0) root         (0)     1376 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/jsapi.py
--rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/miniapp.py
--rw-r--r--   0 root         (0) root         (0)    18973 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/stub.js
--rw-r--r--   0 root         (0) root         (0)      682 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/tabdescription.py
--rw-r--r--   0 root         (0) root         (0)    13005 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/tabwebsocket.py
--rw-r--r--   0 root         (0) root         (0)     8904 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/webelement.py
--rw-r--r--   0 root         (0) root         (0)     1638 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/webhelper.py
--rw-r--r--   0 root         (0) root         (0)     1399 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/webdriver/wspools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/at/wechat/
--rw-r--r--   0 root         (0) root         (0)       79 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wechat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wechat/activtiy.py
--rw-r--r--   0 root         (0) root         (0)      144 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wechat/appvars.py
--rw-r--r--   0 root         (0) root         (0)       80 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/at/wsimp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/case_repair_sdk/
--rw-r--r--   0 root         (0) root         (0)     7663 2022-09-14 13:08:12.000000 minium-1.4.2/minium/native/lib/case_repair_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2816 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/case_repair_sdk/default_trace.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-09-14 13:08:12.000000 minium-1.4.2/minium/native/lib/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/wda/
--rw-r--r--   0 root         (0) root         (0)    40664 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1297 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wda/screenhelper.py
--rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wda/xcui_element_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/lib/wx_wda/
--rw-r--r--   0 root         (0) root         (0)      399 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wx_wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13188 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wx_wda/wdaUI.py
--rw-r--r--   0 root         (0) root         (0)    16169 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/lib/wx_wda/webDriverTool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/qq_native/
--rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/qq_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/qq_native/qandroidnative.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/qq_native/qbasenative.py
--rwxr-xr-x   0 root         (0) root         (0)    16848 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/qq_native/qiosnative.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.699525 minium-1.4.2/minium/native/wx_native/
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.4.2/minium/native/wx_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39266 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/androidnative.py
--rw-r--r--   0 root         (0) root         (0)    23752 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/basenative.py
--rw-r--r--   0 root         (0) root         (0)     8051 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/idenative.py
--rw-r--r--   0 root         (0) root         (0)    34980 2023-06-21 12:00:44.000000 minium-1.4.2/minium/native/wx_native/iosnative.py
--rw-r--r--   0 root         (0) root         (0)     3254 2023-04-27 02:49:44.000000 minium-1.4.2/minium/native/wx_native/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.703525 minium-1.4.2/minium/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.2/minium/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.4.2/minium/utils/emitter.py
--rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.4.2/minium/utils/eventloop.py
--rw-r--r--   0 root         (0) root         (0)     3873 2022-09-19 12:42:30.000000 minium-1.4.2/minium/utils/injectjs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.659526 minium-1.4.2/minium/utils/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.703525 minium-1.4.2/minium/utils/js/es5/
--rw-r--r--   0 root         (0) root         (0)      221 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      255 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      277 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/checkEnv.js
--rw-r--r--   0 root         (0) root         (0)       72 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      535 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/createContext.js
--rw-r--r--   0 root         (0) root         (0)      340 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-30 02:35:45.000000 minium-1.4.2/minium/utils/js/es5/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)      617 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/getUni.js
--rw-r--r--   0 root         (0) root         (0)    38266 2023-06-30 02:35:48.000000 minium-1.4.2/minium/utils/js/es5/helpers.js
--rw-r--r--   0 root         (0) root         (0)      358 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      827 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      487 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      459 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1480 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)     5382 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)     1582 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     2860 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/mockRequestStack.js
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1194 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/requestStack.js
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      198 2023-06-30 02:35:46.000000 minium-1.4.2/minium/utils/js/es5/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)     7138 2023-06-30 02:35:47.000000 minium-1.4.2/minium/utils/js/es5/testAsync.js
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-30 02:35:47.000000 minium-1.4.2/minium/utils/js/es5/uuid.js
--rw-r--r--   0 root         (0) root         (0)      181 2023-06-30 02:35:47.000000 minium-1.4.2/minium/utils/js/es5/waitUtil.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.707526 minium-1.4.2/minium/utils/js/min/
--rw-r--r--   0 root         (0) root         (0)      195 2023-06-30 02:36:00.000000 minium-1.4.2/minium/utils/js/min/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-30 02:35:57.000000 minium-1.4.2/minium/utils/js/min/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      198 2023-06-30 02:35:58.000000 minium-1.4.2/minium/utils/js/min/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-30 02:35:50.000000 minium-1.4.2/minium/utils/js/min/checkEnv.js
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-30 02:35:52.000000 minium-1.4.2/minium/utils/js/min/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      191 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      201 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-30 02:35:52.000000 minium-1.4.2/minium/utils/js/min/createContext.js
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-30 02:35:54.000000 minium-1.4.2/minium/utils/js/min/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-30 02:35:57.000000 minium-1.4.2/minium/utils/js/min/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-30 02:35:55.000000 minium-1.4.2/minium/utils/js/min/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)      555 2023-06-30 02:36:00.000000 minium-1.4.2/minium/utils/js/min/getUni.js
--rw-r--r--   0 root         (0) root         (0)    38266 2023-06-30 02:35:59.000000 minium-1.4.2/minium/utils/js/min/helpers.js
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-30 02:35:55.000000 minium-1.4.2/minium/utils/js/min/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      684 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-30 02:35:50.000000 minium-1.4.2/minium/utils/js/min/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      202 2023-06-30 02:35:49.000000 minium-1.4.2/minium/utils/js/min/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-30 02:35:58.000000 minium-1.4.2/minium/utils/js/min/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      470 2023-06-30 02:35:49.000000 minium-1.4.2/minium/utils/js/min/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1118 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1202 2023-06-30 02:35:55.000000 minium-1.4.2/minium/utils/js/min/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-30 02:35:58.000000 minium-1.4.2/minium/utils/js/min/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-30 02:35:49.000000 minium-1.4.2/minium/utils/js/min/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1413 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-30 02:35:48.000000 minium-1.4.2/minium/utils/js/min/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-30 02:35:52.000000 minium-1.4.2/minium/utils/js/min/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)     4552 2023-06-30 02:35:50.000000 minium-1.4.2/minium/utils/js/min/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)     1386 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-30 02:35:51.000000 minium-1.4.2/minium/utils/js/min/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      664 2023-06-30 02:35:57.000000 minium-1.4.2/minium/utils/js/min/mockRequestStack.js
--rw-r--r--   0 root         (0) root         (0)     1214 2023-06-30 02:35:48.000000 minium-1.4.2/minium/utils/js/min/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-30 02:35:53.000000 minium-1.4.2/minium/utils/js/min/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1041 2023-06-30 02:35:54.000000 minium-1.4.2/minium/utils/js/min/requestStack.js
--rw-r--r--   0 root         (0) root         (0)      284 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      199 2023-06-30 02:35:54.000000 minium-1.4.2/minium/utils/js/min/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-30 02:36:00.000000 minium-1.4.2/minium/utils/js/min/testAsync.js
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-30 02:35:59.000000 minium-1.4.2/minium/utils/js/min/uuid.js
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-30 02:35:56.000000 minium-1.4.2/minium/utils/js/min/waitUtil.js
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.4.2/minium/utils/meta.py
--rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.4.2/minium/utils/platforms.py
--rw-r--r--   0 root         (0) root         (0)    15710 2023-06-21 12:00:44.000000 minium-1.4.2/minium/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-30 02:36:03.659526 minium-1.4.2/minium.egg-info/
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9182 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-30 02:36:03.000000 minium-1.4.2/minium.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-30 02:36:03.707526 minium-1.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2435 2023-05-23 08:31:11.000000 minium-1.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.263971 minium-1.4.3/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-07-06 02:50:01.259971 minium-1.4.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.215971 minium-1.4.3/minium/
+-rw-r--r--   0 root         (0) root         (0)      948 2023-04-27 02:49:43.000000 minium-1.4.3/minium/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.223971 minium-1.4.3/minium/framework/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18577 2023-06-28 02:27:06.000000 minium-1.4.3/minium/framework/assertbase.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.4.3/minium/framework/casedump.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/caseinspect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.223971 minium-1.4.3/minium/framework/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.223971 minium-1.4.3/minium/framework/dist/css/
+-rw-r--r--   0 root         (0) root         (0)      437 2022-09-14 13:08:12.000000 minium-1.4.3/minium/framework/dist/css/app.87891bf0.css
+-rw-r--r--   0 root         (0) root         (0)   240799 2022-09-14 13:08:12.000000 minium-1.4.3/minium/framework/dist/css/chunk-vendors.52eeca6f.css
+-rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/dist/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.223971 minium-1.4.3/minium/framework/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/dist/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/dist/fonts/element-icons.732389de.ttf
+-rw-r--r--   0 root         (0) root         (0)      847 2022-09-14 13:08:12.000000 minium-1.4.3/minium/framework/dist/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.223971 minium-1.4.3/minium/framework/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    17537 2022-09-14 13:08:12.000000 minium-1.4.3/minium/framework/dist/js/app.544bedf4.js
+-rw-r--r--   0 root         (0) root         (0)  1346000 2022-09-14 13:08:12.000000 minium-1.4.3/minium/framework/dist/js/chunk-vendors.22ed339a.js
+-rw-r--r--   0 root         (0) root         (0)     3447 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/errorReport.py
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.227971 minium-1.4.3/minium/framework/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.227971 minium-1.4.3/minium/framework/libs/tgit/
+-rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/libs/tgit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/libs/tgit/auth.py
+-rw-r--r--   0 root         (0) root         (0)    97167 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/libs/tgit/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.227971 minium-1.4.3/minium/framework/libs/unittest/
+-rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.4.3/minium/framework/libs/unittest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22297 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/libs/unittest/case.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/libs/unittest/suite.py
+-rw-r--r--   0 root         (0) root         (0)    20015 2023-06-29 15:00:02.000000 minium-1.4.3/minium/framework/loader.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/logcolor.py
+-rw-r--r--   0 root         (0) root         (0)     7244 2023-04-27 02:49:43.000000 minium-1.4.3/minium/framework/miniconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/miniddt.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.4.3/minium/framework/minidoctor.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/minilimit.py
+-rw-r--r--   0 root         (0) root         (0)      832 2022-09-14 13:08:12.000000 minium-1.4.3/minium/framework/miniprogram.py
+-rw-r--r--   0 root         (0) root         (0)     6617 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/miniresult.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/minisuite.py
+-rw-r--r--   0 root         (0) root         (0)    29964 2023-06-21 12:00:44.000000 minium-1.4.3/minium/framework/minitest.py
+-rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.4.3/minium/framework/report.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-05-09 06:36:06.000000 minium-1.4.3/minium/framework/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.227971 minium-1.4.3/minium/framework/tools/
+-rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.4.3/minium/framework/tools/report_issue.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.4.3/minium/framework/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.231971 minium-1.4.3/minium/miniprogram/
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.4.3/minium/miniprogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.231971 minium-1.4.3/minium/miniprogram/base_driver/
+-rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.4.3/minium/miniprogram/base_driver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49814 2023-06-28 06:28:59.000000 minium-1.4.3/minium/miniprogram/base_driver/app.py
+-rw-r--r--   0 root         (0) root         (0)     3929 2023-06-21 12:00:44.000000 minium-1.4.3/minium/miniprogram/base_driver/callback.py
+-rw-r--r--   0 root         (0) root         (0)    29048 2023-06-29 15:00:02.000000 minium-1.4.3/minium/miniprogram/base_driver/connection.py
+-rw-r--r--   0 root         (0) root         (0)    46455 2023-07-06 02:27:18.000000 minium-1.4.3/minium/miniprogram/base_driver/element.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-27 02:49:43.000000 minium-1.4.3/minium/miniprogram/base_driver/minium.py
+-rw-r--r--   0 root         (0) root         (0)     5959 2023-06-21 12:00:44.000000 minium-1.4.3/minium/miniprogram/base_driver/minium_log.py
+-rw-r--r--   0 root         (0) root         (0)     8998 2023-06-21 12:00:44.000000 minium-1.4.3/minium/miniprogram/base_driver/minium_object.py
+-rw-r--r--   0 root         (0) root         (0)    23516 2023-06-21 12:00:44.000000 minium-1.4.3/minium/miniprogram/base_driver/page.py
+-rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.4.3/minium/miniprogram/base_driver/prefixer.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-06 02:49:59.000000 minium-1.4.3/minium/miniprogram/base_driver/version.json
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-27 02:49:44.000000 minium-1.4.3/minium/miniprogram/base_driver/version.py
+-rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.4.3/minium/miniprogram/base_driver/waiter.py
+-rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.4.3/minium/miniprogram/qq_minium.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-06-21 12:00:44.000000 minium-1.4.3/minium/miniprogram/wx_minium.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.235971 minium-1.4.3/minium/native/
+-rw-r--r--   0 root         (0) root         (0)     3218 2022-12-19 02:27:07.000000 minium-1.4.3/minium/native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.235971 minium-1.4.3/minium/native/lib/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.235971 minium-1.4.3/minium/native/lib/android_base/
+-rw-r--r--   0 root         (0) root         (0)     1012 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/android_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.235971 minium-1.4.3/minium/native/lib/at/
+-rw-r--r--   0 root         (0) root         (0)     4087 2022-09-14 13:08:12.000000 minium-1.4.3/minium/native/lib/at/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/apkapi.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/atproxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.239971 minium-1.4.3/minium/native/lib/at/bin/
+-rw-r--r--   0 root         (0) root         (0)  3566862 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/bin/AtServer.apk
+-rw-r--r--   0 root         (0) root         (0)    95449 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/bin/AtStub.jar
+-rw-r--r--   0 root         (0) root         (0)     3222 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/command_line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.243971 minium-1.4.3/minium/native/lib/at/core/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/accesshelper.py
+-rw-r--r--   0 root         (0) root         (0)    47016 2023-06-21 12:00:44.000000 minium-1.4.3/minium/native/lib/at/core/adbwrap.py
+-rw-r--r--   0 root         (0) root         (0)    10763 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/basedriver.py
+-rw-r--r--   0 root         (0) root         (0)    15919 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/case_repair_adapter.py
+-rw-r--r--   0 root         (0) root         (0)      624 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    31731 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/element.py
+-rw-r--r--   0 root         (0) root         (0)      669 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18740 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/javadriver.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/resguard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.247971 minium-1.4.3/minium/native/lib/at/core/stf/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/stf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/stf/mincap.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/stf/minitouch.py
+-rw-r--r--   0 root         (0) root         (0)    11600 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/uidevice.py
+-rw-r--r--   0 root         (0) root         (0)    17965 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/uixml.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/core/websocketcli.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/eventmonitor.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/hook.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/jlogcat.py
+-rw-r--r--   0 root         (0) root         (0)    36015 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/keycode.py
+-rw-r--r--   0 root         (0) root         (0)     9492 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/perfcollector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/at/tests/
+-rw-r--r--   0 root         (0) root         (0)      690 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/AtEvent.py
+-rw-r--r--   0 root         (0) root         (0)      326 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/AtSocket.py
+-rw-r--r--   0 root         (0) root         (0)       38 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/adbtest.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/airtesttest.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/atdevicetest.py
+-rw-r--r--   0 root         (0) root         (0)      474 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/attestbase.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/drivertest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/elementtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/at/tests/images/
+-rw-r--r--   0 root         (0) root         (0)     7525 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/images/1.jpg
+-rw-r--r--   0 root         (0) root         (0)     4388 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/images/2.jpg
+-rw-r--r--   0 root         (0) root         (0)    80712 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/images/image.jpg
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/javadrivertest.py
+-rw-r--r--   0 root         (0) root         (0)      480 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/minicap_test.py
+-rw-r--r--   0 root         (0) root         (0)      375 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/minitest.py
+-rw-r--r--   0 root         (0) root         (0)      843 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/minitouch_test.py
+-rw-r--r--   0 root         (0) root         (0)      792 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/u2test.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/uixmltest.py
+-rw-r--r--   0 root         (0) root         (0)      493 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/vs_test.py
+-rw-r--r--   0 root         (0) root         (0)      989 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/tests/webdrivertest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/at/utils/
+-rw-r--r--   0 root         (0) root         (0)       37 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4896 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/apkinfo.py
+-rw-r--r--   0 root         (0) root         (0)   105609 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/axmlparser.py
+-rw-r--r--   0 root         (0) root         (0)    27360 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/axmlparser3.py
+-rw-r--r--   0 root         (0) root         (0)      526 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/commonhelper.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      257 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/magic.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/nbsp.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/utils/threadhelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/at/vision/
+-rw-r--r--   0 root         (0) root         (0)       56 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      394 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/vision/template_match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/at/webdriver/
+-rw-r--r--   0 root         (0) root         (0)       72 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15310 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/driver.py
+-rw-r--r--   0 root         (0) root         (0)      425 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/error.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/jsapi.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/miniapp.py
+-rw-r--r--   0 root         (0) root         (0)    18973 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/stub.js
+-rw-r--r--   0 root         (0) root         (0)      682 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/tabdescription.py
+-rw-r--r--   0 root         (0) root         (0)    13005 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/tabwebsocket.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/webelement.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/webhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/webdriver/wspools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/at/wechat/
+-rw-r--r--   0 root         (0) root         (0)       79 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/wechat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/wechat/activtiy.py
+-rw-r--r--   0 root         (0) root         (0)      144 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/wechat/appvars.py
+-rw-r--r--   0 root         (0) root         (0)       80 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/at/wsimp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/case_repair_sdk/
+-rw-r--r--   0 root         (0) root         (0)     7663 2022-09-14 13:08:12.000000 minium-1.4.3/minium/native/lib/case_repair_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/case_repair_sdk/default_trace.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-09-14 13:08:12.000000 minium-1.4.3/minium/native/lib/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/wda/
+-rw-r--r--   0 root         (0) root         (0)    40664 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/wda/screenhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/wda/xcui_element_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.251971 minium-1.4.3/minium/native/lib/wx_wda/
+-rw-r--r--   0 root         (0) root         (0)      399 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/wx_wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/wx_wda/wdaUI.py
+-rw-r--r--   0 root         (0) root         (0)    16169 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/lib/wx_wda/webDriverTool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.255971 minium-1.4.3/minium/native/qq_native/
+-rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/qq_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/qq_native/qandroidnative.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-06-21 12:00:44.000000 minium-1.4.3/minium/native/qq_native/qbasenative.py
+-rwxr-xr-x   0 root         (0) root         (0)    16848 2023-06-21 12:00:44.000000 minium-1.4.3/minium/native/qq_native/qiosnative.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.255971 minium-1.4.3/minium/native/wx_native/
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.4.3/minium/native/wx_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39266 2023-06-21 12:00:44.000000 minium-1.4.3/minium/native/wx_native/androidnative.py
+-rw-r--r--   0 root         (0) root         (0)    23752 2023-06-21 12:00:44.000000 minium-1.4.3/minium/native/wx_native/basenative.py
+-rw-r--r--   0 root         (0) root         (0)     8051 2023-06-21 12:00:44.000000 minium-1.4.3/minium/native/wx_native/idenative.py
+-rw-r--r--   0 root         (0) root         (0)    34980 2023-06-21 12:00:44.000000 minium-1.4.3/minium/native/wx_native/iosnative.py
+-rw-r--r--   0 root         (0) root         (0)     3254 2023-04-27 02:49:44.000000 minium-1.4.3/minium/native/wx_native/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.255971 minium-1.4.3/minium/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.4.3/minium/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.4.3/minium/utils/emitter.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.4.3/minium/utils/eventloop.py
+-rw-r--r--   0 root         (0) root         (0)     3873 2022-09-19 12:42:30.000000 minium-1.4.3/minium/utils/injectjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.215971 minium-1.4.3/minium/utils/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.259971 minium-1.4.3/minium/utils/js/es5/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      255 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      277 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/checkEnv.js
+-rw-r--r--   0 root         (0) root         (0)       72 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      217 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      200 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      340 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      617 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-07-06 02:49:46.000000 minium-1.4.3/minium/utils/js/es5/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      358 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      827 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      207 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      120 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      487 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      216 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      459 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      689 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      441 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      434 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     5382 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-07-06 02:49:44.000000 minium-1.4.3/minium/utils/js/es5/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      726 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1194 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      307 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/uuid.js
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-06 02:49:45.000000 minium-1.4.3/minium/utils/js/es5/waitUtil.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.259971 minium-1.4.3/minium/utils/js/min/
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-06 02:49:58.000000 minium-1.4.3/minium/utils/js/min/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      256 2023-07-06 02:49:55.000000 minium-1.4.3/minium/utils/js/min/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      198 2023-07-06 02:49:56.000000 minium-1.4.3/minium/utils/js/min/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-06 02:49:48.000000 minium-1.4.3/minium/utils/js/min/checkEnv.js
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 02:49:50.000000 minium-1.4.3/minium/utils/js/min/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-06 02:49:52.000000 minium-1.4.3/minium/utils/js/min/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      201 2023-07-06 02:49:51.000000 minium-1.4.3/minium/utils/js/min/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      412 2023-07-06 02:49:50.000000 minium-1.4.3/minium/utils/js/min/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-06 02:49:52.000000 minium-1.4.3/minium/utils/js/min/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-06 02:49:55.000000 minium-1.4.3/minium/utils/js/min/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-06 02:49:53.000000 minium-1.4.3/minium/utils/js/min/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      555 2023-07-06 02:49:58.000000 minium-1.4.3/minium/utils/js/min/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2023-07-06 02:49:57.000000 minium-1.4.3/minium/utils/js/min/helpers.js
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-06 02:49:53.000000 minium-1.4.3/minium/utils/js/min/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-06 02:49:54.000000 minium-1.4.3/minium/utils/js/min/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-06 02:49:48.000000 minium-1.4.3/minium/utils/js/min/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-06 02:49:47.000000 minium-1.4.3/minium/utils/js/min/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-06 02:49:56.000000 minium-1.4.3/minium/utils/js/min/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      470 2023-07-06 02:49:47.000000 minium-1.4.3/minium/utils/js/min/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-06 02:49:50.000000 minium-1.4.3/minium/utils/js/min/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-07-06 02:49:49.000000 minium-1.4.3/minium/utils/js/min/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1202 2023-07-06 02:49:53.000000 minium-1.4.3/minium/utils/js/min/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-06 02:49:56.000000 minium-1.4.3/minium/utils/js/min/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-06 02:49:47.000000 minium-1.4.3/minium/utils/js/min/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-07-06 02:49:49.000000 minium-1.4.3/minium/utils/js/min/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-06 02:49:51.000000 minium-1.4.3/minium/utils/js/min/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      417 2023-07-06 02:49:47.000000 minium-1.4.3/minium/utils/js/min/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      494 2023-07-06 02:49:50.000000 minium-1.4.3/minium/utils/js/min/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)     4552 2023-07-06 02:49:48.000000 minium-1.4.3/minium/utils/js/min/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)     1386 2023-07-06 02:49:54.000000 minium-1.4.3/minium/utils/js/min/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-07-06 02:49:49.000000 minium-1.4.3/minium/utils/js/min/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-06 02:49:55.000000 minium-1.4.3/minium/utils/js/min/mockRequestStack.js
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-07-06 02:49:46.000000 minium-1.4.3/minium/utils/js/min/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-06 02:49:51.000000 minium-1.4.3/minium/utils/js/min/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-06 02:49:52.000000 minium-1.4.3/minium/utils/js/min/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-06 02:49:54.000000 minium-1.4.3/minium/utils/js/min/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      199 2023-07-06 02:49:52.000000 minium-1.4.3/minium/utils/js/min/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-06 02:49:58.000000 minium-1.4.3/minium/utils/js/min/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-06 02:49:57.000000 minium-1.4.3/minium/utils/js/min/uuid.js
+-rw-r--r--   0 root         (0) root         (0)       67 2023-07-06 02:49:54.000000 minium-1.4.3/minium/utils/js/min/waitUtil.js
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.4.3/minium/utils/meta.py
+-rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.4.3/minium/utils/platforms.py
+-rw-r--r--   0 root         (0) root         (0)    15710 2023-06-21 12:00:44.000000 minium-1.4.3/minium/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 02:50:01.219971 minium-1.4.3/minium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      697 2023-07-06 02:50:01.000000 minium-1.4.3/minium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9182 2023-07-06 02:50:01.000000 minium-1.4.3/minium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 02:50:01.000000 minium-1.4.3/minium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-06 02:50:01.000000 minium-1.4.3/minium.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-06 02:50:01.000000 minium-1.4.3/minium.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-06 02:50:01.000000 minium-1.4.3/minium.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 02:50:01.263971 minium-1.4.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-07-06 02:48:35.000000 minium-1.4.3/setup.py
```

### Comparing `minium-1.4.2/PKG-INFO` & `minium-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minium
-Version: 1.4.2
+Version: 1.4.3
 Summary: Minium is the best MiniProgram auto test framework.
 Home-page: https://minitest.weixin.qq.com/#/
 Author: WeChat-Test
 Author-email: minitest@tencent.com
 License: MIT
 Description: 
         install:
```

### Comparing `minium-1.4.2/minium/__init__.py` & `minium-1.4.3/minium/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/assertbase.py` & `minium-1.4.3/minium/framework/assertbase.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/casedump.py` & `minium-1.4.3/minium/framework/casedump.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/caseinspect.py` & `minium-1.4.3/minium/framework/caseinspect.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/dist/css/chunk-vendors.52eeca6f.css` & `minium-1.4.3/minium/framework/dist/css/chunk-vendors.52eeca6f.css`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/dist/favicon.ico` & `minium-1.4.3/minium/framework/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/dist/fonts/element-icons.535877f5.woff` & `minium-1.4.3/minium/framework/dist/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/dist/fonts/element-icons.732389de.ttf` & `minium-1.4.3/minium/framework/dist/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/dist/index.html` & `minium-1.4.3/minium/framework/dist/index.html`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/dist/js/app.544bedf4.js` & `minium-1.4.3/minium/framework/dist/js/app.544bedf4.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/dist/js/chunk-vendors.22ed339a.js` & `minium-1.4.3/minium/framework/dist/js/chunk-vendors.22ed339a.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/errorReport.py` & `minium-1.4.3/minium/framework/errorReport.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/exception.py` & `minium-1.4.3/minium/framework/exception.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/libs/tgit/auth.py` & `minium-1.4.3/minium/framework/libs/tgit/auth.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/libs/tgit/client.py` & `minium-1.4.3/minium/framework/libs/tgit/client.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/libs/unittest/case.py` & `minium-1.4.3/minium/framework/libs/unittest/case.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/libs/unittest/suite.py` & `minium-1.4.3/minium/framework/libs/unittest/suite.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/loader.py` & `minium-1.4.3/minium/framework/loader.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/logcolor.py` & `minium-1.4.3/minium/framework/logcolor.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/miniconfig.py` & `minium-1.4.3/minium/framework/miniconfig.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/miniddt.py` & `minium-1.4.3/minium/framework/miniddt.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/minilimit.py` & `minium-1.4.3/minium/framework/minilimit.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/miniprogram.py` & `minium-1.4.3/minium/framework/miniprogram.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/miniresult.py` & `minium-1.4.3/minium/framework/miniresult.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/minisuite.py` & `minium-1.4.3/minium/framework/minisuite.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/minitest.py` & `minium-1.4.3/minium/framework/minitest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/report.py` & `minium-1.4.3/minium/framework/report.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/session.py` & `minium-1.4.3/minium/framework/session.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/tools/report_issue.py` & `minium-1.4.3/minium/framework/tools/report_issue.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/framework/wording.py` & `minium-1.4.3/minium/framework/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/__init__.py` & `minium-1.4.3/minium/miniprogram/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/app.py` & `minium-1.4.3/minium/miniprogram/base_driver/app.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/callback.py` & `minium-1.4.3/minium/miniprogram/base_driver/callback.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/connection.py` & `minium-1.4.3/minium/miniprogram/base_driver/connection.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/element.py` & `minium-1.4.3/minium/miniprogram/base_driver/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -765,29 +765,30 @@
         初始化
         """
         super(FormElement, self).__init__(element, page_id, connection)
 
     #####################
     #       input       #
     #####################
-    def input(self, text: str):
+    def input(self, text: str, with_confirm=False):
         """
         input 标签输入文本
-        :param text:
+        :param text: 输入的文本
+        :param with_confirm: 输入后触发confirm
         :return:
         """
         if self._tag_name != "input" and self._tag_name != "textarea":
             self.logger.warning(
                 "Element's type is not fit for the method which you call"
             )
             return
         func = "{x}.input".format(x=self._tag_name)
         value = text.strip()
         self.call_func(func, args=[value])
-        if text.endswith("\n"):  # 换行符结尾认为是confirm
+        if text.endswith("\n") or with_confirm:  # 换行符结尾认为是confirm
             self.trigger("confirm", {"value": value})
         # self.trigger("input", {"value": text})
 
     #####################
     #       picker      #
     #####################
     def pick(self, value):
```

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/minium.py` & `minium-1.4.3/minium/miniprogram/base_driver/minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/minium_log.py` & `minium-1.4.3/minium/miniprogram/base_driver/minium_log.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/minium_object.py` & `minium-1.4.3/minium/miniprogram/base_driver/minium_object.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/page.py` & `minium-1.4.3/minium/miniprogram/base_driver/page.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/prefixer.py` & `minium-1.4.3/minium/miniprogram/base_driver/prefixer.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/base_driver/version.py` & `minium-1.4.3/minium/miniprogram/base_driver/version.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/qq_minium.py` & `minium-1.4.3/minium/miniprogram/qq_minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/miniprogram/wx_minium.py` & `minium-1.4.3/minium/miniprogram/wx_minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/__init__.py` & `minium-1.4.3/minium/native/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/android_base/__init__.py` & `minium-1.4.3/minium/native/lib/android_base/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/__init__.py` & `minium-1.4.3/minium/native/lib/at/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/apkapi.py` & `minium-1.4.3/minium/native/lib/at/apkapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/atproxy.py` & `minium-1.4.3/minium/native/lib/at/atproxy.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/bin/AtServer.apk` & `minium-1.4.3/minium/native/lib/at/bin/AtServer.apk`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/bin/AtStub.jar` & `minium-1.4.3/minium/native/lib/at/bin/AtStub.jar`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/command_line.py` & `minium-1.4.3/minium/native/lib/at/command_line.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/accesshelper.py` & `minium-1.4.3/minium/native/lib/at/core/accesshelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/adbwrap.py` & `minium-1.4.3/minium/native/lib/at/core/adbwrap.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/basedriver.py` & `minium-1.4.3/minium/native/lib/at/core/basedriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/case_repair_adapter.py` & `minium-1.4.3/minium/native/lib/at/core/case_repair_adapter.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/config.py` & `minium-1.4.3/minium/native/lib/at/core/config.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/element.py` & `minium-1.4.3/minium/native/lib/at/core/element.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/exceptions.py` & `minium-1.4.3/minium/native/lib/at/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/javadriver.py` & `minium-1.4.3/minium/native/lib/at/core/javadriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/resguard.py` & `minium-1.4.3/minium/native/lib/at/core/resguard.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/stf/mincap.py` & `minium-1.4.3/minium/native/lib/at/core/stf/mincap.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/stf/minitouch.py` & `minium-1.4.3/minium/native/lib/at/core/stf/minitouch.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/uidevice.py` & `minium-1.4.3/minium/native/lib/at/core/uidevice.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/uixml.py` & `minium-1.4.3/minium/native/lib/at/core/uixml.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/core/websocketcli.py` & `minium-1.4.3/minium/native/lib/at/core/websocketcli.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/eventmonitor.py` & `minium-1.4.3/minium/native/lib/at/eventmonitor.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/hook.py` & `minium-1.4.3/minium/native/lib/at/hook.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/jlogcat.py` & `minium-1.4.3/minium/native/lib/at/jlogcat.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/keycode.py` & `minium-1.4.3/minium/native/lib/at/keycode.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/perfcollector.py` & `minium-1.4.3/minium/native/lib/at/perfcollector.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/AtEvent.py` & `minium-1.4.3/minium/native/lib/at/tests/AtEvent.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/atdevicetest.py` & `minium-1.4.3/minium/native/lib/at/tests/atdevicetest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/drivertest.py` & `minium-1.4.3/minium/native/lib/at/tests/drivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/elementtest.py` & `minium-1.4.3/minium/native/lib/at/tests/elementtest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/images/1.jpg` & `minium-1.4.3/minium/native/lib/at/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/images/2.jpg` & `minium-1.4.3/minium/native/lib/at/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/images/image.jpg` & `minium-1.4.3/minium/native/lib/at/tests/images/image.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/minitouch_test.py` & `minium-1.4.3/minium/native/lib/at/tests/minitouch_test.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/u2test.py` & `minium-1.4.3/minium/native/lib/at/tests/u2test.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/uixmltest.py` & `minium-1.4.3/minium/native/lib/at/tests/uixmltest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/tests/webdrivertest.py` & `minium-1.4.3/minium/native/lib/at/tests/webdrivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/utils/apkinfo.py` & `minium-1.4.3/minium/native/lib/at/utils/apkinfo.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/utils/axmlparser.py` & `minium-1.4.3/minium/native/lib/at/utils/axmlparser.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/utils/axmlparser3.py` & `minium-1.4.3/minium/native/lib/at/utils/axmlparser3.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/utils/commonhelper.py` & `minium-1.4.3/minium/native/lib/at/utils/commonhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/utils/decorator.py` & `minium-1.4.3/minium/native/lib/at/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/utils/nbsp.py` & `minium-1.4.3/minium/native/lib/at/utils/nbsp.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/utils/threadhelper.py` & `minium-1.4.3/minium/native/lib/at/utils/threadhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/driver.py` & `minium-1.4.3/minium/native/lib/at/webdriver/driver.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/jsapi.py` & `minium-1.4.3/minium/native/lib/at/webdriver/jsapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/miniapp.py` & `minium-1.4.3/minium/native/lib/at/webdriver/miniapp.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/stub.js` & `minium-1.4.3/minium/native/lib/at/webdriver/stub.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/tabdescription.py` & `minium-1.4.3/minium/native/lib/at/webdriver/tabdescription.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/tabwebsocket.py` & `minium-1.4.3/minium/native/lib/at/webdriver/tabwebsocket.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/webelement.py` & `minium-1.4.3/minium/native/lib/at/webdriver/webelement.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/webhelper.py` & `minium-1.4.3/minium/native/lib/at/webdriver/webhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/webdriver/wspools.py` & `minium-1.4.3/minium/native/lib/at/webdriver/wspools.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/at/wechat/activtiy.py` & `minium-1.4.3/minium/native/lib/at/wechat/activtiy.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/case_repair_sdk/__init__.py` & `minium-1.4.3/minium/native/lib/case_repair_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/case_repair_sdk/default_trace.py` & `minium-1.4.3/minium/native/lib/case_repair_sdk/default_trace.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/wda/__init__.py` & `minium-1.4.3/minium/native/lib/wda/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/wda/screenhelper.py` & `minium-1.4.3/minium/native/lib/wda/screenhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/wda/xcui_element_types.py` & `minium-1.4.3/minium/native/lib/wda/xcui_element_types.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/wx_wda/wdaUI.py` & `minium-1.4.3/minium/native/lib/wx_wda/wdaUI.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/lib/wx_wda/webDriverTool.py` & `minium-1.4.3/minium/native/lib/wx_wda/webDriverTool.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/qq_native/qandroidnative.py` & `minium-1.4.3/minium/native/qq_native/qandroidnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/qq_native/qbasenative.py` & `minium-1.4.3/minium/native/qq_native/qbasenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/qq_native/qiosnative.py` & `minium-1.4.3/minium/native/qq_native/qiosnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/wx_native/androidnative.py` & `minium-1.4.3/minium/native/wx_native/androidnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/wx_native/basenative.py` & `minium-1.4.3/minium/native/wx_native/basenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/wx_native/idenative.py` & `minium-1.4.3/minium/native/wx_native/idenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/wx_native/iosnative.py` & `minium-1.4.3/minium/native/wx_native/iosnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/native/wx_native/wording.py` & `minium-1.4.3/minium/native/wx_native/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/emitter.py` & `minium-1.4.3/minium/utils/emitter.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/injectjs.py` & `minium-1.4.3/minium/utils/injectjs.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/createContext.js` & `minium-1.4.3/minium/utils/js/es5/createContext.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/getUni.js` & `minium-1.4.3/minium/utils/js/es5/getUni.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/helpers.js` & `minium-1.4.3/minium/utils/js/es5/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/hookWxMethod.js` & `minium-1.4.3/minium/utils/js/es5/hookWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/ideMockChooseLocation.js` & `minium-1.4.3/minium/utils/js/es5/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/ideMockGetLocation.js` & `minium-1.4.3/minium/utils/js/es5/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/ideMockGetWeRunData.js` & `minium-1.4.3/minium/utils/js/es5/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/ideMockModal.js` & `minium-1.4.3/minium/utils/js/es5/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/mockChooseImage.js` & `minium-1.4.3/minium/utils/js/es5/mockChooseImage.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/mockCloudCall.js` & `minium-1.4.3/minium/utils/js/es5/mockCloudCall.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/mockNetwork.js` & `minium-1.4.3/minium/utils/js/es5/mockNetwork.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/mockRequestStack.js` & `minium-1.4.3/minium/utils/js/es5/mockRequestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/networkPannel.js` & `minium-1.4.3/minium/utils/js/es5/networkPannel.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/requestStack.js` & `minium-1.4.3/minium/utils/js/es5/requestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/es5/testAsync.js` & `minium-1.4.3/minium/utils/js/es5/testAsync.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/getUni.js` & `minium-1.4.3/minium/utils/js/min/getUni.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/helpers.js` & `minium-1.4.3/minium/utils/js/min/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/hookWxMethod.js` & `minium-1.4.3/minium/utils/js/min/hookWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/ideMockChooseLocation.js` & `minium-1.4.3/minium/utils/js/min/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/ideMockGetLocation.js` & `minium-1.4.3/minium/utils/js/min/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/ideMockGetWeRunData.js` & `minium-1.4.3/minium/utils/js/min/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/ideMockModal.js` & `minium-1.4.3/minium/utils/js/min/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/mockChooseImage.js` & `minium-1.4.3/minium/utils/js/min/mockChooseImage.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/mockCloudCall.js` & `minium-1.4.3/minium/utils/js/min/mockCloudCall.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/mockNetwork.js` & `minium-1.4.3/minium/utils/js/min/mockNetwork.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/mockRequestStack.js` & `minium-1.4.3/minium/utils/js/min/mockRequestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/networkPannel.js` & `minium-1.4.3/minium/utils/js/min/networkPannel.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/js/min/requestStack.js` & `minium-1.4.3/minium/utils/js/min/requestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/meta.py` & `minium-1.4.3/minium/utils/meta.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium/utils/utils.py` & `minium-1.4.3/minium/utils/utils.py`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/minium.egg-info/PKG-INFO` & `minium-1.4.3/minium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minium
-Version: 1.4.2
+Version: 1.4.3
 Summary: Minium is the best MiniProgram auto test framework.
 Home-page: https://minitest.weixin.qq.com/#/
 Author: WeChat-Test
 Author-email: minitest@tencent.com
 License: MIT
 Description: 
         install:
```

### Comparing `minium-1.4.2/minium.egg-info/SOURCES.txt` & `minium-1.4.3/minium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minium-1.4.2/setup.py` & `minium-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 import sys
 
-__version__ = "1.4.2"
+__version__ = "1.4.3"
 
 from setuptools import setup, find_packages
 
 # We do not support Python <3.8
 if sys.version_info < (3, 8):
     print(
         "Unfortunately, your python version is not supported!\n"
```

