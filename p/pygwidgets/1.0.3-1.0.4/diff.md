# Comparing `tmp/pygwidgets-1.0.3.tar.gz` & `tmp/pygwidgets-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygwidgets-1.0.3.tar", last modified: Fri Oct 29 20:33:53 2021, max compression
+gzip compressed data, was "pygwidgets-1.0.4.tar", last modified: Wed Jul  5 19:45:45 2023, max compression
```

## Comparing `pygwidgets-1.0.3.tar` & `pygwidgets-1.0.4.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-10-29 20:33:53.521068 pygwidgets-1.0.3/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      120 2018-12-25 05:37:18.000000 pygwidgets-1.0.3/MANIFEST.in
--rw-r--r--   0 irvkalb    (501) staff       (20)      530 2021-10-29 20:33:53.520770 pygwidgets-1.0.3/PKG-INFO
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      723 2021-10-14 15:58:33.000000 pygwidgets-1.0.3/README
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-10-29 20:33:53.480018 pygwidgets-1.0.3/pygwidgets/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-12 04:16:46.000000 pygwidgets-1.0.3/pygwidgets/__init__.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     5138 2021-04-07 17:43:10.000000 pygwidgets-1.0.3/pygwidgets/conf.py
--rw-rw-r--   0 irvkalb    (501) staff       (20)   135208 2021-10-26 16:28:05.000000 pygwidgets-1.0.3/pygwidgets/pygwidgets.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-10-29 20:33:53.482289 pygwidgets-1.0.3/pygwidgets.egg-info/
--rw-r--r--   0 irvkalb    (501) staff       (20)      530 2021-10-29 20:33:53.000000 pygwidgets-1.0.3/pygwidgets.egg-info/PKG-INFO
--rw-r--r--   0 irvkalb    (501) staff       (20)     2574 2021-10-29 20:33:53.000000 pygwidgets-1.0.3/pygwidgets.egg-info/SOURCES.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)        1 2021-10-29 20:33:53.000000 pygwidgets-1.0.3/pygwidgets.egg-info/dependency_links.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       12 2021-10-29 20:33:53.000000 pygwidgets-1.0.3/pygwidgets.egg-info/requires.txt
--rw-r--r--   0 irvkalb    (501) staff       (20)       27 2021-10-29 20:33:53.000000 pygwidgets-1.0.3/pygwidgets.egg-info/top_level.txt
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-10-29 20:33:53.483074 pygwidgets-1.0.3/pygwidgets_test/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    13597 2021-03-31 04:38:24.000000 pygwidgets-1.0.3/pygwidgets_test/Main_Test_pygwidgets.py
--rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pygwidgets-1.0.3/pygwidgets_test/__init__.py
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-10-29 20:33:53.503203 pygwidgets-1.0.3/pygwidgets_test/images/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      432 2018-07-05 21:35:22.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioHighOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      418 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioHighOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      429 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioHighOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      427 2018-07-05 21:36:00.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioHighOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      416 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioHighOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      426 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioHighOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      415 2018-07-05 21:35:20.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioLowOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      408 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioLowOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      405 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioLowOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      410 2018-07-05 21:37:02.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioLowOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      409 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioLowOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      404 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioLowOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      456 2018-07-05 21:35:22.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioMedOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      441 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioMedOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioMedOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      458 2018-07-05 21:37:06.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioMedOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      447 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioMedOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RadioMedOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2368 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonDisabled.png
--rwxr-xr-x   0 irvkalb    (501) staff       (20)     3954 2021-02-19 19:11:43.000000 pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2509 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     2471 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonUp.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   102101 2018-11-25 19:40:00.000000 pygwidgets-1.0.3/pygwidgets_test/images/background.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      898 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOff.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      906 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOffDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      908 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOffDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1002 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOn.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1050 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOnDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     1047 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOnDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      903 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/dragMeDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      909 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/dragMeDown.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      944 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/dragMeOver.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      907 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/dragMeUp.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      150 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/extenDisabled.png
--rw-r--r--   0 irvkalb    (501) staff       (20)    14357 2019-04-15 15:18:44.000000 pygwidgets-1.0.3/pygwidgets_test/images/frisbee.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10761 2018-11-25 20:54:12.000000 pygwidgets-1.0.3/pygwidgets_test/images/imageDown.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     9915 2018-11-25 20:51:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/imageLeft.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10572 2018-11-25 20:52:36.000000 pygwidgets-1.0.3/pygwidgets_test/images/imageRIght.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10662 2018-11-25 20:55:02.000000 pygwidgets-1.0.3/pygwidgets_test/images/imageStart.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    10078 2018-11-25 20:53:32.000000 pygwidgets-1.0.3/pygwidgets_test/images/imageUp.jpg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     3659 2018-11-15 17:42:06.000000 pygwidgets-1.0.3/pygwidgets_test/images/pythonIcon.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      146 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/sliderExtent.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      147 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/sliderExtentDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/sliderThumb.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      111 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/sliderThumbDisabled.png
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/images/testImage.png
-drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2021-10-29 20:33:53.520227 pygwidgets-1.0.3/pygwidgets_test/sounds/
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   187598 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/Anybutton.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/Coin.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   288056 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/Item.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/Jump.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   137410 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/Nextbutton.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/Warp.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    12948 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/blip.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)    18256 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/boing.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     6180 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/bonus.wav
--rwxrwxrwx   0 irvkalb    (501) staff       (20)     7890 2018-06-07 19:56:48.000000 pygwidgets-1.0.3/pygwidgets_test/sounds/dink.wav
--rw-r--r--   0 irvkalb    (501) staff       (20)       38 2021-10-29 20:33:53.521138 pygwidgets-1.0.3/setup.cfg
--rwxrwxrwx   0 irvkalb    (501) staff       (20)      745 2021-10-14 15:51:23.000000 pygwidgets-1.0.3/setup.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-05 19:45:45.676804 pygwidgets-1.0.4/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1311 2018-09-02 17:50:20.000000 pygwidgets-1.0.4/LICENSE
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      120 2018-12-25 05:37:18.000000 pygwidgets-1.0.4/MANIFEST.in
+-rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-05 19:45:45.676454 pygwidgets-1.0.4/PKG-INFO
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1708 2023-07-01 03:54:42.000000 pygwidgets-1.0.4/README
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-05 19:45:45.646501 pygwidgets-1.0.4/pygwidgets/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)       36 2018-10-12 04:16:46.000000 pygwidgets-1.0.4/pygwidgets/__init__.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     5158 2023-07-05 17:53:31.000000 pygwidgets-1.0.4/pygwidgets/conf.py
+-rw-rw-r--   0 irvkalb    (501) staff       (20)   153310 2023-06-29 18:40:42.000000 pygwidgets-1.0.4/pygwidgets/pygwidgets.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-05 19:45:45.648153 pygwidgets-1.0.4/pygwidgets.egg-info/
+-rw-r--r--   0 irvkalb    (501) staff       (20)      522 2023-07-05 19:45:45.000000 pygwidgets-1.0.4/pygwidgets.egg-info/PKG-INFO
+-rw-r--r--   0 irvkalb    (501) staff       (20)     2582 2023-07-05 19:45:45.000000 pygwidgets-1.0.4/pygwidgets.egg-info/SOURCES.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)        1 2023-07-05 19:45:45.000000 pygwidgets-1.0.4/pygwidgets.egg-info/dependency_links.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       15 2023-07-05 19:45:45.000000 pygwidgets-1.0.4/pygwidgets.egg-info/requires.txt
+-rw-r--r--   0 irvkalb    (501) staff       (20)       27 2023-07-05 19:45:45.000000 pygwidgets-1.0.4/pygwidgets.egg-info/top_level.txt
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-05 19:45:45.649037 pygwidgets-1.0.4/pygwidgets_test/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    13561 2023-05-29 17:59:51.000000 pygwidgets-1.0.4/pygwidgets_test/Main_Test_pygwidgets.py
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)        0 2018-10-12 03:03:28.000000 pygwidgets-1.0.4/pygwidgets_test/__init__.py
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-05 19:45:45.668980 pygwidgets-1.0.4/pygwidgets_test/images/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   102101 2018-11-25 19:40:00.000000 pygwidgets-1.0.4/pygwidgets_test/images/background.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      898 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      906 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      908 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1002 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1050 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     1047 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      903 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/dragMeDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      909 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/dragMeDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      944 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/dragMeOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      907 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/dragMeUp.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      150 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/extenDisabled.png
+-rw-r--r--   0 irvkalb    (501) staff       (20)    14357 2019-04-15 15:18:44.000000 pygwidgets-1.0.4/pygwidgets_test/images/frisbee.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10761 2018-11-25 20:54:12.000000 pygwidgets-1.0.4/pygwidgets_test/images/imageDown.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     9915 2018-11-25 20:51:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/imageLeft.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10572 2018-11-25 20:52:36.000000 pygwidgets-1.0.4/pygwidgets_test/images/imageRight.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10662 2018-11-25 20:55:02.000000 pygwidgets-1.0.4/pygwidgets_test/images/imageStart.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    10078 2018-11-25 20:53:32.000000 pygwidgets-1.0.4/pygwidgets_test/images/imageUp.jpg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     3659 2018-11-15 17:42:06.000000 pygwidgets-1.0.4/pygwidgets_test/images/pythonIcon.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      432 2018-07-05 21:35:22.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioHighOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      418 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioHighOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      429 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioHighOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      427 2018-07-05 21:36:00.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioHighOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      416 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioHighOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      426 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioHighOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      415 2018-07-05 21:35:20.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioLowOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      408 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioLowOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      405 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioLowOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      410 2018-07-05 21:37:02.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioLowOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      409 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioLowOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      404 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioLowOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      456 2018-07-05 21:35:22.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioMedOff.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      441 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioMedOffDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioMedOffDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      458 2018-07-05 21:37:06.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioMedOn.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      447 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioMedOnDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      451 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/radioMedOnDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2368 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/restartButtonDisabled.png
+-rwxr-xr-x   0 irvkalb    (501) staff       (20)     3954 2021-02-19 19:11:43.000000 pygwidgets-1.0.4/pygwidgets_test/images/restartButtonDown.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2509 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/restartButtonOver.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     2471 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/restartButtonUp.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      146 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/sliderExtent.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      147 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/sliderExtentDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/sliderThumb.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      111 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/sliderThumbDisabled.png
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      110 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/images/testImage.png
+drwxr-xr-x   0 irvkalb    (501) staff       (20)        0 2023-07-05 19:45:45.675840 pygwidgets-1.0.4/pygwidgets_test/sounds/
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   187598 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/Anybutton.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/Coin.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   288056 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/Item.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/Jump.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   137410 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/Nextbutton.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)   192056 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/Warp.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    12948 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/blip.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)    18256 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/boing.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     6180 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/bonus.wav
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)     7890 2018-06-07 19:56:48.000000 pygwidgets-1.0.4/pygwidgets_test/sounds/dink.wav
+-rw-r--r--   0 irvkalb    (501) staff       (20)       38 2023-07-05 19:45:45.676916 pygwidgets-1.0.4/setup.cfg
+-rwxrwxrwx   0 irvkalb    (501) staff       (20)      748 2023-03-16 20:30:00.000000 pygwidgets-1.0.4/setup.py
```

### Comparing `pygwidgets-1.0.3/PKG-INFO` & `pygwidgets-1.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pygwidgets
-Version: 1.0.3
+Version: 1.0.4
 Summary: User interface widgets for use with Pygame
 Home-page: https://github.com/IrvKalb/pygwidgets
 Author: Irv Kalb
 Author-email: Irv@furrypants.com
 License: BSD
-Description: User interface widgets for building programs using Pygame
 Keywords: pygame widgets user interface buttons text dragger animation image
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+User interface widgets for building programs using Pygame
```

### Comparing `pygwidgets-1.0.3/pygwidgets/conf.py` & `pygwidgets-1.0.4/pygwidgets/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 
 import os
 import sys
 
-print('Inserting this into the os search path', os.path.join(os.path.dirname(__file__)), 'pygwidgets')
+print('Inserting this into the os search path', os.path.dirname(__file__))
+print()
 
-sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'pygwidgets'))
+sys.path.insert(0, os.path.dirname(__file__))
 
 #print()
 #for path in sys.path:
 #    print(path)
 #print()
 
 
@@ -31,22 +32,23 @@
 project = 'pygwidgets'
 copyright = '2021, Irv Kalb'
 author = 'Irv Kalb'
 
 # The short X.Y version
 version = '1.0'
 # The full version, including alpha/beta/rc tags
-release = '1.0.3'
+release = '1.0.4'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
+toc_object_entries = False  # Added 6/23 to only show class names
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc'
 ]
@@ -66,15 +68,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
@@ -82,21 +84,21 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'classic' # sphinx_rtd_theme'
+html_theme = 'classic'  
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
-#html_theme_options = {}
+html_theme_options = {'stickysidebar': True}
 
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = [ ]  # was:   ['_static']   IK 8/19
```

### Comparing `pygwidgets-1.0.3/pygwidgets/pygwidgets.py` & `pygwidgets-1.0.4/pygwidgets/pygwidgets.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,75 +11,85 @@
 
 Design notes:
 
     The way that you use objects instantiated from all these classes is very similar:
     
         1. Instantiate before the big loop starts.
          
-        2. Call the object's "handleEvent" method every time through the event loop,
+        2. Call the object's "handleEvent()" method every time through the event loop, \
                 passing in the current event (from pygame).
            It  will return False most of the time,
            but returns True when something exciting happens (for example, user clicks on a button).
          
-        3. Call the "draw" method (with no arguments) to draw each widget.
+        3. Call the "draw()" method (with no arguments) to draw each widget.
          
     I have tried to make consistent keyword parameter names across classes.
 
     I have also tried to make consistent names for methods across classes
-    For example "getValue" and "setValue" are available in most classes.
+    For example "getValue()" and "setValue()" are available in most classes.
 
     When instantiating objects from these classes, you typically only need to specify a few parameters.
     The rest will use reasonable default values, but you can change them using keyword arguments.
 
 
 Each of the button widgets comes in two varieties:
 
     Text widget that is drawn using the Python's drawing tools.
 
     Custom widget where the programmer supplies their own graphics for the widget.
 
 For example, "TextButton" below builds a button from a user-supplied text string,
-whereas "CustomButton" is built to work with user-supplied custom images.
+whereas "CustomButton" is built to work with programmer-supplied custom images.
 
 
 
 pygwidgets contains the following classes:
 
-- TextButton - a button built on the fly from a user-supplied text.
+- TextButton - a button built on the fly from a programmer-supplied text.
 - CustomButton - a button where you use your own images
 
-- TextCheckBox - a checkbox built on the fly from a user-supplied text.
+- TextCheckBox - a checkbox built on the fly from a programmer-supplied text.
 - CustomCheckBox - a checkbox where you use your images
 
