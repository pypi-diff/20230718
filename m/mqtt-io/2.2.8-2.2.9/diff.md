# Comparing `tmp/mqtt_io-2.2.8.tar.gz` & `tmp/mqtt_io-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqtt_io-2.2.8.tar", max compression
+gzip compressed data, was "mqtt_io-2.2.9.tar", max compression
```

## Comparing `mqtt_io-2.2.8.tar` & `mqtt_io-2.2.9.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0     1081 2023-01-19 15:54:10.684873 mqtt_io-2.2.8/LICENSE
--rw-r--r--   0        0        0     3798 2023-01-19 15:54:10.684873 mqtt_io-2.2.8/README.md
--rw-r--r--   0        0        0       57 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/__init__.py
--rw-r--r--   0        0        0     3313 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/__main__.py
--rw-r--r--   0        0        0     7815 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/config/__init__.py
--rw-r--r--   0        0        0    34554 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/config/config.schema.yml
--rw-r--r--   0        0        0      421 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/config/validation/__init__.py
--rw-r--r--   0        0        0     4067 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/config/validation/gpio.py
--rw-r--r--   0        0        0     1148 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/config.sockets.yml
--rw-r--r--   0        0        0      426 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/constants.py
--rw-r--r--   0        0        0     3759 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/events.py
--rw-r--r--   0        0        0      531 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/exceptions.py
--rw-r--r--   0        0        0     4759 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/home_assistant.py
--rw-r--r--   0        0        0     1694 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/__init__.py
--rw-r--r--   0        0        0    12250 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/__init__.py
--rw-r--r--   0        0        0     1507 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/beaglebone.py
--rw-r--r--   0        0        0     1790 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/dockerpi.py
--rw-r--r--   0        0        0     6531 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/gpiod.py
--rw-r--r--   0        0        0     3335 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/gpiozero.py
--rw-r--r--   0        0        0     3792 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/mcp23017.py
--rw-r--r--   0        0        0     2794 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/mock.py
--rw-r--r--   0        0        0     1954 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/orangepi.py
--rw-r--r--   0        0        0     1549 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/pcf8574.py
--rw-r--r--   0        0        0     1549 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/pcf8575.py
--rw-r--r--   0        0        0      968 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/piface2.py
--rw-r--r--   0        0        0     2808 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/raspberrypi.py
--rw-r--r--   0        0        0     1283 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/gpio/stdio.py
--rw-r--r--   0        0        0     1722 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/__init__.py
--rw-r--r--   0        0        0     2802 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/ads1x15.py
--rw-r--r--   0        0        0     1597 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/aht20.py
--rw-r--r--   0        0        0     2062 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/bh1750.py
--rw-r--r--   0        0        0     1711 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/bme280.py
--rw-r--r--   0        0        0     2341 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/bme680.py
--rw-r--r--   0        0        0     2211 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/dht22.py
--rw-r--r--   0        0        0     1370 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/ds18b.py
--rw-r--r--   0        0        0     4235 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/hcsr04.py
--rw-r--r--   0        0        0     3539 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/ina219.py
--rw-r--r--   0        0        0     1054 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/lm75.py
--rw-r--r--   0        0        0     1409 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/mcp3008.py
--rw-r--r--   0        0        0     6936 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/mcp3xxx.py
--rw-r--r--   0        0        0      967 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/sensor/mock.py
--rw-r--r--   0        0        0     1615 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/stream/__init__.py
--rw-r--r--   0        0        0     1911 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/stream/pn532.py
--rw-r--r--   0        0        0     2493 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/modules/stream/serial.py
--rw-r--r--   0        0        0     3830 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/mqtt/__init__.py
--rw-r--r--   0        0        0     3834 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/mqtt/asyncio_mqtt.py
--rw-r--r--   0        0        0    52312 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/server.py
--rw-r--r--   0        0        0     7587 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/tests/features/config_main_invalid.feature
--rw-r--r--   0        0        0     2244 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/tests/features/config_main_valid.feature
--rw-r--r--   0        0        0      691 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/tests/features/config_module_gpio_invalid.feature
--rw-r--r--   0        0        0      659 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/tests/features/config_module_gpio_valid.feature
--rw-r--r--   0        0        0      760 2023-01-19 15:54:10.688873 mqtt_io-2.2.8/mqtt_io/tests/features/environment.py
--rw-r--r--   0        0        0     8510 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/module_gpio_runtime.feature
--rw-r--r--   0        0        0       63 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/server_init.feature
--rw-r--r--   0        0        0    13428 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/server_init_gpio.feature
--rw-r--r--   0        0        0      836 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/server_init_sensor.feature
--rw-r--r--   0        0        0     2134 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/steps/config_main.py
--rw-r--r--   0        0        0     2930 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/steps/events.py
--rw-r--r--   0        0        0     7714 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/steps/module_gpio.py
--rw-r--r--   0        0        0     6356 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/tests/features/steps/server.py
--rw-r--r--   0        0        0      327 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/types.py
--rw-r--r--   0        0        0     1099 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/mqtt_io/utils.py
--rw-r--r--   0        0        0     1053 2023-01-19 15:54:10.692873 mqtt_io-2.2.8/pyproject.toml
--rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 mqtt_io-2.2.8/setup.py
--rw-r--r--   0        0        0     4977 1970-01-01 00:00:00.000000 mqtt_io-2.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-18 19:12:06.087965 mqtt_io-2.2.9/LICENSE
+-rw-r--r--   0        0        0     4299 2023-07-18 19:12:06.087965 mqtt_io-2.2.9/README.md
+-rw-r--r--   0        0        0       57 2023-07-18 19:12:06.087965 mqtt_io-2.2.9/mqtt_io/__init__.py
+-rw-r--r--   0        0        0     3313 2023-07-18 19:12:06.087965 mqtt_io-2.2.9/mqtt_io/__main__.py
+-rw-r--r--   0        0        0     7815 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/config/__init__.py
+-rw-r--r--   0        0        0    34554 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/config/config.schema.yml
+-rw-r--r--   0        0        0      421 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/config/validation/__init__.py
+-rw-r--r--   0        0        0     4067 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/config/validation/gpio.py
+-rw-r--r--   0        0        0     1148 2023-07-18 19:12:06.087965 mqtt_io-2.2.9/mqtt_io/config.sockets.yml
+-rw-r--r--   0        0        0      426 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/constants.py
+-rw-r--r--   0        0        0     3759 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/events.py
+-rw-r--r--   0        0        0      531 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/exceptions.py
+-rw-r--r--   0        0        0     4759 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/home_assistant.py
+-rw-r--r--   0        0        0     1694 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/__init__.py
+-rw-r--r--   0        0        0    12250 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/__init__.py
+-rw-r--r--   0        0        0     1507 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/beaglebone.py
+-rw-r--r--   0        0        0     1790 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/dockerpi.py
+-rw-r--r--   0        0        0     6531 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/gpiod.py
+-rw-r--r--   0        0        0     3335 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/gpiozero.py
+-rw-r--r--   0        0        0     3792 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/mcp23017.py
+-rw-r--r--   0        0        0     2794 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/mock.py
+-rw-r--r--   0        0        0     1954 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/orangepi.py
+-rw-r--r--   0        0        0     1566 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/pcf8574.py
+-rw-r--r--   0        0        0     1566 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/pcf8575.py
+-rw-r--r--   0        0        0      968 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/piface2.py
+-rw-r--r--   0        0        0     2808 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/raspberrypi.py
+-rw-r--r--   0        0        0     1283 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/gpio/stdio.py
+-rw-r--r--   0        0        0     1722 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/__init__.py
+-rw-r--r--   0        0        0     2791 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/ads1x15.py
+-rw-r--r--   0        0        0     1597 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/aht20.py
+-rw-r--r--   0        0        0     2062 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/bh1750.py
+-rw-r--r--   0        0        0     1711 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/bme280.py
+-rw-r--r--   0        0        0     2341 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/bme680.py
+-rw-r--r--   0        0        0     2211 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/dht22.py
+-rw-r--r--   0        0        0     1370 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/ds18b.py
+-rw-r--r--   0        0        0     4235 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/hcsr04.py
+-rw-r--r--   0        0        0     3539 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/ina219.py
+-rw-r--r--   0        0        0     1054 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/lm75.py
+-rw-r--r--   0        0        0     1409 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/mcp3008.py
+-rw-r--r--   0        0        0     6936 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/mcp3xxx.py
+-rw-r--r--   0        0        0      967 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/sensor/mock.py
+-rw-r--r--   0        0        0     1615 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/stream/__init__.py
+-rw-r--r--   0        0        0     1911 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/stream/pn532.py
+-rw-r--r--   0        0        0     2493 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/modules/stream/serial.py
+-rw-r--r--   0        0        0     3830 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/mqtt/__init__.py
+-rw-r--r--   0        0        0     3834 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/mqtt/asyncio_mqtt.py
+-rw-r--r--   0        0        0    53874 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/server.py
+-rw-r--r--   0        0        0     7587 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/config_main_invalid.feature
+-rw-r--r--   0        0        0     2244 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/config_main_valid.feature
+-rw-r--r--   0        0        0      691 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/config_module_gpio_invalid.feature
+-rw-r--r--   0        0        0      659 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/config_module_gpio_valid.feature
+-rw-r--r--   0        0        0      760 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/environment.py
+-rw-r--r--   0        0        0     8510 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/module_gpio_runtime.feature
+-rw-r--r--   0        0        0       63 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/server_init.feature
+-rw-r--r--   0        0        0    13428 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/server_init_gpio.feature
+-rw-r--r--   0        0        0      836 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/server_init_sensor.feature
+-rw-r--r--   0        0        0     2134 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/steps/config_main.py
+-rw-r--r--   0        0        0     2930 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/steps/events.py
+-rw-r--r--   0        0        0     7714 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/steps/module_gpio.py
+-rw-r--r--   0        0        0     6356 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/tests/features/steps/server.py
+-rw-r--r--   0        0        0      327 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/types.py
+-rw-r--r--   0        0        0     1099 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/mqtt_io/utils.py
+-rw-r--r--   0        0        0     1053 2023-07-18 19:12:06.091966 mqtt_io-2.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5478 1970-01-01 00:00:00.000000 mqtt_io-2.2.9/PKG-INFO
```

### Comparing `mqtt_io-2.2.8/LICENSE` & `mqtt_io-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/README.md` & `mqtt_io-2.2.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -97,21 +97,40 @@
 # Sensors
 sensor_modules:
   # An LM75 sensor attached to the I2C bus
   - name: lm75_sensor
     module: lm75
     i2c_bus_num: 1
     chip_addr: 0x48
