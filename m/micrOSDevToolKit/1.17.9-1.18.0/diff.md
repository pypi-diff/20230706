# Comparing `tmp/micrOSDevToolKit-1.17.9.tar.gz` & `tmp/micrOSDevToolKit-1.18.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.17.9.tar", last modified: Wed Jul  5 13:47:37 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.18.0.tar", last modified: Wed Jul  5 20:26:38 2023, max compression
```

## Comparing `micrOSDevToolKit-1.17.9.tar` & `micrOSDevToolKit-1.18.0.tar`

### file list

```diff
@@ -1,215 +1,205 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:37.144945 micrOSDevToolKit-1.17.9/
--rw-r--r--   0 bnm        (501) staff       (20)      159 2023-07-05 13:46:58.000000 micrOSDevToolKit-1.17.9/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 13:47:37.144394 micrOSDevToolKit-1.17.9/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    44970 2023-07-04 21:03:33.000000 micrOSDevToolKit-1.17.9/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     9007 2023-02-23 17:12:30.000000 micrOSDevToolKit-1.17.9/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.745344 micrOSDevToolKit-1.17.9/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.758477 micrOSDevToolKit-1.17.9/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.17.9/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.17.9/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.759922 micrOSDevToolKit-1.17.9/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.805322 micrOSDevToolKit-1.17.9/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/micrOS/micropython/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.17.9/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.17.9/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.907672 micrOSDevToolKit-1.17.9/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.17.9/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-03-15 14:20:02.000000 micrOSDevToolKit-1.17.9/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.17.9/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6361 2023-06-15 14:14:20.000000 micrOSDevToolKit-1.17.9/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2475 2023-03-12 13:18:33.000000 micrOSDevToolKit-1.17.9/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6631 2023-06-28 17:39:05.000000 micrOSDevToolKit-1.17.9/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-04 18:36:50.000000 micrOSDevToolKit-1.17.9/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.17.9/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12706 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     2363 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.17.9/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.17.9/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.17.9/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.17.9/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.17.9/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-03-21 14:02:47.000000 micrOSDevToolKit-1.17.9/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-03-04 23:34:06.000000 micrOSDevToolKit-1.17.9/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-06-19 16:03:31.000000 micrOSDevToolKit-1.17.9/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-04 18:31:06.000000 micrOSDevToolKit-1.17.9/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-03-19 12:22:25.000000 micrOSDevToolKit-1.17.9/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/micrOS/source/TinyPLed.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.932855 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     6020 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Common.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5582 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5406 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Debug.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2010 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Hooks.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5232 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/InterConnect.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8402 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4715 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1705 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1901 2023-07-01 19:35:59.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8842 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LM_system.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4265 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6294 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     8881 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/SocketServer.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)    15255 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/TaskManager.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5912 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Time.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      833 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2139 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/micrOS.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     3684 2023-07-01 19:15:09.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     3355 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/urequests.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.17.9/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-03-19 12:20:54.000000 micrOSDevToolKit-1.17.9/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-03-12 13:21:42.000000 micrOSDevToolKit-1.17.9/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)   618293 2023-07-01 20:51:18.000000 micrOSDevToolKit-1.17.9/micrOS/source/pycallgraph.png
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.17.9/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.17.9/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.935723 micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 13:47:36.000000 micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     7044 2023-07-05 13:47:36.000000 micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-05 13:47:36.000000 micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-05 13:47:36.000000 micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-05 13:47:36.000000 micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-05 13:47:37.145093 micrOSDevToolKit-1.17.9/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-05 13:47:11.000000 micrOSDevToolKit-1.17.9/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.946257 micrOSDevToolKit-1.17.9/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.17.9/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.17.9/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31335 2023-07-05 12:50:59.000000 micrOSDevToolKit-1.17.9/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.17.9/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.964210 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.969369 micrOSDevToolKit-1.17.9/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.17.9/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.17.9/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.17.9/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.17.9/toolkit/micrOSdashboard.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-03-15 15:51:44.000000 micrOSDevToolKit-1.17.9/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:36.970822 micrOSDevToolKit-1.17.9/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 13:47:37.142674 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6361 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2475 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6631 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12706 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     2363 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-07-05 12:40:57.000000 micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.670099 micrOSDevToolKit-1.18.0/
+-rw-r--r--   0 bnm        (501) staff       (20)      187 2023-07-05 13:59:32.000000 micrOSDevToolKit-1.18.0/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 20:26:38.669599 micrOSDevToolKit-1.18.0/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    44970 2023-07-04 21:03:33.000000 micrOSDevToolKit-1.18.0/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     9007 2023-02-23 17:12:30.000000 micrOSDevToolKit-1.18.0/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.468115 micrOSDevToolKit-1.18.0/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.471707 micrOSDevToolKit-1.18.0/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.0/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.18.0/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.472454 micrOSDevToolKit-1.18.0/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.515114 micrOSDevToolKit-1.18.0/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/micrOS/micropython/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.18.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.18.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.578812 micrOSDevToolKit-1.18.0/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.18.0/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6056 2023-07-05 19:54:37.000000 micrOSDevToolKit-1.18.0/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8431 2023-03-12 13:10:09.000000 micrOSDevToolKit-1.18.0/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6345 2023-07-05 20:09:42.000000 micrOSDevToolKit-1.18.0/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2363 2023-07-05 20:15:58.000000 micrOSDevToolKit-1.18.0/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6631 2023-06-28 17:39:05.000000 micrOSDevToolKit-1.18.0/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11609 2023-07-05 19:28:08.000000 micrOSDevToolKit-1.18.0/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7944 2023-07-04 16:56:58.000000 micrOSDevToolKit-1.18.0/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12706 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2145 2023-03-02 19:54:55.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1592 2023-07-05 19:30:46.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8246 2023-06-14 13:32:26.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.18.0/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.18.0/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.18.0/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.18.0/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9591 2023-03-12 13:32:36.000000 micrOSDevToolKit-1.18.0/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9190 2023-03-21 14:02:47.000000 micrOSDevToolKit-1.18.0/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-03-04 23:34:06.000000 micrOSDevToolKit-1.18.0/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11616 2023-06-19 16:03:31.000000 micrOSDevToolKit-1.18.0/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19145 2023-07-04 18:31:06.000000 micrOSDevToolKit-1.18.0/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6314 2023-03-19 12:22:25.000000 micrOSDevToolKit-1.18.0/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/micrOS/source/TinyPLed.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.594724 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     6020 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Common.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5582 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5406 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Debug.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2010 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Hooks.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5232 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/InterConnect.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     8402 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4715 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1705 2023-07-01 19:36:00.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1901 2023-07-01 19:35:59.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     8842 2023-07-01 19:33:06.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LM_system.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4265 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6294 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     8881 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/SocketServer.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)    15255 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/TaskManager.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5912 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Time.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      833 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2139 2023-07-01 19:10:18.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/micrOS.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     3684 2023-07-01 19:15:09.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     3355 2023-07-01 19:26:52.000000 micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/urequests.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.18.0/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2765 2023-03-19 12:20:54.000000 micrOSDevToolKit-1.18.0/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4702 2023-03-12 13:21:42.000000 micrOSDevToolKit-1.18.0/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)   618293 2023-07-01 20:51:18.000000 micrOSDevToolKit-1.18.0/micrOS/source/pycallgraph.png
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.18.0/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4929 2023-03-17 16:35:50.000000 micrOSDevToolKit-1.18.0/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.597473 micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54517 2023-07-05 20:26:38.000000 micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     6992 2023-07-05 20:26:38.000000 micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-05 20:26:38.000000 micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-05 20:26:38.000000 micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-05 20:26:38.000000 micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-05 20:26:38.670248 micrOSDevToolKit-1.18.0/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-05 19:28:24.000000 micrOSDevToolKit-1.18.0/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.605575 micrOSDevToolKit-1.18.0/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.18.0/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24176 2023-03-09 17:49:11.000000 micrOSDevToolKit-1.18.0/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31335 2023-07-05 12:50:59.000000 micrOSDevToolKit-1.18.0/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11568 2023-01-04 20:30:41.000000 micrOSDevToolKit-1.18.0/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.622083 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.626854 micrOSDevToolKit-1.18.0/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.18.0/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.18.0/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.18.0/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.18.0/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.641599 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.667388 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-04 22:40:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6512 2023-07-04 22:40:18.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-03-15 15:51:44.000000 micrOSDevToolKit-1.18.0/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-05 20:26:38.668241 micrOSDevToolKit-1.18.0/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.18.0/toolkit/workspace/__init__.py
```

### Comparing `micrOSDevToolKit-1.17.9/PKG-INFO` & `micrOSDevToolKit-1.18.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.17.9
+Version: 1.18.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.17.9/README.md` & `micrOSDevToolKit-1.18.0/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/devToolKit.py` & `micrOSDevToolKit-1.18.0/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/media/dnd.png` & `micrOSDevToolKit-1.18.0/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/media/logo.png` & `micrOSDevToolKit-1.18.0/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/media/logo_mini.png` & `micrOSDevToolKit-1.18.0/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.18.0/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.18.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.18.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.18.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.18.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.18.0/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/Common.py` & `micrOSDevToolKit-1.18.0/micrOS/source/Common.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,36 +69,32 @@
     if len(transitions) == 1:
         return transitions[0], step_ms
     return list(transitions), step_ms
 
 
 class SmartADC:
     """
-    ADC.ATTN_0DB: 0dB attenuation, gives a maximum input voltage of 1.00v - this is the default configuration
-    ADC.ATTN_2_5DB: 2.5dB attenuation, gives a maximum input voltage of approximately 1.34v
-    ADC.ATTN_6DB: 6dB attenuation, gives a maximum input voltage of approximately 2.00v
-    ADC.ATTN_11DB: 11dB attenuation, gives a maximum input voltage of approximately 3.6v
+    ADC.ATTN_0DB: 0 dB attenuation, resulting in a full-scale voltage range of 0-1.1V
+    ADC.ATTN_2_5DB: 2.5 dB attenuation, resulting in a full-scale voltage range of 0-1.5V
+    ADC.ATTN_6DB: 6 dB attenuation, resulting in a full-scale voltage range of 0-2.2V
+    ADC.ATTN_11DB: 11 dB attenuation, resulting in a full-scale voltage range of 0-3.3V
     """
     OBJS = {}
 
     def __init__(self, pin):
         self.adc = None
         self.adp_prop = ()
         if not isinstance(pin, int):
             pin = physical_pin(pin)
