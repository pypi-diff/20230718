# Comparing `tmp/splendaq-0.4.3.tar.gz` & `tmp/splendaq-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splendaq-0.4.3.tar", last modified: Mon Jun 12 21:19:55 2023, max compression
+gzip compressed data, was "splendaq-0.4.4.tar", last modified: Tue Jul 18 19:42:11 2023, max compression
```

## Comparing `splendaq-0.4.3.tar` & `splendaq-0.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.116008 splendaq-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.092008 splendaq-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.096008 splendaq-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-12 21:19:39.000000 splendaq-0.4.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-12 21:19:39.000000 splendaq-0.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-12 21:19:39.000000 splendaq-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-12 21:19:39.000000 splendaq-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 21:19:39.000000 splendaq-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 21:19:55.116008 splendaq-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-12 21:19:39.000000 splendaq-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 21:19:39.000000 splendaq-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-12 21:19:55.116008 splendaq-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-12 21:19:39.000000 splendaq-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.092008 splendaq-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.096008 splendaq-0.4.3/src/splendaq/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.104008 splendaq-0.4.3/src/splendaq/daq/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18531 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_log_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24319 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_offline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/daq/_sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.104008 splendaq-0.4.3/src/splendaq/io/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.112008 splendaq-0.4.3/src/splendaq/io/_liconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/COPYING.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)   716536 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_linux
--rwxr-xr-x   0 runner    (1001) docker     (123)   629104 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_macos
--rw-r--r--   0 runner    (1001) docker     (123)   689928 2023-06-12 21:19:39.000000 splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_windows.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.100008 splendaq-0.4.3/src/splendaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:19:54.000000 splendaq-0.4.3/src/splendaq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-12 21:19:55.000000 splendaq-0.4.3/src/splendaq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.092008 splendaq-0.4.3/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.112008 splendaq-0.4.3/tutorials/daq/
--rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/dc_oscilloscope.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/event_building.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/logging_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/running_the_sequencer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/daq/sequencer_settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:19:55.116008 splendaq-0.4.3/tutorials/io/
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/io/read_files.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-06-12 21:19:39.000000 splendaq-0.4.3/tutorials/io/write_files.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.731939 splendaq-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.723939 splendaq-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.723939 splendaq-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-18 19:41:58.000000 splendaq-0.4.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 19:41:58.000000 splendaq-0.4.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-18 19:41:58.000000 splendaq-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 19:41:58.000000 splendaq-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 19:41:58.000000 splendaq-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-18 19:42:11.731939 splendaq-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 19:41:58.000000 splendaq-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-18 19:41:58.000000 splendaq-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-18 19:42:11.731939 splendaq-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 19:41:58.000000 splendaq-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.723939 splendaq-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.723939 splendaq-0.4.4/src/splendaq/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.727939 splendaq-0.4.4/src/splendaq/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/daq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19827 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/daq/_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24319 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/daq/_offline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/daq/_oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/daq/_sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.727939 splendaq-0.4.4/src/splendaq/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/io/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.727939 splendaq-0.4.4/src/splendaq/io/_liconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/io/_liconvert/COPYING.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)   716536 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/io/_liconvert/liconvert_linux
+-rwxr-xr-x   0 runner    (1001) docker     (123)   629104 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/io/_liconvert/liconvert_macos
+-rw-r--r--   0 runner    (1001) docker     (123)   689928 2023-07-18 19:41:58.000000 splendaq-0.4.4/src/splendaq/io/_liconvert/liconvert_windows.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.723939 splendaq-0.4.4/src/splendaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 19:42:11.000000 splendaq-0.4.4/src/splendaq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.723939 splendaq-0.4.4/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.731939 splendaq-0.4.4/tutorials/daq/
+-rw-r--r--   0 runner    (1001) docker     (123)     6868 2023-07-18 19:41:58.000000 splendaq-0.4.4/tutorials/daq/dc_oscilloscope.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-07-18 19:41:58.000000 splendaq-0.4.4/tutorials/daq/event_building.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-18 19:41:58.000000 splendaq-0.4.4/tutorials/daq/logging_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-18 19:41:58.000000 splendaq-0.4.4/tutorials/daq/running_the_sequencer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-18 19:41:58.000000 splendaq-0.4.4/tutorials/daq/sequencer_settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:42:11.731939 splendaq-0.4.4/tutorials/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-18 19:41:58.000000 splendaq-0.4.4/tutorials/io/read_files.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8853 2023-07-18 19:41:58.000000 splendaq-0.4.4/tutorials/io/write_files.ipynb
```

### Comparing `splendaq-0.4.3/.github/workflows/python-package.yml` & `splendaq-0.4.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/.github/workflows/python-publish.yml` & `splendaq-0.4.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/.gitignore` & `splendaq-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/LICENSE` & `splendaq-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/PKG-INFO` & `splendaq-0.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.4.3
+Version: 0.4.4
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendaq-0.4.3/README.md` & `splendaq-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/setup.cfg` & `splendaq-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/_cli.py` & `splendaq-0.4.4/src/splendaq/_cli.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/daq/_log_data.py` & `splendaq-0.4.4/src/splendaq/daq/_log_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,19 +38,21 @@
             Take ownership of the Moku even if it is being used by
             someone else. Default is False.
         fs : float, optional
             The digitization rate of the data to be taken in Hz. The
             allowed values are 10 to 10e6 Hz for the Moku:Pro for 1
             channel logging, where the max decreases to 5e6 Hz for 2
             channel logging and to 1.25e6 for 3 or 4 channel logging.
