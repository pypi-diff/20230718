# Comparing `tmp/gammarer.aws-ec2-instance-running-scheduler-0.4.1.tar.gz` & `tmp/gammarer.aws-ec2-instance-running-scheduler-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-0.4.1.tar", last modified: Tue Jul 18 08:29:44 2023, max compression
+gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-0.4.2.tar", last modified: Tue Jul 18 19:20:56 2023, max compression
```

## Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1.tar` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:29:44.015638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-18 08:29:44.015638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:29:44.015638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:29:44.011638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:29:44.011638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:29:44.015638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:29:44.015638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:29:32.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:29:44.015638 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-18 08:29:43.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-18 08:29:43.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:29:43.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 08:29:43.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 08:29:43.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:20:56.519206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-18 19:20:56.519206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:20:56.519206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:20:56.515206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:20:56.515206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:20:56.519206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:20:56.519206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20662 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:20:41.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:20:56.519206 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-18 19:20:56.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-18 19:20:56.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:20:56.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 19:20:56.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 19:20:56.000000 gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/LICENSE` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 0.4.1
+Version: 0.4.2
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/README.md` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/setup.py` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-instance-running-scheduler",
-    "version": "0.4.1",
+    "version": "0.4.2",
     "description": "AWS EC2 Instance Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-ec2-instance-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_ec2_instance_running_scheduler",
         "gammarer.aws_ec2_instance_running_scheduler._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_instance_running_scheduler._jsii": [
-            "aws-ec2-instance-running-scheduler@0.4.1.jsii.tgz"
+            "aws-ec2-instance-running-scheduler@0.4.2.jsii.tgz"
         ],
         "gammarer.aws_ec2_instance_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.1.jsii.tgz` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.2.jsii.tgz`

 * *Files 15% similar despite different names*

#### Comparing `aws-ec2-instance-running-scheduler@0.4.1.jsii.tgz-content` & `aws-ec2-instance-running-scheduler@0.4.2.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'3FkUqynUnfaCItwMinaEG9qN5yHwzkR3IuEOzuekaII='", "'version'": "'0.4.2'"}*