-- TextRadioButton - a radio button built on the fly from a user-supplied text.
+- TextRadioButton - a radio button built on the fly from a programmer-supplied text.
 - CustomRadioButton - a radio button where you use your images
 
 - DisplayText - a text field used just for output (display)
 
 - InputText - a text field intended for user input
 
 - Dragger - gives the ability to drag any screen object with the mouse
 
 - Image - simple display of an image at a location
 
-- ImageCollection - A collection of Images, any of which can be shown at one time
+- ImageCollection - A collection of Images, any one of which can be currently shown
 
-- Animation - display a set number of images, each at its own rate
-- SpriteSheetAnimation - display an animation directly from a sprite sheet
+- Animation - display an ordered set of images, each at its own rate
+
+- SpriteSheetAnimation - display an animation from a sprite sheet
   (one file made up of many images)
 
+- AnimationCollection - a collection of Animations, where you can choose which to play
+
+- SpriteSheetAnimationCollection - similar to AnimationCollections but starts with sprite sheets
+
+- SoundEffect - used for playing short sound files (typically .wav file)
+
+- BackgroundSound - used for playing longer background music (typically .mp3 files)
+
 
 Many widgets also allow the use of a callBack (a function or method to be called when an action happens)
-    Any widget that uses a callBack can be set up like this:
-          def <callBackMethodName>(self, nickName)
+    Any widget that uses a callBack can be set up like this: 
+    |      def <callBackMethodName>(self, nickName)
     When the appropriate action happens, the callBack method will be called and the nickName will be passed
     If you don't need the nickname, you can just ignore that parameter
  
 ************************************************************************************************
-
+"""
+"""
 Simplified BSD License:
 
 Copyright 2017 Irv Kalb. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are
 permitted provided that the following conditions are met:
 
@@ -106,31 +116,47 @@
 
 ******************************************************************************************
 
 
 
 History:
 
-8/14/21  Version 1.0.3
+6/23  Version 1.1
+        Added SpriteSheetAnimationCollection class
+        Added AnimationCollection class
+        TextRadioButton: Added optional color for text and circle (radio button)
+        Added ability to work with PyInstaller to create executable application
+                    (builds proper paths on-the-fly)
+        Added SoundEffect and BackgroundSound classes
+        Button classes: added activationKeysList to press a button based on any list of keys
+            (enterToActivate still works and builds the list of activation keys for you)
+        CheckBox classes: Added toggleValue() method
+        
+3/23 Version 1.0.4
+        Image - fixed two scale and rotate bugs (thanks to Lando Chan)
+        TextInput - add setLoc to work correctly when moving an input field (thanks to Renato Monteiro)
+        SpriteSheetAnimation - fixed bug in splitting images (thanks to Alex Stamps)
+        Button classes: 'soundOnClick' didn't do anything ... now plays the sound on click
+
+11/5/21  Version 1.0.3
         Changed DisplayText.setValue to also allow passing in tuple or list - displayed one element per line
         Added __all__ to define what gets imported when you import *
         Changed SpriteSheetAnimation to calculate number of columns in SpriteSheet.
         Added ImageCollection.getCurrentKey()
         Use abc module to implement abstract classes and abstract methods
         Added pygwidgets font manager to load and remember fonts
         Use pygame.custom_event to generate custom event (pygame 2.0). Replaces pygame.USEREVENT
         Added code to make callBack's work in Button, CheckBox, and RadioButtons.
         Added mew method render() to DisplayText to make this class more inheritable
         Added specific exceptions when a call raises exception
         Animation - Added getRect (since different images can be different sizes)
         Added _loadImageAndConvert for loading and converting alpha of all images
-        Changes to InputText:
-            Added giveFocus() to programmatically give focus to one field
-            Added keepFocusOnSubmit keyword param, to allow field to keep focus programmatically
-            Added setNextFieldOnTab - to allow tabbing through InputText fields
+        InputText - Added giveFocus() to programmatically give focus to one field
+        InputText - Added keepFocusOnSubmit keyword param, to allow field to keep focus programmatically
+        InputText - Added setNextFieldOnTab - to allow tabbing through InputText fields
 
 5/26/20  Version 1.0.2
         Rewrote PygButton to be a state machine - much cleaner
         Added __version__  and function  getVersion()
 
 4/26/20  Minor documentation changes for handleEvent in a few classes
 
@@ -147,29 +173,28 @@
     to indicate that the object should show no image.
     Added Image and ImageCollection to recognize clicks by adding handleEvents method
 
 7/18   Added ability for all appropriate widgets to allow an optional callBack
     Changed "textButton" in Button, CheckBox, and RadioButton to "text"
     Change "label" to "nickname" in all widgets.
 
-
 6/18   Added Animation and SpriteSheetAnimation
 
 6/18   Added getRect (removed copy from Dragger and Image)
     In TextButton, changed param 'label' to 'text' to avoid confusion with superclass
 
 5/18   Added Image object.  Allows you to set a loc and window at the instantiation.
     That way, all you need to do to show the image is to call its draw method.
 
 1/18   Changed Button->TexButton, CheckBox->TextCheckBox, RadioButton->TextRadioButton
     Changed SetVisible->show, setInVisible->hide
     Created PygWidget base class, and have all classes inherit from it
     initializes and contains: nickname, visible, isEnabled
 
-11/17  Added Dragger, changed main "surface" to "window"  Irv Kalb
+11/17  Added Dragger, changed main "surface" to "window"  
     Changed 'caption' in the Button class to 'nickname', made it a positional parameter
     (instead of optional keyword param)
     Added 'nickname' and getNickname method to most classes
     Modified Button to grow to fit very long nicknames - defaults to minimum of 100 pixels.
     Added setPos to DisplayText 
 
 4/17  Version 1.1 by Irv Kalb
@@ -239,14 +264,16 @@
 The views and conclusions contained in the software and documentation are those of the
 authors and should not be interpreted as representing official policies, either expressed
 or implied, of Al Sweigart.
 """
 
 __all__ = [
     'Animation',
+    'AnimationCollection',
+    'BackgroundSound',
     'CustomButton',
     'CustomCheckBox',
     'CustomRadioButton',
     'DisplayText',
     'Dragger',
     'Image',
     'ImageCollection',
@@ -266,26 +293,30 @@
     'PygAnimation',
     'PygWidget',
     'PygWidgetsButton',
     'PygWidgetsCheckBox',
     'PygWidgetsRadioButton',
     'PygwidgetsFontManager',
     'SpriteSheetAnimation',
+    'SpriteSheetAnimationCollection',
+    'SoundEffect',
     'TextButton',
     'TextCheckBox',
     'TextRadioButton',
 ]
 
 import pygame
 import time
 from pygame.locals import *
 from abc import ABC, abstractmethod
+import os
+import sys
 
 
-__version__ = "1.0.3"
+__version__ = "x1.1"
 
 PYGWIDGETS_BLACK = (0, 0, 0)
 PYGWIDGETS_WHITE = (255, 255, 255)
 PYGWIDGETS_DARK_GRAY = (64, 64, 64)
 PYGWIDGETS_GRAY = (128, 128, 128)
 PYGWIDGETS_DOWN_GRAY = (140, 140, 140)
 PYGWIDGETS_NORMAL_GRAY = (170, 170, 170)
@@ -294,62 +325,93 @@
 PYGWIDGETS_ANIMATION_PLAYING = 'playing'
 PYGWIDGETS_ANIMATION_PAUSED = 'paused'
 PYGWIDGETS_ANIMATION_STOPPED = 'stopped'
 if pygame.version.vernum == 1:    # gives a tuple like (2, 0, 1), check for version 1
     PYGWIDGETS_CUSTOM_EVENT = pygame.USEREVENT  # older approach
 else:  # pygame version 2 and later
     PYGWIDGETS_CUSTOM_EVENT = pygame.event.custom_type() # new in pygame 2.0
+PYGWIDGETS_MOUSE_EVENTS_DICT = (MOUSEMOTION, MOUSEBUTTONUP, MOUSEBUTTONDOWN)
 
 
 
 def getVersion():
     """Returns the current version number of the pygwidgets package"""
-    return __version__
+    version = "x1.1"
+    return version
+
+def loadImage(path):
+    """This function is used to resolve the path to an external image file, and load the contents.
+         It returns an image ready to be shown in the window.
+         It is a wrapper for the internal function _loadImageAndConvert()
+         """
+    return _loadImageAndConvert(path)
+
+def buildPathFromRelativePath(relPath):
+    """This function is needed because of the way that PyInstaller works.
+        PyInstaller creates a temp folder and stores the path in _MEIPASS
+        When running as an executable, this function modifies the path
+        to look for assets in this temporary folder, instead of the current
+        relative folder.
+    """
+    try:
+        base_path = sys._MEIPASS
+    except Exception:
+        base_path = os.path.abspath(".")
+    absolutePath = os.path.join(base_path, relPath)
+    #print('absolutePath is', absolutePath)
+    return absolutePath
 
 def _loadImageAndConvert(path):
+    # This call allows for running inside a development environment
+    # and also works when running as an application built using PyInstaller.
+    path = buildPathFromRelativePath(path)
+        
     # Internal function to load an image and convert for putting on screen
-    try:
+    try:        
         image = pygame.image.load(path)
     except:
         raise FileNotFoundError('Cannot load file: ' + path)
 
     if image.get_alpha() is None:
         image = image.convert()
         #print('Calling convert for:', path)
     else:
         image = image.convert_alpha()
         #print('Calling convert_alpha for:', path)
     return image
 
 class PygwidgetsFontManager():
-    '''
+    """
     This is an internal font manager that loads fonts for any classes that
     render text (e.g., TextButton, TextRadioButton, TextCheckBox, InputText, DisplayText)
     It keeps a cache of loaded fonts as an optimization.