-            The allowed values are 10 to 1e6 Hz for 1 channel logging,
-            wheere the maximum allowed value decreases to 500e3 Hz for
-            2 channel logging. Default is the lowest allowed maximum
-            value for the given device (i.e. 1.25e6 for Moku:Pro and
-            500e3 for Moku:Go).
+            For the Moku:Lab, the allowed values are 10 to 2.5e5 Hz.
+            For the Moku:Go, the allowed values are 10 to 1e6 Hz for
+            1 channel logging, where the maximum allowed value
+            decreases to 500e3 Hz for 2 channel logging. Default is the
+            lowest allowed maximum value for the given device (i.e.
+            1.25e6 for Moku:Pro, 2.5e5 for Moku:Lab, and 500e3 for
+            Moku:Go).
         max_duration_per_file : float, optional
             The maximum amount of seconds to save to a single file.
             Avoids creating very large single files. Default is 60
             seconds.
         acquisition_mode : str, optional
             Changes acquisition mode between 'Normal' and 'Precision'.
             Precision mode is also known as decimation, it samples at
@@ -63,22 +65,24 @@
         self.DL = Datalogger(
             ip_address, force_connect=force_connect, session_trust_env=False,
         )
         self.DL.set_acquisition_mode(acquisition_mode)
         self._max_dur_per_file = max_duration_per_file
 
         self._device = self.DL.describe()['hardware']
-        if self._device not in ['Moku:Pro', 'Moku:Go']:
+        if self._device not in ['Moku:Pro', 'Moku:Lab', 'Moku:Go']:
             raise ValueError(
-                "Unrecognized device, is not a Moku:Go or Moku:Pro."
+                "Unrecognized device, is not a Moku:Go, Moku:Lab, or Moku:Pro."
             )
 
         if fs is None:
             if self._device == "Moku:Pro":
                 self._fs = 1.25e6
+            elif self._device == "Moku:Lab":
+                self._fs = 2.5e5
             elif self._device == "Moku:Go":
                 self._fs = 500e3
         else:
             self._fs = fs
 
     def __enter__(self):
         """Returns self when entered via with."""
