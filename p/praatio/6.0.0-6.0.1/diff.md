# Comparing `tmp/praatio-6.0.0.tar.gz` & `tmp/praatio-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "praatio-6.0.0.tar", last modified: Sun Feb  5 09:51:15 2023, max compression
+gzip compressed data, was "praatio-6.0.1.tar", last modified: Tue Jul 18 14:14:12 2023, max compression
```

## Comparing `praatio-6.0.0.tar` & `praatio-6.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-02-05 09:51:15.939938 praatio-6.0.0/
--rw-r--r--   0 tmahrt     (501) staff       (20)     1130 2023-02-05 09:50:21.000000 praatio-6.0.0/LICENSE
--rw-r--r--   0 tmahrt     (501) staff       (20)     8768 2023-02-05 09:51:15.942359 praatio-6.0.0/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)     8392 2023-02-05 09:50:40.000000 praatio-6.0.0/README.md
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-02-05 09:51:15.871321 praatio-6.0.0/praatio/
--rw-r--r--   0 tmahrt     (501) staff       (20)     1853 2021-12-31 13:39:38.000000 praatio-6.0.0/praatio/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    16122 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/audio.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-02-05 09:51:15.889923 praatio-6.0.0/praatio/data_classes/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2021-12-31 12:35:23.000000 praatio-6.0.0/praatio/data_classes/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     4047 2022-01-02 03:11:43.000000 praatio-6.0.0/praatio/data_classes/data_point.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    26223 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/data_classes/interval_tier.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     8145 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/data_classes/klattgrid.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    13118 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/data_classes/point_tier.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    21548 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/data_classes/textgrid.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     7762 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/data_classes/textgrid_tier.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     3318 2022-01-02 03:40:34.000000 praatio-6.0.0/praatio/data_points.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     8004 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/klattgrid.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    19983 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/pitch_and_intensity.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-02-05 09:51:15.902144 praatio-6.0.0/praatio/praatScripts/
--rw-r--r--   0 tmahrt     (501) staff       (20)     1082 2021-07-09 10:24:21.000000 praatio-6.0.0/praatio/praatScripts/annotate_silences.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      515 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/change_gender.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      311 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/change_intensity.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     1736 2019-01-01 00:20:01.000000 praatio-6.0.0/praatio/praatScripts/get_formants.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     1518 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/get_intensity.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     3790 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/get_pitch.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     4110 2021-04-04 00:19:55.000000 praatio-6.0.0/praatio/praatScripts/get_pitch_and_intensity.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     2311 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/get_pitch_and_intensity_segments.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     2726 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/get_pitchtier.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      588 2019-01-01 00:20:01.000000 praatio-6.0.0/praatio/praatScripts/get_pulses.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     3272 2019-01-01 00:20:01.000000 praatio-6.0.0/praatio/praatScripts/get_spectral_info.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      627 2019-01-01 00:20:01.000000 praatio-6.0.0/praatio/praatScripts/resynthesize_duration.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      376 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/resynthesize_from_klattgrid.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      703 2019-01-01 00:20:01.000000 praatio-6.0.0/praatio/praatScripts/resynthesize_pitch.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      668 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/praatScripts/sound_to_klattgrid.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)     8091 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/praat_scripts.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    18014 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/praatio_scripts.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     4441 2023-01-08 06:39:23.000000 praatio-6.0.0/praatio/textgrid.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      501 2021-08-09 12:32:45.000000 praatio-6.0.0/praatio/tgio.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-02-05 09:51:15.938173 praatio-6.0.0/praatio/utilities/
--rw-r--r--   0 tmahrt     (501) staff       (20)       58 2021-12-31 12:45:19.000000 praatio-6.0.0/praatio/utilities/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2530 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/utilities/constants.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     3946 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/utilities/errors.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     7025 2022-01-02 03:16:24.000000 praatio-6.0.0/praatio/utilities/my_math.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    20156 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/utilities/textgrid_io.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1170 2021-08-08 06:37:30.000000 praatio-6.0.0/praatio/utilities/timit.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    15558 2023-02-05 09:50:21.000000 praatio-6.0.0/praatio/utilities/utils.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-02-05 09:51:15.874443 praatio-6.0.0/praatio.egg-info/
--rw-r--r--   0 tmahrt     (501) staff       (20)     8768 2023-02-05 09:51:15.000000 praatio-6.0.0/praatio.egg-info/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)     1520 2023-02-05 09:51:15.000000 praatio-6.0.0/praatio.egg-info/SOURCES.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        1 2023-02-05 09:51:15.000000 praatio-6.0.0/praatio.egg-info/dependency_links.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       18 2023-02-05 09:51:15.000000 praatio-6.0.0/praatio.egg-info/requires.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        8 2023-02-05 09:51:15.000000 praatio-6.0.0/praatio.egg-info/top_level.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       73 2023-02-05 09:51:15.943493 praatio-6.0.0/setup.cfg
--rw-r--r--   0 tmahrt     (501) staff       (20)      869 2023-02-05 09:50:21.000000 praatio-6.0.0/setup.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-18 14:14:12.070642 praatio-6.0.1/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1130 2023-02-05 09:50:21.000000 praatio-6.0.1/LICENSE
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8768 2023-07-18 14:14:12.070830 praatio-6.0.1/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8392 2023-02-05 09:56:38.000000 praatio-6.0.1/README.md
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-18 14:14:12.037724 praatio-6.0.1/praatio/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1853 2021-12-31 13:39:38.000000 praatio-6.0.1/praatio/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    16122 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/audio.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-18 14:14:12.047695 praatio-6.0.1/praatio/data_classes/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2021-12-31 12:35:23.000000 praatio-6.0.1/praatio/data_classes/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     4047 2022-01-02 03:11:43.000000 praatio-6.0.1/praatio/data_classes/data_point.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    26259 2023-07-18 14:10:38.000000 praatio-6.0.1/praatio/data_classes/interval_tier.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8145 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/data_classes/klattgrid.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    13118 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/data_classes/point_tier.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    21548 2023-02-18 07:50:58.000000 praatio-6.0.1/praatio/data_classes/textgrid.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     7762 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/data_classes/textgrid_tier.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3318 2022-01-02 03:40:34.000000 praatio-6.0.1/praatio/data_points.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8004 2023-02-05 09:50:21.000000 praatio-6.0.1/praatio/klattgrid.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    19983 2023-02-05 09:50:21.000000 praatio-6.0.1/praatio/pitch_and_intensity.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-18 14:14:12.062252 praatio-6.0.1/praatio/praatScripts/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1082 2021-07-09 10:24:21.000000 praatio-6.0.1/praatio/praatScripts/annotate_silences.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      515 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/change_gender.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      311 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/change_intensity.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1736 2019-01-01 00:20:01.000000 praatio-6.0.1/praatio/praatScripts/get_formants.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1518 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/get_intensity.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3790 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/get_pitch.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     4110 2021-04-04 00:19:55.000000 praatio-6.0.1/praatio/praatScripts/get_pitch_and_intensity.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2311 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/get_pitch_and_intensity_segments.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2726 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/get_pitchtier.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      588 2019-01-01 00:20:01.000000 praatio-6.0.1/praatio/praatScripts/get_pulses.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3272 2019-01-01 00:20:01.000000 praatio-6.0.1/praatio/praatScripts/get_spectral_info.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      627 2019-01-01 00:20:01.000000 praatio-6.0.1/praatio/praatScripts/resynthesize_duration.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      376 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/resynthesize_from_klattgrid.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      703 2019-01-01 00:20:01.000000 praatio-6.0.1/praatio/praatScripts/resynthesize_pitch.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      668 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/praatScripts/sound_to_klattgrid.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8091 2023-02-05 09:50:21.000000 praatio-6.0.1/praatio/praat_scripts.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    18014 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/praatio_scripts.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     4441 2023-01-08 06:39:23.000000 praatio-6.0.1/praatio/textgrid.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      501 2021-08-09 12:32:45.000000 praatio-6.0.1/praatio/tgio.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-18 14:14:12.069833 praatio-6.0.1/praatio/utilities/
+-rw-r--r--   0 tmahrt     (501) staff       (20)       58 2021-12-31 12:45:19.000000 praatio-6.0.1/praatio/utilities/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2530 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/utilities/constants.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3946 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/utilities/errors.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     7025 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/utilities/my_math.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    20156 2023-02-05 09:50:21.000000 praatio-6.0.1/praatio/utilities/textgrid_io.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1170 2021-08-08 06:37:30.000000 praatio-6.0.1/praatio/utilities/timit.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    15558 2023-07-18 13:54:54.000000 praatio-6.0.1/praatio/utilities/utils.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-18 14:14:12.041034 praatio-6.0.1/praatio.egg-info/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     8768 2023-07-18 14:14:11.000000 praatio-6.0.1/praatio.egg-info/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1520 2023-07-18 14:14:11.000000 praatio-6.0.1/praatio.egg-info/SOURCES.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        1 2023-07-18 14:14:11.000000 praatio-6.0.1/praatio.egg-info/dependency_links.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       18 2023-07-18 14:14:11.000000 praatio-6.0.1/praatio.egg-info/requires.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        8 2023-07-18 14:14:11.000000 praatio-6.0.1/praatio.egg-info/top_level.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       73 2023-07-18 14:14:12.071510 praatio-6.0.1/setup.cfg
+-rw-r--r--   0 tmahrt     (501) staff       (20)      869 2023-07-18 14:10:38.000000 praatio-6.0.1/setup.py
```

### Comparing `praatio-6.0.0/LICENSE` & `praatio-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/PKG-INFO` & `praatio-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praatio
-Version: 6.0.0
+Version: 6.0.1
 Summary: A library for working with praat, textgrids, time aligned audio transcripts, and audio files.
 Home-page: https://github.com/timmahrt/praatIO
 Author: Tim Mahrt
 Author-email: timmahrt@gmail.com
 License: LICENSE
 Platform: UNKNOWN
 Requires-Python: >3.6.0
