# Comparing `tmp/pump_offline_calibration_plugin-1.0.0-py3-none-any.whl.zip` & `tmp/pump_offline_calibration_plugin-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 10278 bytes, number of entries: 10
+Zip file size: 10265 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      109 b- defN 23-Jun-21 19:56 pump_offline_calibration_plugin/__init__.py
--rw-r--r--  2.0 unx    20533 b- defN 23-Jun-22 04:27 pump_offline_calibration_plugin/pump_offline_calibration.py
+-rw-r--r--  2.0 unx    20523 b- defN 23-Jun-22 21:04 pump_offline_calibration_plugin/pump_offline_calibration.py
 -rw-r--r--  2.0 unx     6885 b- defN 23-Jun-21 15:28 pump_offline_calibration_plugin/test_pump_offline_calibration.py
 -rw-r--r--  2.0 unx      145 b- defN 23-Jun-21 19:50 pump_offline_calibration_plugin/ui/contrib/jobs/pump_offline_calibration_plugin.yaml
--rw-rw-r--  2.0 unx     1055 b- defN 23-Jun-22 04:41 pump_offline_calibration_plugin-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1250 b- defN 23-Jun-22 04:41 pump_offline_calibration_plugin-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 04:41 pump_offline_calibration_plugin-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-22 04:41 pump_offline_calibration_plugin-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       32 b- defN 23-Jun-22 04:41 pump_offline_calibration_plugin-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1106 b- defN 23-Jun-22 04:41 pump_offline_calibration_plugin-1.0.0.dist-info/RECORD
-10 files, 31294 bytes uncompressed, 8302 bytes compressed:  73.5%
+-rw-rw-r--  2.0 unx     1055 b- defN 23-Jul-18 19:32 pump_offline_calibration_plugin-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1250 b- defN 23-Jul-18 19:32 pump_offline_calibration_plugin-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-18 19:32 pump_offline_calibration_plugin-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jul-18 19:32 pump_offline_calibration_plugin-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       32 b- defN 23-Jul-18 19:32 pump_offline_calibration_plugin-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-18 19:32 pump_offline_calibration_plugin-1.0.1.dist-info/RECORD
+10 files, 31284 bytes uncompressed, 8289 bytes compressed:  73.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: pump_offline_calibration_plugin/test_pump_offline_calibration.py
 Comment: 
 
 Filename: pump_offline_calibration_plugin/ui/contrib/jobs/pump_offline_calibration_plugin.yaml
 Comment: 
 
-Filename: pump_offline_calibration_plugin-1.0.0.dist-info/LICENSE.txt
+Filename: pump_offline_calibration_plugin-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pump_offline_calibration_plugin-1.0.0.dist-info/METADATA
+Filename: pump_offline_calibration_plugin-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pump_offline_calibration_plugin-1.0.0.dist-info/WHEEL
+Filename: pump_offline_calibration_plugin-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pump_offline_calibration_plugin-1.0.0.dist-info/entry_points.txt
+Filename: pump_offline_calibration_plugin-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pump_offline_calibration_plugin-1.0.0.dist-info/top_level.txt
+Filename: pump_offline_calibration_plugin-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pump_offline_calibration_plugin-1.0.0.dist-info/RECORD
+Filename: pump_offline_calibration_plugin-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pump_offline_calibration_plugin/pump_offline_calibration.py

```diff
@@ -158,15 +158,14 @@
             )
         return ("waste", remove_waste)
     else:
         raise ValueError()
 
 
 def choose_settings() -> tuple[float, float]:
-    current_hz = 
     hz = click.prompt(
         click.style(
             "Optional: Enter frequency of PWM. [enter] for current setting 250 hz", fg="green"
         ),
         type=click.FloatRange(0.1, 10000),
         default=250,
         show_default=False,
@@ -280,15 +279,15 @@
             while not click.confirm(
                 click.style(f"Ready to test {duration:.2f}s?", fg="green")
             ):
                 pass
 
             execute_pump(
                 duration=duration,
-                source_of_event="pump_calibration",
+                source_of_event="pump_offline_calibration",
                 unit=get_unit_name(),
                 experiment=get_latest_testing_experiment_name(),
                 calibration=empty_calibration,
             )
 
             r = click.prompt(
                 click.style(
```

