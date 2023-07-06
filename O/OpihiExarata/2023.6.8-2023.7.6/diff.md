# Comparing `tmp/OpihiExarata-2023.6.8.tar.gz` & `tmp/OpihiExarata-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpihiExarata-2023.6.8.tar", last modified: Thu Jun  8 02:48:22 2023, max compression
+gzip compressed data, was "OpihiExarata-2023.7.6.tar", last modified: Thu Jul  6 05:36:47 2023, max compression
```

## Comparing `OpihiExarata-2023.6.8.tar` & `OpihiExarata-2023.7.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.614615 OpihiExarata-2023.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/configuration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/jplhorizons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39220 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)   129487 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/name.py
--rw-r--r--   0 runner    (1001) docker     (123)    41611 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/old_automatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.622615 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/automatic.ui
--rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
--rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
--rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/old_manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/selector.ui
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/window_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    50589 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/library/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/mpcrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/phototable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/tcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/opihi/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/orbit/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/orbfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/photometry/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/photometry/panstarrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/photometry/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/src/opihiexarata/propagate/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/propagate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/propagate/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/propagate/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/tests/test_global.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-06 05:36:29.000000 OpihiExarata-2023.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-06 05:36:29.000000 OpihiExarata-2023.7.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.305630 OpihiExarata-2023.7.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.313629 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 05:36:47.000000 OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.313629 OpihiExarata-2023.7.6/src/opihiexarata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.313629 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29924 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/astrometry/webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16247 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/configuration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.317630 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/jplhorizons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.317630 OpihiExarata-2023.7.6/src/opihiexarata/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39220 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129487 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41611 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/old_automatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.325630 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/automatic.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
+-rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/old_manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/selector.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/window_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50589 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/gui/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.329630 OpihiExarata-2023.7.6/src/opihiexarata/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/mpcrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/phototable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/tcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/library/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.329630 OpihiExarata-2023.7.6/src/opihiexarata/opihi/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46007 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/opihi/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/src/opihiexarata/orbit/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/orbfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/orbit/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/src/opihiexarata/photometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/photometry/panstarrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/photometry/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/src/opihiexarata/propagate/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/propagate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/propagate/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/propagate/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/src/opihiexarata/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 05:36:47.333629 OpihiExarata-2023.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-06 05:36:30.000000 OpihiExarata-2023.7.6/tests/test_global.py
```

### Comparing `OpihiExarata-2023.6.8/LICENSE` & `OpihiExarata-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/PKG-INFO` & `OpihiExarata-2023.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.6.8
+Version: 2023.7.6
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.6.8/README.md` & `OpihiExarata-2023.7.6/README.md`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/setup.py` & `OpihiExarata-2023.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/PKG-INFO` & `OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.6.8
+Version: 2023.7.6
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/SOURCES.txt` & `OpihiExarata-2023.7.6/src/OpihiExarata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/__init__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/__main__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/__main__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/astrometry/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/astrometry/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/astrometry/webclient.py` & `OpihiExarata-2023.7.6/src/opihiexarata/astrometry/webclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,20 +65,20 @@
             # These parameters are for licensing and distribution terms.
             ("allow_commercial_use", "d", str),
             ("allow_modifications", "d", str),
             # For visibility by the general public.
             ("publicly_visible", "n", str),
             # Image scaling parameters, if provided, when known, helps the
             # processing a little.
-            ("scale_units", "degwidth", str),
-            ("scale_type", "ev", str),
-            ("scale_lower", None, float),
-            ("scale_upper", None, float),
-            ("scale_est", 0.5, float),
-            ("scale_err", 10, float),
+            ("scale_units", "arcsecperpix", str),
+            ("scale_type", "ul", str),
+            ("scale_lower", 0.9, float),
+            ("scale_upper", 1.0, float),
+            ("scale_est", None, float),
+            ("scale_err", None, float),
             # These parameters allows for the establishment of an initial guess
             # specified byt he centers, and its maximal deviation as specified
             # by the radius parameter. (In degrees.)
             ("center_ra", None, float),
             ("center_dec", None, float),
             ("radius", None, float),
             # Image properties, preprocessing it a little can help in its
```

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/configuration.yaml` & `OpihiExarata-2023.7.6/src/opihiexarata/configuration.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,19 @@
 MONITOR_PLOT_FILTER_R_LINE_COLOR : "#FFA500"
 MONITOR_PLOT_FILTER_I_LINE_COLOR : "#4B0082"
 MONITOR_PLOT_FILTER_Z_LINE_COLOR : "#383838"
 MONITOR_PLOT_FILTER_1_LINE_COLOR : "#00FFFF"
 MONITOR_PLOT_FILTER_2_LINE_COLOR : "#FF00FF"
 MONITOR_PLOT_FILTER_B_LINE_COLOR : "#FFFF00"
 