```

### Comparing `praatio-6.0.0/README.md` & `praatio-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/__init__.py` & `praatio-6.0.1/praatio/__init__.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/audio.py` & `praatio-6.0.1/praatio/audio.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/data_classes/data_point.py` & `praatio-6.0.1/praatio/data_classes/data_point.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/data_classes/interval_tier.py` & `praatio-6.0.1/praatio/data_classes/interval_tier.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,16 @@
                     f"cannot occur after its end time ({entry.end})"
                 )
 
         for entry, nextEntry in zip(self.entries[0::], self.entries[1::]):
             if entry.end > nextEntry.start:
                 raise errors.TextgridStateError(
                     "Two intervals in the same tier overlap in time:\n"
-                    f"({entry.start}, {entry.end}, {entry.label}) and ({entry.start}, {entry.end}, {entry.label})"
+                    f"({entry.start}, {entry.end}, {entry.label}) and "
+                    f"({nextEntry.start}, {nextEntry.end}, {nextEntry.label})"
                 )
 
     def crop(
         self,
         cropStart: float,
         cropEnd: float,
         mode: Literal["strict", "lax", "truncated"],
```

### Comparing `praatio-6.0.0/praatio/data_classes/klattgrid.py` & `praatio-6.0.1/praatio/data_classes/klattgrid.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/data_classes/point_tier.py` & `praatio-6.0.1/praatio/data_classes/point_tier.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/data_classes/textgrid.py` & `praatio-6.0.1/praatio/data_classes/textgrid.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/data_classes/textgrid_tier.py` & `praatio-6.0.1/praatio/data_classes/textgrid_tier.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/data_points.py` & `praatio-6.0.1/praatio/data_points.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/klattgrid.py` & `praatio-6.0.1/praatio/klattgrid.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/pitch_and_intensity.py` & `praatio-6.0.1/praatio/pitch_and_intensity.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/annotate_silences.praat` & `praatio-6.0.1/praatio/praatScripts/annotate_silences.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/change_gender.praat` & `praatio-6.0.1/praatio/praatScripts/change_gender.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_formants.praat` & `praatio-6.0.1/praatio/praatScripts/get_formants.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_intensity.praat` & `praatio-6.0.1/praatio/praatScripts/get_intensity.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_pitch.praat` & `praatio-6.0.1/praatio/praatScripts/get_pitch.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_pitch_and_intensity.praat` & `praatio-6.0.1/praatio/praatScripts/get_pitch_and_intensity.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_pitch_and_intensity_segments.praat` & `praatio-6.0.1/praatio/praatScripts/get_pitch_and_intensity_segments.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_pitchtier.praat` & `praatio-6.0.1/praatio/praatScripts/get_pitchtier.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_pulses.praat` & `praatio-6.0.1/praatio/praatScripts/get_pulses.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/get_spectral_info.praat` & `praatio-6.0.1/praatio/praatScripts/get_spectral_info.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/resynthesize_duration.praat` & `praatio-6.0.1/praatio/praatScripts/resynthesize_duration.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/resynthesize_pitch.praat` & `praatio-6.0.1/praatio/praatScripts/resynthesize_pitch.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatScripts/sound_to_klattgrid.praat` & `praatio-6.0.1/praatio/praatScripts/sound_to_klattgrid.praat`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praat_scripts.py` & `praatio-6.0.1/praatio/praat_scripts.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/praatio_scripts.py` & `praatio-6.0.1/praatio/praatio_scripts.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/textgrid.py` & `praatio-6.0.1/praatio/textgrid.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/utilities/constants.py` & `praatio-6.0.1/praatio/utilities/constants.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/utilities/errors.py` & `praatio-6.0.1/praatio/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/utilities/my_math.py` & `praatio-6.0.1/praatio/utilities/my_math.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/utilities/textgrid_io.py` & `praatio-6.0.1/praatio/utilities/textgrid_io.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/utilities/timit.py` & `praatio-6.0.1/praatio/utilities/timit.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio/utilities/utils.py` & `praatio-6.0.1/praatio/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/praatio.egg-info/PKG-INFO` & `praatio-6.0.1/praatio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: praatio
-Version: 6.0.0
+Version: 6.0.1
 Summary: A library for working with praat, textgrids, time aligned audio transcripts, and audio files.
 Home-page: https://github.com/timmahrt/praatIO
 Author: Tim Mahrt
 Author-email: timmahrt@gmail.com
 License: LICENSE
 Platform: UNKNOWN
 Requires-Python: >3.6.0
```

### Comparing `praatio-6.0.0/praatio.egg-info/SOURCES.txt` & `praatio-6.0.1/praatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `praatio-6.0.0/setup.py` & `praatio-6.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from setuptools import setup
 import io
 
 setup(
     name="praatio",
     python_requires=">3.6.0",
-    version="6.0.0",
+    version="6.0.1",
     author="Tim Mahrt",
     author_email="timmahrt@gmail.com",
     url="https://github.com/timmahrt/praatIO",
     package_dir={"praatio": "praatio"},
     packages=["praatio", "praatio.utilities", "praatio.data_classes"],
     package_data={
         "praatio": [
```

