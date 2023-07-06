# Comparing `tmp/joserfc-0.3.0.tar.gz` & `tmp/joserfc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joserfc-0.3.0.tar", last modified: Thu Jun 29 13:07:28 2023, max compression
+gzip compressed data, was "joserfc-0.4.0.tar", last modified: Thu Jul  6 13:29:56 2023, max compression
```

## Comparing `joserfc-0.3.0.tar` & `joserfc-0.4.0.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-29 13:07:03.000000 joserfc-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 13:07:28.495389 joserfc-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-29 13:07:03.000000 joserfc-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-29 13:07:03.000000 joserfc-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:07:28.495389 joserfc-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 13:07:03.000000 joserfc-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.487389 joserfc-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/drafts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/drafts/jwe_chacha20.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/drafts/jwe_ecdh_1pu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jwe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jwk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/rfc7515/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7515/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc/rfc7516/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7516/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7517/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7517/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7518/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/derive_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/ec_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jwe_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jwe_encs.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jwe_zips.py
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/jws_algs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/oct_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/rsa_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7518/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7519/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7519/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7519/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7519/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc7638/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc7638/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc8037/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8037/jws_eddsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8037/okp_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.495389 joserfc-0.3.0/src/joserfc/rfc8812/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/rfc8812/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-29 13:07:03.000000 joserfc-0.3.0/src/joserfc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:07:28.491389 joserfc-0.3.0/src/joserfc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 13:07:28.000000 joserfc-0.3.0/src/joserfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.502500 joserfc-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-06 13:29:43.000000 joserfc-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-06 13:29:56.502500 joserfc-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-06 13:29:43.000000 joserfc-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-06 13:29:43.000000 joserfc-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:29:56.502500 joserfc-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 13:29:43.000000 joserfc-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.490499 joserfc-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/drafts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/drafts/jwe_chacha20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/drafts/jwe_ecdh_1pu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7927 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jwe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jwk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/rfc7515/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7515/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc/rfc7516/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8734 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7516/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7517/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/keyset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7517/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7518/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/derive_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/ec_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jwe_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jwe_encs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jwe_zips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/jws_algs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/oct_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/rsa_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7518/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7519/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7519/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7519/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7519/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc7638/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc7638/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc8037/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8037/jws_eddsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8037/okp_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.498500 joserfc-0.4.0/src/joserfc/rfc8812/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/rfc8812/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-06 13:29:43.000000 joserfc-0.4.0/src/joserfc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.494500 joserfc-0.4.0/src/joserfc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:29:56.000000 joserfc-0.4.0/src/joserfc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:29:56.502500 joserfc-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-06 13:29:43.000000 joserfc-0.4.0/tests/test_util.py
```

### Comparing `joserfc-0.3.0/LICENSE` & `joserfc-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/PKG-INFO` & `joserfc-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.3.0
+Version: 0.4.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
+Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -21,15 +22,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# JOSE RFC
+JOSE RFC
+========
 
 ``joserfc`` is a Python implementation of **JSON Object Signing and Encryption** (JOSE).
 
 This package contains implementation of:
 
 - RFC7515: JSON Web Signature
 - RFC7516: JSON Web Encryption
```

### Comparing `joserfc-0.3.0/README.rst` & `joserfc-0.4.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# JOSE RFC
+JOSE RFC
+========
 
 ``joserfc`` is a Python implementation of **JSON Object Signing and Encryption** (JOSE).
 
 This package contains implementation of:
 
 - RFC7515: JSON Web Signature
 - RFC7516: JSON Web Encryption
```

### Comparing `joserfc-0.3.0/pyproject.toml` & `joserfc-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Topic :: Security",
   "Topic :: Security :: Cryptography",
 ]
 
 [project.urls]
 Documentation = "https://jose.authlib.org/"
+Source = "https://github.com/authlib/joserfc"
 Blog = "https://blog.authlib.org/"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
```

### Comparing `joserfc-0.3.0/src/joserfc/drafts/jwe_chacha20.py` & `joserfc-0.4.0/src/joserfc/drafts/jwe_chacha20.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/drafts/jwe_ecdh_1pu.py` & `joserfc-0.4.0/src/joserfc/drafts/jwe_ecdh_1pu.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         "apu": HeaderParameter("Agreement PartyUInfo", "str"),
         "apv": HeaderParameter("Agreement PartyVInfo", "str"),
         "skid": HeaderParameter("Sender Key ID", "str"),
     }
     tag_aware = True
     recommended: bool = False
 
-    def __init__(self, key_wrapping: t.Optional[JWEKeyWrapping]=None):
+    def __init__(self, key_wrapping: t.Optional[JWEKeyWrapping]):
         if key_wrapping is None:
             self.name = "ECDH-1PU"
             self.description = "ECDH-1PU using one-pass KDF and CEK in the Direct Key Agreement mode"
             self.key_size = None
         else:
             self.name = f"ECDH-1PU+{key_wrapping.name}"
             self.description = f"ECDH-1PU using one-pass KDF and CEK wrapped with {key_wrapping.name}"
```

### Comparing `joserfc-0.3.0/src/joserfc/errors.py` & `joserfc-0.4.0/src/joserfc/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,18 @@
 
 
 class MissingAlgorithmError(JoseError):
     error = "missing_algorithm"
     description = 'Missing "alg" value in header'
 
 
+class ConflictAlgorithmError(JoseError):
+    error = "conflict_algorithm"
+
+
 class MissingEncryptionError(JoseError):
     error = "missing_encryption"
     description = 'Missing "enc" value in header'
 
 
 class BadSignatureError(JoseError):
     """This error is designed for JWS/JWT. It is raised when signature
```

### Comparing `joserfc-0.3.0/src/joserfc/jwe.py` & `joserfc-0.4.0/src/joserfc/jwe.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 from .rfc7516.message import perform_encrypt, perform_decrypt
 from .rfc7516.compact import represent_compact, extract_compact
 from .rfc7516.json import represent_json, extract_json
 from .rfc7518.jwe_algs import JWE_ALG_MODELS
 from .rfc7518.jwe_encs import JWE_ENC_MODELS
 from .rfc7518.jwe_zips import JWE_ZIP_MODELS
-from .jwk import CurveKey, KeySet, KeyFlexible, guess_key
+from .jwk import KeySet, CurveKey, KeyFlexible, guess_key
 from .util import to_bytes
 from .registry import Header
 
 __all__ = [
     "types",
     "JWERegistry",
     "JWEEncModel",
@@ -54,15 +54,15 @@
 
 def encrypt_compact(
         protected: Header,
         plaintext: t.AnyStr,
         public_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWERegistry] = None,
-        sender_key: t.Optional[CurveKey] = None) -> str:
+        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None) -> str:
     """Generate a JWE Compact Serialization. The JWE Compact Serialization represents
     encrypted content as a compact, URL-safe string.  This string is::
 
         BASE64URL(UTF8(JWE Protected Header)) || '.' ||
         BASE64URL(JWE Encrypted Key) || '.' ||
         BASE64URL(JWE Initialization Vector) || '.' ||
         BASE64URL(JWE Ciphertext) || '.' ||
