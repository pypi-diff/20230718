# Comparing `tmp/irisml-tasks-azureml-0.1.4.tar.gz` & `tmp/irisml-tasks-azureml-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azureml-0.1.4.tar", last modified: Fri May 19 06:09:56 2023, max compression
+gzip compressed data, was "irisml-tasks-azureml-0.1.5.tar", last modified: Tue Jul 18 06:07:12 2023, max compression
```

## Comparing `irisml-tasks-azureml-0.1.4.tar` & `irisml-tasks-azureml-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.492418 irisml-tasks-azureml-0.1.4/irisml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.492418 irisml-tasks-azureml-0.1.4/irisml/azureml/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/azureml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/azureml/azureml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.492418 irisml-tasks-azureml-0.1.4/irisml/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/commands/cancel_aml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/commands/run_aml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/irisml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/tasks/add_aml_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/irisml/tasks/run_azureml_child.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-19 06:09:56.000000 irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 06:09:56.496418 irisml-tasks-azureml-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/test/test_add_aml_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-19 06:07:12.000000 irisml-tasks-azureml-0.1.4/test/test_azureml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/irisml/azureml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/irisml/azureml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/irisml/azureml/azureml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/irisml/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/irisml/commands/cancel_aml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/irisml/commands/run_aml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/irisml/tasks/add_aml_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/irisml/tasks/run_azureml_child.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-18 06:07:12.000000 irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-18 06:07:12.000000 irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:07:12.000000 irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 06:07:12.000000 irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 06:07:12.000000 irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 06:07:12.000000 irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:07:12.297009 irisml-tasks-azureml-0.1.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/test/test_add_aml_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-18 06:04:42.000000 irisml-tasks-azureml-0.1.5/test/test_azureml.py
```

### Comparing `irisml-tasks-azureml-0.1.4/LICENSE` & `irisml-tasks-azureml-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.4/PKG-INFO` & `irisml-tasks-azureml-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azureml
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utility tools to use IrisML on AzureML
 Home-page: https://github.com/microsoft/irisml-tasks-azureml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,15 +18,15 @@
 pip install irisml-tasks-azureml
 ```
 
 ## Available commands
 ```bash
 irisml_run_aml [-h] [--env ENV] [--no_cache] [--include_local_tasks [INCLUDE_LOCAL_TASKS]] [--custom_packages CUSTOM_PACKAGES [CUSTOM_PACKAGES ...]]
                       [--extra_index_url EXTRA_INDEX_URL] [--no_wait] [--compute_target COMPUTE_TARGET] [--subscription_id SUBSCRIPTION_ID] [--workspace WORKSPACE] [--experiment EXPERIMENT]
-                      [--base_docker_image BASE_DOCKER_IMAGE] [--base_docker_image_registry BASE_DOCKER_IMAGE_REGISTRY] [--use_sp_on_remote]
+                      [--base_docker_image BASE_DOCKER_IMAGE] [--base_docker_image_registry BASE_DOCKER_IMAGE_REGISTRY] [--use_sp_on_remote] [-vv]
                       job_filepath
 ```
 This command submits an experiment to a remote AzureML node.
 
 If --include_local_tasks option is used, python scripts in the current directory or the specified directory will be sent to AzureML and be loaded as custom tasks.
 
 If environment variable AZURE_TENANT_ID, AZURE_CLIENT_ID, and AZURE_CLIENT_SECRET are set, this command will use ServicePrincipalAuthentication. Otherwise, the AzureML's default authentication method will be used.
```

### Comparing `irisml-tasks-azureml-0.1.4/README.md` & `irisml-tasks-azureml-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 pip install irisml-tasks-azureml
 ```
 
 ## Available commands
 ```bash
 irisml_run_aml [-h] [--env ENV] [--no_cache] [--include_local_tasks [INCLUDE_LOCAL_TASKS]] [--custom_packages CUSTOM_PACKAGES [CUSTOM_PACKAGES ...]]
                       [--extra_index_url EXTRA_INDEX_URL] [--no_wait] [--compute_target COMPUTE_TARGET] [--subscription_id SUBSCRIPTION_ID] [--workspace WORKSPACE] [--experiment EXPERIMENT]
-                      [--base_docker_image BASE_DOCKER_IMAGE] [--base_docker_image_registry BASE_DOCKER_IMAGE_REGISTRY] [--use_sp_on_remote]
+                      [--base_docker_image BASE_DOCKER_IMAGE] [--base_docker_image_registry BASE_DOCKER_IMAGE_REGISTRY] [--use_sp_on_remote] [-vv]
                       job_filepath
 ```
 This command submits an experiment to a remote AzureML node.
 
 If --include_local_tasks option is used, python scripts in the current directory or the specified directory will be sent to AzureML and be loaded as custom tasks.
 
 If environment variable AZURE_TENANT_ID, AZURE_CLIENT_ID, and AZURE_CLIENT_SECRET are set, this command will use ServicePrincipalAuthentication. Otherwise, the AzureML's default authentication method will be used.
```

### Comparing `irisml-tasks-azureml-0.1.4/irisml/azureml/azureml.py` & `irisml-tasks-azureml-0.1.5/irisml/azureml/azureml.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,32 +104,35 @@
 
     def cancel(self, run_id: str):
         run = azureml.core.run.get_run(self._experiment, run_id)
         run.cancel()
 
 
 class Job:
-    def __init__(self, job_description_filepath: pathlib.Path, environment_variables: typing.Dict):
+    def __init__(self, job_description_filepath: pathlib.Path, environment_variables: typing.Dict, very_verbose=False):
         # Check if the given file is a valid JobDescription
         job_description_dict = json.loads(job_description_filepath.read_text())
         job_description = JobDescription.from_dict(job_description_dict)
         if job_description is None:
             raise RuntimeError(f"The given file is not a valid job description: {job_description_filepath}")
 
         self._job_description_filepath = job_description_filepath
         self._environment_variables = environment_variables