@@ -89,15 +93,15 @@
         Always run relinquish ownership and turn off inputs and outputs
         when exiting.
 
         """
 
         if self._device == "Moku:Pro":
             chan_list = [1, 2, 3, 4]
-        elif self._device == "Moku:Go":
+        elif self._device in ["Moku:Lab", "Moku:Go"]:
             chan_list = [1, 2]
 
         for chan in chan_list:
             self.DL.generate_waveform(chan, 'Off') # disable outputs
             self.DL.disable_channel(chan) # disable inputs
 
         self.DL.relinquish_ownership()
@@ -109,41 +113,45 @@
 
         Parameters
         ----------
         channels : int, list of int
             Which input channels to log data from. Can be a single
             value for one channel, or a list of the channels. For the
             Moku:Pro, valid channel numbers are 1, 2, 3, and 4. For the
-            Moku:Go, valid channel numbers are 1 and 2.
+            Moku:Lab and Moku:Go, valid channel numbers are 1 and 2.
         impedance : str, list of str, optional
             The output impedance to use for each channel. For the
-            Moku:Pro, options are '1MOhm' and '50Ohm'. For the Moku:Go,
-            the only option is '1MOhm'. Can pass a list of the same
-            length as channels if different impedances are desired for
-            a Moku:Pro. Default is '1MOhm' for all channels.
+            Moku:Pro and Moku:Lab, options are '1MOhm' and '50Ohm'. For
+            the Moku:Go, the only option is '1MOhm'. Can pass a list of
+            the same length as channels if different impedances are
+            desired for a Moku:Pro. Default is '1MOhm' for all channels.
         coupling : str, list of str, optional
             The coupling to use for each channel. Options are 'DC' and
             'AC'. Can pass a list of the same length as channels if
             different couplings are desired. Default is 'DC' for all
             channels.
         vrange : str, list of str, optional
             The voltage range to use for each channel. For the
             Moku:Pro, options are '400mVpp', '4Vpp' and '40Vpp'. For
-            the Moku:Go, options are '10Vpp' and '50Vpp'. Can pass a
-            list of the same length as channels if different voltage
-            ranges are desired for specific channels. Default is the
-            smallest allowed value for the device for all channels
-            (i.e. '400mVpp' for the Moku:Pro and '10Vpp' for the
-            Moku:Go).
+            the Moku:Lab, the options are '1Vpp' and '10Vpp'. For the
+            Moku:Go, options are '10Vpp' and '50Vpp'. Can pass a list
+            of the same length as channels if different voltage ranges
+            are desired for specific channels. Default is the smallest
+            allowed value for the device for all channels (i.e.
+            '400mVpp' for the Moku:Pro, '1Vpp' for the Moku:Lab, and
+            '10Vpp' for the Moku:Go).
 
         """
 
         if self._device == "Moku:Pro":
             chan_list = [1, 2, 3, 4]
             vrange = '400mVpp' if vrange is None else vrange
+        elif self._device == "Moku:Lab":
+            chan_list = [1, 2]
+            vrange = '1Vpp' if vrange is None else vrange
         elif self._device == "Moku:Go":
             chan_list = [1, 2]
             vrange = '10Vpp' if vrange is None else vrange
 
         if np.isscalar(channels):
             channels = [channels]
         if np.isscalar(impedance):
@@ -172,33 +180,35 @@
         """
         Method to return a dictionary with the valid sine wave
         settings to be passed to `self.set_output_channel`.
 
         Parameters
         ----------
         amplitude : float, optional
-             Waveform peak-to-peak amplitude in Volts. Allowed values
-             are 2e-3 to 10 for the Moku:Go and 1e-3 to 10 for the
-             Moku:Pro (For Moku:Pro, the output voltage is limited to
-             between -1V and 1V above 1MHz). Default is 1 V.
+            Waveform peak-to-peak amplitude in Volts. Allowed values
+            are 2e-3 to 10 for the Moku:Go, 2e-3 to 4 for the
+            Moku:Lab, and 1e-3 to 10 for the Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 1 V.
         frequency : float, optional
-             Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
-             for the Moku:Go and 1e-3 to 500e6 for the Moku:Pro.
-             Default is 10000 Hz.
+            Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
+            for the Moku:Go, 1e-3 to 100e6 for the Moku:Lab, and 1e-3
+            to 500e6 for the Moku:Pro. Default is 10000 (1e4) Hz.
         offset : float, optional
-             DC offset applied to the waveform in V. Allowed values are
-             -5 to 5 for Moku:Go and Moku:Pro (For Moku:Pro, the output
-             voltage is limited to between -1V and 1V above 1MHz).
-             Default is 0.
+            DC offset applied to the waveform in V. Allowed values are
+            -5 to 5 for Moku:Go, Moku:Lab, and Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 0.
         phase : float, optional
             Waveform phase offset in degrees. Allowed values are 0 to
-            360 for Moku:Go and Moku:Pro. Default is 0.
+            360 for Moku:Go, Moku:Lab, and Moku:Pro. Default is 0.
         symmetry : float, optional
             Fraction of the cycle rising in %. Allowed values are 0.0
-            to 100.0 for Moku:Go and Moku:Pro. Default is 50.
+            to 100.0 for Moku:Go, Moku:Lab, and Moku:Pro. Default is
+            50.
 
         Returns
         -------
         settings_dict : dict
 
         """
 
