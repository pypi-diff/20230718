# Comparing `tmp/azureml-assets-1.5.2.tar.gz` & `tmp/azureml-assets-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azureml-assets-1.5.2.tar", last modified: Mon Jul 17 14:36:55 2023, max compression
+gzip compressed data, was "azureml-assets-1.6.0.tar", last modified: Tue Jul 18 15:52:45 2023, max compression
```

## Comparing `azureml-assets-1.5.2.tar` & `azureml-assets-1.6.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.732984 azureml-assets-1.5.2/azureml/
--rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.736984 azureml-assets-1.5.2/azureml/assets/
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/asset_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/copy_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/deployment_config.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.740984 azureml-assets-1.5.2/azureml/assets/environment/
--rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17109 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/build.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/pin_image_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/pin_package_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/environment/pin_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/extract_tagged_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.740984 azureml-assets-1.5.2/azureml/assets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/model/mlflow_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/model/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/tag_released_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11282 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/update_assets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/update_spec.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/azureml/assets/util/
--rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/template.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15565 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/util/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17280 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/azureml/assets/validate_assets.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-17 14:36:55.744984 azureml-assets-1.5.2/azureml_assets.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-17 14:36:55.000000 azureml-assets-1.5.2/azureml_assets.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-17 14:36:55.748984 azureml-assets-1.5.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-17 14:36:15.000000 azureml-assets-1.5.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 15:52:45.982920 azureml-assets-1.6.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-18 15:52:45.982920 azureml-assets-1.6.0/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 15:52:45.978920 azureml-assets-1.6.0/azureml/
+-rw-r--r--   0 vsts      (1001) docker     (123)       75 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 15:52:45.978920 azureml-assets-1.6.0/azureml/assets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4119 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/asset_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    36392 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7115 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/copy_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8518 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/deployment_config.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 15:52:45.982920 azureml-assets-1.6.0/azureml/assets/environment/
+-rw-r--r--   0 vsts      (1001) docker     (123)      244 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/environment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17109 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/environment/build.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6900 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/environment/pin_image_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5124 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/environment/pin_package_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/environment/pin_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4436 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/extract_tagged_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 15:52:45.982920 azureml-assets-1.6.0/azureml/assets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      155 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1187 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/model/mlflow_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3408 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/model/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2869 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/tag_released_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12150 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/update_assets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5934 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/update_spec.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 15:52:45.982920 azureml-assets-1.6.0/azureml/assets/util/
+-rw-r--r--   0 vsts      (1001) docker     (123)      533 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6906 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/util/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2564 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/util/template.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    15662 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/util/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17280 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/azureml/assets/validate_assets.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-18 15:52:45.982920 azureml-assets-1.6.0/azureml_assets.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      790 2023-07-18 15:52:45.000000 azureml-assets-1.6.0/azureml_assets.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      979 2023-07-18 15:52:45.000000 azureml-assets-1.6.0/azureml_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-18 15:52:45.000000 azureml-assets-1.6.0/azureml_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       78 2023-07-18 15:52:45.000000 azureml-assets-1.6.0/azureml_assets.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        8 2023-07-18 15:52:45.000000 azureml-assets-1.6.0/azureml_assets.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-18 15:52:45.982920 azureml-assets-1.6.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1275 2023-07-18 15:52:08.000000 azureml-assets-1.6.0/setup.py
```

### Comparing `azureml-assets-1.5.2/PKG-INFO` & `azureml-assets-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.5.2
+Version: 1.6.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.5.2/azureml/assets/__init__.py` & `azureml-assets-1.6.0/azureml/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/asset_utils.py` & `azureml-assets-1.6.0/azureml/assets/asset_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/config.py` & `azureml-assets-1.6.0/azureml/assets/config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/copy_assets.py` & `azureml-assets-1.6.0/azureml/assets/copy_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/deployment_config.py` & `azureml-assets-1.6.0/azureml/assets/deployment_config.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/environment/build.py` & `azureml-assets-1.6.0/azureml/assets/environment/build.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/environment/pin_image_versions.py` & `azureml-assets-1.6.0/azureml/assets/environment/pin_image_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/environment/pin_package_versions.py` & `azureml-assets-1.6.0/azureml/assets/environment/pin_package_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/environment/pin_versions.py` & `azureml-assets-1.6.0/azureml/assets/environment/pin_versions.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/extract_tagged_assets.py` & `azureml-assets-1.6.0/azureml/assets/extract_tagged_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/model/mlflow_utils.py` & `azureml-assets-1.6.0/azureml/assets/model/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/model/utils.py` & `azureml-assets-1.6.0/azureml/assets/model/utils.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/tag_released_assets.py` & `azureml-assets-1.6.0/azureml/assets/tag_released_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/update_assets.py` & `azureml-assets-1.6.0/azureml/assets/update_assets.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,144 +85,144 @@
     latest_tag = ordered_tags[-1].name
     _, _, latest_version = assets.AssetConfig.parse_full_name(latest_tag)
 
     return latest_version
 
 
 def update_asset(asset_config: assets.AssetConfig,
-                 release_directory_root: Path,
-                 copy_only: bool,
-                 skip_unreleased: bool,
-                 output_directory_root: Path = None) -> str:
+                 output_directory_root: Path,
+                 release_directory_root: Path = None,
+                 skip_unreleased: bool = False,
+                 use_version_dir: bool = False) -> str:
     """Update asset to prepare for release.
 
     Args:
         asset_config (assets.AssetConfig): Asset config
-        release_directory_root (Path): Release branch location
-        copy_only (bool): Only copy assets, don't actually update
-        skip_unreleased (bool): Skip unreleased explicitly-versioned assets
-        output_directory_root (Path, optional): Output directory for updated assets, otherwise update them in-place
+        output_directory_root (Path): Output directory for updated assets
+        release_directory_root (Path, optional): Release branch location
+        skip_unreleased (bool, optional): Skip unreleased explicitly-versioned assets. Defaults to False.
+        use_version_dir (bool, optional): Use version directory for output. Defaults to False.
 
     Returns:
         str: Version of updated asset, or None if not updated
     """
