# Comparing `tmp/ndp-app-migration-0.4.tar.gz` & `tmp/ndp-app-migration-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndp-app-migration-0.4.tar", last modified: Tue Jul 11 05:58:34 2023, max compression
+gzip compressed data, was "ndp-app-migration-0.5.tar", last modified: Tue Jul 18 07:04:21 2023, max compression
```

## Comparing `ndp-app-migration-0.4.tar` & `ndp-app-migration-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 05:58:34.007391 ndp-app-migration-0.4/
--rw-r--r--   0 harshal    (502) staff       (20)      961 2023-07-11 05:58:34.006932 ndp-app-migration-0.4/PKG-INFO
--rwxrwxr-x   0 harshal    (502) staff       (20)      492 2023-07-11 05:54:04.000000 ndp-app-migration-0.4/README.md
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 05:58:34.004751 ndp-app-migration-0.4/ndp_app_migration.egg-info/
--rw-r--r--   0 harshal    (502) staff       (20)      961 2023-07-11 05:58:33.000000 ndp-app-migration-0.4/ndp_app_migration.egg-info/PKG-INFO
--rw-r--r--   0 harshal    (502) staff       (20)      283 2023-07-11 05:58:33.000000 ndp-app-migration-0.4/ndp_app_migration.egg-info/SOURCES.txt
--rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-11 05:58:33.000000 ndp-app-migration-0.4/ndp_app_migration.egg-info/dependency_links.txt
--rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-11 05:58:33.000000 ndp-app-migration-0.4/ndp_app_migration.egg-info/requires.txt
--rw-r--r--   0 harshal    (502) staff       (20)       14 2023-07-11 05:58:33.000000 ndp-app-migration-0.4/ndp_app_migration.egg-info/top_level.txt
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-11 05:58:34.005425 ndp-app-migration-0.4/ndp_migration/
--rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-migration-0.4/ndp_migration/__init__.py
--rw-r--r--   0 harshal    (502) staff       (20)    10532 2023-07-11 05:55:13.000000 ndp-app-migration-0.4/ndp_migration/objects_migration.py
--rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-11 05:58:34.007516 ndp-app-migration-0.4/setup.cfg
--rwxrwxr-x   0 harshal    (502) staff       (20)     1438 2023-07-11 05:49:26.000000 ndp-app-migration-0.4/setup.py
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:04:21.084296 ndp-app-migration-0.5/
+-rw-r--r--   0 harshal    (502) staff       (20)      961 2023-07-18 07:04:21.083829 ndp-app-migration-0.5/PKG-INFO
+-rwxrwxr-x   0 harshal    (502) staff       (20)      492 2023-07-18 07:03:46.000000 ndp-app-migration-0.5/README.md
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:04:21.082659 ndp-app-migration-0.5/ndp_app_migration.egg-info/
+-rw-r--r--   0 harshal    (502) staff       (20)      961 2023-07-18 07:04:20.000000 ndp-app-migration-0.5/ndp_app_migration.egg-info/PKG-INFO
+-rw-r--r--   0 harshal    (502) staff       (20)      283 2023-07-18 07:04:20.000000 ndp-app-migration-0.5/ndp_app_migration.egg-info/SOURCES.txt
+-rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-18 07:04:20.000000 ndp-app-migration-0.5/ndp_app_migration.egg-info/dependency_links.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-18 07:04:20.000000 ndp-app-migration-0.5/ndp_app_migration.egg-info/requires.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       14 2023-07-18 07:04:20.000000 ndp-app-migration-0.5/ndp_app_migration.egg-info/top_level.txt
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:04:21.083337 ndp-app-migration-0.5/ndp_migration/
+-rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-migration-0.5/ndp_migration/__init__.py
+-rw-r--r--   0 harshal    (502) staff       (20)    10556 2023-07-18 07:03:27.000000 ndp-app-migration-0.5/ndp_migration/objects_migration.py
+-rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-18 07:04:21.084473 ndp-app-migration-0.5/setup.cfg
+-rwxrwxr-x   0 harshal    (502) staff       (20)     1438 2023-07-18 07:04:02.000000 ndp-app-migration-0.5/setup.py
```

### Comparing `ndp-app-migration-0.4/PKG-INFO` & `ndp-app-migration-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ndp-app-migration
-Version: 0.4
+Version: 0.5
 Summary: Data Objects Migration Mechanism for Zetaris Platform (https://www.zetaris.com/)
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
-pip3 install ndp-app-migration==0.4
+pip3 install ndp-app-migration==0.5
 
 from ndp_migration.objects_migration import migration_data_objects
 
 migration_data_objects(folder_path,key_decrypt,api_url,jar_file_name,option_for_backup,target_host,target_user_id,target_password,con_name,pipe_name,object_type)
 
 migration_data_objects(source_email_address, source_password, folder_path, source_api_url, option_for_backup,target_api_url, ,target_user_id,target_password,con_name,pipe_name,object_type)
```

### Comparing `ndp-app-migration-0.4/ndp_app_migration.egg-info/PKG-INFO` & `ndp-app-migration-0.5/ndp_app_migration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ndp-app-migration
-Version: 0.4
+Version: 0.5
 Summary: Data Objects Migration Mechanism for Zetaris Platform (https://www.zetaris.com/)
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
-pip3 install ndp-app-migration==0.4
+pip3 install ndp-app-migration==0.5
 
 from ndp_migration.objects_migration import migration_data_objects
 
 migration_data_objects(folder_path,key_decrypt,api_url,jar_file_name,option_for_backup,target_host,target_user_id,target_password,con_name,pipe_name,object_type)
 
 migration_data_objects(source_email_address, source_password, folder_path, source_api_url, option_for_backup,target_api_url, ,target_user_id,target_password,con_name,pipe_name,object_type)
```

### Comparing `ndp-app-migration-0.4/ndp_migration/objects_migration.py` & `ndp-app-migration-0.5/ndp_migration/objects_migration.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 def clear_query_cache(username:str):
     auth = get_auth()
     requests.delete(url=f'{api_url}/api/v1.0/query/sql/clear/{username}',headers=auth)
 #----------------------------------------#
 #GET ORD ID FROM EMAIL
 def get_org_id_from_email(lightning_username):
-    orgId_query = 'select id from metastore.organisation where lower(trim(email))='+"\'"+str(lightning_username)+"\'"
+    orgId_query = 'select fk_organisation_id as id from metastore.lightning_user where lower(trim(email))='+"\'"+str(lightning_username)+"\'"
     x = open_sql_query(orgId_query,100)
     orgid_dict = x['records']
     if isinstance(orgid_dict[0],dict):
         orgId = orgid_dict[0]['id']
     return orgId
 #----------------------------------------#
 def run_fetch_metastore(api_url,lightning_username,lightning_pass,folder_path,option_for_backup,container_name,object_name):
```

### Comparing `ndp-app-migration-0.4/setup.py` & `ndp-app-migration-0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
   
 setuptools.setup(
     # Here is the module name.
     name="ndp-app-migration",
   
     # version of the module
-    version="0.4",
+    version="0.5",
   
     # Name of Author
     author="Harshal Shah",
 
     #License
     license="Proprietary",
```