@@ -216,36 +226,38 @@
         """
         Method to return a dictionary with the valid square wave
         settings to be passed to `self.set_output_channel`.
 
         Parameters
         ----------
         amplitude : float, optional
-             Waveform peak-to-peak amplitude in Volts. Allowed values
-             are 2e-3 to 10 for the Moku:Go and 1e-3 to 10 for the
-             Moku:Pro (For Moku:Pro, the output voltage is limited to
-             between -1V and 1V above 1MHz). Default is 1 V.
+            Waveform peak-to-peak amplitude in Volts. Allowed values
+            are 2e-3 to 10 for the Moku:Go, 2e-3 to 4 for the
+            Moku:Lab, and 1e-3 to 10 for the Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 1 V.
         frequency : float, optional
-             Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
-             for the Moku:Go and 1e-3 to 500e6 for the Moku:Pro.
-             Default is 10000 Hz.
+            Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
+            for the Moku:Go, 1e-3 to 100e6 for the Moku:Lab, and 1e-3
+            to 500e6 for the Moku:Pro. Default is 10000 (1e4) Hz.
         offset : float, optional
-             DC offset applied to the waveform in V. Allowed values are
-             -5 to 5 for Moku:Go and Moku:Pro (For Moku:Pro, the output
-             voltage is limited to between -1V and 1V above 1MHz).
-             Default is 0.
+            DC offset applied to the waveform in V. Allowed values are
+            -5 to 5 for Moku:Go, Moku:Lab, and Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 0.
         phase : float, optional
             Waveform phase offset in degrees. Allowed values are 0 to
-            360 for Moku:Go and Moku:Pro. Default is 0.
+            360 for Moku:Go, Moku:Lab, and Moku:Pro. Default is 0.
         duty : float, optional
             Duty cycle as percentage in %. Allowed values are 0 to 100
             for Moku:Go and Moku:Pro. Default is 0.
         symmetry : float, optional
             Fraction of the cycle rising in %. Allowed values are 0.0
-            to 100.0 for Moku:Go and Moku:Pro. Default is 50.
+            to 100.0 for Moku:Go, Moku:Lab, and Moku:Pro. Default is
+            50.
 
         Returns
         -------
         settings_dict : dict
             A dictionary containing all of the required settings
             needed to set up a square wave output.
 
@@ -266,33 +278,35 @@
         """
         Method to return a dictionary with the valid ramp wave
         settings to be passed to `self.set_output_channel`.
 
         Parameters
         ----------
         amplitude : float, optional
-             Waveform peak-to-peak amplitude in Volts. Allowed values
-             are 2e-3 to 10 for the Moku:Go and 1e-3 to 10 for the
-             Moku:Pro (For Moku:Pro, the output voltage is limited to
-             between -1V and 1V above 1MHz). Default is 1 V.
+            Waveform peak-to-peak amplitude in Volts. Allowed values
+            are 2e-3 to 10 for the Moku:Go, 2e-3 to 4 for the
+            Moku:Lab, and 1e-3 to 10 for the Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 1 V.
         frequency : float, optional
