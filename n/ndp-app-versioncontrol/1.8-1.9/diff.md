# Comparing `tmp/ndp-app-versioncontrol-1.8.tar.gz` & `tmp/ndp-app-versioncontrol-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndp-app-versioncontrol-1.8.tar", last modified: Tue Jul 18 07:08:33 2023, max compression
+gzip compressed data, was "ndp-app-versioncontrol-1.9.tar", last modified: Tue Jul 18 07:22:53 2023, max compression
```

## Comparing `ndp-app-versioncontrol-1.8.tar` & `ndp-app-versioncontrol-1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:08:33.257080 ndp-app-versioncontrol-1.8/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-18 07:08:33.256520 ndp-app-versioncontrol-1.8/PKG-INFO
--rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-18 07:08:09.000000 ndp-app-versioncontrol-1.8/README.md
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:08:33.250496 ndp-app-versioncontrol-1.8/ndp_app_versioncontrol.egg-info/
--rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-18 07:08:33.000000 ndp-app-versioncontrol-1.8/ndp_app_versioncontrol.egg-info/PKG-INFO
--rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-18 07:08:33.000000 ndp-app-versioncontrol-1.8/ndp_app_versioncontrol.egg-info/SOURCES.txt
--rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-18 07:08:33.000000 ndp-app-versioncontrol-1.8/ndp_app_versioncontrol.egg-info/dependency_links.txt
--rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-18 07:08:33.000000 ndp-app-versioncontrol-1.8/ndp_app_versioncontrol.egg-info/requires.txt
--rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-18 07:08:33.000000 ndp-app-versioncontrol-1.8/ndp_app_versioncontrol.egg-info/top_level.txt
-drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:08:33.251584 ndp-app-versioncontrol-1.8/ndp_versioncontrol/
--rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.8/ndp_versioncontrol/__init__.py
--rwxrwxr-x   0 harshal    (502) staff       (20)    22915 2023-07-18 07:07:41.000000 ndp-app-versioncontrol-1.8/ndp_versioncontrol/generate_backup_sql.py
--rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-18 07:08:33.257376 ndp-app-versioncontrol-1.8/setup.cfg
--rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-18 07:07:57.000000 ndp-app-versioncontrol-1.8/setup.py
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:22:53.309254 ndp-app-versioncontrol-1.9/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-18 07:22:53.308782 ndp-app-versioncontrol-1.9/PKG-INFO
+-rwxrwxr-x   0 harshal    (502) staff       (20)      298 2023-07-18 07:22:37.000000 ndp-app-versioncontrol-1.9/README.md
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:22:53.306637 ndp-app-versioncontrol-1.9/ndp_app_versioncontrol.egg-info/
+-rw-r--r--   0 harshal    (502) staff       (20)      765 2023-07-18 07:22:53.000000 ndp-app-versioncontrol-1.9/ndp_app_versioncontrol.egg-info/PKG-INFO
+-rw-r--r--   0 harshal    (502) staff       (20)      320 2023-07-18 07:22:53.000000 ndp-app-versioncontrol-1.9/ndp_app_versioncontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 harshal    (502) staff       (20)        1 2023-07-18 07:22:53.000000 ndp-app-versioncontrol-1.9/ndp_app_versioncontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       65 2023-07-18 07:22:53.000000 ndp-app-versioncontrol-1.9/ndp_app_versioncontrol.egg-info/requires.txt
+-rw-r--r--   0 harshal    (502) staff       (20)       19 2023-07-18 07:22:53.000000 ndp-app-versioncontrol-1.9/ndp_app_versioncontrol.egg-info/top_level.txt
+drwxr-xr-x   0 harshal    (502) staff       (20)        0 2023-07-18 07:22:53.307364 ndp-app-versioncontrol-1.9/ndp_versioncontrol/
+-rw-r--r--   0 harshal    (502) staff       (20)        0 2021-07-15 08:59:23.000000 ndp-app-versioncontrol-1.9/ndp_versioncontrol/__init__.py
+-rwxrwxr-x   0 harshal    (502) staff       (20)    23091 2023-07-18 07:21:46.000000 ndp-app-versioncontrol-1.9/ndp_versioncontrol/generate_backup_sql.py
+-rw-r--r--   0 harshal    (502) staff       (20)       38 2023-07-18 07:22:53.309430 ndp-app-versioncontrol-1.9/setup.cfg
+-rwxrwxr-x   0 harshal    (502) staff       (20)     1436 2023-07-18 07:22:22.000000 ndp-app-versioncontrol-1.9/setup.py
```

### Comparing `ndp-app-versioncontrol-1.8/PKG-INFO` & `ndp-app-versioncontrol-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.8
+Version: 1.9
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
-pip3 install ndp-app-versioncontrol==1.8
+pip3 install ndp-app-versioncontrol==1.9
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.8/ndp_app_versioncontrol.egg-info/PKG-INFO` & `ndp-app-versioncontrol-1.9/ndp_app_versioncontrol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ndp-app-versioncontrol
-Version: 1.8
+Version: 1.9
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
-pip3 install ndp-app-versioncontrol==1.8
+pip3 install ndp-app-versioncontrol==1.9
 
 from ndp_versioncontrol.generate_backup_sql import object_versioncontrol
 
 object_versioncontrol(folder_path,user_email,user_password,api_url,backup_or_restore,data_object_type,data_object_container_name,data_object_name)
 
 ```
```

