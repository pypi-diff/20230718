# Comparing `tmp/hyfi_template-0.4.6.tar.gz` & `tmp/hyfi_template-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.4.6.tar", max compression
+gzip compressed data, was "hyfi_template-0.4.7.tar", max compression
```

## Comparing `hyfi_template-0.4.6.tar` & `hyfi_template-0.4.7.tar`

### file list

```diff
@@ -1,50 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-07-16 11:31:03.338362 hyfi_template-0.4.6/LICENSE
--rw-r--r--   0        0        0     2215 2023-07-16 11:31:03.338362 hyfi_template-0.4.6/README.md
--rw-r--r--   0        0        0     3012 2023-07-16 11:31:32.898674 hyfi_template-0.4.6/pyproject.toml
--rw-r--r--   0        0        0      286 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/__init__.py
--rw-r--r--   0        0        0       22 2023-07-16 11:31:32.838673 hyfi_template-0.4.6/src/hyfit/_version.py
--rw-r--r--   0        0        0        0 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/__init__.py
--rw-r--r--   0        0        0      249 2023-07-16 11:31:32.838673 hyfi_template-0.4.6/src/hyfit/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      969 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/path/__init__.yaml
--rw-r--r--   0        0        0      125 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/project/__init__.yaml
--rw-r--r--   0        0        0      160 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      298 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/task/__init__.yaml
--rw-r--r--   0        0        0      183 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/task/__test__.yaml
--rw-r--r--   0        0        0      124 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0      148 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-07-16 11:31:03.342362 hyfi_template-0.4.6/src/hyfit/py.typed
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 hyfi_template-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-18 09:11:25.541863 hyfi_template-0.4.7/LICENSE
+-rw-r--r--   0        0        0     2215 2023-07-18 09:11:25.541863 hyfi_template-0.4.7/README.md
+-rw-r--r--   0        0        0     3013 2023-07-18 09:12:04.078076 hyfi_template-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/__cli__.py
+-rw-r--r--   0        0        0      438 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-18 09:12:04.006076 hyfi_template-0.4.7/src/hyfit/_version.py
+-rw-r--r--   0        0        0        0 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-18 09:12:04.006076 hyfi_template-0.4.7/src/hyfit/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      159 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/config.yaml
+-rw-r--r--   0        0        0      662 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/copier/__init__.yaml
+-rw-r--r--   0        0        0      709 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      926 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      846 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/__init__.yaml
+-rw-r--r--   0        0        0       91 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      286 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      424 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0       69 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      746 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       38 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      329 2023-07-18 09:11:25.545863 hyfi_template-0.4.7/src/hyfit/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      124 2023-07-18 09:11:25.549863 hyfi_template-0.4.7/src/hyfit/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-18 09:11:25.549863 hyfi_template-0.4.7/src/hyfit/py.typed
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 hyfi_template-0.4.7/PKG-INFO
```

### Comparing `hyfi_template-0.4.6/LICENSE` & `hyfi_template-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.6/README.md` & `hyfi_template-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.6/pyproject.toml` & `hyfi_template-0.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.4.6"
+version = "0.4.7"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfit", from = "src" }]
 
 [tool.poetry.scripts]
 hyfit = 'hyfit.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.2.8"
+hyfi = "^1.2.14"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi_template-0.4.6/src/hyfit/conf/batch/__init__.yaml` & `hyfi_template-0.4.7/src/hyfit/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.6/src/hyfit/conf/copier/conf.yaml` & `hyfi_template-0.4.7/src/hyfit/conf/copier/__init__.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 # Filetypes to copy.
 filetypes:
   - yaml
   - yml
   - py
 # User-chosen additional file exclusion patterns.
 exclude:
-# User-chosen additional file skip patterns.
+# If `True`, exclude files that match the patterns for testing. (default: True)
+exclude_test_files: true
+# Skip files that already exist?
 skip_if_exists: false
 # Delete `dst_path` if there's an error?
 cleanup_on_error: false
 # When `True`, Overwrite files that already exist, without asking.
 overwrite: false
 # When `True`, produce no real rendering.
 dry_run: false