@@ -81,28 +81,30 @@
         registry = JWERegistry(algorithms=algorithms)
     elif registry is None:
         registry = default_registry
 
     obj = CompactEncryption(protected, to_bytes(plaintext))
     recipient = Recipient(obj)
     key = guess_key(public_key, recipient)
+    key.check_use("enc")
     recipient.recipient_key = key
-    recipient.sender_key = sender_key
+    if sender_key:
+        recipient.sender_key = _guess_sender_key(recipient, sender_key)
     obj.recipient = recipient
     perform_encrypt(obj, registry)
     out = represent_compact(obj)
     return out.decode("utf-8")
 
 
 def decrypt_compact(
         value: t.AnyStr,
         private_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWERegistry] = None,
-        sender_key: t.Optional[CurveKey] = None) -> CompactEncryption:
+        sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None) -> CompactEncryption:
     """Extract and validate the JWE Compact Serialization (in string, or bytes)
     with the given key. An JWE Compact Serialization looks like:
 
     .. code-block:: text
         :caption: line breaks for display purposes only
 
         OKOawDo13gRp2ojaHV7LFpZcgV7T6DVZKTyKOMTYUmKoTCVJRgckCL9kiMT03JGe
@@ -122,22 +124,25 @@
     obj = extract_compact(to_bytes(value))
     if algorithms:
         registry = JWERegistry(algorithms=algorithms)
     elif registry is None:
         registry = default_registry
 
     recipient = obj.recipient
-    recipient.recipient_key = guess_key(private_key, recipient)
-    recipient.sender_key = sender_key
+    key = guess_key(private_key, recipient)
+    key.check_use("enc")
+    recipient.recipient_key = key
+    if sender_key:
+        recipient.sender_key = _guess_sender_key(recipient, sender_key)
     return perform_decrypt(obj, registry)
 
 
 def encrypt_json(
         obj: JSONEncryption,
-        public_key: KeyFlexible,
+        public_key: t.Optional[KeyFlexible],
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWERegistry] = None,
         sender_key: t.Optional[t.Union[CurveKey, KeySet]] = None) -> JSONSerialization:
     """Generate a JWE JSON Serialization (in dict). The JWE JSON Serialization
     represents encrypted content as a JSON object. This representation is neither
     optimized for compactness nor URL safe.
 
@@ -168,15 +173,17 @@
     elif registry is None:
         registry = default_registry
 
     for recipient in obj.recipients:
         if sender_key and not recipient.sender_key:
             recipient.sender_key = _guess_sender_key(recipient, sender_key)
         if not recipient.recipient_key:
-            recipient.recipient_key = guess_key(public_key, recipient)
+            key = guess_key(public_key, recipient)
+            key.check_use("enc")
+            recipient.recipient_key = key
 
     perform_encrypt(obj, registry)
     return represent_json(obj)
 
 
 def decrypt_json(
         data: JSONSerialization,
@@ -197,15 +204,17 @@
 
     if algorithms:
         registry = JWERegistry(algorithms=algorithms)
     elif registry is None:
         registry = default_registry
 
     for recipient in obj.recipients:
-        recipient.recipient_key = guess_key(private_key, recipient)
+        key = guess_key(private_key, recipient)
+        key.check_use("enc")
+        recipient.recipient_key = key
         if sender_key:
             recipient.sender_key = _guess_sender_key(recipient, sender_key)
 
     return perform_decrypt(obj, registry)
 
 
 def _guess_sender_key(recipient, key: t.Union[CurveKey, KeySet]):
```

### Comparing `joserfc-0.3.0/src/joserfc/jwk.py` & `joserfc-0.4.0/src/joserfc/jwk.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,22 +33,24 @@
     "RSAKey",
     "ECKey",
     "OKPKey",
     "KeySet",
     "guess_key",
 ]
 
+
 def __register():
     JWKRegistry.register(OctKey)
     JWKRegistry.register(RSAKey)
     JWKRegistry.register(ECKey)
     JWKRegistry.register(OKPKey)
     # add {"crv": "secp256k1"} for ECKey
     register_secp256k1()
 
+
 # register all key types
 __register()
 
 
 class GuestProtocol(Protocol):  # pragma: no cover
     def headers(self) -> Header:
         ...
@@ -59,29 +61,35 @@
 
 def guess_key(key: KeyFlexible, obj: GuestProtocol) -> Key:
     """Guess key from a various sources.
 
     :param key: a very flexible key
     :param obj: a protocol that has ``headers`` and ``set_kid`` methods
     """
+    headers = obj.headers()
+
     if isinstance(key, (str, bytes)):
-        return OctKey.import_key(key)
+        rv_key = OctKey.import_key(key)
 
     elif isinstance(key, (SymmetricKey, AsymmetricKey)):
-        return key
+        rv_key = key
 
     elif isinstance(key, KeySet):
-        headers = obj.headers()
         kid = headers.get("kid")
-
         if not kid:
             # choose one key by random
             key: Key = random.choice(key.keys)
             # use side effect to add kid information
             obj.set_kid(key.kid)
-            return key
-        return key.get_by_kid(kid)
+            rv_key = key
+        else:
+            rv_key = key.get_by_kid(kid)
 
     elif callable(key):
-        return key(obj)
+        rv_key = key(obj)
+
+    else:
+        raise ValueError("Invalid key")
 
