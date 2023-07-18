# Comparing `tmp/butler-connect-0.7.2.tar.gz` & `tmp/butler-connect-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.7.2.tar", last modified: Fri Jul 14 19:27:03 2023, max compression
+gzip compressed data, was "butler-connect-0.7.3.tar", last modified: Tue Jul 18 21:28:19 2023, max compression
```

## Comparing `butler-connect-0.7.2.tar` & `butler-connect-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.339659 butler-connect-0.7.2/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     2712 2023-07-14 19:27:03.338657 butler-connect-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0      933 2023-07-14 19:26:32.000000 butler-connect-0.7.2/README.md
--rw-rw-rw-   0        0        0      738 2023-07-14 19:25:40.000000 butler-connect-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 19:27:03.339659 butler-connect-0.7.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.304568 butler-connect-0.7.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.307568 butler-connect-0.7.2/src/butlerConnect/
--rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.2/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.2/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.320599 butler-connect-0.7.2/src/butlerDescription/
--rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.2/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.2/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.2/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0      209 2023-05-12 19:37:37.000000 butler-connect-0.7.2/src/butlerDescription/group.py
--rw-rw-rw-   0        0        0     2596 2023-07-14 19:26:51.000000 butler-connect-0.7.2/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-07-14 19:27:03.337637 butler-connect-0.7.2/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     2712 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-14 19:27:03.000000 butler-connect-0.7.2/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.580041 butler-connect-0.7.3/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0     2828 2023-07-18 21:28:19.579101 butler-connect-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2023-07-18 21:27:25.000000 butler-connect-0.7.3/README.md
+-rw-rw-rw-   0        0        0      738 2023-07-18 21:27:42.000000 butler-connect-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 21:28:19.581065 butler-connect-0.7.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.492148 butler-connect-0.7.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.501840 butler-connect-0.7.3/src/butlerConnect/
+-rw-rw-rw-   0        0        0      123 2023-05-18 09:03:28.000000 butler-connect-0.7.3/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    18719 2023-05-20 09:13:29.000000 butler-connect-0.7.3/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.534489 butler-connect-0.7.3/src/butlerDescription/
+-rw-rw-rw-   0        0        0      208 2023-05-18 09:13:48.000000 butler-connect-0.7.3/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.7.3/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.7.3/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0      512 2023-07-18 21:25:05.000000 butler-connect-0.7.3/src/butlerDescription/group.py
+-rw-rw-rw-   0        0        0     2844 2023-07-18 21:21:52.000000 butler-connect-0.7.3/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:28:19.573027 butler-connect-0.7.3/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2828 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-07-18 21:28:19.000000 butler-connect-0.7.3/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.7.2/LICENSE` & `butler-connect-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.2/PKG-INFO` & `butler-connect-0.7.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.2
+Version: 0.7.3
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,7 +61,10 @@
 
 ### 0.7.1
 - Bugifx in Signal().__init__(.. ext was missing)
 ### 0.7.2
 - create SignalDirection()
 - add convertFrom to SignalOptionType
 - add different consumptionSignals to SignalType
+### 0.7.3
+- add buildingHardware to signalOptionType and groupOptionType
+- add agent_building to groupOptionType
```

### Comparing `butler-connect-0.7.2/README.md` & `butler-connect-0.7.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,8 +25,11 @@
 - change signal Description and add ext. !!! No backwards compatibility! if Using Schmema for parsing
 
 ### 0.7.1
 - Bugifx in Signal().__init__(.. ext was missing)
 ### 0.7.2
 - create SignalDirection()
 - add convertFrom to SignalOptionType
-- add different consumptionSignals to SignalType
+- add different consumptionSignals to SignalType
+### 0.7.3
+- add buildingHardware to signalOptionType and groupOptionType
+- add agent_building to groupOptionType
```

### Comparing `butler-connect-0.7.2/pyproject.toml` & `butler-connect-0.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.7.2"
+version = "0.7.3"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.7.2/src/butlerConnect/pikaButler.py` & `butler-connect-0.7.3/src/butlerConnect/pikaButler.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.2/src/butlerDescription/control.py` & `butler-connect-0.7.3/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.7.2/src/butlerDescription/signal.py` & `butler-connect-0.7.3/src/butlerDescription/signal.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,20 @@
     
     
 
 class SignalOptionType():
     unDef = 'undef'
     forwardingMQTT = 'forwarding_mqtt'
     convertFrom    = 'convert_from'
+    class buildingHardware():
+        unDef = 'undef'
+        heating = 'building_hardware_heating'
+        cooling = 'building_hardware_cooling'
+        ventilation = 'building_hardware_ventilation'
+        lighting = 'building_hardware_lighting'
     
 class SignalDirection():
     input = 'input'
     output = 'output'
```

### Comparing `butler-connect-0.7.2/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.7.3/src/butler_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.7.2
+Version: 0.7.3
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -61,7 +61,10 @@
 
 ### 0.7.1
 - Bugifx in Signal().__init__(.. ext was missing)
 ### 0.7.2
 - create SignalDirection()
 - add convertFrom to SignalOptionType
 - add different consumptionSignals to SignalType
+### 0.7.3
+- add buildingHardware to signalOptionType and groupOptionType
+- add agent_building to groupOptionType
```

