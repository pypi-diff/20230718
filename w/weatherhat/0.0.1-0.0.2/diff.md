# Comparing `tmp/weatherhat-0.0.1.tar.gz` & `tmp/weatherhat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/weatherhat-0.0.1.tar", last modified: Thu Jan 27 12:02:29 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `weatherhat-0.0.1.tar` & `weatherhat-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,41 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-01-27 12:02:29.000000 weatherhat-0.0.1/
--rw-r--r--   0 pi        (1000) pi        (1000)      111 2021-07-22 07:49:48.000000 weatherhat-0.0.1/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)       31 2021-07-22 07:48:38.000000 weatherhat-0.0.1/CHANGELOG.txt
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-01-27 12:02:29.000000 weatherhat-0.0.1/weatherhat/
--rw-r--r--   0 pi        (1000) pi        (1000)     3547 2022-01-19 11:42:00.000000 weatherhat-0.0.1/weatherhat/history.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6422 2022-01-19 11:42:24.000000 weatherhat-0.0.1/weatherhat/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     7973 2022-01-27 12:02:29.000000 weatherhat-0.0.1/PKG-INFO
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-01-27 12:02:29.000000 weatherhat-0.0.1/weatherhat.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2022-01-27 12:02:29.000000 weatherhat-0.0.1/weatherhat.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      280 2022-01-27 12:02:29.000000 weatherhat-0.0.1/weatherhat.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-01-27 12:02:29.000000 weatherhat-0.0.1/weatherhat.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     7973 2022-01-27 12:02:29.000000 weatherhat-0.0.1/weatherhat.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)       50 2022-01-27 12:02:29.000000 weatherhat-0.0.1/weatherhat.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     5487 2022-01-27 11:59:41.000000 weatherhat-0.0.1/README.md
--rwxr-xr-x   0 pi        (1000) pi        (1000)     1388 2021-07-22 07:48:38.000000 weatherhat-0.0.1/setup.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2021-07-22 07:48:38.000000 weatherhat-0.0.1/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1152 2022-01-27 12:02:29.000000 weatherhat-0.0.1/setup.cfg
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 weatherhat-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 weatherhat-0.0.2/Makefile
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 weatherhat-0.0.2/README.md
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 weatherhat-0.0.2/check.sh
+-rwxr-xr-x   0        0        0     5536 2020-02-02 00:00:00.000000 weatherhat-0.0.2/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 weatherhat-0.0.2/requirements-dev.txt
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 weatherhat-0.0.2/tox.ini
+-rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 weatherhat-0.0.2/uninstall.sh
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/BME280-compensated.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/BME280.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/adafruit-io.py
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/averaging.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/basic.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/buttons.py
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/lcd.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/settings.yml
+-rw-r--r--   0        0        0    21514 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/weather.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-alarm.png
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-backdrop.png
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-channel.png
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-circle.png
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-drop.png
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-help.png
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-nodrop.png
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-return.png
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-rightarrow.png
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-settings.png
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-snooze.png
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 weatherhat-0.0.2/examples/icons/icon-warningdrop.png
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 weatherhat-0.0.2/testing/RPi/GPIO/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 weatherhat-0.0.2/testing/ST7789/__init__.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 weatherhat-0.0.2/testing/weatherhat/__init__.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 weatherhat-0.0.2/testing/weatherhat/history.py -> ../../weatherhat/history.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 weatherhat-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 weatherhat-0.0.2/tests/test_setup.py
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 weatherhat-0.0.2/weatherhat/__init__.py
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 weatherhat-0.0.2/weatherhat/history.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 weatherhat-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 weatherhat-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 weatherhat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 weatherhat-0.0.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `weatherhat-0.0.1/weatherhat/history.py` & `weatherhat-0.0.2/weatherhat/history.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,25 @@
     135: "South East",
     180: "South",
     225: "South West",
     270: "West",
     315: "North West"
 }
 
+wind_degrees_to_short_cardinal = {
+    0: "N",
+    45: "NE",
+    90: "E",
+    135: "SE",
+    180: "S",
+    225: "SW",
+    270: "W",
+    315: "NW"
+}
+
 
 class HistoryEntry:
     __slots__ = 'value', 'timestamp'
 
     def __init__(self, value, timestamp=None):
         self.timestamp = timestamp if timestamp is not None else time.time()
         self.value = value
@@ -80,18 +91,18 @@
         return self.ms_to_kmph(self.gust(seconds))
 
     def ms_to_mph(self, ms):
         """Convert meters/second to miles/hour."""
         return ((ms * 60 * 60) / 1000.0) * 0.621371
 
     def latest_mph(self):
-        return self.cms_to_mph(self.latest().value)
+        return self.ms_to_mph(self.latest().value)
 
     def average_mph(self, sample_over=None):
-        return self.cms_to_mph(self.average(sample_over))
+        return self.ms_to_mph(self.average(sample_over))
 
     def gust_mph(self, seconds=3.0):
         """Wind gust in miles/hour."""
         return self.ms_to_mph(self.gust(seconds))
 
     def gust(self, seconds=3.0):
         """Wind gust in meters/second."""
@@ -101,15 +112,28 @@
 
 
 class WindDirectionHistory(History):
     def degrees_to_cardinal(self, degrees):
         value, cardinal = min(wind_degrees_to_cardinal.items(), key=lambda item: abs(item[0] - degrees))
         return cardinal
 
+    def degrees_to_short_cardinal(self, degrees):
+        value, cardinal = min(wind_degrees_to_short_cardinal.items(), key=lambda item: abs(item[0] - degrees))
+        return cardinal
+
     def average_compass(self, sample_over=None):
         return self.degrees_to_cardinal(self.average(sample_over))
 
+    def average_short_compass(self, sample_over=None):
+        return self.degrees_to_short_cardinal(self.average(sample_over))
+
     def latest_compass(self):
         return self.degrees_to_cardinal(self.latest().value)
 
+    def latest_short_compass(self):
+        return self.degrees_to_short_cardinal(self.latest().value)
+
     def history_compass(self, depth=None):
         return [HistoryEntry(self.degrees_to_cardinal(entry.value), timestamp=entry.timestamp) for entry in self.history(depth)]
+
+    def history_short_compass(self, depth=None):
+        return [HistoryEntry(self.degrees_to_short_cardinal(entry.value), timestamp=entry.timestamp) for entry in self.history(depth)]
```

