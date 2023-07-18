# Comparing `tmp/tap-mailchimp-1.2.0.tar.gz` & `tmp/tap-mailchimp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-mailchimp-1.2.0.tar", last modified: Thu Jun  8 13:21:27 2023, max compression
+gzip compressed data, was "tap-mailchimp-1.2.1.tar", last modified: Tue Jul 18 07:31:39 2023, max compression
```

## Comparing `tap-mailchimp-1.2.0.tar` & `tap-mailchimp-1.2.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-12-12 10:22:04.000000 tap-mailchimp-1.2.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2856 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.965123 tap-mailchimp-1.2.0/tap_mailchimp/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-06-08 13:03:55.000000 tap-mailchimp-1.2.0/tap_mailchimp/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4389 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/tap_mailchimp/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1701 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.969123 tap-mailchimp-1.2.0/tap_mailchimp/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6687 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/automations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8473 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2587 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segment_members.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2023-01-04 05:38:09.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/lists.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/reports_email_activity.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      800 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.0/tap_mailchimp/schemas/unsubscribes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21929 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.0/tap_mailchimp/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-08 13:21:27.965123 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      700 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-06-08 13:21:27.000000 tap-mailchimp-1.2.0/tap_mailchimp.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 07:31:39.578882 tap-mailchimp-1.2.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-07-18 07:31:39.578882 tap-mailchimp-1.2.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2856 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-18 07:31:39.578882 tap-mailchimp-1.2.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2023-07-18 07:23:27.000000 tap-mailchimp-1.2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 07:31:39.578882 tap-mailchimp-1.2.1/tap_mailchimp/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1097 2023-06-08 13:03:55.000000 tap-mailchimp-1.2.1/tap_mailchimp/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4501 2023-07-18 07:23:27.000000 tap-mailchimp-1.2.1/tap_mailchimp/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1701 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schema.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 07:31:39.578882 tap-mailchimp-1.2.1/tap_mailchimp/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6687 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/automations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8473 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/list_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2587 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/list_segment_members.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1807 2023-01-04 05:38:09.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/list_segments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5360 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/lists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/reports_email_activity.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      800 2023-05-23 19:31:42.000000 tap-mailchimp-1.2.1/tap_mailchimp/schemas/unsubscribes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    21929 2023-06-08 13:03:43.000000 tap-mailchimp-1.2.1/tap_mailchimp/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-18 07:31:39.578882 tap-mailchimp-1.2.1/tap_mailchimp.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      299 2023-07-18 07:31:39.000000 tap-mailchimp-1.2.1/tap_mailchimp.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      692 2023-07-18 07:31:39.000000 tap-mailchimp-1.2.1/tap_mailchimp.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-18 07:31:39.000000 tap-mailchimp-1.2.1/tap_mailchimp.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-07-18 07:31:39.000000 tap-mailchimp-1.2.1/tap_mailchimp.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       86 2023-07-18 07:31:39.000000 tap-mailchimp-1.2.1/tap_mailchimp.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-07-18 07:31:39.000000 tap-mailchimp-1.2.1/tap_mailchimp.egg-info/top_level.txt
```

### Comparing `tap-mailchimp-1.2.0/README.md` & `tap-mailchimp-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/setup.py` & `tap-mailchimp-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-mailchimp',
-      version='1.2.0',
+      version='1.2.1',
       description='Singer.io tap for extracting data from the Mailchimp API',
       author='Stitch',
       url='https://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_mailchimp'],
       install_requires=[
           'backoff==1.8.0',
```

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/__init__.py` & `tap-mailchimp-1.2.1/tap_mailchimp/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/client.py` & `tap-mailchimp-1.2.1/tap_mailchimp/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,18 +21,20 @@
         self.__api_key = config.get('api_key')
         self.__session = requests.Session()
         self.__base_url = None
         self.page_size = int(config.get('page_size', '1000'))
 
         # performs date-window calculation for fetching campaigns
         try:
-            date_window_duration = int(config.get('email_activity_date_window', 0))
+            date_window_duration = int(config.get('email_activity_date_window') or 0)
             self.adjusted_start_date = False if date_window_duration == 0 else \
                 (singer.utils.now().date() - singer.utils.datetime.timedelta(days = date_window_duration))
-        except ValueError:
+        # Raises TypeError for None / Null Value
+        # Raises ValueError for "" / bool value
+        except (ValueError, TypeError):
             LOGGER.info("Invalid Value: %s, for date windowing", config.get('email_activity_date_window', 0))
             LOGGER.critical("Date windowing disabled")
             self.adjusted_start_date = False
         # Set request timeout to config param `request_timeout` value.
         # If value is 0,"0","" or not passed then it set default to 300 seconds.
         config_request_timeout = config.get('request_timeout')
         if config_request_timeout and float(config_request_timeout):
```

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/discover.py` & `tap-mailchimp-1.2.1/tap_mailchimp/discover.py`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schema.py` & `tap-mailchimp-1.2.1/tap_mailchimp/schema.py`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/automations.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/automations.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/campaigns.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_members.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/list_members.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segment_members.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/list_segment_members.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/list_segments.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/list_segments.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/lists.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/reports_email_activity.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/reports_email_activity.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/schemas/unsubscribes.json` & `tap-mailchimp-1.2.1/tap_mailchimp/schemas/unsubscribes.json`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp/sync.py` & `tap-mailchimp-1.2.1/tap_mailchimp/sync.py`

 * *Files identical despite different names*

### Comparing `tap-mailchimp-1.2.0/tap_mailchimp.egg-info/SOURCES.txt` & `tap-mailchimp-1.2.1/tap_mailchimp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 tap_mailchimp/__init__.py
 tap_mailchimp/client.py
 tap_mailchimp/discover.py
 tap_mailchimp/schema.py
 tap_mailchimp/sync.py
```

