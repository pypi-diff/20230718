# Comparing `tmp/dms-influx2-0.3.4.tar.gz` & `tmp/dms-influx2-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dms-influx2-0.3.4.tar", last modified: Mon Jul 17 06:12:24 2023, max compression
+gzip compressed data, was "dist\dms-influx2-0.3.5.tar", last modified: Tue Jul 18 12:09:10 2023, max compression
```

## Comparing `dms-influx2-0.3.4.tar` & `dms-influx2-0.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.439363 dms-influx2-0.3.4/
--rw-rw-rw-   0        0        0      556 2023-07-17 06:12:24.438365 dms-influx2-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.433359 dms-influx2-0.3.4/dms_influx2/
--rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/__init__.py
--rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/authorizations.py
--rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.4/dms_influx2/buckets.py
--rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.4/dms_influx2/checks.py
--rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/decorators.py
--rw-rw-rw-   0        0        0     2729 2023-07-03 09:35:10.000000 dms-influx2-0.3.4/dms_influx2/delete.py
--rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.4/dms_influx2/dtv_files.py
--rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/exceptions.py
--rw-rw-rw-   0        0        0    25730 2023-07-14 15:05:32.000000 dms-influx2-0.3.4/dms_influx2/lib.py
--rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/notifications.py
--rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/organisations.py
--rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.4/dms_influx2/query.py
--rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.4/dms_influx2/sync.py
--rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.4/dms_influx2/tasks.py
--rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.4/dms_influx2/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.436365 dms-influx2-0.3.4/dms_influx2.egg-info/
--rw-rw-rw-   0        0        0      556 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-17 06:12:24.000000 dms-influx2-0.3.4/dms_influx2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 06:12:24.439363 dms-influx2-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     3023 2023-07-17 06:11:13.000000 dms-influx2-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 06:12:24.438365 dms-influx2-0.3.4/tests/
--rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.4/tests/test_auth.py
--rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.4/tests/test_buckets.py
--rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.4/tests/test_copy-values.py
--rw-rw-rw-   0        0        0    16796 2023-07-14 12:09:20.000000 dms-influx2-0.3.4/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:09:10.927886 dms-influx2-0.3.5/
+-rw-rw-rw-   0        0        0      556 2023-07-18 12:09:10.927314 dms-influx2-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 12:09:10.904699 dms-influx2-0.3.5/dms_influx2/
+-rw-rw-rw-   0        0        0        0 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/dms_influx2/__init__.py
+-rw-rw-rw-   0        0        0     5108 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/dms_influx2/authorizations.py
+-rw-rw-rw-   0        0        0     6376 2023-03-22 11:19:56.000000 dms-influx2-0.3.5/dms_influx2/buckets.py
+-rw-rw-rw-   0        0        0     5591 2023-01-19 07:18:35.000000 dms-influx2-0.3.5/dms_influx2/checks.py
+-rw-rw-rw-   0        0        0      630 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/dms_influx2/decorators.py
+-rw-rw-rw-   0        0        0     2902 2023-07-18 11:25:41.000000 dms-influx2-0.3.5/dms_influx2/delete.py
+-rw-rw-rw-   0        0        0     1487 2023-01-19 06:30:10.000000 dms-influx2-0.3.5/dms_influx2/dtv_files.py
+-rw-rw-rw-   0        0        0      327 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/dms_influx2/exceptions.py
+-rw-rw-rw-   0        0        0    35137 2023-07-18 12:07:41.000000 dms-influx2-0.3.5/dms_influx2/lib.py
+-rw-rw-rw-   0        0        0     3562 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/dms_influx2/notifications.py
+-rw-rw-rw-   0        0        0     1012 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/dms_influx2/organisations.py
+-rw-rw-rw-   0        0        0     7217 2023-07-04 18:39:09.000000 dms-influx2-0.3.5/dms_influx2/query.py
+-rw-rw-rw-   0        0        0        0 2023-01-18 17:42:37.000000 dms-influx2-0.3.5/dms_influx2/sync.py
+-rw-rw-rw-   0        0        0     4025 2023-01-09 21:18:36.000000 dms-influx2-0.3.5/dms_influx2/tasks.py
+-rw-rw-rw-   0        0        0     1203 2023-01-26 19:35:58.000000 dms-influx2-0.3.5/dms_influx2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:09:10.914202 dms-influx2-0.3.5/dms_influx2.egg-info/
+-rw-rw-rw-   0        0        0      556 2023-07-18 12:09:10.000000 dms-influx2-0.3.5/dms_influx2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-18 12:09:10.000000 dms-influx2-0.3.5/dms_influx2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 12:09:10.000000 dms-influx2-0.3.5/dms_influx2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-07-18 12:09:10.000000 dms-influx2-0.3.5/dms_influx2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 12:09:10.000000 dms-influx2-0.3.5/dms_influx2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 12:09:10.927886 dms-influx2-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     3023 2023-07-18 12:08:45.000000 dms-influx2-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:09:10.926219 dms-influx2-0.3.5/tests/
+-rw-rw-rw-   0        0        0     1882 2023-07-03 09:02:50.000000 dms-influx2-0.3.5/tests/test_auth.py
+-rw-rw-rw-   0        0        0     4632 2023-07-03 09:02:50.000000 dms-influx2-0.3.5/tests/test_buckets.py
+-rw-rw-rw-   0        0        0     2018 2023-07-03 09:11:49.000000 dms-influx2-0.3.5/tests/test_copy-values.py
+-rw-rw-rw-   0        0        0    17628 2023-07-18 10:52:13.000000 dms-influx2-0.3.5/tests/test_data.py
```

### Comparing `dms-influx2-0.3.4/PKG-INFO` & `dms-influx2-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.4/dms_influx2/authorizations.py` & `dms-influx2-0.3.5/dms_influx2/authorizations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/buckets.py` & `dms-influx2-0.3.5/dms_influx2/buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/checks.py` & `dms-influx2-0.3.5/dms_influx2/checks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/decorators.py` & `dms-influx2-0.3.5/dms_influx2/decorators.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/delete.py` & `dms-influx2-0.3.5/dms_influx2/delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import itertools
+import logging
 from datetime import datetime, timedelta
 from typing import Union
 
 from dateutil.parser import parse
 from influxdb_client import DeleteApi
 
 from dms_influx2.utils import timestamp_to_influx_string
 