### Comparing `weatherhat-0.0.1/weatherhat/__init__.py` & `weatherhat-0.0.2/weatherhat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-import time
-import threading
 import math
+import threading
+import time
 
-import RPi.GPIO as GPIO
 import ioexpander as io
+import RPi.GPIO as GPIO
 from bme280 import BME280
 from ltr559 import LTR559
 from smbus2 import SMBus
 
 from .history import wind_degrees_to_cardinal
 
-
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 
 # Wind Vane
 PIN_WV = 8     # P0.3 ANE6
 
 # Anemometer
 PIN_ANE1 = 5       # P0.0
@@ -79,30 +78,30 @@
         self._ioe.output(PIN_R3, 0)
         self._ioe.set_pin_interrupt(PIN_R4, True)
         self._ioe.on_interrupt(self.handle_ioe_interrupt)
         self._ioe.clear_interrupt()
 
         # Data API... kinda
         self.temperature_offset = -7.5
-        self.device_temperature = 0
-        self.temperature = 0
+        self.device_temperature = 0.0
+        self.temperature = 0.0
 
-        self.pressure = 0
+        self.pressure = 0.0
 
-        self.humidity = 0
-        self.relative_humidity = 0
-        self.dewpoint = 0
+        self.humidity = 0.0
+        self.relative_humidity = 0.0
+        self.dewpoint = 0.0
 