```

### Comparing `hyfi_template-0.4.6/src/hyfit/conf/dotenv/__init__.yaml` & `hyfi_template-0.4.7/src/hyfit/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.6/src/hyfit/conf/hydra/help/help.yaml` & `hyfi_template-0.4.7/src/hyfit/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.6/src/hyfit/conf/mode/__init__.yaml` & `hyfi_template-0.4.7/src/hyfit/conf/mode/__init__.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # @package _global_
 debug_mode: false
 resolve: true
 verbose: false
 ignore_warnings: true
-logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
-hydra_log_dir: ${oc.select:project.global_hyfi_root, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}}/${oc.select:project.global_workspace_name, ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}}/logs/hydra
+logging_level: WARNING
+hydra_log_dir: ${oc.select:project.global_hyfi_root, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}}/${oc.select:project.global_workspace_name, ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}}/logs/hydra
 
 hydra:
   job:
-    name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}}
+    name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi}}}
     chdir: true
   run:
     dir: ${hydra_log_dir}/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
   sweep:
     dir: ${hydra_log_dir}/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
     subdir: ${hydra.job.num}
   verbose: false
```

### Comparing `hyfi_template-0.4.6/src/hyfit/conf/path/__init__.yaml` & `hyfi_template-0.4.7/src/hyfit/conf/path/__init__.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -5,13 +5,13 @@
   - dirnames: __init__
 
 home: ${__home_path__:}
 hyfi: ${__hyfi_path__:}
 resources: ${alt:${oc.env:HYFI_RESOURCE_DIR,null},${.hyfi}/resources}
 runtime: ${get_original_cwd:}
 # global paths
-global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}}
-global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}}
+global_hyfi_root: ${oc.select:..global_hyfi_root,${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}}
+global_workspace_name: ${oc.select:..global_workspace_name,${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}}
 # project specific paths
-project_name: ${oc.select:..project_name,${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}
+project_name: ${oc.select:..project_name,${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi}}
 project_root: ${oc.select:..project_root,${alt:${oc.env:HYFI_PROJECT_ROOT,null},${get_original_cwd:}}}
-project_workspace_name: ${oc.select:..project_workspace_name,${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}}
+project_workspace_name: ${oc.select:..project_workspace_name,${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},workspace}}
```

### Comparing `hyfi_template-0.4.6/src/hyfit/conf/project/__init__.yaml` & `hyfi_template-0.4.7/src/hyfit/conf/project/__init__.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 defaults:
   - /dotenv: __init__
   - /joblib: __init__
   - /path: __init__
 
 _config_name_: __init__
-project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}
+project_name: ${alt:${oc.env:HYFI_PROJECT_NAME,null},${oc.select:about.__package_name__,hyfi}}
 project_description: ${oc.env:HYFI_PROJECT_DESC,""}
 project_root: ${alt:${oc.env:HYFI_PROJECT_ROOT,null},${.global_hyfi_root}/${.global_workspace_name}/projects/${.project_name}}
-project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},${.global_workspace_name}}
-global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}
-global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}
+project_workspace_name: ${alt:${oc.env:HYFI_PROJECT_WORKSPACE_NAME,null},workspace}
+global_hyfi_root: ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}}
+global_workspace_name: ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},.hyfi}
 num_workers: ${oc.env:HYFI_NUM_WORKERS,1}
 use_huggingface_hub: false
 use_wandb: false
 verbose: ${alt:${oc.env:HYFI_VERBOSE,null},false}
```

### Comparing `hyfi_template-0.4.6/PKG-INFO` & `hyfi_template-0.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.4.6
+Version: 0.4.7
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=1.2.8,<2.0.0)
+Requires-Dist: hyfi (>=1.2.14,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-template
 Description-Content-Type: text/markdown
 
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

