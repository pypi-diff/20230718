# Comparing `tmp/easy_boto3-0.1.0.tar.gz` & `tmp/easy_boto3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_boto3-0.1.0.tar", max compression
+gzip compressed data, was "easy_boto3-0.1.1.tar", max compression
```

## Comparing `easy_boto3-0.1.0.tar` & `easy_boto3-0.1.1.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-07-10 17:55:57.377097 easy_boto3-0.1.0/LICENSE
--rw-r--r--   0        0        0     6990 2023-07-17 23:02:00.586125 easy_boto3-0.1.0/README.md
--rw-r--r--   0        0        0       27 2023-07-17 21:41:25.728959 easy_boto3-0.1.0/easy_boto3/.easy_boto3_internal.yaml
--rw-r--r--   0        0        0      526 2023-07-17 22:51:50.692181 easy_boto3-0.1.0/easy_boto3/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 18:20:59.907784 easy_boto3-0.1.0/easy_boto3/cloudwatch/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 18:45:34.715085 easy_boto3-0.1.0/easy_boto3/cloudwatch/cloudwatch_alarm_management.py
--rw-r--r--   0        0        0     1377 2023-07-17 21:33:51.494495 easy_boto3-0.1.0/easy_boto3/cloudwatch/create.py
--rw-r--r--   0        0        0     1415 2023-07-17 21:38:49.957012 easy_boto3-0.1.0/easy_boto3/cloudwatch/delete.py
--rw-r--r--   0        0        0      878 2023-07-17 21:13:41.987198 easy_boto3-0.1.0/easy_boto3/cloudwatch/list.py
--rw-r--r--   0        0        0        0 2023-07-14 16:10:48.468896 easy_boto3-0.1.0/easy_boto3/ec2/__init__.py
--rw-r--r--   0        0        0     2535 2023-07-17 21:41:22.416004 easy_boto3-0.1.0/easy_boto3/ec2/config_parser.py
--rw-r--r--   0        0        0     1550 2023-07-14 17:08:05.703887 easy_boto3-0.1.0/easy_boto3/ec2/create.py
--rw-r--r--   0        0        0     2586 2023-07-12 15:54:07.724121 easy_boto3-0.1.0/easy_boto3/ec2/ec2_connections_management.py
--rw-r--r--   0        0        0     1494 2023-07-14 18:20:23.864509 easy_boto3-0.1.0/easy_boto3/ec2/ec2_instance_management.py
--rw-r--r--   0        0        0     1741 2023-07-17 21:37:31.124132 easy_boto3-0.1.0/easy_boto3/ec2/list.py
--rw-r--r--   0        0        0      642 2023-07-14 18:11:41.517039 easy_boto3-0.1.0/easy_boto3/ec2/stop.py
--rw-r--r--   0        0        0        0 2023-07-14 16:22:08.810157 easy_boto3-0.1.0/easy_boto3/ec2/stop_all.py
--rw-r--r--   0        0        0      846 2023-07-17 21:40:08.536409 easy_boto3-0.1.0/easy_boto3/ec2/terminate.py
--rw-r--r--   0        0        0     5184 2023-07-17 22:54:25.084059 easy_boto3-0.1.0/easy_boto3/main.py
--rw-r--r--   0        0        0        0 2023-07-14 16:35:55.922225 easy_boto3-0.1.0/easy_boto3/profile/__init__.py
--rw-r--r--   0        0        0     1368 2023-07-14 16:36:35.646841 easy_boto3-0.1.0/easy_boto3/profile/profile.py
--rw-r--r--   0        0        0      895 2023-07-13 16:14:54.469901 easy_boto3-0.1.0/easy_boto3/setup_session.py
--rw-r--r--   0        0        0        0 2023-07-11 17:01:45.508281 easy_boto3-0.1.0/easy_boto3/utilities/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-12 23:06:33.332283 easy_boto3-0.1.0/easy_boto3/utilities/aws_profile_parser.py
--rw-r--r--   0        0        0     2471 2023-07-17 19:36:39.848635 easy_boto3-0.1.0/easy_boto3/utilities/decorators.py
--rw-r--r--   0        0        0     1270 2023-07-10 14:50:20.270314 easy_boto3-0.1.0/easy_boto3/utilities/logger_maker.py
--rw-r--r--   0        0        0     2215 2023-07-14 16:58:55.762236 easy_boto3-0.1.0/easy_boto3/utilities/script_manager.py
--rw-r--r--   0        0        0      994 2023-07-17 23:03:56.468066 easy_boto3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8101 1970-01-01 00:00:00.000000 easy_boto3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6960 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/README.md
+-rw-r--r--   0        0        0      526 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/cloudwatch/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/cloudwatch/cloudwatch_alarm_management.py
+-rw-r--r--   0        0        0     1377 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/cloudwatch/create.py
+-rw-r--r--   0        0        0     1415 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/cloudwatch/delete.py
+-rw-r--r--   0        0        0      878 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/cloudwatch/list.py
+-rw-r--r--   0        0        0        0 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/__init__.py
+-rw-r--r--   0        0        0     2535 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/config_parser.py
+-rw-r--r--   0        0        0     1550 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/create.py
+-rw-r--r--   0        0        0     2586 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/ec2_connections_management.py
+-rw-r--r--   0        0        0     1494 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/ec2_instance_management.py
+-rw-r--r--   0        0        0     1741 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/list.py
+-rw-r--r--   0        0        0      642 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/stop.py
+-rw-r--r--   0        0        0        0 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/stop_all.py
+-rw-r--r--   0        0        0      846 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/ec2/terminate.py
+-rw-r--r--   0        0        0     5184 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/main.py
+-rw-r--r--   0        0        0        0 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/profile/__init__.py
+-rw-r--r--   0        0        0     1368 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/profile/profile.py
+-rw-r--r--   0        0        0      895 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/setup_session.py
+-rw-r--r--   0        0        0        0 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/utilities/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/utilities/aws_profile_parser.py
+-rw-r--r--   0        0        0     2471 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/utilities/decorators.py
+-rw-r--r--   0        0        0     1270 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/utilities/logger_maker.py
+-rw-r--r--   0        0        0     2215 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/easy_boto3/utilities/script_manager.py
+-rw-r--r--   0        0        0      994 2023-07-17 23:16:11.619642 easy_boto3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     8071 1970-01-01 00:00:00.000000 easy_boto3-0.1.1/PKG-INFO
```

### Comparing `easy_boto3-0.1.0/LICENSE` & `easy_boto3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/README.md` & `easy_boto3-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# `easy_boto3` CLI and Python `boto3` made simple 
+# `boto3` made easy 
 
 `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 
 ### Contents
 - [`easy_boto3` CLI and Python `boto3` made simple](#easy_boto3-cli-and-python-boto3-made-simple)
     - [Contents](#contents)
   - [Installation](#installation)
@@ -14,15 +14,15 @@
     - [Creating an ec2 instance](#creating-an-ec2-instance)
 
 ## Installation 
 
 You can install `easy_boto3` via `pip` as
 
 ```bash
