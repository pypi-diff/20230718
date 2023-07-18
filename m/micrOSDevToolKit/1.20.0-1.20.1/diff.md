# Comparing `tmp/micrOSDevToolKit-1.20.0.tar.gz` & `tmp/micrOSDevToolKit-1.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/micrOSDevToolKit-1.20.0.tar", last modified: Mon Jul 17 20:59:10 2023, max compression
+gzip compressed data, was "dist/micrOSDevToolKit-1.20.1.tar", last modified: Tue Jul 18 20:47:32 2023, max compression
```

## Comparing `micrOSDevToolKit-1.20.0.tar` & `micrOSDevToolKit-1.20.1.tar`

### file list

```diff
@@ -1,249 +1,249 @@
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.301960 micrOSDevToolKit-1.20.0/
--rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.20.0/MANIFEST.in
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-17 20:59:10.301295 micrOSDevToolKit-1.20.0/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.0/README.md
--rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.0/devToolKit.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.020279 micrOSDevToolKit-1.20.0/env/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/env/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.034878 micrOSDevToolKit-1.20.0/media/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.0/media/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/media/dnd.png
--rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.0/media/logo.png
--rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/media/logo_mini.png
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.040236 micrOSDevToolKit-1.20.0/micrOS/
--rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.0/micrOS/SchedulerUT.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.081676 micrOSDevToolKit-1.20.0/micrOS/micropython/
--rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/esp32-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
--rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
--rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.153963 micrOSDevToolKit-1.20.0/micrOS/source/
--rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.0/micrOS/source/.DS_Store
--rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.0/micrOS/source/Common.py
--rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.0/micrOS/source/ConfigHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.0/micrOS/source/Debug.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.0/micrOS/source/Hooks.py
--rw-r--r--   0 bnm        (501) staff       (20)     6889 2023-07-17 15:14:53.000000 micrOSDevToolKit-1.20.0/micrOS/source/InterConnect.py
--rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-17 14:43:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/InterpreterShell.py
--rw-r--r--   0 bnm        (501) staff       (20)     7239 2023-07-17 17:38:40.000000 micrOSDevToolKit-1.20.0/micrOS/source/InterruptHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_L298N_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_bme280.py
--rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_buzzer.py
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_cct.py
--rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_co2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_dht11.py
--rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_dht22.py
--rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_ds18.py
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_genIO.py
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_intercon.py
--rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_light_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2870 2023-07-17 20:27:42.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_lmpacman.py
--rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_neoeffects.py
--rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_oled.py
--rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_sh1106.py
--rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_ui.py
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_presence.py
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_rgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_roboarm.py
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_servo.py
--rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_stepper.py
--rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_switch.py
--rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_system.py
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_telegram.py
--rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LM_tinyrgb.py
--rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s3.py
--rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_rp2.py
--rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.0/micrOS/source/LP_tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.0/micrOS/source/LogicalPins.py
--rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.0/micrOS/source/Network.py
--rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.0/micrOS/source/Notify.py
--rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.0/micrOS/source/Scheduler.py
--rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.0/micrOS/source/SocketServer.py
--rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-17 15:01:38.000000 micrOSDevToolKit-1.20.0/micrOS/source/TaskManager.py
--rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.0/micrOS/source/Time.py
--rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/source/TinyPLed.py
--rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.0/micrOS/source/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.0/micrOS/source/micrOS.py
--rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.0/micrOS/source/micrOSloader.py
--rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.0/micrOS/source/reset.py
--rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.0/micrOS/source/urequests.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.156912 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/
--rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/PKG-INFO
--rw-r--r--   0 bnm        (501) staff       (20)     8792 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/SOURCES.txt
--rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/dependency_links.txt
--rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/requires.txt
--rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-17 20:59:09.000000 micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/top_level.txt
--rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-17 20:59:10.302177 micrOSDevToolKit-1.20.0/setup.cfg
--rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-17 19:37:44.000000 micrOSDevToolKit-1.20.0/setup.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.165563 micrOSDevToolKit-1.20.0/toolkit/
--rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.0/toolkit/DevEnvCompile.py
--rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.0/toolkit/DevEnvOTA.py
--rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.0/toolkit/DevEnvUSB.py
--rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/Gateway.py
--rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.0/toolkit/MicrOSDevEnv.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.184115 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/
--rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityBME280.py
--rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
--rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CatGame.py
--rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Dimmer.py
--rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/GetVersion.py
--rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/MicrophoneTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeoEffectsDemo.py
--rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeopixelTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RGBTest.py
--rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RoboArm.py
--rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SED_test.py
--rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SystemTest.py
--rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Template_app.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/_micPlotting.py
--rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/uLightDemo.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.190248 micrOSDevToolKit-1.20.0/toolkit/lib/
--rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.0/toolkit/lib/LocalMachine.py
--rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.0/toolkit/lib/SearchDevices.py
--rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/lib/SerialDriverHandler.py
--rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/lib/TerminalColors.py
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/lib/__init__.py
--rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.0/toolkit/lib/micrOSClient.py
--rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.0/toolkit/micrOSdashboard.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.207990 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/
--rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/LP_darwin.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.244901 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
--rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
--rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/dotstar.py
--rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/ds18x20.py
--rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/framebuf.py
--rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/machine.py
--rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/micropython.py
--rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/neopixel.py
--rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/network.py
--rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/ntptime.py
--rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/onewire.py
--rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/sim_console.py
--rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/simgc.py
--rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/simulator.py
--rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/tinypico.py
--rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/uasyncio.py
--rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/utime.py
--rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/simulator_lib/webrepl.py
--rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.20.0/toolkit/socketClient.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.245909 micrOSDevToolKit-1.20.0/toolkit/workspace/
--rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/__init__.py
-drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-17 20:59:10.299912 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/
--rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Common.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/ConfigHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Debug.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Hooks.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2111 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterConnect.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterpreterShell.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2141 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterruptHandler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
--rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_VL53L0X.py
--rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_bme280.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_buzzer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_catgame.py
--rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_cct.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_co2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_demo.py
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht11.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht22.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dimmer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_distance.py
--rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ds18.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_esp32.py
--rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_genIO.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_i2c.py
--rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_intercon.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_light_sensor.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1453 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_lmpacman.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neoeffects.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neopixel.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_ui.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_pet_feeder.py
--rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ph_sensor.py
--rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_presence.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rencoder.py
--rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_roboarm.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_robustness.py
--rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_servo.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_stepper.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_switch.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_system.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_telegram.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s3.mpy
--rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_rp2.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_tinypico.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LogicalPins.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Network.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Notify.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Scheduler.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/SocketServer.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     5760 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/TaskManager.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Time.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/TinyPLed.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-17 20:50:00.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/main.py
--rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOS.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOSloader.mpy
--rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/reset.mpy
--rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-17 20:49:59.000000 micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/urequests.mpy
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.286632 micrOSDevToolKit-1.20.1/
+-rw-r--r--   0 bnm        (501) staff       (20)      223 2023-07-06 08:46:44.000000 micrOSDevToolKit-1.20.1/MANIFEST.in
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-18 20:47:32.286043 micrOSDevToolKit-1.20.1/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)    45024 2023-07-05 20:30:41.000000 micrOSDevToolKit-1.20.1/README.md
+-rwxr-xr-x   0 bnm        (501) staff       (20)     8984 2023-07-05 20:33:26.000000 micrOSDevToolKit-1.20.1/devToolKit.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:31.917755 micrOSDevToolKit-1.20.1/env/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.1/env/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:31.920913 micrOSDevToolKit-1.20.1/media/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.1/media/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    42752 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/media/dnd.png
+-rw-r--r--   0 bnm        (501) staff       (20)   482208 2022-11-25 09:53:28.000000 micrOSDevToolKit-1.20.1/media/logo.png
+-rw-r--r--   0 bnm        (501) staff       (20)    24854 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/media/logo_mini.png
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:31.922783 micrOSDevToolKit-1.20.1/micrOS/
+-rw-r--r--   0 bnm        (501) staff       (20)     1312 2023-07-13 18:57:05.000000 micrOSDevToolKit-1.20.1/micrOS/SchedulerUT.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.1/micrOS/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:31.959227 micrOSDevToolKit-1.20.1/micrOS/micropython/
+-rw-r--r--   0 bnm        (501) staff       (20)  1560976 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.1/micrOS/micropython/esp32-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1230192 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1446848 2023-06-14 11:15:48.000000 micrOSDevToolKit-1.20.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin
+-rw-r--r--   0 bnm        (501) staff       (20)  1400832 2023-05-11 08:44:05.000000 micrOSDevToolKit-1.20.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2
+-rw-r--r--   0 bnm        (501) staff       (20)  1519248 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.015861 micrOSDevToolKit-1.20.1/micrOS/source/
+-rw-r--r--   0 bnm        (501) staff       (20)     6148 2023-02-01 11:41:53.000000 micrOSDevToolKit-1.20.1/micrOS/source/.DS_Store
+-rw-r--r--   0 bnm        (501) staff       (20)     6198 2023-07-17 14:02:35.000000 micrOSDevToolKit-1.20.1/micrOS/source/Common.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8423 2023-07-17 14:17:45.000000 micrOSDevToolKit-1.20.1/micrOS/source/ConfigHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6331 2023-07-17 14:19:18.000000 micrOSDevToolKit-1.20.1/micrOS/source/Debug.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-07-17 14:24:13.000000 micrOSDevToolKit-1.20.1/micrOS/source/Hooks.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6889 2023-07-17 15:14:53.000000 micrOSDevToolKit-1.20.1/micrOS/source/InterConnect.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11569 2023-07-18 20:08:00.000000 micrOSDevToolKit-1.20.1/micrOS/source/InterpreterShell.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7239 2023-07-17 17:38:40.000000 micrOSDevToolKit-1.20.1/micrOS/source/InterruptHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2358 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_L298N_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12710 2023-07-15 21:14:31.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_bme280.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8364 2023-06-26 10:58:53.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_buzzer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)    14014 2023-03-13 19:15:23.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_cct.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5149 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_co2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-03-19 11:46:39.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 21:11:36.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_dht11.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2149 2023-07-15 19:50:30.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_dht22.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8137 2023-03-13 17:50:37.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1532 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_ds18.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4106 2022-12-29 20:58:04.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_genIO.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1608 2023-03-09 18:56:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_intercon.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1618 2023-07-06 20:03:50.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_light_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2890 2023-07-18 20:07:19.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_lmpacman.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10473 2022-12-30 23:37:13.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_neoeffects.py
+-rw-r--r--   0 bnm        (501) staff       (20)    13027 2023-03-13 17:52:36.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6745 2023-06-26 12:47:51.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_oled.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9649 2023-06-26 12:52:45.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_oled_sh1106.py
+-rw-r--r--   0 bnm        (501) staff       (20)    18965 2023-07-04 18:36:10.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_oled_ui.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-01-21 00:34:37.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     8081 2023-03-08 10:25:44.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_presence.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-01-21 19:25:04.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11895 2023-03-13 17:53:56.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_rgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9383 2023-03-07 15:19:00.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_roboarm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-02-01 13:23:22.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3427 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_servo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4228 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_stepper.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7567 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_switch.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6374 2023-07-17 18:21:37.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_system.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-03-19 11:48:09.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_telegram.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2947 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LM_tinyrgb.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2183 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LP_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2051 2023-06-26 12:00:43.000000 micrOSDevToolKit-1.20.1/micrOS/source/LP_esp32s2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2104 2023-06-14 17:40:43.000000 micrOSDevToolKit-1.20.1/micrOS/source/LP_esp32s3.py
+-rw-r--r--   0 bnm        (501) staff       (20)       99 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.1/micrOS/source/LP_rp2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2200 2022-12-04 14:42:28.000000 micrOSDevToolKit-1.20.1/micrOS/source/LP_tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5742 2023-06-14 13:29:12.000000 micrOSDevToolKit-1.20.1/micrOS/source/LogicalPins.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9579 2023-07-17 14:33:44.000000 micrOSDevToolKit-1.20.1/micrOS/source/Network.py
+-rw-r--r--   0 bnm        (501) staff       (20)     9189 2023-07-15 18:23:05.000000 micrOSDevToolKit-1.20.1/micrOS/source/Notify.py
+-rw-r--r--   0 bnm        (501) staff       (20)     7744 2023-07-09 11:44:18.000000 micrOSDevToolKit-1.20.1/micrOS/source/Scheduler.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11566 2023-07-15 19:57:59.000000 micrOSDevToolKit-1.20.1/micrOS/source/SocketServer.py
+-rw-r--r--   0 bnm        (501) staff       (20)    19574 2023-07-17 15:01:38.000000 micrOSDevToolKit-1.20.1/micrOS/source/TaskManager.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6254 2023-07-15 20:34:18.000000 micrOSDevToolKit-1.20.1/micrOS/source/Time.py
+-rw-r--r--   0 bnm        (501) staff       (20)      981 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.1/micrOS/source/TinyPLed.py
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2022-11-25 09:53:11.000000 micrOSDevToolKit-1.20.1/micrOS/source/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2657 2023-07-17 14:37:17.000000 micrOSDevToolKit-1.20.1/micrOS/source/micrOS.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4678 2023-07-17 14:34:26.000000 micrOSDevToolKit-1.20.1/micrOS/source/micrOSloader.py
+-rw-r--r--   0 bnm        (501) staff       (20)      183 2023-03-09 19:11:59.000000 micrOSDevToolKit-1.20.1/micrOS/source/reset.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4926 2023-07-17 14:41:23.000000 micrOSDevToolKit-1.20.1/micrOS/source/urequests.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.019007 micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/
+-rw-r--r--   0 bnm        (501) staff       (20)    54579 2023-07-18 20:47:31.000000 micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/PKG-INFO
+-rw-r--r--   0 bnm        (501) staff       (20)     8792 2023-07-18 20:47:31.000000 micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/SOURCES.txt
+-rw-r--r--   0 bnm        (501) staff       (20)        1 2023-07-18 20:47:31.000000 micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/dependency_links.txt
+-rw-r--r--   0 bnm        (501) staff       (20)      149 2023-07-18 20:47:31.000000 micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/requires.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       25 2023-07-18 20:47:31.000000 micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/top_level.txt
+-rw-r--r--   0 bnm        (501) staff       (20)       38 2023-07-18 20:47:32.286782 micrOSDevToolKit-1.20.1/setup.cfg
+-rw-r--r--   0 bnm        (501) staff       (20)     1282 2023-07-18 20:45:22.000000 micrOSDevToolKit-1.20.1/setup.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.027331 micrOSDevToolKit-1.20.1/toolkit/
+-rw-r--r--   0 bnm        (501) staff       (20)     8377 2023-01-04 20:19:38.000000 micrOSDevToolKit-1.20.1/toolkit/DevEnvCompile.py
+-rw-r--r--   0 bnm        (501) staff       (20)    24453 2023-07-15 18:35:28.000000 micrOSDevToolKit-1.20.1/toolkit/DevEnvOTA.py
+-rw-r--r--   0 bnm        (501) staff       (20)    31441 2023-07-12 17:35:49.000000 micrOSDevToolKit-1.20.1/toolkit/DevEnvUSB.py
+-rw-r--r--   0 bnm        (501) staff       (20)    12307 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/Gateway.py
+-rw-r--r--   0 bnm        (501) staff       (20)    11615 2023-07-17 15:49:40.000000 micrOSDevToolKit-1.20.1/toolkit/MicrOSDevEnv.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.043763 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/
+-rw-r--r--   0 bnm        (501) staff       (20)      747 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/AirQualityBME280.py
+-rw-r--r--   0 bnm        (501) staff       (20)      749 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1278 2023-01-14 18:12:52.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/CCTDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3798 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/CCTTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1487 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/CatGame.py
+-rw-r--r--   0 bnm        (501) staff       (20)      937 2023-01-16 18:30:18.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/Dimmer.py
+-rw-r--r--   0 bnm        (501) staff       (20)      542 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/GetVersion.py
+-rw-r--r--   0 bnm        (501) staff       (20)      407 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/MicrophoneTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2409 2023-01-14 15:33:34.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/NeoEffectsDemo.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3938 2023-01-05 18:02:55.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/NeopixelTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3920 2023-01-05 18:11:07.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/RGBTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2084 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/RoboArm.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2782 2023-01-05 18:10:36.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/SED_test.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16516 2023-07-04 19:11:19.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/SystemTest.py
+-rw-r--r--   0 bnm        (501) staff       (20)      760 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/Template_app.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3901 2023-03-08 10:26:06.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/_micPlotting.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3380 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/uLightDemo.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.048978 micrOSDevToolKit-1.20.1/toolkit/lib/
+-rw-r--r--   0 bnm        (501) staff       (20)    18734 2023-02-07 20:49:31.000000 micrOSDevToolKit-1.20.1/toolkit/lib/LocalMachine.py
+-rw-r--r--   0 bnm        (501) staff       (20)     5421 2023-07-05 11:31:18.000000 micrOSDevToolKit-1.20.1/toolkit/lib/SearchDevices.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6222 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/lib/SerialDriverHandler.py
+-rw-r--r--   0 bnm        (501) staff       (20)      847 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/lib/TerminalColors.py
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/lib/__init__.py
+-rw-r--r--   0 bnm        (501) staff       (20)    16808 2023-03-15 15:54:40.000000 micrOSDevToolKit-1.20.1/toolkit/lib/micrOSClient.py
+-rw-r--r--   0 bnm        (501) staff       (20)    52184 2023-07-01 21:55:14.000000 micrOSDevToolKit-1.20.1/toolkit/micrOSdashboard.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.067567 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/
+-rw-r--r--   0 bnm        (501) staff       (20)     2071 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/LP_darwin.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.096057 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1005 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      473 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      483 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/dotstar.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      794 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/esp32.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      367 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/esp32.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      319 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/framebuf.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     6832 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     7029 2023-07-04 17:16:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1124 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1340 2023-03-17 15:56:36.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2985 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     2991 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/onewire.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      430 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/onewire.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1063 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1065 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      362 2022-11-25 19:04:35.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/simgc.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      471 2023-02-01 12:53:53.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/simgc.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     4799 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     5397 2023-07-15 16:13:28.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-04 14:44:01.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      450 2022-12-15 16:06:52.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/tinypico.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      976 2022-12-14 21:38:13.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1355 2023-06-27 16:26:11.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2022-11-25 19:04:34.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)     1583 2023-06-27 12:57:10.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2022-12-03 14:47:41.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-38.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)      254 2023-01-01 15:36:25.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/webrepl.cpython-39.pyc
+-rw-r--r--   0 bnm        (501) staff       (20)       95 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/dotstar.py
+-rw-r--r--   0 bnm        (501) staff       (20)      193 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/ds18x20.py
+-rw-r--r--   0 bnm        (501) staff       (20)       71 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)       47 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/framebuf.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4430 2023-07-01 22:39:14.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/machine.py
+-rw-r--r--   0 bnm        (501) staff       (20)      909 2023-03-17 15:56:08.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/micropython.py
+-rw-r--r--   0 bnm        (501) staff       (20)      567 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/neopixel.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2490 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/network.py
+-rw-r--r--   0 bnm        (501) staff       (20)      109 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/ntptime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       77 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/onewire.py
+-rw-r--r--   0 bnm        (501) staff       (20)      943 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/sim_console.py
+-rw-r--r--   0 bnm        (501) staff       (20)      140 2023-02-01 12:53:17.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/simgc.py
+-rw-r--r--   0 bnm        (501) staff       (20)     6545 2023-07-15 16:13:22.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/simulator.py
+-rw-r--r--   0 bnm        (501) staff       (20)      156 2022-12-04 14:42:29.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/tinypico.py
+-rw-r--r--   0 bnm        (501) staff       (20)      528 2023-06-27 16:23:56.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/uasyncio.py
+-rw-r--r--   0 bnm        (501) staff       (20)      942 2023-06-27 12:56:02.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/utime.py
+-rw-r--r--   0 bnm        (501) staff       (20)       37 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/simulator_lib/webrepl.py
+-rwxr-xr-x   0 bnm        (501) staff       (20)    16943 2023-07-06 10:48:06.000000 micrOSDevToolKit-1.20.1/toolkit/socketClient.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.096891 micrOSDevToolKit-1.20.1/toolkit/workspace/
+-rw-r--r--   0 bnm        (501) staff       (20)        0 2022-11-25 09:53:27.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/__init__.py
+drwxr-xr-x   0 bnm        (501) staff       (20)        0 2023-07-18 20:47:32.284565 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/
+-rw-r--r--   0 bnm        (501) staff       (20)     1791 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Common.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2996 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/ConfigHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1927 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Debug.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      759 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Hooks.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2111 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/InterConnect.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     4174 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/InterpreterShell.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2141 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/InterruptHandler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      869 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1774 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py
+-rw-r--r--   0 bnm        (501) staff       (20)    10011 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_VL53L0X.py
+-rw-r--r--   0 bnm        (501) staff       (20)     4280 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_bme280.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2604 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_buzzer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1647 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_catgame.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3836 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_cct.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1359 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_co2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1948 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_demo.py
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_dht11.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      793 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_dht22.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2353 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_dimmer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2433 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_distance.py
+-rw-r--r--   0 bnm        (501) staff       (20)      522 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_ds18.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1470 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_esp32.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1364 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_genIO.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1015 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_i2c.py
+-rw-r--r--   0 bnm        (501) staff       (20)      616 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_intercon.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      512 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_light_sensor.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1477 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_lmpacman.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2865 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_neoeffects.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3650 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_neopixel.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2295 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_oled.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3203 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     6082 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_oled_ui.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2344 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_pet_feeder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1279 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_ph_sensor.py
+-rw-r--r--   0 bnm        (501) staff       (20)     2558 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_presence.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2998 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_rencoder.py
+-rw-r--r--   0 bnm        (501) staff       (20)     3508 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_rgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2946 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_roboarm.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1751 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_robustness.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1143 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_servo.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1471 2023-07-18 20:40:18.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_stepper.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2167 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_switch.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2754 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_system.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      872 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_telegram.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1001 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      550 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_esp32.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      563 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_esp32s2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      553 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_esp32s3.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)       54 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_rp2.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      491 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_tinypico.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1348 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LogicalPins.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3400 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Network.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2900 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Notify.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1903 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Scheduler.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     3763 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/SocketServer.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     5760 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/TaskManager.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     2727 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Time.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      434 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/TinyPLed.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      440 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/main.py
+-rw-r--r--   0 bnm        (501) staff       (20)     1186 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/micrOS.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1730 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/micrOSloader.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)      198 2023-07-18 20:40:19.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/reset.mpy
+-rw-r--r--   0 bnm        (501) staff       (20)     1451 2023-07-18 20:40:20.000000 micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/urequests.mpy
```

### Comparing `micrOSDevToolKit-1.20.0/PKG-INFO` & `micrOSDevToolKit-1.20.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.0
+Version: 1.20.1
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.0/README.md` & `micrOSDevToolKit-1.20.1/README.md`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/devToolKit.py` & `micrOSDevToolKit-1.20.1/devToolKit.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/media/dnd.png` & `micrOSDevToolKit-1.20.1/media/dnd.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/media/logo.png` & `micrOSDevToolKit-1.20.1/media/logo.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/media/logo_mini.png` & `micrOSDevToolKit-1.20.1/media/logo_mini.png`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/SchedulerUT.py` & `micrOSDevToolKit-1.20.1/micrOS/SchedulerUT.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/micropython/esp32-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.1/micrOS/micropython/esp32-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s2-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.1/micrOS/micropython/esp32s2-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin` & `micrOSDevToolKit-1.20.1/micrOS/micropython/esp32s3_spiram_oct-20230426-v1.20.0.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2` & `micrOSDevToolKit-1.20.1/micrOS/micropython/rp2-pico-w-20230426-v1.20.0.uf2`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/micropython/tinypico-20220618-v1.19.1.bin` & `micrOSDevToolKit-1.20.1/micrOS/micropython/tinypico-20220618-v1.19.1.bin`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/.DS_Store` & `micrOSDevToolKit-1.20.1/micrOS/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/Common.py` & `micrOSDevToolKit-1.20.1/micrOS/source/Common.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/ConfigHandler.py` & `micrOSDevToolKit-1.20.1/micrOS/source/ConfigHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/Debug.py` & `micrOSDevToolKit-1.20.1/micrOS/source/Debug.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/Hooks.py` & `micrOSDevToolKit-1.20.1/micrOS/source/Hooks.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/InterConnect.py` & `micrOSDevToolKit-1.20.1/micrOS/source/InterConnect.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/InterpreterShell.py` & `micrOSDevToolKit-1.20.1/micrOS/source/InterpreterShell.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 #################################################################
 #                  SHELL Interpreter FUNCTIONS                  #
 #################################################################
 
 class Shell:
-    MICROS_VERSION = '1.20.0-0'
+    MICROS_VERSION = '1.20.1-0'
 
     def __init__(self, msg_obj=None):
         """
         comm_obj - communication object - send messages back
                  - comm_obj.reply('msg')
         """
         self.msg_obj = msg_obj
```

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/InterruptHandler.py` & `micrOSDevToolKit-1.20.1/micrOS/source/InterruptHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_L298N_DCmotor.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_L298N_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_bme280.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_bme280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_buzzer.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_buzzer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_catgame.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_cct.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_cct.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_co2.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_co2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_demo.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_dht11.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_dht11.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_dht22.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_dht22.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_dimmer.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_distance.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_ds18.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_ds18.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_esp32.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_genIO.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_genIO.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_i2c.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_intercon.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_intercon.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_light_sensor.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_light_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_lmpacman.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_lmpacman.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from os import listdir, remove
 from Common import socket_stream
 from sys import modules
 
 
 @socket_stream
-def list(msgobj=None):
+def listlm(msgobj=None):
     """
     Load module package manager
     - list all load modules
     """
     # Dump available LMs
     msg_buf = []
     for k in (res.replace('LM_', '') for res in listdir() if 'LM_' in res):
         if msgobj is None:
             msg_buf.append('   {}'.format(k))
         else:
             msgobj('   {}'.format(k))
     return msg_buf if len(msg_buf) > 0 else ''
 
 
-def delm(lm=None):
+def dellm(lm=None):
     """
     Load module package manager
     - delete load module
     :param lm: Delete Load Module with full name: module.py or module.mpy
     """
     if lm is not None and lm.endswith('py'):
         # LM exception list - system and lmpacman cannot be deleted
@@ -50,16 +50,16 @@
         state = True
         if m in py and m != 'main':
             to_delete = f'{m}.py'
             try:
                 remove(to_delete)
             except:
                 state = False
-            msg_buf.append('Delete {} {}'.format(to_delete, state))
-    return msg_buf if len(msg_buf) > 0 else 'Nothing to delete.'
+            msg_buf.append('   Delete {} {}'.format(to_delete, state))
+    return '\n'.join(msg_buf) if len(msg_buf) > 0 else 'Nothing to delete.'
 
 
 def module(unload=None):
     """
     List / unload loaded upython Load Modules
     :param unload: module name to unload
     :param unload: None - list active modules
@@ -85,9 +85,9 @@
             cs = hexlify(sha1(f.read()).digest()).decode('utf-8')
         msgobj("{} {}".format(cs, f_name))
         gclean()
     return "micrOS version: {}".format(cfgget('version'))
 
 
 def help():
-    return 'list', 'delm lm=<module>.py/.mpy', 'del_duplicates',\
+    return 'listlm', 'dellm lm=<module>.py/.mpy', 'del_duplicates',\
            'module unload="LM_rgb/None"', 'micros_checksum'
```

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_neoeffects.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_neoeffects.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_neopixel.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_oled.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_oled.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_sh1106.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_oled_sh1106.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_oled_ui.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_oled_ui.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_presence.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_presence.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_rencoder.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_rgb.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_rgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_roboarm.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_roboarm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_robustness.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_servo.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_servo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_stepper.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_stepper.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_switch.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_switch.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_system.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_system.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_telegram.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_telegram.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LM_tinyrgb.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LM_tinyrgb.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LP_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s2.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LP_esp32s2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LP_esp32s3.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LP_esp32s3.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LP_tinypico.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LP_tinypico.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/LogicalPins.py` & `micrOSDevToolKit-1.20.1/micrOS/source/LogicalPins.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/Network.py` & `micrOSDevToolKit-1.20.1/micrOS/source/Network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/Notify.py` & `micrOSDevToolKit-1.20.1/micrOS/source/Notify.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/Scheduler.py` & `micrOSDevToolKit-1.20.1/micrOS/source/Scheduler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/SocketServer.py` & `micrOSDevToolKit-1.20.1/micrOS/source/SocketServer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/TaskManager.py` & `micrOSDevToolKit-1.20.1/micrOS/source/TaskManager.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/Time.py` & `micrOSDevToolKit-1.20.1/micrOS/source/Time.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/TinyPLed.py` & `micrOSDevToolKit-1.20.1/micrOS/source/TinyPLed.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/micrOS.py` & `micrOSDevToolKit-1.20.1/micrOS/source/micrOS.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/micrOSloader.py` & `micrOSDevToolKit-1.20.1/micrOS/source/micrOSloader.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOS/source/urequests.py` & `micrOSDevToolKit-1.20.1/micrOS/source/urequests.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/PKG-INFO` & `micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micrOSDevToolKit
-Version: 1.20.0
+Version: 1.20.1
 Summary: Development and deployment environment for micrOS, the diy micropython automation OS (IoT)
 Home-page: https://github.com/BxNxM/micrOS
 Author: Marcell Ban
 Author-email: miros.framework@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/BxNxM/micrOS/issues
 Project-URL: GitHub Discussions, https://github.com/BxNxM/micrOS/discussions