+  # An INA219 sensor attached to the I2C bus
+  - name: ina219_sensor
+    module: ina219
+    i2c_bus_num: 1
+    chip_addr: 0x43
+
 
 sensor_inputs:
-  # The configuration of the specific sensor value to use (LM75 only has temperature)
+  # lm75 - The configuration of the specific sensor value to use (LM75 only has temperature)
   - name: porch_temperature
     module: lm75_sensor
+  # ina219 - The configuration of the specific sensor value to use (4 options for the ina219 sensor)
+  - name: power
+    type: power
+    module: ina219_sensor
+  - name: bus_voltage
+    type: bus_voltage
+    module: ina219_sensor
+  - name: current
+    type: current
+    module: ina219_sensor
+  - name: shunt_voltage
+    type: shunt_voltage
+    module: ina219_sensor
 
 # Streams
 stream_modules:
   # A serial port to communicate with the house alarm system
   - name: alarm_system
     module: serial
     device: /dev/ttyUSB0
     baud: 9600
-```
+```
```

### Comparing `mqtt_io-2.2.8/mqtt_io/__main__.py` & `mqtt_io-2.2.9/mqtt_io/__main__.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/config/__init__.py` & `mqtt_io-2.2.9/mqtt_io/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/config/config.schema.yml` & `mqtt_io-2.2.9/mqtt_io/config/config.schema.yml`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/config/validation/gpio.py` & `mqtt_io-2.2.9/mqtt_io/config/validation/gpio.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/config.sockets.yml` & `mqtt_io-2.2.9/mqtt_io/config.sockets.yml`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/events.py` & `mqtt_io-2.2.9/mqtt_io/events.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/exceptions.py` & `mqtt_io-2.2.9/mqtt_io/exceptions.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/home_assistant.py` & `mqtt_io-2.2.9/mqtt_io/home_assistant.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/__init__.py` & `mqtt_io-2.2.9/mqtt_io/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/__init__.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/beaglebone.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/beaglebone.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/dockerpi.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/dockerpi.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/gpiod.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/gpiod.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/gpiozero.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/gpiozero.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/mcp23017.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/mcp23017.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/mock.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/mock.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/orangepi.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/orangepi.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/pcf8574.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/pcf8575.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
-PCF8574 IO expander
+PCF8575 IO expander
 """
 
 from typing import Optional, cast
 
 from ...types import ConfigType, PinType
 from . import GenericGPIO, PinDirection, PinPUD
 
-REQUIREMENTS = ("pcf8574",)
+REQUIREMENTS = ("pcf8575",)
 CONFIG_SCHEMA = {
     "i2c_bus_num": {"type": "integer", "required": True, "empty": False},
     "chip_addr": {"type": "integer", "required": True, "empty": False},
 }
 
 
 class GPIO(GenericGPIO):
     """
