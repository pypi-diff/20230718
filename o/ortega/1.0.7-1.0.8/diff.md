# Comparing `tmp/ortega-1.0.7.tar.gz` & `tmp/ortega-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ortega-1.0.7.tar", last modified: Thu Jun 29 23:27:56 2023, max compression
+gzip compressed data, was "ortega-1.0.8.tar", last modified: Tue Jul 18 03:29:16 2023, max compression
```

## Comparing `ortega-1.0.7.tar` & `ortega-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:27:56.347926 ortega-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 23:27:41.000000 ortega-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 23:27:56.347926 ortega-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-29 23:27:41.000000 ortega-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:27:56.347926 ortega-1.0.7/ortega/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/STPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/ellipses.py
--rw-r--r--   0 runner    (1001) docker     (123)    27623 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/ortega.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-29 23:27:41.000000 ortega-1.0.7/ortega/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:27:56.347926 ortega-1.0.7/ortega.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 23:27:56.000000 ortega-1.0.7/ortega.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 23:27:56.347926 ortega-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 23:27:41.000000 ortega-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:29:16.847339 ortega-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 03:29:05.000000 ortega-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 03:29:16.847339 ortega-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-18 03:29:05.000000 ortega-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:29:16.843339 ortega-1.0.8/ortega/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/STPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8448 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/ellipses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31036 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/ortega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-18 03:29:05.000000 ortega-1.0.8/ortega/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:29:16.843339 ortega-1.0.8/ortega.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-18 03:29:16.000000 ortega-1.0.8/ortega.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:29:16.847339 ortega-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-18 03:29:05.000000 ortega-1.0.8/setup.py
```

### Comparing `ortega-1.0.7/LICENSE` & `ortega-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ortega-1.0.7/README.md` & `ortega-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ortega-1.0.7/ortega/STPoint.py` & `ortega-1.0.8/ortega/STPoint.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.7/ortega/ellipses.py` & `ortega-1.0.8/ortega/ellipses.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.7/ortega/ortega.py` & `ortega-1.0.8/ortega/ortega.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .ellipses import Ellipse, EllipseList
 from pandas.api.types import is_datetime64_dtype
 from typing import List, Tuple
 from .common import __timedifcheck
 from .common import *
 from .output import *
 
+
 def __check_spatial_intersect(item: Ellipse, others: Ellipse) -> bool:
     """
     test
     :param item:
     :param others:
     :return:
     """
@@ -92,18 +93,40 @@
     p1_start_time, p1_end_time, p2_start_time, p2_end_time = [], [], [], []
     p1_start_index, p1_end_index = [], []
     p1_start_time.append(p1start[0])
     p1_start_index.append(0)
     for i in range(1, len(p1start)):
         if datetime.strptime(str(p1start[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i - 1]),
                                                                                         '%Y-%m-%d %H:%M:%S'):
