# Comparing `tmp/pyvesync-2.1.7.tar.gz` & `tmp/pyvesync-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvesync-2.1.7.tar", last modified: Fri May 19 02:06:02 2023, max compression
+gzip compressed data, was "pyvesync-2.1.8.tar", last modified: Mon Jul 17 15:39:51 2023, max compression
```

## Comparing `pyvesync-2.1.7.tar` & `pyvesync-2.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.447202 pyvesync-2.1.7/
--rw-rw-rw-   0        0        0     1089 2021-04-26 21:24:56.000000 pyvesync-2.1.7/LICENSE
--rw-rw-rw-   0        0        0       44 2021-04-26 21:24:56.000000 pyvesync-2.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0    31937 2023-05-19 02:06:02.447202 pyvesync-2.1.7/PKG-INFO
--rw-rw-rw-   0        0        0    31205 2023-05-19 01:46:13.000000 pyvesync-2.1.7/README.md
--rw-rw-rw-   0        0        0       16 2021-04-26 21:24:56.000000 pyvesync-2.1.7/requirements.txt
--rw-rw-rw-   0        0        0      342 2023-05-19 02:06:02.449202 pyvesync-2.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1271 2023-05-19 02:02:56.000000 pyvesync-2.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.394202 pyvesync-2.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.432201 pyvesync-2.1.7/src/pyvesync/
--rw-rw-rw-   0        0        0      216 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/__init__.py
--rw-rw-rw-   0        0        0    20649 2023-05-19 01:42:51.000000 pyvesync-2.1.7/src/pyvesync/helpers.py
--rw-rw-rw-   0        0        0    13951 2023-05-18 23:52:27.000000 pyvesync-2.1.7/src/pyvesync/vesync.py
--rw-rw-rw-   0        0        0     5682 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/vesyncbasedevice.py
--rw-rw-rw-   0        0        0    45082 2023-05-18 23:52:27.000000 pyvesync-2.1.7/src/pyvesync/vesyncbulb.py
--rw-rw-rw-   0        0        0    54642 2023-05-19 00:27:27.000000 pyvesync-2.1.7/src/pyvesync/vesyncfan.py
--rw-rw-rw-   0        0        0    24285 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/vesynckitchen.py
--rw-rw-rw-   0        0        0    25884 2022-06-11 01:15:51.000000 pyvesync-2.1.7/src/pyvesync/vesyncoutlet.py
--rw-rw-rw-   0        0        0    13023 2023-03-31 13:13:29.000000 pyvesync-2.1.7/src/pyvesync/vesyncswitch.py
-drwxrwxrwx   0        0        0        0 2023-05-19 02:06:02.446202 pyvesync-2.1.7/src/pyvesync.egg-info/
--rw-rw-rw-   0        0        0    31937 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-11-03 00:59:55.000000 pyvesync-2.1.7/src/pyvesync.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-19 02:06:02.000000 pyvesync-2.1.7/src/pyvesync.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.195637 pyvesync-2.1.8/
+-rw-rw-rw-   0        0        0     1089 2023-07-14 00:55:01.000000 pyvesync-2.1.8/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-07-14 00:55:01.000000 pyvesync-2.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    34658 2023-07-17 15:39:51.195637 pyvesync-2.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    33905 2023-07-17 13:14:50.000000 pyvesync-2.1.8/README.md
+-rw-rw-rw-   0        0        0       16 2023-07-14 00:55:01.000000 pyvesync-2.1.8/requirements.txt
+-rw-rw-rw-   0        0        0      342 2023-07-17 15:39:51.196637 pyvesync-2.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2023-07-17 13:55:24.000000 pyvesync-2.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.163636 pyvesync-2.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.175637 pyvesync-2.1.8/src/pyvesync/
+-rw-rw-rw-   0        0        0      216 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/__init__.py
+-rw-rw-rw-   0        0        0    20649 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/helpers.py
+-rw-rw-rw-   0        0        0    13951 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesync.py
+-rw-rw-rw-   0        0        0     5682 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncbasedevice.py
+-rw-rw-rw-   0        0        0    45082 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncbulb.py
+-rw-rw-rw-   0        0        0    70455 2023-07-17 13:55:29.000000 pyvesync-2.1.8/src/pyvesync/vesyncfan.py
+-rw-rw-rw-   0        0        0    24285 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesynckitchen.py
+-rw-rw-rw-   0        0        0    25884 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncoutlet.py
+-rw-rw-rw-   0        0        0    13023 2023-07-14 00:55:01.000000 pyvesync-2.1.8/src/pyvesync/vesyncswitch.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:39:51.195637 pyvesync-2.1.8/src/pyvesync.egg-info/
+-rw-rw-rw-   0        0        0    34658 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      525 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-14 03:41:33.000000 pyvesync-2.1.8/src/pyvesync.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       51 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 15:39:51.000000 pyvesync-2.1.8/src/pyvesync.egg-info/top_level.txt
```

### Comparing `pyvesync-2.1.7/LICENSE` & `pyvesync-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/PKG-INFO` & `pyvesync-2.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyvesync
-Version: 2.1.7
+Version: 2.1.8
 Summary: pyvesync is a library to manage Etekcity                 Devices, Cosori Air Fryers and Levoit Air                      Purifiers run on the VeSync app.
 Home-page: https://github.com/webdjoe/pyvesync
 Author: Mark Perdue, Joe Trabulsy
 Author-email: webdjoe@gmail.com
 License: MIT
 Keywords: iot,vesync,levoit,etekcity,cosori,valceno
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # pyvesync [![build status](https://img.shields.io/pypi/v/pyvesync.svg)](https://pypi.python.org/pypi/pyvesync) [![Build Status](https://dev.azure.com/webdjoe/pyvesync/_apis/build/status/webdjoe.pyvesync?branchName=master)](https://dev.azure.com/webdjoe/pyvesync/_build/latest?definitionId=4&branchName=master) [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) <!-- omit in toc -->
 
 pyvesync is a library to manage VeSync compatible [smart home devices](#supported-devices)
 
 ## Table of Contents <!-- omit in toc -->
@@ -43,16 +44,17 @@
     - [Standard Methods](#standard-methods)
   - [Outlet API Methods \& Properties](#outlet-api-methods--properties)
     - [Outlet power and energy API Methods \& Properties](#outlet-power-and-energy-api-methods--properties)
     - [Model ESW15-USA 15A/1800W Methods (Have a night light)](#model-esw15-usa-15a1800w-methods-have-a-night-light)
   - [Standard Air Purifier Properties \& Methods](#standard-air-purifier-properties--methods)
     - [Air Purifier Properties](#air-purifier-properties)
     - [Air Purifier Methods](#air-purifier-methods)
-    - [Levoit Purifier Core200S/300S/400S Properties](#levoit-purifier-core200s300s400s-properties)
-    - [Levoit Purifier Core200S/300S/400S Methods](#levoit-purifier-core200s300s400s-methods)
+    - [Levoit Purifier Core200S/300S/400S and Vital 100S/200S Properties](#levoit-purifier-core200s300s400s-and-vital-100s200s-properties)
+    - [Levoit Purifier Core200S/300S/400S and Vital 100S/200S Methods](#levoit-purifier-core200s300s400s-and-vital-100s200s-methods)
+    - [Levoit Vital 100S/200S Properties and Methods](#levoit-vital-100s200s-properties-and-methods)
   - [Lights API Methods \& Properties](#lights-api-methods--properties)
     - [Brightness Light Bulb Method and Properties](#brightness-light-bulb-method-and-properties)
     - [Light Bulb Color Temperature Methods and Properties](#light-bulb-color-temperature-methods-and-properties)
     - [Multicolor Light Bulb Methods and Properties](#multicolor-light-bulb-methods-and-properties)
     - [Dimmable Switch Methods and Properties](#dimmable-switch-methods-and-properties)
   - [Levoit Humidifier Methods and Properties](#levoit-humidifier-methods-and-properties)
     - [Humidifier Properties](#humidifier-properties)
@@ -105,14 +107,16 @@
 ### Levoit Air Purifiers
 
 1. LV-PUR131S
 2. Core 200S
 3. Core 300S
 4. Core 400S
 5. Core 600S
+6. Vital 100S
+7. Vital 200S
 
 ### Etekcity Bulbs
 
 1. Soft White Dimmable Smart Bulb (ESL100)
 2. Cool to Soft White Tunable Dimmable Bulb (ESL100CW)
 
 ### Valceno Bulbs
@@ -338,22 +342,23 @@
 `VeSyncFan.change_fan_speed(speed=None)` - Change fan speed. Call without speed to toggle to next speed
 
 Compatible levels for each model:
 
 - Core 200S [1, 2, 3]
 - Core 300S/400S [1, 2, 3, 4]
 - PUR131S [1, 2, 3]
+- Vital 100S/200S [1, 2, 3, 4]
 
-#### Levoit Purifier Core200S/300S/400S Properties
+#### Levoit Purifier Core200S/300S/400S and Vital 100S/200S Properties
 
 `VeSyncFan.child_lock` - Return the state of the child lock (True=On/False=off)
 
-`VeSyncAir.night_light` - Return the state of the night light (on/dim/off)
+`VeSyncAir.night_light` - Return the state of the night light (on/dim/off) **Not available on Vital 100S/200S**
 
-#### Levoit Purifier Core200S/300S/400S Methods
+#### Levoit Purifier Core200S/300S/400S and Vital 100S/200S Methods
 
 `VeSyncFan.child_lock_on()` Enable child lock
 
 `VeSyncFan.child_lock_off()` Disable child lock
 
 `VeSyncFan.turn_on_display()` Turn display on
 
@@ -363,14 +368,34 @@
 
 `VeSyncFan.get_timer()` - Get any running timers, stores Timer DataClass in `VeSyncFan.timer`
 
 `VeSyncFan.set_timer(timer_duration=3000)` - Set a timer for the device, only turns device off. Timer DataClass stored in `VeSyncFan.timer`
 
 `VeSyncFan.clear_timer()` - Cancel any running timer
 
+#### Levoit Vital 100S/200S Properties and Methods
+
+The Levoit Vital 100S/200S has additional features not available on other models.
+
+`VeSyncFan.set_fan_speed` - The manual fan speed that is currently set (remains constant when in auto/sleep mode)
+
+`VeSyncFan.fan_level` - Returns the fan level purifier is currently operating on whether in auto/manual/sleep mode
+
+`VeSyncFan.light_detection` - Returns the state of the light detection mode (True=On/False=off)
+
+`VeSyncFan.light_detection_state` - Returns whether light is detected (True/False)
+
+`VeSyncFan.pet_mode()` - Set pet mode **NOTE: Only available on Vital 200S**
+
+`VeSyncFan.set_auto_preference(preference='default', room_size=600)` - Set the auto mode preference. Preference can be 'default', 'efficient' or quiet. Room size defaults to 600
+
+`VeSyncFan.set_light_detection_on()` - Turn on light detection mode
+
+`VeSyncFan.set_light_detection_off()` - Turn off light detection mode
+
 ### Lights API Methods & Properties
 
 #### Brightness Light Bulb Method and Properties
 
 *Compatible with all bulbs*
 `VeSyncBulb.brightness` - Return brightness in percentage (1 - 100)
 
@@ -879,23 +904,88 @@
 manager.login()
 manager.update()
 # Prints device list returned from Vesync
 ```
 
 ## Feature Requests
 
-~~If you would like new devices to be added, you will need to capture the packets from the app. The easiest way to do this is by using [Packet Capture for Android](https://play.google.com/store/apps/details?id=app.greyshirts.sslcapture&hl=en_US&gl=US). This works without rooting the device. If you do not have an android or are concerned with adding an app that uses a custom certificate to read the traffic, you can use an Android emulator such as [Nox](https://www.bignox.com/).~~
+Before filing an issue to request a new feature or device, please ensure that you will take the time to test the feature throuroughly. New features cannot be simply tested on Home Assistant. A separate integration must be created which is not part of this library. In order to test a new feature, clone the branch and install into a new virtual environment.
+
+```bash
+mkdir python_test && cd python_test
 
-SSL pinning makes capturing packets with Android ~~not feasible anymore~~ harder than before. A system-wide proxy [ProxyDroid](https://play.google.com/store/apps/details?id=org.proxydroid&hl=en) can be used if ssl pinning is disabled [TrustMeAlready](https://github.com/ViRb3/TrustMeAlready).
+# Check Python version is 3.8 or higher
+python3 --version # or python --version or python3.8 --version
+# Create a new venv
+python3 -m venv pyvesync-venv
+# Activate the venv on linux
+source pyvesync-venv/bin/activate
+# or ....
+pyvesync-venv\Scripts\activate.ps1 # on powershell
+pyvesync-venv\Scripts\activate.bat # on command prompt
+
+# Install branch to be tested into new virtual environment
+pip install git+https://github.com/webdjoe/pyvesync@BRANCHNAME
+```
+
+Test functionality with a script
+
+`test.py`
+
+```python
+import sys
+import logging
+import json
+from pyvesync import VeSync
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
+def test_device():
+  # Instantiate VeSync class and login
+  manager = VeSync(user, password, debug=True)
+  if manager.login() == False
+    logger("Unable to login")
+    return
+
+  # Test specific device
+  # If this were a humidifier and there is only one humidifier/purifier
+  # You can access it with the device index
+  fan = manager.fans[0]
+  # or loop through the fan devices and test for device with "My Device" name
+  # Use lower() to avoid capitalization issues
+  my_device_name = "My Device"
+  fan = None
+  for dev in manager.fans:
+    if dev.name.lower() == my_device_name.lower()
+      fan = dev
+  if fan == None:
+    logger.debug("Device not found")
+    logger.debug("Devices found - \n" + json.dumps(manager._dev_list))
+    return
+
+  # Test all device methods and functionality
+  # Be aware some devices lose internet connectivity if turned off
+  fan.turn_on()
+  fan.turn_off()
+  fan.sleep_mode()
+
+# Make script runnable from command line
+if __name__ == "__main__":
+  logger.debug("Testing device")
+  test_device()
+...
+
+```
 
-Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
+## Device Requests
 
-When capturing packets make sure all packets are captured from the device list, along with all functions that the app contains. The captured packets are stored in text files, please do not capture with pcap format.
+SSL pinning makes capturing packets much harder. In order to be able to capture packets, SSL pinning needs to be disabled before running an SSL proxy. Use an Android emulator such as Android Studio, which is available for Windows and Linux for free. Download the APK from APKPure or a similiar site and use [Objection](https://github.com/sensepost/objection) or [Frida](https://frida.re/docs/gadget/). Followed by capturing the packets with Charles Proxy or another SSL proxy application.
 
-After you capture the packets, please redact the `accountid` and `token`. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
+Be sure to capture all packets from the device list and each of the possible device menus and actions. Please redact the `accountid` and `token` from the captured packets. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
 
 For example:
 
 Before:
 
 ```json
 {
@@ -911,12 +1001,12 @@
 {
   "tk": "AAA111AAA111==1AA",
   "accountId": "111111111",
   "cid": "AAAAAA11-1AA-AA"
 }
 ```
 
-All [contributions](CONTRIBUTING.md) are welcome, please run `tox` before submitting a PR to ensure code is valid.
+# Contributing
 
-Ensure new devices are integrated in tests, please review the [testing](tests/README.md) documentation for more information.
+All [contributions](CONTRIBUTING.md) are welcome.
 
 This project is licensed under [MIT](LICENSE).
```

### Comparing `pyvesync-2.1.7/README.md` & `pyvesync-2.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,16 +25,17 @@
     - [Standard Methods](#standard-methods)
   - [Outlet API Methods \& Properties](#outlet-api-methods--properties)
     - [Outlet power and energy API Methods \& Properties](#outlet-power-and-energy-api-methods--properties)
     - [Model ESW15-USA 15A/1800W Methods (Have a night light)](#model-esw15-usa-15a1800w-methods-have-a-night-light)
   - [Standard Air Purifier Properties \& Methods](#standard-air-purifier-properties--methods)
     - [Air Purifier Properties](#air-purifier-properties)
     - [Air Purifier Methods](#air-purifier-methods)
-    - [Levoit Purifier Core200S/300S/400S Properties](#levoit-purifier-core200s300s400s-properties)
-    - [Levoit Purifier Core200S/300S/400S Methods](#levoit-purifier-core200s300s400s-methods)
+    - [Levoit Purifier Core200S/300S/400S and Vital 100S/200S Properties](#levoit-purifier-core200s300s400s-and-vital-100s200s-properties)
+    - [Levoit Purifier Core200S/300S/400S and Vital 100S/200S Methods](#levoit-purifier-core200s300s400s-and-vital-100s200s-methods)
+    - [Levoit Vital 100S/200S Properties and Methods](#levoit-vital-100s200s-properties-and-methods)
   - [Lights API Methods \& Properties](#lights-api-methods--properties)
     - [Brightness Light Bulb Method and Properties](#brightness-light-bulb-method-and-properties)
     - [Light Bulb Color Temperature Methods and Properties](#light-bulb-color-temperature-methods-and-properties)
     - [Multicolor Light Bulb Methods and Properties](#multicolor-light-bulb-methods-and-properties)
     - [Dimmable Switch Methods and Properties](#dimmable-switch-methods-and-properties)
   - [Levoit Humidifier Methods and Properties](#levoit-humidifier-methods-and-properties)
     - [Humidifier Properties](#humidifier-properties)
@@ -87,14 +88,16 @@
 ### Levoit Air Purifiers
 
 1. LV-PUR131S
 2. Core 200S
 3. Core 300S
 4. Core 400S
 5. Core 600S
+6. Vital 100S
+7. Vital 200S
 
 ### Etekcity Bulbs
 
 1. Soft White Dimmable Smart Bulb (ESL100)
 2. Cool to Soft White Tunable Dimmable Bulb (ESL100CW)
 
 ### Valceno Bulbs
@@ -320,22 +323,23 @@
 `VeSyncFan.change_fan_speed(speed=None)` - Change fan speed. Call without speed to toggle to next speed
 
 Compatible levels for each model:
 
 - Core 200S [1, 2, 3]
 - Core 300S/400S [1, 2, 3, 4]
 - PUR131S [1, 2, 3]
+- Vital 100S/200S [1, 2, 3, 4]
 
-#### Levoit Purifier Core200S/300S/400S Properties
+#### Levoit Purifier Core200S/300S/400S and Vital 100S/200S Properties
 
 `VeSyncFan.child_lock` - Return the state of the child lock (True=On/False=off)
 
-`VeSyncAir.night_light` - Return the state of the night light (on/dim/off)
+`VeSyncAir.night_light` - Return the state of the night light (on/dim/off) **Not available on Vital 100S/200S**
 
-#### Levoit Purifier Core200S/300S/400S Methods
+#### Levoit Purifier Core200S/300S/400S and Vital 100S/200S Methods
 
 `VeSyncFan.child_lock_on()` Enable child lock
 
 `VeSyncFan.child_lock_off()` Disable child lock
 
 `VeSyncFan.turn_on_display()` Turn display on
 
@@ -345,14 +349,34 @@
 
 `VeSyncFan.get_timer()` - Get any running timers, stores Timer DataClass in `VeSyncFan.timer`
 
 `VeSyncFan.set_timer(timer_duration=3000)` - Set a timer for the device, only turns device off. Timer DataClass stored in `VeSyncFan.timer`
 
 `VeSyncFan.clear_timer()` - Cancel any running timer
 
+#### Levoit Vital 100S/200S Properties and Methods
+
+The Levoit Vital 100S/200S has additional features not available on other models.
+
+`VeSyncFan.set_fan_speed` - The manual fan speed that is currently set (remains constant when in auto/sleep mode)
+
+`VeSyncFan.fan_level` - Returns the fan level purifier is currently operating on whether in auto/manual/sleep mode
+
+`VeSyncFan.light_detection` - Returns the state of the light detection mode (True=On/False=off)
+
+`VeSyncFan.light_detection_state` - Returns whether light is detected (True/False)
+
+`VeSyncFan.pet_mode()` - Set pet mode **NOTE: Only available on Vital 200S**
+
+`VeSyncFan.set_auto_preference(preference='default', room_size=600)` - Set the auto mode preference. Preference can be 'default', 'efficient' or quiet. Room size defaults to 600
+
+`VeSyncFan.set_light_detection_on()` - Turn on light detection mode
+
+`VeSyncFan.set_light_detection_off()` - Turn off light detection mode
+
 ### Lights API Methods & Properties
 
 #### Brightness Light Bulb Method and Properties
 
 *Compatible with all bulbs*
 `VeSyncBulb.brightness` - Return brightness in percentage (1 - 100)
 
@@ -861,23 +885,88 @@
 manager.login()
 manager.update()
 # Prints device list returned from Vesync
 ```
 
 ## Feature Requests
 
-~~If you would like new devices to be added, you will need to capture the packets from the app. The easiest way to do this is by using [Packet Capture for Android](https://play.google.com/store/apps/details?id=app.greyshirts.sslcapture&hl=en_US&gl=US). This works without rooting the device. If you do not have an android or are concerned with adding an app that uses a custom certificate to read the traffic, you can use an Android emulator such as [Nox](https://www.bignox.com/).~~
+Before filing an issue to request a new feature or device, please ensure that you will take the time to test the feature throuroughly. New features cannot be simply tested on Home Assistant. A separate integration must be created which is not part of this library. In order to test a new feature, clone the branch and install into a new virtual environment.
+
+```bash
+mkdir python_test && cd python_test
 
-SSL pinning makes capturing packets with Android ~~not feasible anymore~~ harder than before. A system-wide proxy [ProxyDroid](https://play.google.com/store/apps/details?id=org.proxydroid&hl=en) can be used if ssl pinning is disabled [TrustMeAlready](https://github.com/ViRb3/TrustMeAlready).
+# Check Python version is 3.8 or higher
+python3 --version # or python --version or python3.8 --version
+# Create a new venv
+python3 -m venv pyvesync-venv
+# Activate the venv on linux
+source pyvesync-venv/bin/activate
+# or ....
+pyvesync-venv\Scripts\activate.ps1 # on powershell
+pyvesync-venv\Scripts\activate.bat # on command prompt
+
+# Install branch to be tested into new virtual environment
+pip install git+https://github.com/webdjoe/pyvesync@BRANCHNAME
+```
+
+Test functionality with a script
+
+`test.py`
+
+```python
+import sys
+import logging
+import json
+from pyvesync import VeSync
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
+def test_device():
+  # Instantiate VeSync class and login
+  manager = VeSync(user, password, debug=True)
+  if manager.login() == False
+    logger("Unable to login")
+    return
+
+  # Test specific device
+  # If this were a humidifier and there is only one humidifier/purifier
+  # You can access it with the device index
+  fan = manager.fans[0]
+  # or loop through the fan devices and test for device with "My Device" name
+  # Use lower() to avoid capitalization issues
+  my_device_name = "My Device"
+  fan = None
+  for dev in manager.fans:
+    if dev.name.lower() == my_device_name.lower()
+      fan = dev
+  if fan == None:
+    logger.debug("Device not found")
+    logger.debug("Devices found - \n" + json.dumps(manager._dev_list))
+    return
+
+  # Test all device methods and functionality
+  # Be aware some devices lose internet connectivity if turned off
+  fan.turn_on()
+  fan.turn_off()
+  fan.sleep_mode()
+
+# Make script runnable from command line
+if __name__ == "__main__":
+  logger.debug("Testing device")
+  test_device()
+...
+
+```
 
-Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
+## Device Requests
 
-When capturing packets make sure all packets are captured from the device list, along with all functions that the app contains. The captured packets are stored in text files, please do not capture with pcap format.
+SSL pinning makes capturing packets much harder. In order to be able to capture packets, SSL pinning needs to be disabled before running an SSL proxy. Use an Android emulator such as Android Studio, which is available for Windows and Linux for free. Download the APK from APKPure or a similiar site and use [Objection](https://github.com/sensepost/objection) or [Frida](https://frida.re/docs/gadget/). Followed by capturing the packets with Charles Proxy or another SSL proxy application.
 
-After you capture the packets, please redact the `accountid` and `token`. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
+Be sure to capture all packets from the device list and each of the possible device menus and actions. Please redact the `accountid` and `token` from the captured packets. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
 
 For example:
 
 Before:
 
 ```json
 {
@@ -893,12 +982,12 @@
 {
   "tk": "AAA111AAA111==1AA",
   "accountId": "111111111",
   "cid": "AAAAAA11-1AA-AA"
 }
 ```
 
-All [contributions](CONTRIBUTING.md) are welcome, please run `tox` before submitting a PR to ensure code is valid.
+# Contributing
 
-Ensure new devices are integrated in tests, please review the [testing](tests/README.md) documentation for more information.
+All [contributions](CONTRIBUTING.md) are welcome.
 
 This project is licensed under [MIT](LICENSE).
```

### Comparing `pyvesync-2.1.7/setup.py` & `pyvesync-2.1.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='pyvesync',
-    version='2.1.7',
+    version='2.1.8',
     description='pyvesync is a library to manage Etekcity\
                  Devices, Cosori Air Fryers and Levoit Air \
                      Purifiers run on the VeSync app.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/webdjoe/pyvesync',
     author='Mark Perdue, Joe Trabulsy',
@@ -28,9 +28,12 @@
         'Programming Language :: Python :: 3.8',
     ],
     keywords=['iot', 'vesync', 'levoit', 'etekcity', 'cosori', 'valceno'],
     packages=find_packages('src', exclude=['tests', 'tests.*']),
     package_dir={'': 'src'},
     zip_safe=False,
     install_requires=['requests>=2.20.0'],
+    extras_require={
+        'dev': ['pytest', 'pytest-cov', 'yaml', 'tox']
+    },
     python_requires='>=3.8',
 )
```

### Comparing `pyvesync-2.1.7/src/pyvesync/helpers.py` & `pyvesync-2.1.8/src/pyvesync/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/src/pyvesync/vesync.py` & `pyvesync-2.1.8/src/pyvesync/vesync.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/src/pyvesync/vesyncbasedevice.py` & `pyvesync-2.1.8/src/pyvesync/vesyncbasedevice.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/src/pyvesync/vesyncbulb.py` & `pyvesync-2.1.8/src/pyvesync/vesyncbulb.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/src/pyvesync/vesyncfan.py` & `pyvesync-2.1.8/src/pyvesync/vesyncfan.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """VeSync API for controling fans and purifiers."""
 
 import json
 import logging
-from typing import Dict, Tuple, Union, Optional
+from typing import Any, Dict, List, Tuple, Union, Optional
 from pyvesync.vesyncbasedevice import VeSyncBaseDevice
 from pyvesync.helpers import Helpers, Timer
 
 
 humid_features: dict = {
     'Classic300S': {
         'module': 'VeSyncHumid200300S',
@@ -42,15 +42,15 @@
         'features': ['warm_mist', 'nightlight'],
         'mist_modes': ['humidity', 'sleep', 'manual'],
         'mist_levels': list(range(1, 10)),
         'warm_mist_levels': [0, 1, 2, 3]
     },
     'OASISMIST': {
             'module': 'VeSyncHumid200300S',
-            'models': ['LUH-O451S-WUS'],
+            'models': ['LUH-O451S-WUS', 'LUH-O451S-WEU'],
             'features': ['warm_mist'],
             'mist_modes': ['humidity', 'sleep', 'manual'],
             'mist_levels': list(range(1, 10)),
             'warm_mist_levels': list(range(4))
         },
 }
 
@@ -91,14 +91,30 @@
         'levels': list(range(1, 5))
     },
     'LV-PUR131S': {
         'module': 'VeSyncAir131',
         'models': ['LV-PUR131S', 'LV-RH131S'],
         'features': ['air_quality']
     },
+    'Vital100S': {
+        'module': 'VeSyncVital',
+        'models': ['LAP-V102S-AASR', 'LAP-V102S-WUS', 'LAP-V102S-WEU',
+                   'LAP-V102S-AUSR', 'LAP-V102S-WJP'],
+        'modes': ['manual', 'auto', 'sleep', 'off'],
+        'features': ['air_quality'],
+        'levels': list(range(1, 5))
+    },
+    'Vital200S': {
+        'module': 'VeSyncVital',
+        'models': ['LAP-V201S-AASR', 'LAP-V201S-WJP', 'LAP-V201S-WEU',
+                   'LAP-V102S-AUSR', 'LAP-V201S-WUS'],
+        'modes': ['manual', 'auto', 'sleep', 'off', 'pet'],
+        'features': ['air_quality'],
+        'levels': list(range(1, 5))
+    }
 }
 
 
 logger = logging.getLogger(__name__)
 
 
 def model_dict() -> dict:
@@ -141,15 +157,15 @@
                 self.device_type)
             raise KeyError(f'Modes not set in configuration for {self.device_name}')
         self.modes = self.config_dict['modes']
         if 'air_quality' in self.features:
             self.air_quality_feature = True
         else:
             self.air_quality_feature = False
-        self.details: Dict[str, Union[str, int, float, bool]] = {
+        self.details: Dict[str, Any] = {
             'filter_life': 0,
             'mode': 'manual',
             'level': 0,
             'display': False,
             'child_lock': False,
             'night_light': 'off',
         }
@@ -714,14 +730,447 @@
             )
             sup_val.update(
                 {'Air Quality Value': str(self.details.get('air_quality_value', ''))}
             )
         return json.dumps(sup_val, indent=4)
 
 
+class VeSyncVital(VeSyncAirBypass):
+    """Levoit Vital 100S/200S Air Purifier Class."""
+
+    def __init__(self, details: Dict[str, list], manager):
+        """Initialize the VeSync Vital 100S/200S Air Purifier Class."""
+        super().__init__(details, manager)
+        self.set_speed_level: Optional[int] = None
+        self.auto_prefences: List[str] = ['default', 'efficient', 'quiet']
+
+    @property
+    def light_detection(self) -> bool:
+        """Return true if light detection feature is enabled."""
+        return self.details['light_detection_switch']
+
+    @light_detection.setter
+    def light_detection(self, toggle: bool) -> None:
+        """Set light detection feature."""
+        self.details['light_detection_switch'] = toggle
+
+    @property
+    def light_detection_state(self) -> bool:
+        """Return true if light is detected."""
+        return self.details['environment_light_state']
+
+    def get_details(self) -> None:
+        """Build Levoit 100S Purifier details dictionary."""
+        head, body = self.build_api_dict('getPurifierStatus')
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+        if not isinstance(r, dict):
+            logger.debug('Error in purifier response')
+            return
+        if not isinstance(r.get('result'), dict):
+            logger.debug('Error in purifier response')
+            return
+        outer_result = r.get('result', {})
+        inner_result = None
+
+        if outer_result:
+            inner_result = r.get('result', {}).get('result')
+        if inner_result is not None and Helpers.code_check(r):
+            if outer_result.get('code') == 0:
+                self.build_purifier_dict(inner_result)
+            else:
+                logger.debug('error in inner result dict from purifier')
+            if inner_result.get('configuration', {}):
+                self.build_config_dict(inner_result.get('configuration', {}))
+            else:
+                logger.debug('No configuration found in purifier status')
+        else:
+            logger.debug('Error in purifier response')
+
+    def build_api_dict(self, method: str) -> Tuple[Dict, Dict]:
+        """Return default body for Levoit Vital 100S/200S API."""
+        header = Helpers.bypass_header()
+        body = Helpers.bypass_body_v2(self.manager)
+        body['cid'] = self.cid
+        body['deviceId'] = self.cid
+        body['configModule'] = self.config_module
+        body['configModel'] = self.config_module
+        body['payload'] = {
+            'method': method,
+            'source': 'APP',
+            'data': {}
+        }
+        return header, body
+
+    def build_purifier_dict(self, dev_dict: dict) -> None:
+        """Build Bypass purifier status dictionary."""
+        power_switch = dev_dict.get('power_switch', 0)
+        self.enabled = power_switch
+        self.device_status = 'on' if power_switch else 'off'
+        self.mode = dev_dict.get('workMode', 'manual')
+
+        self.speed = dev_dict.get('fanSpeedLevel', 0)
+
+        self.set_speed_level = dev_dict.get('manualSpeedLevel', 1)
+
+        self.details['filter_life'] = dev_dict.get('filterLifePercent', 0)
+        self.details['display'] = dev_dict.get('display', False)
+        self.details['child_lock'] = bool(dev_dict.get('childLockSwitch', 0))
+        self.details['night_light'] = dev_dict.get('night_light', 'off')
+        self.details['display'] = bool(dev_dict.get('screenState', 0))
+        self.details['display_forever'] = dev_dict.get('display_forever', False)
+        self.details['light_detection_switch'] = bool(
+            dev_dict.get('lightDetectionSwitch', 0))
+        self.details['environment_light_state'] = bool(
+            dev_dict.get('environmentLightState', 0))
+        self.details['screen_state'] = bool(dev_dict.get('screenState', 0))
+        self.details['screen_switch'] = bool(dev_dict.get('screenSwitch', 0))
+
+        if self.air_quality_feature is True:
+            self.details['air_quality_value'] = dev_dict.get(
+                'PM25', 0)
+            self.details['air_quality'] = dev_dict.get('air_quality', 0)
+        if dev_dict.get('timerRemain') is not None:
+            self.timer = Timer(dev_dict['timerRemain'], 'off')
+        if isinstance(dev_dict.get('autoPreference'), dict):
+            self.details['auto_preference_type'] = dev_dict.get(
+                'autoPreference', {}).get('autoPreferenceType', 'default')
+        else:
+            self.details['auto_preference_type'] = None
+
+    def pet_mode(self) -> bool:
+        """Set Pet Mode for Levoit Vital 200S."""
+        return self.mode_toggle('pet')
+
+    def set_light_detection(self, toggle: bool) -> bool:
+        """Enable/Disable Light Detection Feature."""
+        if toggle is True:
+            toggle_id = 1
+        else:
+            toggle_id = 0
+        if self.details['light_detection_switch'] == toggle_id:
+            logger.debug("Light Detection is already set to %s", toggle_id)
+            return True
+
+        head, body = self.build_api_dict('setLightDetectionSwitch')
+        body['payload']['data']['lightDetectionSwitch'] = toggle_id
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            self.details['light_detection'] = toggle
+            return True
+        logger.debug("Error toggling purifier - %s",
+                     self.device_name)
+        return False
+
+    def set_light_detection_on(self) -> bool:
+        """Turn on light detection feature."""
+        return self.set_light_detection(True)
+
+    def set_light_detection_off(self) -> bool:
+        """Turn off light detection feature."""
+        return self.set_light_detection(False)
+
+    def toggle_switch(self, toggle: bool) -> bool:
+        """Toggle purifier on/off."""
+        if not isinstance(toggle, bool):
+            logger.debug('Invalid toggle value for purifier switch')
+            return False
+
+        head, body = self.build_api_dict('setSwitch')
+        if toggle is True:
+            power = 1
+        else:
+            power = 0
+        body['payload']['data'] = {
+                'powerSwitch': power,
+                'switchIdx': 0
+            }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            if toggle:
+                self.device_status = 'on'
+            else:
+                self.device_status = 'off'
+            return True
+        logger.debug("Error toggling purifier - %s",
+                     self.device_name)
+        return False
+
+    def set_child_lock(self, mode: bool) -> bool:
+        """Levoit 100S set Child Lock."""
+        if mode:
+            toggle_id = 1
+        else:
+            toggle_id = 0
+        head, body = self.build_api_dict('setChildLock')
+        body['payload']['data'] = {
+            'childLockSwitch': toggle_id
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            self.details['child_lock'] = mode
+            return True
+
+        logger.debug("Error toggling purifier child lock - %s", self.device_name)
+        return False
+
+    def set_display(self, mode: bool) -> bool:
+        """Levoit Vital 100S/200S Set Display on/off with True/False."""
+        if mode:
+            mode_id = 1
+        else:
+            mode_id = 0
+        head, body = self.build_api_dict('setDisplay')
+        body['payload']['data'] = {
+            'screenSwitch': mode_id
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            self.details['screen_switch'] = mode
+            return True
+
+        logger.debug("Error toggling purifier display - %s", self.device_name)
+        return False
+
+    def set_timer(self, timer_duration: int, action: str = 'off',
+                  method: str = 'powerSwitch') -> bool:
+        """Set timer for Levoit 100S.
+
+        Parameters
+        ----------
+        timer_duration : int
+            Timer duration in seconds.
+        action : str, optional
+            Action to perform, on or off, by default 'off'
+        method : str, optional
+            Method to use, by default 'powerSwitch' - TODO: Implement other methods
+        Returns
+        -------
+        bool
+        """
+        if action not in ['on', 'off']:
+            logger.debug('Invalid action for timer')
+            return False
+        if method not in ['powerSwitch']:
+            logger.debug('Invalid method for timer')
+            return False
+        action_id = 1 if action == 'on' else 0
+
+        head, body = self.build_api_dict('addTimerV2')
+        body['payload']['subDeviceNo'] = 0
+        body['payload']['data'] = {
+            "startAct": [{
+                "type": method,
+                "num": 0,
+                "act": action_id,
+            }],
+            "total": timer_duration,
+            "subDeviceNo": 0
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            self.timer = Timer(timer_duration, action)
+            return True
+
+        logger.debug("Error setting timer for - %s", self.device_name)
+        return False
+
+    def clear_timer(self) -> bool:
+        """Clear running timer."""
+        head, body = self.build_api_dict('delTimerV2')
+        body['payload']['subDeviceNo'] = 0
+        body['payload']['data'] = {'id': 1, "subDeviceNo": 0}
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            self.timer = None
+            return True
+
+        logger.debug("Error setting timer for - %s", self.device_name)
+        return False
+
+    def set_auto_preference(self, preference: str = 'default',
+                            room_size: int = 600) -> bool:
+        """Set Levoit Vital 100S/200S auto mode.
+
+        Parameters
+        ----------
+        preference : str, optional
+            Preference for auto mode, by default 'default'
+            options are: default, efficient, quiet
+        room_size : int, optional
+            Room size in square feet, by default 600
+        """
+        if preference not in self.auto_prefences:
+            logger.debug("%s is invalid preference -"
+                         " valid preferences are default, efficient, quiet",
+                         preference)
+            return False
+        head, body = self.build_api_dict('setAutoPreference')
+        body['payload']['data'] = {
+            'autoPreference': preference,
+            'roomSize': room_size,
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            self.details['auto_preference'] = preference
+            return True
+
+        logger.debug("Error setting auto preference for - %s", self.device_name)
+        return False
+
+    def change_fan_speed(self, speed=None) -> bool:
+        """Change fan speed based on levels in configuration dict.
+
+        Parameters
+        ----------
+        speed : int, optional
+            Speed to set based on levels in configuration dict, by default None
+            If None, will cycle through levels in configuration dict
+        """
+        speeds: list = self.config_dict.get('levels', [])
+        current_speed = self.set_speed_level or 0
+
+        if speed is not None:
+            if speed not in speeds:
+                logger.debug("%s is invalid speed - valid speeds are %s",
+                             speed, str(speeds))
+                return False
+            new_speed = speed
+        else:
+            if current_speed in [speeds[-1], 0]:
+                new_speed = speeds[0]
+            else:
+                current_index = speeds.index(current_speed)
+                new_speed = speeds[current_index + 1]
+
+        head, body = self.build_api_dict('setLevel')
+        if not head or not body:
+            return False
+        body['payload']['data'] = {
+            'levelIdx': 0,
+            'manualSpeedLevel': new_speed,
+            'levelType': 'wind'
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if r is not None and Helpers.code_check(r):
+            self.set_speed_level = new_speed
+            self.mode = 'manual'
+            return True
+        logger.debug('Error changing %s speed', self.device_name)
+        return False
+
+    def mode_toggle(self, mode: str) -> bool:
+        """Set Levoit 100S purifier mode.
+
+        Parameters
+        ----------
+        mode : str
+            Mode to set purifier to, options are: auto, manual, sleep
+
+        Returns
+        -------
+        bool
+        """
+        if mode.lower() not in self.modes:
+            logger.debug('Invalid purifier mode used - %s',
+                         mode)
+            return False
+
+        # Call change_fan_speed if mode is set to manual
+        if mode == 'manual':
+            if self.speed is None or self.speed == 0:
+                return self.change_fan_speed(1)
+            return self.change_fan_speed(self.speed)
+
+        if mode == 'off':
+            return self.turn_off()
+
+        head, body = self.build_api_dict('setPurifierMode')
+        if not head and not body:
+            return False
+
+        body['deviceId'] = self.cid
+        body['payload']['data'] = {
+            'workMode': mode.lower()
+        }
+
+        r, _ = Helpers.call_api(
+            '/cloud/v2/deviceManaged/bypassV2',
+            method='post',
+            headers=head,
+            json_object=body,
+        )
+
+        if Helpers.code_check(r):
+            self.mode = mode
+            return True
+        logger.debug('Error setting purifier mode')
+        return False
+
+
 class VeSyncAir131(VeSyncBaseDevice):
     """Levoit Air Purifier Class."""
 
     def __init__(self, details, manager):
         """Initilize air purifier class."""
         super().__init__(details, manager)
```

### Comparing `pyvesync-2.1.7/src/pyvesync/vesynckitchen.py` & `pyvesync-2.1.8/src/pyvesync/vesynckitchen.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/src/pyvesync/vesyncoutlet.py` & `pyvesync-2.1.8/src/pyvesync/vesyncoutlet.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/src/pyvesync/vesyncswitch.py` & `pyvesync-2.1.8/src/pyvesync/vesyncswitch.py`

 * *Files identical despite different names*

### Comparing `pyvesync-2.1.7/src/pyvesync.egg-info/PKG-INFO` & `pyvesync-2.1.8/src/pyvesync.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyvesync
-Version: 2.1.7
+Version: 2.1.8
 Summary: pyvesync is a library to manage Etekcity                 Devices, Cosori Air Fryers and Levoit Air                      Purifiers run on the VeSync app.
 Home-page: https://github.com/webdjoe/pyvesync
 Author: Mark Perdue, Joe Trabulsy
 Author-email: webdjoe@gmail.com
 License: MIT
 Keywords: iot,vesync,levoit,etekcity,cosori,valceno
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # pyvesync [![build status](https://img.shields.io/pypi/v/pyvesync.svg)](https://pypi.python.org/pypi/pyvesync) [![Build Status](https://dev.azure.com/webdjoe/pyvesync/_apis/build/status/webdjoe.pyvesync?branchName=master)](https://dev.azure.com/webdjoe/pyvesync/_build/latest?definitionId=4&branchName=master) [![Open Source? Yes!](https://badgen.net/badge/Open%20Source%20%3F/Yes%21/blue?icon=github)](https://github.com/Naereen/badges/) [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/) <!-- omit in toc -->
 
 pyvesync is a library to manage VeSync compatible [smart home devices](#supported-devices)
 
 ## Table of Contents <!-- omit in toc -->
@@ -43,16 +44,17 @@
     - [Standard Methods](#standard-methods)
   - [Outlet API Methods \& Properties](#outlet-api-methods--properties)
     - [Outlet power and energy API Methods \& Properties](#outlet-power-and-energy-api-methods--properties)
     - [Model ESW15-USA 15A/1800W Methods (Have a night light)](#model-esw15-usa-15a1800w-methods-have-a-night-light)
   - [Standard Air Purifier Properties \& Methods](#standard-air-purifier-properties--methods)
     - [Air Purifier Properties](#air-purifier-properties)
     - [Air Purifier Methods](#air-purifier-methods)
-    - [Levoit Purifier Core200S/300S/400S Properties](#levoit-purifier-core200s300s400s-properties)
-    - [Levoit Purifier Core200S/300S/400S Methods](#levoit-purifier-core200s300s400s-methods)
+    - [Levoit Purifier Core200S/300S/400S and Vital 100S/200S Properties](#levoit-purifier-core200s300s400s-and-vital-100s200s-properties)
+    - [Levoit Purifier Core200S/300S/400S and Vital 100S/200S Methods](#levoit-purifier-core200s300s400s-and-vital-100s200s-methods)
+    - [Levoit Vital 100S/200S Properties and Methods](#levoit-vital-100s200s-properties-and-methods)
   - [Lights API Methods \& Properties](#lights-api-methods--properties)
     - [Brightness Light Bulb Method and Properties](#brightness-light-bulb-method-and-properties)
     - [Light Bulb Color Temperature Methods and Properties](#light-bulb-color-temperature-methods-and-properties)
     - [Multicolor Light Bulb Methods and Properties](#multicolor-light-bulb-methods-and-properties)
     - [Dimmable Switch Methods and Properties](#dimmable-switch-methods-and-properties)
   - [Levoit Humidifier Methods and Properties](#levoit-humidifier-methods-and-properties)
     - [Humidifier Properties](#humidifier-properties)
@@ -105,14 +107,16 @@
 ### Levoit Air Purifiers
 
 1. LV-PUR131S
 2. Core 200S
 3. Core 300S
 4. Core 400S
 5. Core 600S
+6. Vital 100S
+7. Vital 200S
 
 ### Etekcity Bulbs
 
 1. Soft White Dimmable Smart Bulb (ESL100)
 2. Cool to Soft White Tunable Dimmable Bulb (ESL100CW)
 
 ### Valceno Bulbs
@@ -338,22 +342,23 @@
 `VeSyncFan.change_fan_speed(speed=None)` - Change fan speed. Call without speed to toggle to next speed
 
 Compatible levels for each model:
 
 - Core 200S [1, 2, 3]
 - Core 300S/400S [1, 2, 3, 4]
 - PUR131S [1, 2, 3]
+- Vital 100S/200S [1, 2, 3, 4]
 
-#### Levoit Purifier Core200S/300S/400S Properties
+#### Levoit Purifier Core200S/300S/400S and Vital 100S/200S Properties
 
 `VeSyncFan.child_lock` - Return the state of the child lock (True=On/False=off)
 
-`VeSyncAir.night_light` - Return the state of the night light (on/dim/off)
+`VeSyncAir.night_light` - Return the state of the night light (on/dim/off) **Not available on Vital 100S/200S**
 
-#### Levoit Purifier Core200S/300S/400S Methods
+#### Levoit Purifier Core200S/300S/400S and Vital 100S/200S Methods
 
 `VeSyncFan.child_lock_on()` Enable child lock
 
 `VeSyncFan.child_lock_off()` Disable child lock
 
 `VeSyncFan.turn_on_display()` Turn display on
 
@@ -363,14 +368,34 @@
 
 `VeSyncFan.get_timer()` - Get any running timers, stores Timer DataClass in `VeSyncFan.timer`
 
 `VeSyncFan.set_timer(timer_duration=3000)` - Set a timer for the device, only turns device off. Timer DataClass stored in `VeSyncFan.timer`
 
 `VeSyncFan.clear_timer()` - Cancel any running timer
 
+#### Levoit Vital 100S/200S Properties and Methods
+
+The Levoit Vital 100S/200S has additional features not available on other models.
+
+`VeSyncFan.set_fan_speed` - The manual fan speed that is currently set (remains constant when in auto/sleep mode)
+
+`VeSyncFan.fan_level` - Returns the fan level purifier is currently operating on whether in auto/manual/sleep mode
+
+`VeSyncFan.light_detection` - Returns the state of the light detection mode (True=On/False=off)
+
+`VeSyncFan.light_detection_state` - Returns whether light is detected (True/False)
+
+`VeSyncFan.pet_mode()` - Set pet mode **NOTE: Only available on Vital 200S**
+
+`VeSyncFan.set_auto_preference(preference='default', room_size=600)` - Set the auto mode preference. Preference can be 'default', 'efficient' or quiet. Room size defaults to 600
+
+`VeSyncFan.set_light_detection_on()` - Turn on light detection mode
+
+`VeSyncFan.set_light_detection_off()` - Turn off light detection mode
+
 ### Lights API Methods & Properties
 
 #### Brightness Light Bulb Method and Properties
 
 *Compatible with all bulbs*
 `VeSyncBulb.brightness` - Return brightness in percentage (1 - 100)
 
@@ -879,23 +904,88 @@
 manager.login()
 manager.update()
 # Prints device list returned from Vesync
 ```
 
 ## Feature Requests
 
-~~If you would like new devices to be added, you will need to capture the packets from the app. The easiest way to do this is by using [Packet Capture for Android](https://play.google.com/store/apps/details?id=app.greyshirts.sslcapture&hl=en_US&gl=US). This works without rooting the device. If you do not have an android or are concerned with adding an app that uses a custom certificate to read the traffic, you can use an Android emulator such as [Nox](https://www.bignox.com/).~~
+Before filing an issue to request a new feature or device, please ensure that you will take the time to test the feature throuroughly. New features cannot be simply tested on Home Assistant. A separate integration must be created which is not part of this library. In order to test a new feature, clone the branch and install into a new virtual environment.
+
+```bash
+mkdir python_test && cd python_test
 
-SSL pinning makes capturing packets with Android ~~not feasible anymore~~ harder than before. A system-wide proxy [ProxyDroid](https://play.google.com/store/apps/details?id=org.proxydroid&hl=en) can be used if ssl pinning is disabled [TrustMeAlready](https://github.com/ViRb3/TrustMeAlready).
+# Check Python version is 3.8 or higher
+python3 --version # or python --version or python3.8 --version
+# Create a new venv
+python3 -m venv pyvesync-venv
+# Activate the venv on linux
+source pyvesync-venv/bin/activate
+# or ....
+pyvesync-venv\Scripts\activate.ps1 # on powershell
+pyvesync-venv\Scripts\activate.bat # on command prompt
+
+# Install branch to be tested into new virtual environment
+pip install git+https://github.com/webdjoe/pyvesync@BRANCHNAME
+```
+
+Test functionality with a script
+
+`test.py`
+
+```python
+import sys
+import logging
+import json
+from pyvesync import VeSync
+
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.DEBUG)
+
+def test_device():
+  # Instantiate VeSync class and login
+  manager = VeSync(user, password, debug=True)
+  if manager.login() == False
+    logger("Unable to login")
+    return
+
+  # Test specific device
+  # If this were a humidifier and there is only one humidifier/purifier
+  # You can access it with the device index
+  fan = manager.fans[0]
+  # or loop through the fan devices and test for device with "My Device" name
+  # Use lower() to avoid capitalization issues
+  my_device_name = "My Device"
+  fan = None
+  for dev in manager.fans:
+    if dev.name.lower() == my_device_name.lower()
+      fan = dev
+  if fan == None:
+    logger.debug("Device not found")
+    logger.debug("Devices found - \n" + json.dumps(manager._dev_list))
+    return
+
+  # Test all device methods and functionality
+  # Be aware some devices lose internet connectivity if turned off
+  fan.turn_on()
+  fan.turn_off()
+  fan.sleep_mode()
+
+# Make script runnable from command line
+if __name__ == "__main__":
+  logger.debug("Testing device")
+  test_device()
+...
+
+```
 
-Charles Proxy is a proxy that allows you to perform MITM SSL captures on an iOS device. This is the only way to capture packets that I am aware of that is currently possible.
+## Device Requests
 
-When capturing packets make sure all packets are captured from the device list, along with all functions that the app contains. The captured packets are stored in text files, please do not capture with pcap format.
+SSL pinning makes capturing packets much harder. In order to be able to capture packets, SSL pinning needs to be disabled before running an SSL proxy. Use an Android emulator such as Android Studio, which is available for Windows and Linux for free. Download the APK from APKPure or a similiar site and use [Objection](https://github.com/sensepost/objection) or [Frida](https://frida.re/docs/gadget/). Followed by capturing the packets with Charles Proxy or another SSL proxy application.
 
-After you capture the packets, please redact the `accountid` and `token`. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
+Be sure to capture all packets from the device list and each of the possible device menus and actions. Please redact the `accountid` and `token` from the captured packets. If you feel you must redact other keys, please do not delete them entirely. Replace letters with "A" and numbers with "1", leave all punctuation intact and maintain length.
 
 For example:
 
 Before:
 
 ```json
 {
@@ -911,12 +1001,12 @@
 {
   "tk": "AAA111AAA111==1AA",
   "accountId": "111111111",
   "cid": "AAAAAA11-1AA-AA"
 }
 ```
 
-All [contributions](CONTRIBUTING.md) are welcome, please run `tox` before submitting a PR to ensure code is valid.
+# Contributing
 
-Ensure new devices are integrated in tests, please review the [testing](tests/README.md) documentation for more information.
+All [contributions](CONTRIBUTING.md) are welcome.
 
 This project is licensed under [MIT](LICENSE).
```

### Comparing `pyvesync-2.1.7/src/pyvesync.egg-info/SOURCES.txt` & `pyvesync-2.1.8/src/pyvesync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