-    Implementation of GPIO class for the PCF8574 IO expander chip.
+    Implementation of GPIO class for the pcf8575 IO expander chip.
     """
 
     def setup_module(self) -> None:
         # pylint: disable=import-outside-toplevel,import-error
         # pylint: disable=no-name-in-module
         self.pullup_map = {PinPUD.OFF: None, PinPUD.UP: True, PinPUD.DOWN: False}
-        from pcf8574 import PCF8574  # type: ignore
+        from pcf8575 import PCF8575  # type: ignore
 
-        self.io = PCF8574(self.config["i2c_bus_num"], self.config["chip_addr"])
+        self.io = PCF8575(self.config["i2c_bus_num"], self.config["chip_addr"])
 
     def setup_pin(
         self,
         pin: PinType,
         direction: PinDirection,
         pullup: PinPUD,
         pin_config: ConfigType,
         initial: Optional[str] = None,
     ) -> None:
-        if direction == PinDirection.INPUT and pullup is not None:
+        if direction == PinDirection.INPUT and self.pullup_map[pullup] is not None:
             self.io.port[pin] = self.pullup_map[pullup]
         initial = pin_config.get("initial")
         if initial is not None:
             if initial == "high":
                 self.set_pin(pin, True)
             elif initial == "low":
                 self.set_pin(pin, False)
```

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/pcf8575.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/pcf8574.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
-PCF8575 IO expander
+PCF8574 IO expander
 """
 
 from typing import Optional, cast
 
 from ...types import ConfigType, PinType
 from . import GenericGPIO, PinDirection, PinPUD
 
