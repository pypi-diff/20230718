# Comparing `tmp/ndp-app-versioncontrol-1.6.tar.gz` & `tmp/ndp-app-versioncontrol-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndp-app-versioncontrol-1.6.tar", last modified: Fri Jul 14 06:40:48 2023, max compression
+gzip compressed data, was "ndp-app-versioncontrol-1.7.tar", last modified: Tue Jul 18 07:06:05 2023, max compression
```

## Comparing `ndp-app-versioncontrol-1.6.tar` & `ndp-app-versioncontrol-1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 06:40:48.135995 ndp-app-versioncontrol-1.6/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 06:40:48.135553 ndp-app-versioncontrol-1.6/PKG-INFO
--rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-14 06:39:26.000000 ndp-app-versioncontrol-1.6/README.md
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 06:40:48.133025 ndp-app-versioncontrol-1.6/ndp_app_versioncontrol.egg-info/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-14 06:40:47.000000 ndp-app-versioncontrol-1.6/ndp_app_versioncontrol.egg-info/PKG-INFO
--rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-14 06:40:48.000000 ndp-app-versioncontrol-1.6/ndp_app_versioncontrol.egg-info/SOURCES.txt
--rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-14 06:40:47.000000 ndp-app-versioncontrol-1.6/ndp_app_versioncontrol.egg-info/dependency_links.txt
--rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-14 06:40:47.000000 ndp-app-versioncontrol-1.6/ndp_app_versioncontrol.egg-info/requires.txt
--rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-14 06:40:47.000000 ndp-app-versioncontrol-1.6/ndp_app_versioncontrol.egg-info/top_level.txt
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-14 06:40:48.133758 ndp-app-versioncontrol-1.6/ndp_versioncontrol/
--rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.6/ndp_versioncontrol/__init__.py
--rwxrwxr-x   0 harshal    (502) staff       (20)    22891 2023-07-14 06:38:25.000000 ndp-app-versioncontrol-1.6/ndp_versioncontrol/generate_backup_sql.py
--rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-14 06:40:48.136310 ndp-app-versioncontrol-1.6/setup.cfg
--rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-14 06:39:04.000000 ndp-app-versioncontrol-1.6/setup.py
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:06:05.571924 ndp-app-versioncontrol-1.7/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-18 07:06:05.571544 ndp-app-versioncontrol-1.7/PKG-INFO
+-rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-18 07:05:35.000000 ndp-app-versioncontrol-1.7/README.md
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:06:05.570068 ndp-app-versioncontrol-1.7/ndp_app_versioncontrol.egg-info/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-18 07:06:05.000000 ndp-app-versioncontrol-1.7/ndp_app_versioncontrol.egg-info/PKG-INFO
+-rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-18 07:06:05.000000 ndp-app-versioncontrol-1.7/ndp_app_versioncontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-18 07:06:05.000000 ndp-app-versioncontrol-1.7/ndp_app_versioncontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-18 07:06:05.000000 ndp-app-versioncontrol-1.7/ndp_app_versioncontrol.egg-info/requires.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-18 07:06:05.000000 ndp-app-versioncontrol-1.7/ndp_app_versioncontrol.egg-info/top_level.txt
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:06:05.570946 ndp-app-versioncontrol-1.7/ndp_versioncontrol/
+-rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.7/ndp_versioncontrol/__init__.py
+-rwxrwxr-x   0 harshal    (502) staff       (20)    22916 2023-07-18 07:05:20.000000 ndp-app-versioncontrol-1.7/ndp_versioncontrol/generate_backup_sql.py
+-rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-18 07:06:05.572054 ndp-app-versioncontrol-1.7/setup.cfg
+-rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-18 07:05:46.000000 ndp-app-versioncontrol-1.7/setup.py
```

### Comparing `ndp-app-versioncontrol-1.6/PKG-INFO` & `ndp-app-versioncontrol-1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.6
+Version: 1.7
 Summary: Version Control Mechanism for Zetaris Platform (https://www.zetaris.com/)
 Home-page: https://github.com/zetaris/versioncontrol
 Author: Harshal Shah
 Author-email: harshal.shah@zetaris.com
 License: Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ### Usage and Installation
 ```
-pip3 install ndp-app-versioncontrol==1.6
+pip3 install ndp-app-versioncontrol==1.7
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.6/ndp_app_versioncontrol.egg-info/PKG-INFO` & `ndp-app-versioncontrol-1.7/ndp_app_versioncontrol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.6
+Version: 1.7
 Summary: Version Control Mechanism for Zetaris Platform (https://www.zetaris.com/)
 Home-page: https://github.com/zetaris/versioncontrol
 Author: Harshal Shah
 Author-email: harshal.shah@zetaris.com
 License: Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ### Usage and Installation
 ```
-pip3 install ndp-app-versioncontrol==1.6
+pip3 install ndp-app-versioncontrol==1.7
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.6/ndp_versioncontrol/generate_backup_sql.py` & `ndp-app-versioncontrol-1.7/ndp_versioncontrol/generate_backup_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     for i in range(2,max_pages+1):
         page_data=page_sql_query(query_token,page_limit,i)
         res += page_data['records']
     return res
 #----------------------------------------# 
 #GET ORD ID FROM EMAIL
 def get_org_id_from_email(lightning_username):
-    orgId_query = 'select id from metastore.organisation where lower(trim(email))='+"\'"+str(lightning_username)+"\'"
+    orgId_query = 'sselect fk_organisation_id as id from metastore.lightning_user where lower(trim(email))='+"\'"+str(lightning_username)+"\'"
     x = open_sql_query(orgId_query,100)
     orgid_dict = x['records']
     if isinstance(orgid_dict[0],dict):
         orgId = orgid_dict[0]['id']
     return orgId
 #----------------------------------------#
 #BACKUP OF PIPELINES AT INDIVIDUAL LEVEL
```

### Comparing `ndp-app-versioncontrol-1.6/setup.py` & `ndp-app-versioncontrol-1.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
   
 setuptools.setup(
     # Here is the module name.
     name="ndp-app-versioncontrol",
   
     # version of the module
-    version="1.6",
+    version="1.7",
   
     # Name of Author
     author="Harshal Shah",
 
     #License
     license="Proprietary",
```

