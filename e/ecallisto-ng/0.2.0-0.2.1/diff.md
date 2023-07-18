# Comparing `tmp/ecallisto_ng-0.2.0.tar.gz` & `tmp/ecallisto_ng-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecallisto_ng-0.2.0.tar", last modified: Mon Jul 17 12:16:37 2023, max compression
+gzip compressed data, was "ecallisto_ng-0.2.1.tar", last modified: Tue Jul 18 10:10:03 2023, max compression
```

## Comparing `ecallisto_ng-0.2.0.tar` & `ecallisto_ng-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.0/LICENSE
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.0/README.md
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-17 12:16:23.000000 ecallisto_ng-0.2.0/pyproject.toml
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/setup.cfg
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/src/
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/src/ecallisto_ng/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/__init__.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/src/ecallisto_ng/data_fetching/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/data_fetching/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7505 2023-07-17 12:16:13.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/data_fetching/get_data.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2006 2023-07-13 17:59:20.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/data_fetching/get_information.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/src/ecallisto_ng/data_processing/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/data_processing/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/data_processing/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/src/ecallisto_ng/plotting/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/plotting/__init__.py
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.2.0/src/ecallisto_ng/plotting/utils.py
-drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-17 12:16:37.515696 ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-17 12:16:37.000000 ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/PKG-INFO
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-17 12:16:37.000000 ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/SOURCES.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-17 12:16:37.000000 ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/dependency_links.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-17 12:16:37.000000 ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/requires.txt
--rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-17 12:16:37.000000 ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/top_level.txt
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     1083 2023-07-06 16:13:05.000000 ecallisto_ng-0.2.1/LICENSE
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3028 2023-07-17 09:45:19.000000 ecallisto_ng-0.2.1/README.md
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      858 2023-07-18 10:09:00.000000 ecallisto_ng-0.2.1/pyproject.toml
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       38 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/setup.cfg
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-06 17:35:07.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/__init__.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:51.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     7501 2023-07-17 13:11:37.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_data.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3398 2023-07-18 10:05:42.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_information.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:39:54.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     5256 2023-07-11 08:45:15.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        0 2023-07-13 16:40:01.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/__init__.py
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     2425 2023-07-10 17:56:33.000000 ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/utils.py
+drwxr-xr-x   0 kenfus    (1000) kenfus    (1000)        0 2023-07-18 10:10:03.848899 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)     3608 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/PKG-INFO
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      556 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)        1 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)      129 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/requires.txt
+-rw-r--r--   0 kenfus    (1000) kenfus    (1000)       13 2023-07-18 10:10:03.000000 ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/top_level.txt
```

### Comparing `ecallisto_ng-0.2.0/LICENSE` & `ecallisto_ng-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.0/PKG-INFO` & `ecallisto_ng-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto_ng
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.0/README.md` & `ecallisto_ng-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.0/pyproject.toml` & `ecallisto_ng-0.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ecallisto_ng"
-version = "0.2.0"
+version = "0.2.1"
 authors = [{name = "Vincenzo Timmel", email = "vincenzo.timmel@fhnw.ch"}]
 description = "A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API."
 readme = "README.md"
 
 requires-python = ">=3.9"
 
 classifiers = [
```

### Comparing `ecallisto_ng-0.2.0/src/ecallisto_ng/data_fetching/get_data.py` & `ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     # Create file path
     file_path = os.path.join(data_folder, f"{instrument_name}_{start_datetime}_{end_datetime}_{timebucket}_{agg_function}.parquet")
     os.makedirs(data_folder, exist_ok=True)
     if os.path.exists(file_path):
         print(f"Reading data from {file_path}")
         return pd.read_parquet(file_path)
-    
+
     # Send the request to the API
     response = requests.post(BASE_URL + "/api/data", json=data, timeout=180)
 
     # Check if the request was successful
     if response.status_code == 200:
         if verbose:
             print("Data retrieval started successfully. Waiting for file to be ready...")
```

### Comparing `ecallisto_ng-0.2.0/src/ecallisto_ng/data_fetching/get_information.py` & `ecallisto_ng-0.2.1/src/ecallisto_ng/data_fetching/get_information.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,7 +60,47 @@
     if response.status_code == 200:
         table_names = response.json()['table_names']
         if verbose:
             print(f"Received table names: {table_names}")
         return table_names
     else:
         raise ValueError(f"Error getting table names from API: {response.text}")
+
+def check_table_data_availability(instrument_name, start_datetime, end_datetime, verbose=False, **kwargs):
+    """
+    Check if a table has data between the specified dates using the eCallisto API.
+
+    Parameters
+    ----------
+    table_name : str
+        The name of the table to check.
+    start_datetime : str
+        The start datetime of the data availability check.
+    end_datetime : str
+        The end datetime of the data availability check.
+    verbose : bool
+        Whether to print out the response from the API.
+
+    Returns
+    -------
+    bool
+        True if the table has data between the specified dates, False otherwise.
+    """
+    data = {
+        "instrument_name": instrument_name,
+        "start_datetime": start_datetime,
+        "end_datetime": end_datetime,
+    }
+
+    assert pd.to_datetime(start_datetime) <= pd.to_datetime(end_datetime), (
+        f"start_datetime ({start_datetime}) must be before end_datetime ({end_datetime})"
+    )
+
+    response = requests.post(BASE_URL + "/api/table_data_check", json=data)
+
+    if response.status_code == 200:
+        has_data = response.json()['has_data']
+        if verbose:
+            print(f"Table '{instrument_name}' has data between {start_datetime} and {end_datetime}: {has_data}")
+        return has_data
+    else:
+        raise ValueError(f"Error checking table data availability from API: {response.text}")
```

### Comparing `ecallisto_ng-0.2.0/src/ecallisto_ng/data_processing/utils.py` & `ecallisto_ng-0.2.1/src/ecallisto_ng/data_processing/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.0/src/ecallisto_ng/plotting/utils.py` & `ecallisto_ng-0.2.1/src/ecallisto_ng/plotting/utils.py`

 * *Files identical despite different names*

### Comparing `ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/PKG-INFO` & `ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecallisto-ng
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package for the fetching (and some processing) of eCallisto data via the eCallisto API.
 Author-email: Vincenzo Timmel <vincenzo.timmel@fhnw.ch>
 Project-URL: Homepage, https://github.com/i4Ds/ecallisto_ng
 Project-URL: Bug Tracker, https://github.com/i4Ds/ecallisto_ng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecallisto_ng-0.2.0/src/ecallisto_ng.egg-info/SOURCES.txt` & `ecallisto_ng-0.2.1/src/ecallisto_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