-    raise ValueError("Invalid key")
+    if "alg" in headers:
+        rv_key.check_alg(headers["alg"])
+    return rv_key
```

### Comparing `joserfc-0.3.0/src/joserfc/jws.py` & `joserfc-0.4.0/src/joserfc/jws.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
     obj = extract_compact(to_bytes(value))
     validate_compact(obj, public_key, algorithms, registry)
     return obj
 
 
 def serialize_json(
         members: t.Union[HeaderDict, t.List[HeaderDict]],
-        payload: bytes,
+        payload: t.AnyStr,
         private_key: KeyFlexible,
         algorithms: t.Optional[t.List[str]] = None,
         registry: t.Optional[JWSRegistry] = None) -> JSONSerialization:
     """Generate a JWS JSON Serialization (in dict). The JWS JSON Serialization
     represents digitally signed or MACed content as a JSON object. This representation
     is neither optimized for compactness nor URL-safe.
 
@@ -201,14 +201,15 @@
         members = [members]
     else:
         flatten = False
         for member in members:
             __check_member(registry, member)
 
     members = [HeaderMember(**member) for member in members]
+    payload = to_bytes(payload)
     obj = JSONSignature(members, payload)
     obj.segments["payload"] = urlsafe_b64encode(payload)
     obj.flattened = flatten
 
     find_key = lambda d: guess_key(private_key, d)
     return sign_json(obj, registry.get_alg, find_key)
```

### Comparing `joserfc-0.3.0/src/joserfc/jwt.py` & `joserfc-0.4.0/src/joserfc/jwt.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/registry.py` & `joserfc-0.4.0/src/joserfc/registry.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,52 +63,62 @@
     "int": is_int,
     "bool": is_bool,
     "url": is_url,
     "jwk": is_jwk,
     "none": not_support,
 }
 
+
 class HeaderParameter:
-    def __init__(self, description: str, validate: t.Union[str, Validate], required: bool=False):
+    """Define the header parameter for JWS and JWE."""
+    def __init__(self, description: str, validate: t.Union[str, Validate], required: bool = False):
+        #: a short description of the header parameter
         self.description: str = description
         if isinstance(validate, str):
-            self.validate: Validate = _value_validators[validate]
-        else:
-            self.validate: Validate = validate
+            validate: Validate = _value_validators[validate]
+        #: a function for validating the header parameter's value
+        self.validate: Validate = validate
+        #: if this header parameter is required
         self.required = required
 
+
 #: Define header parameters for JWS and JWE
 HeaderRegistryDict = t.Dict[str, HeaderParameter]
 
 
 class KeyParameter:
+    """Define the key parameter for JWK."""
     def __init__(
             self,
-             description: str,
-             validate: t.Union[str, Validate],
-             private: t.Optional[bool]=None,
-             required: bool=False):
+            description: str,
+            validate: t.Union[str, Validate],
+            private: t.Optional[bool] = None,
+            required: bool = False):
+        #: a short description of the key parameter
         self.description: str = description
         if isinstance(validate, str):
-            self.validate: Validate = _value_validators[validate]
-        else:
-            self.validate: Validate = validate
+            validate: Validate = _value_validators[validate]
+        #: a function for validating the key parameter's value
+        self.validate: Validate = validate
+        #: if this key parameter for private key only
         self.private = private
+        #: if this key parameter is required
         self.required = required
 
+
 #: Define parameters for JWK
 KeyParameterRegistryDict = t.Dict[str, KeyParameter]
 KeyOperation = namedtuple("KeyOperation", ["description", "use", "private"])
 KeyOperationRegistryDict = t.Dict[str, KeyOperation]
 
 #: Basic JWS header registry
 JWS_HEADER_REGISTRY: HeaderRegistryDict = {
     "alg": HeaderParameter("Algorithm", is_str, True),
     "jku": HeaderParameter("JWK Set URL", is_url),
-    "jwk": HeaderParameter("JSON Web Key",  is_jwk),
+    "jwk": HeaderParameter("JSON Web Key", is_jwk),
     "kid": HeaderParameter("Key ID", is_str),
     "x5u": HeaderParameter("X.509 URL", is_url),
     "x5c": HeaderParameter("X.509 Certificate Chain", is_list_str),
     "x5t": HeaderParameter("X.509 Certificate SHA-1 Thumbprint", is_str),
     "x5t#S256": HeaderParameter("X.509 Certificate SHA-256 Thumbprint", is_str),
     "typ": HeaderParameter("Type", is_str),
     "cty": HeaderParameter("Content Type", is_str),
@@ -120,15 +130,15 @@
     "enc": HeaderParameter("Encryption Algorithm", is_str, True),
     "zip": HeaderParameter("Compression Algorithm", is_str),
     **JWS_HEADER_REGISTRY,
 }
 
 #: Basic JWK parameter registry
 JWK_PARAMETER_REGISTRY = {
-    "kty": KeyParameter("Key ID", is_str, required=True),  # This member MUST be present in a JWK.
+    "kty": KeyParameter("Key Type", is_str, required=True),  # This member MUST be present in a JWK.
     "use": KeyParameter("Public Key Use", in_choices(["sig", "enc"])),
     "key_ops": KeyParameter(
         "Key Operations",
         in_choices([
             "sign",
             "verify",
             "encrypt",
@@ -161,28 +171,38 @@
 }
 
 
 def check_supported_header(registry: HeaderRegistryDict, header: Header):
     allowed_keys = set(registry.keys())
     unsupported_keys = set(header.keys()) - allowed_keys
     if unsupported_keys:
-        raise ValueError(f'Unsupported "{unsupported_keys} in header')
+        raise ValueError(f'Unsupported {unsupported_keys} in header')
 
 
 def check_registry_header(registry: HeaderRegistryDict, header: Header):
     for key in registry:
         reg: HeaderParameter = registry[key]
         if reg.required and key not in header:
             raise ValueError(f'Required "{key}" is missing in header')
         if key in header:
             try:
                 reg.validate(header[key])
             except ValueError as error:
                 raise ValueError(f'"{key}" in header {error}')
 
 
+def check_registry_header_types(registry: HeaderRegistryDict, header: Header):
+    for key in registry:
+        if key in header:
+            try:
+                reg: HeaderParameter = registry[key]
+                reg.validate(header[key])
+            except ValueError as error:
+                raise ValueError(f'"{key}" in header {error}')
+
+
 def check_crit_header(header: Header):
     # check crit header
     if "crit" in header:
         for k in header["crit"]:
             if k not in header:
                 raise ValueError(f'"{k}" is a critical header')
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7515/compact.py` & `joserfc-0.4.0/src/joserfc/rfc7515/compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7515/json.py` & `joserfc-0.4.0/src/joserfc/rfc7515/json.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,17 +80,18 @@
         }
         if "header" in value:
             _sig["header"] = value["header"]
         signatures = [_sig]
 
     members = []
     for sig in signatures:
-        protected_segment = sig["protected"]
-        protected = json_b64decode(protected_segment)
-        member = HeaderMember(protected)
+        member = HeaderMember()
+        if "protected" in sig:
+            protected_segment = sig["protected"]
+            member.protected = json_b64decode(protected_segment)
         if "header" in sig:
             member.header = sig["header"]
         members.append(member)
 
     obj = JSONSignature(members, payload)
     obj.segments.update({"payload": payload_segment})
     obj.flattened = flatten
@@ -115,15 +116,18 @@
         key.check_use("sig")
         if not _verify_signature(signature, payload_segment, alg, key):
             return False
     return True
 
 
 def _verify_signature(signature: JSONSignatureDict, payload_segment, alg: JWSAlgModel, key) -> bool:
-    protected_segment = signature["protected"].encode("utf-8")
+    if "protected" in signature:
+        protected_segment = signature["protected"].encode("utf-8")
+    else:
+        protected_segment = b""
     sig = urlsafe_b64decode(signature["signature"].encode("utf-8"))
     signing_input = b".".join([protected_segment, payload_segment])
     return alg.verify(signing_input, sig, key)
 
 
 def detach_json_content(value: JSONSerialization) -> JSONSerialization:
     # https://www.rfc-editor.org/rfc/rfc7515#appendix-F
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7515/model.py` & `joserfc-0.4.0/src/joserfc/rfc7515/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,17 +63,14 @@
 
     name: str
     description: str
     recommended: bool = False
     algorithm_type = "JWS"
     algorithm_location = "sig"
 
-    def __str__(self):
-        return self.name
-
     @abstractmethod
     def sign(self, msg: bytes, key) -> bytes:
         """Sign the text msg with a private/sign key.
 
         :param msg: message bytes to be signed
         :param key: private key to sign the message
         :return: bytes
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7515/registry.py` & `joserfc-0.4.0/src/joserfc/rfc7515/registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 
 
 class JWSRegistry(object):
     """A registry for JSON Web Signature to keep all the supported algorithms.
     An instance of ``JWSRegistry`` is usually used together with methods in
     ``joserfc.jws``.
 
-    :param headers: extra header parameter definitions
+    :param header_registry: extra header parameters registry
     :param algorithms: allowed algorithms to be used
     :param strict_check_header: only allow header key in the registry to be used
     """
     algorithms: Dict[str, JWSAlgModel] = {}
     recommended: List[str] = []
 
     def __init__(
             self,
-            headers: Optional[HeaderRegistryDict] = None,
+            header_registry: Optional[HeaderRegistryDict] = None,
             algorithms: Optional[List[str]] = None,
             strict_check_header: bool = True):
         self.header_registry: HeaderRegistryDict = {}
         self.header_registry.update(JWS_HEADER_REGISTRY)