+# The monitor plot uses datetime objects to display the time. By default, we 
+# use UTC as the timezone which to plot everything in. However, this can be 
+# modified here by supplying an IANA timezone name to convert to.
+MONITOR_PLOT_IANA_TIMEZONE : "Etc/UTC"
+
 ############################################################
 ##########     Opihi Preprocess Configuration
 ############################################################
 
 # The bias frame of the image.
 PREPROCESS_BIAS_FITS_FILENAME : ""
```

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/jplhorizons.py` & `OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/jplhorizons.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/ephemeris/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/__init__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/automatic.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/functions.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/functions.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/manual.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/manual.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/name.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/name.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/old_automatic.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/old_automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/automatic.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/automatic.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/manual.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/old_manual.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/old_manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_automatic.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_automatic.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_manual.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_manual.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_selector.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/qtui_selector.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/selector.ui` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/selector.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/window_icon.png` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/qtui/window_icon.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/gui/selector.py` & `OpihiExarata-2023.7.6/src/opihiexarata/gui/selector.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/__init__.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/config.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/config.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/conversion.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/conversion.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """For miscellaneous conversions."""
 
 import time
+import datetime
+import zoneinfo
 import numpy as np
 import astropy.coordinates as ap_coordinates
 import astropy.time as ap_time
 import astropy.units as ap_units
 
 import opihiexarata.library as library
 import opihiexarata.library.error as error
@@ -319,14 +321,76 @@
     """
     # We can just derive it from the system UNIX time.
     current_unix_time = time.time()
     current_jd = unix_time_to_julian_day(unix_time=current_unix_time)
     return current_jd
 
 
+def datetime_timezone_1_to_timezone_2(
+    from_datetime: hint.Union[hint.datetime, str], from_timezone: str, to_timezone: str
+) -> hint.datetime:
+    """This function converts a date time from one timezone to another timezone.
+
+    If the datetime provided is a string of an ISO 8601 time, we convert it,
+    otherwise, we raise. The timezones provided can be any IANA timezone.
+
+    Parameters
+    ----------
+    from_datetime : datetime or str
+        The data time, or string representation of one to convert.
+    from_timezone : str
+        The timezone which date_time is currently in.
+    to_timezone : str
+        The timezone which we are converting to.
+
+    Returns
+    -------
+    to_datetime : datetime
+        The datetime after the conversion.
+    """
+    # Check if the datetime is really a datetime or a string representation
+    # thereof.
+    if isinstance(from_datetime, datetime.datetime):
+        # All good.
+        pass
+    elif isinstance(from_datetime, str):
+        # Try and convert.
+        try:
+            from_datetime = datetime.datetime.fromisoformat(from_datetime)
+        except ValueError:
+            raise error.InputError(
+                "The string format of the datetime is not valid and cannot be"
+                " converted. We require it to be in an ISO 8601-like format. The input:"
+                " {inp}".format(inp=from_datetime)
+            )
+    else:
+        raise error.InputError(
+            "The datetime input provided is neither a datetime or a datetime string to"
+            " be converted. The input: {inp}".format(inp=from_datetime)
+        )
+
+    # Adding the important timezone information, using the built in class.
+    from_timezone = zoneinfo.ZoneInfo(key=from_timezone)
+    to_timezone = zoneinfo.ZoneInfo(key=to_timezone)
+    # Adding it to the datetime.
+    from_datetime_zone_aware = datetime.datetime(
+        year=from_datetime.year,
+        month=from_datetime.month,
+        day=from_datetime.day,
+        hour=from_datetime.hour,
+        minute=from_datetime.minute,
+        second=from_datetime.second,
+        microsecond=from_datetime.microsecond,
+        tzinfo=from_timezone,
+    )
+    # Converting it to a different timezone.
+    to_datetime = from_datetime_zone_aware.astimezone(to_timezone)
+    return to_datetime
+
+
 def string_month_to_number(month_str: str) -> int:
     """A function to convert from the name of a month to the month number.
     This is just because it is easy to have here and to add a package import
     for something like this is silly.
 
     Parameters
     ----------
```

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/engine.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/engine.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/error.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/error.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/fits.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/fits.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,23 +187,25 @@
             continue
         else:
             # Otherwise, we just use the default.
             valuedex = defaultdex
 
         # We type check as FITS header files are picky about the object types
         # they get FITS headers really only support some specific basic types.