```diff
@@ -3304,15 +3304,15 @@
             }
         }
     },
     "description": "AWS EC2 Instance Running Scheduler",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "ZPOhfvbUfEUgGMtPRu4m9KweDYxSdHe8Z2k/BjZw7VQ=",
+    "fingerprint": "3FkUqynUnfaCItwMinaEG9qN5yHwzkR3IuEOzuekaII=",
     "homepage": "https://github.com/yicr/aws-ec2-instance-running-scheduler.git",
     "jsiiVersion": "1.85.0 (build 08ee592)",
     "keywords": [
         "auto",
         "aws",
         "aws-cdk",
         "cdk",
@@ -3574,9 +3574,9 @@
                         "fqn": "@gammarer/aws-ec2-instance-running-scheduler.ScheduleProperty"
                     }
                 }
             ],
             "symbolId": "src/index:TargetsProperty"
         }
     },
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -111,10 +111,10 @@
         }
     }
 }
 exports.Ec2InstanceRunningScheduler = Ec2InstanceRunningScheduler;
 _a = JSII_RTTI_SYMBOL_1;
 Ec2InstanceRunningScheduler[_a] = {
     fqn: "@gammarer/aws-ec2-instance-running-scheduler.Ec2InstanceRunningScheduler",
-    version: "0.4.1"
+    version: "0.4.2"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSxpQ0FBaUM7QUFDakMsbUNBQW1DO0FBQ25DLDJDQUEyQztBQUMzQyx1REFBdUQ7QUFDdkQsMkNBQXVDO0FBbUJ2QyxNQUFhLDJCQUE0QixTQUFRLHNCQUFTO0lBQ3hELFlBQVksS0FBZ0IsRUFBRSxFQUFVLEVBQUUsS0FBdUM7UUFDL0UsS0FBSyxDQUFDLEtBQUssRUFBRSxFQUFFLENBQUMsQ0FBQztRQUVqQixNQUFNLE9BQU8sR0FBRyxHQUFHLENBQUMsS0FBSyxDQUFDLEVBQUUsQ0FBQyxJQUFJLENBQUMsQ0FBQyxPQUFPLENBQUM7UUFDM0MseURBQXlEO1FBQ3pELDJDQUEyQztRQUUzQyxNQUFNLGFBQWEsR0FBRyxNQUFNLENBQUMsVUFBVSxDQUFDLFVBQVUsRUFBRSxFQUFFLFlBQVksRUFBRSxDQUFDLEVBQUUsQ0FBQzthQUNyRSxNQUFNLENBQUMsR0FBRyxHQUFHLENBQUMsS0FBSyxDQUFDLFFBQVEsQ0FBQyxLQUFLLENBQUMsSUFBSSxHQUFHLENBQUMsS0FBSyxDQUFDLFFBQVEsQ0FBQyxJQUFJLENBQUMsRUFBRSxDQUFDO2FBQ2xFLE1BQU0sQ0FBQyxLQUFLLENBQUMsQ0FBQztRQUVqQixtQ0FBbUM7UUFDbkMsTUFBTSxzQkFBc0IsR0FBRyxJQUFJLEdBQUcsQ0FBQyxJQUFJLENBQUMsSUFBSSxFQUFFLHdCQUF3QixFQUFFO1lBQzFFLFFBQVEsRUFBRSw4QkFBOEIsYUFBYSxZQUFZO1lBQ2pFLFNBQVMsRUFBRSxJQUFJLEdBQUcsQ0FBQyxnQkFBZ0IsQ0FBQyx5QkFBeUIsQ0FBQztZQUM5RCxjQUFjLEVBQUU7Z0JBQ2QsQ0FBQywwQkFBMEIsQ0FBQyxFQUFFLElBQUksR0FBRyxDQUFDLGNBQWMsQ0FBQztvQkFDbkQsVUFBVSxFQUFFO3dCQUNWLElBQUksR0FBRyxDQUFDLGVBQWUsQ0FBQzs0QkFD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TUFBTSxDQUFDLGFBQWEsQ0FBQyxJQUFJLElBQUksU0FBUyxDQUFDO29CQUM1RCxPQUFPLFFBQVEsTUFBTSxJQUFJLElBQUksUUFBUSxJQUFJLEtBQUssQ0FBQztnQkFDakQsQ0FBQyxDQUFDLEVBQUU7Z0JBQ0osTUFBTSxFQUFFO29CQUNOLEdBQUcsRUFBRSxnREFBZ0Q7b0JBQ3JELE9BQU8sRUFBRSxzQkFBc0IsQ0FBQyxPQUFPO29CQUN2QyxLQUFLLEVBQUUsSUFBSSxDQUFDLFNBQVMsQ0FBQyxFQUFFLFdBQVcsRUFBRSxNQUFNLENBQUMsU0FBUyxFQUFFLENBQUM7b0JBQ3hELFdBQVcsRUFBRTt3QkFDWCx3QkFBd0IsRUFBRSxFQUFFO3dCQUM1QixvQkFBb0IsRUFBRSxDQUFDO3FCQUN4QjtpQkFDRjthQUNGLENBQUMsQ0FBQztTQUNKO0lBQ0gsQ0FBQzs7QUFsR0gsa0VBbUdDIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0ICogYXMgY3J5cHRvIGZyb20gJ2NyeXB0byc7XG5pbXBvcnQgKiBhcyBjZGsgZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0ICogYXMgaWFtIGZyb20gJ2F3cy1jZGstbGliL2F3cy1pYW0nO1xuaW1wb3J0ICogYXMgc2NoZWR1bGVyIGZyb20gJ2F3cy1jZGstbGliL2F3cy1zY2hlZHVsZXInO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5cbmV4cG9ydCBpbnRlcmZhY2UgU2NoZWR1bGVQcm9wZXJ0eSB7XG4gIHJlYWRvbmx5IHRpbWV6b25lOiBzdHJpbmc7XG4gIHJlYWRvbmx5IG1pbnV0ZT86IHN0cmluZztcbiAgcmVhZG9ubHkgaG91cj86IHN0cmluZztcbiAgcmVhZG9ubHkgd2Vlaz86IHN0cmluZztcbn1cblxuZXhwb3J0IGludGVyZmFjZSBUYXJnZXRzUHJvcGVydHkge1xuICByZWFkb25seSBpbnN0YW5jZXM6IHN0cmluZ1tdO1xuICByZWFkb25seSBzdG9wU2NoZWR1bGU6IFNjaGVkdWxlUHJvcGVydHk7XG4gIHJlYWRvbmx5IHN0YXJ0U2NoZWR1bGU6IFNjaGVkdWxlUHJvcGVydHk7XG59XG5cbmV4cG9ydCBpbnRlcmZhY2UgRWMySW5zdGFuY2VSdW5uaW5nU2NoZWR1bGVyUHJvcHMge1xuICByZWFkb25seSB0YXJnZXRzOiBUYXJnZXRzUHJvcGVydHlbXTtcbn1cblxuZXhwb3J0IGNsYXNzIEVjMkluc3RhbmNlUnVubmluZ1NjaGVkdWxlciBleHRlbmRzIENvbnN0cnVjdCB7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBFYzJJbnN0YW5jZVJ1bm5pbmdTY2hlZHVsZXJQcm9wcykge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG5cbiAgICBjb25zdCBhY2NvdW50ID0gY2RrLlN0YWNrLm9mKHRoaXMpLmFjY291bnQ7XG4gICAgLy9jb25zdCBzdGFja05hbWU6IHN0cmluZyA9IGNkay5TdGFjay5vZih0aGlzKS5zdGFja05hbWU7XG4gICAgLy9jb25zdCByZWdpb24gPSBjZGsuU3RhY2sub2YodGhpcykucmVnaW9uO1xuXG4gICAgY29uc3QgcmFuZG9tTmFtZUtleSA9IGNyeXB0by5jcmVhdGVIYXNoKCdzaGFrZTI1NicsIHsgb3V0cHV0TGVuZ3RoOiA0IH0pXG4gICAgICAudXBkYXRlKGAke2Nkay5OYW1lcy51bmlxdWVJZChzY29wZSl9LSR7Y2RrLk5hbWVzLnVuaXF1ZUlkKHRoaXMpfWApXG4gICAgICAuZGlnZXN0KCdoZXgnKTtcblxuICAgIC8vIPCfkYdFdmVudEJyaWRnZSBTY2hlZHVsZXIgSUFNIFJvbGVcbiAgICBjb25zdCBzY2hlZHVsZXJFeGVjdXRpb25Sb2xlID0gbmV3IGlhbS5Sb2xlKHRoaXMsICdTY2hlZHVsZXJFeGVjdXRpb25Sb2xlJywge1xuICAgICAgcm9sZU5hbWU6IGBzdG9wLWVjMi1pbnN0YW5jZS1zY2hlZHVsZS0ke3JhbmRvbU5hbWVLZXl9LWV4ZWMtcm9sZWAsXG4gICAgICBhc3N1bWVkQnk6IG5ldyBpYW0uU2VydmljZVByaW5jaXBhbCgnc2NoZWR1bGVyLmFtYXpvbmF3cy5jb20nKSxcbiAgICAgIGlubGluZVBvbGljaWVzOiB7XG4gICAgICAgIFsnZWMyLWluc3RhbmNlLXN0b3AtcG9saWN5J106IG5ldyBpYW0uUG9saWN5RG9jdW1lbnQoe1xuICAgICAgICAgIHN0YXRlbWVudHM6IFtcbiAgICAgICAgICAgIG5ldyBpYW0uUG9saWN5U3RhdGVtZW50KHtcbiAgICAgICAgICAgICAgZWZmZWN0OiBpYW0uRWZmZWN0LkFMTE9XLFxuICAgICAgICAgICAgICBhY3Rpb25zOiBbXG4gICAgICAgICAgICAgICAgJ2VjMjpTdGFydEluc3RhbmNlcycsXG4gICAgICAgICAgICAgICAgJ2VjMjpTdG9wSW5zdGFuY2VzJyxcbiAgICAgICAgICAgICAgXSxcbiAgICAgICAgICAgICAgcmVzb3VyY2VzOiBbXG4gICAgICAgICAgICAgICAgYGFybjphd3M6ZWMyOio6JHthY2NvdW50fTppbnN0YW5jZS8qYCxcbiAgICAgICAgICAgICAgXSxcbiAgICAgICAgICAgIH0pLFxuICAgICAgICAgIF0sXG4gICAgICAgIH0pLFxuICAgICAgfSxcbiAgICB9KTtcblxuICAgIC8vIE9iamVjdC5lbnRyaWVzKHByb3BzLnRhcmdldHMpXG5cbiAgICBmb3IgKGNvbnN0IHRhcmdldCBvZiBwcm9wcy50YXJnZXRzKSB7XG4gICAgICAvLyDwn5GHQ3JlYXRlIHJhbmRvbSBzdHJpbmdcbiAgICAgIGNvbnN0IHNjaGVkdWxlTmFtZUtleSA9IGNyeXB0by5jcmVhdGVIYXNoKCdzaGFrZTI1NicsIHsgb3V0cHV0TGVuZ3RoOiA0IH0pXG4gICAgICAgIC51cGRhdGUodGFyZ2V0Lmluc3RhbmNlcy50b1N0cmluZygpKVxuICAgICAgICAuZGlnZXN0KCdoZXgnKTtcblxuICAgICAgLy8g8J+Rh0V2ZW50QnJpZGdlIFNjaGVkdWxlciBmb3IgREIgSW5zdGFuY2UgU3RvcFxuICAgICAgbmV3IHNjaGVkdWxlci5DZm5TY2hlZHVsZSh0aGlzLCBgU3RvcFNjaGVkdWxlJHtzY2hlZHVsZU5hbWVLZXkudG9VcHBlckNhc2UoKX1gLCB7XG4gICAgICAgIG5hbWU6IGBhdXRvLXN0b3AtZWMyLWluc3RhbmNlLSR7c2NoZWR1bGVOYW1lS2V5fS1zY2hlZHVsZWAsXG4gICAgICAgIGRlc2NyaXB0aW9uOiBgYXV0byBzdG9wIGVjMiBpbnN0YW5jZSAoJHt0YXJnZXQuaW5zdGFuY2VzLmpvaW4oJywnKX0pIHNjaGVkdWxlLmAsXG4gICAgICAgIHN0YXRlOiAnRU5BQkxFRCcsXG4gICAgICAgIC8vZ3JvdXBOYW1lOiBzY2hlZHVsZUdyb3VwLm5hbWUsIC8vIGRlZmF1bHRcbiAgICAgICAgZmxleGlibGVUaW1lV2luZG93OiB7XG4gICAgICAgICAgbW9kZTogJ09GRicsXG4gICAgICAgIH0sXG4gICAgICAgIHNjaGVkdWxlRXhwcmVzc2lvblRpbWV6b25lOiB0YXJnZXQuc3RvcFNjaGVkdWxlLnRpbWV6b25lLFxuICAgICAgICBzY2hlZHVsZUV4cHJlc3Npb246ICgoKSA9PiB7XG4gICAgICAgICAgLy8gZGVmYXVsdDogd2Vla2RheSAyMToxMFxuICAgICAgICAgIGNvbnN0IG1pbnV0ZTogc3RyaW5nID0gdGFyZ2V0LnN0b3BTY2hlZHVsZS5taW51dGUgPz8gJzEwJztcbiAgICAgICAgICBjb25zdCBob3VyOiBzdHJpbmcgPSB0YXJnZXQuc3RvcFNjaGVkdWxlLmhvdXIgPz8gJzIxJztcbiAgICAgICAgICBjb25zdCB3ZWVrOiBzdHJpbmcgPSB0YXJnZXQuc3RvcFNjaGVkdWxlLndlZWsgPz8gJ01PTi1GUkknO1xuICAgICAgICAgIHJldHVybiBgY3Jvbigke21pbnV0ZX0gJHtob3VyfSA/ICogJHt3ZWVrfSAqKWA7XG4gICAgICAgIH0pKCksXG4gICAgICAgIHRhcmdldDoge1xuICAgICAgICAgIGFybjogJ2Fybjphd3M6c2NoZWR1bGVyOjo6YXdzLXNkazplYzI6c3RvcEluc3RhbmNlcycsXG4gICAgICAgICAgcm9sZUFybjogc2NoZWR1bGVyRXhlY3V0aW9uUm9sZS5yb2xlQXJuLFxuICAgICAgICAgIGlucHV0OiBKU09OLnN0cmluZ2lmeSh7IEluc3RhbmNlSWRzOiB0YXJnZXQuaW5zdGFuY2VzIH0pLFxuICAgICAgICAgIHJldHJ5UG9saWN5OiB7XG4gICAgICAgICAgICBtYXhpbXVtRXZlbnRBZ2VJblNlY29uZHM6IDYwLFxuICAgICAgICAgICAgbWF4aW11bVJldHJ5QXR0ZW1wdHM6IDAsXG4gICAgICAgICAgfSxcbiAgICAgICAgfSxcbiAgICAgIH0pO1xuXG4gICAgICAvLyDwn5GHRXZlbnRCcmlkZ2UgU2NoZWR1bGVyIGZvciBEQiBJbnN0YW5jZSBTdGFydFxuICAgICAgbmV3IHNjaGVkdWxlci5DZm5TY2hlZHVsZSh0aGlzLCBgU3RhcnRTY2hlZHVsZSR7c2NoZWR1bGVOYW1lS2V5LnRvVXBwZXJDYXNlKCl9YCwge1xuICAgICAgICBuYW1lOiBgYXV0by1zdGFydC1lYzItaW5zdGFuY2UtJHtzY2hlZHVsZU5hbWVLZXl9LXNjaGVkdWxlYCxcbiAgICAgICAgZGVzY3JpcHRpb246IGBhdXRvIHN0YXJ0IGVjMiBpbnN0YW5jZSgke3RhcmdldC5pbnN0YW5jZXMuam9pbignLCcpfSkgc2NoZWR1bGUuYCxcbiAgICAgICAgc3RhdGU6ICdFTkFCTEVEJyxcbiAgICAgICAgLy9ncm91cE5hbWU6IHNjaGVkdWxlR3JvdXAubmFtZSwgLy8gZGVmYXVsdFxuICAgICAgICBmbGV4aWJsZVRpbWVXaW5kb3c6IHtcbiAgICAgICAgICBtb2RlOiAnT0ZGJyxcbiAgICAgICAgfSxcbiAgICAgICAgc2NoZWR1bGVFeHByZXNzaW9uVGltZXpvbmU6IHRhcmdldC5zdGFydFNjaGVkdWxlLnRpbWV6b25lLFxuICAgICAgICBzY2hlZHVsZUV4cHJlc3Npb246ICgoKSA9PiB7XG4gICAgICAgICAgLy8gZGVmYXVsdDogd2Vla2RheSAwNzo1MFxuICAgICAgICAgIGNvbnN0IG1pbnV0ZTogc3RyaW5nID0gdGFyZ2V0LnN0YXJ0U2NoZWR1bGUubWludXRlID8/ICc1MCc7XG4gICAgICAgICAgY29uc3QgaG91cjogc3RyaW5nID0gdGFyZ2V0LnN0YXJ0U2NoZWR1bGUuaG91ciA/PyAnNyc7XG4gICAgICAgICAgY29uc3Qgd2Vlazogc3RyaW5nID0gdGFyZ2V0LnN0YXJ0U2NoZWR1bGUud2VlayA/PyAnTU9OLUZSSSc7XG4gICAgICAgICAgcmV0dXJuIGBjcm9uKCR7bWludXRlfSAke2hvdXJ9ID8gKiAke3dlZWt9ICopYDtcbiAgICAgICAgfSkoKSxcbiAgICAgICAgdGFyZ2V0OiB7XG4gICAgICAgICAgYXJuOiAnYXJuOmF3czpzY2hlZHVsZXI6Ojphd3Mtc2RrOmVjMjpzdGFydEluc3RhbmNlcycsXG4gICAgICAgICAgcm9sZUFybjogc2NoZWR1bGVyRXhlY3V0aW9uUm9sZS5yb2xlQXJuLFxuICAgICAgICAgIGlucHV0OiBKU09OLnN0cmluZ2lmeSh7IEluc3RhbmNlSWRzOiB0YXJnZXQuaW5zdGFuY2VzIH0pLFxuICAgICAgICAgIHJldHJ5UG9saWN5OiB7XG4gICAgICAgICAgICBtYXhpbXVtRXZlbnRBZ2VJblNlY29uZHM6IDYwLFxuICAgICAgICAgICAgbWF4aW11bVJldHJ5QXR0ZW1wdHM6IDAsXG4gICAgICAgICAgfSxcbiAgICAgICAgfSxcbiAgICAgIH0pO1xuICAgIH1cbiAgfVxufVxuIl19
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9731121281464531%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.71.142'}", "'version'": "'0.4.2'"}*

```diff
@@ -21,15 +21,15 @@
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.85.0",
         "jsii-docgen": "^7.2.9",
         "jsii-pacmak": "^1.85.0",
         "jsii-rosetta": "1.x",
         "npm-check-updates": "^16",
-        "projen": "^0.71.141",
+        "projen": "^0.71.142",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.1",
         "typescript": "^5.1.6"
     },
     "engines": {
         "node": ">= 16.0.0"
@@ -138,9 +138,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.4.1"
+    "version": "0.4.2"
 }
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 0.4.1
+Version: 0.4.2
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-0.4.1/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt` & `gammarer.aws-ec2-instance-running-scheduler-0.4.2/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
 src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
 src/gammarer/aws_ec2_instance_running_scheduler/py.typed
 src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
-src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.1.jsii.tgz
+src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@0.4.2.jsii.tgz
```

