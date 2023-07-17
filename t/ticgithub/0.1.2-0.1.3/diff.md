# Comparing `tmp/ticgithub-0.1.2.tar.gz` & `tmp/ticgithub-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticgithub-0.1.2.tar", last modified: Thu Apr 20 21:48:13 2023, max compression
+gzip compressed data, was "ticgithub-0.1.3.tar", last modified: Mon Jul 17 22:02:33 2023, max compression
```

## Comparing `ticgithub-0.1.2.tar` & `ticgithub-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.004928 ticgithub-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-20 21:47:59.000000 ticgithub-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-20 21:47:59.000000 ticgithub-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-20 21:48:13.004928 ticgithub-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-04-20 21:47:59.000000 ticgithub-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-20 21:48:13.004928 ticgithub-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-20 21:47:59.000000 ticgithub-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.000928 ticgithub-0.1.2/ticgithub/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 21:48:12.000000 ticgithub-0.1.2/ticgithub/_installed_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.000928 ticgithub-0.1.2/ticgithub/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.000928 ticgithub-0.1.2/ticgithub/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/templates/email_reply.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/templates/unassigned.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/templates/unclosed.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.000928 ticgithub-0.1.2/ticgithub/data/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/workflows/assignment-to-gmail.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/data/workflows/scheduled_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/inbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/issues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.004928 ticgithub-0.1.2/ticgithub/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tasks/assignment_to_gmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tasks/emails_to_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tasks/reminder_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tasks/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tasks/unassigned_reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tasks/unclosed_reminder.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/team.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.004928 ticgithub-0.1.2/ticgithub/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/tests/test_something.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.004928 ticgithub-0.1.2/ticgithub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/utils/datafiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-04-20 21:47:59.000000 ticgithub-0.1.2/ticgithub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:48:13.000928 ticgithub-0.1.2/ticgithub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-04-20 21:48:12.000000 ticgithub-0.1.2/ticgithub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 21:48:12.000000 ticgithub-0.1.2/ticgithub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:48:12.000000 ticgithub-0.1.2/ticgithub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-20 21:48:12.000000 ticgithub-0.1.2/ticgithub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 21:48:12.000000 ticgithub-0.1.2/ticgithub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-17 22:02:19.000000 ticgithub-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 22:02:19.000000 ticgithub-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-07-17 22:02:33.590149 ticgithub-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-07-17 22:02:19.000000 ticgithub-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-17 22:02:33.590149 ticgithub-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-17 22:02:19.000000 ticgithub-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-17 22:02:33.000000 ticgithub-0.1.3/ticgithub/_installed_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/build_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/templates/email_reply.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/templates/unassigned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/templates/unclosed.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub/data/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/workflows/assignment-to-gmail.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/data/workflows/scheduled_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/inbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/issues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tasks/assignment_to_gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tasks/emails_to_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tasks/reminder_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tasks/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tasks/unassigned_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tasks/unclosed_reminder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/team.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/tests/test_something.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/utils/datafiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-07-17 22:02:19.000000 ticgithub-0.1.3/ticgithub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:02:33.590149 ticgithub-0.1.3/ticgithub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-07-17 22:02:33.000000 ticgithub-0.1.3/ticgithub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-17 22:02:33.000000 ticgithub-0.1.3/ticgithub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:02:33.000000 ticgithub-0.1.3/ticgithub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 22:02:33.000000 ticgithub-0.1.3/ticgithub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 22:02:33.000000 ticgithub-0.1.3/ticgithub.egg-info/top_level.txt
```

### Comparing `ticgithub-0.1.2/LICENSE` & `ticgithub-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/PKG-INFO` & `ticgithub-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ticgithub
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use GitHub as a ticketing system for shared GMail
 Home-page: https://github.com/dwhswenson/ticgithub
 Author: David W.H. Swenson
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `ticgithub-0.1.2/README.md` & `ticgithub-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/setup.cfg` & `ticgithub-0.1.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ticgithub
-version = 0.1.2
+version = 0.1.3
 short_description = Use GitHub as a ticketing system for shared GMail
 description = Use GitHub as a ticketing system for shared GMail
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = David W.H. Swenson
 author_email = dwhs@hyperblazer.net
 license = MIT
```

### Comparing `ticgithub-0.1.2/setup.py` & `ticgithub-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/bot.py` & `ticgithub-0.1.3/ticgithub/bot.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/build.py` & `ticgithub-0.1.3/ticgithub/build.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/gmail.py` & `ticgithub-0.1.3/ticgithub/gmail.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/inbox.py` & `ticgithub-0.1.3/ticgithub/inbox.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/issues.py` & `ticgithub-0.1.3/ticgithub/issues.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/tasks/assignment_to_gmail.py` & `ticgithub-0.1.3/ticgithub/tasks/assignment_to_gmail.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/tasks/emails_to_issues.py` & `ticgithub-0.1.3/ticgithub/tasks/emails_to_issues.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/tasks/reminder_task.py` & `ticgithub-0.1.3/ticgithub/tasks/reminder_task.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/tasks/task.py` & `ticgithub-0.1.3/ticgithub/tasks/task.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/tasks/unassigned_reminder.py` & `ticgithub-0.1.3/ticgithub/tasks/unassigned_reminder.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/tasks/unclosed_reminder.py` & `ticgithub-0.1.3/ticgithub/tasks/unclosed_reminder.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub/version.py` & `ticgithub-0.1.3/ticgithub/version.py`

 * *Files identical despite different names*

### Comparing `ticgithub-0.1.2/ticgithub.egg-info/PKG-INFO` & `ticgithub-0.1.3/ticgithub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ticgithub
-Version: 0.1.2
+Version: 0.1.3
 Summary: Use GitHub as a ticketing system for shared GMail
 Home-page: https://github.com/dwhswenson/ticgithub
 Author: David W.H. Swenson
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `ticgithub-0.1.2/ticgithub.egg-info/SOURCES.txt` & `ticgithub-0.1.3/ticgithub.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ticgithub/version.py
 ticgithub.egg-info/PKG-INFO
 ticgithub.egg-info/SOURCES.txt
 ticgithub.egg-info/dependency_links.txt
 ticgithub.egg-info/requires.txt
 ticgithub.egg-info/top_level.txt
 ticgithub/data/__init__.py
+ticgithub/data/build_config.yml
 ticgithub/data/templates/__init__.py
 ticgithub/data/templates/email_reply.txt
 ticgithub/data/templates/unassigned.txt
 ticgithub/data/templates/unclosed.txt
 ticgithub/data/workflows/__init__.py
 ticgithub/data/workflows/assignment-to-gmail.yml
 ticgithub/data/workflows/scheduled_workflow.yml
```