-    # Determine asset's release directory
-    release_dir = util.get_asset_release_dir(asset_config, release_directory_root)
-
-    # Define output directory, which may be different from the release directory
-    if output_directory_root:
-        output_directory = util.get_asset_output_dir(asset_config, output_directory_root)
-    else:
-        output_directory = release_dir
-
-    # Simpler operation that just copies the directory
-    if copy_only:
-        util.copy_asset_to_output_dir(asset_config=asset_config, output_directory=output_directory)
-        return asset_config.spec_as_object().version
-
-    # Get version from main branch, set a few defaults
-    main_version = asset_config.version
-    auto_version = asset_config.auto_version
-    release_version = None
-    check_contents = False
-    pending_release = False
-
-    # Check existing release dir
-    if release_dir.exists():
-        release_asset_configs = util.find_assets(input_dirs=release_dir,
-                                                 asset_config_filename=asset_config.file_name)
-        if not release_asset_configs:
-            logger.log_error(f"Release directory {release_dir} exists, but it's missing an asset config file")
-            exit(1)
-        release_asset_config = release_asset_configs[0]
-        release_version = release_asset_config.version
-        check_contents = True
-
-        # See if the asset version is unreleased
-        pending_release = not release_tag_exists(release_asset_config, release_directory_root)
-        if pending_release and not auto_version and main_version != release_version and skip_unreleased:
-            # Skip the unreleased asset version
-            logger.log_warning(f"Skipping {release_asset_config.type.value} {release_asset_config.name} because "
-                               f"version {release_version} hasn't been released yet")
-            return None
-
-    # Determine new version
-    if not auto_version:
-        # Use explicit version
-        new_version = main_version
-    elif pending_release:
-        # Reuse existing auto version
-        new_version = release_version
-    else:
-        # Increment auto version
-        new_version = int(release_version) + 1 if release_version else 1
+    # The release directory is required if auto-versioning
+    if asset_config.auto_version and release_directory_root is None:
+        logger.log_error(f"Asset {asset_config.name} is auto-versioned but can't be updated because no release "
+                         "directory was specified to compare against")
+        exit(1)
+
+    # Identify output directory
+    output_is_release = (release_directory_root is not None and output_directory_root.exists()
+                         and output_directory_root.samefile(release_directory_root))
+    if output_is_release:
+        # Prevent release directory corruption
+        use_version_dir = False
+    output_directory = util.get_asset_output_dir(asset_config, output_directory_root, use_version_dir)
 