-             Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
-             for the Moku:Go and 1e-3 to 500e6 for the Moku:Pro.
-             Default is 10000 Hz.
+            Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
+            for the Moku:Go, 1e-3 to 100e6 for the Moku:Lab, and 1e-3
+            to 500e6 for the Moku:Pro. Default is 10000 (1e4) Hz.
         offset : float, optional
-             DC offset applied to the waveform in V. Allowed values are
-             -5 to 5 for Moku:Go and Moku:Pro (For Moku:Pro, the output
-             voltage is limited to between -1V and 1V above 1MHz).
-             Default is 0.
+            DC offset applied to the waveform in V. Allowed values are
+            -5 to 5 for Moku:Go, Moku:Lab, and Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 0.
         phase : float, optional
             Waveform phase offset in degrees. Allowed values are 0 to
-            360 for Moku:Go and Moku:Pro. Default is 0.
+            360 for Moku:Go, Moku:Lab, and Moku:Pro. Default is 0.
         symmetry : float, optional
             Fraction of the cycle rising in %. Allowed values are 0.0
-            to 100.0 for Moku:Go and Moku:Pro. Default is 50.
+            to 100.0 for Moku:Go, Moku:Lab, and Moku:Pro. Default is
+            50.
 
         Returns
         -------
         settings_dict : dict
             A dictionary containing all of the required settings
             needed to set up a ramp wave output.
 
@@ -312,42 +326,46 @@
         """
         Method to return a dictionary with the valid pulse train
         settings to be passed to `self.set_output_channel`.
 
         Parameters
         ----------
         amplitude : float, optional
-             Waveform peak-to-peak amplitude in Volts. Allowed values
-             are 2e-3 to 10 for the Moku:Go and 1e-3 to 10 for the
-             Moku:Pro (For Moku:Pro, the output voltage is limited to
-             between -1V and 1V above 1MHz). Default is 1 V.
+            Waveform peak-to-peak amplitude in Volts. Allowed values
+            are 2e-3 to 10 for the Moku:Go, 2e-3 to 4 for the
+            Moku:Lab, and 1e-3 to 10 for the Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 1 V.
         frequency : float, optional
-             Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
-             for the Moku:Go and 1e-3 to 500e6 for the Moku:Pro.
-             Default is 10000 Hz.
+            Waveform frequency in Hz. Allowed values are 1e-3 to 20e6
+            for the Moku:Go, 1e-3 to 100e6 for the Moku:Lab, and 1e-3
+            to 500e6 for the Moku:Pro. Default is 10000 (1e4) Hz.
         offset : float, optional
-             DC offset applied to the waveform in V. Allowed values are
-             -5 to 5 for Moku:Go and Moku:Pro (For Moku:Pro, the output
-             voltage is limited to between -1V and 1V above 1MHz).
-             Default is 0.
+            DC offset applied to the waveform in V. Allowed values are
+            -5 to 5 for Moku:Go, Moku:Lab, and Moku:Pro (For Moku:Pro,
+            the output voltage is limited to between -1V and 1V above
+            1MHz). Default is 0.
         phase : float, optional
             Waveform phase offset in degrees. Allowed values are 0 to
-            360 for Moku:Go and Moku:Pro. Default is 0.
+            360 for Moku:Go, Moku:Lab, and Moku:Pro. Default is 0.
         symmetry : float, optional
             Fraction of the cycle rising in %. Allowed values are 0.0
-            to 100.0 for Moku:Go and Moku:Pro. Default is 50.
+            to 100.0 for Moku:Go, Moku:Lab, and Moku:Pro. Default is
+            50.
         edge_time : float, optional
             Edge-time of the waveform in s. Allowed values are 16e-9 to
-            pulse_width for the Moku:Go and 2e-9 to pulse_width for the
-            Moku:Pro. Default is 0 (i.e. the shortest time).
+            pulse_width for the Moku:Go, 4e-9 to pulse_width for the
+            Moku:Lab, and 2e-9 to pulse_width for the Moku:Pro. Default
+            is 0 (which sets it to the shortest allowed time).
         pulse_width : float, optional
             Pulse width of the waveform in s. Allowed values are 16e-9
-            to waveform period for the Moku:Go and 2e-9 to waveform
-            period for the Moku:Pro. Default is 0 (i.e. ths shortest
-            time).
+            to waveform period for the Moku:Go, 4e-9 to waveform period
+            for the Moku:Lab and 2e-9 to waveform period for the
+            Moku:Pro. Default is 0 (which sets it to the shortest
+            allowed time).
 
         Returns
         -------
         settings_dict : dict
             A dictionary containing all of the required settings
             needed to set up a pulse train output.
 
@@ -396,30 +414,31 @@
         at a time.
 
         Parameters
         ----------
         channel : int
             The output channel to generate a waveform on. With a
             Moku:Pro, this must be an integer of 1, 2, 3 or 4. With a
-            Moku:Go, this must be an integer of 1 or 2.
+            Moku:Go or Moku:Lab, this must be an integer of 1 or 2.
         waveformtype : str
             The waveform type to generate, must be one of 'Sine',
             'Square', 'Ramp', 'Pulse', 'DC'. Can also be set to 'Off'
             to turn the channel off.
         load : str, optional
             The load impedance to use for the output channel. For a
-            Moku:Pro, this must be one of '1MOhm' or '50Ohm'. For a
-            Moku:Go, this can only be '1MOhm'. Default is '1MOhm'.
+            Moku:Pro or Moku:Lab, this must be one of '1MOhm' or
+            '50Ohm'. For a Moku:Go, this can only be '1MOhm'. Default
+            is '1MOhm'.
         settings : dict
             The dictionary containing all of the settings needed for
             the specified waveform type.
 
         """
 
