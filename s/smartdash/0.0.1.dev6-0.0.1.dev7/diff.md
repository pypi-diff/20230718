# Comparing `tmp/smartdash-0.0.1.dev6.tar.gz` & `tmp/smartdash-0.0.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdash-0.0.1.dev6.tar", last modified: Tue May 30 10:25:46 2023, max compression
+gzip compressed data, was "smartdash-0.0.1.dev7.tar", last modified: Tue Jul 18 08:05:17 2023, max compression
```

## Comparing `smartdash-0.0.1.dev6.tar` & `smartdash-0.0.1.dev7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/smartdash/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/dash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-30 10:25:36.000000 smartdash-0.0.1.dev6/smartdash/smartdash_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:25:46.513612 smartdash-0.0.1.dev6/smartdash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 10:25:46.000000 smartdash-0.0.1.dev6/smartdash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:05:17.755785 smartdash-0.0.1.dev7/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 08:05:17.755785 smartdash-0.0.1.dev7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-18 08:05:06.000000 smartdash-0.0.1.dev7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:05:17.755785 smartdash-0.0.1.dev7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-18 08:05:06.000000 smartdash-0.0.1.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:05:17.755785 smartdash-0.0.1.dev7/smartdash/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-18 08:05:06.000000 smartdash-0.0.1.dev7/smartdash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 08:05:06.000000 smartdash-0.0.1.dev7/smartdash/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-07-18 08:05:06.000000 smartdash-0.0.1.dev7/smartdash/dash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-18 08:05:06.000000 smartdash-0.0.1.dev7/smartdash/smartdash_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:05:17.755785 smartdash-0.0.1.dev7/smartdash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 08:05:17.000000 smartdash-0.0.1.dev7/smartdash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-18 08:05:17.000000 smartdash-0.0.1.dev7/smartdash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:05:17.000000 smartdash-0.0.1.dev7/smartdash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 08:05:17.000000 smartdash-0.0.1.dev7/smartdash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 08:05:17.000000 smartdash-0.0.1.dev7/smartdash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 08:05:17.000000 smartdash-0.0.1.dev7/smartdash.egg-info/top_level.txt
```

### Comparing `smartdash-0.0.1.dev6/PKG-INFO` & `smartdash-0.0.1.dev7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
-python logging client for SmartDash
+
+### Start SmartDash
+
+```
+# Start smartdash server
+smartdash --dash --server_url "http://localhost:8080" --port 6788 --save_dir ./
+
+# Start smartdash dashboard
+smartdash --dash --server_url "http://localhost:8080" --port 6788 --save_dir ./
+```
```

### Comparing `smartdash-0.0.1.dev6/setup.py` & `smartdash-0.0.1.dev7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = "smartdash"
 DESCRIPTION = "python logging client for SmartDash"
 URL = "https://github.com/notAI-tech/smartdash"
 EMAIL = "praneeth@bpraneeth.com"
 AUTHOR = "BEDAPUDI PRANEETH"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1.dev6"
+VERSION = "0.0.1.dev7"
 
 # What packages are required for this module to be executed?
 REQUIRED = ["requests", "liteindex", "streamlit", "plotly"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
```

### Comparing `smartdash-0.0.1.dev6/smartdash/__init__.py` & `smartdash-0.0.1.dev7/smartdash/__init__.py`

 * *Files identical despite different names*

### Comparing `smartdash-0.0.1.dev6/smartdash/dash.py` & `smartdash-0.0.1.dev7/smartdash/dash.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         app_name = st.sidebar.selectbox(
             "Select App",
             requests.get(f"{SERVER_URL}/app_names").json()["app_names"],
             index=0,
         )
         time_range = st.sidebar.selectbox(
             "Select Time Range",
-            ["8 hours", "12 hours", "Last day", "Last week"],
+            ["8 hours", "12 hours", "Last day", "Last week", "All time"],
             index=0,
         )
 
         long_running_range = st.sidebar.selectbox(
             "Highlight long running uids", ["1 hour", "30 min", "15 min"], index=0
         )
 
@@ -65,14 +65,15 @@
             "8 hours": 8,
             "12 hours": 12,
             "Last day": 24,
             "Last week": 168,
             "1 hour": 1,
             "15 min": 0.25,
             "30 min": 0.5,
+            "All time": 10000000,
         }
 
         long_running_n_hours = time_mapping[long_running_range]
         last_n_hours = time_mapping[time_range]
 
         data_by_uid, _ = fetch_dash_data(app_name, last_n_hours, long_running_n_hours)
```

### Comparing `smartdash-0.0.1.dev6/smartdash/smartdash_server.py` & `smartdash-0.0.1.dev7/smartdash/smartdash_server.py`

 * *Files identical despite different names*

### Comparing `smartdash-0.0.1.dev6/smartdash.egg-info/PKG-INFO` & `smartdash-0.0.1.dev7/smartdash.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: smartdash
-Version: 0.0.1.dev6
+Version: 0.0.1.dev7
 Summary: python logging client for SmartDash
 Home-page: https://github.com/notAI-tech/smartdash
 Author: BEDAPUDI PRANEETH
 Author-email: praneeth@bpraneeth.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
-python logging client for SmartDash
+
+### Start SmartDash
+
+```
+# Start smartdash server
+smartdash --dash --server_url "http://localhost:8080" --port 6788 --save_dir ./
+
+# Start smartdash dashboard
+smartdash --dash --server_url "http://localhost:8080" --port 6788 --save_dir ./
+```
```