+    # To keep things simple, we'll create a temporary directory for each update
     with tempfile.TemporaryDirectory() as temp_dir:
         temp_dir_path = Path(temp_dir)
+
         # Copy asset to temp directory and pin image/package versions
-        util.copy_asset_to_output_dir(asset_config=asset_config, output_directory=temp_dir_path, add_subdir=True)
+        temp_asset_dir = util.copy_asset_to_output_dir(asset_config=asset_config, output_directory=temp_dir_path,
+                                                       add_subdir=True)
         temp_asset_config = util.find_assets(input_dirs=temp_dir_path, asset_config_filename=asset_config.file_name)[0]
         if temp_asset_config.type == assets.AssetType.ENVIRONMENT:
             temp_env_config = temp_asset_config.extra_config_as_object()
-            if temp_env_config:
-                pin_env_files(temp_env_config)
-
-        temp_asset_dir = util.get_asset_output_dir(asset_config=asset_config, output_directory_root=temp_dir_path)
+            pin_env_files(temp_env_config)
 
-        # Compare temporary version with one in release
-        if check_contents:
-            assets.update_spec(temp_asset_config, version=release_version)
-            dirs_equal = util.are_dir_trees_equal(temp_asset_dir, release_dir)
-            if dirs_equal:
+        # Get version info, set a few defaults
+        main_version = asset_config.version
+        auto_version = asset_config.auto_version
+        release_version = None
+        pending_release = False
+
+        # Look in release directory for existing asset
+        if release_directory_root is not None:
+            release_dir = util.get_asset_release_dir(asset_config, release_directory_root)
+            if release_dir.exists():
+                # Check existing release dir
+                release_asset_configs = util.find_assets(input_dirs=release_dir,
+                                                         asset_config_filename=asset_config.file_name)
+                if not release_asset_configs:
+                    logger.log_error(f"Release directory {release_dir} exists, but it's missing an asset config file")
+                    exit(1)
+                release_asset_config = release_asset_configs[0]
+                release_version = release_asset_config.version
+
+                # Compare temporary version with one in release
+                assets.update_spec(temp_asset_config, version=release_version)
+                dirs_equal = util.are_dir_trees_equal(temp_asset_dir, release_dir)
+                if dirs_equal:
+                    return None
+
+            # See if the asset version is unreleased
+            pending_release = not release_tag_exists(release_asset_config, release_directory_root)
+            if pending_release and not auto_version and main_version != release_version and skip_unreleased:
+                # Skip the unreleased asset version
+                logger.log_warning(f"Skipping {release_asset_config.type.value} {release_asset_config.name} because "
+                                   f"version {release_version} hasn't been released yet")
                 return None
 