-        if self._device == "Moku:Pro":
+        if self._device in ["Moku:Pro", "Moku:Lab"]:
             self.DL.set_output_load(channel, load)
         self.DL.generate_waveform(
             channel,
             waveformtype,
             **settings,
         )
 
@@ -475,13 +494,20 @@
                     remaining_time = progress['time_remaining']
                     is_logging = remaining_time >= 0
                 except:
                     is_logging = False
 
             filenames.append(logfile['file_name'])
 
+        if self._device == "Moku:Pro":
+            target = "ssd"
+        elif self._device == "Moku:Lab":
+            target = "media"
+        elif self._device == "Moku:Go":
+            target = "persist"
+
         for fname in filenames:
             self.DL.download(
-                "ssd" if self._device == "Moku:Pro" else "persist",
+                target,
                 fname,
                 os.path.abspath(savepath + os.sep + fname),
             )
```

### Comparing `splendaq-0.4.3/src/splendaq/daq/_offline_trigger.py` & `splendaq-0.4.4/src/splendaq/daq/_offline_trigger.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/daq/_oscilloscope.py` & `splendaq-0.4.4/src/splendaq/daq/_oscilloscope.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 
         self.Osc = Osc(
             ip_address, force_connect=force_connect, session_trust_env=False,
         )
         self.Osc.set_acquisition_mode(acquisition_mode)
 
         self._device = self.Osc.describe()['hardware']
-        if self._device not in ['Moku:Pro', 'Moku:Go']:
+        if self._device not in ['Moku:Pro', 'Moku:Lab', 'Moku:Go']:
             raise ValueError(
-                "Unrecognized device, is not a Moku:Go or Moku:Pro."
+                "Unrecognized device, is not a Moku:Go, Moku:Lab, or Moku:Pro."
             )
 
     def __enter__(self):
         """Returns self when entered via with."""
         return self
 
     def __exit__(self, type, value, traceback):