-        if 'esp8266' in platform:
-            self.adc = ADC(pin)  # 1V measure range
-            self.adp_prop = (1023, 1.0)
-        else:
-            self.adc = ADC(Pin(pin))
-            self.adc.atten(ADC.ATTN_11DB)  # 3.3V measure range
-            self.adp_prop = (4095, 3.6)
+        self.adc = ADC(Pin(pin))
+        self.adc.atten(ADC.ATTN_11DB)   # 3.3V measure range
+        self.adp_prop = (4095, 3.3)
 
     def get(self):
-        raw = self.adc.read()
+        raw = self.adc.read()           # 12-bit ADC value (0-4095)
         percent = raw / self.adp_prop[0]
         volt = round(percent * self.adp_prop[1], 1)
         return {'raw': raw, 'percent': round(percent*100, 1), 'volt': volt}
 
     @staticmethod
     def get_singleton(pin):
         if pin in SmartADC.OBJS.keys():
```

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.18.0/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/Debug.py` & `micrOSDevToolKit-1.18.0/micrOS/source/Debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,20 +36,20 @@
             # Progress led for TinyPico
             DebugCfg._init_apa102()
         elif pinmap_dump('builtin')['builtin'] is not None:
             if micro_platform == "esp32s3":
                 # Progress led for esp32s3
                 DebugCfg._init_ws2812()
             else:
-                # Progress led for esp8266/esp32/etc
+                # Progress led for esp32/etc
                 DebugCfg._init_simple()
 
     @staticmethod
     def _init_simple():
-        # Progress led for esp8266/esp32/etc
+        # Progress led for esp32/etc
         DebugCfg.PLED_OBJ = Pin(physical_pin('builtin'), Pin.OUT)
 
     @staticmethod
     def _init_apa102():
         # Progress led for TinyPico
         DebugCfg.PLED_OBJ = TinyPLed.init_APA102()
```

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.18.0/micrOS/source/Hooks.py`

 * *Files 22% similar despite different names*

```diff
@@ -51,24 +51,20 @@
             console_write("|-[BOOTHOOK] DONE")
         else:
             console_write("|-[BOOTHOOK] ERROR")
 
     # Set boostmd (boost mode)
     if cfgget('boostmd') is True:
         console_write(f"[BOOT HOOKS] Set up CPU high Hz - boostmd: {cfgget('boostmd')}")