+logger = logging.getLogger(__name__)
+
 
 class Delete(DeleteApi):
     def __init__(self, client):
         self.org = client.org
         self.time_offset = client.time_offset
         self.query_str = client.query_str
         super().__init__(client)
@@ -19,15 +22,15 @@
                     bucket,
                     measurements=None,
                     device_ids=None,
                     descriptions=None,
                     org: str = None,
                     time_range: str = None,
                     time_from: Union[str, datetime] = None,
-                    time_to:  Union[str, datetime] = None) -> dict:
+                    time_to: Union[str, datetime] = None) -> dict:
 
         # TODO: add time_range
         if time_range is not None:
             pass
 
         if org is None:
             org = self.org
@@ -67,8 +70,9 @@
         # Filter empty lists and find all combinations for predicates, execute all queries
         predicates = list(filter(None, predicates))
         predicates = [predicate for predicate in itertools.product(*predicates)]
         predicates = [" and ".join(i for i in predicate) for predicate in predicates]
         predicates = list(dict.fromkeys(predicates))
         for predicate in predicates:
             self.delete(start=parse(start), stop=parse(stop), predicate=predicate, bucket=bucket, org=org)
+            logger.debug(f"Delete data {parse(start)}->{parse(stop)} from bucket: {bucket}, predicate: {predicate}")
         return {"start": start, "stop": stop, "predicates": predicates}
```

### Comparing `dms-influx2-0.3.4/dms_influx2/dtv_files.py` & `dms-influx2-0.3.5/dms_influx2/dtv_files.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/lib.py` & `dms-influx2-0.3.5/dms_influx2/lib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import math
-from typing import List, Union
+from time import sleep, time
+from typing import List, Union, Literal
 
 from ciso8601 import parse_datetime
 from dateutil.parser import parse
 from influxdb_client import InfluxDBClient, Point
 from datetime import datetime, timedelta
 from influxdb_client.client.flux_table import FluxTable
 from influxdb_client.client.write_api import WriteOptions
