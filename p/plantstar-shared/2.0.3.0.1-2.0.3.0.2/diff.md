# Comparing `tmp/plantstar-shared-2.0.3.0.1.tar.gz` & `tmp/plantstar-shared-2.0.3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantstar-shared-2.0.3.0.1.tar", last modified: Mon May 22 19:09:01 2023, max compression
+gzip compressed data, was "plantstar-shared-2.0.3.0.2.tar", last modified: Mon May 22 19:11:52 2023, max compression
```

## Comparing `plantstar-shared-2.0.3.0.1.tar` & `plantstar-shared-2.0.3.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:09:01.155114 plantstar-shared-2.0.3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 19:09:01.155114 plantstar-shared-2.0.3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:09:01.155114 plantstar-shared-2.0.3.0.1/plantstar_shared/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/DataCollectionModuleProcessNames.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/HuskyInterfacePacketTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/MockRawDataProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/RawDataProcessorInterfaceActions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/SysconType.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/add_size_onto_string_and_return.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/api_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/convert_bytes_to_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/convert_object_to_bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/global_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/is_valid_signed_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/syscon_image_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/syscon_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/plantstar_shared/tcp_socket_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:09:01.155114 plantstar-shared-2.0.3.0.1/plantstar_shared.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 19:09:01.000000 plantstar-shared-2.0.3.0.1/plantstar_shared.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-22 19:09:01.000000 plantstar-shared-2.0.3.0.1/plantstar_shared.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:09:01.000000 plantstar-shared-2.0.3.0.1/plantstar_shared.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 19:09:01.000000 plantstar-shared-2.0.3.0.1/plantstar_shared.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 19:09:01.000000 plantstar-shared-2.0.3.0.1/plantstar_shared.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:09:01.155114 plantstar-shared-2.0.3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-22 19:08:44.000000 plantstar-shared-2.0.3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:11:52.016171 plantstar-shared-2.0.3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 19:11:52.016171 plantstar-shared-2.0.3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:11:52.016171 plantstar-shared-2.0.3.0.2/plantstar_shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/DataCollectionModuleProcessNames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/HuskyInterfacePacketTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/MockRawDataProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/RawDataProcessorInterfaceActions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/SysconType.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/add_size_onto_string_and_return.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/api_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/convert_bytes_to_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/convert_object_to_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/global_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/is_valid_signed_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/syscon_image_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/syscon_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/plantstar_shared/tcp_socket_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:11:52.016171 plantstar-shared-2.0.3.0.2/plantstar_shared.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 19:11:52.000000 plantstar-shared-2.0.3.0.2/plantstar_shared.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-22 19:11:52.000000 plantstar-shared-2.0.3.0.2/plantstar_shared.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:11:52.000000 plantstar-shared-2.0.3.0.2/plantstar_shared.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 19:11:52.000000 plantstar-shared-2.0.3.0.2/plantstar_shared.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 19:11:52.000000 plantstar-shared-2.0.3.0.2/plantstar_shared.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:11:52.016171 plantstar-shared-2.0.3.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-22 19:11:38.000000 plantstar-shared-2.0.3.0.2/setup.py
```

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/HuskyInterfacePacketTypes.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/HuskyInterfacePacketTypes.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/MockRawDataProcessor.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/MockRawDataProcessor.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/RawDataProcessorInterfaceActions.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/RawDataProcessorInterfaceActions.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/SysconType.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/SysconType.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/api_types.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/api_types.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/global_definitions.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/global_definitions.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     return syscon_json.dumps(base_dictionary, default=lambda _: "Not Serializeable")
 
 
 # TODO: Inherit from SyconType and remove `convert_to_json``
 class StatusCodes:
     OK = 200
+    NO_CONTENT = 204
     MOVED_PERMANENTLY = 301
     FOUND = 302
     BAD_REQUEST = 400
     UNAUTHORIZED = 401
     FORBIDDEN = 403
     INTERNAL_SERVER_ERROR = 500
     NOT_IMPLEMENTED = 501
```

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/obtain_raw_data_processor_function_for_action_name.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/syscon_json.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/syscon_json.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared/tcp_socket_utils.py` & `plantstar-shared-2.0.3.0.2/plantstar_shared/tcp_socket_utils.py`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/plantstar_shared.egg-info/SOURCES.txt` & `plantstar-shared-2.0.3.0.2/plantstar_shared.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plantstar-shared-2.0.3.0.1/setup.py` & `plantstar-shared-2.0.3.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as file_handle:
     long_description = file_handle.read()
 
 setuptools.setup(
     name="plantstar-shared",
     # MAJOR_VERSION.MINOR_VERSION.MAJOR_PATCH_VERSION.MINOR_PATCH_VERSION.SUBVERSION
-    version="2.0.3.0.1",
+    version="2.0.3.0.2",
     author="SYSCON International",
     author_email="dev@syscon-intl.com",
     description="Shared code used in plantstar_apu and plantstar_dcm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SYSCON-International/plantstar_shared",
     packages=setuptools.find_packages(),
```

