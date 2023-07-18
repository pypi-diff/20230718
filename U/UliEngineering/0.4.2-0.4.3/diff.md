# Comparing `tmp/UliEngineering-0.4.2.tar.gz` & `tmp/UliEngineering-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UliEngineering-0.4.2.tar", last modified: Sat May 20 01:59:18 2023, max compression
+gzip compressed data, was "UliEngineering-0.4.3.tar", last modified: Tue Jul 18 16:03:19 2023, max compression
```

## Comparing `UliEngineering-0.4.2.tar` & `UliEngineering-0.4.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.390939 UliEngineering-0.4.2/
--rw-rw-r--   0 uli       (1000) uli       (1000)    11342 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/LICENSE
--rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2023-05-20 01:59:18.390939 UliEngineering-0.4.2/PKG-INFO
--rw-rw-r--   0 uli       (1000) uli       (1000)     6576 2023-05-20 01:18:20.000000 UliEngineering-0.4.2/README.md
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.370938 UliEngineering-0.4.2/UliEngineering/
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.374938 UliEngineering-0.4.2/UliEngineering/Economics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     3661 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Economics/Interest.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Economics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.378938 UliEngineering-0.4.2/UliEngineering/Electronics/
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1798 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Capacitors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     5427 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Crystal.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     7882 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Hysteresis.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)      753 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Inductors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2557 2023-05-20 01:18:20.000000 UliEngineering-0.4.2/UliEngineering/Electronics/LED.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1960 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/MOSFET.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     7077 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Microstrip.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1035 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/OpAmp.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      873 2022-09-01 22:45:17.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Power.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/PowerFactor.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)      786 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Reactance.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     6324 2023-03-06 14:19:49.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Resistors.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6543 2022-09-01 22:45:17.000000 UliEngineering-0.4.2/UliEngineering/Electronics/TemperatureCoefficient.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      884 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/Tolerance.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     5948 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/VoltageDivider.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Electronics/__init__.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)    21499 2022-09-01 22:45:17.000000 UliEngineering-0.4.2/UliEngineering/EngineerIO.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      534 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Exceptions.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2622 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Length.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.378938 UliEngineering-0.4.2/UliEngineering/Math/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1890 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Math/Coordinates.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2885 2023-05-20 01:18:20.000000 UliEngineering-0.4.2/UliEngineering/Math/Decibel.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.378938 UliEngineering-0.4.2/UliEngineering/Math/Geometry/
--rw-rw-r--   0 uli       (1000) uli       (1000)      591 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Math/Geometry/Circle.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3668 2023-05-20 01:56:07.000000 UliEngineering-0.4.2/UliEngineering/Math/Geometry/Cylinder.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1588 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Math/Geometry/Polygon.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1113 2022-09-13 18:18:08.000000 UliEngineering-0.4.2/UliEngineering/Math/Geometry/Sphere.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Math/Geometry/__init__.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Math/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.378938 UliEngineering-0.4.2/UliEngineering/Mechanics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1493 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Mechanics/Threads.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Mechanics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.382938 UliEngineering-0.4.2/UliEngineering/Physics/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1968 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/Acceleration.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3378 2023-05-20 01:51:18.000000 UliEngineering-0.4.2/UliEngineering/Physics/Density.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      953 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/Frequency.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1835 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/JohnsonNyquistNoise.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1023 2022-09-01 22:45:17.000000 UliEngineering-0.4.2/UliEngineering/Physics/Light.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      991 2023-03-06 14:19:49.000000 UliEngineering-0.4.2/UliEngineering/Physics/MagneticResonance.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1451 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/NTC.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1012 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/NoiseDensity.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1355 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/Pressure.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     2234 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/RF.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     4945 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/RTD.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2175 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/Rotation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2489 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/Temperature.py
--rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Physics/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.386938 UliEngineering-0.4.2/UliEngineering/SignalProcessing/
--rw-rw-r--   0 uli       (1000) uli       (1000)     8963 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Chunks.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      492 2022-09-01 22:45:17.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Correlation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1747 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/DateTime.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)    12299 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/FFT.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    11914 2022-09-01 22:45:17.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Filter.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3030 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Normalize.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     9022 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Resampling.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    19078 2022-09-01 22:45:17.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Selection.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)     2446 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Simulation.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     9831 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Utils.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1710 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Weight.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3332 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/Window.py
--rw-rw-r--   0 uli       (1000) uli       (1000)       22 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/SignalProcessing/__init__.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2081 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Units.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.390939 UliEngineering-0.4.2/UliEngineering/Utils/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1173 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Compression.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      662 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Concurrency.py
--rw-rw-r--   0 uli       (1000) uli       (1000)    11868 2023-03-06 14:19:49.000000 UliEngineering-0.4.2/UliEngineering/Utils/Date.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6193 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Files.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     3687 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Iterable.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      606 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/JSON.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     6972 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/NumPy.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      664 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Parser.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1806 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Range.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      286 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Slice.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     1348 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/String.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2372 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/Temporary.py
--rw-rw-r--   0 uli       (1000) uli       (1000)     2621 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/ZIP.py
--rw-rw-r--   0 uli       (1000) uli       (1000)      104 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/Utils/__init__.py
--rwxrwxr-x   0 uli       (1000) uli       (1000)       23 2022-05-19 23:48:15.000000 UliEngineering-0.4.2/UliEngineering/__init__.py
-drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-05-20 01:59:18.370938 UliEngineering-0.4.2/UliEngineering.egg-info/
--rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2023-05-20 01:59:18.000000 UliEngineering-0.4.2/UliEngineering.egg-info/PKG-INFO
--rw-rw-r--   0 uli       (1000) uli       (1000)     2954 2023-05-20 01:59:18.000000 UliEngineering-0.4.2/UliEngineering.egg-info/SOURCES.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)        1 2023-05-20 01:59:18.000000 UliEngineering-0.4.2/UliEngineering.egg-info/dependency_links.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)       56 2023-05-20 01:59:18.000000 UliEngineering-0.4.2/UliEngineering.egg-info/requires.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)       15 2023-05-20 01:59:18.000000 UliEngineering-0.4.2/UliEngineering.egg-info/top_level.txt
--rw-rw-r--   0 uli       (1000) uli       (1000)      100 2023-05-20 01:59:18.390939 UliEngineering-0.4.2/setup.cfg
--rwxrwxr-x   0 uli       (1000) uli       (1000)     1578 2023-05-20 01:58:59.000000 UliEngineering-0.4.2/setup.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11342 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/LICENSE
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/PKG-INFO
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6808 2023-07-18 15:59:30.000000 UliEngineering-0.4.3/README.md
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.888412 UliEngineering-0.4.3/UliEngineering/
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.888412 UliEngineering-0.4.3/UliEngineering/Economics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3661 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Economics/Interest.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Economics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.892412 UliEngineering-0.4.3/UliEngineering/Electronics/
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1798 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Capacitors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     5427 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Crystal.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     7882 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Hysteresis.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)      753 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Inductors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2557 2023-05-20 01:18:20.000000 UliEngineering-0.4.3/UliEngineering/Electronics/LED.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1960 2023-07-18 16:02:10.000000 UliEngineering-0.4.3/UliEngineering/Electronics/MOSFET.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     7077 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Microstrip.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1035 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/OpAmp.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      873 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Power.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/PowerFactor.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)      786 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Reactance.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     6324 2023-03-06 14:19:49.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Resistors.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6543 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/Electronics/TemperatureCoefficient.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      884 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/Tolerance.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     5948 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/VoltageDivider.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Electronics/__init__.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)    21499 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/EngineerIO.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      534 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Exceptions.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2622 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Length.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.896412 UliEngineering-0.4.3/UliEngineering/Math/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1890 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Coordinates.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2885 2023-05-20 01:18:20.000000 UliEngineering-0.4.3/UliEngineering/Math/Decibel.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.896412 UliEngineering-0.4.3/UliEngineering/Math/Geometry/
+-rw-rw-r--   0 uli       (1000) uli       (1000)      591 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Circle.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3668 2023-05-20 01:56:07.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Cylinder.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1588 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Polygon.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1113 2022-09-13 18:18:08.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/Sphere.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/Geometry/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Math/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.896412 UliEngineering-0.4.3/UliEngineering/Mechanics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1493 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Mechanics/Threads.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Mechanics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.900412 UliEngineering-0.4.3/UliEngineering/Physics/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1968 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Acceleration.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3378 2023-05-20 01:51:18.000000 UliEngineering-0.4.3/UliEngineering/Physics/Density.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      953 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Frequency.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1835 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/JohnsonNyquistNoise.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1023 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/Physics/Light.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      991 2023-03-06 14:19:49.000000 UliEngineering-0.4.3/UliEngineering/Physics/MagneticResonance.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1451 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/NTC.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1012 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/NoiseDensity.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1355 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Pressure.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     2234 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/RF.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     4945 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/RTD.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2175 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Rotation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2489 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/Temperature.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)        0 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Physics/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.904412 UliEngineering-0.4.3/UliEngineering/SignalProcessing/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     8963 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Chunks.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      492 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Correlation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1747 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/DateTime.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)    12299 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/FFT.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11914 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Filter.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3030 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Normalize.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     9022 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Resampling.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    19078 2022-09-01 22:45:17.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Selection.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     2446 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Simulation.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     9831 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Utils.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1710 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Weight.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3332 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/Window.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)       22 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/SignalProcessing/__init__.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2081 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Units.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/UliEngineering/Utils/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1173 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Compression.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      662 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Concurrency.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)    11944 2023-07-18 15:59:54.000000 UliEngineering-0.4.3/UliEngineering/Utils/Date.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6193 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Files.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     3687 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Iterable.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      606 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/JSON.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     6972 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/NumPy.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      664 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Parser.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1806 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Range.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      286 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Slice.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1348 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/String.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2372 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/Temporary.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2621 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/ZIP.py
+-rw-rw-r--   0 uli       (1000) uli       (1000)      104 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/Utils/__init__.py
+-rwxrwxr-x   0 uli       (1000) uli       (1000)       23 2022-05-19 23:48:15.000000 UliEngineering-0.4.3/UliEngineering/__init__.py
+drwxrwxr-x   0 uli       (1000) uli       (1000)        0 2023-07-18 16:03:19.888412 UliEngineering-0.4.3/UliEngineering.egg-info/
+-rw-rw-r--   0 uli       (1000) uli       (1000)     1048 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/PKG-INFO
+-rw-rw-r--   0 uli       (1000) uli       (1000)     2954 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/SOURCES.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)        1 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/dependency_links.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)       56 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/requires.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)       15 2023-07-18 16:03:19.000000 UliEngineering-0.4.3/UliEngineering.egg-info/top_level.txt
+-rw-rw-r--   0 uli       (1000) uli       (1000)      100 2023-07-18 16:03:19.908412 UliEngineering-0.4.3/setup.cfg
+-rwxrwxr-x   0 uli       (1000) uli       (1000)     1578 2023-07-18 16:00:52.000000 UliEngineering-0.4.3/setup.py
```

### Comparing `UliEngineering-0.4.2/LICENSE` & `UliEngineering-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/PKG-INFO` & `UliEngineering-0.4.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UliEngineering
-Version: 0.4.2
+Version: 0.4.3
 Summary: Computational tools for electronics engineering
 Home-page: https://techoverflow.net/
 Author: Uli Köhler
 Author-email: ukoehler@techoverflow.net
 License: Apache License v2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `UliEngineering-0.4.2/README.md` & `UliEngineering-0.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,15 @@
   - [How to generate datetime for every hour on a given day in Python](https://techoverflow.net/2022/06/19/how-to-generate-datetime-for-every-hour-on-a-given-day-in-python/)
   - [How to generate datetime for every minute on a given day in Python](https://techoverflow.net/2022/06/19/how-to-generate-datetime-for-every-minute-on-a-given-day-in-python/)
   - [How to generate datetime for every second on a given day in Python](https://techoverflow.net/2022/06/19/how-to-generate-datetime-for-every-second-on-a-given-day-in-python/)
   - [How to compute MRI Larmor frequency for a given magnetic field using Pythonf](https://techoverflow.net/2023/02/04/how-to-compute-mri-larmor-frequency-for-a-given-magnetic-field-using-python/)
   - [How to compute voltage divider output voltage using Python](https://techoverflow.net/2023/02/05/how-to-compute-voltage-divider-output-voltage-using-python/)
   - [How to format axis as dB (decibel) using matplotlib](https://techoverflow.net/2023/03/13/how-to-format-axis-as-db-decibel-using-matplotlib/)
   - [How to compute Buck/Boost/LDO output voltage by feedback resistors using Python](https://techoverflow.net/2023/04/09/how-to-compute-buck-boost-ldo-output-voltage-by-feedback-resistors-using-python/)
+  - [How to compute the weight of a titanium or stainless steel rod using UliEngineering in Python](https://techoverflow.net/2023/05/21/how-to-compute-the-weight-of-a-titanium-or-stainless-steel-rod-using-uliengineering-in-python/)
 
 ## Testing
 
 In order to run the unit tests, first install tox:
 
 ```sh
 pip install --user tox