@@ -513,99 +514,268 @@
             "measurement": device_id.split('.')[0],
             "device_id": device_id,
             "values": data['values'],
             "unit": data['unit']
         }
         self.save_data(bucket=bucket, data=data_write)
 
+    def _get_time_from_aggregate_window(self,
+                                        time_window: str,
+                                        dt: datetime = datetime.utcnow(),
+                                        operator: Literal['plus', 'minus'] = 'minus') -> datetime:
+        window_type = time_window[-1]
+        window_number = int(time_window[0:-1])
+        if dt is None:
+            dt = datetime.utcnow()
+        if window_type == 'y':
+            window_type = 'd'
+            window_number = window_number * 365
+        d = {
+            "s": "seconds",
+            "m": "minutes",
+            "h": "hours",
+            "d": "days"
+        }
+        if operator == 'plus':
+            return dt + timedelta(**{d[window_type]: window_number})
+        if operator == 'minus':
+            return dt - timedelta(**{d[window_type]: window_number})
+
     def down_sample(self,
                     bucket: str,
                     aggregate_window: str,
                     measurement: str = None,
+                    device_id: str = None,
                     time_from: Union[str, datetime] = None,
                     time_to: Union[str, datetime] = None,
                     older_than: str = None,
-                    decimal_places: int = None):
+                    decimal_places: int = None,
+                    use_utc: bool = False,
+                    to_int: bool = False):
+
+        # TODO what about 55.mio and dates with 1970
+
         if time_from is None and time_to is None and older_than is None:
             raise ValueError("Params (`time_from`, `time_to`, `older_than`) must not all be None")
 
         if type(time_from) == str:
             parse(time_from)
         if type(time_to) == str:
             parse(time_to)
 
         if decimal_places is None:
             decimal_places = 3
 
+        if use_utc is None:
+            use_utc = False
+
         if older_than is not None:
-            window_type = older_than[-1]
-            window_number = int(older_than[0:-1])
-            dt = localize_dt(datetime.utcnow())
-            if window_type == 'y':
-                window_type = 'd'
-                window_number = window_number * 365
-            d = {
-                "s": "seconds",
-                "m": "minutes",
-                "h": "hours",
-                "d": "days"
-            }
-            time_to = dt - timedelta(**{d[window_type]: window_number})
+            if use_utc:
+                dt = datetime.utcnow()
+            else:
+                dt = localize_dt(datetime.utcnow())
+            time_to = self._get_time_from_aggregate_window(time_window=older_than,
+                                                           dt=dt,
+                                                           operator='minus')
             time_from = None
 
         if time_from is not None:
             start = timestamp_to_influx_string(time_from)
         else:
-            start = '-100y'
+            start = timestamp_to_influx_string(datetime(1980, 1, 1, 0, 0, 0))
 
         if time_to is not None:
             stop = timestamp_to_influx_string(time_to)
         else:
-            stop = timestamp_to_influx_string(localize_dt(datetime.utcnow()))
+            if use_utc:
+                stop = timestamp_to_influx_string(datetime.utcnow())
+            else:
+                stop = timestamp_to_influx_string(localize_dt(datetime.utcnow()))
 
         # Erase bucket every each time for this operation
         downsampled_bucket = self.downsample_temp_bucket
         if self.buckets_api().bucket_exists(bucket_name=downsampled_bucket):
             self.buckets_api().delete_bucket_by_name(bucket_name=downsampled_bucket)
         self.buckets_api().create_bucket(bucket_name=downsampled_bucket)
 
         decimal_places_number = math.pow(10, decimal_places)
 
+        query_str = 'import "math"'
+        query_str += f'''\n\tfrom(bucket:"{bucket}") |> range(start: {start}, stop: {stop})'''
         if measurement is not None:
-            query = f'''
-                import "math"
-                from(bucket: "{bucket}") |> range(start: {start}, stop: {stop})
-                    |> filter(fn: (r) => r["_measurement"] == "{measurement}")
-                    |> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)
-                    |> map(
-                        fn: (r) =>
-                        ({{r with _value: (math.round(x: r._value * {decimal_places_number}) / {decimal_places_number}),}}),
-                    )
-                    |> to(bucket: "{downsampled_bucket}", org: "{self.org}")
-            '''
-        else:
-            query = f'''
-                from(bucket: "{bucket}") |> range(start: {start}, stop: {stop})
-                    |> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)
-                    |> map(
-                        fn: (r) =>
-                        ({{r with _value: (math.round(x: r._value * {decimal_places_number}) / {decimal_places_number}),}}),
-                    )
-                    |> to(bucket: "{downsampled_bucket}", org: "{self.org}")
-            '''
-        self.query_api().query(query=query)
+            query_str += f'''\n\t|> filter(fn: (r) => r["_measurement"] == "{measurement}")'''
+        if device_id is not None:
+            query_str += f'''\n\t|> filter(fn: (r) => r["device_id"] == "{device_id}")'''
+        query_str += f'''\n\t|> filter(fn: (r) => r["_value"] != 55000000)'''
+        query_str += f'''\n\t|> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)'''
+        query_str += f'''\n\t|> map(
+                            fn: (r) =>
+                            ({{r with _value: (math.round(x: r._value * {decimal_places_number}) / {decimal_places_number}),}}),
+                        )'''
+        if to_int:
+            query_str += f'''\n\t|> toInt()'''
+        query_str += f'''\n\t|> to(bucket: "{downsampled_bucket}", org: "{self.org}")'''
+
+        self.query_api().query(query=query_str)
 
         if measurement:
-            predicates = self.delete_api().delete_data(bucket=bucket,
-                                                       time_from=time_from,
-                                                       time_to=time_to,
-                                                       measurements=[measurement])
+            if device_id is None:
+                predicates = self.delete_api().delete_data(bucket=bucket,
+                                                           time_from=time_from,
+                                                           time_to=time_to,
+                                                           measurements=[measurement])
+            else:
+                predicates = self.delete_api().delete_data(bucket=bucket,
+                                                           time_from=time_from,
+                                                           time_to=time_to,
+                                                           device_ids=[device_id],
+                                                           measurements=[measurement])
+
         else:
             predicates = self.delete_api().delete_data(bucket=bucket,
                                                        time_from=time_from,
                                                        time_to=time_to)
 
         query = f'''
             from(bucket: "{downsampled_bucket}") |> range(start: -100y)
                 |> to(bucket: "{bucket}", org: "{self.org}")
         '''
         self.query_api().query(query=query)
