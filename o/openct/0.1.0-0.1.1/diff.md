# Comparing `tmp/openct-0.1.0.tar.gz` & `tmp/openct-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openct-0.1.0.tar", max compression
+gzip compressed data, was "openct-0.1.1.tar", max compression
```

## Comparing `openct-0.1.0.tar` & `openct-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-07-17 18:31:15.125436 openct-0.1.0/LICENSE
--rw-r--r--   0        0        0      661 2023-07-17 18:31:15.125436 openct-0.1.0/README.md
--rw-r--r--   0        0        0      128 2023-07-17 18:31:15.125436 openct-0.1.0/openct/__init__.py
--rw-r--r--   0        0        0     1032 2023-07-17 18:31:15.125436 openct-0.1.0/openct/__main__.py
--rw-r--r--   0        0        0      155 2023-07-17 18:31:15.125436 openct-0.1.0/openct/config/__init__.py
--rw-r--r--   0        0        0      563 2023-07-17 18:31:15.125436 openct-0.1.0/openct/config/__main__.py
--rw-r--r--   0        0        0     1441 2023-07-17 18:31:15.125436 openct-0.1.0/openct/config/config.py
--rw-r--r--   0        0        0      608 2023-07-17 18:31:15.125436 openct-0.1.0/openct/config/config_schema.py
--rw-r--r--   0        0        0       83 2023-07-17 18:31:15.125436 openct-0.1.0/openct/connections/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-17 18:31:15.125436 openct-0.1.0/openct/connections/connections.py
--rw-r--r--   0        0        0       73 2023-07-17 18:31:15.125436 openct-0.1.0/openct/datastore/__init__.py
--rw-r--r--   0        0        0     1359 2023-07-17 18:31:15.125436 openct-0.1.0/openct/datastore/datastore.py
--rw-r--r--   0        0        0       65 2023-07-17 18:31:15.125436 openct-0.1.0/openct/devices/__init__.py
--rw-r--r--   0        0        0      817 2023-07-17 18:31:15.125436 openct-0.1.0/openct/devices/devices.py
--rw-r--r--   0        0        0      418 2023-07-17 18:31:15.125436 openct-0.1.0/openct/logging_init.py
--rw-r--r--   0        0        0      592 2023-07-17 18:31:15.125436 openct-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 openct-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-18 18:59:08.983315 openct-0.1.1/LICENSE
+-rw-r--r--   0        0        0      661 2023-07-18 18:59:08.983315 openct-0.1.1/README.md
+-rw-r--r--   0        0        0       89 2023-07-18 18:59:08.983315 openct-0.1.1/openct/__init__.py
+-rw-r--r--   0        0        0      859 2023-07-18 18:59:08.983315 openct-0.1.1/openct/__main__.py
+-rw-r--r--   0        0        0       83 2023-07-18 18:59:08.983315 openct-0.1.1/openct/connections/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-18 18:59:08.983315 openct-0.1.1/openct/connections/connections.py
+-rw-r--r--   0        0        0       73 2023-07-18 18:59:08.983315 openct-0.1.1/openct/datastore/__init__.py
+-rw-r--r--   0        0        0     1359 2023-07-18 18:59:08.983315 openct-0.1.1/openct/datastore/datastore.py
+-rw-r--r--   0        0        0       65 2023-07-18 18:59:08.983315 openct-0.1.1/openct/devices/__init__.py
+-rw-r--r--   0        0        0      817 2023-07-18 18:59:08.983315 openct-0.1.1/openct/devices/devices.py
+-rw-r--r--   0        0        0      201 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/__init__.py
+-rw-r--r--   0        0        0      556 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/__main__.py
+-rw-r--r--   0        0        0     1440 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/config.py
+-rw-r--r--   0        0        0      626 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/config_schema.py
+-rw-r--r--   0        0        0     1354 2023-07-18 18:59:08.983315 openct-0.1.1/openct/setup/setup.py
+-rw-r--r--   0        0        0      592 2023-07-18 18:59:08.983315 openct-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1309 1970-01-01 00:00:00.000000 openct-0.1.1/PKG-INFO
```

### Comparing `openct-0.1.0/LICENSE` & `openct-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openct-0.1.0/README.md` & `openct-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openct-0.1.0/openct/config/__main__.py` & `openct-0.1.1/openct/setup/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
         "connection_timeout": 3,
         "backup_max_age": 60,
         "log_max_age": 30,
         "log_max_count": 10,
     },
 }
 
-with open(file="config/config.yml", mode="a", encoding="utf-8") as file:
+with open(file="config.yml", mode="a", encoding="utf-8") as file:
     yaml.dump(mt_backup_config, file, default_flow_style=False)
```

### Comparing `openct-0.1.0/openct/config/config.py` & `openct-0.1.1/openct/setup/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 import yaml
 
 from .config_schema import Config, ConfigDirs, ConfigIdentity, ConfigSettings
 
 
-def load_config(config_file: str = "config/config.yml") -> Config:
+def load_config(config_file: str) -> Config:
     """Try loading config."""
     try:
         return load_config_from_file(config_file)
     except FileNotFoundError:
         print(f"Config file {config_file} not found. Please create it.")
         sys.exit(1)
     except TypeError:
@@ -28,14 +28,15 @@
         username=config_data["identity"]["username"],
         key_file=config_data["identity"]["key_file"],
     )
 
     dirs = ConfigDirs(
         backup_dir=config_data["dirs"]["backup_dir"],
         log_dir=config_data["dirs"]["log_dir"],
+        root_dir="",
     )
 
     settings = ConfigSettings(
         datastore_type=config_data["settings"]["datastore_type"],
         connection_timeout=config_data["settings"]["connection_timeout"],
         backup_max_age=config_data["settings"]["backup_max_age"],
         log_max_age=config_data["settings"]["log_max_age"],
```

### Comparing `openct-0.1.0/openct/config/config_schema.py` & `openct-0.1.1/openct/setup/config_schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     key_file: str
 
 
 @dataclass
 class ConfigDirs:
     """Config directories dataclass."""
 
+    root_dir: str
     backup_dir: str
     log_dir: str
 
 
 @dataclass
 class ConfigSettings:
     """Config settings dataclass."""
```

### Comparing `openct-0.1.0/openct/connections/connections.py` & `openct-0.1.1/openct/connections/connections.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.0/openct/datastore/datastore.py` & `openct-0.1.1/openct/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.0/openct/devices/devices.py` & `openct-0.1.1/openct/devices/devices.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.0/pyproject.toml` & `openct-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openct"
-version = "0.1.0"
+version = "0.1.1"
 description = "Configuration backup and analysis tools for devices running pfSense and RouterOS"
 authors = ["Weehooey <info@weehooey.com>"]
 license = "GNU GPL v3.0"
 readme = "README.md"
 repository = "https://github.com/weehooey/openct"
 
 [tool.poetry.dependencies]
```

### Comparing `openct-0.1.0/PKG-INFO` & `openct-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openct
-Version: 0.1.0
+Version: 0.1.1
 Summary: Configuration backup and analysis tools for devices running pfSense and RouterOS
 Home-page: https://github.com/weehooey/openct
 License: GNU GPL v3.0
 Author: Weehooey
 Author-email: info@weehooey.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

