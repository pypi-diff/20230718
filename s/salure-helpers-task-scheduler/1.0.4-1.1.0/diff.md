# Comparing `tmp/salure_helpers_task_scheduler-1.0.4.tar.gz` & `tmp/salure_helpers_task_scheduler-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_task_scheduler-1.0.4.tar", last modified: Thu May 11 09:09:10 2023, max compression
+gzip compressed data, was "dist/salure_helpers_task_scheduler-1.1.0.tar", last modified: Tue Jul 18 07:47:51 2023, max compression
```

## Comparing `salure_helpers_task_scheduler-1.0.4.tar` & `salure_helpers_task_scheduler-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-11 09:08:57.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    38959 2023-05-11 09:08:57.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/task_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      414 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/salure_helpers_task_scheduler.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 09:09:10.000000 salure_helpers_task_scheduler-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      614 2023-05-11 09:08:57.000000 salure_helpers_task_scheduler-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-18 07:47:38.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39810 2023-07-18 07:47:38.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/task_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/salure_helpers_task_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 07:47:51.000000 salure_helpers_task_scheduler-1.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      614 2023-07-18 07:47:38.000000 salure_helpers_task_scheduler-1.1.0/setup.py
```

### Comparing `salure_helpers_task_scheduler-1.0.4/salure_helpers/task_scheduler/task_scheduler.py` & `salure_helpers_task_scheduler-1.1.0/salure_helpers/task_scheduler/task_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import sys
+import os
 import datetime
 import inspect
 import time
 import typing
+import pandas as pd
 from salure_helpers.mandrill import MailClient
 from salure_helpers.salure_functions import SalureFunctions
 from salure_helpers.salureconnect import SalureConnect
 from salure_helpers.mysql import MySQL
+from salure_helpers.elastic import Elastic
 import warnings
 import re
 
 
 class TaskScheduler(SalureConnect):
 
     def __init__(self, task_id=None, loglevel='INFO', email_after_errors=False):
@@ -214,63 +217,86 @@
             raise Exception(f'Variable with name \'{variable_name}\' does not exist')
         else:
             value = response[0][0]
             if value is None and default_value_if_temp_is_empty is True and len(response[0]) > 0:
                 value = response[0][1]
             return value
 
-    def write_execution_log(self, message: str, loglevel='INFO'):
+    def write_execution_log(self, message: str, loglevel='INFO', data: tuple[pd.DataFrame, pd.Series] = None):
         """
         Writes messages to the database. Give the message and the level of the log
         :param message: A string with a message for the log
         :param loglevel: You can choose between DEBUG, INFO, ERROR or CRITICAL (DEBUG is most granulated, CRITICAL the less)
+        :param data: Optional. Uploaded data by the interface that has to be logged in ElasticSearch
         :return: If the write to the database is successful or not
         """
         allowed_loglevels = ['DEBUG', 'INFO', 'ERROR', 'CRITICAL']
         if loglevel not in allowed_loglevels:
             raise Exception('You\'ve entered a not allowed loglevel. Choose one of: {}'.format(allowed_loglevels))