-pip install easy_boto3
+pip install easy-boto3
 ```
 
 ## Using `easy_boto3` CLI
 
 ### Creating an ec2 instance with cloudwatch alarm
 
 `easy_boto3` allows you to translate a standard `boto3` pythonic infrastructure task like instantiating an `ec2` instance with an attached `cloudwatch` cpu usage alarm from complex pythonic implementation like the following
```

### Comparing `easy_boto3-0.1.0/easy_boto3/__init__.py` & `easy_boto3-0.1.1/easy_boto3/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/cloudwatch/create.py` & `easy_boto3-0.1.1/easy_boto3/cloudwatch/create.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/cloudwatch/delete.py` & `easy_boto3-0.1.1/easy_boto3/cloudwatch/delete.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/cloudwatch/list.py` & `easy_boto3-0.1.1/easy_boto3/cloudwatch/list.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/ec2/config_parser.py` & `easy_boto3-0.1.1/easy_boto3/ec2/config_parser.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/ec2/create.py` & `easy_boto3-0.1.1/easy_boto3/ec2/create.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/ec2/ec2_connections_management.py` & `easy_boto3-0.1.1/easy_boto3/ec2/ec2_connections_management.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/ec2/ec2_instance_management.py` & `easy_boto3-0.1.1/easy_boto3/ec2/ec2_instance_management.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/ec2/list.py` & `easy_boto3-0.1.1/easy_boto3/ec2/list.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/ec2/stop.py` & `easy_boto3-0.1.1/easy_boto3/ec2/stop.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/ec2/terminate.py` & `easy_boto3-0.1.1/easy_boto3/ec2/terminate.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/main.py` & `easy_boto3-0.1.1/easy_boto3/main.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/profile/profile.py` & `easy_boto3-0.1.1/easy_boto3/profile/profile.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/setup_session.py` & `easy_boto3-0.1.1/easy_boto3/setup_session.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/utilities/aws_profile_parser.py` & `easy_boto3-0.1.1/easy_boto3/utilities/aws_profile_parser.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/utilities/decorators.py` & `easy_boto3-0.1.1/easy_boto3/utilities/decorators.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/utilities/logger_maker.py` & `easy_boto3-0.1.1/easy_boto3/utilities/logger_maker.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/easy_boto3/utilities/script_manager.py` & `easy_boto3-0.1.1/easy_boto3/utilities/script_manager.py`

 * *Files identical despite different names*

### Comparing `easy_boto3-0.1.0/pyproject.toml` & `easy_boto3-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easy_boto3"
-version = "0.1.0"
+version = "0.1.1"
 description = "`easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file."
 authors = ["Jeremy Watt <jermwatt@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jermwatt/easy_boto3"
 packages = [{include = "easy_boto3"}]
 include = ["easy_boto3/.easy_boto3_internal.yaml"]
```

### Comparing `easy_boto3-0.1.0/PKG-INFO` & `easy_boto3-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-boto3
-Version: 0.1.0
+Version: 0.1.1
 Summary: `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 Home-page: https://github.com/jermwatt/easy_boto3
 Author: Jeremy Watt
 Author-email: jermwatt@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -18,15 +18,15 @@
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# `easy_boto3` CLI and Python `boto3` made simple 
+# `boto3` made easy 
 
 `easy_boto3` simplifies `boto3` usage by adding a command line interface (CLI) and abridged Python API that allows you to easily create, manage, and tear-down AWS resources using `boto3` and `awscli` in a simple, easy to use, and easy to refactor `.yaml` configuration file.
 
 ### Contents
 - [`easy_boto3` CLI and Python `boto3` made simple](#easy_boto3-cli-and-python-boto3-made-simple)
     - [Contents](#contents)
   - [Installation](#installation)
@@ -38,15 +38,15 @@
     - [Creating an ec2 instance](#creating-an-ec2-instance)
 
 ## Installation 
 
 You can install `easy_boto3` via `pip` as
 
 ```bash
-pip install easy_boto3
+pip install easy-boto3
 ```
 
 ## Using `easy_boto3` CLI
 
 ### Creating an ec2 instance with cloudwatch alarm
 
 `easy_boto3` allows you to translate a standard `boto3` pythonic infrastructure task like instantiating an `ec2` instance with an attached `cloudwatch` cpu usage alarm from complex pythonic implementation like the following
```