-REQUIREMENTS = ("pcf8575",)
+REQUIREMENTS = ("pcf8574",)
 CONFIG_SCHEMA = {
     "i2c_bus_num": {"type": "integer", "required": True, "empty": False},
     "chip_addr": {"type": "integer", "required": True, "empty": False},
 }
 
 
 class GPIO(GenericGPIO):
     """
-    Implementation of GPIO class for the pcf8575 IO expander chip.
+    Implementation of GPIO class for the PCF8574 IO expander chip.
     """
 
     def setup_module(self) -> None:
         # pylint: disable=import-outside-toplevel,import-error
         # pylint: disable=no-name-in-module
         self.pullup_map = {PinPUD.OFF: None, PinPUD.UP: True, PinPUD.DOWN: False}
-        from pcf8575 import PCF8575  # type: ignore
+        from pcf8574 import PCF8574  # type: ignore
 
-        self.io = PCF8575(self.config["i2c_bus_num"], self.config["chip_addr"])
+        self.io = PCF8574(self.config["i2c_bus_num"], self.config["chip_addr"])
 
     def setup_pin(
         self,
         pin: PinType,
         direction: PinDirection,
         pullup: PinPUD,
         pin_config: ConfigType,
         initial: Optional[str] = None,
     ) -> None:
-        if direction == PinDirection.INPUT and pullup is not None:
+        if direction == PinDirection.INPUT and self.pullup_map[pullup] is not None:
             self.io.port[pin] = self.pullup_map[pullup]
         initial = pin_config.get("initial")
         if initial is not None:
             if initial == "high":
                 self.set_pin(pin, True)
             elif initial == "low":
                 self.set_pin(pin, False)