-        else:
-            # Get the linenumber from where the logline is executed. Get the stacktrace of this action, jump 1 file up and pick then the linenumber (second item)
-            linenumber = inspect.getouterframes(inspect.currentframe())[1][2]
-            # Write the logline to the database, depends on the chosen loglevel in the task
-            print('{} at line: {}'.format(message, linenumber))
-            # Remove quotes from message since these break the query
-            message = re.sub("[']", '', message)
-            timestamp = time.strftime("%Y-%m-%d %H:%M:%S")
-            information = {
+
+        if data is not None:
+            es = Elastic()
+
+            # If the data is a series, convert it to a dataframe
+            if isinstance(data, pd.Series):
+                data = pd.DataFrame(data).T
+
+            payload = {
                 'reload_id': self.run_id,
                 'task_id': self.task_id,
-                'log_level': loglevel,
-                'line_number': linenumber,
-                'message': message,
-                'created_at': timestamp
+                'customer_id': os.getenv('SALURECONNECT_CUSTOMER_NAME').lower().replace(' ', '_'),
+                'started_at': self.started_at.isoformat(),
+                'records': len(data),
+                'columns': len(data.columns),
+                'cells': len(data) * len(data.columns),
+                'data': data.to_csv(sep='|', index=False),
+                'loglevel': loglevel,
+                'message': message
             }
-            if self.loglevel == 'DEBUG':
-                # Count the errors
-                if loglevel == 'ERROR' or loglevel == 'CRITICAL':
-                    self.error_count += 1
-                return self.mysql.raw_query(
-                    "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
-                return self.mysql.update(table='task_execution_log',
-                                         columns=['reload_id', 'task_id', 'log_level', 'created_at', 'line_number', 'message'],
-                                         values=[self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message])
-            elif self.loglevel == 'INFO' and (loglevel == 'INFO' or loglevel == 'ERROR' or loglevel == 'CRITICAL'):
-                # Count the errors
-                if loglevel == 'ERROR' or loglevel == 'CRITICAL':
-                    self.error_count += 1
-                return self.mysql.raw_query(
-                    "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
-            elif self.loglevel == 'ERROR' and (loglevel == 'ERROR' or loglevel == 'CRITICAL'):
+
+            es.log_line(payload)
+
+        # Get the linenumber from where the logline is executed. Get the stacktrace of this action, jump 1 file up and pick then the linenumber (second item)
+        linenumber = inspect.getouterframes(inspect.currentframe())[1][2]
+        # Write the logline to the database, depends on the chosen loglevel in the task
+        print('{} at line: {}'.format(message, linenumber))
+        # Remove quotes from message since these break the query
+        message = re.sub("[']", '', message)
+        timestamp = time.strftime("%Y-%m-%d %H:%M:%S")
+        information = {
+            'reload_id': self.run_id,
+            'task_id': self.task_id,
+            'log_level': loglevel,
+            'line_number': linenumber,
+            'message': message,
+            'created_at': timestamp
+        }
+        if self.loglevel == 'DEBUG':
+            # Count the errors
+            if loglevel == 'ERROR' or loglevel == 'CRITICAL':
                 self.error_count += 1
-                return self.mysql.raw_query(
-                    "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
-            elif self.loglevel == 'CRITICAL' and loglevel == 'CRITICAL':
+            return self.mysql.raw_query(
+                "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
+            return self.mysql.update(table='task_execution_log',
+                                     columns=['reload_id', 'task_id', 'log_level', 'created_at', 'line_number', 'message'],
+                                     values=[self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message])
+        elif self.loglevel == 'INFO' and (loglevel == 'INFO' or loglevel == 'ERROR' or loglevel == 'CRITICAL'):
+            # Count the errors
+            if loglevel == 'ERROR' or loglevel == 'CRITICAL':
                 self.error_count += 1
-                return self.mysql.raw_query(
-                    "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
+            return self.mysql.raw_query(
+                "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
+        elif self.loglevel == 'ERROR' and (loglevel == 'ERROR' or loglevel == 'CRITICAL'):
+            self.error_count += 1
+            return self.mysql.raw_query(
+                "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
+        elif self.loglevel == 'CRITICAL' and loglevel == 'CRITICAL':
+            self.error_count += 1
+            return self.mysql.raw_query(
+                "INSERT INTO `task_execution_log` (reload_id, task_id, log_level, created_at, line_number, message) VALUES ({}, {}, '{}', '{}', {}, '{}')".format(self.run_id, self.task_id, loglevel, datetime.datetime.now(), linenumber, message), insert=True)
 
     def update_execution_step(self, step_number: int):
         """
         Update the current step number in the task_scheduler table so that user's in the frontend of SalureConnect can see where a task is at any moment
         :param step_number: Give only a number
         :return: nothing
         """
```

### Comparing `salure_helpers_task_scheduler-1.0.4/setup.py` & `salure_helpers_task_scheduler-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_task_scheduler',
-    version='1.0.4',
+    version='1.1.0',
     description='Task Scheduler from Salure',
     long_description='Task Schedule from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.task_scheduler"],
     license='Salure License',
     install_requires=[
```