-        if detect_platform() == 'esp8266':
-            freq(160000000)
-        if detect_platform() == 'esp32':
-            freq(240000000)
+        if 'esp32' in detect_platform():
+            freq(240_000_000)   # 240 Mhz
     else:
         console_write(f"[BOOT HOOKS] Set up CPU low Hz - boostmd: {cfgget('boostmd')}")
-        if detect_platform() == 'esp8266':
-            freq(80000000)
-        if detect_platform() == 'esp32':
-            freq(80000000)
+        if 'esp32' in detect_platform():
+            freq(160_000_000)   # 160 Mhz
 
     # Scripts for file structure / config changes
     software_migration()
 
 
 def profiling_info(label=""):
     """
```

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.18.0/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.18.0/micrOS/source/InterpreterShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.17.1-2'
+    MICROS_VERSION = '1.18.0-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply_message('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.18.0/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_light_sensor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,44 @@
 """
 Source: https://how2electronics.com/temt6000-ambient-light-sensor-arduino-measure-light-intensity/
 ADC.ATTN_0DB — the full range voltage: 1.2V
 ADC.ATTN_2_5DB — the full range voltage: 1.5V
 ADC.ATTN_6DB — the full range voltage: 2.0V
 ADC.ATTN_11DB — the full range voltage: 3.3V
 """
-from sys import platform
 from LogicalPins import physical_pin, pinmap_dump
+from Common import SmartADC
 
-__ADC = None
-# [0] ADC RESOLUTION, [1] ADC VOLTAGE MEASURE RANGE
-__ADC_PROP = (1024, 1.0)
+ADC = None
 
 
 def __init_tempt6000():
     """
     Setup ADC