```

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/piface2.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/piface2.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/raspberrypi.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/raspberrypi.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/gpio/stdio.py` & `mqtt_io-2.2.9/mqtt_io/modules/gpio/stdio.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/__init__.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/ads1x15.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/ads1x15.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,17 @@
         type="string",
         required=True,
         empty=False,
         allowed=SENSOR_TYPES,
     ),
     "pins": dict(type="list", required=True, empty=False, allowed=[0, 1, 2, 3]),
     "gain": dict(
-        type="integer",
         required=False,
         empty=False,
-        allowed=[2 / 3, 1, 2, 4, 8, 16],
+        allowed=[0.6666666666666666, 1, 2, 4, 8, 16],
         default=1,
     ),
 }
 
 
 class Sensor(GenericSensor):
     """
```

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/aht20.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/aht20.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/bh1750.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/bh1750.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/bme280.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/bme280.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/bme680.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/bme680.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/dht22.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/dht22.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/ds18b.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/ds18b.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/hcsr04.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/hcsr04.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/ina219.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/ina219.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/lm75.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/lm75.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/mcp3008.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/mcp3008.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/mcp3xxx.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/mcp3xxx.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/sensor/mock.py` & `mqtt_io-2.2.9/mqtt_io/modules/sensor/mock.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/stream/__init__.py` & `mqtt_io-2.2.9/mqtt_io/modules/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/stream/pn532.py` & `mqtt_io-2.2.9/mqtt_io/modules/stream/pn532.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/modules/stream/serial.py` & `mqtt_io-2.2.9/mqtt_io/modules/stream/serial.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/mqtt/__init__.py` & `mqtt_io-2.2.9/mqtt_io/mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/mqtt/asyncio_mqtt.py` & `mqtt_io-2.2.9/mqtt_io/mqtt/asyncio_mqtt.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/server.py` & `mqtt_io-2.2.9/mqtt_io/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1043,14 +1043,43 @@
                 await entry.coro
             except MQTTException:
                 raise
             except Exception:  # pylint: disable=broad-except
                 _LOG.exception("Exception while handling MQTT task:")
             self.mqtt_task_queue.task_done()
 
+    async def _mqtt_keep_alive_loop(self) -> None:
+        """
+        Publish a message on the status topic regularly to keep the connection alive.
+        This is a workaround for 2 different problems:
+        - keepalive was not implemented in early versions of asyncio_mqtt
+        - due to the way we receive messages asynchronously in our own queue we are not able
+          to capture the disconnected exception and trigger the reconnection. This publish call
+          will trigger the exception if the connection was lost and reconnect. (Issue #282)
+        """
+        config: ConfigType = self.config["mqtt"]
+        topic_prefix: str = config["topic_prefix"]
+        if not self.mqtt_connected.is_set():
+            _LOG.debug("_mqtt_keep_alive_loop awaiting MQTT connection")
+            await self.mqtt_connected.wait()
+            _LOG.debug("_mqtt_keep_alive_loop unblocked after MQTT connection")
+        while True:
+            if self.mqtt is None:
+                _LOG.error("Attempted to ping MQTT server before client initialised")
+                while self.mqtt is None:
+                    await asyncio.sleep(1)
+                continue
+            await self.mqtt.publish(MQTTMessageSend(
+                        "/".join((topic_prefix, config["status_topic"])),
+                        config["status_payload_running"].encode("utf8"),
+                        qos=1,
+                        retain=True,
+                    ))
+            await asyncio.sleep(config["keepalive"])
+
     async def _mqtt_rx_loop(self) -> None:
         if not self.mqtt_connected.is_set():
             _LOG.debug("_mqtt_rx_loop awaiting MQTT connection")
             await self.mqtt_connected.wait()
             _LOG.debug("_mqtt_rx_loop unblocked after MQTT connection")
         while True:
             if self.mqtt is None:
@@ -1171,14 +1200,15 @@
                 # Reset reconnects remaining once successful
                 reconnects_remaining = self.config["mqtt"]["reconnect_count"]
                 self.critical_tasks = [
                     self.loop.create_task(coro)
                     for coro in (
                         self._mqtt_task_loop(),
                         self._mqtt_rx_loop(),
+                        self._mqtt_keep_alive_loop(),
                         self._remove_finished_transient_tasks(),
                     )
                 ]
 
                 self.running.set()
 
                 if self.config["mqtt"].get("ha_discovery", {}).get("enabled"):
