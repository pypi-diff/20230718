# Comparing `tmp/OBP_monitoring_v2-0.0.2.tar.gz` & `tmp/OBP_monitoring_v2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_monitoring_v2-0.0.2.tar", last modified: Tue Jan 24 13:34:53 2023, max compression
+gzip compressed data, was "OBP_monitoring_v2-0.0.3.tar", last modified: Tue Jul 18 05:33:45 2023, max compression
```

## Comparing `OBP_monitoring_v2-0.0.2.tar` & `OBP_monitoring_v2-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 13:34:53.085340 OBP_monitoring_v2-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-01-24 13:34:53.052550 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/
--rw-rw-rw-   0        0        0     1771 2023-01-24 13:34:12.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/__init__.py
--rw-rw-rw-   0        0        0     2112 2023-01-24 10:21:31.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/asg_elb_healthcheck_required.py
--rw-rw-rw-   0        0        0     2244 2023-01-24 13:31:15.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1999 2023-01-24 13:31:37.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/guard_duty_enabled.py
--rw-rw-rw-   0        0        0     2361 2023-01-24 13:34:12.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/lambda_concurrency_check.py
--rw-rw-rw-   0        0        0     1950 2023-01-24 13:34:12.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/lambda_dlq_check.py
--rw-rw-rw-   0        0        0     2137 2023-01-24 13:33:38.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py
--rw-rw-rw-   0        0        0     1637 2023-01-24 13:33:38.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/s3_event_notifications_enabled.py
--rw-rw-rw-   0        0        0     1627 2023-01-17 06:00:31.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-24 13:34:53.069696 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2.egg-info/
--rw-rw-rw-   0        0        0      376 2023-01-24 13:34:52.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-01-24 13:34:52.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 13:34:52.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-01-24 13:34:52.000000 OBP_monitoring_v2-0.0.2/OBP_monitoring_v2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      376 2023-01-24 13:34:53.069696 OBP_monitoring_v2-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_monitoring_v2-0.0.2/README.md
--rw-rw-rw-   0        0        0      557 2023-01-24 13:34:12.000000 OBP_monitoring_v2-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-24 13:34:53.085340 OBP_monitoring_v2-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 05:33:45.835538 OBP_monitoring_v2-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-18 05:33:45.796543 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/
+-rw-rw-rw-   0        0        0     1771 2023-07-18 05:31:32.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/__init__.py
+-rw-rw-rw-   0        0        0     2112 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/asg_elb_healthcheck_required.py
+-rw-rw-rw-   0        0        0     2244 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     1999 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/guard_duty_enabled.py
+-rw-rw-rw-   0        0        0     2361 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_concurrency_check.py
+-rw-rw-rw-   0        0        0     1950 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_dlq_check.py
+-rw-rw-rw-   0        0        0     2137 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py
+-rw-rw-rw-   0        0        0     1853 2023-07-18 05:31:32.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/s3_event_notifications_enabled.py
+-rw-rw-rw-   0        0        0     1627 2023-01-25 05:47:41.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-18 05:33:45.829548 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-18 05:33:45.000000 OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      376 2023-07-18 05:33:45.834540 OBP_monitoring_v2-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_monitoring_v2-0.0.3/README.md
+-rw-rw-rw-   0        0        0      557 2023-07-18 05:32:06.000000 OBP_monitoring_v2-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 05:33:45.836539 OBP_monitoring_v2-0.0.3/setup.cfg
```

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/__init__.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 __author__ = 'Klera DevOps'
-__version__ = '0.0.2'
+__version__ = '0.0.3'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
             self.session = session.Session(
                 aws_access_key_id=kwargs['aws_access_key_id'],
```

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/asg_elb_healthcheck_required.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/asg_elb_healthcheck_required.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/ec2_instance_detailed_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/guard_duty_enabled.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/guard_duty_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/lambda_concurrency_check.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_concurrency_check.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/lambda_dlq_check.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/lambda_dlq_check.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/rds_enhanced_monitoring_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/s3_event_notifications_enabled.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/s3_event_notifications_enabled.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from botocore.exceptions import ClientError
+
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
 # checks the compliance.py for s3 bucket versioning enabled
 def s3_event_notifications_enabled(self):
     """
@@ -39,14 +41,18 @@
                 raise KeyError
             
         except KeyError:
             result = False
             failReason = "Notifications are turned off for S3 buckets."
             offenders.append(bucket_name)
             continue
+        except ClientError:
+            result = False
+            failReason = "Access denied for get_bucket_logging api"
+            offenders.append(bucket_name)
 
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
```

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2/utils.py` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/OBP_monitoring_v2.egg-info/SOURCES.txt` & `OBP_monitoring_v2-0.0.3/OBP_monitoring_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OBP_monitoring_v2-0.0.2/pyproject.toml` & `OBP_monitoring_v2-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "OBP_monitoring_v2"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="dheeraj.banodha", email="dheeraj.banodha@impetus.com" },
   { name="ravish.sharma", email="ravish.sharma@impetus.com"}
 ]
 description = "Provides AWS compliance details"
 readme = "README.md"
 requires-python = ">=3.7"
```