-    read        0(0V)-1024(1,2V) MAX 1V input on esp8266
-    read        0(0V)-1024(1,2-3,3V) input on esp32 (based on settings)
-    read_u16    0 - 65535 range
-    """
-    global __ADC, __ADC_PROP
-    if __ADC is None:
-        from machine import ADC, Pin
-        if 'esp8266' in platform:
-            __ADC = ADC(physical_pin('temp6000'))
-            __ADC_PROP = (1023, 1.0)         # Resolution on esp8266
-        else:
-            __ADC = ADC(Pin(physical_pin('temp6000')))
-            __ADC.atten(ADC.ATTN_11DB)       # 0 - 3,6V sampling range
-            __ADC_PROP = (4095, 3.6)         # Resolution on esp32
-    return __ADC
+    """
+    global ADC
+    if ADC is None:
+        ADC = SmartADC(physical_pin('temp6000'))
+    return ADC
 
 
 def intensity():
     """
     Measure light intensity in %
-    max value: 65535
     """
-    value = __init_tempt6000().read_u16()
-    percent = '{:.2f}'.format((value / 65535) * 100)
+    percent = __init_tempt6000().get()['percent']
     return {'light intensity [%]': percent}
 
 
 def illuminance():
     """
     Measure light illuminance in flux
     """
-    volts = __init_tempt6000().read() * __ADC_PROP[1] / __ADC_PROP[0]   # read a raw analog value in the range 0-ADC_RES
-    amps = volts / 10000.0                                              # across 10,000 Ohms
+    volts = __init_tempt6000().get()['volt']
+    amps = volts / 10000.0                    # across 10,000 Ohms
     microamps = amps * 1000000
     lux = '{:.2f}'.format(microamps * 2.0)
     return {'illuminance [lux]': lux}
 
 
 #######################
 # LM helper functions #