-    '''
+    """
     def __init__(self):
         pygame.font.init()   # Initialize pygame's font system
-        self.__fontsLoaded = {}  # dictionary of fonts loaded for current program
+        self._fontsLoaded = {}  # dictionary of fonts loaded for current program
 
     def loadFont(self, fontName, fontSize):
         if fontName is None:   # Request to use system font
             fontKey = 'None_' + str(fontSize)
         else:
             fontKey = fontName.lower() + '_' + str(fontSize)
             
-        if fontKey in self.__fontsLoaded:  # if already loaded
-            oFont = self.__fontsLoaded[fontKey]
+        if fontKey in self._fontsLoaded:  # if already loaded
+            oFont = self._fontsLoaded[fontKey]
         else:  # not loaded yet
             # If this font is None (for default system font)
-            # or has a period (implies a file name) of a True-Type Font file:  xxx.ttf
-            if (fontName is None) or ('.' in fontName):
+            # or has a period (implies a file name) of a True-Type Font file:  xxx.ttf or .otf
+            if fontName is None:  # font file
                 oFont = pygame.font.Font(fontName, fontSize)
-            else:
+            elif '.' in fontName:  # file name with extension
+                fontName = buildPathFromRelativePath(fontName)
+                oFont = pygame.font.Font(fontName, fontSize)
+            else: # use system font
                 oFont = pygame.font.SysFont(fontName, fontSize)
-            self.__fontsLoaded[fontKey] = oFont
+            self._fontsLoaded[fontKey] = oFont
 
         return oFont
 
 # create one instance of the font manager
 _PYGWIDGETS_FONT_MANAGER = PygwidgetsFontManager()  
 
 class PygWidget(ABC):
@@ -360,20 +422,14 @@
         - ability to enable or disable any widget
         - save and retrieve a nickname associated with the widget
         - ability to get and set the loc, and get the rect of any widget
 
     """
     @abstractmethod
     def __init__(self, nickname):
-        """Initializes PygWidget.  Just sets a few key instance variables.
-
-        Parameter:
-            |   nickname - any name you want to associate with this widget
-            
-        """
         self.visible = True
         self.isEnabled = True
         self.nickname = nickname  # any nickname you want to associate with this widget
         self.dependentsList = [] # list of objects are depend on this object (for enabled/disabled)
         self.enableDependents = False
         self.rect = pygame.Rect(0, 0, 0, 0)
         self.loc = (0, 0)
@@ -421,69 +477,93 @@
         self.rect[0] = self.loc[0]
         self.rect[1] = self.loc[1]
 
     def getLoc(self):
         """Returns the location of this widget as a tuple of values (X,Y) ."""
         return self.loc
 
+    def setCenteredLoc(self, loc):
+        """Sets a new location for this widget.  loc is a tuple of X and Y values (X, Y)
+            But it sets the center of the image of this widget to the X,Y position
+            It also changes the rect of the widget
+
+        Parameter:
+            |   loc - a tuple of X,Y coordinates
+
+        """
+        thisRect = self.getRect()
+        xOffset = thisRect.width // 2
+        yOffset = thisRect.height // 2
+        newLoc = [loc[0] - xOffset, loc[1] - yOffset]
+        self.setLoc(newLoc)
+
+
     def getRect(self):
         """Returns the rect of this widget."""
         return self.rect
 
     # Left in for historical reasons
     def overlaps(self, otherRect):
         collided = otherRect.colliderect(self.rect)
         return collided
 
     def overlapsRect(self, otherRect):
         """Returns True if the rect object overlaps another rect
+
         Parameter:
             |   otherRect - a second rectangle to compare to           
 
         """
+        
         overlaps = self.rect.colliderect(otherRect)
         return overlaps
 
     def overlapsObject(self, oOther):
-        """Returns True if the rect of this object
-        overlaps with rect of another pygwidgets object
+        """Returns True if the rect of this object overlaps with rect of another pygwidgets object
+        
         Parameter:
             |    oOther - a second object to compare to           
 
         """
+        
         otherRect = oOther.getRect()
         overlaps = self.rect.colliderect(otherRect)
         return overlaps
 
     def getX(self):
         return self.rect.left
 
     def getY(self):
         return self.rect.top
 
     def moveX(self, nPixels):
         """Move some number of pixels in the X direction
+
         Parameter:
             |    nPixels - the number of pixels to move           
 
         """
+        
         self.loc = (self.loc[0] + nPixels, self.loc[1])
         self.rect.left = self.loc[0]
 
     def moveY(self, nPixels):
         """Move some number of pixels in the Y direction
+
         Parameter:
             |    nPixels - the number of pixels to move           
 
         """
+        
         self.loc = (self.loc[0], self.loc[1] + nPixels)
         self.rect.top = self.loc[1]
 
     def moveXY(self, nPixelsX, nPixelsY):
         """Move some number of pixels in the X and Y directions
+
         Parameters:
             |    nPixelsX - the number of pixels to move in the X direction 
             |    nPixelsY - the number of pixels to move in the Y direction       
 
         """
 
         self.moveX(nPixelsX)
@@ -531,38 +611,47 @@
     STATE_IDLE = 'idle'
     STATE_ARMED = 'armed'
     STATE_DISARMED = 'disarmed'
     STATE_OVER = 'OVER'
 
     @abstractmethod
     def __init__(self, window, loc, surfaceUp, surfaceOver, surfaceDown, surfaceDisabled, 
-                 theRect, soundOnClick, nickname, enterToActivate, callBack):
+                 theRect, soundOnClick, nickname, enterToActivate, callBack, activationKeysList):
 
         super().__init__(nickname)  # initialize base class
         self.window = window
         self.loc = loc
         self.surfaceUp = surfaceUp
         self.surfaceOver = surfaceOver
         self.surfaceDown = surfaceDown
         self.surfaceDisabled = surfaceDisabled
         self.rect = theRect
         self.soundOnClick = soundOnClick
         self.enterToActivate = enterToActivate
+        if self.enterToActivate:
+            self.activationKeysList = [pygame.K_RETURN, pygame.K_KP_ENTER]
+        else:
+
+            self.activationKeysList = activationKeysList
         self.callBack = callBack
 
 
         if self.soundOnClick is not None:
             self.playSoundOnClick = True
             if type(self.soundOnClick) is str:  # user specified sound path, load it here
                 pygame.mixer.init()
                 self.soundOnClick = pygame.mixer.Sound(self.soundOnClick)  # save in same instance variable
         else:
             self.playSoundOnClick = False
 
-        self.state = PygWidgetsButton.STATE_IDLE  # starting state
+        mouseLoc = pygame.mouse.get_pos()
+        if self.rect.collidepoint(mouseLoc):
+            self.state = PygWidgetsButton.STATE_OVER # rare case, but possible
+        else:
+            self.state = PygWidgetsButton.STATE_IDLE  # typical starting state
 
     def handleEvent(self, eventObj):
         """This method should be called every time through the event loop (inside the main loop).
 
         It handles showing the up, over, and down images of the button.
 
         Parameters:
@@ -574,25 +663,25 @@
 
         """
         if not self.isEnabled:
             return False
         if not self.visible:
             return False
 
-        if self.enterToActivate:
+        if self.activationKeysList is not None:
             if eventObj.type == pygame.KEYDOWN:
 
                 # Return or Enter key
-                if eventObj.key == pygame.K_RETURN:
+                if eventObj.key in (pygame.K_RETURN, pygame.K_KP_ENTER):
                     self.state = PygWidgetsButton.STATE_IDLE
                     if self.callBack is not None:
                         self.callBack(self.nickname)  # call the callBack
                     return True
 
-        if eventObj.type not in (MOUSEMOTION, MOUSEBUTTONUP, MOUSEBUTTONDOWN):
+        if eventObj.type not in PYGWIDGETS_MOUSE_EVENTS_DICT:
             # The button only cares about mouse-related events
             return False  # early exit
 
         eventPointInButtonRect = self.rect.collidepoint(eventObj.pos)
 
         if self.state == PygWidgetsButton.STATE_IDLE:
             if (eventObj.type == MOUSEMOTION) and eventPointInButtonRect:
@@ -612,16 +701,18 @@
                 self.state = PygWidgetsButton.STATE_ARMED
 
             if (eventObj.type == MOUSEMOTION) and (not eventPointInButtonRect):
                 self.state = PygWidgetsButton.STATE_IDLE
 
 
         elif self.state == PygWidgetsButton.STATE_ARMED:
-            if (eventObj.type == MOUSEBUTTONUP) and eventPointInButtonRect:
+            if (eventObj.type == MOUSEBUTTONUP) and eventPointInButtonRect:  # clicked!
                 self.state = PygWidgetsButton.STATE_OVER
+                if self.playSoundOnClick:
+                    self.soundOnClick.play()
                 if self.callBack is not None:
                     self.callBack(self.nickname)  # call the callBack
                 return True  # clicked!
 
             if (eventObj.type == MOUSEMOTION) and (not eventPointInButtonRect):
                 self.state = PygWidgetsButton.STATE_DISARMED
 
@@ -690,14 +781,15 @@
 
         myButton.draw()
 
     Parameters:
         | window - the window to draw the button in
         | loc - the location (left and top) of the button as a tuple e.g. (10, 200).
         | text - the text to show on the button
+
     Optional keyword parameters:
         | width - the width of the button (default is wide enough to fit the text)
         | height - the height of the button (default is 40)
         | textColor - the rgb color of the text. (default is black).
         | upColor - the background rgb color of the up button (default is a medium gray)
         | overColor - the background rgb color of the over button (default is a lighter gray)
         | downColor - the background rgb color of down button (default is a darker gray)
@@ -711,15 +803,15 @@
     """
 
     MINIMUM_WIDTH = 100
 
     def __init__(self, window, loc, text, width=None, height=40, textColor=PYGWIDGETS_BLACK, 
                  upColor=PYGWIDGETS_NORMAL_GRAY, overColor=PYGWIDGETS_OVER_GRAY, downColor=PYGWIDGETS_DOWN_GRAY, 
                  fontName=None, fontSize=20, soundOnClick=None, 
-                 enterToActivate=False, callBack=None, nickname=None):
+                 enterToActivate=False, callBack=None, nickname=None, activationKeysList=None):
 
         # Create the button's Surface objects.
         if nickname is None:
             nickname = text  # use the text as the internal name
         text = ' ' + text + ' '  # add padding for drawn text
         self.textColor = textColor
         self.upColor = upColor
@@ -801,15 +893,15 @@
         pygame.draw.line(surfaceDisabled, PYGWIDGETS_GRAY, (w - 1, 1), (w - 1, h - 1))
         pygame.draw.line(surfaceDisabled, PYGWIDGETS_GRAY, (2, h - 2), (w - 2, h - 2))
         pygame.draw.line(surfaceDisabled, PYGWIDGETS_GRAY, (w - 2, 2), (w - 2, h - 2))
 
         # call the PygWidgetsButton superclass to finish initialization
 
         super().__init__(window, loc, surfaceUp, surfaceOver, surfaceDown, surfaceDisabled, 
-                         buttonRect, soundOnClick, nickname, enterToActivate, callBack)
+                         buttonRect, soundOnClick, nickname, enterToActivate, callBack, activationKeysList)
 
 
 ## Older way to do the same thing:
 ##     super(TextButton, self).__init__(window, loc, surfaceUp, surfaceOver, surfaceDown, surfaceDisabled, 
 ##                   buttonRect, soundOnClick, nickname, enterToActivate)
 
 
@@ -833,37 +925,38 @@
         if myButton.handleEvent(event):  # When the button is clicked, this returns True
             #  the button was clicked, do whatever you want here
 
     3) At the bottom of your big loop, draw the button:
 
         myButton.draw()
 
-
-    The up, down, over, and disabled images must all be the same size.
     Only the up image needs to be specified. If any of the others are left out, 
-    they will default to be a copy of the up surface.
+    they will default to be a copy of the up image.  (It's recommended that you supply all four.)
 
     Parameters:
         | window - the window to draw the button in
         | loc - a tuple specifying the position (upper left corner) for the button to be drawn.
         | up - a path to a file with the button's up appearance.
+
     Optional keyword parameters:
         | down - a path to a file with the button's pushed down appearance.
         | over - a path to a file with the button's appearance when the mouse is over it.
         | disabled - a path to a file with the button's disabled appearance.
         | soundOnClick - a path to a sound effect file. Plays when the button is clicked (defaults to None)
         | enterToActivate - if user presses Enter (or Return), button will activate (default is False)
         | nickname - any name you want to use to identify this button (default is None)
         | callBack - a function or object.method to call when the button is clicked (default is None)
-    Raises FileNotFoundError if a file at a given path cannot be found
+        
+    Raises:
+        | FileNotFoundError if a file at a given path cannot be found
 
     """
 
     def __init__(self, window, loc, up, down=None, over=None, disabled=None, soundOnClick=None, 
-                 nickname=None, enterToActivate=False, callBack=None):
+                 nickname=None, enterToActivate=False, callBack=None, activationKeysList=None):
 
         # Create the button's Surface objects.
         surfaceUp = _loadImageAndConvert(up)
 
         if down is None:
             surfaceDown = surfaceUp
         else:
@@ -887,15 +980,15 @@
                 #== surfaceOver.get_size() == surfaceDisabled.get_size():
             #pass  # typical case, sizes all match
         #else:
             #raise Exception('Custom button files (starting with: ' + up + ') are not all the same size')
 
         # call the PygWidgetsButton superclass to finish initialization
         super().__init__(window, loc, surfaceUp, surfaceOver, surfaceDown, surfaceDisabled,
-                                    buttonRect, soundOnClick, nickname, enterToActivate, callBack)
+                                    buttonRect, soundOnClick, nickname, enterToActivate, callBack, activationKeysList)
 # Older way to do the same thing:
 #    super(CustomButton, self).__init__(window, loc, surfaceUp, surfaceOver, surfaceDown, surfaceDisabled,
 #                                       buttonRect, soundOnClick, nickname, enterToActivate)
 
 
 #
 #
@@ -911,15 +1004,14 @@
 
     """
 
     @abstractmethod
     def __init__(self, window, loc, theRect, 
                  surfaceOn, surfaceOff, surfaceOnDown, surfaceOffDown,
                  surfaceOnDisabled, surfaceOffDisabled, soundOnClick, value, nickname, callBack):
-        """Initializer for the PygWidgetsCheckBox base class."""
 
         super().__init__(nickname)  # initialize base class
         self.window = window
         self.loc = loc
         self.rect = theRect
         self.surfaceOn = surfaceOn
         self.surfaceOff = surfaceOff
@@ -959,15 +1051,15 @@
 
         Returns:
             | False most of the time
             | True when the user has toggled the checkbox.
 
         """
 
-        if eventObj.type not in (MOUSEMOTION, MOUSEBUTTONUP, MOUSEBUTTONDOWN) or not self.visible:
+        if eventObj.type not in PYGWIDGETS_MOUSE_EVENTS_DICT or not self.visible:
             # The checkBox only cares bout mouse-related events (or no events, if it is invisible)
             return False
 
         if not self.isEnabled:
             return False
         if not self.visible:
             return False
@@ -1053,14 +1145,19 @@
         """Returns the value of the checkbox  (True/False)."""
         return self.value
 
     def setValue(self, trueOrFalse):
         """Sets a new value for the checkBox to the value passed in."""
         self.value = trueOrFalse
 
+    def toggleValue(self):
+        """Switches the current value of a checkBox and returns the new value"""
+        self.value = not self.value
+        return self.value
+
 
 class TextCheckBox(PygWidgetsCheckBox):
     """Builds a checkbox with a default text appearance.
 
     Each TextCheckBox has six states:  on, off, onDown, offDown, onDisabled, and offDisabled
 
     Typical use:
@@ -1080,14 +1177,15 @@
 
         myCheckBox.draw()
 
     Parameters:
         | window - the window to draw the checkbox in
         | loc - a tuple specifying the upper left corner to draw the checkbox on the surface
         | text - the text for the label that appears next to the checkbox
+
     Optional keyword parameters:
         | value - True for on, False for off (default is True)
         | fontName - font to use for text, or font file, or None for system font (default is None)
         | fontSize - size of the font to use (defaults to 20)
         | size - used for both the width and the height (assuming a square box) - (default is 16 pixels)
         | edgeColor - the rgb color of the edges of the checkBox. (default is black)
         | insideColor = the rgb color of the inside of the checkBox.  (default is white)
@@ -1213,43 +1311,46 @@
     Only the on and off states need to be specified.
     If left out, the others will default to be a copy of the on and off images.
 
     Typical use:
 
     1) Create a CustomCheckBox - giving a location tuple - as (left, top) and at least two images:
 
-        myCheckBox = pygwidgets.CustomButton(window, (500, 430), 
+        myCheckBox = pygwidgets.CustomCheckBox(window, (500, 430), 
                                 on='images/CheckBoxOn.png',
-                                off='images/CheckBoxDown.png',
+                                off='images/CheckBoxOff.png',
                                 value=True)
 
     2) In your event loop, check for the button being clicked by calling its handleEvent method:
 
-        if myCheckBox.handleEvent(event):  # When clicked on to toggle, this returns True
+        if myCheckBox.handleEvent(event):  # When clicked to toggle, this returns True
             #  CheckBox was clicked, do whatever you want here
 
     3) At the bottom of your big loop, draw the checkBox:
 
         myCheckBox.draw()
 
     Parameters:
         | window - the window to draw the checkbox in
         | loc - a tuple specifying the position (upper left corner) for where the checkBox should be drawn.
         | on - a path to a file with the checkBox's on appearance.
         | off - a path to a file with the checkBox's off appearance.
+
     Optional keyword parameters:
-        | value = True for on, False for off (defaults to False)
+        | value - True for on, False for off (defaults to False)
         | onDown - a path to a file with the checkBox's appearance when the user has clicked on the on image (defaults to None)
         | offDown - a path to a file with the checkBox's appearance when the user has clicked on the off image (defaults to None)
         | onDisabled - a path to a file with the checkBox's on appearance when not clickable (defaults to None)
         | offDisabled - a path to a file with the checkBox's of appearance not clickable (defaults to None)
         | soundOnClick - a path to a sound effects file. Plays when the button is clicked (defaults to None)
         | nickname - Any nickname you want to use to identify this button (default is None)
         | callBack - a function or object.method to call when the button is clicked (default is None)
-    Raises FileNotFoundError if a file at a given path cannot be found
+        
+    Raises:
+        | FileNotFoundError if a file at a given path cannot be found
 
     """
 
     def __init__(self, window, loc, on, off, value=False, 
                  onDown=None, offDown=None, onDisabled=None, offDisabled=None,
                  soundOnClick=None, nickname=None, callBack=None):
 
@@ -1307,16 +1408,14 @@
     #     selected radioButton, when it is requested.
     __PygWidgets__Radio__Buttons__Groups__Dicts__ = {}
 
 
     @abstractmethod
     def __init__(self, window, loc, group, buttonRect, 
                  on, off, onDown, offDown, onDisabled, offDisabled, soundOnClick, value, nickname, callBack):
-        """Initializer for PygWidgetsRadioButton."""
-
 
         super().__init__(nickname)  # initialize base class
         self.window = window
         self.loc = loc
         self.group = group
         self.rect = buttonRect
         self.surfaceOn = on
@@ -1367,15 +1466,15 @@
 
         Returns:
             | False most of the time
             | True when the user selects a radio button from the group
 
         """
 
-        if eventObj.type not in (MOUSEMOTION, MOUSEBUTTONUP, MOUSEBUTTONDOWN) or not self.visible:
+        if eventObj.type not in PYGWIDGETS_MOUSE_EVENTS_DICT or not self.visible:
             # The radioButton only cares bout mouse-related events (or no events, if it is invisible)
             return False
 
         if not self.isEnabled:
             return False
         if not self.visible:
             return False
@@ -1393,15 +1492,15 @@
         if self.rect.collidepoint(eventObj.pos):
 
             if eventObj.type == MOUSEBUTTONDOWN:
                 self.buttonDown = True
                 self.lastMouseDownOverButton = True
 
         else:
-            if eventObj.type in (MOUSEBUTTONUP, MOUSEBUTTONDOWN):
+            if eventObj.type in PYGWIDGETS_MOUSE_EVENTS_DICT:
                 # if an up/down happens off the radioButton, then the next up won't cause mouseClick()
                 self.lastMouseDownOverButton = False
 
         if eventObj.type == MOUSEBUTTONDOWN:
             self.mouseIsDown = True
             
         # mouse up is handled whether or not it was over the radioButton
@@ -1441,14 +1540,23 @@
         for radioButton in radioButtonListInGroup:
             if radioButton.getValue():
                 selectedNickname = radioButton.getNickname()
                 return selectedNickname
 
         raise RuntimeError('No radio button was selected')
 
+    def setSelectedRadioButton(self):
+        """Sets this radio button on (and turns currently selected off)."""
+        radioButtonListInGroup = PygWidgetsRadioButton.__PygWidgets__Radio__Buttons__Groups__Dicts__[self.group]
+        for radioButton in radioButtonListInGroup:
+            radioButton.setValue(False)
+        self.setValue(True)
+        return
+
+
     def draw(self):
         """Draws the current state of the radio button."""
         if not self.visible:
             return
 
         # Blit the radioButton's appropriate appearance
         if self.isEnabled:
@@ -1499,15 +1607,15 @@
         self.value = trueOrFalse
 
     def getValue(self):
         """Returns the current value of the current radio button (True or False)."""
         return self.value
 
     def removeGroup(self, groupName):
-        """Removes a group of radion buttons
+        """Removes a group of radio buttons
             This could be called when leaving a page/scene, so the group is eliminated.
 
         """
         if groupName in PygWidgetsRadioButton.__PygWidgets__Radio__Buttons__Groups__Dicts__:
             PygWidgetsRadioButton.__PygWidgets__Radio__Buttons__Groups__Dicts__.pop(groupName)
         else:
             raise NameError('Attempt to removeGroup ' + groupName + 'but that group was not created.')
@@ -1540,90 +1648,94 @@
 
     Parameters:
         | window - the window to draw the radio button in
         | loc - a tuple specifying the position (upper left corner) for where the radioButton should be drawn.
         | group - a name for the group that this radio button belongs to
         |         (all radio buttons in the group need to use the same group name)
         | text - the text for a label label to appear next to the radio button
+
     Optional keyword parameters:
         | value - True for on, False for off  (defaults to False)
         | fontName - font to use for text, or font file, or None for system font (default is None)
         | fontSize - size of the font to use (defaults to 20)
         | value - True for on, False for off  (defaults to False)
         | soundOnClick - A path to a sound effect file. Plays when the button is clicked (defaults to None)
         | nickname - a nickname, which is returned when querying (see getSelectedRadioButton)
-        | callBack - a function or object.method that is called when this item is clcked (defaults to None)
+        | callBack - a function or object.method that is called when this item is clicked (defaults to None)
 
 
     """
     CIRCLE_DIAMETER = 14
     CIRCLE_LINE_WIDTH = 2
     TEXT_OFFSET = 18
 
-    def __init__(self, window, loc, group, text, value=False, fontName=None, fontSize=20, 
-                       soundOnClick=None, nickname=None, callBack=None):
+    def __init__(self, window, loc, group, text, value=False, fontName=None, fontSize=20,
+                    textColorSelected=PYGWIDGETS_BLACK, circleColorSelected=PYGWIDGETS_BLACK,
+                    textColorDeselected=PYGWIDGETS_BLACK, circleColorDeselected=PYGWIDGETS_BLACK,
+                    soundOnClick=None, nickname=None, callBack=None):
 
 
         radius = TextRadioButton.CIRCLE_DIAMETER // 2
         center = TextRadioButton.CIRCLE_DIAMETER // 2
         if nickname is None:
             nickname = text  # use the text on the button as the internal name
 
         # set up to draw the different states of the radioButton
         self.font = _PYGWIDGETS_FONT_MANAGER.loadFont(fontName, fontSize)
         self.fontHeight = self.font.size('Anything')[1]   # returns a tuple of (width, height)
 
-        lineSurfaceBlack = self.font.render(text, True, PYGWIDGETS_BLACK)
-        lineSurfaceGray = self.font.render(text, True, PYGWIDGETS_DISABLED_GRAY)
-        thisRect = lineSurfaceBlack.get_rect()
+        textSurfaceSelected = self.font.render(text, True, textColorSelected)
+        textSurfaceDeselected = self.font.render(text, True, textColorDeselected)
+        textSurfaceGray = self.font.render(text, True, PYGWIDGETS_DISABLED_GRAY)
+        thisRect = textSurfaceSelected.get_rect()
         actualWidth = thisRect.width + TextRadioButton.TEXT_OFFSET
 
         if TextRadioButton.CIRCLE_DIAMETER > self.fontHeight:
             actualHeight = TextRadioButton.CIRCLE_DIAMETER
         else:
             actualHeight = self.fontHeight
         thisRect = pygame.Rect(loc[0], loc[1], actualWidth, actualHeight)
 
         # For each state of the button, create one larger surface, then blit the circle and the text
         # Special flags are needed to set the background alpha as transparent
 
         # draw the On TextRadioButton
         surfaceOn = pygame.Surface((actualWidth, actualHeight), pygame.SRCALPHA, 32)
         pygame.draw.circle(surfaceOn, PYGWIDGETS_WHITE, (center, center), radius, 0)
-        pygame.draw.circle(surfaceOn, PYGWIDGETS_BLACK, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
-        pygame.draw.circle(surfaceOn, PYGWIDGETS_BLACK, (center, center), 3, 0)
-        surfaceOn.blit(lineSurfaceBlack, (TextRadioButton.TEXT_OFFSET, 0))
+        pygame.draw.circle(surfaceOn, circleColorSelected, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
+        pygame.draw.circle(surfaceOn, circleColorSelected, (center, center), 3, 0)
+        surfaceOn.blit(textSurfaceSelected, (TextRadioButton.TEXT_OFFSET, 0))
         surfaceOn = pygame.Surface.convert_alpha(surfaceOn)  # optimizes blitting
 
         # draw the Off TextRadioButton
         surfaceOff = pygame.Surface((actualWidth, actualHeight), pygame.SRCALPHA, 32)
         pygame.draw.circle(surfaceOff, PYGWIDGETS_WHITE, (center, center), radius, 0)
-        pygame.draw.circle(surfaceOff, PYGWIDGETS_BLACK, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
-        surfaceOff.blit(lineSurfaceBlack, (TextRadioButton.TEXT_OFFSET, 0))
+        pygame.draw.circle(surfaceOff, circleColorDeselected, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
+        surfaceOff.blit(textSurfaceDeselected, (TextRadioButton.TEXT_OFFSET, 0))
         surfaceOff = pygame.Surface.convert_alpha(surfaceOff)  # optimizes blitting
 
         # draw the onDown and offDown surfaces
         surfaceOnDown = pygame.Surface((actualWidth, actualHeight), pygame.SRCALPHA, 32)
         pygame.draw.circle(surfaceOnDown, PYGWIDGETS_GRAY, (center, center), radius, 0)
-        pygame.draw.circle(surfaceOnDown, PYGWIDGETS_BLACK, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
-        surfaceOnDown.blit(lineSurfaceBlack, (TextRadioButton.TEXT_OFFSET, 0))
+        pygame.draw.circle(surfaceOnDown, circleColorSelected, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
+        surfaceOnDown.blit(textSurfaceSelected, (TextRadioButton.TEXT_OFFSET, 0))
         surfaceOnDown = pygame.Surface.convert_alpha(surfaceOnDown)  # optimizes blitting
         surfaceOffDown = surfaceOnDown   # Copy the same surface as the onDown state
 
         # draw the OnDisabled radioButton
         surfaceOnDisabled = pygame.Surface((actualWidth, actualHeight), pygame.SRCALPHA, 32)
         pygame.draw.circle(surfaceOnDisabled, PYGWIDGETS_DISABLED_GRAY, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
         pygame.draw.circle(surfaceOnDisabled, PYGWIDGETS_DISABLED_GRAY, (center, center), 3, 0)
-        surfaceOnDisabled.blit(lineSurfaceGray, (TextRadioButton.TEXT_OFFSET, 0))
+        surfaceOnDisabled.blit(textSurfaceGray, (TextRadioButton.TEXT_OFFSET, 0))
         surfaceOnDisabled = pygame.Surface.convert_alpha(surfaceOnDisabled)  # optimizes blitting
 
         # draw the OffDisabled radioButton
         surfaceOffDisabled = pygame.Surface((actualWidth, actualHeight), pygame.SRCALPHA, 32)
         pygame.draw.circle(surfaceOffDisabled, PYGWIDGETS_DISABLED_GRAY, (center, center), radius, TextRadioButton.CIRCLE_LINE_WIDTH)
-        surfaceOffDisabled.blit(lineSurfaceGray, (TextRadioButton.TEXT_OFFSET, 0))
+        surfaceOffDisabled.blit(textSurfaceGray, (TextRadioButton.TEXT_OFFSET, 0))
         surfaceOffDisabled = pygame.Surface.convert_alpha(surfaceOffDisabled)  # optimizes blitting
 
         # call the PygWidgetsRadio superclass to initialize
         super().__init__(window, loc, group, thisRect, 
                                           surfaceOn, surfaceOff, 
                                           surfaceOnDown, surfaceOffDown, 
                                           surfaceOnDisabled, surfaceOffDisabled, 
@@ -1640,18 +1752,18 @@
     Only the on and off states need to be specified.
     If left out, the others will default to copies of the on and off surfaces.
 
     Typical use:
 
     1) Create a CustomRadioButton - giving a window, loc as (left, top), a group, and path to two images (on and off):
 
-        myRadioButton = pygwidgets.CustomButton(window, (500, 430), 
+        myRadioButton = pygwidgets.CustomRadioButton(window, (500, 430), 
                                 'MyRadioButtonGroup',
-                                'images/CheckBoxOn.png',
-                                'images/CheckBoxDown.png')
+                                'images/RadioChoice1On.png',
+                                'images/RadioChoice1Off.png')
 
     2) In your event loop, check for the radioButton being clicked by calling its handleEvent method:
 
         if myRadioButton.handleEvent(event):  # When clicked on to select, this returns True
             #  RadioButton was clicked, do whatever you want here
 
     3) At the bottom of your big loop, draw the radioButton:
@@ -1662,24 +1774,27 @@
     Parameters:
         | window - the window to draw the radio button in
         | loc - a tuple specifying the position (upper left corner) for where the radioButton should be drawn.
         | group - a name for the group that this radio button belongs to
         |         (all radio buttons in the group need to use the same group name)
         | on - a path to a file with the radioButton's on appearance.
         | off - a path to a file with the radioButton's off appearance.
+
     Optional keyword parameters:
         | value - True for selected, False for not selected (defaults to False)
         | onDown - a path to the file with the radioButton's on down appearance. (defaults to copy of on)
-        | offDown - a path to the file withthe radioButton's off down appearance.(defaults to copy of off)
+        | offDown - a path to the file with the radioButton's off down appearance.(defaults to copy of off)
         | onDisabled - a path to a file with the radioButton's on appearance when not clickable. (defaults to copy of on)
         | offDisabled - a path to a file with the radioButton's of appearance not clickable. (defaults to copy of off)
         | soundOnClick - a path to a sound effects file. Plays when the button is clicked (defaults to None)
         | nickname - a nickname, which is returned when querying (see getSelectedRadioButton)
-        | callBack - a function or object.method that is called when this item is clcked (defaults to None)
-    Raises FileNotFoundError if a file at a given path cannot be found
+        | callBack - a function or object.method that is called when this item is clicked (defaults to None)
+        
+    Raises:
+        | FileNotFoundError if a file at a given path cannot be found
 
     """
 
     def __init__(self, window, loc, group, on, off, value=False, 
                  onDown=None, offDown=None, onDisabled=None, offDisabled=None, 
                  soundOnClick=None, nickname=None, callBack=None):
 
@@ -1737,28 +1852,30 @@
     3) To show the text field in your window, call the draw method every time through the main loop:
 
            myDisplayText.draw()
 
     Parameters:
         | window - The window of the to draw the text into
         | loc - location of where the text should be drawn
+
     Optional keyword parameters:
         | value - any initial text (defaults to the empty string)
         | fontName - font to use for text, or font file, or None for system font (default is None)
         | fontSize - size of font to use (defaults to 18)
         | width - width of the input text field (defaults to width of text to draw)
         | height - height of display text field (defaults to height of text to draw)
         | textColor - rgb color of the text (default to black)
-        | backgroundColor - background rgb color of the text (defaults to white)
+        | backgroundColor - background rgb color of the text (defaults to None - transparent)
         | justified - 'left', 'center', or 'right' (defaults to 'left')
         |     Note: If you want center or right justified, you probably want to specify a width value
         |     (Otherwise, with a single text line, you will not see any difference)
         | nickname - a text name to refer to this object (defaults to None)
 
-    Raises ValueError if justified is not 'left', 'center', or 'right'
+    Raises:
+        | ValueError if justified is not 'left', 'center', or 'right'
 
 
     Inspired by a similar module written by David Clark (da_clark at shaw.ca)
     Changed parameters, defaults, methods to call, etc.
 
     """
 
@@ -1775,15 +1892,15 @@
         self.textLines = None
         self.font = _PYGWIDGETS_FONT_MANAGER.loadFont(fontName, fontSize)
         self.textColor = textColor
         self.backgroundColor = backgroundColor
         self.userHeight = height
         self.userWidth = width
         if justified not in ('left', 'center', 'right'):
-            raise ValueError('Value of justified was: ' + self.justified + '. Must be left, center, or right')
+            raise ValueError('Value of justified was: ' + justified + '. Must be left, center, or right')
         self.justified = justified
         self.textImage = None
 
         self.fontHeight = self.font.size('Anything')[1]   # returns a tuple of (width, height)
         if (height is None) and (width is None):
             self.useSpecifiedArea = False
         else:
@@ -1806,15 +1923,15 @@
             if newText == self.text:
                 return  # nothing to change
             self.text = newText
             self.textLines = newText.splitlines()
         self.render()
 
     def render(self):
-        ''' Convert the text into an image so it can be drawn in the window.'''
+        """ Convert the text into an image so it can be drawn in the window.  (Called by setValue.)"""
         nLines = len(self.textLines)
         surfacesList = []  # build up a list of surfaces, one for each line of original text
         actualWidth = 0  # will eventually be set the width of longest line
 
         for line in self.textLines:
             lineSurface = self.font.render(line, True, self.textColor)
             surfacesList.append(lineSurface)
@@ -1904,50 +2021,51 @@
 
 #
 #
 # INPUT TEXT
 #
 #
 class InputText(PygWidget):
-    """Creates a field where the user enter text (an editable field).
+    """Creates a field where the user can enter text (an editable field).
     
     Typical use:
 
     1) Create an InputText field:
 
         myInputText = pygwidgets.InputText(myWindow, (100, 200))  # Other optional arguments ...
 
-    2) In your event loop, call the 'handleEvent' method of the InputText object(s)
+    2) In your event loop, call the 'handleEvent' method of the InputText object
         It will return False most of the time, and will return True when the user presses RETURN or ENTER
         Here is the typical code to use:
 
         if myInputText.handleEvent(event):
-            theText = myInputText.getValue()  # call this method to get the text in the field
+            theText = myInputText.getValue()  # call this method to get the text the user typed in the field
             # Do whatever you want with theText
 
     3) To show the text field in your window, call the draw method every time through the main loop:
 
         myInputText.draw()
 
     Parameters:
         | window - the window to draw the text field in
         | loc - Location of where the text should be drawn
+
     Optional keyword parameters:
         | value - any initial text (defaults to the empty string)
         | fontName - font to use for text, or font file, or None for system font (default is None)
         | fontSize - size of font to use (defaults to 24)
-        | width - width of the input text field (defauls to 200 pixels)
+        | width - width of the input text field (defaults to 200 pixels)
         | textColor - rgb color of the text (default to black)
         | backgroundColor - background rgb color of the text (defaults to white)
         | focusColor - rgb color of a rectangle around the text when focused (defaults to black)
         | initialFocus - should this field have focus when at the beginning? (defaults to False)
         |       Note:  Only one field should have focus.
-        |              If more than one, all focused fields will get keys
+        |              If more than one has focus, all focused fields will get keys
         | nickname - an internal nickname for this object (defaults to None)
-        | callBack - a function or object & method to call back when user presses Enter or Return
+        | callBack - a function or object.method to call back when user presses Enter or Return
         |             (defaults to None)
         | mask - a character used to mask the text, typically set to asterisk for password field (defaults to None)
         | keepFocusOnSubmit - when user presses Return/Enter should the field keep focus (defaults to False)
 
     """
 
     #  Inspired by (and code borrowed from) NEAROO (Silas Gyger) Found on GitHub dated: 11/14/2014
@@ -2038,15 +2156,15 @@
         """
 
         if not self.isEnabled:
             return False
         if not self.visible:
             return False
 
-        if (event.type == pygame.MOUSEBUTTONDOWN) and (event.button == 1): # user clicked
+        if (event.type == MOUSEBUTTONDOWN) and (event.button == 1): # user clicked
             theX, theY = event.pos
 
             if self.imageRect.collidepoint(theX, theY):
                 if not self.focus:
                     self.focus = True   # give this field focus
                     pygame.key.set_repeat(InputText.KEY_REPEAT_DELAY, InputText.KEY_REPEAT_RATE)
                 else:
@@ -2209,67 +2327,80 @@
 
          Might want to call this (and getValue above), if there is some button to say user has finished typing
 
          """
         self.focus = False
 
     def giveFocus(self):
-        ''' Give focus to this field
+        """ Give focus to this field
         Make sure focus is removed from any previous field before calling this
-        '''
+        """
         self.focus = True
 
     def setNextFieldOnTab(self, oNextFieldOnTab):