+        self._very_verbose = very_verbose
         self._custom_task_relative_paths = []
 
     @property
     def name(self):
         return self._job_description_filepath.name
 
     @property
     def command(self):
         c = f'irisml_run {self.name} -v'
+        if self._very_verbose:
+            c += ' -vv'
         for key, value in self._environment_variables.items():
             c += f' -e {key}="{value}"'
         if self._custom_task_relative_paths:  # Add the current directory to PYTHONPATH so that the custom tasks can be loaded.
             c = 'PYTHONPATH=.:$PYTHONPATH ' + c
         return c
 
     def add_custom_tasks(self, tasks_dir: pathlib.Path):
```

### Comparing `irisml-tasks-azureml-0.1.4/irisml/commands/cancel_aml.py` & `irisml-tasks-azureml-0.1.5/irisml/commands/cancel_aml.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.4/irisml/commands/run_aml.py` & `irisml-tasks-azureml-0.1.5/irisml/commands/run_aml.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     parser.add_argument('--subscription_id', default=os.getenv('IRISML_AML_SUBSCRIPTION_ID'))
     parser.add_argument('--workspace', default=os.getenv('IRISML_AML_WORKSPACE_NAME'))
     parser.add_argument('--experiment', default=os.getenv('IRISML_AML_EXPERIMENT_NAME', 'irisml'))
     parser.add_argument('--base_docker_image')
     parser.add_argument('--base_docker_image_registry')
     parser.add_argument('--no_docker_build_date_label', action='store_true')
     parser.add_argument('--use_sp_on_remote', '--sp', action='store_true', help="Use Service Principal id and secret on the AML job.")
+    parser.add_argument('--very_verbose', '-vv', action='store_true')
 
     args = parser.parse_args()
 
     if not args.workspace:
         parser.error("Workspace name is required. Please set IRISML_AML_WORKSPACE_NAME or use --workspace option.")
     if not args.subscription_id:
         parser.error("Subscription ID is required. Please set IRISML_AML_SUBSCRIPTION_ID or use --subscription_id option.")
@@ -48,15 +49,15 @@
 
     envs = args.env
     cache_url = os.getenv('IRISML_CACHE_URL') if not args.no_cache else None
     if cache_url and args.include_local_tasks:
         logger.warning("Cache is disabled since local task implementations are used.")
         cache_url = None
 
-    job = Job(args.job_filepath, envs)
+    job = Job(args.job_filepath, envs, very_verbose=args.very_verbose)
     if args.include_local_tasks:
         job.add_custom_tasks(args.include_local_tasks)
 
     custom_packages = args.custom_packages
     if args.requirement:
         custom_packages = custom_packages + args.requirement.read_text().splitlines()
     env = JobEnvironment(args.base_docker_image, args.base_docker_image_registry, custom_packages, args.extra_index_url, not args.no_docker_build_date_label)
```

### Comparing `irisml-tasks-azureml-0.1.4/irisml/tasks/add_aml_tag.py` & `irisml-tasks-azureml-0.1.5/irisml/tasks/add_aml_tag.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/PKG-INFO` & `irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azureml
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utility tools to use IrisML on AzureML
 Home-page: https://github.com/microsoft/irisml-tasks-azureml
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,15 +18,15 @@
 pip install irisml-tasks-azureml
 ```
 
 ## Available commands
 ```bash
 irisml_run_aml [-h] [--env ENV] [--no_cache] [--include_local_tasks [INCLUDE_LOCAL_TASKS]] [--custom_packages CUSTOM_PACKAGES [CUSTOM_PACKAGES ...]]
                       [--extra_index_url EXTRA_INDEX_URL] [--no_wait] [--compute_target COMPUTE_TARGET] [--subscription_id SUBSCRIPTION_ID] [--workspace WORKSPACE] [--experiment EXPERIMENT]
-                      [--base_docker_image BASE_DOCKER_IMAGE] [--base_docker_image_registry BASE_DOCKER_IMAGE_REGISTRY] [--use_sp_on_remote]
+                      [--base_docker_image BASE_DOCKER_IMAGE] [--base_docker_image_registry BASE_DOCKER_IMAGE_REGISTRY] [--use_sp_on_remote] [-vv]
                       job_filepath
 ```
 This command submits an experiment to a remote AzureML node.
 
 If --include_local_tasks option is used, python scripts in the current directory or the specified directory will be sent to AzureML and be loaded as custom tasks.
 
 If environment variable AZURE_TENANT_ID, AZURE_CLIENT_ID, and AZURE_CLIENT_SECRET are set, this command will use ServicePrincipalAuthentication. Otherwise, the AzureML's default authentication method will be used.
```

### Comparing `irisml-tasks-azureml-0.1.4/irisml_tasks_azureml.egg-info/SOURCES.txt` & `irisml-tasks-azureml-0.1.5/irisml_tasks_azureml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.4/setup.cfg` & `irisml-tasks-azureml-0.1.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-azureml
-version = 0.1.4
+version = 0.1.5
 url = https://github.com/microsoft/irisml-tasks-azureml
 description = Utility tools to use IrisML on AzureML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
```

### Comparing `irisml-tasks-azureml-0.1.4/test/test_add_aml_tag.py` & `irisml-tasks-azureml-0.1.5/test/test_add_aml_tag.py`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azureml-0.1.4/test/test_azureml.py` & `irisml-tasks-azureml-0.1.5/test/test_azureml.py`

 * *Files identical despite different names*