```

### Comparing `UliEngineering-0.4.2/UliEngineering/Economics/Interest.py` & `UliEngineering-0.4.3/UliEngineering/Economics/Interest.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Capacitors.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Capacitors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Crystal.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Crystal.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Hysteresis.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Hysteresis.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Inductors.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Inductors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/LED.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/LED.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/MOSFET.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/MOSFET.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Microstrip.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Microstrip.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/OpAmp.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/OpAmp.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Power.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Power.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/PowerFactor.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/PowerFactor.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Reactance.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Reactance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Resistors.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Resistors.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/TemperatureCoefficient.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/TemperatureCoefficient.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/Tolerance.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/Tolerance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Electronics/VoltageDivider.py` & `UliEngineering-0.4.3/UliEngineering/Electronics/VoltageDivider.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/EngineerIO.py` & `UliEngineering-0.4.3/UliEngineering/EngineerIO.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Exceptions.py` & `UliEngineering-0.4.3/UliEngineering/Exceptions.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Length.py` & `UliEngineering-0.4.3/UliEngineering/Length.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Math/Coordinates.py` & `UliEngineering-0.4.3/UliEngineering/Math/Coordinates.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Math/Decibel.py` & `UliEngineering-0.4.3/UliEngineering/Math/Decibel.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Math/Geometry/Circle.py` & `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Circle.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Math/Geometry/Cylinder.py` & `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Cylinder.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Math/Geometry/Polygon.py` & `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Polygon.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Math/Geometry/Sphere.py` & `UliEngineering-0.4.3/UliEngineering/Math/Geometry/Sphere.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Mechanics/Threads.py` & `UliEngineering-0.4.3/UliEngineering/Mechanics/Threads.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/Acceleration.py` & `UliEngineering-0.4.3/UliEngineering/Physics/Acceleration.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/Density.py` & `UliEngineering-0.4.3/UliEngineering/Physics/Density.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/Frequency.py` & `UliEngineering-0.4.3/UliEngineering/Physics/Frequency.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/JohnsonNyquistNoise.py` & `UliEngineering-0.4.3/UliEngineering/Physics/JohnsonNyquistNoise.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/Light.py` & `UliEngineering-0.4.3/UliEngineering/Physics/Light.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/MagneticResonance.py` & `UliEngineering-0.4.3/UliEngineering/Physics/MagneticResonance.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/NTC.py` & `UliEngineering-0.4.3/UliEngineering/Physics/NTC.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/NoiseDensity.py` & `UliEngineering-0.4.3/UliEngineering/Physics/NoiseDensity.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/Pressure.py` & `UliEngineering-0.4.3/UliEngineering/Physics/Pressure.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/RF.py` & `UliEngineering-0.4.3/UliEngineering/Physics/RF.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/RTD.py` & `UliEngineering-0.4.3/UliEngineering/Physics/RTD.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/Rotation.py` & `UliEngineering-0.4.3/UliEngineering/Physics/Rotation.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Physics/Temperature.py` & `UliEngineering-0.4.3/UliEngineering/Physics/Temperature.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Chunks.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Chunks.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/DateTime.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/DateTime.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/FFT.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/FFT.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Filter.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Filter.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Normalize.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Normalize.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Resampling.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Resampling.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Selection.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Selection.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Simulation.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Simulation.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Utils.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Utils.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Weight.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Weight.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/SignalProcessing/Window.py` & `UliEngineering-0.4.3/UliEngineering/SignalProcessing/Window.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Units.py` & `UliEngineering-0.4.3/UliEngineering/Units.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Compression.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Compression.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Concurrency.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Concurrency.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Date.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Date.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "extract_day_of_week", "is_first_day_of_month", "is_first_day_of_week",
     "is_month_change", "is_year_change", "yield_hours_on_day",
     "yield_minutes_on_day", "yield_seconds_on_day",
     "generate_datetime_filename"]
 
 Date = namedtuple("Date", ["year", "month", "day"])
 