-        ''' Allows TAB key to move to a field of programmers choice
+        """ Allows TAB key to move to a field of programmers choice
 
     Parameters:
         | oNextFieldOnTab - an InputText object that should gain focus if user hits TAB
 
-        '''
+        """
 
         self.oNextFieldOnTab = oNextFieldOnTab
 
+    def setLoc(self, loc):
+        '''Move the field to some other location'''
+        super().setLoc(loc)
+        self.imageRect = pygame.Rect(self.loc[0], self.loc[1], self.width, self.height)
+        self.rect = pygame.Rect(self.loc[0], self.loc[1], self.width, self.height)
+        # Set the rect of the focus highlight rectangle (when the text has been clicked on and has focus)
+        self.focusedImageRect = pygame.Rect(self.loc[0] - 3, self.loc[1] - 3, self.width + 6, self.height + 6)
+        self.cursorLoc = [self.loc[0], self.loc[1]]  # this is a list because element 0 will change as the user edits
+
 #
 #
 # DRAGGER
 #
 #
 class Dragger(PygWidget):
     """Dragger - Allows the user to drag an object around in the window.
 
     Typical use:
 
     1) Create a Dragger:
 
         myDragger= pygwidgets.Dragger(myWindow, (100, 200), 'images/DragMe.png')  # Other optional arguments ...
 
