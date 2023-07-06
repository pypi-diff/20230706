# Comparing `tmp/pysunday-0.3.3.tar.gz` & `tmp/pysunday-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysunday-0.3.3.tar", last modified: Sat Apr 29 07:49:40 2023, max compression
+gzip compressed data, was "pysunday-0.3.4.tar", last modified: Thu Jul  6 04:47:24 2023, max compression
```

## Comparing `pysunday-0.3.3.tar` & `pysunday-0.3.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.050987 pysunday-0.3.3/
--rw-r--r--   0 rnet       (501) staff       (20)       85 2022-11-17 05:46:23.000000 pysunday-0.3.3/MANIFEST.in
--rw-r--r--   0 rnet       (501) staff       (20)     7373 2023-04-29 07:49:40.050778 pysunday-0.3.3/PKG-INFO
--rw-r--r--   0 rnet       (501) staff       (20)     6537 2022-08-11 15:20:07.000000 pysunday-0.3.3/README.md
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.032826 pysunday-0.3.3/bin/
--rwx------   0 rnet       (501) staff       (20)    13723 2022-10-21 08:10:21.000000 pysunday-0.3.3/bin/sunday_install
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.033403 pysunday-0.3.3/pysunday.egg-info/
--rw-r--r--   0 rnet       (501) staff       (20)     7373 2023-04-29 07:49:39.000000 pysunday-0.3.3/pysunday.egg-info/PKG-INFO
--rw-r--r--   0 rnet       (501) staff       (20)     1512 2023-04-29 07:49:39.000000 pysunday-0.3.3/pysunday.egg-info/SOURCES.txt
--rw-r--r--   0 rnet       (501) staff       (20)       25 2023-04-29 07:49:39.000000 pysunday-0.3.3/pysunday.egg-info/dependency_links.txt
--rw-r--r--   0 rnet       (501) staff       (20)      172 2023-04-29 07:49:39.000000 pysunday-0.3.3/pysunday.egg-info/requires.txt
--rw-r--r--   0 rnet       (501) staff       (20)        7 2023-04-29 07:49:39.000000 pysunday-0.3.3/pysunday.egg-info/top_level.txt
--rw-r--r--   0 rnet       (501) staff       (20)      150 2023-04-20 05:47:20.000000 pysunday-0.3.3/requirements.txt
--rw-r--r--   0 rnet       (501) staff       (20)       38 2023-04-29 07:49:40.051038 pysunday-0.3.3/setup.cfg
--rw-r--r--   0 rnet       (501) staff       (20)     2543 2023-04-29 07:48:28.000000 pysunday-0.3.3/setup.py
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.033740 pysunday-0.3.3/src/
--rw-r--r--   0 rnet       (501) staff       (20)       25 2022-07-21 09:31:41.000000 pysunday-0.3.3/src/__init__.py
--rw-r--r--   0 rnet       (501) staff       (20)      247 2022-07-21 09:35:04.000000 pysunday-0.3.3/src/config.ini
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.041252 pysunday-0.3.3/src/core/
--rw-r--r--   0 rnet       (501) staff       (20)     2106 2023-02-02 05:57:39.000000 pysunday-0.3.3/src/core/MultiThread.py
--rw-r--r--   0 rnet       (501) staff       (20)      525 2023-02-03 02:26:35.000000 pysunday-0.3.3/src/core/__init__.py
--rw-r--r--   0 rnet       (501) staff       (20)     2499 2023-02-02 17:17:50.000000 pysunday-0.3.3/src/core/aesCbc.py
--rw-r--r--   0 rnet       (501) staff       (20)     3333 2023-01-04 03:10:51.000000 pysunday-0.3.3/src/core/auth.py
--rw-r--r--   0 rnet       (501) staff       (20)      395 2022-07-26 15:14:48.000000 pysunday-0.3.3/src/core/cachevar.py
--rw-r--r--   0 rnet       (501) staff       (20)     1042 2022-07-26 15:43:25.000000 pysunday-0.3.3/src/core/checkPacNet.py
--rw-r--r--   0 rnet       (501) staff       (20)     1503 2023-02-02 16:36:01.000000 pysunday-0.3.3/src/core/cmdexec.py
--rw-r--r--   0 rnet       (501) staff       (20)     2036 2023-02-02 09:31:26.000000 pysunday-0.3.3/src/core/common.py
--rw-r--r--   0 rnet       (501) staff       (20)      907 2022-07-26 15:39:08.000000 pysunday-0.3.3/src/core/enver.py
--rw-r--r--   0 rnet       (501) staff       (20)    10225 2023-04-10 02:50:33.000000 pysunday-0.3.3/src/core/fetch.py
--rw-r--r--   0 rnet       (501) staff       (20)     1173 2023-02-03 01:50:46.000000 pysunday-0.3.3/src/core/getConfig.py
--rw-r--r--   0 rnet       (501) staff       (20)      128 2023-02-03 01:52:02.000000 pysunday-0.3.3/src/core/getEnv.py
--rw-r--r--   0 rnet       (501) staff       (20)     1702 2023-02-02 06:25:19.000000 pysunday-0.3.3/src/core/getException.py
--rw-r--r--   0 rnet       (501) staff       (20)     3320 2023-01-16 07:49:09.000000 pysunday-0.3.3/src/core/getParser.py
--rw-r--r--   0 rnet       (501) staff       (20)      216 2023-01-16 05:59:19.000000 pysunday-0.3.3/src/core/globalKeyMaps.py
--rw-r--r--   0 rnet       (501) staff       (20)      489 2023-02-03 01:53:12.000000 pysunday-0.3.3/src/core/globalvar.py
--rw-r--r--   0 rnet       (501) staff       (20)     1551 2022-09-07 02:41:44.000000 pysunday-0.3.3/src/core/init.py
--rw-r--r--   0 rnet       (501) staff       (20)     1519 2022-08-02 13:48:47.000000 pysunday-0.3.3/src/core/inner.py
--rw-r--r--   0 rnet       (501) staff       (20)     2558 2023-02-03 02:50:37.000000 pysunday-0.3.3/src/core/logger.py
--rw-r--r--   0 rnet       (501) staff       (20)     1131 2023-01-17 07:27:28.000000 pysunday-0.3.3/src/core/paths.py
--rw-r--r--   0 rnet       (501) staff       (20)     2760 2023-02-03 02:49:51.000000 pysunday-0.3.3/src/core/premust.py
--rw-r--r--   0 rnet       (501) staff       (20)     1180 2023-02-02 07:36:17.000000 pysunday-0.3.3/src/core/printTable.py
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.041554 pysunday-0.3.3/src/login/
--rw-r--r--   0 rnet       (501) staff       (20)        0 2022-07-21 09:31:41.000000 pysunday-0.3.3/src/login/__init__.py
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.041642 pysunday-0.3.3/src/tools/
--rw-r--r--   0 rnet       (501) staff       (20)        0 2022-07-21 09:31:41.000000 pysunday-0.3.3/src/tools/__init__.py
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.045123 pysunday-0.3.3/src/utils/
--rw-r--r--   0 rnet       (501) staff       (20)     3460 2023-04-29 07:48:19.000000 pysunday-0.3.3/src/utils/Email.py
--rw-r--r--   0 rnet       (501) staff       (20)     5093 2023-02-02 16:41:23.000000 pysunday-0.3.3/src/utils/LoginBase.py
--rw-r--r--   0 rnet       (501) staff       (20)      166 2023-04-20 05:47:56.000000 pysunday-0.3.3/src/utils/__init__.py
-drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-04-29 07:49:40.050521 pysunday-0.3.3/src/utils/cryptanalysis/
--rw-r--r--   0 rnet       (501) staff       (20)     1712 2023-02-06 03:08:56.000000 pysunday-0.3.3/src/utils/cryptanalysis/aesToolsNsrd.js
--rw-r--r--   0 rnet       (501) staff       (20)   191937 2022-12-06 08:30:57.000000 pysunday-0.3.3/src/utils/cryptanalysis/cryptojs.js
--rw-r--r--   0 rnet       (501) staff       (20)      189 2023-02-06 03:06:38.000000 pysunday-0.3.3/src/utils/cryptanalysis/decrypt_aestoolsnsrd.js
--rw-r--r--   0 rnet       (501) staff       (20)      374 2023-02-06 02:14:17.000000 pysunday-0.3.3/src/utils/cryptanalysis/decrypt_cryptojs_ECB.js
--rw-r--r--   0 rnet       (501) staff       (20)      170 2022-11-16 02:07:03.000000 pysunday-0.3.3/src/utils/cryptanalysis/decrypt_sm4.js
--rw-r--r--   0 rnet       (501) staff       (20)      394 2023-02-06 02:09:18.000000 pysunday-0.3.3/src/utils/cryptanalysis/encrypt_cryptojs_ECB.js
--rw-r--r--   0 rnet       (501) staff       (20)      245 2023-04-10 02:50:53.000000 pysunday-0.3.3/src/utils/cryptanalysis/encrypt_jsencrypt.js
--rw-r--r--   0 rnet       (501) staff       (20)      254 2022-11-24 07:44:35.000000 pysunday-0.3.3/src/utils/cryptanalysis/encrypt_jsencrypt_hex.js
--rw-r--r--   0 rnet       (501) staff       (20)      204 2022-11-16 02:26:01.000000 pysunday-0.3.3/src/utils/cryptanalysis/encrypt_sm2.js
--rw-r--r--   0 rnet       (501) staff       (20)      170 2022-11-16 02:07:03.000000 pysunday-0.3.3/src/utils/cryptanalysis/encrypt_sm4.js
--rw-r--r--   0 rnet       (501) staff       (20)   130999 2022-11-24 05:55:46.000000 pysunday-0.3.3/src/utils/cryptanalysis/jsencrypt.js
--rw-r--r--   0 rnet       (501) staff       (20)    35644 2022-11-16 02:07:03.000000 pysunday-0.3.3/src/utils/cryptanalysis/sm2.js
--rw-r--r--   0 rnet       (501) staff       (20)     4011 2022-11-16 02:07:03.000000 pysunday-0.3.3/src/utils/cryptanalysis/sm3.js
--rw-r--r--   0 rnet       (501) staff       (20)     5414 2022-11-16 02:07:03.000000 pysunday-0.3.3/src/utils/cryptanalysis/sm4.js
--rw-r--r--   0 rnet       (501) staff       (20)     7504 2023-02-06 03:19:03.000000 pysunday-0.3.3/src/utils/cryptanalyst.py
--rw-r--r--   0 rnet       (501) staff       (20)     1003 2023-04-20 05:54:42.000000 pysunday-0.3.3/src/utils/cryptanalyst_js.py
--rw-r--r--   0 rnet       (501) staff       (20)     1872 2023-02-02 09:58:49.000000 pysunday-0.3.3/src/utils/image.py
--rw-r--r--   0 rnet       (501) staff       (20)      682 2022-07-21 09:31:41.000000 pysunday-0.3.3/src/utils/initOptions.py
--rw-r--r--   0 rnet       (501) staff       (20)      227 2023-02-02 10:00:16.000000 pysunday-0.3.3/src/utils/md5.py
--rw-r--r--   0 rnet       (501) staff       (20)     1214 2023-02-02 10:06:26.000000 pysunday-0.3.3/src/utils/tools.py
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.504652 pysunday-0.3.4/
+-rw-r--r--   0 rnet       (501) staff       (20)       85 2022-11-17 05:46:23.000000 pysunday-0.3.4/MANIFEST.in
+-rw-r--r--   0 rnet       (501) staff       (20)     4785 2023-07-06 04:47:24.504488 pysunday-0.3.4/PKG-INFO
+-rw-r--r--   0 rnet       (501) staff       (20)     3949 2023-07-06 04:35:16.000000 pysunday-0.3.4/README.md
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.491533 pysunday-0.3.4/bin/
+-rwx------   0 rnet       (501) staff       (20)    13723 2022-10-21 08:10:21.000000 pysunday-0.3.4/bin/sunday_install
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.492118 pysunday-0.3.4/pysunday.egg-info/
+-rw-r--r--   0 rnet       (501) staff       (20)     4785 2023-07-06 04:47:24.000000 pysunday-0.3.4/pysunday.egg-info/PKG-INFO
+-rw-r--r--   0 rnet       (501) staff       (20)     1512 2023-07-06 04:47:24.000000 pysunday-0.3.4/pysunday.egg-info/SOURCES.txt
+-rw-r--r--   0 rnet       (501) staff       (20)       25 2023-07-06 04:47:24.000000 pysunday-0.3.4/pysunday.egg-info/dependency_links.txt
+-rw-r--r--   0 rnet       (501) staff       (20)      172 2023-07-06 04:47:24.000000 pysunday-0.3.4/pysunday.egg-info/requires.txt
+-rw-r--r--   0 rnet       (501) staff       (20)        7 2023-07-06 04:47:24.000000 pysunday-0.3.4/pysunday.egg-info/top_level.txt
+-rw-r--r--   0 rnet       (501) staff       (20)      150 2023-04-20 05:47:20.000000 pysunday-0.3.4/requirements.txt
+-rw-r--r--   0 rnet       (501) staff       (20)       38 2023-07-06 04:47:24.504700 pysunday-0.3.4/setup.cfg
+-rw-r--r--   0 rnet       (501) staff       (20)     2543 2023-07-06 04:30:38.000000 pysunday-0.3.4/setup.py
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.492529 pysunday-0.3.4/src/
+-rw-r--r--   0 rnet       (501) staff       (20)       25 2022-07-21 09:31:41.000000 pysunday-0.3.4/src/__init__.py
+-rw-r--r--   0 rnet       (501) staff       (20)      247 2022-07-21 09:35:04.000000 pysunday-0.3.4/src/config.ini
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.497687 pysunday-0.3.4/src/core/
+-rw-r--r--   0 rnet       (501) staff       (20)     2164 2023-05-03 08:46:25.000000 pysunday-0.3.4/src/core/MultiThread.py
+-rw-r--r--   0 rnet       (501) staff       (20)      525 2023-02-03 02:26:35.000000 pysunday-0.3.4/src/core/__init__.py
+-rw-r--r--   0 rnet       (501) staff       (20)     2499 2023-02-02 17:17:50.000000 pysunday-0.3.4/src/core/aesCbc.py
+-rw-r--r--   0 rnet       (501) staff       (20)     3333 2023-01-04 03:10:51.000000 pysunday-0.3.4/src/core/auth.py
+-rw-r--r--   0 rnet       (501) staff       (20)      395 2022-07-26 15:14:48.000000 pysunday-0.3.4/src/core/cachevar.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1042 2022-07-26 15:43:25.000000 pysunday-0.3.4/src/core/checkPacNet.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1503 2023-02-02 16:36:01.000000 pysunday-0.3.4/src/core/cmdexec.py
+-rw-r--r--   0 rnet       (501) staff       (20)     2036 2023-02-02 09:31:26.000000 pysunday-0.3.4/src/core/common.py
+-rw-r--r--   0 rnet       (501) staff       (20)      907 2022-07-26 15:39:08.000000 pysunday-0.3.4/src/core/enver.py
+-rw-r--r--   0 rnet       (501) staff       (20)    10227 2023-05-23 06:42:13.000000 pysunday-0.3.4/src/core/fetch.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1173 2023-02-03 01:50:46.000000 pysunday-0.3.4/src/core/getConfig.py
+-rw-r--r--   0 rnet       (501) staff       (20)      128 2023-02-03 01:52:02.000000 pysunday-0.3.4/src/core/getEnv.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1702 2023-02-02 06:25:19.000000 pysunday-0.3.4/src/core/getException.py
+-rw-r--r--   0 rnet       (501) staff       (20)     3320 2023-01-16 07:49:09.000000 pysunday-0.3.4/src/core/getParser.py
+-rw-r--r--   0 rnet       (501) staff       (20)      216 2023-01-16 05:59:19.000000 pysunday-0.3.4/src/core/globalKeyMaps.py
+-rw-r--r--   0 rnet       (501) staff       (20)      489 2023-02-03 01:53:12.000000 pysunday-0.3.4/src/core/globalvar.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1551 2022-09-07 02:41:44.000000 pysunday-0.3.4/src/core/init.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1519 2022-08-02 13:48:47.000000 pysunday-0.3.4/src/core/inner.py
+-rw-r--r--   0 rnet       (501) staff       (20)     2558 2023-02-03 02:50:37.000000 pysunday-0.3.4/src/core/logger.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1131 2023-01-17 07:27:28.000000 pysunday-0.3.4/src/core/paths.py
+-rw-r--r--   0 rnet       (501) staff       (20)     2760 2023-02-03 02:49:51.000000 pysunday-0.3.4/src/core/premust.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1180 2023-02-02 07:36:17.000000 pysunday-0.3.4/src/core/printTable.py
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.497915 pysunday-0.3.4/src/login/
+-rw-r--r--   0 rnet       (501) staff       (20)        0 2022-07-21 09:31:41.000000 pysunday-0.3.4/src/login/__init__.py
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.498004 pysunday-0.3.4/src/tools/
+-rw-r--r--   0 rnet       (501) staff       (20)        0 2022-07-21 09:31:41.000000 pysunday-0.3.4/src/tools/__init__.py
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.499866 pysunday-0.3.4/src/utils/
+-rw-r--r--   0 rnet       (501) staff       (20)     3460 2023-04-29 07:48:19.000000 pysunday-0.3.4/src/utils/Email.py
+-rw-r--r--   0 rnet       (501) staff       (20)     5093 2023-02-02 16:41:23.000000 pysunday-0.3.4/src/utils/LoginBase.py
+-rw-r--r--   0 rnet       (501) staff       (20)      166 2023-04-20 05:47:56.000000 pysunday-0.3.4/src/utils/__init__.py
+drwxr-xr-x   0 rnet       (501) staff       (20)        0 2023-07-06 04:47:24.504243 pysunday-0.3.4/src/utils/cryptanalysis/
+-rw-r--r--   0 rnet       (501) staff       (20)     1712 2023-02-06 03:08:56.000000 pysunday-0.3.4/src/utils/cryptanalysis/aesToolsNsrd.js
+-rw-r--r--   0 rnet       (501) staff       (20)   191937 2022-12-06 08:30:57.000000 pysunday-0.3.4/src/utils/cryptanalysis/cryptojs.js
+-rw-r--r--   0 rnet       (501) staff       (20)      189 2023-02-06 03:06:38.000000 pysunday-0.3.4/src/utils/cryptanalysis/decrypt_aestoolsnsrd.js
+-rw-r--r--   0 rnet       (501) staff       (20)      374 2023-02-06 02:14:17.000000 pysunday-0.3.4/src/utils/cryptanalysis/decrypt_cryptojs_ECB.js
+-rw-r--r--   0 rnet       (501) staff       (20)      170 2022-11-16 02:07:03.000000 pysunday-0.3.4/src/utils/cryptanalysis/decrypt_sm4.js
+-rw-r--r--   0 rnet       (501) staff       (20)      394 2023-02-06 02:09:18.000000 pysunday-0.3.4/src/utils/cryptanalysis/encrypt_cryptojs_ECB.js
+-rw-r--r--   0 rnet       (501) staff       (20)      245 2023-04-10 02:50:53.000000 pysunday-0.3.4/src/utils/cryptanalysis/encrypt_jsencrypt.js
+-rw-r--r--   0 rnet       (501) staff       (20)      254 2022-11-24 07:44:35.000000 pysunday-0.3.4/src/utils/cryptanalysis/encrypt_jsencrypt_hex.js
+-rw-r--r--   0 rnet       (501) staff       (20)      204 2022-11-16 02:26:01.000000 pysunday-0.3.4/src/utils/cryptanalysis/encrypt_sm2.js
+-rw-r--r--   0 rnet       (501) staff       (20)      170 2022-11-16 02:07:03.000000 pysunday-0.3.4/src/utils/cryptanalysis/encrypt_sm4.js
+-rw-r--r--   0 rnet       (501) staff       (20)   130999 2022-11-24 05:55:46.000000 pysunday-0.3.4/src/utils/cryptanalysis/jsencrypt.js
+-rw-r--r--   0 rnet       (501) staff       (20)    35644 2022-11-16 02:07:03.000000 pysunday-0.3.4/src/utils/cryptanalysis/sm2.js
+-rw-r--r--   0 rnet       (501) staff       (20)     4011 2022-11-16 02:07:03.000000 pysunday-0.3.4/src/utils/cryptanalysis/sm3.js
+-rw-r--r--   0 rnet       (501) staff       (20)     5414 2022-11-16 02:07:03.000000 pysunday-0.3.4/src/utils/cryptanalysis/sm4.js
+-rw-r--r--   0 rnet       (501) staff       (20)     7504 2023-02-06 03:19:03.000000 pysunday-0.3.4/src/utils/cryptanalyst.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1003 2023-04-20 05:54:42.000000 pysunday-0.3.4/src/utils/cryptanalyst_js.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1872 2023-02-02 09:58:49.000000 pysunday-0.3.4/src/utils/image.py
+-rw-r--r--   0 rnet       (501) staff       (20)      682 2022-07-21 09:31:41.000000 pysunday-0.3.4/src/utils/initOptions.py
+-rw-r--r--   0 rnet       (501) staff       (20)      227 2023-02-02 10:00:16.000000 pysunday-0.3.4/src/utils/md5.py
+-rw-r--r--   0 rnet       (501) staff       (20)     1214 2023-02-02 10:06:26.000000 pysunday-0.3.4/src/utils/tools.py
```

### Comparing `pysunday-0.3.3/bin/sunday_install` & `pysunday-0.3.4/bin/sunday_install`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/pysunday.egg-info/SOURCES.txt` & `pysunday-0.3.4/pysunday.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/setup.py` & `pysunday-0.3.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import stat
 import pdb
 from os import path, chmod, listdir, system
 from setuptools import setup
 from setuptools.command.install import install
 
-version = '0.3.3'
+version = '0.3.4'
 
 binCwd = path.join(path.dirname(path.realpath(__file__)), 'bin')
 if path.exists(binCwd):
     for name in listdir(binCwd): chmod(path.join(binCwd, name), stat.S_IRWXU)
 
 with open('./README.md', 'r') as f:
     readme = f.read()
```