```

### Comparing `micrOSDevToolKit-1.20.0/micrOSDevToolKit.egg-info/SOURCES.txt` & `micrOSDevToolKit-1.20.1/micrOSDevToolKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/setup.py` & `micrOSDevToolKit-1.20.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # https://towardsdatascience.com/create-your-custom-python-package-that-you-can-pip-install-from-your-git-repository-f90465867893
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='micrOSDevToolKit',
-    version='1.20.0',
+    version='1.20.1',
     author='Marcell Ban',
     author_email='miros.framework@gmail.com',
     description='Development and deployment environment for micrOS, the diy micropython automation OS (IoT)',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/BxNxM/micrOS',
     project_urls={
```

### Comparing `micrOSDevToolKit-1.20.0/toolkit/DevEnvCompile.py` & `micrOSDevToolKit-1.20.1/toolkit/DevEnvCompile.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/DevEnvOTA.py` & `micrOSDevToolKit-1.20.1/toolkit/DevEnvOTA.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/DevEnvUSB.py` & `micrOSDevToolKit-1.20.1/toolkit/DevEnvUSB.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/Gateway.py` & `micrOSDevToolKit-1.20.1/toolkit/Gateway.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/MicrOSDevEnv.py` & `micrOSDevToolKit-1.20.1/toolkit/MicrOSDevEnv.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityBME280.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/AirQualityBME280.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/AirQualityDHT22_CO2.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/AirQualityDHT22_CO2.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTDemo.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/CCTDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CCTTest.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/CCTTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/CatGame.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/CatGame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Dimmer.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/Dimmer.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/GetVersion.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/GetVersion.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeoEffectsDemo.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/NeoEffectsDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/NeopixelTest.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/NeopixelTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RGBTest.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/RGBTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/RoboArm.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/RoboArm.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SED_test.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/SED_test.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/SystemTest.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/SystemTest.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/Template_app.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/Template_app.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/_micPlotting.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/_micPlotting.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/dashboard_apps/uLightDemo.py` & `micrOSDevToolKit-1.20.1/toolkit/dashboard_apps/uLightDemo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/lib/LocalMachine.py` & `micrOSDevToolKit-1.20.1/toolkit/lib/LocalMachine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/lib/SearchDevices.py` & `micrOSDevToolKit-1.20.1/toolkit/lib/SearchDevices.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/lib/SerialDriverHandler.py` & `micrOSDevToolKit-1.20.1/toolkit/lib/SerialDriverHandler.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/lib/TerminalColors.py` & `micrOSDevToolKit-1.20.1/toolkit/lib/TerminalColors.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/lib/micrOSClient.py` & `micrOSDevToolKit-1.20.1/toolkit/lib/micrOSClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/micrOSdashboard.py` & `micrOSDevToolKit-1.20.1/toolkit/micrOSdashboard.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/LP_darwin.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/LP_darwin.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/LP_darwin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/ds18x20.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/machine.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/machine.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/micropython.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/micropython.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/neopixel.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/network.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/network.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/sim_console.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/simulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/simulator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/uasyncio.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/utime.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/__pycache__/utime.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/machine.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/machine.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/micropython.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/micropython.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/neopixel.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/neopixel.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/network.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/network.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/sim_console.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/sim_console.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/simulator.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/simulator.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/uasyncio.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/uasyncio.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/simulator_lib/utime.py` & `micrOSDevToolKit-1.20.1/toolkit/simulator_lib/utime.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/socketClient.py` & `micrOSDevToolKit-1.20.1/toolkit/socketClient.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Common.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Common.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/ConfigHandler.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/ConfigHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Debug.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Debug.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Hooks.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Hooks.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterConnect.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/InterConnect.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterpreterShell.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/InterpreterShell.mpy`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6366 6770 7574 001a 436f 6e66 6967 4861  cfgput..ConfigHa
 00000050: 6e64 6c65 7200 1865 7865 635f 6c6d 5f63  ndler..exec_lm_c
 00000060: 6f72 6500 1654 6173 6b4d 616e 6167 6572  ore..TaskManager
 00000070: 001a 636f 6e73 6f6c 655f 7772 6974 6500  ..console_write.
 00000080: 1465 7272 6c6f 675f 6164 6400 0a44 6562  .errlog_add..Deb
 00000090: 7567 000a 7265 7365 7400 1473 6f66 745f  ug..reset..soft_
 000000a0: 7265 7365 7400 0e6d 6163 6869 6e65 000a  reset..machine..
-000000b0: 5368 656c 6c00 1031 2e32 302e 302d 3000  Shell..1.20.0-0.
+000000b0: 5368 656c 6c00 1031 2e32 302e 312d 3000  Shell..1.20.1-0.
 000000c0: 230e 6d73 675f 6f62 6a00 0c64 6576 6669  #.msg_obj..devfi
 000000d0: 6400 105f 5f64 6576 6669 6400 0861 7574  d..__devfid..aut
 000000e0: 6800 165f 5f61 7574 685f 6d6f 6465 000a  h..__auth_mode..
 000000f0: 6877 7569 6400 0e5f 5f68 7775 6964 0012  hwuid..__hwuid..
 00000100: 5f5f 6175 7468 5f6f 6b00 165f 5f63 6f6e  __auth_ok..__con
 00000110: 665f 6d6f 6465 000e 7665 7273 696f 6e00  f_mode..version.
 00000120: 1c4d 4943 524f 535f 5645 5253 494f 4e00  .MICROS_VERSION.
```

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/InterruptHandler.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/InterruptHandler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_L298N_DCmotor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_L9110_DCmotor.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_L9110_DCmotor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_VL53L0X.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_VL53L0X.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_bme280.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_bme280.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_buzzer.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_buzzer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_catgame.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_catgame.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_cct.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_cct.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_co2.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_co2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_demo.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_demo.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht11.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_dht11.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dht22.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_dht22.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_dimmer.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_dimmer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_distance.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_distance.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ds18.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_ds18.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_esp32.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_esp32.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_genIO.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_genIO.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_i2c.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_i2c.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_intercon.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_intercon.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_light_sensor.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_light_sensor.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neoeffects.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_neoeffects.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_neopixel.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_neopixel.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_oled.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_sh1106.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_oled_sh1106.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_oled_ui.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_oled_ui.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_pet_feeder.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_pet_feeder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_ph_sensor.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_ph_sensor.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_presence.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_presence.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rencoder.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_rencoder.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_rgb.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_rgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_roboarm.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_roboarm.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_robustness.py` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_robustness.py`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_servo.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_servo.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_stepper.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_stepper.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_switch.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_switch.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_system.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_system.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_telegram.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_telegram.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LM_tinyrgb.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LM_tinyrgb.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_esp32.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s2.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_esp32s2.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LP_esp32s3.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LP_esp32s3.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/LogicalPins.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/LogicalPins.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Network.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Network.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Notify.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Notify.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Scheduler.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Scheduler.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/SocketServer.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/SocketServer.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/TaskManager.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/TaskManager.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/Time.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/Time.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOS.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/micrOS.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/micrOSloader.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/micrOSloader.mpy`

 * *Files identical despite different names*

### Comparing `micrOSDevToolKit-1.20.0/toolkit/workspace/precompiled/urequests.mpy` & `micrOSDevToolKit-1.20.1/toolkit/workspace/precompiled/urequests.mpy`

 * *Files identical despite different names*