-    2) In your event loop, call the 'handleEvent' method of the Dragger object(s)
-        It will return False most of the time, and will return True when the user presses and lifts up on the mouse
+    2) In your event loop, call the handleEvent method of the Dragger object
+        It will return False most of the time, and will return True when the has pressed on this image and lifts up on the mouse.
         Here is the typical code to use:
 
         if myDragger.handleEvent(event):
             # print('Done dragging')  # do whatever you want here
             # Could call inherited getRect where dragger was released (and check if it is over a target)
 
-    3) To show the dragger in your window, the typical code is to call the draw method:
+    3) To show the dragger in your window, call the draw method:
 
         myDragger.draw()
 
 
     Parameters:
         | window - the window of the application for the draw method to draw into
         | loc - location of where the dragger image should be drawn
         | up -  path to up image
+
     Optional keyword parameters:
+
         | down - path to down image (defaults to None, copy of up image)
         | over -  path to over image (defaults to None, copy of up image)
         | disabled - path to disabled image (defaults to None, copy of up image)
         | nickname - any nickname you want to use to identify this dragger (defaults to None)
         | callBack - a function or method of an object to call back when done dragging (defaults to None)
-    Raises FileNotFoundError if a file at a given path cannot be found
+        
+    Raises:
+        | FileNotFoundError if a file at a given path cannot be found
 
     """    
     def __init__(self, window, loc, up, down=None, over=None, disabled=None, nickname=None, callBack=None):
 
         super().__init__(nickname)  # initialize base class
         self.window = window
         self.loc = loc
@@ -2319,15 +2450,15 @@
 
         """
         if not self.isEnabled:
             return False
         if not self.visible:
             return False
 
-        if eventObj.type not in (MOUSEMOTION, MOUSEBUTTONUP, MOUSEBUTTONDOWN) :
+        if eventObj.type not in PYGWIDGETS_MOUSE_EVENTS_DICT:
             # The dragger only cares about mouse-related events
             return False
 
         clicked = False
         if eventObj.type == MOUSEBUTTONDOWN:
             if self.rect.collidepoint(eventObj.pos):
                 self.dragging = True
@@ -2408,53 +2539,61 @@
 
     Typical use:
     
     1) Create an Image object:
 
         myImage = pygwidgets.Image(myWindow, (100, 200), 'images/SomeImage.png')
 
-        You can call the inherited getRect tmethod o get the rectangle of the image
+        You can call the inherited getRect method to get the rectangle of the image
+
+    2) (Optional) if you want to be able to check if the user clicked on an image, you can call handleEvent:
+
+        if myImage.handleEvent(eventObj):    # will return True if the user clicks on it
 
-    2) To show the Image in your window, the typical code is to call the draw method:
+    3) To show the Image in your window, the typical code is to call the draw method:
 
         myImage.draw()
 
+
     Parameters:
         | window - The window of the application so the draw method can draw into
         | loc - location of where the image should be drawn
         | pathOrLoadedImage -  path to the image (string), or an already loaded image
+
     Optional keyword parameters:
         | nickname - any nickname you want to use to identify this image (defaults to None)
-    Raises FileNotFoundError if a file at a given path cannot be found
+        
+    Raises:
+        | FileNotFoundError if a file at a given path cannot be found
 
     """
     def __init__(self, window, loc, pathOrLoadedImage, nickname=None):
 
         super().__init__(nickname)  # initialize base class
         self.window = window
         self.loc = loc
         self.angle = 0
         self.percent = 100
         self.scaleFromCenter = True
         self.flipH = False
         self.flipV = False
         self.focus = False
+        self.rect = None  # flag for first image not being loaded yet
 
         ###  SPECIAL NOTE HERE
         # In the following line of code, I want to call  the "replace" method
         # in the Image class.  Using the following call to specifically reference the "Image"
         # class makes this work correctly.  I originally had:
         #      self.replace(pathOrLoadedImage)
-        # but that failed when used inside the "ImageCollection" subclas, because it was
+        # but that failed when used inside the "ImageCollection" subclass, because it was
         # calling the "replace" method inside the ImageCollection class.
         # This solution allows both the Image and ImageCollection classes to have a method named "replace"
         Image.replace(self, pathOrLoadedImage)      # creates self.originalImage
         self.image = self.originalImage.copy()
 
-
     def replace(self, newPathOrImage):
         """replace the image with a different image.
 
         Parameters:
             | newPathOrImage - the path to the replacement image to show
             |                  if you specify the empty string(''), the image will go away
 
@@ -2465,35 +2604,30 @@
             self.originalImage = pygame.Surface(size)
             
         elif isinstance(newPathOrImage, str):
             self.originalImage = _loadImageAndConvert(newPathOrImage)
 
         else:  # must be an image
             self.originalImage = newPathOrImage
-            
-        self.image = self.originalImage.copy()
 
+        self.image = self.originalImage.copy()
+        if self.rect is None:
+            self.rect = self.image.get_rect()
+            self.rect[0] = self.loc[0]
+            self.rect[1] = self.loc[1]
 
-
-        # Set the rect of the image to appropriate values - using the current image
-        # then scale and rotate
-        self.rect = self.image.get_rect()
-        self.rect.x = self.loc[0]
-        self.rect.y = self.loc[1]
-
-        self.scale(self.percent, self.scaleFromCenter)
-        self.rotate(self.angle)
+        self._transmogrophy(self.angle, self.percent, self.scaleFromCenter, self.flipH, self.flipV)
 
     def handleEvent(self, event):
         """If you want to check for a click, this method should be called every time through the event loop.
 
         It checks to see if the user has done a mouse down on the image.
 
         Parameters:
-            | eventObj - the event object obtained by calling pygame.event.get()
+            | event - the event object obtained by calling pygame.event.get()
 
         Returns:
             | False most of the time
             | True when the user clicks down on the image.
 
         """
 
@@ -2503,15 +2637,15 @@
                 return True
             else:
                 self.focus = False
 
         return False
 
     def getFocus(self):
-        '''Returns True or False depending on if this Image has focus.'''
+        """Returns True or False depending on if this Image has focus."""
         return self.focus
 
     def flipHorizontal(self):
         """ flips an image object horizontally
         """
         
         self.flipH = not self.flipH
@@ -2551,14 +2685,15 @@
         """scales an Image object
 
         Parameters:
             | percent - a percent of the original size
             |           numbers bigger than 100 scale up
             |           numbers less than 100 scale down
             |           100 scales to the original size
+
         Optional keyword parameters:
             | scaleFromCenter - should the image scale from the center or from the upper left hand corner
             |           (default is True, scale from the center)
 
         """
         self._transmogrophy(self.angle, percent, scaleFromCenter, self.flipH, self.flipV)
 
@@ -2571,16 +2706,15 @@
 
         self.angle = angle % 360
         self.percent = percent
         self.scaleFromCenter = scaleFromCenter
 
         previousRect = self.rect
         previousCenter = previousRect.center
-        previousX = previousRect.x
-        previousY = previousRect.y
+        previousLoc = self.loc
 
         # Rotate - pygame rotates in the opposite direction
         pygameAngle = -self.angle
         # print('Pygame Transmogrophy')
         rotatedImage = pygame.transform.rotate(self.originalImage, pygameAngle)
         rotatedRect = rotatedImage.get_rect()
         rotatedWidth = rotatedRect.width
@@ -2594,40 +2728,42 @@
         # Flip
         if flipH:
             self.image = pygame.transform.flip(self.image, True, False)
         if flipV:
             self.image = pygame.transform.flip(self.image, False, True)
 
         # Placement
-
         self.rect = self.image.get_rect()
         if self.scaleFromCenter:
             self.rect.center = previousCenter
 