-        if headers is not None:
-            self.header_registry.update(headers)
+        if header_registry is not None:
+            self.header_registry.update(header_registry)
         self.allowed = algorithms
         self.strict_check_header = strict_check_header
 
     @classmethod
     def register(cls, alg: JWSAlgModel):
         """Register a given JWS algorithm instance to the registry."""
         cls.algorithms[alg.name] = alg
         if alg.recommended:
             cls.recommended.append(alg.name)
 
     def get_alg(self, name: str):
-        """Get the algorithm instance of the given name.
+        """Get the allowed algorithm instance of the given name.
 
         :param name: value of the ``alg``, e.g. ``HS256``, ``RS256``
         """
         if name not in self.algorithms:
             raise ValueError(f'Algorithm of "{name}" is not supported')
         if self.allowed:
             allowed = self.allowed
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7515/types.py` & `joserfc-0.4.0/src/joserfc/rfc7515/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7516/compact.py` & `joserfc-0.4.0/src/joserfc/rfc7516/compact.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7516/json.py` & `joserfc-0.4.0/src/joserfc/rfc7516/json.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7516/message.py` & `joserfc-0.4.0/src/joserfc/rfc7516/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import typing as t
 from .models import (
-    JWEDirectEncryption,
     CompactEncryption,
     JSONEncryption,
     Recipient,
     JWEAlgModel,
     JWEEncModel,
 )
 from .registry import JWERegistry
 from ..errors import (
     DecodeError,
     InvalidCEKLengthError,
     InvalidEncryptedKeyError,
+    ConflictAlgorithmError,
 )
 from ..util import (
     json_b64encode,
     urlsafe_b64encode,
 )
 
 EncryptionData = t.Union[CompactEncryption, JSONEncryption]
@@ -120,15 +120,15 @@
         alg = registry.get_alg(headers["alg"])
 
         if alg.key_agreement:
             alg.prepare_ephemeral_key(recipient)
 
         if alg.direct_mode:
             if len(recipients) > 1:
-                raise
+                raise ConflictAlgorithmError(f"Algorithm {alg.name} SHOULD have 1 recipient only")
 
             if alg.key_agreement:
                 # 3. When Direct Key Agreement is employed,
                 # let the CEK be the agreed upon key.
                 cek: bytes = alg.encrypt_agreed_upon_key(enc, recipient)
                 if len(cek) * 8 != enc.cek_size:
                     raise InvalidCEKLengthError(f"A key of size {enc.cek_size} bits MUST be used")
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7516/models.py` & `joserfc-0.4.0/src/joserfc/rfc7516/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class Recipient:
     def __init__(
             self,
             parent: t.Union["CompactEncryption", "JSONEncryption"],
             header: t.Optional[Header] = None,
-            recipient_key: t.Optional[Key]=None):
+            recipient_key: t.Optional[Key] = None):
         self.__parent = parent
         self.header = header
         self.recipient_key = recipient_key
         self.sender_key: t.Optional[Key] = None
         self.encrypted_key: t.Optional[bytes] = None
         self.ephemeral_key: t.Optional[CurveKey] = None
         self.segments = {}  # store temporary segments
@@ -91,15 +91,15 @@
     """
     def __init__(
             self,
             protected: Header,
             plaintext: t.Optional[bytes] = None,
             unprotected: t.Optional[Header] = None,
             aad: t.Optional[bytes] = None,
-            flatten: bool=False):
+            flatten: bool = False):
         #: protected header in dict
         self.protected: Header = protected
         #: the plaintext in bytes
         self.plaintext: bytes = plaintext
         #: unprotected header in dict
         self.unprotected: t.Optional[Header] = unprotected
         #: an optional additional authenticated data
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7516/registry.py` & `joserfc-0.4.0/src/joserfc/rfc7516/registry.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .models import JWEAlgModel, JWEEncModel, JWEZipModel
 from ..registry import (
     Header,
     HeaderRegistryDict,
     JWE_HEADER_REGISTRY,
     check_supported_header,
     check_registry_header,
+    check_registry_header_types,
     check_crit_header,
 )
 
 JWEAlgorithm = t.Union[JWEAlgModel, JWEEncModel, JWEZipModel]
 
 AlgorithmsDict = t.TypedDict("AlgorithmsDict", {
     "alg": t.Dict[str, JWEAlgModel],
@@ -20,69 +21,90 @@
     "alg": t.List[str],
     "enc": t.List[str],
     "zip": t.List[str],
 }, total=False)
 
 
 class JWERegistry:
+    """A registry for JSON Web Encryption to keep all the supported algorithms.
+    An instance of ``JWERegistry`` is usually used together with methods in
+    ``joserfc.jwe``.
+
+    :param header_registry: extra header parameters registry
+    :param algorithms: allowed algorithms to be used
+    :param strict_check_header: only allow header key in the registry to be used
+    """
     algorithms: AlgorithmsDict = {
         "alg": {},
         "enc": {},
         "zip": {},
     }
     recommended: t.List[str] = []
 
     def __init__(
             self,
-            headers: t.Optional[HeaderRegistryDict] = None,
+            header_registry: t.Optional[HeaderRegistryDict] = None,
             algorithms: t.Optional[t.List[str]] = None,
             strict_check_header: bool = True):
         self.header_registry: HeaderRegistryDict = {}
         self.header_registry.update(JWE_HEADER_REGISTRY)
-        if headers is not None:
-            self.header_registry.update(headers)
+        if header_registry is not None:
+            self.header_registry.update(header_registry)
         self.allowed = algorithms
         self.strict_check_header = strict_check_header
 
     @classmethod
     def register(cls, model: JWEAlgorithm):
         location: t.Literal["alg", "enc", "zip"] = model.algorithm_location
         cls.algorithms[location][model.name] = model
         if model.recommended:
             cls.recommended.append(model.name)
 
     def check_header(self, header: Header, check_more=False):
+        """Check and validate the fields in header part of a JWS object."""
         check_crit_header(header)
         check_registry_header(self.header_registry, header)
 
         alg = self.get_alg(header["alg"])
         if alg.more_header_registry:
             if check_more:
                 check_registry_header(alg.more_header_registry, header)
+            else:
+                check_registry_header_types(alg.more_header_registry, header)
 
             if self.strict_check_header:
                 allowed_registry = self.header_registry.copy()
                 allowed_registry.update(alg.more_header_registry)
                 check_supported_header(allowed_registry, header)
         elif self.strict_check_header:
             check_supported_header(self.header_registry, header)
 
     def get_alg(self, name: str) -> JWEAlgModel:
+        """Get the allowed ("alg") algorithm instance of the given name.
+
+        :param name: value of the ``alg``, e.g. ``ECDH-ES``, ``A128KW``
+        """
         return self._get_algorithm("alg", name)
 
     def get_enc(self, name: str) -> JWEEncModel:
+        """Get the allowed ("enc") algorithm instance of the given name.
+
+        :param name: value of the ``enc``, e.g. ``A128CBC-HS256``, ``A128GCM``
+        """
         return self._get_algorithm("enc", name)
 
     def get_zip(self, name: str) -> JWEZipModel:
+        """Get the allowed ("zip") algorithm instance of the given name.
+
+        :param name: value of the ``zip``, e.g. ``DEF``
+        """
         return self._get_algorithm("zip", name)
 
-    def _get_algorithm(self, location: str, name: str):
-        if location not in self.algorithms:
-            raise ValueError(f'Invalid location "{location}"')
-        registry: t.Dict[str, JWEAlgorithm] = self.algorithms[location]  # type: ignore
+    def _get_algorithm(self, location: t.Literal["alg", "enc", "zip"], name: str):
+        registry: t.Dict[str, JWEAlgorithm] = self.algorithms[location]
         if name not in registry:
             raise ValueError(f'Algorithm of "{name}" is not supported')
 
         if self.allowed:
             allowed = self.allowed
         else:
             allowed = self.recommended
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7516/types.py` & `joserfc-0.4.0/src/joserfc/rfc7516/types.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7517/models.py` & `joserfc-0.4.0/src/joserfc/rfc7517/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing as t
 from abc import ABCMeta, abstractmethod
-from .types import KeyDict, KeyAny, KeyOptions
+from .types import KeyDict, KeyAny, KeyParameters
 from ..registry import (
     KeyParameterRegistryDict,
     JWK_PARAMETER_REGISTRY,
     KeyOperationRegistryDict,
     JWK_OPERATION_REGISTRY,
 )
 from ..util import to_bytes
@@ -38,15 +38,15 @@
 
     @classmethod
     @abstractmethod
     def import_from_bytes(cls, value: bytes):
         pass
 
     @staticmethod
-    def as_bytes(key: "BaseKey", encoding=None, private=None, password=None) -> bytes:
+    def as_bytes(key: "BaseKey", encoding=None, private=None, password=None) -> bytes:  # pragma: no cover
         return key.raw_value
 
     @classmethod
     def validate_dict_key_registry(cls, dict_key: KeyDict, registry: KeyParameterRegistryDict):
         for k in registry:
             if registry[k].required and k not in dict_key:
                 raise ValueError(f'"{k}" is required')
@@ -59,33 +59,33 @@
 
     @classmethod
     def validate_dict_key_use_operations(cls, dict_key: KeyDict):
         if "use" in dict_key and "key_ops" in dict_key:
             operations = cls.use_key_ops_registry[dict_key["use"]]
             for op in dict_key["key_ops"]:
                 if op not in operations:
-                    raise ValueError(f'"use" and "key_ops" does not match')
+                    raise ValueError('"use" and "key_ops" does not match')
 
 
 class BaseKey(t.Generic[NativePublicKey, NativePrivateKey]):
     key_type: str
     value_registry: KeyParameterRegistryDict
     param_registry: KeyParameterRegistryDict = JWK_PARAMETER_REGISTRY
     operation_registry: KeyOperationRegistryDict = JWK_OPERATION_REGISTRY
     binding = NativeKeyBinding
 
-    def __init__(self, raw_value, original_value, options: KeyOptions = None):
+    def __init__(self, raw_value, original_value, parameters: KeyParameters = None):
         self._raw_value = raw_value
         self.original_value = original_value
-        self.options = options
+        self.extra_parameters = parameters
         if isinstance(original_value, dict):
             data = original_value.copy()
             data["kty"] = self.key_type
-            if options:
-                data.update(dict(options))
+            if parameters:
+                data.update(dict(parameters))
 
             self.validate_dict_key(data)
             self._dict_value = data
         else:
             self._dict_value = None
 
     def keys(self):