-        if isinstance(valuedex, (int, float, bool, str)):
+        if isinstance(valuedex, str):
+            # This is a valid entry.
+            pass
+        elif isinstance(valuedex, (int, float, bool)):
             # These are generally accepted types.
             if np.isfinite(valuedex):
                 # All good.
                 pass
             else:
                 if np.isnan(valuedex):
                     valuedex = "NaN"
-            pass
         elif valuedex is None:
             # Astropy may be able to handle it.
             pass
         else:
             raise error.InputError(
                 "The input value {v} has a type of {t}. FITS file headers really"
                 " only accept strings or numbers.".format(v=valuedex, t=type(valuedex))
```

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/hint.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 imports and other nasty things.
 """
 
 from typing import *
 from collections import *
 from collections.abc import *
 
+from datetime import *
+
 from argparse import ArgumentParser, Namespace
 
 from astropy.io.fits import Header, FITS_rec
 from astropy.table import Table, Row
 from astropy.wcs import WCS
 
 from matplotlib.backend_bases import MouseEvent
```

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/http.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/http.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/image.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/image.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/json.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/json.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/mpcrecord.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/mpcrecord.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/path.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/path.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/phototable.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/phototable.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/tcs.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/tcs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/library/temporary.py` & `OpihiExarata-2023.7.6/src/opihiexarata/library/temporary.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/opihi/database.py` & `OpihiExarata-2023.7.6/src/opihiexarata/opihi/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """The database solution for storing and recording zero point data. 
 We use a flat file database here with ordered directories to make it easily 
 transversal by other tools and to have it be simple. A single instance of 
 this class should monitor its own database."""
 
 import os
 import datetime
+import zoneinfo
 import glob
+import copy
 import astropy.table as ap_table
 import plotly.express as px
 
 import opihiexarata.library as library
 import opihiexarata.library.error as error
 import opihiexarata.library.hint as hint
 
@@ -864,23 +866,72 @@
             end_day=e_dy,
             end_hour=e_hr,
             end_minute=e_mi,
             end_second=e_sc,
         )
         # All done.
         return query_record_table