@@ -65,15 +65,15 @@
         Always run relinquish ownership and turn off inputs and outputs
         when exiting.
 
         """
 
         if self._device == "Moku:Pro":
             chan_list = [1, 2, 3, 4]
-        elif self._device == "Moku:Go":
+        elif self._device in ["Moku:Lab", "Moku:Go"]:
             chan_list = [1, 2]
 
         for chan in chan_list:
             self.Osc.generate_waveform(chan, 'Off') # disable outputs
             self.Osc.disable_input(chan) # disable inputs
 
         self.Osc.relinquish_ownership()
@@ -85,41 +85,45 @@
 
         Parameters
         ----------
         channels : int, list of int
             Which input channels to log data from. Can be a single
             value for one channel, or a list of the channels. For the
             Moku:Pro, valid channel numbers are 1, 2, 3, and 4. For the
-            Moku:Go, valid channel numbers are 1 and 2.
+            Moku:Lab and Moku:Go, valid channel numbers are 1 and 2.
         impedance : str, list of str, optional
             The output impedance to use for each channel. For the
-            Moku:Pro, options are '1MOhm' and '50Ohm'. For the Moku:Go,
-            the only option is '1MOhm'. Can pass a list of the same
-            length as channels if different impedances are desired for
-            a Moku:Pro. Default is '1MOhm' for all channels.
+            Moku:Pro and Moku:Lab, options are '1MOhm' and '50Ohm'. For
+            the Moku:Go, the only option is '1MOhm'. Can pass a list of
+            the same length as channels if different impedances are
+            desired for a Moku:Pro. Default is '1MOhm' for all channels.
         coupling : str, list of str, optional
             The coupling to use for each channel. Options are 'DC' and
             'AC'. Can pass a list of the same length as channels if
             different couplings are desired. Default is 'DC' for all
             channels.
         vrange : str, list of str, optional
             The voltage range to use for each channel. For the
             Moku:Pro, options are '400mVpp', '4Vpp' and '40Vpp'. For
-            the Moku:Go, options are '10Vpp' and '50Vpp'. Can pass a
-            list of the same length as channels if different voltage
-            ranges are desired for specific channels. Default is the
-            smallest allowed value for the device for all channels
-            (i.e. '400mVpp' for the Moku:Pro and '10Vpp' for the
-            Moku:Go).
+            the Moku:Lab, the options are '1Vpp' and '10Vpp'. For the
+            Moku:Go, options are '10Vpp' and '50Vpp'. Can pass a list
+            of the same length as channels if different voltage ranges
+            are desired for specific channels. Default is the smallest
+            allowed value for the device for all channels (i.e.
+            '400mVpp' for the Moku:Pro, '1Vpp' for the Moku:Lab, and
+            '10Vpp' for the Moku:Go).
 
         """
 
         if self._device == "Moku:Pro":
             chan_list = [1, 2, 3, 4]
             vrange = '400mVpp' if vrange is None else vrange
+        elif self._device == "Moku:Lab":
+            chan_list = [1, 2]
+            vrange = '1Vpp' if vrange is None else vrange
         elif self._device == "Moku:Go":
             chan_list = [1, 2]
             vrange = '10Vpp' if vrange is None else vrange
 
         if np.isscalar(channels):
             channels = [channels]
         if np.isscalar(impedance):
@@ -151,40 +155,41 @@
         at a time.
 
         Parameters
         ----------
         channel : int, list of int
             The output channel to generate a waveform on. With a
             Moku:Pro, this must be an integer of 1, 2, 3 or 4. With a
-            Moku:Go, this must be an integer of 1 or 2.
+            Moku:Lab or Moku:Go, this must be an integer of 1 or 2.
         waveformtype : str, list of str, optional
             The waveform type to generate, only supports 'DC' waveforms
             at the moment. Can also be set to 'Off' to turn the channel
             off. Default is 'DC'.
         load : str, list of str, optional
             The load impedance to use for the output channel. For a
-            Moku:Pro, this must be one of '1MOhm' or '50Ohm'. For a
-            Moku:Go, this can only be '1MOhm'. Default is '1MOhm'.
+            Moku:Pro or Moku:Lab, this must be one of '1MOhm' or
+            '50Ohm'. For a Moku:Go, this can only be '1MOhm'. Default
+            is '1MOhm'.
         dc_level : float, list of float, optional