+
+    def __get_query_telegraf_fields(self,
+                                    bucket: str,
+                                    measurement: str,
+                                    start: str,
+                                    stop: str,
+                                    aggregate_window: str,
+                                    fields: List[str],
+                                    to_int: bool = False):
+
+        query = 'import "math"'
+        query += f'''\n\tfrom(bucket:"{bucket}") |> range(start: {start}, stop: {stop})'''
+        query += f'''\n\t|> filter(fn: (r) => r["_measurement"] == "{measurement}")'''
+        if fields is not None:
+            first_field = fields[0]
+            query += f'''\n\t|> filter(fn: (r) => r["_field"] == "{first_field}"'''
+            if len(fields) >= 1:
+                for field in fields[1:]:
+                    query += f''' or r["_field"] == "{field}"'''
+            query += f')'
+        query += f'''\n\t|> aggregateWindow(every: {aggregate_window}, fn: mean, createEmpty: false)'''
+        if to_int:
+            query += f'''\n\t|> toInt()'''
+        query += f'''\n\t|> to(bucket: "{self.downsample_temp_bucket}", org: "{self.org}")'''
+
+        return query
+
+    def _downsample_telegraf_fields(self,
+                                    bucket: str,
+                                    measurement: str,
+                                    aggregate_window: str = '1h',
+                                    older_than: str = '30d',
+                                    normal_fields: List[str] = None,
+                                    to_int_fields: List[str] = None):
+
+        if measurement is None:
+            raise ValueError('Invalid value for argument `measurement`, cannot be None')
+
+        time_to = self._get_time_from_aggregate_window(time_window=older_than,
+                                                       dt=datetime.utcnow(),
+                                                       operator='minus')
+        time_from = None
+
+        # Erase bucket every each time for this operation
+        downsampled_bucket = self.downsample_temp_bucket
+        if self.buckets_api().bucket_exists(bucket_name=downsampled_bucket):
+            self.buckets_api().delete_bucket_by_name(bucket_name=downsampled_bucket)
+        self.buckets_api().create_bucket(bucket_name=downsampled_bucket)
+
+        start = timestamp_to_influx_string(datetime(1980, 1, 1, 0, 0))
+        stop = timestamp_to_influx_string(time_to)
+
+        if normal_fields is not None:
+            query_normal_fields = self.__get_query_telegraf_fields(bucket=bucket,
+                                                                   measurement=measurement,
+                                                                   aggregate_window=aggregate_window,
+                                                                   start=start,
+                                                                   stop=stop,
+                                                                   fields=normal_fields,
+                                                                   to_int=False)
+            self.query_api().query(query=query_normal_fields)
+
+        if to_int_fields is not None:
+            query_to_int_fields = self.__get_query_telegraf_fields(bucket=bucket,
+                                                                   measurement=measurement,
+                                                                   aggregate_window=aggregate_window,
+                                                                   start=start,
+                                                                   stop=stop,
+                                                                   fields=to_int_fields,
+                                                                   to_int=True)
+            self.query_api().query(query=query_to_int_fields)
+
+        self.delete_api().delete_data(bucket=bucket,
+                                      measurements=[measurement],
+                                      time_to=time_to)
+
+        query_copy_to_bucket = f'''
+            from(bucket: "{downsampled_bucket}") |> range(start: -100y)
+                |> to(bucket: "{bucket}", org: "{self.org}")
+        '''
+        self.query_api().query(query=query_copy_to_bucket)
+
+    def downsample_telegraf_stats(self,
+                                  bucket: str,
+                                  aggregate_window: str = '1h',
+                                  older_than: str = '30d'):
+        """
+        cpu-fields: usage_guest, usage_guest_nice, usage_idle, usage_iowait, usage_irq, usage_nice, usage_softirq,
+            usage_steal, usage_system, usage_user
+        disk-fields: free, inodes_free, inodes_total, inodes_used, total, used, used_percent
+        kernel-fields: boot_time, context_switches, entropy_avail, interrupts, processes_forked
+        mem-fields: active, available, available_percent, buffered, cached, commit_limit, committed_as, dirty, free,
+            high_free, high_total, huge_page_size, huge_pages_free, huge_pages_total, inactive, low_free, low_total,
+            mapped, page_tables, shared, slab, sreclaimable, sunreclaim, swap_cached, swap_free, swap_total, total,
+            used, used_percent, vmalloc_chunk, vmalloc_total, vmalloc_used, write_back, write_back_tmp
+        """
+        if older_than is None:
+            older_than = '30d'
+        items = [
+            {
+                "measurement": "cpu",
+                "normal_fields": ["usage_guest", "usage_guest_nice", "usage_idle", "usage_iowait", "usage_irq",
+                                  "usage_nice", "usage_softirq", "usage_steal", "usage_system", "usage_user"],
+                "to_int_fields": None
+            },
+            {
+                "measurement": "disk",
+                "normal_fields": ["used_percent"],
+                "to_int_fields": ['free', 'inodes_free', 'inodes_total', 'inodes_used', "total", 'used']
+            },
+            {
+                "measurement": "kernel",
+                "normal_fields": None,
+                "to_int_fields": ['boot_time', 'context_switches', 'entropy_avail', 'interrupts', 'processes_forked']
+            },
+            {
+                "measurement": "mem",
+                "normal_fields": ['available_percent', 'used_percent'],
+                "to_int_fields": ["active", 'available', 'buffered', 'cached', 'commit_limit', 'committed_as', 'dirty',
+                                  'free', 'high_free', 'high_total', 'huge_page_size', 'huge_pages_free',
+                                  'huge_pages_total', 'inactive', 'low_free', 'low_total', 'mapped', 'page_tables',
+                                  'shared', 'slab', 'sreclaimable', 'sunreclaim', 'swap_cached', 'swap_free',
+                                  'swap_total', 'total', 'used', 'vmalloc_chunk', 'vmalloc_total', 'vmalloc_used',
+                                  'write_back', 'write_back_tmp']
+            }
+        ]
+
+        start = time()
+        for item in items:
+            try:
+                self._downsample_telegraf_fields(bucket=bucket,
+                                                 aggregate_window=aggregate_window,
+                                                 measurement=item['measurement'],
+                                                 older_than=older_than,
+                                                 normal_fields=item['normal_fields'],
+                                                 to_int_fields=item['to_int_fields'])
+            except Exception as e:
+                logger.error(f'Cannot downsample telegraf stats for: {item["measurement"]}, e:{e}')
+        logger.info(f'Downsample complete, bucket: {bucket}, type: telegraf_stats, runtime:{round(time() - start, 2)}s')
```

### Comparing `dms-influx2-0.3.4/dms_influx2/notifications.py` & `dms-influx2-0.3.5/dms_influx2/notifications.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/organisations.py` & `dms-influx2-0.3.5/dms_influx2/organisations.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/query.py` & `dms-influx2-0.3.5/dms_influx2/query.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/tasks.py` & `dms-influx2-0.3.5/dms_influx2/tasks.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2/utils.py` & `dms-influx2-0.3.5/dms_influx2/utils.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/dms_influx2.egg-info/PKG-INFO` & `dms-influx2-0.3.5/dms_influx2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dms-influx2
-Version: 0.3.4
+Version: 0.3.5
 Summary: Library to connect and retrieve data from DMS influxdb
 Home-page: https://github.com/belingarb/dms-influx2
 Author: Bozidar Belingar
 Author-email: bozidar.belingar@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dms-influx2-0.3.4/dms_influx2.egg-info/SOURCES.txt` & `dms-influx2-0.3.5/dms_influx2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/setup.py` & `dms-influx2-0.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'dms-influx2'
 DESCRIPTION = 'Library to connect and retrieve data from DMS influxdb'
 URL = 'https://github.com/belingarb/dms-influx2'
 EMAIL = 'bozidar.belingar@gmail.com'
 AUTHOR = 'Bozidar Belingar'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.3.4'
