# Comparing `tmp/cyrating-1.0.8.tar.gz` & `tmp/cyrating-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cyrating-1.0.8.tar", last modified: Fri Mar 26 14:45:34 2021, max compression
+gzip compressed data, was "dist/cyrating-1.0.9.tar", last modified: Thu Apr 22 09:25:07 2021, max compression
```

## Comparing `cyrating-1.0.8.tar` & `cyrating-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-03-26 14:45:34.000000 cyrating-1.0.8/
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      207 2021-03-26 13:44:43.000000 cyrating-1.0.8/cyrating/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    16450 2021-03-26 14:45:21.000000 cyrating-1.0.8/cyrating/api.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating.egg-info/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7435 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      263 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating.egg-info/not-zip-safe
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       22 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        9 2021-03-26 14:45:34.000000 cyrating-1.0.8/cyrating.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1081 2020-08-21 09:52:08.000000 cyrating-1.0.8/LICENSE
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5360 2021-03-26 14:45:21.000000 cyrating-1.0.8/README.md
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      102 2021-03-26 14:45:34.000000 cyrating-1.0.8/setup.cfg
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      937 2020-08-21 09:46:47.000000 cyrating-1.0.8/setup.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7435 2021-03-26 14:45:34.000000 cyrating-1.0.8/PKG-INFO
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-04-22 09:25:07.000000 cyrating-1.0.9/
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      207 2021-04-22 09:24:52.000000 cyrating-1.0.9/cyrating/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    16553 2021-04-22 09:24:52.000000 cyrating-1.0.9/cyrating/api.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating.egg-info/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7502 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      263 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating.egg-info/not-zip-safe
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       22 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        9 2021-04-22 09:25:07.000000 cyrating-1.0.9/cyrating.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1081 2020-08-21 09:52:08.000000 cyrating-1.0.9/LICENSE
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5427 2021-04-22 09:24:52.000000 cyrating-1.0.9/README.md
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      102 2021-04-22 09:25:07.000000 cyrating-1.0.9/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      937 2020-08-21 09:46:47.000000 cyrating-1.0.9/setup.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7502 2021-04-22 09:25:07.000000 cyrating-1.0.9/PKG-INFO
```

### Comparing `cyrating-1.0.8/cyrating/api.py` & `cyrating-1.0.9/cyrating/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,16 +356,19 @@
       res += '\r\n'
     return res
 
   def format_result_us(self, us):
     res = '{} detected on port {}/{}'.format(names[us['service']], us['port'], us['proto'])
     return res
 
-  def facts(self, company, assets=None):
-    filter = {'where': json.dumps({'companies': company['_id']})}
+  def facts(self, company, assets=None, extra_filter=None):
+    where = {'companies': company['_id']}
+    if extra_filter is not None:
+      where.update(extra_filter)
+    filter = {'where': json.dumps(where)}
     filter.update({'max_results': 1000})
     assessements = self.findall(ASSESSMENT_ENDPOINT, 1, filter)
     global_us = dict()
 
     res = []
     for assessment in assessements:
       tags = assets[assessment['domainname']]['tags'] if assets else None
```

### Comparing `cyrating-1.0.8/cyrating.egg-info/PKG-INFO` & `cyrating-1.0.9/cyrating.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyrating
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python wrapper for https://www.cyrating.com.
 Home-page: UNKNOWN
 Author: Cyrating
 Author-email: tech@cyrating.com
 License: MIT
 Description: # python-cyrating
         
@@ -104,15 +104,15 @@
         [...]
         ```
         
         
         **Get results of best practices controls**
         
         The method facts returns the results of best practices controls. _assets_
-        parameter is optional and is needed to provide tags association.
+        parameter is optional and is needed to provide tags association. _extra_filter_ is also an optional to filter results server-side. 
         
         An best practice result includes the following attributes:
         
         - domain: domain name / AS Number linked with the asset
         - category: name of the best practice's category
         - entities: list of entities linked with the asset. Entities are the ones included in the subscription.
         - tags: list of tags linked with the asset
```

### Comparing `cyrating-1.0.8/LICENSE` & `cyrating-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cyrating-1.0.8/README.md` & `cyrating-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 [...]
 ```
 
 
 **Get results of best practices controls**
 
 The method facts returns the results of best practices controls. _assets_
-parameter is optional and is needed to provide tags association.
+parameter is optional and is needed to provide tags association. _extra_filter_ is also an optional to filter results server-side. 
 
 An best practice result includes the following attributes:
 
 - domain: domain name / AS Number linked with the asset
 - category: name of the best practice's category
 - entities: list of entities linked with the asset. Entities are the ones included in the subscription.
 - tags: list of tags linked with the asset
```

### Comparing `cyrating-1.0.8/setup.py` & `cyrating-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `cyrating-1.0.8/PKG-INFO` & `cyrating-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyrating
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python wrapper for https://www.cyrating.com.
 Home-page: UNKNOWN
 Author: Cyrating
 Author-email: tech@cyrating.com
 License: MIT
 Description: # python-cyrating
         
@@ -104,15 +104,15 @@
         [...]
         ```
         
         
         **Get results of best practices controls**
         
         The method facts returns the results of best practices controls. _assets_
-        parameter is optional and is needed to provide tags association.
+        parameter is optional and is needed to provide tags association. _extra_filter_ is also an optional to filter results server-side. 
         
         An best practice result includes the following attributes:
         
         - domain: domain name / AS Number linked with the asset
         - category: name of the best practice's category
         - entities: list of entities linked with the asset. Entities are the ones included in the subscription.
         - tags: list of tags linked with the asset
```