```

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/config_main_invalid.feature` & `mqtt_io-2.2.9/mqtt_io/tests/features/config_main_invalid.feature`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/config_main_valid.feature` & `mqtt_io-2.2.9/mqtt_io/tests/features/config_main_valid.feature`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/config_module_gpio_invalid.feature` & `mqtt_io-2.2.9/mqtt_io/tests/features/config_module_gpio_invalid.feature`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/config_module_gpio_valid.feature` & `mqtt_io-2.2.9/mqtt_io/tests/features/config_module_gpio_valid.feature`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/environment.py` & `mqtt_io-2.2.9/mqtt_io/tests/features/environment.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/module_gpio_runtime.feature` & `mqtt_io-2.2.9/mqtt_io/tests/features/module_gpio_runtime.feature`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/server_init_gpio.feature` & `mqtt_io-2.2.9/mqtt_io/tests/features/server_init_gpio.feature`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/server_init_sensor.feature` & `mqtt_io-2.2.9/mqtt_io/tests/features/server_init_sensor.feature`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/steps/config_main.py` & `mqtt_io-2.2.9/mqtt_io/tests/features/steps/config_main.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/steps/events.py` & `mqtt_io-2.2.9/mqtt_io/tests/features/steps/events.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/steps/module_gpio.py` & `mqtt_io-2.2.9/mqtt_io/tests/features/steps/module_gpio.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/tests/features/steps/server.py` & `mqtt_io-2.2.9/mqtt_io/tests/features/steps/server.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/mqtt_io/utils.py` & `mqtt_io-2.2.9/mqtt_io/utils.py`

 * *Files identical despite different names*

### Comparing `mqtt_io-2.2.8/pyproject.toml` & `mqtt_io-2.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mqtt-io"
-version = "2.2.8"
+version = "2.2.9"
 description = "Expose GPIO modules (Raspberry Pi, Beaglebone, PCF8754, PiFace2 etc.), digital sensors (LM75 etc.) and serial streams to an MQTT server for remote control and monitoring."
 readme = "README.md"
 authors = ["Ellis Percival <mqtt-io@failcode.co.uk>"]
 license = "MIT"
 documentation = "https://flyte.github.io/mqtt-io/"
 
 [tool.poetry.dependencies]
```

### Comparing `mqtt_io-2.2.8/PKG-INFO` & `mqtt_io-2.2.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqtt-io
-Version: 2.2.8
+Version: 2.2.9
 Summary: Expose GPIO modules (Raspberry Pi, Beaglebone, PCF8754, PiFace2 etc.), digital sensors (LM75 etc.) and serial streams to an MQTT server for remote control and monitoring.
 License: MIT
 Author: Ellis Percival
 Author-email: mqtt-io@failcode.co.uk
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -123,21 +123,41 @@
 # Sensors
 sensor_modules:
   # An LM75 sensor attached to the I2C bus
   - name: lm75_sensor
     module: lm75
     i2c_bus_num: 1
     chip_addr: 0x48
+  # An INA219 sensor attached to the I2C bus
+  - name: ina219_sensor
+    module: ina219
+    i2c_bus_num: 1
+    chip_addr: 0x43
+
 
 sensor_inputs:
-  # The configuration of the specific sensor value to use (LM75 only has temperature)
+  # lm75 - The configuration of the specific sensor value to use (LM75 only has temperature)
   - name: porch_temperature
     module: lm75_sensor
+  # ina219 - The configuration of the specific sensor value to use (4 options for the ina219 sensor)
+  - name: power
+    type: power
+    module: ina219_sensor
+  - name: bus_voltage
+    type: bus_voltage
+    module: ina219_sensor
+  - name: current
+    type: current
+    module: ina219_sensor
+  - name: shunt_voltage
+    type: shunt_voltage
+    module: ina219_sensor
 
 # Streams
 stream_modules:
   # A serial port to communicate with the house alarm system
   - name: alarm_system
     module: serial
     device: /dev/ttyUSB0
     baud: 9600
 ```
+
```