+        # Determine new version
+        if not auto_version:
+            # Use explicit version
+            new_version = main_version
+        elif pending_release:
+            # Reuse existing auto version
+            new_version = release_version
+        else:
+            # Increment auto version
+            new_version = int(release_version) + 1 if release_version else 1
+
         # Copy and replace any existing directory
         util.copy_replace_dir(source=temp_asset_dir, dest=output_directory)
 
         # Update version in spec by copying clean spec and updating it
         asset_config_relative_path = temp_asset_config.file_name_with_path.relative_to(temp_asset_dir)
         output_asset_config = assets.AssetConfig(output_directory / asset_config_relative_path)
         shutil.copyfile(asset_config.spec_with_path, output_asset_config.spec_with_path)
         assets.update_spec(output_asset_config, version=str(new_version))
 
         return new_version
 
 
 def update_assets(input_dirs: List[Path],
                   asset_config_filename: str,
-                  release_directory_root: Path,
-                  copy_only: bool,
-                  skip_unreleased: bool,
-                  output_directory_root: Path = None):
+                  output_directory_root: Path,
+                  release_directory_root: Path = None,
+                  skip_unreleased: bool = False,
+                  use_version_dirs: bool = False):
     """Update assets to prepare for release.
 
     Args:
         input_dirs (List[Path]): List of directories to search for assets.
         asset_config_filename (str): Asset config filename to search for
-        release_directory_root (Path): Release directory location
-        copy_only (bool): Only copy assets, don't actually update
-        skip_unreleased (bool): Skip unreleased explicitly-versioned assets
-        output_directory_root (Path, optional): Output directory for updated assets, otherwise update them in-place
+        output_directory_root (Path): Output directory for updated assets
+        release_directory_root (Path, optional): Release directory location
+        skip_unreleased (bool, optional): Skip unreleased explicitly-versioned assets. Defaults to False.
+        use_version_dirs (bool, optional): Use version directories for output. Defaults to False.
     """
     # Find assets under input dirs
     counters = Counter()
     for asset_config in util.find_assets(input_dirs, asset_config_filename):
         counters[ASSET_COUNT] += 1
 
         # Update asset if it's changed
         new_version = update_asset(asset_config=asset_config,
+                                   output_directory_root=output_directory_root,
                                    release_directory_root=release_directory_root,
-                                   copy_only=copy_only,
                                    skip_unreleased=skip_unreleased,
-                                   output_directory_root=output_directory_root)
+                                   use_version_dir=use_version_dirs)
         if new_version:
             logger.print(f"Updated {asset_config.type.value} {asset_config.name} version {new_version}")
             counters[UPDATED_COUNT] += 1
 
-            # Track updated environments by OS
+            # Track updated environments
             if asset_config.type == assets.AssetType.ENVIRONMENT:
                 counters[UPDATED_ENV_COUNT] += 1
         else:
             logger.log_debug(f"No changes detected for {asset_config.type.value} {asset_config.name}")
     logger.print(f"{counters[UPDATED_COUNT]} of {counters[ASSET_COUNT]} asset(s) updated")
 
     # Set variables
@@ -233,27 +233,32 @@
 if __name__ == '__main__':
     # Handle command-line args
     parser = argparse.ArgumentParser()
     parser.add_argument("-i", "--input-dirs", required=True,
                         help="Comma-separated list of directories containing assets")
     parser.add_argument("-a", "--asset-config-filename", default=assets.DEFAULT_ASSET_FILENAME,
                         help="Asset config file name to search for")
-    parser.add_argument("-r", "--release-directory", required=True, type=Path,
-                        help="Directory to which the release branch has been cloned")
-    parser.add_argument("-o", "--output-directory", type=Path,
-                        help="Directory to which new/updated assets will be written, defaults to release directory")
-    parser.add_argument("-c", "--copy-only", action="store_true",
-                        help="Just copy assets into the release directory")
+    parser.add_argument("-o", "--output-directory", required=True, type=Path,
+                        help="Copy new/updated assets into this directory, can be the same as --release-directory")
+    parser.add_argument("-r", "--release-directory", type=Path,
+                        help="Directory to which the release branch has been cloned; if specified, only unreleased "
+                        "and updated assets will be copied to the output directory")
     parser.add_argument("-s", "--skip-unreleased", action="store_true",
                         help="Skip unreleased explicitly-versioned assets in the release branch")
+    parser.add_argument("-v", "--use-version-dirs", action="store_true",
+                        help="Use version directories when storing assets in output directory")
     args = parser.parse_args()
 