-        self.lux = 0
+        self.lux = 0.0
 
-        self.wind_speed = 0
-        self.wind_direction = 0
+        self.wind_speed = 0.0
+        self.wind_direction = 0.0
 
-        self.rain = 0
-        self.rain_total = 0
+        self.rain = 0.0
+        self.rain_total = 0.0
 
         self.reset_counts()
 
     def reset_counts(self):
         self._lock.acquire(blocking=True)
         self._ioe.clear_switch_counter(PIN_ANE2)
         self._ioe.clear_switch_counter(PIN_R4)
@@ -125,24 +124,24 @@
         return min(100, max(0, corrected_humidity))
 
     def get_dewpoint(self, humidity, temperature):
         """Calculate Dewpoint."""
         return temperature - ((100 - humidity) / 5)
 
     def hpa_to_inches(self, hpa):
-        """Convert hextopascals to inches of mercury."""
+        """Convert hectopascals to inches of mercury."""
         return hpa * 0.02953
 
     def degrees_to_cardinal(self, degrees):
         value, cardinal = min(wind_degrees_to_cardinal.items(), key=lambda item: abs(item[0] - degrees))
         return cardinal
 
     def update(self, interval=60.0):
         # Time elapsed since last update
-        delta = time.time() - self._t_start
+        delta = float(time.time() - self._t_start)
 
         self.updated_wind_rain = False
 
         # Always update TPHL & Wind Direction
         self._lock.acquire(blocking=True)
 
         self.device_temperature = self._bme280.get_temperature()