-            continue
+            if datetime.strptime(str(p2start[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p2start[i - 1]),
+                                                                                            '%Y-%m-%d %H:%M:%S'):
+                continue
+            elif datetime.strptime(str(p2end[i - 1]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(
+                    str(p2start[i]),'%Y-%m-%d %H:%M:%S') or datetime.strptime(
+                    str(p2start[i - 1]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p2end[i]), '%Y-%m-%d %H:%M:%S'):
+                continue
+            else:
+                p1_end_time.append(p1end[i - 1])
+                p1_end_index.append(i - 1)
+                p1_start_time.append(p1start[i])
+                p1_start_index.append(i)
         elif datetime.strptime(str(p1end[i - 1]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p1start[i]),
                                                                                         '%Y-%m-%d %H:%M:%S'):
-            continue
+            if datetime.strptime(str(p2start[i]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p2start[i - 1]),
+                                                                                            '%Y-%m-%d %H:%M:%S'):
+                continue
+            elif datetime.strptime(str(p2end[i - 1]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(
+                    str(p2start[i]), '%Y-%m-%d %H:%M:%S') or datetime.strptime(
+                    str(p2start[i - 1]), '%Y-%m-%d %H:%M:%S') == datetime.strptime(str(p2end[i]), '%Y-%m-%d %H:%M:%S'):
+                continue
+            else:
+                p1_end_time.append(p1end[i - 1])
+                p1_end_index.append(i - 1)
+                p1_start_time.append(p1start[i])
+                p1_start_index.append(i)
         else:
             p1_end_time.append(p1end[i - 1])
             p1_end_index.append(i - 1)
             p1_start_time.append(p1start[i])
             p1_start_index.append(i)
     p1_end_time.append(p1end[len(p1end) - 1])
     p1_end_index.append(len(p1end) - 1)
@@ -497,14 +520,15 @@
                     (self.data[self.time_field] >= start_time) & (self.data[self.time_field] <= end_time)]
                 self.df1 = self.subset[self.subset[self.id_field] == self.id1]
                 self.df2 = self.subset[self.subset[self.id_field] == self.id2]
             else:
                 self.df1 = self.data[self.data[self.id_field] == self.id1]
                 self.df2 = self.data[self.data[self.id_field] == self.id2]
 
+            # Check time overlap and lag, stop initialization if conditions are not met
             if not self.__check_time_lag_and_overlap():
                 raise ValueError(f"Skipping pair {self.id1} and {self.id2} due to time lag greater than {self.minute_max_delay}!")
 
     def __start(self):
         """
         create PPAs for two moving objects (private method, only can be called inside the class)
         ellipses_list: all PPAs for two objects
@@ -542,14 +566,44 @@
             print(datetime.now(), f'Complete! {df_continues.shape[0]} interaction events identified!')
             if df_continues.shape[0] != 0:
                 results.set_df_interaction_events(df_continues)
                 return results
             else:
                 return None
 
+    def interaction_analysis2(self):
+        # old method， voided but just keep it for reference
+        print(datetime.now(), 'Implement interaction analysis...')
+        spatial_pairs = self.__get_spatial_intersect_pairs()
+        all_intersection_pairs = get_timedelay_pairs(spatial_pairs, self.minute_min_delay, self.minute_max_delay)
+        if not all_intersection_pairs:
+            print(datetime.now(), 'Complete! No interaction found!')
+            return None
+        else:
+            print(datetime.now(), f'Complete! {len(all_intersection_pairs)} pairs of intersecting PPAs found!')
+            results = ORTEGAResults()
+            results.set_intersection_ellipse_pair(all_intersection_pairs)
+
+            # convert the list of intersecting ellipses to dataframe format - df_all_intersection_pairs
+            df_all_intersection_pairs = intersect_ellipse_todataframe(all_intersection_pairs)
+            df_all_intersection_pairs = interaction_compute_speed_diff(df_all_intersection_pairs)
+            df_all_intersection_pairs = interaction_compute_direction_diff(df_all_intersection_pairs)
+            df_all_intersection_pairs = interaction_compute_time_diff(df_all_intersection_pairs)
+            results.set_df_all_intersection_pairs(df_all_intersection_pairs)
+
+            # compute duration of interaction and output as a dataframe - df_duration
+            print(datetime.now(), 'Compute duration of interaction...')
+            df_duration = durationEstimator(df_all_intersection_pairs, self.id1, self.id2)
+            print(datetime.now(), f'Complete! {df_duration.shape[0]} interaction events identified!')
+            if df_duration.shape[0] != 0:
+                results.set_df_interaction_events(df_duration)
+                return results
+            else:
+                return None
+
     def __check_time_lag_and_overlap(self):
         """
         Check time overlap and time lag between the movements of two individuals (private method, only can be called inside the class).
         Returns a boolean value indicating whether the time lag is less than or equal to the allowable maximum delay (True) or not (False).
         """
         # Extract the start and end times for each individual
         start1, end1 = self.df1[self.time_field].min(), self.df1[self.time_field].max()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ortega-1.0.7/ortega/output.py` & `ortega-1.0.8/ortega/output.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.7/ortega/visualization.py` & `ortega-1.0.8/ortega/visualization.py`

 * *Files identical despite different names*

### Comparing `ortega-1.0.7/setup.py` & `ortega-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 if __name__ == "__main__":
     setup(
         name='ortega',
-        version='1.0.7',
+        version='1.0.8',
         author='MOVE lab@UCSB',
         author_email="rongxiangsu@ucsb.edu",
         packages=["ortega"],
         url='https://github.com/move-ucsb/ORTEGA',
         license='MIT',
         description='ORTEGA',
         install_requires=[
```