+    # Check interdependencies
+    if args.skip_unreleased and args.release_directory is None:
+        parser.error("--skip-unreleased requires --release-directory")
+
     # Convert comma-separated values to lists
     input_dirs = [Path(d) for d in args.input_dirs.split(",")]
 
     # Update assets
     update_assets(input_dirs=input_dirs,
                   asset_config_filename=args.asset_config_filename,
+                  output_directory_root=args.output_directory,
                   release_directory_root=args.release_directory,
-                  copy_only=args.copy_only,
                   skip_unreleased=args.skip_unreleased,
-                  output_directory_root=args.output_directory)
+                  use_version_dirs=args.use_version_dirs)
```

### Comparing `azureml-assets-1.5.2/azureml/assets/update_spec.py` & `azureml-assets-1.6.0/azureml/assets/update_spec.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/util/__init__.py` & `azureml-assets-1.6.0/azureml/assets/util/__init__.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/util/logger.py` & `azureml-assets-1.6.0/azureml/assets/util/logger.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/util/template.py` & `azureml-assets-1.6.0/azureml/assets/util/template.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml/assets/util/util.py` & `azureml-assets-1.6.0/azureml/assets/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,30 +180,34 @@
     Returns:
         Path: The release directory
     """
     return get_asset_output_dir_from_parts(type, name, release_directory_root / RELEASE_SUBDIR)
 
 
 def copy_asset_to_output_dir(asset_config: assets.AssetConfig, output_directory: Path, add_subdir: bool = False,
-                             use_version_dir: bool = False):
+                             use_version_dir: bool = False) -> Path:
     """Copy asset directory to output directory.
 
     Args:
         asset_config (assets.AssetConfig): Asset config to copy
         output_directory_root (Path): Output directory root
         add_subdir (bool, optional): Add asset-specific subdirectories to output_directory
         use_version_dir (bool, optional): Store asset in version-specific directory
+
+    Returns:
+        Path: The asset's output directory
     """
     if add_subdir:
         output_directory = get_asset_output_dir(asset_config, output_directory, use_version_dir)
     elif use_version_dir:
         output_directory = output_directory / asset_config.version
 
     common_dir, relative_release_paths = find_common_directory(asset_config.release_paths)
     copy_replace_dir(source=common_dir, dest=output_directory, paths=relative_release_paths)
+    return output_directory
 
 
 def apply_tag_template(full_image_name: str, template: str = None) -> str:
     """Apply a template to an image's tag.
 
     Args:
         full_image_name (str): The full image name, which must include a tag suffix.
```

### Comparing `azureml-assets-1.5.2/azureml/assets/validate_assets.py` & `azureml-assets-1.6.0/azureml/assets/validate_assets.py`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/azureml_assets.egg-info/PKG-INFO` & `azureml-assets-1.6.0/azureml_assets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azureml-assets
-Version: 1.5.2
+Version: 1.6.0
 Summary: Utilities for publishing assets to Azure Machine Learning system registries.
 Author: Microsoft Corp
 License: MIT
 Project-URL: Source, https://github.com/Azure/azureml-assets/
 Project-URL: Changelog, https://github.com/Azure/azureml-assets/blob/main/scripts/azureml-assets/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `azureml-assets-1.5.2/azureml_assets.egg-info/SOURCES.txt` & `azureml-assets-1.6.0/azureml_assets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `azureml-assets-1.5.2/setup.py` & `azureml-assets-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Set up azureml-assets package."""
 
 from setuptools import setup, find_packages
 
 setup(
    name="azureml-assets",
-   version="1.5.2",
+   version="1.6.0",
    description="Utilities for publishing assets to Azure Machine Learning system registries.",
    author="Microsoft Corp",
    packages=find_packages(),
    install_requires=[
       "GitPython>=3.1",
       "ruamel.yaml==0.17.21",
       "pip>=21",
```