-            The dictionary containing all of the settings needed for
-            the specified waveform type. Default is 0.
+            The DC level of the output of the channel in V. Default is
+            0.
 
         """
 
         if np.isscalar(channels):
             channels = [channels]
         if np.isscalar(waveformtype):
             waveformtype = [waveformtype] * len(channels)
         if np.isscalar(load):
             load = [load] * len(channels)
         if np.isscalar(dc_level):
             dc_level = [dc_level] * len(channels)
 
         for ind, chan in enumerate(channels):
-            if self._device == "Moku:Pro":
+            if self._device in ["Moku:Pro", "Moku:Lab"]:
                 self.Osc.set_output_load(chan, load[ind])
             self.Osc.generate_waveform(
                 channel=chan,
                 type=waveformtype[ind],
                 dc_level=dc_level[ind],
             )
 
@@ -194,17 +199,17 @@
         Returns a dictionary with the time domain values.
 
         Parameters
         ----------
         sources : str, list of str
             The sources which to read out in order of increasing
             channel number. Can be some combination of "Input1",
-            "Input2", "Output1", "Output2" for the Moku:Go, with
-            "Input3", "Input4", "Output3", and "Output4" also available
-            for the Moku:Pro.
+            "Input2", "Output1", "Output2" for the Moku:Go or Moku:Lab,
+            with "Input3", "Input4", "Output3", and "Output4" also
+            available for the Moku:Pro.
         duration : float
             The total time in seconds to collect data with the current
             configuration.
 
         Returns
         -------
         data : dict
@@ -220,8 +225,7 @@
 
         self.Osc.set_timebase(0, duration)
         time.sleep(duration)
 
         data = self.Osc.get_data()
 
         return data
-
```

### Comparing `splendaq-0.4.3/src/splendaq/daq/_sequencer.py` & `splendaq-0.4.4/src/splendaq/daq/_sequencer.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/io/_io.py` & `splendaq-0.4.4/src/splendaq/io/_io.py`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/io/_liconvert/COPYING.txt` & `splendaq-0.4.4/src/splendaq/io/_liconvert/COPYING.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_linux` & `splendaq-0.4.4/src/splendaq/io/_liconvert/liconvert_linux`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_macos` & `splendaq-0.4.4/src/splendaq/io/_liconvert/liconvert_macos`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq/io/_liconvert/liconvert_windows.exe` & `splendaq-0.4.4/src/splendaq/io/_liconvert/liconvert_windows.exe`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/src/splendaq.egg-info/PKG-INFO` & `splendaq-0.4.4/src/splendaq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splendaq
-Version: 0.4.3
+Version: 0.4.4
 Summary: Generalized offline data acquisition with a focus on the Moku
 Home-page: https://github.com/splendor-collab/splendaq
 Author: SPLENDOR Collaboration
 Maintainer: SPLENDOR Collaboration
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `splendaq-0.4.3/src/splendaq.egg-info/SOURCES.txt` & `splendaq-0.4.4/src/splendaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/tutorials/daq/dc_oscilloscope.ipynb` & `splendaq-0.4.4/tutorials/daq/dc_oscilloscope.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/tutorials/daq/event_building.ipynb` & `splendaq-0.4.4/tutorials/daq/event_building.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/tutorials/daq/logging_data.ipynb` & `splendaq-0.4.4/tutorials/daq/logging_data.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/tutorials/daq/running_the_sequencer.ipynb` & `splendaq-0.4.4/tutorials/daq/running_the_sequencer.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/tutorials/daq/sequencer_settings.yaml` & `splendaq-0.4.4/tutorials/daq/sequencer_settings.yaml`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/tutorials/io/read_files.ipynb` & `splendaq-0.4.4/tutorials/io/read_files.ipynb`

 * *Files identical despite different names*

### Comparing `splendaq-0.4.3/tutorials/io/write_files.ipynb` & `splendaq-0.4.4/tutorials/io/write_files.ipynb`

 * *Files identical despite different names*