+    
+    def query_database_all(self) -> hint.Table:
+        """This queries the table for all of the data within it.
+        
+        This is a wrapper function around the normal query tool for a range 
+        of dates which starts and ends way beyond the normal date ranges of 
+        Opihi, and so, will cover all of the data within the database.
+        
+        Parameters
+        ----------
+        None
+        
+        Returns
+        -------
+        query_record_table : Table
+            A table containing the data as queried from the database across 
+            all reasonable times.
+        """
+        # These two dates are far enough apart that it should cover the entire
+        # database.
+        all_begin_year=2000
+        all_begin_month=1
+        all_begin_day=1
+        all_begin_hour=0
+        all_begin_minute=0
+        all_begin_second=0
+        all_end_year=2101
+        all_end_month=1
+        all_end_day=1
+        all_end_hour=0
+        all_end_minute=0
+        all_end_second=0
+        # Pulling the table between this large date range.
+        query_record_table = self.query_database_between_datetimes(
+            begin_year=all_begin_year,
+            begin_month=all_begin_month,
+            begin_day=all_begin_day,
+            begin_hour=all_begin_hour,
+            begin_minute=all_begin_minute,
+            begin_second=all_begin_second,
+            end_year=all_end_year,
+            end_month=all_end_month,
+            end_day=all_end_day,
+            end_hour=all_end_hour,
+            end_minute=all_end_minute,
+            end_second=all_end_second,
+        )
+        return query_record_table
 
     def create_plotly_monitoring_html_plot(
         self,
         html_filename: str,
         plot_query_begin_jd: float,
         plot_query_end_jd: float,
         plot_lower_zero_point: float = None,
         plot_upper_zero_point: float = None,
         include_plotlyjs: str = True,
+        using_timezone: str = None,
     ) -> None:
         """This function creates the monitoring plot for the monitoring
         service webpage. It plots data from the zero point database depending
         on the range of times desires.
 
         Parameters
         ----------
@@ -897,26 +948,45 @@
             upper limit is not set, we default to Plotly's best judgement.
         plot_upper_zero_point : float, default = None
             This sets the upper limit of the zero point plot. If it and the
             lower limit is not set, we default to Plotly's best judgement.
         include_plotlyjs : string, default = True
             The setting for how the plotly javascript file will be included.
             Consult the plotly documentation for available options.
+        using_timezone : string, default = None
+            The timezone to use for the plot. By default, we use UTC, but,
+            a different timezone can be provided to convert to.
 
         Returns
         -------
         None
         """
         # We need to fetch the data to query. We query just a little outside
         # of the range provided so that the plots are continuous and connect
         # to points outside of the range. A day is more than enough.
         zero_point_record_table = self.query_database_between_julian_days(
             begin_jd=plot_query_begin_jd - 1, end_jd=plot_query_end_jd + 1
         )
 
+        # We convert to a different timezone if needed, else, we just add the
+        # timezones to the original simple datetime objects.
+        using_timezone = "Etc/UTC" if using_timezone is None else using_timezone
+        zprc_datetimes = zero_point_record_table["datetime"]
+        # Converting the datetimes.
+        zprc_tz_datetimes = [
+            library.conversion.datetime_timezone_1_to_timezone_2(
+                from_datetime=datetimedex,
+                from_timezone="Etc/UTC",
+                to_timezone=using_timezone,
+            )
+            for datetimedex in zprc_datetimes
+        ]
+        zero_point_record_table_timezone = copy.deepcopy(zero_point_record_table)
+        zero_point_record_table_timezone["datetime"][:] = zprc_tz_datetimes
+
         # We group similar filters into lines.
         symbol_group_table_key = "filter_name"
 
         # The color of the lines are based on the filter being observed. We
         # supply a color map so that it derives the colors from the filter
         # names themselves.
         symbol_color_table_key = "filter_name"