```

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.18.0/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/Network.py` & `micrOSDevToolKit-1.18.0/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/Notify.py` & `micrOSDevToolKit-1.18.0/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.18.0/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.18.0/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.18.0/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/Time.py` & `micrOSDevToolKit-1.18.0/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.18.0/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Common.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/ConfigHandler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Debug.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Debug.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Hooks.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Hooks.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/InterConnect.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/InterConnect.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/InterpreterShell.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/InterruptHandler.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LM_intercon.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LM_robustness.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LM_system.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LM_system.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/LogicalPins.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Network.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/SocketServer.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/SocketServer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/TaskManager.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/TaskManager.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/Time.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/Time.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/TinyPLed.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/micrOS.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/micrOS.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/micrOSloader.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/__pycache__/urequests.cpython-39.pyc` & `micrOSDevToolKit-1.18.0/micrOS/source/__pycache__/urequests.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.18.0/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.18.0/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/pycallgraph.png` & `micrOSDevToolKit-1.18.0/micrOS/source/pycallgraph.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOS/source/urequests.py` & `micrOSDevToolKit-1.18.0/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.17.9
+Version: 1.18.0
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.17.9/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.18.0/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -130,71 +130,60 @@
 toolkit/dashboard_apps/uLightDemo.py
 toolkit/lib/LocalMachine.py
 toolkit/lib/SearchDevices.py
 toolkit/lib/SerialDriverHandler.py
 toolkit/lib/TerminalColors.py
 toolkit/lib/__init__.py
 toolkit/lib/micrOSClient.py
-toolkit/workspace/__init__.py
-toolkit/workspace/simulator/Common.py
-toolkit/workspace/simulator/ConfigHandler.py
-toolkit/workspace/simulator/Debug.py
-toolkit/workspace/simulator/Hooks.py
-toolkit/workspace/simulator/InterConnect.py
-toolkit/workspace/simulator/InterpreterShell.py
-toolkit/workspace/simulator/InterruptHandler.py
-toolkit/workspace/simulator/LM_L298N_DCmotor.py
-toolkit/workspace/simulator/LM_L9110_DCmotor.py
-toolkit/workspace/simulator/LM_VL53L0X.py
-toolkit/workspace/simulator/LM_bme280.py
-toolkit/workspace/simulator/LM_buzzer.py
-toolkit/workspace/simulator/LM_catgame.py
-toolkit/workspace/simulator/LM_cct.py
-toolkit/workspace/simulator/LM_co2.py
-toolkit/workspace/simulator/LM_demo.py
-toolkit/workspace/simulator/LM_dht11.py
-toolkit/workspace/simulator/LM_dht22.py
-toolkit/workspace/simulator/LM_dimmer.py
-toolkit/workspace/simulator/LM_distance.py
-toolkit/workspace/simulator/LM_ds18.py
-toolkit/workspace/simulator/LM_esp32.py
-toolkit/workspace/simulator/LM_genIO.py
-toolkit/workspace/simulator/LM_i2c.py
-toolkit/workspace/simulator/LM_intercon.py
-toolkit/workspace/simulator/LM_light_sensor.py
-toolkit/workspace/simulator/LM_neoeffects.py
-toolkit/workspace/simulator/LM_neopixel.py
-toolkit/workspace/simulator/LM_oled.py
-toolkit/workspace/simulator/LM_oled_sh1106.py
-toolkit/workspace/simulator/LM_oled_ui.py
-toolkit/workspace/simulator/LM_pet_feeder.py
-toolkit/workspace/simulator/LM_ph_sensor.py
-toolkit/workspace/simulator/LM_presence.py
-toolkit/workspace/simulator/LM_rencoder.py
-toolkit/workspace/simulator/LM_rgb.py
-toolkit/workspace/simulator/LM_roboarm.py
-toolkit/workspace/simulator/LM_robustness.py
-toolkit/workspace/simulator/LM_servo.py
-toolkit/workspace/simulator/LM_stepper.py
-toolkit/workspace/simulator/LM_switch.py
-toolkit/workspace/simulator/LM_system.py
-toolkit/workspace/simulator/LM_telegram.py
-toolkit/workspace/simulator/LM_tinyrgb.py
-toolkit/workspace/simulator/LP_esp32.py
-toolkit/workspace/simulator/LP_esp32s2.py
-toolkit/workspace/simulator/LP_esp32s3.py
-toolkit/workspace/simulator/LP_rp2.py
-toolkit/workspace/simulator/LP_tinypico.py
-toolkit/workspace/simulator/LogicalPins.py
-toolkit/workspace/simulator/Network.py
-toolkit/workspace/simulator/Notify.py
-toolkit/workspace/simulator/Scheduler.py
-toolkit/workspace/simulator/SocketServer.py
-toolkit/workspace/simulator/TaskManager.py
-toolkit/workspace/simulator/Time.py
-toolkit/workspace/simulator/TinyPLed.py
-toolkit/workspace/simulator/__init__.py
-toolkit/workspace/simulator/main.py
-toolkit/workspace/simulator/micrOS.py
-toolkit/workspace/simulator/micrOSloader.py
-toolkit/workspace/simulator/reset.py
-toolkit/workspace/simulator/urequests.py
+toolkit/simulator_lib/LP_darwin.py
+toolkit/simulator_lib/dotstar.py
+toolkit/simulator_lib/ds18x20.py
+toolkit/simulator_lib/esp32.py
+toolkit/simulator_lib/framebuf.py
+toolkit/simulator_lib/machine.py
+toolkit/simulator_lib/micropython.py
+toolkit/simulator_lib/neopixel.py
+toolkit/simulator_lib/network.py
+toolkit/simulator_lib/ntptime.py
+toolkit/simulator_lib/onewire.py
+toolkit/simulator_lib/sim_console.py
+toolkit/simulator_lib/simgc.py
+toolkit/simulator_lib/simulator.py
+toolkit/simulator_lib/tinypico.py
+toolkit/simulator_lib/uasyncio.py
+toolkit/simulator_lib/utime.py
+toolkit/simulator_lib/webrepl.py
+toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+toolkit/workspace/__init__.py
```