-def generate_datetime_filename(label="data", extension="csv", fractional=True, dt=None):
+def generate_datetime_filename(label="data", extension="csv", postfix=None, fractional=True, dt=None):
     """
     Generate a filename such as
 
     mydata-2022-09-02_00-31-50-613015.csv
     where "mydata" is the label and "csv" is the extensions.
 
     You can also generate the filename without fractional seconds
@@ -35,14 +35,16 @@
     :param datetime.datetime dt Set this to a datetime.datetime to use a custom timestamp. If None, uses datetime.now()
     """
     if dt is None:
         dt = datetime.now()
     filename = "" if label is None else f"{label}-"
     fractional_str = f"-{dt.microsecond:06d}" if fractional is True else ""
     filename += f"{dt.year}-{dt.month:02d}-{dt.day:02d}_{dt.hour:02d}-{dt.minute:02d}-{dt.second:02d}{fractional_str}"
+    if postfix is not None:
+        filename += f"-{postfix}"
     if extension is not None:
         filename += f".{extension}"
     return filename
 
 def number_of_days_in_month(year=2019, month=1):
     """
     Returns the number of days in a month, e.g. 31 in January (month=1).
```

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Files.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Files.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Iterable.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Iterable.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/JSON.py` & `UliEngineering-0.4.3/UliEngineering/Utils/JSON.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/NumPy.py` & `UliEngineering-0.4.3/UliEngineering/Utils/NumPy.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Parser.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Parser.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Range.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Range.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/String.py` & `UliEngineering-0.4.3/UliEngineering/Utils/String.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/Temporary.py` & `UliEngineering-0.4.3/UliEngineering/Utils/Temporary.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering/Utils/ZIP.py` & `UliEngineering-0.4.3/UliEngineering/Utils/ZIP.py`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/UliEngineering.egg-info/PKG-INFO` & `UliEngineering-0.4.3/UliEngineering.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UliEngineering
-Version: 0.4.2
+Version: 0.4.3
 Summary: Computational tools for electronics engineering
 Home-page: https://techoverflow.net/
 Author: Uli Köhler
 Author-email: ukoehler@techoverflow.net
 License: Apache License v2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `UliEngineering-0.4.2/UliEngineering.egg-info/SOURCES.txt` & `UliEngineering-0.4.3/UliEngineering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UliEngineering-0.4.2/setup.py` & `UliEngineering-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 if sys.version_info < (3, 0):
     print('ERROR: UliEngineering currently requires at least Python 3.0 to run.')
     sys.exit(1)
 
 setup(name='UliEngineering',
-      version='0.4.2',
+      version='0.4.3',
       description='Computational tools for electronics engineering',
       author='Uli Köhler',
       author_email='ukoehler@techoverflow.net',
       url='https://techoverflow.net/',
       license='Apache License v2.0',
       packages=find_packages(exclude=['tests*']),
       include_package_data=True,
```