@@ -950,15 +1020,15 @@
         line_x_table_key = "datetime"
         line_y_table_key = "zero_point"
         line_y_error_table_key = "zero_point_error"
 
         # We make the plot here. Further visual and aesthetic formatting is
         # done below.
         fig = px.scatter(
-            zero_point_record_table.to_pandas(),
+            zero_point_record_table_timezone.to_pandas(),
             x=line_x_table_key,
             y=line_y_table_key,
             error_y=line_y_error_table_key,
             symbol=symbol_group_table_key,
             color=symbol_color_table_key,
             color_discrete_map=plot_color_map,
             custom_data=custom_data_headers,
@@ -970,19 +1040,24 @@
         # version of ISO 8601 time formatting.
         iso_8601_time_format = R"%Y-%m-%d %H:%M:%S"
         # Datetime only takes seconds as an integer.
         int_only = lambda array: [int(valuedex) for valuedex in array]
         utc_now_tuple = library.conversion.julian_day_to_full_date(
             jd=library.conversion.current_utc_to_julian_day()
         )
-        utc_now_datetime = datetime.datetime(*int_only(utc_now_tuple))
-        utc_time_string = utc_now_datetime.strftime(iso_8601_time_format)
+        utc_now_datetime = datetime.datetime(
+            *int_only(utc_now_tuple), tzinfo=zoneinfo.ZoneInfo("Etc/UTC")
+        )
+        using_timezone_zoneinfo = zoneinfo.ZoneInfo(key=using_timezone)
+        tz_time_string = utc_now_datetime.astimezone(using_timezone_zoneinfo).strftime(
+            iso_8601_time_format
+        )
         fig.update_layout(
-            title_text="Opihi Zero Point Trends (Current: {curr} UTC)".format(
-                curr=utc_time_string
+            title_text="Opihi Zero Point Trends (Current: {curr} {tz})".format(
+                curr=tz_time_string, tz=using_timezone
             )
         )
         # All datetimes should have the same formatting. We rotate it so it
         # is a little more readable.
         tick_rotation = 15
         fig.update_xaxes(tickformat=iso_8601_time_format, tickangle=tick_rotation)
 
@@ -992,15 +1067,17 @@
 
         # A unified x-axis label is a little bit more clear to understand
         # and locate because of all of the different filters (lines) which
         # are plotted.
         fig.update_layout(hovermode="x unified")
         # We also fix the x-axis and y-axis and legend title.
         fig.update_layout(
-            xaxis_title="Time", yaxis_title="Zero Point", legend_title_text="Filter"
+            xaxis_title="Time [{tz}]".format(tz=using_timezone),
+            yaxis_title="Zero Point",
+            legend_title_text="Filter",
         )
 
         # We only want to plot between the provided time range. We queried
         # outside of that range so that we could be continuous for our plot
         # lines.
         begin_datetime_tuple = library.conversion.julian_day_to_full_date(
             jd=plot_query_begin_jd
@@ -1008,14 +1085,25 @@
         end_datetime_tuple = library.conversion.julian_day_to_full_date(
             jd=plot_query_end_jd
         )
         # We use integer seconds only for the datetimes, the best way to do
         # this is to just trim off the decimal seconds.
         datetime_lower_limit = datetime.datetime(*int_only(begin_datetime_tuple))
         datetime_upper_limit = datetime.datetime(*int_only(end_datetime_tuple))
+        # The range should also be timezone aware.
+        datetime_lower_limit = library.conversion.datetime_timezone_1_to_timezone_2(
+                from_datetime=datetime_lower_limit,
+                from_timezone="Etc/UTC",
+                to_timezone=using_timezone,
+            )
+        datetime_upper_limit = library.conversion.datetime_timezone_1_to_timezone_2(
+                from_datetime=datetime_upper_limit,
+                from_timezone="Etc/UTC",
+                to_timezone=using_timezone,
+            )
         fig.update_layout(xaxis_range=[datetime_lower_limit, datetime_upper_limit])
 
         # The upper and lower zero point plot limits.
         if plot_lower_zero_point is not None and plot_upper_zero_point is not None:
             fig.update_layout(
                 yaxis_range=[plot_lower_zero_point, plot_upper_zero_point]
             )
@@ -1064,18 +1152,22 @@
 
         # The path where the html file will be saved to along with instructions
         # on how to handle the javascript file.
         html_filename = library.config.MONITOR_PLOT_HTML_FILENAME
         # And, the setting for how to handle the javascript.
         include_plotlyjs = library.config.MONITOR_PLOT_PLOTLY_JAVASCRIPT_METHOD
 
+        # The timezone which to convert to.
+        using_timezone = library.config.MONITOR_PLOT_IANA_TIMEZONE
+
         # Create the plot using this configuration parameters.
         self.create_plotly_monitoring_html_plot(
             html_filename=html_filename,
             plot_query_begin_jd=query_begin_jd,
             plot_query_end_jd=query_end_jd,
             plot_lower_zero_point=lower_zero_point,
             plot_upper_zero_point=upper_zero_point,
             include_plotlyjs=include_plotlyjs,
+            using_timezone=using_timezone,
         )
         # All done.
         return None
```

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/opihi/preprocess.py` & `OpihiExarata-2023.7.6/src/opihiexarata/opihi/preprocess.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/opihi/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/opihi/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/orbit/custom.py` & `OpihiExarata-2023.7.6/src/opihiexarata/orbit/custom.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/orbit/orbfit.py` & `OpihiExarata-2023.7.6/src/opihiexarata/orbit/orbfit.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/orbit/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/orbit/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/photometry/panstarrs.py` & `OpihiExarata-2023.7.6/src/opihiexarata/photometry/panstarrs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/photometry/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/photometry/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/propagate/polynomial.py` & `OpihiExarata-2023.7.6/src/opihiexarata/propagate/polynomial.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.8/src/opihiexarata/propagate/solution.py` & `OpihiExarata-2023.7.6/src/opihiexarata/propagate/solution.py`

 * *Files identical despite different names*