```

### Comparing `weatherhat-0.0.1/PKG-INFO` & `weatherhat-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,239 +1,219 @@
-Metadata-Version: 2.1
-Name: weatherhat
-Version: 0.0.1
-Summary: Library for Weather HAT
-Home-page: https://www.pimoroni.com
-Author: Philip Howard
-Author-email: phil@pimoroni.com
-License: MIT
-Project-URL: GitHub, https://www.github.com/pimoroni/weatherhat-python
-Description: # Weather HAT Python Library & Examples
-        
-        [![Build Status](https://shields.io/github/workflow/status/pimoroni/weatherhat-python/Python%20Tests.svg)](https://github.com/pimoroni/weatherhat-python/actions/workflows/test.yml)
-        [![Coverage Status](https://coveralls.io/repos/github/pimoroni/weatherhat-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/weatherhat-python?branch=master)
-        [![PyPi Package](https://img.shields.io/pypi/v/weatherhat.svg)](https://pypi.python.org/pypi/weatherhat)
-        [![Python Versions](https://img.shields.io/pypi/pyversions/weatherhat.svg)](https://pypi.python.org/pypi/weatherhat)
-        
-        # Pre-requisites
-        
-        You must enable:
-        
-        * i2c: `sudo raspi-config nonint do_i2c 0`
-        * spi: `sudo raspi-config nonint do_spi 0`
-        
-        You can optionally run `sudo raspi-config` or the graphical Raspberry Pi Configuration UI to enable interfaces.
-        
-        # Installing
-        
-        Stable library from PyPi:
-        
-        * Just run `pip3 install weatherhat`
-        
-        In some cases you may need to use `sudo` or install pip with: `sudo apt install python3-pip`
-        
-        Latest/development library from GitHub:
-        
-        * `git clone https://github.com/pimoroni/weatherhat-python`
-        * `cd weatherhat-python`
-        * `sudo ./install.sh`
-        
-        Some of the examples use additional libraries. You can install them with:
-        
-        ```bash
-        pip3 install fonts font-manrope pyyaml adafruit-io
-        ```
-        
-        # Using The Library
-        
-        Import the `weatherhat` module and create an instance of the `WeatherHAT` class.
-        
-        ```python
-        import weatherhat
-        
-        sensor = weatherhat.WeatherHAT()
-        ```
-        
-        Weather HAT updates the sensors when you call `update(interval=5)`.
-        
-        Temperature, pressure, humidity, light and wind direction are updated continuously.
-        
-        Rain and Wind measurements are measured over an `interval` period. Weather HAT will count ticks of the rain gauge and (half) rotations of the anemometer, calculate rain/wind every `interval` seconds and reset the counts for the next pass.
-        
-        For example the following code will update rain/wind speed every 5 seconds, and all other readings will be updated on demand:
-        
-        ```python
-        import time
-        import weatherhat
-        
-        sensor = weatherhat.WeatherHAT()
-        
-        while True:
-            sensor.update(interval=5.0)
-            time.sleep(1.0)
-        ```
-        
-        # Averaging Readings
-        
-        The Weather HAT library supplies set of "history" classes intended to save readings over a period of time and provide access to things like minimum, maximum and average values with unit conversions.
-        
-        For example `WindSpeedHistory` allows you to store wind readings and retrieve them in mp/h or km/h, in addition to determining the "gust" (maximum wind speed) in a given period of time:
-        
-        ```python
-        import time
-        import weatherhat
-        from weatherhat.history import WindSpeedHistory
-        
-        sensor = weatherhat.WeatherHAT()
-        wind_speed_history = WindSpeedHistory()
-        
-        while True:
-            sensor.update(interval=5.0)
-            if sensor.updated_wind_rain:
-                wind_speed_history.append(sensor.wind_speed)
-                print(f"Average wind speed: {wind_speed_history.average_mph()}mph")
-                print(f"Wind gust: {wind_speed_history.gust_mph()}mph")
-            time.sleep(1.0)
-        ```
-        
-        # Quick Reference
-        
-        ## Temperature
-        
-        Temperature readings are given as degrees celsius and are measured from the Weather HAT's onboard BME280.
-        
-        ### Device Temperature
-        
-        ```python
-        sensor.device_temperature
-        ```
-        
-        Device temperature in degrees celsius.
-        
-        This is the temperature read directly from the BME280 onboard Weather HAT. It's not compensated and tends to read slightly higher than ambient due to heat from the Pi.
-        
-        ### Compensated (Air) Temperature
-        
-        ```python
-        sensor.temperature
-        ```
-        
-        Temperature in degrees celsius.
-        
-        This is the temperature once an offset has been applied. This offset is fixed, and taken from `sensor.temperature_offset`.
-        
-        ## Pressure
-        
-        ```python
-        sensor.pressure
-        ```
-        
-        Pressure in hectopascals.
-        
-        ## Humidity
-        
-        ```python
-        sensor.humidity
-        ```
-        
-        Humidity in %.
-        
-        ### Relative Humidity
-        
-        ```python
-        sensor.relative_humidity
-        ```
-        
-        Relative humidity in %.
-        
-        Relative humidity is the water content of the air compensated for temperature, since warmer air can hold more water.
-        
-        It's expressed as a percentage from 0 (no moisture) to 100 (fully saturated).
-        
-        ### Dew Point
-        
-        ```python
-        sensor.dewpoint
-        ```
-        
-        Dew point in degrees celsius.
-        
-        Dew point is the temperature at which water - at the current humidity - will condense out of the air.
-        
-        ## Light / Lux
-        
-        ```python
-        sensor.lux
-        ```
-        
-        Light is given in lux.
-        
-        Lux ranges from 0 (complete darkness) to.
-        
-        ## Wind
-        
-        Both wind and rain are updated on an interval, rather than on-demand.
-        
-        To see if an `update()` call has resulted in new wind/rain measurements, check:
-        
-        ```python
-        sensor.updated_wind_rain
-        ```
-        
-        ### Wind Direction
-        
-        ```python
-        sensor.wind_direction
-        ```
-        
-        Wind direction in degrees.
-        
-        Wind direction is measured using a potentiometer and uses an analog reading internally. This is converted to degrees for convenience, and will snap to the nearest 45-degree increment with 0 degrees indicating North.
-        
-        ### Wind Speed
-        
-        ```python
-        sensor.wind_speed
-        ```
-        
-        Wind speed in meters per second.
-        
-        Weather HAT counts every half rotation and converts this to cm/s using the anemometer circumference and factor.
-        
-        It's updated depending on the update interval requested.
-        
-        ## Rain
-        
-        ```python
-        sensor.rain
-        ```
-        
-        Rain amount in millimeters per second.
-        
-        Weather HAT counts every "tick" of the rain gauge (roughly .28mm) over the given update internal and converts this into mm/sec.
-        
-        ### Total Rain
-        
-        ```python
-        sensor.rain_total
-        ```
-        
-        Total rain amount in millimeters for the current update period.
-        
-        # Changelog
-        0.0.1
-        -----
-        
-        * Initial Release
-        
-Keywords: Raspberry Pi
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: System :: Hardware
-Requires-Python: >= 3.6
-Description-Content-Type: text/markdown
+# Weather HAT Python Library & Examples
+
+[![Build Status](https://img.shields.io/github/actions/workflow/status/pimoroni/weatherhat-python/test.yml?branch=main)](https://github.com/pimoroni/weatherhat-python/actions/workflows/test.yml)
+[![Coverage Status](https://coveralls.io/repos/github/pimoroni/weatherhat-python/badge.svg?branch=master)](https://coveralls.io/github/pimoroni/weatherhat-python?branch=master)
+[![PyPi Package](https://img.shields.io/pypi/v/weatherhat.svg)](https://pypi.python.org/pypi/weatherhat)
+[![Python Versions](https://img.shields.io/pypi/pyversions/weatherhat.svg)](https://pypi.python.org/pypi/weatherhat)
+
+# Pre-requisites
+
+This library requires Python ≥3.6 so we'd recommend using it with Raspberry Pi OS Buster or later.
+
+You must enable:
+
+* i2c: `sudo raspi-config nonint do_i2c 0`
+* spi: `sudo raspi-config nonint do_spi 0`
+
+You can optionally run `sudo raspi-config` or the graphical Raspberry Pi Configuration UI to enable interfaces.
+
+# Installing
+
+Stable library from PyPi:
+
+* Just run `pip3 install weatherhat`
+
+In some cases you may need to use `sudo` or install pip with: `sudo apt install python3-pip`
+
+Latest/development library from GitHub:
+
+* `git clone https://github.com/pimoroni/weatherhat-python`
+* `cd weatherhat-python`
+* `./install.sh --unstable`
+
+Some of the examples use additional libraries. You can install them with:
+
+```bash
+pip3 install fonts font-manrope pyyaml adafruit-io numpy
+```
+
+You may also need to install `libatlas-base-dev`
+
+```
+sudo apt-get install libatlas-base-dev
+```
+
+# Using The Library
+
+Import the `weatherhat` module and create an instance of the `WeatherHAT` class.
+
+```python
+import weatherhat
+
+sensor = weatherhat.WeatherHAT()
+```
+
+Weather HAT updates the sensors when you call `update(interval=5)`.
+
+Temperature, pressure, humidity, light and wind direction are updated continuously.
+
+Rain and Wind measurements are measured over an `interval` period. Weather HAT will count ticks of the rain gauge and (half) rotations of the anemometer, calculate rain/wind every `interval` seconds and reset the counts for the next pass.
+
+For example the following code will update rain/wind speed every 5 seconds, and all other readings will be updated on demand:
+
+```python
+import time
+import weatherhat
+
+sensor = weatherhat.WeatherHAT()
+
+while True:
+    sensor.update(interval=5.0)
+    time.sleep(1.0)
+```
+
+# Averaging Readings
+
+The Weather HAT library supplies set of "history" classes intended to save readings over a period of time and provide access to things like minimum, maximum and average values with unit conversions.
+
+For example `WindSpeedHistory` allows you to store wind readings and retrieve them in mp/h or km/h, in addition to determining the "gust" (maximum wind speed) in a given period of time:
+
+```python
+import time
+import weatherhat
+from weatherhat.history import WindSpeedHistory
+
+sensor = weatherhat.WeatherHAT()
+wind_speed_history = WindSpeedHistory()
+
+while True:
+    sensor.update(interval=5.0)
+    if sensor.updated_wind_rain:
+        wind_speed_history.append(sensor.wind_speed)
+        print(f"Average wind speed: {wind_speed_history.average_mph()}mph")
+        print(f"Wind gust: {wind_speed_history.gust_mph()}mph")
+    time.sleep(1.0)
+```
+
+# Quick Reference
+
+## Temperature
+
+Temperature readings are given as degrees celsius and are measured from the Weather HAT's onboard BME280.
+
+### Device Temperature
+
+```python
+sensor.device_temperature
+```
+
+Device temperature in degrees celsius.
+
+This is the temperature read directly from the BME280 onboard Weather HAT. It's not compensated and tends to read slightly higher than ambient due to heat from the Pi.
+
+### Compensated (Air) Temperature
+
+```python
+sensor.temperature
+```
+
+Temperature in degrees celsius.
+
+This is the temperature once an offset has been applied. This offset is fixed, and taken from `sensor.temperature_offset`.
+
+## Pressure
+
+```python
+sensor.pressure
+```
+
+Pressure in hectopascals.
+
+## Humidity
+
+```python
+sensor.humidity
+```
+
+Humidity in %.
+
+### Relative Humidity
+
+```python
+sensor.relative_humidity
+```
+
+Relative humidity in %.
+
+Relative humidity is the water content of the air compensated for temperature, since warmer air can hold more water.
+
+It's expressed as a percentage from 0 (no moisture) to 100 (fully saturated).
+
+### Dew Point
+
+```python
+sensor.dewpoint
+```
+
+Dew point in degrees celsius.
+
+Dew point is the temperature at which water - at the current humidity - will condense out of the air.
+
+## Light / Lux
+
+```python
+sensor.lux
+```
+
+Light is given in lux.
+
+Lux ranges from 0 (complete darkness) to 64,000 (full brightness).
+
+## Wind
+
+Both wind and rain are updated on an interval, rather than on-demand.
+
+To see if an `update()` call has resulted in new wind/rain measurements, check:
+
+```python
+sensor.updated_wind_rain
+```
+
+### Wind Direction
+
+```python
+sensor.wind_direction
+```
+
+Wind direction in degrees.
+
+Wind direction is measured using a potentiometer and uses an analog reading internally. This is converted to degrees for convenience, and will snap to the nearest 45-degree increment with 0 degrees indicating North.
+
+### Wind Speed
+
+```python
+sensor.wind_speed
+```
+
+Wind speed in meters per second.
+
+Weather HAT counts every half rotation and converts this to cm/s using the anemometer circumference and factor.
+
+It's updated depending on the update interval requested.
+
+## Rain
+
+```python
+sensor.rain
+```
+
+Rain amount in millimeters per second.
+
+Weather HAT counts every "tick" of the rain gauge (roughly .28mm) over the given update internal and converts this into mm/sec.
+
+### Total Rain
+
+```python
+sensor.rain_total
+```
+
+Total rain amount in millimeters for the current update period.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `weatherhat-0.0.1/setup.py` & `weatherhat-0.0.2/LICENSE`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-"""
-Copyright (c) 2016 Pimoroni
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
-of the Software, and to permit persons to whom the Software is furnished to do
-so, subject to the following conditions:
+Copyright (c) 2018 Pimoroni Ltd.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-"""
-
-from setuptools import setup, __version__
-from pkg_resources import parse_version
-
-minimum_version = parse_version('30.4.0')
-
-if parse_version(__version__) < minimum_version:
-    raise RuntimeError("Package setuptools must be at least version {}".format(minimum_version))
-
-setup()
```