### Comparing `ndp-app-versioncontrol-1.8/ndp_versioncontrol/generate_backup_sql.py` & `ndp-app-versioncontrol-1.9/ndp_versioncontrol/generate_backup_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 def get_individual_pipelines(folder_path,lightning_username,lightning_pass,api_url):
     set_api_base_url(api_url)
     login(lightning_username,lightning_pass)
     logger.info('Backup of Pipelines at an individual level')
     orgId = get_org_id_from_email(lightning_username)
     sql_ind_pipeline="select r.name as rname,c.name as cname from metastore.pipeline_relation r inner join metastore.pipeline_container c on c.id=r.fk_pipeline_container_id where c.fk_organisation_id="+str(orgId).strip()
     res = exec_query_get_res(sql_ind_pipeline)
-    if isinstance(res[0],dict):
+    if isinstance(res, list) and len(res) > 0 and isinstance(res[0], dict):
         for dic in res:
             con_name=list(dic.values())[0]
             pipe_name=list(dic.values())[1]
             if (len(str(pipe_name))>1):
                 print(str(pipe_name)+'.'+str(con_name))
                 run_fetch_metastore(str(api_url),str(lightning_username),str(lightning_pass),str(folder_path).strip(),"2",str(pipe_name),str(con_name))
 
@@ -195,43 +195,43 @@
     set_api_base_url(api_url)
     login(lightning_username,lightning_pass)
     logger.info('Backup of Pipelines at container level')
     orgId = get_org_id_from_email(lightning_username)
     print(orgId)
     sql_query_pipeline="select name from metastore.pipeline_container where fk_organisation_id="+str(orgId).strip()
     res = exec_query_get_res(sql_query_pipeline)
-    if isinstance(res[0],dict):
+    if isinstance(res, list) and len(res) > 0 and isinstance(res[0], dict):
         for i in res:
             name = str(i['name'])
             print(name)
             run_fetch_metastore(str(api_url),str(lightning_username),str(lightning_pass),str(folder_path).strip(),"1",str(name),"")
 
 #BACKUP OF PERMANENT VIEWS
 def get_data_views(folder_path,lightning_username,lightning_pass,api_url):
     set_api_base_url(api_url)
     login(lightning_username,lightning_pass)
     logger.info('Backup of Permanent Views')
     orgId = get_org_id_from_email(lightning_username)
     sql_query_view="select name from metastore.schema_store_view where fk_organisation_id="+str(orgId).strip()
     res = exec_query_get_res(sql_query_view)
-    if isinstance(res[0],dict):
+    if isinstance(res, list) and len(res) > 0 and isinstance(res[0], dict):
         for i in res:
             name = str(i['name'])
             print(name)
             run_fetch_metastore(str(api_url),str(lightning_username),str(lightning_pass),str(folder_path).strip(),"7",str(name),"")
 
 #BACKUP OF DATA MARTS AT CONTAINER LEVEL
 def get_data_marts(folder_path,lightning_username,lightning_pass,api_url):
     set_api_base_url(api_url)
     login(lightning_username,lightning_pass)
     logger.info('Backup of Data Marts')
     orgId = get_org_id_from_email(lightning_username)
     sql_query_mart="select name from metastore.data_mart where fk_organisation_id="+str(orgId).strip()
     res = exec_query_get_res(sql_query_mart)
-    if isinstance(res[0],dict):
+    if isinstance(res, list) and len(res) > 0 and isinstance(res[0], dict):
         for i in res:
             name = str(i['name'])
             print(name)
             run_fetch_metastore(str(api_url),str(lightning_username),str(lightning_pass),str(folder_path).strip(),"5",str(name),"")
 #----------------------------------------#
 #GENERATE FILE NAME FOR RESTORE FUCNTIONALITY
 def generate_file_name(arg1,arg2,object_type,type_of_restore,folder_path,api_url):
```

### Comparing `ndp-app-versioncontrol-1.8/setup.py` & `ndp-app-versioncontrol-1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
   
 setuptools.setup(
     # Here is the module name.
     name="ndp-app-versioncontrol",
   
     # version of the module
-    version="1.8",
+    version="1.9",
   
     # Name of Author
     author="Harshal Shah",
 
     #License
     license="Proprietary",
```