### Comparing `micrOSDevToolKit-1.17.9/setup.py` & `micrOSDevToolKit-1.18.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.17.9',
+    version='1.18.0',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.17.9/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.18.0/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.18.0/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.18.0/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/Gateway.py` & `micrOSDevToolKit-1.18.0/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.18.0/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.18.0/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.18.0/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.18.0/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.18.0/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.18.0/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.18.0/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.18.0/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/socketClient.py` & `micrOSDevToolKit-1.18.0/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.17.9/toolkit/workspace/simulator/LP_esp32.py` & `micrOSDevToolKit-1.18.0/toolkit/simulator_lib/LP_darwin.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,25 +45,25 @@
 
 # I2C BUS
 i2c_sda = const(21)    # D22 - oled - data
 i2c_scl = const(22)    # D21 - oled - clock
 
 
 # EXTERNAL EVENT IRQ
-irq1 = const(4)         # D4  - event irq pin
-irq2 = const(18)        # D18 - event irq pin
-irq3 = const(5)         # D19  - event irq pin
-irq4 = const(13)        # D13  - event irq pin
-oleduibttn = const(34)  # D34 - oled_ui center/ok button
+irq1 = const(4)        # D4  - event irq pin
+irq2 = const(18)       # D18 - event irq pin
+irq3 = const(5)        # D19  - event irq pin
+irq4 = const(13)       # D13  - event irq pin
 
 touch_0 = const(13)    # D13 - touch sensor TODO
 
 
 # SENSORS
 hcsrtrig = const(32)   # D32 - distance HCSR04 trigger pin
 hcsrecho = const(35)   # D35 - distance HCSR04 echo pin
 dhtpin = const(32)     # D32 - dht_pin 11 and 22
-co2 = const(35)        # D35 - [ADC] CO2
-temp6000 = const(36)   # VP  - [ADC] light sensor TEMP6000
-ph = const(39)         # VN  - [ADC] PH sensor
+co2 = const(35)        # D35 - CO2
+temp6000 = const(36)   # VP - light sensor TEMP6000
+ph = const(39)         # VN - PH sensor
 ds18 = const(19)       # D19 - DS18B20 - temp. sensor
-mic = const(39)        # VN  - [ADC] microphone
+
+mic = const(39)
```