## Comparing `pump_offline_calibration_plugin-1.0.0.dist-info/LICENSE.txt` & `pump_offline_calibration_plugin-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pump_offline_calibration_plugin-1.0.0.dist-info/METADATA` & `pump_offline_calibration_plugin-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pump-offline-calibration-plugin
-Version: 1.0.0
+Version: 1.0.1
 Summary: Perform an offline calibration of pumps.
 Home-page: https://github.com/odcambc/pump_offline_calibration_plugin
 Author: Chris Macdonald
 Author-email: christian.macdonald@ucsf.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `pump_offline_calibration_plugin-1.0.0.dist-info/RECORD` & `pump_offline_calibration_plugin-1.0.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pump_offline_calibration_plugin/__init__.py,sha256=LDYIa0VP7xyltbl3qS4R0VtTBBjZEMBJo6bM1XHVTHs,109
-pump_offline_calibration_plugin/pump_offline_calibration.py,sha256=4IG2DgWbEn8_3SJnsvPV8zrISq0-wSDdoUfzPP0axqc,20533
+pump_offline_calibration_plugin/pump_offline_calibration.py,sha256=_4uTho0Li-uE7VmnC0lMkSn5Q87MZipTlp6xUFi3OnQ,20523
 pump_offline_calibration_plugin/test_pump_offline_calibration.py,sha256=J2CqdM3SVxWQWzJBIOJHZ5xzU1X7E392XQ4rBrXuWSw,6885
 pump_offline_calibration_plugin/ui/contrib/jobs/pump_offline_calibration_plugin.yaml,sha256=uULBDc_imxWKKDp0B4MvwSg0nGwiSYzKLk93tGx78nU,145
-pump_offline_calibration_plugin-1.0.0.dist-info/LICENSE.txt,sha256=4cGjN4WDkfnBYIZNxNLrtNoai7jxokShSPCzz-qtFN4,1055
-pump_offline_calibration_plugin-1.0.0.dist-info/METADATA,sha256=xWX07EKsUiatPVlG16f1ZLpCkLvX-8QT-8afsQk2IJo,1250
-pump_offline_calibration_plugin-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pump_offline_calibration_plugin-1.0.0.dist-info/entry_points.txt,sha256=eRVbtB3jH4WG3Ux-Ye8QqYxqXlSxeLxrWDquMoDJnu8,87
-pump_offline_calibration_plugin-1.0.0.dist-info/top_level.txt,sha256=iZsyOttC-iz_ZEigYfJRFkJ4D6rwt_l-ixK-nES09R0,32
-pump_offline_calibration_plugin-1.0.0.dist-info/RECORD,,
+pump_offline_calibration_plugin-1.0.1.dist-info/LICENSE.txt,sha256=4cGjN4WDkfnBYIZNxNLrtNoai7jxokShSPCzz-qtFN4,1055
+pump_offline_calibration_plugin-1.0.1.dist-info/METADATA,sha256=tgaaAFyjuk7sdqtG8sH2E4Zbmqy73IvJMicBOf_0JGI,1250
+pump_offline_calibration_plugin-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pump_offline_calibration_plugin-1.0.1.dist-info/entry_points.txt,sha256=eRVbtB3jH4WG3Ux-Ye8QqYxqXlSxeLxrWDquMoDJnu8,87
+pump_offline_calibration_plugin-1.0.1.dist-info/top_level.txt,sha256=iZsyOttC-iz_ZEigYfJRFkJ4D6rwt_l-ixK-nES09R0,32
+pump_offline_calibration_plugin-1.0.1.dist-info/RECORD,,
```