-        else:  # use previous X, Y
-            self.rect.x = previousX
-            self.rect.y = previousY
+        else:  # set new center based on previous X, Y
+            self.rect.center = ((previousLoc[0] + self.rect.width // 2),
+                                        (previousLoc[1] + self.rect.height // 2))
+            self.scaleFromCenter = True  # only do the above once
 
         self.setLoc((self.rect.left, self.rect.top))
 
 
+
+
     def getAngle(self):
         return self.angle
 
     def getSize(self):
         return self.image.get_size()
 
 
-    def draw(self, scrollOffsetX=0, scrollOffsetY=0):
+    def draw(self):
         """Draws the image at the given location."""
         if not self.visible:
             return
 
-        self.window.blit(self.image, (self.loc[0] - scrollOffsetX,
-                                      self.loc[1] - scrollOffsetY))
+        self.window.blit(self.image, self.loc)
+
 
 
 #
 #
 # ImageCollection
 #
 #
@@ -2657,35 +2793,38 @@
     3) To draw the current image in your window, call the draw method:
 
         myImage.draw()
 
     Parameters:
         | window - The window of the application so the draw method can draw into
         | loc - location of where the image should be drawn
-        | dictOfImages -  dictionary of key/value pairs of paths to different images
+        | imagesDict -  dictionary of key/value pairs of paths to different images
         |        Each value in the dictionary can be either a path or an image already loaded with a call to pygame.load
-        |        A key of the empty string ('') is automaticaly added to the dictOfImages - use this key to make the image go away       
+        |        A key of the empty string ('') is automatically added to the dictOfImages - use this key to make the image go away
         | startImageKey - the key of the first image to be drawn  (This image will show until replace is called)
+
     Optional keyword parameters:
         | path - any path that you want to prepend to each image  for example,
-        |        if all images are in a folder, give the relative path to that folder (defaults to empty string)
+        |        if all images are in a folder named 'images', give the relative path to that folder as 'images/' (defaults to empty string)
         | nickname - any nickname you want to use to identify this ImageCollection (defaults to None)
+
     Raises:
         | ValueError if the startImageKey is not found in the imagesDict dictionary
+        | KeyError if a call to replace() contains a key that is not in the imagesDict
         | FileNotFoundError if a file at a given path cannot be found
 
     """
 
     def __init__(self, window, loc, imagesDict, startImageKey, path='', nickname=None):
 
-
         self.window = window
         self.loc = loc
         self.percent = 100
         self.imagesDict = {}
+        self.rect = None
 
         for key, pathOrLoadedImage in imagesDict.items():
             if isinstance(pathOrLoadedImage, str):
                 fullPath = path + pathOrLoadedImage
                 image = _loadImageAndConvert(fullPath)
 
             else:
@@ -2703,47 +2842,49 @@
 
         if not (startImageKey in self.imagesDict):
             message = 'ImageCollection: The starting image key "' + startImageKey + '" was not found in the collection of images dictionary'
             raise KeyError(message)
         self.currentKey = startImageKey
         startImage = self.imagesDict[self.currentKey]
 
-        super().__init__(window, loc, startImage, nickname)  # initialize base class
+        super().__init__(window, loc, startImage, nickname)  # initialize Image base class
 
         self.percent = 100
         self.angle = 0
         self.scaleFromCenter = True
         self.originalImage = self.imagesDict[startImageKey]
         self.replace(self.currentKey)
 
 
     def replace(self, key):
         """Selects a different image to be shown.
 
         Parameters:
             | key - a key in the original dictionary that specifies which image to show
 
-        Raises KeyError if the key to use to replace an image is not found in the dictionary
+        Raises:
+            | KeyError if the key to use to replace an image is not found in the dictionary
 
         """
         if not (key in self.imagesDict):
             message = 'ImageCollection: The  key "' + key + '" was not found in the collection of images dictionary'
             raise KeyError(message)
         self.currentKey = key
         self.originalImage = self.imagesDict[self.currentKey]
         self.image = self.originalImage.copy()
 
         # Set the rect of the image to appropriate values - using the current image
         # then scale and rotate
-        self.rect = self.image.get_rect()
-        self.rect.x = self.loc[0]
-        self.rect.y = self.loc[1]
+        if self.rect is None:
+            self.rect = self.image.get_rect()
+            self.rect.x = self.loc[0]
+            self.rect.y = self.loc[1]
 
         self.scale(self.percent, self.scaleFromCenter)
-        self.rotate(self.angle)
+        self.rotateTo(self.angle)
 
     def getCurrentKey(self):
         """Returns the currently selected key in an ImageCollection"""
         return self.currentKey
 
 
 #
@@ -2758,40 +2899,42 @@
     Instead, you should instantiate either an Animation class (using multiple images)
     or a SpriteSheetAnimation (single file made up of equally spaces images).
     Details are in comments for those classes below.
 
     """
 
     @abstractmethod
-    def __init__(self, window, loc, loop, showFirstImageAtEnd, nickname, callBack, nTimes):
+    def __init__(self, window, loc, loop, showFirstImageAtEnd, nickname, callBack,
+                 nTimes):
 
         super().__init__(nickname)
-        # Iniialize instance variables common to both types of Animations
+        # Initialize instance variables common to both types of Animations
         self.window = window
         self.loc = loc
         self.loop = loop
         self.showFirstImageAtEnd = showFirstImageAtEnd
         self.nickname = nickname
         self.callBack = callBack
         self.nTimes = nTimes
 
         self.imagesList = []
         self.endTimesList = []
         self.offsetsList = []
         self.index = 0  # Used to index into all three lists
-        self.elasped = 0  # Time that has elapsed in the current animation
+        self.elapsed = 0  # Time that has elapsed in the current animation
         self.nIterationsLeft = 0
         self.state = PYGWIDGETS_ANIMATION_STOPPED
 
+
     def handleEvent(self, eventObj):
         """This method should be called every time through the event loop (inside the main loop).
 
         Returns:
-            False - if no event happens.
-            True - if the user clicks the animation to start it playing.
+            | False - if no event happens on this widget.
+            | True - if the user clicks the animation (typically to start it playing).
         """
         if not self.visible:
             return
         if not self.isEnabled:
             return False
 
         if eventObj.type != MOUSEBUTTONDOWN:
@@ -2812,33 +2955,34 @@
         """Starts an animation playing."""
         if self.state == PYGWIDGETS_ANIMATION_PLAYING:
             pass  # nothing to do
 
         elif self.state == PYGWIDGETS_ANIMATION_STOPPED:  # restart from beginning of animation
             self.index = 0  # first image in list
             self.elapsed = 0
-            self.playingStartTime = time.time()
+            self.animationPlayingStartTime = time.time()
             self.elapsedStopTime = self.endTimesList[-1]  # end of last animation image time
             self.nextElapsedThreshold = self.endTimesList[0]
             self.nIterationsLeft = self.nTimes  # typically 1
 
         elif self.state == PYGWIDGETS_ANIMATION_PAUSED:  # restart where we left off
-            self.playingStartTime = time.time() - self.elapsedAtPause  # recalc start time
+            self.animationPlayingStartTime = time.time() - self.elapsedAtPause  # recalc start time
             self.elapsed = self.elapsedAtPause
             self.elapsedStopTime = self.endTimesList[-1]  # end of last animation image time
             self.nextElapsedThreshold = self.endTimesList[self.index]
 
         self.state = PYGWIDGETS_ANIMATION_PLAYING
 
     # Leaving in for historical reasons.  (Old programs called "play")
     def play(self):
+        """Same as start()"""
         self.start()
 
     def stop(self):
-        """Stops a a playing animation.  A subsequent call to play will start from the beginning."""
+        """Stops a a playing animation.  A subsequent call to start will play from the beginning."""
         if self.state == PYGWIDGETS_ANIMATION_PLAYING:
             self.index = 0  # set up for first image in list
             self.elapsed = 0
             self.nIterationsLeft = 0
 
         elif self.state == PYGWIDGETS_ANIMATION_STOPPED:
             pass  # nothing to do
@@ -2874,69 +3018,70 @@
         """
         if self.state != PYGWIDGETS_ANIMATION_PLAYING:
             return False
         returnValue = False  # typical return value
 
         # The job here is to figure out the index of the image to show
         # and the matching elapsed time threshold for the current image
-        self.elapsed = (time.time() - self.playingStartTime)
+        self.elapsed = (time.time() - self.animationPlayingStartTime)
 
         if self.elapsed > self.elapsedStopTime:  # anim finished
             if self.loop:  # restart the animation
-                self.playingStartTime = time.time()
+                self.animationPlayingStartTime = time.time()
                 self.nextElapsedThreshold = self.endTimesList[0]
                 self.index = 0
             else:  # not looping
                 self.nIterationsLeft = self.nIterationsLeft - 1
                 if self.nIterationsLeft == 0:  # done
                     self.state = PYGWIDGETS_ANIMATION_STOPPED
                     if self.callBack is not None:  # if there is a callBack
                         self.callBack(self.nickname)  # do it
                     returnValue = True  # animation has ended
 
                 else:  # another iteration - start over again
-                    self.playingStartTime = time.time()
+                    self.animationPlayingStartTime = time.time()
                     self.nextElapsedThreshold = self.endTimesList[0]
             if self.showFirstImageAtEnd:
                 self.index = 0  # show first image
             else:
                  self.index = len(self.imagesList) - 1  # show last image
 
         elif self.elapsed > self.nextElapsedThreshold:
             # Time to move on to next picture
             self.index = self.index + 1
             self.nextElapsedThreshold = self.endTimesList[self.index]
 
         return returnValue
 
-    def draw(self, scrollOffsetX=0, scrollOffsetY=0):
+    def draw(self):
         """Draws the current frame of the animation
 
         Should be called in every frame.
 
         """
         # Assumes that self.index has been set earlier (typically in update method)
         # it is used as the index of the current image/endTime/loc
         theImage = self.imagesList[self.index]  # choose the image to show
 
         if theImage is None:  # if there is no image to show
             return
 
-        if self.visible:
-            theImageOffset = self.offsetsList[self.index]
-            theLoc = ((self.loc[0] + theImageOffset[0]) - scrollOffsetX,
-                      (self.loc[1] + theImageOffset[1]) - scrollOffsetY)
-            self.window.blit(theImage, theLoc)  # show it
+        if not self.visible:
+            return
+
+        theImageOffset = self.offsetsList[self.index]
+        self.window.blit(theImage, self.loc)
+
 
     def getRect(self):
         """Returns the rect of the current animation image
         """
         theImage = self.imagesList[self.index]
         if theImage is None:
-            return pygame.rect(0, 0, 0, 0)
+            return pygame.Rect(0, 0, 0, 0)
         else:
             theRect = theImage.get_rect()
             theRect[0] = self.loc[0]
             theRect[1] = self.loc[1]
             return theRect
 
 ### For this to work correctly, I need to figure out the matching elapsedTime
@@ -3005,180 +3150,176 @@
 
     Parameters:
         | window - the window of the application for the draw method to draw into
         | loc - location of where the animation image should be drawn
         | animTuplesList -  list of tuples, where each tuple looks like this:
         |     (<path to image>, <duration>, <optional offset>)
         |     In most cases you will only need a path and a duration
+        |     The duration is in seconds, e.g., 1 for one second, or .5 for half a second
         |     If an optional offset is given, it is used as an offset from loc
 
     Optional keyword parameters:
         | autoStart - should the animation start right away (default False)
         | loop -  should the animation loop continuously (default False)
         | showFirstImageAtEnd - when an animation ends, show the first image again (default True)
+        | path - a path to be prepended to all file paths (default is the empty string)
         | nickname -  an internal name to refer to this animation (default None)
         | callBack - function or object.method to call when the animation finishes (default None)
         | nIterations - number of iterations (default 1)
 
-    Raises FileNotFoundError if a file at a given path cannot be found
+    Raises:
+        | FileNotFoundError if a file at a given path cannot be found
 
     """
 
     def __init__(self, window, loc, animTuplesList, autoStart=False, loop=False, 
-                 showFirstImageAtEnd=True, nickname=None, callBack=None, nIterations=1):
+                 showFirstImageAtEnd=True, path='', nickname=None, callBack=None,
+                 nIterations=1):
 
         # Takes incoming list of animation tuples and creates three lists:
         # 1) imagesList list of images to show (empty string means no image)
         # 2) endTimesList - list of (elapsed times) when next pic should show
         # 3) offsetsList - list of offsets from the base loc to show each image
         #             if no offset given, use (0, 0) - (most typical)
         #
         # self.state is one of:  PYGWIDGETS_ANIMATION_PLAYING, PYGWIDGETS_ANIMATION_PAUSED, PYGWIDGETS_ANIMATION_STOPPED
         # self.endTimesList is used to decide when it is time to move onto the next image
 
-        super().__init__(window, loc, loop, showFirstImageAtEnd, nickname, callBack, nIterations)
+        super().__init__(window, loc, loop, showFirstImageAtEnd, nickname, callBack,
+                         nIterations)
 
         # Load the images
         endTime = 0
         self.rect = None
         for animTuple in animTuplesList:
             picPath = animTuple[0]
             duration = animTuple[1]
             if len(animTuple) == 2:
                 self.offsetsList.append((0, 0))  # use default location - no offset
             else:
                 self.offsetsList.append(animTuple[2])  # use specific location offset
 
-            if picPath == '':
-                image = None  # special value, meaning no image to show
+            if isinstance(picPath, str):  #typical case, picPath is a string
+                if picPath == '':
+                    image = None  # special value, meaning no image to show
+                else:
+                    image = _loadImageAndConvert(path + picPath)  # normal case, load an image
+
             else:
-                image = _loadImageAndConvert(picPath)  # normal case, load an image
-                if self.rect is None:  # first time through the loop - build rect of 1st image
+                image = picPath  # assume that picPath is an pre-loaded image
+
+            if self.rect is None:  # first time through the loop - build rect of 1st image
+                if image is not None:
                     thisWidth, thisHeight = image.get_size()
                     self.rect = pygame.Rect(self.loc[0], self.loc[1], thisWidth, thisHeight)
 
             self.imagesList.append(image)
             endTime = endTime + duration
             self.endTimesList.append(endTime)
 
         if autoStart:
             self.start()  # start animation playing
 
 
-#
+
 #
 # SPRITESHEETANIMATION
 #
-#
 class SpriteSheetAnimation(PygAnimation):
     """SpriteSheetAnimation.  Use with a single file containing multiple images.
 
     Typical use:
 
     1) Create SpriteSheetAnimation specifying a number of parameters:
+        | myAnimation = pygwidgets.SpriteSheetAnimation(
+        |                         window, loc, imagePath, nImages, width, height, durationPerImage)
 
-        myAnimation = pygwidgets.SpriteSheetAnimation(
-                                window, loc, imagePath, nImages, width, height, durationPerImage)
-
-        See below for details and optional parameters.
+        | See below for details and optional parameters.
 
     2) If you want to allow clicking on the animation to start the animation playing,
-        then you need to call the handleEvent method every time through the event loop.
-        Most of the time it will return False, but will return True when the animation is clicked on
+        | then you need to call the handleEvent method every time through the event loop.
+        | Most of the time it will return False, but will return True when the animation is clicked on
 
-        if myAnimation.handleEvent(event):
-            myAnimation.start()  # tell animation to start playing when clicked on (or anything else)
+        | if myAnimation.handleEvent(event):
+        |     myAnimation.start()  # tell animation to start playing when clicked on (or anything else)
 
 
     3) In your big loop, call the update method to allow the animation to update itself in every frame.
-        It figures out when it is time to show the next image.
-        It typically returns False, but will return True when the animation finishes.
-        If you want to check for the end of the animation, you can check the returned value like this:
+        | It figures out when it is time to show the next image.
+        | It typically returns False, but will return True when the animation finishes.
+        | If you want to check for the end of the animation, you can check the returned value like this:
 
-        if myAnimation.update():
-            # Animation has finished.  Do whatever you want to do here.
+        | if myAnimation.update():
+        |     # Animation has finished.  Do whatever you want to do here.
 
-        Alternatively, if you specified a callBack, that function or method will be called
-        when the animation is finished.
+        | Alternatively, if you specified a callBack, that function or method will be called
+        | when the animation is finished.
 
     4) At the bottom of your big loop, draw the animation:
-
-
-        myAnimation.draw()
-
+        | myAnimation.draw()
 
     Parameters:
         | window - the window of the application for the draw method to draw into
-        | loc - location of where the dragger image should be drawn
+        | loc - location of where the current animation image should be drawn
         | imagePath - path to the file containing multiple images
         | nImages - total number of images in the single file
         | width - width of each individual image
         | height = height of each individual image
         | durationOrDurationsList - two options:
         |     If a single value, then all images will use this duration
         |     If a list or tuple, duration to show each image.
+
     Optional keyword parameters:
         | autoStart - should the animation start right away (default False)
         | loop -  should the animation loop continuously (default False)
-        | showFirstImageAtEnd - when an animation ends, show the firist image again (default True)
+        | showFirstImageAtEnd - when an animation ends, show the first image again (default True)
+        | path - a path to be prepended to all file paths (default is the empty string)
         | nickname -  an internal name to refer to this animation (default None)
         | callBack - function or object.method to call when the animation finishes (default None)
         | nIterations - number of iterations (default 1)
 
     Raises:
         | ValueError if the number of images and the length of the durations list don't match
         | FileNotFoundError if a file at a given path cannot be found
 
     """
 
     def __init__(self, window, loc, imagePath, nImages, width, height, durationOrDurationsList, 
-                 autoStart=False, loop=False, showFirstImageAtEnd=True,
+                 autoStart=False, loop=False, showFirstImageAtEnd=True, path='',
                  nickname=None, callBack=None, nIterations=1):
 
-        # Takes a single SpriteSheet image and breaks it up into multiple images.
-        # All images must have the same height and width, and all have the same duration
-
-        # Create three lists:
-        # 1) imagesList list of images to show (empty string means no image)
-        # 2) endTimesList - list of (elapsed times) when next pic should show
-        # 3) offsetsList - list of offsets from the base loc to show each image
-        #              if no loc given, use original loc in call (most typical)
-        #
-        # self.state is one of:
-        #  PYGWIDGETS_ANIMATION_PLAYING, PYGWIDGETS_ANIMATION_PAUSED, PYGWIDGETS_ANIMATION_STOPPED
-        # self.endTimesList is used to decide when it is time to move onto the next image
-
-        super().__init__(window, loc, loop, showFirstImageAtEnd, nickname, callBack, nIterations)
+        super().__init__(window, loc, loop, showFirstImageAtEnd, nickname, callBack,
+                         nIterations)
 
         # Create images by taking subSurfaces of the sprite sheet
         endTime = 0
         if isinstance(durationOrDurationsList, tuple) or isinstance(durationOrDurationsList, list):
             useSameDuration = False  # this is a list of durations
             if nImages != len(durationOrDurationsList):
-                raise ValueError('Number of images ' + str(nImages) + 
-                                ' and number of duration times ' + str(len(durationOrDurationsList)) + 
+                raise ValueError('In SpriteSheetAnimation, number of images ' + str(nImages) +
+                                ' and number of duration times ' + str(len(durationOrDurationsList)) +
                                 ' do not match.')
 
         else:
             useSameDuration = True  # this is a single duration
 
         self.rect = pygame.Rect(loc[0], loc[1], width, height)
 
         # Load the sprite sheet.
-        spriteSheetImage = _loadImageAndConvert(imagePath)
+        spriteSheetImage = _loadImageAndConvert(path + imagePath)
 
         # Calculate the number of columns in the starting image
         nCols = spriteSheetImage.get_width() // width
 
         # Break the starting image into subimages
         row = 0
         col = 0
         for imageNumber in range(nImages):
-            x = col * height
-            y = row * width
+            x = col * width
+            y = row * height
 
             # Create a sub-image
             subsurfaceRect = pygame.Rect(x, y, width, height)
             image = spriteSheetImage.subsurface(subsurfaceRect)
 
             self.imagesList.append(image)
             self.offsetsList.append((0, 0))  # use default location - no offsets
@@ -3194,7 +3335,287 @@
                 col = 0
                 row = row + 1
 
         # self.nextElapsedThreshold = self.endTimesList[0]  # endpoint for current image
         self.state = PYGWIDGETS_ANIMATION_STOPPED
         if autoStart:
             self.start()  # start animation playing
+
+
+class AnimationCollection(Animation):
+    """AnimationCollection - Show an animation chosen from a collection of animations.
+
+    Typical use:
+
+    1) Create an AnimationCollection object (first define some animation tuples):
+        | walkNorthTuple = (('images/walker/walkN0.png', .2), ('images/walker/walkN1.png', .1),
+        |                   ('images/walker/walkN2.png', .2), ('images/walker/walkN3.png', .2),
+        |                    ('images/walker/walkN4.png', .1), ('images/walker/walkN5.png', .2))
+        | walkEastTuple = (('images/walker/walkE0.png', .2), ('images/walker/walkE1.png', .1),
+        |                   ('images/walker/walkE2.png', .2), ('images/walker/walkE3.png', .2),
+        |                   ('images/walker/walkE4.png', .1), ('images/walker/walkE5.png', .2))
+        | walkWestTuple = (('images/walker/walkW0.png', .2), ('images/walker/walkW1.png', .1),
+        |                  ('images/walker/walkW2.png', .2), ('images/walker/walkW3.png', .2),
+        |                   ('images/walker/walkW4.png', .1), ('images/walker/walkW5.png', .2))
+        | walkSouthTuple = (('images/walker/walkS0.png', .2), ('images/walker/walkS1.png', .1),
+        |                   ('images/walker/walkS2.png', .2), ('images/walker/walkS3.png', .2),
+        |                  ('images/walker/walkS4.png', .1), ('images/walker/walkS5.png', .2))
+
+        | myAnimations = AnimationCollection(window, (10, 10),
+        |                                         {SOUTH: walkSouthTuple,
+        |                                        NORTH: walkNorthTuple,
+        |                                         WEST: walkWestTuple,
+        |                                         EAST: walkEastTuple},
+        |                                         SOUTH,
+        |                                        loop=True, autoStart=False)
+
+
+    2) To display a different animation, call the replace method, and specify the key of the animation to display:
+        | myAnimations.replace('EAST')
+
+    3) To display the current animation in your window, call the draw method:
+        | myAnimation.draw()
+
+    Parameters:
+        | window - The window of the application so the draw method can draw into
+        | loc - location of where the image should be drawn
+        | animationTuplesDict -  dictionary of key/value pairs of animations
+        |        Each entry in the tuples list is a path and a time for that image to show
+        | startImageKey - the key of the first animation to be drawn  (This image will show until replace is called)
+
+    Optional keyword parameters:
+        | path - any path that you want to prepend to each animation, for example,
+        |        if all images are in a folder named 'animations', give the relative path to that folder as 'animations/' (defaults to empty string)
+        | nickname - any nickname you want to use to identify this AnimationCollection (defaults to None)
+
+    Raises:
+        | ValueError if the startImageKey is not found in the animationsDict dictionary
+        | FileNotFoundError if a file at a given path cannot be found
+
+    """
+    def __init__(self, window, loc, animationsTuplesDict, startAnimationKey,
+                 autoStart=False, loop=False, showFirstImageAtEnd=True, path='',
+                 nickname=None, callBack=None, nIterations=1):
+        self.window = window
+        self.loc = loc
+        self.animationsDict = {}
+
+        for key, animationTuple in animationsTuplesDict.items():
+            oAnimation = Animation(self.window, self.loc, animationTuple, autoStart,
+                                              loop, showFirstImageAtEnd, path, nickname, callBack, nIterations)
+            self.animationsDict[key] = oAnimation
+
+        self.replace(startAnimationKey)
+
+    def replace(self, key):
+        """Selects a different animation to be shown.
+
+        Parameters:
+            | key - a key in the animations dictionary that specifies which animation to show
+
+        Raises:
+            | KeyError if the key to use to replace an animation is not found in the dictionary
+
+        """
+        if not (key in self.animationsDict):
+            message = 'AnimationCollection: The  key "' + key + '" was not found in the animations dictionary'
+            raise KeyError(message)
+
+        self.currentAnimationKey = key
+        self.oCurrentAnimation = self.animationsDict[self.currentAnimationKey]
+
+    def start(self):
+        self.oCurrentAnimation.start()
+
+    def stop(self):
+        self.oCurrentAnimation.stop()
+
+    def pause(self):
+        self.oCurrentAnimation.pause()
+
+    def play(self):
+        self.oCurrentAnimation.play()
+
+    def update(self):
+        self.oCurrentAnimation.update()
+
+    def getRect(self):
+        return self.oCurrentAnimation.getRect()
+
+    def setLoc(self, locTuple):
+        for key, oAnimation in self.animationsDict.items():
+            oAnimation.setLoc(locTuple)
+
+    def draw(self):
+        self.oCurrentAnimation.draw()
+
+
+class SpriteSheetAnimationCollection(AnimationCollection):
+    """SpriteSheetAnimationCollection - Show an animation chosen from a collection of sprite sheet animations.
+
+    Typical use:
+
+    1) First define a dictionary sprite sheet animation info.  Each key value pair looks like this:
+        | <someKey>:(<imagePath>, <nImages>, <width>, <height>, <durationsOrDurationsList>)
+
+        |       animationCollectionDict = {'right' : ('images/runRight.png',
+        |                                               10, 30, 40, .1),
+        |                                            'left' : ('images/characters/runLeft.png',
+        |                                              10, 30, 40, .1)}
+        |
+        | Then create a SpriteSheetAnimationCollection object with multiple sprite sheet animations
+        | myAnimCollection = pygwidgets.SpriteSheetAnimationCollection(window, (50, 50),
+        |                                       animationCollectionDict, 'right', autoStart=True, loop=True)
+
+
+    2) To display a different animation, call the replace method, and specify the key of the animation to display:
+        |
+        | myAnimCollection.replace('left')
+
+    3) To display the current animation in your window, call the draw method:
+        |
+        | myAnimCollection.draw()
+
+    Parameters:
+        | window - the window of the application for the draw method to draw into
+        | loc - location of where the current animation image should be drawn
+        | spriteSheetAnimationsDict, a dictionary of animations where each key/value pair looks like:
+        |   <someKey>:(<imagePath>, <nImages>, <width>, <height>, <durationsOrDurationsList>)
+        |    This tuple must consist of 5 elements:
+        |         imagePath - path to the file containing multiple images (element 0)
+        |         nImages - total number of images in the single file (element 1)
+        |         width - width of each individual image  (element 2)
+        |         height = height of each individual image (element 3)
+        |         durationOrDurationsList (element 4)  - two options:
+        |               If a single value, then all images will use this duration
+        |               If a list or tuple, duration to show each image.
+
+    Optional keyword parameters:
+        | autoStart - should the animation start right away (default False)
+        | loop -  should the animation loop continuously (default False)
+        | showFirstImageAtEnd - when an animation ends, show the first image again (default True)
+        | path - a path to be prepended to all file paths (default is the empty string)
+        | nickname -  an internal name to refer to this animation (default None)
+        | callBack - function or object.method to call when the animation finishes (default None)
+        | nIterations - number of iterations (default 1)
+
+    Raises:
+        | ValueError if the number of images and the length of the durations list don't match
+        | FileNotFoundError if a file at a given path cannot be found
+
+        """
+
+    def __init__(self, window, loc, spriteSheetAnimationsDict, startAnimationKey,
+                 autoStart=False, loop=False, showFirstImageAtEnd=True, path='',
+                 nickname=None, callBack=None, nIterations=1):
+        self.window = window
+        self.loc = loc
+        self.animationsDict = {}
+
+        for key, animationInfo in spriteSheetAnimationsDict.items():
+            oAnimation = SpriteSheetAnimation(self.window, self.loc,
+                                            animationInfo[0], animationInfo[1], animationInfo[2],
+                                            animationInfo[3],animationInfo[4],
+                                            autoStart, loop, showFirstImageAtEnd, path,
+                                            nickname, callBack, nIterations)
+            self.animationsDict[key] = oAnimation
+
+        self.replace(startAnimationKey)
+
+
+class SoundEffect():
+    """SoundEffect - allows you to play a short sound effect.
+         Each is typically a .wav file.
+
+    Typical use:
+
+    1) Create a SoundEffect object specifying a path to a sound effect file (.wav)
+        | crashSound = pygwidgets.SoundEffect('sounds/crash.wav')
+
+    2) To play the sound effect:
+        | crashSound.play()
+
+    Parameters:
+        | relativePath - a relative path to the sound file
+
+    Raises:
+        | FileNotFoundError if a file at a given path cannot be found
+
+    """
+    def __init__(self, relativePath):
+        fullPath = buildPathFromRelativePath(relativePath)
+        pygame.mixer.init()
+        try:
+            self.oSound = pygame.mixer.Sound(fullPath)
+        except FileNotFoundError:
+            raise FileNotFoundError(f'Trying to create SoundEffect, but the file {relativePath} count not be found')
+
+    def play(self):
+        '''Starts the sound effect playing'''
+        self.oSound.play()
+
+class BackgroundSound():
+    """BackgroundSound - allows you to play a long background file - typically music.
+           Each is typically a .mp3 file.
+
+    Typical use:
+
+    1) Create a BackgroundSound object specifying a path to a sound effect file (.wav)
+        | musicSound = pygwidgets.BackgroundSound('sounds/myMusic.mp3')
+
+    2) To play the backgroundSound:
+        | musicSound.play()
+
+    Parameters:
+          | relativePath - a relative path to the sound file
+
+    Raises:
+          | FileNotFoundError if a file at a given path cannot be found
+
+     """
+    def __init__(self, relativePath):
+        fullPath = buildPathFromRelativePath(relativePath)
+        try:
+            pygame.mixer.music.load(fullPath)
+        except FileNotFoundError:
+            raise FileNotFoundError(f'Trying create BackgroundSound, but the file: {relativePath} count not be found')
+
+        self.musicPlaying = False
+        self.musicPaused = False
+
+    def start(self, nLoops=-1, start=0.0):
+        """Starts the music playing
+
+        Parameters:
+            | nLoops - number of times to loop the music (default is -1 meaning continuously)
+            | start - how far into the music to start (default is 0.0 meaning start at the beginning)
+
+        """
+        pygame.mixer.music.play(nLoops, start)
+        self.musicPlaying = True
+
+    def play(self, nLoops=-1, start=0.0):
+        '''Starts the music playing (same as start)'''
+        pygame.mixer.music.play(nLoops, start)
+        self.musicPlaying = True
+
+    def pause(self):
+        '''If music is playing, pause the music'''
+        if self.musicPlaying:
+            pygame.mixer.music.pause()
+            self.musicPaused = True
+
+    def unPause(self):
+        '''If music is playing, but is paused, unpause the music to let it play again'''
+        if self.musicPlaying and self.musicPaused:
+            pygame.mixer.music.unpause()
+            self.musicPaused = False
+
+    def stop(self):
+        '''Stops the current music that is playing'''
+        pygame.mixer.music.stop()
+        self.musicPlaying = False
+        self.musicPaused = False
+
+    def getPlaying(self):
+        '''Returns True if the music is playing, or False if it is not'''
+        return self.musicPlaying
```

### Comparing `pygwidgets-1.0.3/pygwidgets.egg-info/PKG-INFO` & `pygwidgets-1.0.4/pygwidgets.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pygwidgets
-Version: 1.0.3
+Version: 1.0.4
 Summary: User interface widgets for use with Pygame
 Home-page: https://github.com/IrvKalb/pygwidgets
 Author: Irv Kalb
 Author-email: Irv@furrypants.com
 License: BSD
-Description: User interface widgets for building programs using Pygame
 Keywords: pygame widgets user interface buttons text dragger animation image
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+License-File: LICENSE
+
+User interface widgets for building programs using Pygame
```

### Comparing `pygwidgets-1.0.3/pygwidgets.egg-info/SOURCES.txt` & `pygwidgets-1.0.4/pygwidgets.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,21 @@
+LICENSE
 MANIFEST.in
 README
 setup.py
 pygwidgets/__init__.py
 pygwidgets/conf.py
 pygwidgets/pygwidgets.py
 pygwidgets.egg-info/PKG-INFO
 pygwidgets.egg-info/SOURCES.txt
 pygwidgets.egg-info/dependency_links.txt
 pygwidgets.egg-info/requires.txt
 pygwidgets.egg-info/top_level.txt
 pygwidgets_test/Main_Test_pygwidgets.py
 pygwidgets_test/__init__.py
-pygwidgets_test/images/RadioHighOff.png
-pygwidgets_test/images/RadioHighOffDisabled.png
-pygwidgets_test/images/RadioHighOffDown.png
-pygwidgets_test/images/RadioHighOn.png
-pygwidgets_test/images/RadioHighOnDisabled.png
-pygwidgets_test/images/RadioHighOnDown.png
-pygwidgets_test/images/RadioLowOff.png
-pygwidgets_test/images/RadioLowOffDisabled.png
-pygwidgets_test/images/RadioLowOffDown.png
-pygwidgets_test/images/RadioLowOn.png
-pygwidgets_test/images/RadioLowOnDisabled.png
-pygwidgets_test/images/RadioLowOnDown.png
-pygwidgets_test/images/RadioMedOff.png
-pygwidgets_test/images/RadioMedOffDisabled.png
-pygwidgets_test/images/RadioMedOffDown.png
-pygwidgets_test/images/RadioMedOn.png
-pygwidgets_test/images/RadioMedOnDisabled.png
-pygwidgets_test/images/RadioMedOnDown.png
-pygwidgets_test/images/RestartButtonDisabled.png
-pygwidgets_test/images/RestartButtonDown.png
-pygwidgets_test/images/RestartButtonOver.png
-pygwidgets_test/images/RestartButtonUp.png
 pygwidgets_test/images/background.jpg
 pygwidgets_test/images/checkBoxOff.png
 pygwidgets_test/images/checkBoxOffDisabled.png
 pygwidgets_test/images/checkBoxOffDown.png
 pygwidgets_test/images/checkBoxOn.png
 pygwidgets_test/images/checkBoxOnDisabled.png
 pygwidgets_test/images/checkBoxOnDown.png
@@ -44,18 +23,40 @@
 pygwidgets_test/images/dragMeDown.png
 pygwidgets_test/images/dragMeOver.png
 pygwidgets_test/images/dragMeUp.png
 pygwidgets_test/images/extenDisabled.png
 pygwidgets_test/images/frisbee.png
 pygwidgets_test/images/imageDown.jpg
 pygwidgets_test/images/imageLeft.jpg
-pygwidgets_test/images/imageRIght.jpg
+pygwidgets_test/images/imageRight.jpg
 pygwidgets_test/images/imageStart.jpg
 pygwidgets_test/images/imageUp.jpg
 pygwidgets_test/images/pythonIcon.png
+pygwidgets_test/images/radioHighOff.png
+pygwidgets_test/images/radioHighOffDisabled.png
+pygwidgets_test/images/radioHighOffDown.png
+pygwidgets_test/images/radioHighOn.png
+pygwidgets_test/images/radioHighOnDisabled.png
+pygwidgets_test/images/radioHighOnDown.png
+pygwidgets_test/images/radioLowOff.png
+pygwidgets_test/images/radioLowOffDisabled.png
+pygwidgets_test/images/radioLowOffDown.png
+pygwidgets_test/images/radioLowOn.png
+pygwidgets_test/images/radioLowOnDisabled.png
+pygwidgets_test/images/radioLowOnDown.png
+pygwidgets_test/images/radioMedOff.png
+pygwidgets_test/images/radioMedOffDisabled.png
+pygwidgets_test/images/radioMedOffDown.png
+pygwidgets_test/images/radioMedOn.png
+pygwidgets_test/images/radioMedOnDisabled.png
+pygwidgets_test/images/radioMedOnDown.png
+pygwidgets_test/images/restartButtonDisabled.png
+pygwidgets_test/images/restartButtonDown.png
+pygwidgets_test/images/restartButtonOver.png
+pygwidgets_test/images/restartButtonUp.png
 pygwidgets_test/images/sliderExtent.png
 pygwidgets_test/images/sliderExtentDisabled.png
 pygwidgets_test/images/sliderThumb.png
 pygwidgets_test/images/sliderThumbDisabled.png
 pygwidgets_test/images/testImage.png
 pygwidgets_test/sounds/Anybutton.wav
 pygwidgets_test/sounds/Coin.wav
```

### Comparing `pygwidgets-1.0.3/pygwidgets_test/Main_Test_pygwidgets.py` & `pygwidgets-1.0.4/pygwidgets_test/Main_Test_pygwidgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,103 +45,103 @@
 pygame.init()
 window = pygame.display.set_mode([WINDOW_WIDTH, WINDOW_HEIGHT])
 clock = pygame.time.Clock()  # create a clock object
 oTest = Test()
  
 # 4 - Load assets: image(s), sounds,  etc.
 oBackgroundImage = pygwidgets.Image(window, (0, 0), 'images/background.jpg')
-oDisplayTextTitle = pygwidgets.DisplayText(window, (0, 20), 'pygwidgets example by Irv Kalb', \
+oDisplayTextTitle = pygwidgets.DisplayText(window, (0, 20), 'pygwidgets example by Irv Kalb', 
                                     fontSize=36, width= 640, textColor=BLACK, justified='center')
 
-oInputTextA = pygwidgets.InputText(window, (20, 100), 'Default input text',\
+oInputTextA = pygwidgets.InputText(window, (20, 100), 'Default input text',
                                     textColor=WHITE, backgroundColor=BLACK,
                                     fontSize=24, width=250)
 
-oInputTextB = pygwidgets.InputText(window, (20, 200), initialFocus=True,\
+oInputTextB = pygwidgets.InputText(window, (20, 200), initialFocus=True,
                                     textColor=(0, 0, 255),
                                     fontSize=28)  # add: , mask='*' for passwords
 
 
-oDisplayTextA = pygwidgets.DisplayText(window, (20, 300), 'Here is some display text', \
+oDisplayTextA = pygwidgets.DisplayText(window, (20, 300), 'Here is some display text', 
                                     fontSize=24, textColor=WHITE, justified='center')
 
-oDisplayTextB = pygwidgets.DisplayText(window, (20, 400), 'Here is some display text', \
+oDisplayTextB = pygwidgets.DisplayText(window, (20, 400), 'Here is some display text', 
                                     fontSize=24, textColor=BLACK, backgroundColor=WHITE)
 
-oRestartButton = pygwidgets.CustomButton(window, (100, 430), \
+oRestartButton = pygwidgets.CustomButton(window, (100, 430), 
                                     'images/restartButtonUp.png',
                                     down='images/restartButtonDown.png',
                                     over='images/restartButtonOver.png',
                                     disabled='images/restartButtonDisabled.png',
                                     soundOnClick='sounds/blip.wav',
                                     nickname='restartButton',
                                     callBack=myFunction)  #  callBack here is not required
 
 # oCheckBoxA controls the availability the custom radio buttons
 # oCheckBoxB controls the availability of the text radio buttons
 oCheckBoxA = pygwidgets.CustomCheckBox(window, (450, 110), value=True,
-                            on='images/checkBoxOn.png', off='images/checkBoxOff.png', \
-                            onDown='images/checkBoxOnDown.png', offDown='images/checkBoxOffDown.png', \
+                            on='images/checkBoxOn.png', off='images/checkBoxOff.png', 
+                            onDown='images/checkBoxOnDown.png', offDown='images/checkBoxOffDown.png', 
                             onDisabled='images/checkBoxOnDisabled.png', offDisabled='images/checkBoxOffDisabled.png')
 
-oRadioCustom1 = pygwidgets.CustomRadioButton(window, (500, 150), 'Custom Group', \
-                            on='images/RadioLowOn.png', off='images/RadioLowOff.png', \
-                            onDown='images/RadioLowOnDown.png', offDown='images/RadioLowOffDown.png', \
-                            onDisabled='images/RadioLowOnDisabled.png', offDisabled='images/RadioLowOffDisabled.png', \
+oRadioCustom1 = pygwidgets.CustomRadioButton(window, (500, 150), 'Custom Group', 
+                            on='images/radioLowOn.png', off='images/radioLowOff.png', 
+                            onDown='images/radioLowOnDown.png', offDown='images/radioLowOffDown.png', 
+                            onDisabled='images/radioLowOnDisabled.png', offDisabled='images/radioLowOffDisabled.png', 
                             value=True, nickname='Low')
 
-oRadioCustom2 = pygwidgets.CustomRadioButton(window, (500, 190), 'Custom Group', \
-                            on='images/RadioMedOn.png', off='images/RadioMedOff.png', \
-                            onDown='images/RadioMedOnDown.png', offDown='images/RadioMedOffDown.png', \
-                            onDisabled='images/RadioMedOnDisabled.png', offDisabled='images/RadioMedOffDisabled.png', \
+oRadioCustom2 = pygwidgets.CustomRadioButton(window, (500, 190), 'Custom Group', 
+                            on='images/radioMedOn.png', off='images/radioMedOff.png', 
+                            onDown='images/radioMedOnDown.png', offDown='images/radioMedOffDown.png', 
+                            onDisabled='images/radioMedOnDisabled.png', offDisabled='images/radioMedOffDisabled.png', 
                             value=False, nickname='Med')
 
-oRadioCustom3 = pygwidgets.CustomRadioButton(window, (500, 230), 'Custom Group', \
-                            on='images/RadioHighOn.png', off='images/RadioHighOff.png', \
-                            onDown='images/RadioHighOnDown.png', offDown='images/RadioHighOffDown.png', \
-                            onDisabled='images/RadioHighOnDisabled.png', offDisabled='images/RadioHighOffDisabled.png', \
+oRadioCustom3 = pygwidgets.CustomRadioButton(window, (500, 230), 'Custom Group', 
+                            on='images/radioHighOn.png', off='images/radioHighOff.png', 
+                            onDown='images/radioHighOnDown.png', offDown='images/radioHighOffDown.png', 
+                            onDisabled='images/radioHighOnDisabled.png', offDisabled='images/radioHighOffDisabled.png', 
                             value=False, nickname='High')
 
 oCheckBoxB = pygwidgets.TextCheckBox(window, (450, 295), 'Allow Radio Buttons')
 
-oRadioText1 = pygwidgets.TextRadioButton(window, (500, 320), 'Default Group', 'Radio Text 1', \
+oRadioText1 = pygwidgets.TextRadioButton(window, (500, 320), 'Default Group', 'Radio Text 1', 
                                       value=False)
 
-oRadioText2 = pygwidgets.TextRadioButton(window, (500, 360), 'Default Group', 'Radio Text 2', \
+oRadioText2 = pygwidgets.TextRadioButton(window, (500, 360), 'Default Group', 'Radio Text 2', 
                                       value=True)
 
-oRadioText3 = pygwidgets.TextRadioButton(window, (500, 400), 'Default Group', 'Radio Text 3', \
+oRadioText3 = pygwidgets.TextRadioButton(window, (500, 400), 'Default Group', 'Radio Text 3', 
                                       value=False)
 
 oStatusButton = pygwidgets.TextButton(window, (500, 430), 'Show Status',
                                      callBack=oTest.myMethod)  # callBack here is not required
 
 oDragger = pygwidgets.Dragger(window, (300, 200), 
-                        'images/dragMeUp.png', \
-                        'images/dragMeDown.png', \
-                        'images/dragMeOver.png', \
-                        'images/dragMeDisabled.png', \
+                        'images/dragMeUp.png', 
+                        'images/dragMeDown.png', 
+                        'images/dragMeOver.png', 
+                        'images/dragMeDisabled.png', 
                         nickname='My Dragger')
 
 oPythonIcon = pygwidgets.Image(window, (15, 500), 'images/pythonIcon.png')
 
-oImageCollection = pygwidgets.ImageCollection(window, (400, 490), \
-                                {'start':'imageStart.jpg', \
-                                 'left':'imageLeft.jpg', \
-                                 'right':'imageRight.jpg', \
-                                 'up':'imageUp.jpg', \
-                                 'down':'imageDown.jpg'}, \
+oImageCollection = pygwidgets.ImageCollection(window, (400, 490), 
+                                {'start':'imageStart.jpg', 
+                                 'left':'imageLeft.jpg', 
+                                 'right':'imageRight.jpg', 
+                                 'up':'imageUp.jpg', 
+                                 'down':'imageDown.jpg'}, 
                                 'start', path='images/')
 
 oImageInstructions = pygwidgets.DisplayText(window, (400, 595), 'Click then type l, r, d, u, s, or Space')
 
 
 oIconInstructions = pygwidgets.DisplayText(window, (15, 595),
-                                          'Click then up or down arrow to resize,\n' + \
-                                          'left or right arrow to rotate, \n' + \
+                                          'Click then up or down arrow to resize,\n' + 
+                                          'left or right arrow to rotate, \n' + 
                                           'h or v to flip horizontal or vertical')
 
 oFrisbeeImage = pygwidgets.Image(window, (562, 2), 'images/frisbee.png')
 
 
 
 # 5 - Initialize variables
@@ -285,15 +285,15 @@
         oPythonIcon.scale(pct, scaleFromCenter=scaleFromCenter)
         #print('Scaling down to', pct, '%')
  
 
 
     # 8  Do any "per frame" actions
     counter = counter + 1
-    oDisplayTextA.setValue('Here is some centered display text.\n' + \
+    oDisplayTextA.setValue('Here is some centered display text.\n' + 
                          'Showing the \nnumber of frames.\nLoop counter:' + str(counter))
     oDisplayTextB.setValue('Here is some display text.  Loop counter:' + str(counter))
     
     # 9 - Clear the window
     oBackgroundImage.draw()
 
     # 10 - Draw all window elements
```

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonDisabled.png` & `pygwidgets-1.0.4/pygwidgets_test/images/restartButtonDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonDown.png` & `pygwidgets-1.0.4/pygwidgets_test/images/restartButtonDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonOver.png` & `pygwidgets-1.0.4/pygwidgets_test/images/restartButtonOver.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/RestartButtonUp.png` & `pygwidgets-1.0.4/pygwidgets_test/images/restartButtonUp.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/background.jpg` & `pygwidgets-1.0.4/pygwidgets_test/images/background.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOff.png` & `pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOff.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOffDisabled.png` & `pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOffDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOffDown.png` & `pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOffDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOn.png` & `pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOn.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOnDisabled.png` & `pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOnDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/checkBoxOnDown.png` & `pygwidgets-1.0.4/pygwidgets_test/images/checkBoxOnDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/dragMeDisabled.png` & `pygwidgets-1.0.4/pygwidgets_test/images/dragMeDisabled.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/dragMeDown.png` & `pygwidgets-1.0.4/pygwidgets_test/images/dragMeDown.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/dragMeOver.png` & `pygwidgets-1.0.4/pygwidgets_test/images/dragMeOver.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/dragMeUp.png` & `pygwidgets-1.0.4/pygwidgets_test/images/dragMeUp.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/frisbee.png` & `pygwidgets-1.0.4/pygwidgets_test/images/frisbee.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/imageDown.jpg` & `pygwidgets-1.0.4/pygwidgets_test/images/imageDown.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/imageLeft.jpg` & `pygwidgets-1.0.4/pygwidgets_test/images/imageLeft.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/imageRIght.jpg` & `pygwidgets-1.0.4/pygwidgets_test/images/imageRight.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/imageStart.jpg` & `pygwidgets-1.0.4/pygwidgets_test/images/imageStart.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/imageUp.jpg` & `pygwidgets-1.0.4/pygwidgets_test/images/imageUp.jpg`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/images/pythonIcon.png` & `pygwidgets-1.0.4/pygwidgets_test/images/pythonIcon.png`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/Anybutton.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/Anybutton.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/Coin.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/Coin.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/Item.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/Item.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/Jump.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/Jump.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/Nextbutton.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/Nextbutton.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/Warp.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/Warp.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/blip.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/blip.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/boing.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/boing.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/bonus.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/bonus.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/pygwidgets_test/sounds/dink.wav` & `pygwidgets-1.0.4/pygwidgets_test/sounds/dink.wav`

 * *Files identical despite different names*

### Comparing `pygwidgets-1.0.3/setup.py` & `pygwidgets-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import find_packages, setup
 
 setup(
     name='pygwidgets',
-    version='1.0.3',
+    version='1.0.4',
     author='Irv Kalb',
     author_email='Irv@furrypants.com',
     description='User interface widgets for use with Pygame',
     long_description='User interface widgets for building programs using Pygame',
     packages=find_packages(),
     include_package_data=True,
     license="BSD",
     url='https://github.com/IrvKalb/pygwidgets',
     install_requires=[
-        'pygame>=2.0',
+        'pygame-ce>=2.0',
         ],
     keywords="pygame widgets user interface buttons text dragger animation image",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent"
       ]
```