+VERSION = '0.3.5'
 
 # Get required packages from requirements.txt file
 with open('requirements/base.txt') as f:
     REQUIRED = f.read().splitlines()
 
 dir_path = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `dms-influx2-0.3.4/tests/test_auth.py` & `dms-influx2-0.3.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/tests/test_buckets.py` & `dms-influx2-0.3.5/tests/test_buckets.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/tests/test_copy-values.py` & `dms-influx2-0.3.5/tests/test_copy-values.py`

 * *Files identical despite different names*

### Comparing `dms-influx2-0.3.4/tests/test_data.py` & `dms-influx2-0.3.5/tests/test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -290,83 +290,99 @@
                                           device_id=test_data['device_id'],
                                           time_range='all')
     assert data == {}
 
 
 def test_downsample_data():
     bucket = 'downsample_test'
-    values = [(datetime.now() - timedelta(hours=i), i) for i in range(5, 100)]
-    test_data = {
-        "measurement": 'downsample',
-        "device_id": 'downsample.12',
-        "values": values
-
-    }
+    values = [(str(datetime.now() - timedelta(hours=i)), i) for i in range(5, 100)]
+    test_data = [
+        {
+            "measurement": 'downsample',
+            "device_id": 'downsample.12',
+            "values": values
+        },
+        {
+            "measurement": 'downsample',
+            "device_id": 'downsample.123',
+            "values": values
+        }
+    ]
     CLIENT.save_data(bucket=bucket, data=test_data)
     '''Test time_from and time_to'''