@@ -116,16 +116,16 @@
     @property
     def dict_value(self) -> KeyDict:
         """Property of the Key in Dict (JSON)."""
         if self._dict_value:
             return self._dict_value
 
         data = self.binding.convert_raw_key_to_dict(self.raw_value, self.is_private)
-        if self.options:
-            data.update(dict(self.options))
+        if self.extra_parameters:
+            data.update(dict(self.extra_parameters))
         data["kty"] = self.key_type
         self.validate_dict_key(data)
         self._dict_value = data
         return data
 
     @property
     def public_key(self) -> NativePublicKey:
@@ -212,25 +212,25 @@
     @classmethod
     def validate_dict_key(cls, data: KeyDict):
         cls.binding.validate_dict_key_registry(data, cls.param_registry)
         cls.binding.validate_dict_key_registry(data, cls.value_registry)
         cls.binding.validate_dict_key_use_operations(data)
 
     @classmethod
-    def import_key(cls, value: KeyAny, options: KeyOptions = None) -> "BaseKey":
+    def import_key(cls, value: KeyAny, parameters: KeyParameters = None) -> "BaseKey":
         if isinstance(value, dict):
             cls.validate_dict_key(value)
             raw_key = cls.binding.import_from_dict(value)
-            return cls(raw_key, value, options)
+            return cls(raw_key, value, parameters)
 
         raw_key = cls.binding.import_from_bytes(to_bytes(value))
-        return cls(raw_key, value, options)
+        return cls(raw_key, value, parameters)
 
     @classmethod
-    def generate_key(cls, size_or_crv, options: KeyOptions = None, private: bool = True) -> "BaseKey":
+    def generate_key(cls, size_or_crv, parameters: KeyParameters = None, private: bool = True) -> "BaseKey":
         raise NotImplementedError()
 
 
 class SymmetricKey(BaseKey[NativePublicKey, NativePrivateKey], metaclass=ABCMeta):
     @property
     def raw_value(self) -> bytes:
         """The raw key in bytes."""
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7517/pem.py` & `joserfc-0.4.0/src/joserfc/rfc7517/pem.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,47 @@
 import typing as t
 from abc import ABCMeta, abstractmethod
-from cryptography.x509 import load_pem_x509_certificate
 from cryptography.hazmat.primitives.serialization import (
     load_pem_private_key,
     load_pem_public_key,
     load_ssh_public_key,
     load_ssh_private_key,
+    load_der_private_key,
+    load_der_public_key,
     Encoding,
     PrivateFormat,
     PublicFormat,
     BestAvailableEncryption,
     NoEncryption,
 )
 from cryptography.hazmat.backends import default_backend
 from .models import NativeKeyBinding
 from .types import KeyDict
 from ..util import to_bytes
 
 
-def load_pem_key(
-        raw: bytes,
-        ssh_type: t.Optional[bytes]=None,
-        key_type: t.Optional[str]=None,
-        password: t.Optional[bytes]=None):
+def load_pem_key(raw: bytes, ssh_type: t.Optional[bytes] = None, password: t.Optional[bytes] = None):
     if ssh_type and raw.startswith(ssh_type):
-        return load_ssh_public_key(raw, backend=default_backend())
+        key = load_ssh_public_key(raw, backend=default_backend())
 
-    if key_type == "public":
-        return load_pem_public_key(raw, backend=default_backend())
+    elif b"OPENSSH PRIVATE" in raw:
+        key = load_ssh_private_key(raw, password=password, backend=default_backend())
 
-    if key_type == "private" or password is not None:
-        return __load_private_key(raw, password=password)
+    elif b"PUBLIC" in raw:
+        key = load_pem_public_key(raw, backend=default_backend())
 
-    if b"PUBLIC" in raw:
-        return load_pem_public_key(raw, backend=default_backend())
+    elif b"PRIVATE" in raw:
+        key = load_pem_private_key(raw, password=password, backend=default_backend())
 
-    if b"OPENSSH PRIVATE" in raw:
-        return load_ssh_private_key(raw, password=password, backend=default_backend())
-
-    if b"PRIVATE" in raw:
-        return __load_private_key(raw, password=password)
-
-    if b"CERTIFICATE" in raw:
-        cert = load_pem_x509_certificate(raw, default_backend())
-        return cert.public_key()
-
-    try:
-        return __load_private_key(raw, password=password)
-    except ValueError:
-        return load_pem_public_key(raw, backend=default_backend())
-
-
-def __load_private_key(raw: bytes, password: t.Optional[bytes]=None):
-    try:
-        return load_pem_private_key(raw, password=password, backend=default_backend())
-    except ValueError:
-        return load_ssh_private_key(raw, password=password, backend=default_backend())
+    else:
+        try:
+            key = load_der_private_key(raw, password=password, backend=default_backend())
+        except ValueError:
+            key = load_der_public_key(raw, backend=default_backend())
+    return key
 
 
 def dump_pem_key(key, encoding=None, private=False, password=None) -> bytes:
     """Export key into PEM/DER format bytes.
 
     :param key: native cryptography key
     :param encoding: "PEM" or "DER"
@@ -68,15 +50,15 @@
     :return: bytes
     """
 
     if encoding is None or encoding == "PEM":
         encoding = Encoding.PEM
     elif encoding == "DER":
         encoding = Encoding.DER
-    else:
+    else:  # pragma: no cover
         raise ValueError("Invalid encoding: {!r}".format(encoding))
 
     if private:
         if password is None:
             encryption_algorithm = NoEncryption()
         else:
             encryption_algorithm = BestAvailableEncryption(to_bytes(password))
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7517/types.py` & `joserfc-0.4.0/src/joserfc/rfc7517/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import typing as t
 
-__all__ = ["KeyDict", "KeyAny", "KeyOptions", "KeySetDict"]
+__all__ = ["KeyDict", "KeyAny", "KeyParameters", "KeySetDict"]
 
 #: JSON Web Key in dict
 KeyDict = t.Dict[str, t.Union[str, t.List[str]]]
 
 #: Key in str, bytes and dict
 KeyAny = t.Union[str, bytes, KeyDict]
 