### Comparing `pysunday-0.3.3/src/core/MultiThread.py` & `pysunday-0.3.4/src/core/MultiThread.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,15 +46,17 @@
         开始执行多线程任务
 
         **Parameters:**
 
         * **isDelay:** `bool` -- 是否等待执行完成，默认为True，False表示后台运行
         * **isBar:** `bool` -- 是否显示进度条, 默认False
         """
-        for i in self.threads: i.start()
+        for i in self.threads:
+            if not isDelay: i.setDaemon(True)
+            i.start()
         if isDelay:
             isShowBar = isBar and self.data_count > 0
             if isShowBar:
                 self.pbar = tqdm.tqdm(total=self.data_count)
             for i in self.threads: i.join()
             if isShowBar:
                 self.pbar.close()
```

### Comparing `pysunday-0.3.3/src/core/__init__.py` & `pysunday-0.3.4/src/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/aesCbc.py` & `pysunday-0.3.4/src/core/aesCbc.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/auth.py` & `pysunday-0.3.4/src/core/auth.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/checkPacNet.py` & `pysunday-0.3.4/src/core/checkPacNet.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/cmdexec.py` & `pysunday-0.3.4/src/core/cmdexec.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/common.py` & `pysunday-0.3.4/src/core/common.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/enver.py` & `pysunday-0.3.4/src/core/enver.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/fetch.py` & `pysunday-0.3.4/src/core/fetch.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             password = auth.addParams('pac_pass', 'PAC代理密码', value=getenv('pac_pass'), isPass=True)
             logger.warning('pac认证网络, 网络交互使用代理中')
             session.proxy_auth = HTTPProxyAuth(username, password)
             self._hasPacProxy = True
             return True
         return False
 
-    def requestByType(self, type, times, *args, **kwargs):
+    def requestByType(self, type, times=0, *args, **kwargs):
         try:
             stime = time.time()
             params = omit(kwargs, ['timeout_time'])
             logger.debug('fetching %s %s' % (args, params))
             if 'timeout' not in params: params['timeout'] = 15
             res = getattr(self.session, type)(*args, **params)
             logger.info('fetch result %s (状态: %d, 用时: %.3f)' % (res.url, res.status_code, time.time() - stime))
```

### Comparing `pysunday-0.3.3/src/core/getConfig.py` & `pysunday-0.3.4/src/core/getConfig.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/getException.py` & `pysunday-0.3.4/src/core/getException.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/getParser.py` & `pysunday-0.3.4/src/core/getParser.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/init.py` & `pysunday-0.3.4/src/core/init.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/inner.py` & `pysunday-0.3.4/src/core/inner.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/logger.py` & `pysunday-0.3.4/src/core/logger.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/paths.py` & `pysunday-0.3.4/src/core/paths.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/premust.py` & `pysunday-0.3.4/src/core/premust.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/core/printTable.py` & `pysunday-0.3.4/src/core/printTable.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/Email.py` & `pysunday-0.3.4/src/utils/Email.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/LoginBase.py` & `pysunday-0.3.4/src/utils/LoginBase.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalysis/aesToolsNsrd.js` & `pysunday-0.3.4/src/utils/cryptanalysis/aesToolsNsrd.js`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalysis/cryptojs.js` & `pysunday-0.3.4/src/utils/cryptanalysis/cryptojs.js`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalysis/jsencrypt.js` & `pysunday-0.3.4/src/utils/cryptanalysis/jsencrypt.js`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalysis/sm2.js` & `pysunday-0.3.4/src/utils/cryptanalysis/sm2.js`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalysis/sm3.js` & `pysunday-0.3.4/src/utils/cryptanalysis/sm3.js`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalysis/sm4.js` & `pysunday-0.3.4/src/utils/cryptanalysis/sm4.js`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalyst.py` & `pysunday-0.3.4/src/utils/cryptanalyst.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/cryptanalyst_js.py` & `pysunday-0.3.4/src/utils/cryptanalyst_js.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/image.py` & `pysunday-0.3.4/src/utils/image.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/initOptions.py` & `pysunday-0.3.4/src/utils/initOptions.py`

 * *Files identical despite different names*

### Comparing `pysunday-0.3.3/src/utils/tools.py` & `pysunday-0.3.4/src/utils/tools.py`

 * *Files identical despite different names*