-    time_from = test_data['values'][-1][0] - timedelta(seconds=1)
-    time_to = test_data['values'][0][0] + timedelta(seconds=1)
+    time_from = parse(test_data[0]['values'][-1][0]) - timedelta(seconds=1)
+    time_to = parse(test_data[0]['values'][0][0]) + timedelta(seconds=1)
     aggregate_window = '30m'
     aggregated_data = CLIENT.get_data_from_device_id(bucket=bucket,
-                                                     measurement=test_data['measurement'],
-                                                     device_id=test_data['device_id'],
+                                                     measurement=test_data[0]['measurement'],
+                                                     device_id=test_data[0]['device_id'],
                                                      time_from=time_from,
                                                      time_to=time_to,
                                                      aggregate_window=aggregate_window)
     # Perform a downsample and check if all data are downsampled within bucket
     CLIENT.down_sample(bucket=bucket,
-                       measurement=test_data['measurement'],
+                       measurement=test_data[0]['measurement'],
+                       device_id=test_data[0]['device_id'],
                        aggregate_window=aggregate_window,
                        time_from=time_from,
                        time_to=time_to)
     data_in_downsampled_bucket = CLIENT.get_data_from_device_id(bucket=CLIENT.downsample_temp_bucket,
-                                                                measurement=test_data['measurement'],
-                                                                device_id=test_data['device_id'],
+                                                                measurement=test_data[0]['measurement'],
+                                                                device_id=test_data[0]['device_id'],
                                                                 time_range='all')
     assert aggregated_data['values'] == data_in_downsampled_bucket['values']
     # New data in this bucket must be equal to aggregated data
     new_data = CLIENT.get_data_from_device_id(bucket=bucket,
-                                              measurement=test_data['measurement'],
-                                              device_id=test_data['device_id'],
+                                              measurement=test_data[0]['measurement'],
+                                              device_id=test_data[0]['device_id'],
                                               time_from=time_from - timedelta(seconds=1),
                                               time_to=time_to + timedelta(seconds=1))
     assert aggregated_data['values'] == new_data['values']
+    # New data for second device must be the same as origin
+    new_data_second = CLIENT.get_data_from_device_id(bucket=bucket,
+                                                     measurement=test_data[-1]['measurement'],
+                                                     device_id=test_data[-1]['device_id'],
+                                                     time_range='all')
+    assert test_data[-1]['values'] == new_data_second['values']
 
     '''Test2: test older_than param'''
     bucket = 'downsample_test1'
     older_than = '1d'
     aggregate_window = '4h'
     CLIENT.save_data(bucket=bucket, data=test_data)
     time_from = datetime(1970, 1, 1, 12, 0, 0)
     time_to = datetime.now() - timedelta(days=1) + timedelta(seconds=1)
     aggregated_data = CLIENT.get_data_from_device_id(bucket=bucket,
-                                                     measurement=test_data['measurement'],
-                                                     device_id=test_data['device_id'],
+                                                     measurement=test_data[0]['measurement'],
+                                                     device_id=test_data[0]['device_id'],
                                                      time_from=time_from,
                                                      time_to=time_to,
                                                      aggregate_window=aggregate_window)
     # Perform a downsample and check if all data are downsampled within bucket
     CLIENT.down_sample(bucket=bucket,
-                       measurement=test_data['measurement'],
+                       measurement=test_data[0]['measurement'],
+                       device_id=test_data[0]['device_id'],
                        aggregate_window=aggregate_window,
                        older_than=older_than)
     data_in_downsampled_bucket = CLIENT.get_data_from_device_id(bucket=CLIENT.downsample_temp_bucket,
-                                                                measurement=test_data['measurement'],
-                                                                device_id=test_data['device_id'],
+                                                                measurement=test_data[0]['measurement'],
+                                                                device_id=test_data[0]['device_id'],
                                                                 time_range='all')
     assert len(aggregated_data['values']) == len(data_in_downsampled_bucket['values'])
     # Old data must remain the same
     old_data = CLIENT.get_data_from_device_id(bucket=bucket,
-                                              measurement=test_data['measurement'],
-                                              device_id=test_data['device_id'],
+                                              measurement=test_data[0]['measurement'],
+                                              device_id=test_data[0]['device_id'],
                                               time_from=time_to)
     old_data_values = []
     for value in values:
-        if value[0] > (time_to - timedelta(seconds=1)):
+        if parse(value[0]) > (time_to - timedelta(seconds=1)):
             old_data_values.append((str(value[0]), value[1]))
     assert old_data_values == old_data['values']
     new_data = CLIENT.get_data_from_device_id(bucket=bucket,
-                                              measurement=test_data['measurement'],
-                                              device_id=test_data['device_id'],
+                                              measurement=test_data[0]['measurement'],
+                                              device_id=test_data[0]['device_id'],
                                               time_from=time_from,
                                               time_to=time_to)
     assert len(aggregated_data['values']) == len(new_data['values'])
+
+
```