-#: extra options for JWK
-KeyOptions = t.TypedDict("KeyOptions", {
+#: extra key parameters for JWK
+KeyParameters = t.TypedDict("KeyParameters", {
     "use": str,
     "key_ops": t.List[str],
     "alg": str,
     "kid": str,
     "x5u": str,
     "x5c": t.List[str],
     "x5t": str,
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/derive_key.py` & `joserfc-0.4.0/src/joserfc/rfc7518/derive_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 
 __all__ = [
     "derive_key_for_concat_kdf",
     "u32be_len_input",
 ]
 
+
 def derive_key_for_concat_kdf(
         shared_key: bytes,
         header: Header,
         cek_size: int,
         key_size: t.Optional[int],
-        tag: t.Optional[bytes]=None):
+        tag: t.Optional[bytes] = None):
     # PartyUInfo
     apu_info = u32be_len_input(header.get("apu"), True)
     # PartyVInfo
     apv_info = u32be_len_input(header.get("apv"), True)
     # SuppPubInfo
 
     if key_size:
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/ec_key.py` & `joserfc-0.4.0/src/joserfc/rfc7518/ec_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     SECP256R1,
     SECP384R1,
     SECP521R1,
 )
 from cryptography.hazmat.backends import default_backend
 from ..rfc7517.models import CurveKey
 from ..rfc7517.pem import CryptographyBinding
-from ..rfc7517.types import KeyDict, KeyOptions
+from ..rfc7517.types import KeyDict, KeyParameters
 from ..util import base64_to_int, int_to_base64
 from ..registry import KeyParameter
 
 
 DSS_CURVES = {
     "P-256": SECP256R1,
     "P-384": SECP384R1,
@@ -117,18 +117,18 @@
     def curve_key_size(self) -> int:
         return self.raw_value.curve.key_size
 
     @classmethod
     def generate_key(
             cls,
             crv: str = "P-256",
-            options: KeyOptions = None,
+            parameters: KeyParameters = None,
             private: bool = True) -> "ECKey":
         if crv not in DSS_CURVES:
             raise ValueError('Invalid crv value: "{}"'.format(crv))
         raw_key = generate_private_key(
             curve=DSS_CURVES[crv](),
             backend=default_backend(),
         )
         if not private:
             raw_key = raw_key.public_key()
-        return cls(raw_key, raw_key, options)
+        return cls(raw_key, raw_key, parameters)
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/jwe_algs.py` & `joserfc-0.4.0/src/joserfc/rfc7518/jwe_algs.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,18 +125,18 @@
     }
 
     def __init__(self, key_size: int):
         self.name = f"A{key_size}GCMKW"
         self.description = f"Key wrapping with AES GCM using {key_size}-bit key"
         self.key_size = key_size
 
-    def wrap_cek(self, cek: bytes, key: bytes) -> bytes:
+    def wrap_cek(self, cek: bytes, key: bytes) -> bytes:  # pragma: no cover
         raise RuntimeError(f"{self.name} can not be used together with Key Agreement")
 
-    def unwrap_cek(self, ek: bytes, key: bytes):
+    def unwrap_cek(self, ek: bytes, key: bytes):  # pragma: no cover
         raise RuntimeError(f"{self.name} can not be used together with Key Agreement")
 
     def encrypt_cek(self, cek: bytes, recipient: Recipient) -> bytes:
         key = self.check_recipient_key(recipient.recipient_key)
         op_key = key.get_op_key("wrapKey")
         self.check_op_key(op_key)
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/jwe_encs.py` & `joserfc-0.4.0/src/joserfc/rfc7518/jwe_encs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,30 +42,30 @@
         al = encode_int(len(aad) * 8, 64)
         msg = aad + iv + ciphertext + al
         d = hmac.new(key, msg, self.hash_alg).digest()
         return d[: self.key_len]
 
     def encrypt(self, plaintext: bytes, cek: bytes, iv: bytes, aad: bytes) -> (bytes, bytes):
         """Key Encryption with AES_CBC_HMAC_SHA2."""
-        hkey = cek[: self.key_len]
-        ekey = cek[self.key_len :]
+        hkey = cek[:self.key_len]
+        ekey = cek[self.key_len:]
 
         pad = PKCS7(AES.block_size).padder()
         padded_data = pad.update(plaintext) + pad.finalize()
 
         cipher = Cipher(AES(ekey), CBC(iv), backend=default_backend())
         enc = cipher.encryptor()
         ciphertext = enc.update(padded_data) + enc.finalize()
         tag = self._hmac(ciphertext, aad, iv, hkey)
         return ciphertext, tag
 
     def decrypt(self, ciphertext: bytes, tag: bytes, cek: bytes, iv: bytes, aad: bytes) -> bytes:
         """Key Decryption with AES AES_CBC_HMAC_SHA2."""
-        hkey = cek[: self.key_len]
-        dkey = cek[self.key_len :]
+        hkey = cek[:self.key_len]
+        dkey = cek[self.key_len:]
 
         ctag = self._hmac(ciphertext, aad, iv, hkey)
         if not hmac.compare_digest(ctag, tag):
             raise ValueError("tag does not match")
 
         cipher = Cipher(AES(dkey), CBC(iv), backend=default_backend())
         d = cipher.decryptor()
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/jwe_zips.py` & `joserfc-0.4.0/src/joserfc/rfc7518/jwe_zips.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/jws_algs.py` & `joserfc-0.4.0/src/joserfc/rfc7518/jws_algs.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/oct_key.py` & `joserfc-0.4.0/src/joserfc/rfc7518/oct_key.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ..util import (
     to_bytes,
     urlsafe_b64decode,
     urlsafe_b64encode,
 )
 from ..registry import KeyParameter
 from ..rfc7517.models import SymmetricKey, NativeKeyBinding
-from ..rfc7517.types import KeyOptions, KeyDict
+from ..rfc7517.types import KeyParameters, KeyDict
 
 
 POSSIBLE_UNSAFE_KEYS = (
     b"-----BEGIN ",
     b"ssh-rsa ",
     b"ssh-ed25519 ",
     b"ecdsa-sha2-",
@@ -42,26 +42,26 @@
     key_type: str = "oct"
     binding = OctBinding
 
     #: https://www.rfc-editor.org/rfc/rfc7518#section-6.4
     value_registry = {"k": KeyParameter("Key Value", "str", True, True)}
 
     @classmethod
-    def generate_key(cls, key_size=256, options: KeyOptions = None, private: bool = True) -> "OctKey":
+    def generate_key(cls, key_size=256, parameters: KeyParameters = None, private: bool = True) -> "OctKey":
         """Generate a ``OctKey`` with the given bit size (not bytes).
 
         :param key_size: size in bit
-        :param options: extra parameter in JWK
+        :param parameters: extra parameter in JWK
         :param private: must be True
         """
         if not private:
             raise ValueError("oct key can not be generated as public")
 
         if key_size % 8 != 0:
             raise ValueError("Invalid bit size for oct key")
 
         length = key_size // 8
         rand = random.SystemRandom()
         chars = string.ascii_letters + string.digits
         value = "".join(rand.choice(chars) for _ in range(length))
         raw_key = to_bytes(value)
-        return cls(raw_key, raw_key, options)
+        return cls(raw_key, raw_key, parameters)
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7518/rsa_key.py` & `joserfc-0.4.0/src/joserfc/rfc7518/rsa_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     rsa_crt_dmq1,
     rsa_crt_iqmp,
 )
 from cryptography.hazmat.backends import default_backend
 from ..registry import KeyParameter
 from ..rfc7517.models import AsymmetricKey
 from ..rfc7517.pem import CryptographyBinding
-from ..rfc7517.types import KeyDict, KeyOptions
+from ..rfc7517.types import KeyDict, KeyParameters
 from ..util import int_to_base64, base64_to_int
 
 
 class RSABinding(CryptographyBinding):
     ssh_type = b"ssh-rsa"
 
     @staticmethod
@@ -113,28 +113,28 @@
             return self.raw_value
         return None
 
     @classmethod
     def generate_key(
             cls,
             key_size: int = 2048,
-            options: KeyOptions = None,
+            parameters: KeyParameters = None,
             private: bool = True) -> "RSAKey":
         if key_size < 512:
             raise ValueError("key_size must not be less than 512")
         if key_size % 8 != 0:
             raise ValueError("Invalid key_size for RSAKey")
         raw_key = generate_private_key(
             public_exponent=65537,
             key_size=key_size,
             backend=default_backend(),
         )
         if not private:
             raw_key = raw_key.public_key()
-        return cls(raw_key, raw_key, options)
+        return cls(raw_key, raw_key, parameters)
 
 
 def has_all_prime_factors(obj) -> bool:
     props = ["p", "q", "dp", "dq", "qi"]
     props_found = [prop in obj for prop in props]
     if all(props_found):
         return True
```

### Comparing `joserfc-0.3.0/src/joserfc/rfc7519/claims.py` & `joserfc-0.4.0/src/joserfc/rfc7519/claims.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc7519/registry.py` & `joserfc-0.4.0/src/joserfc/rfc7519/registry.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc8037/jws_eddsa.py` & `joserfc-0.4.0/src/joserfc/rfc8037/jws_eddsa.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc/rfc8037/okp_key.py` & `joserfc-0.4.0/src/joserfc/rfc8037/okp_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
     PublicFormat,
     PrivateFormat,
     NoEncryption,
 )
 from ..rfc7517.models import CurveKey
-from ..rfc7517.types import KeyDict, KeyOptions
+from ..rfc7517.types import KeyDict, KeyParameters
 from ..rfc7517.pem import CryptographyBinding
 from ..util import to_bytes, urlsafe_b64decode, urlsafe_b64encode
 from ..registry import KeyParameter
 
 PUBLIC_KEYS_MAP = {
     "Ed25519": Ed25519PublicKey,
     "Ed448": Ed448PublicKey,
@@ -105,24 +105,24 @@
     def curve_name(self) -> str:
         return get_key_curve(self.raw_value)
 
     @classmethod
     def generate_key(
             cls,
             crv: str = "Ed25519",
-            options: KeyOptions = None,
+            parameters: KeyParameters = None,
             private: bool = True) -> "OKPKey":
         if crv not in PRIVATE_KEYS_MAP:
             raise ValueError('Invalid crv value: "{}"'.format(crv))
 
         private_key_cls = PRIVATE_KEYS_MAP[crv]
         raw_key = private_key_cls.generate()
         if not private:
             raw_key = raw_key.public_key()
-        return cls(raw_key, raw_key, options=options)
+        return cls(raw_key, raw_key, parameters)
 
 
 def get_key_curve(key: Union[PublicOKPKey, PrivateOKPKey]):
     if isinstance(key, (Ed25519PublicKey, Ed25519PrivateKey)):
         return "Ed25519"
     elif isinstance(key, (Ed448PublicKey, Ed448PrivateKey)):
         return "Ed448"
```

### Comparing `joserfc-0.3.0/src/joserfc/util.py` & `joserfc-0.4.0/src/joserfc/util.py`

 * *Files identical despite different names*

### Comparing `joserfc-0.3.0/src/joserfc.egg-info/PKG-INFO` & `joserfc-0.4.0/src/joserfc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: joserfc
-Version: 0.3.0
+Version: 0.4.0
 Summary: The ultimate Python library for JOSE RFCs, including JWS, JWE, JWK, JWA, JWT
 Author-email: Hsiaoming Yang <me@lepture.com>
 License: BSD-3-Clause
 Project-URL: Documentation, https://jose.authlib.org/
+Project-URL: Source, https://github.com/authlib/joserfc
 Project-URL: Blog, https://blog.authlib.org/
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -21,15 +22,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-# JOSE RFC
+JOSE RFC
+========
 
 ``joserfc`` is a Python implementation of **JSON Object Signing and Encryption** (JOSE).
 
 This package contains implementation of:
 
 - RFC7515: JSON Web Signature
 - RFC7516: JSON Web Encryption
```

### Comparing `joserfc-0.3.0/src/joserfc.egg-info/SOURCES.txt` & `joserfc-0.4.0/src/joserfc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/joserfc/rfc7516/compact.py
 src/joserfc/rfc7516/json.py
 src/joserfc/rfc7516/message.py
 src/joserfc/rfc7516/models.py
 src/joserfc/rfc7516/registry.py
 src/joserfc/rfc7516/types.py
 src/joserfc/rfc7517/__init__.py
+src/joserfc/rfc7517/keyset.py
 src/joserfc/rfc7517/models.py
 src/joserfc/rfc7517/pem.py
 src/joserfc/rfc7517/registry.py
 src/joserfc/rfc7517/types.py
 src/joserfc/rfc7518/__init__.py
 src/joserfc/rfc7518/derive_key.py
 src/joserfc/rfc7518/ec_key.py
@@ -49,8 +50,9 @@
 src/joserfc/rfc7519/__init__.py
 src/joserfc/rfc7519/claims.py
 src/joserfc/rfc7519/registry.py
 src/joserfc/rfc7638/__init__.py
 src/joserfc/rfc8037/__init__.py
 src/joserfc/rfc8037/jws_eddsa.py
 src/joserfc/rfc8037/okp_key.py
-src/joserfc/rfc8812/__init__.py
+src/joserfc/rfc8812/__init__.py
+tests/test_util.py
```

