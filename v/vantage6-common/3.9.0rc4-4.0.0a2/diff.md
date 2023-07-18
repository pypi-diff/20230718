# Comparing `tmp/vantage6-common-3.9.0rc4.tar.gz` & `tmp/vantage6-common-4.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-common-3.9.0rc4.tar", last modified: Wed May 24 09:34:08 2023, max compression
+gzip compressed data, was "vantage6-common-4.0.0a2.tar", last modified: Tue Jul 18 13:32:07 2023, max compression
```

## Comparing `vantage6-common-3.9.0rc4.tar` & `vantage6-common-4.0.0a2.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/__build__
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6/common/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/docker/addons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/docker/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-24 09:33:56.000000 vantage6-common-3.9.0rc4/vantage6/common/utest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 09:34:08.497724 vantage6-common-3.9.0rc4/vantage6_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 09:34:08.000000 vantage6-common-3.9.0rc4/vantage6_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:07.372662 vantage6-common-4.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 13:32:07.372662 vantage6-common-4.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:32:07.372662 vantage6-common-4.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:07.368662 vantage6-common-4.0.0a2/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:07.368662 vantage6-common-4.0.0a2/vantage6/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/__build__
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:07.368662 vantage6-common-4.0.0a2/vantage6/common/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/client/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/client/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/client/node_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:07.368662 vantage6-common-4.0.0a2/vantage6/common/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/docker/addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/docker/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-18 13:31:55.000000 vantage6-common-4.0.0a2/vantage6/common/utest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:32:07.372662 vantage6-common-4.0.0a2/vantage6_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 13:32:07.000000 vantage6-common-4.0.0a2/vantage6_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-18 13:32:07.000000 vantage6-common-4.0.0a2/vantage6_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:32:07.000000 vantage6-common-4.0.0a2/vantage6_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 13:32:07.000000 vantage6-common-4.0.0a2/vantage6_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 13:32:07.000000 vantage6-common-4.0.0a2/vantage6_common.egg-info/top_level.txt
```

### Comparing `vantage6-common-3.9.0rc4/PKG-INFO` & `vantage6-common-4.0.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a2 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.9.0rc4/setup.py` & `vantage6-common-4.0.0a2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,19 +32,21 @@
     url='https://github.com/vantage6/vantage6',
     packages=find_namespace_packages(),
     python_requires='>=3.6',
     install_requires=[
         'appdirs==1.4.4',
         'click==8.1.3',
         'colorama==0.4.6',
-        'cryptography==39.0.1',
+        'cryptography==41.0.0',
         'docker==6.1.2',
         'pyfiglet==0.8.post1',
+        'PyJWT==2.6.0',
         'PyYAML==6.0',
         'python-dateutil==2.8.2',
+        'requests==2.31.0',
         'schema==0.7.5',
     ],
     package_data={
         'vantage6.common': [
             '__build__',
         ],
     }
```

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/__init__.py` & `vantage6-common-4.0.0a2/vantage6/common/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -332,19 +332,10 @@
             "label": "database_label",
             "uri": "database_uri",
             "db_type": "database_type"
         }
     ]
 
     """
-    # FIXME The old format should be removed in v4+.
-    old_format = isinstance(databases, dict)
-    if old_format:
-        return {
-            "label": label,
-            "uri": databases[label],
-            "type": None
-        }
-    else:
-        for database in databases:
-            if database["label"] == label:
-                return database
+    for database in databases:
+        if database["label"] == label:
+            return database
```

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/_version.py` & `vantage6-common-4.0.0a2/vantage6/common/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, '__build__')) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (3, 9, 0, 'candidate', __build__, 0)
+version_info = (4, 0, 0, 'alpha', __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {'alpha': 'a', 'beta': 'b', 'candidate': 'rc', 'final': ''}
 version = f'{version_info[0]}.{version_info[1]}.{version_info[2]}'
 pre_release = '' if version_info[3] == 'final' else \
   '.'+_specifier_[version_info[3]]+str(version_info[4])
 post_release = '' if not version_info[5] else f'.post{version_info[5]}'
```

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/colors.py` & `vantage6-common-4.0.0a2/vantage6/common/colors.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/context.py` & `vantage6-common-4.0.0a2/vantage6/common/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging.handlers
 
 from pathlib import Path
 from typing import Tuple
 
 from vantage6.common import Singleton, error, Fore, Style, logger_name
 from vantage6.common.colors import ColorStreamHandler
-from vantage6.common.globals import DEFAULT_ENVIRONMENT, APPNAME
+from vantage6.common.globals import APPNAME
 from vantage6.common.configuration_manager import (
     ConfigurationManager
 )
 from vantage6.common._version import __version__
 
 
 class AppContext(metaclass=Singleton):
@@ -25,64 +25,50 @@
     #        be set in __init__
     #        I think the same applies to LOGGING_ENABLED
     INST_CONFIG_MANAGER = ConfigurationManager
     LOGGING_ENABLED = True
 
     def __init__(
         self, instance_type: str, instance_name: str,
-        environment: str = DEFAULT_ENVIRONMENT, system_folders: bool = False,
-        config_file: Path | str = None
+        system_folders: bool = False, config_file: Path | str = None
     ) -> None:
         """
         Create a new AppContext instance.
 
         Parameters
         ----------
         instance_type: str
             'server' or 'node'
         instance_name: str
             Name of the configuration
         system_folders: bool
             Use system folders instead of user folders
-        environment: str
-            Environment within the config file to use. Can be any of
-            'application', 'dev', 'test', 'acc' or 'prod'.
         config_file: str
             Path to a specific config file. If left as None, OS specific folder
             will be used to find the configuration file specified by
             `instance_name`.
         """
         self.scope: str = "system" if system_folders else "user"
         self.name: str = instance_name
         self.instance_type = instance_type
 
-        # configuration environment, load a single configuration from
-        # entire confiration file (which can contain multiple environments)
-        # self.config_file = self.config_dir / f"{instance_name}.yaml"
-
         # if config_file is None:
         #     config_file = f"{instance_name}.yaml"
         self.config_file = self.find_config_file(
             instance_type,
             self.name,
             system_folders,
             config_file
         )
 
-        # will load a specific environment in the config_file, this
-        # triggers to set the logging as this is env dependant
-        self.environment: str = environment
-
-        # lookup system / user directories, this needs to be done after
-        # the environment is been set. This way we can check if the
+        # look up system / user directories. This way we can check if the
         # config file container custom directories
         self.set_folders(instance_type, self.name, system_folders)
 
-        # after both the folders and the environment have been set, we
-        # can start logging!
+        # after the folders have been set, we can start logging!
         if self.LOGGING_ENABLED:
             self.setup_logging()
 
         # Log some history
         # FIXME: this should probably be moved to the actual app
         module_name = __name__.split('.')[-1]
         self.log = logging.getLogger(module_name)
@@ -97,39 +83,34 @@
         self.log.info(" --> Blog: https://vantage6.ai")
         self.log.info("-" * 60)
         self.log.info("Cite us!")
         self.log.info("If you publish your findings obtained using vantage6, ")
         self.log.info("please cite the proper sources as mentioned in:")
         self.log.info("https://vantage6.ai/vantage6/references")
         self.log.info("-" * 60)
-        self.log.info(f"Started application {APPNAME} with environment "
-                      f"{self.environment}")
+        self.log.info(f"Started application {APPNAME}")
         self.log.info("Current working directory is '%s'" % os.getcwd())
         self.log.info(f"Successfully loaded configuration from "
                       f"'{self.config_file}'")
         self.log.info("Logging to '%s'" % self.log_file)
         self.log.info(f"Common package version '{__version__}'")
 
     @classmethod
     def from_external_config_file(
-        cls, path: Path | str, instance_type: str,
-        environment: str = DEFAULT_ENVIRONMENT, system_folders: bool = False
+        cls, path: Path | str, instance_type: str, system_folders: bool = False
     ) -> "AppContext":
         """
         Create a new AppContext instance from an external config file.
 
         Parameters
         ----------
         path: str
             Path to the config file
         instance_type: str
             'server' or 'node'
-        environment: str
-            Environment within the config file to use. Can be any of
-            'application', 'dev', 'test', 'acc' or 'prod'.
         system_folders: bool
             Use system folders rather than user folders
 
         Returns
         -------
         AppContext
             A new AppContext instance
@@ -137,40 +118,36 @@
         instance_name = Path(path).stem
 
         self_ = cls.__new__(cls)
         self_.name = instance_name
         self_.scope = "system" if system_folders else "user"
         self_.config_dir = Path(path).parent
         self_.config_file = path
-        self_.environment = environment
         self_.instance_type = instance_type
         self_.set_folders(instance_type, instance_name, system_folders)
         module_name = logger_name(__name__)
         self_.log = logging.getLogger(module_name)
         if self_.LOGGING_ENABLED:
             self_.setup_logging()
 
         return self_
 
     @classmethod
     def config_exists(
         cls, instance_type: str, instance_name: str,
-        environment: str = DEFAULT_ENVIRONMENT, system_folders: bool = False
+        system_folders: bool = False
     ) -> bool:
         """Check if a config file exists for the given instance type and name.
 
         Parameters
         ----------
         instance_type: str
             'server' or 'node'
         instance_name: str
             Name of the configuration
-        environment: str
-            Environment within the config file to use. Can be any of
-            'application', 'dev', 'test', 'acc' or 'prod'.
         system_folders: bool
             Use system folders rather than user folders
 
         Returns
         -------
         bool
             True if the config file exists, False otherwise
@@ -182,17 +159,17 @@
                 system_folders,
                 verbose=False
             )
 
         except Exception:
             return False
 
-        # check that environment is present in config-file
-        config_manager = cls.INST_CONFIG_MANAGER.from_file(config_file)
-        return bool(getattr(config_manager, environment))
+        # check that configuration is present in config-file
+        config = cls.INST_CONFIG_MANAGER.from_file(config_file)
+        return bool(config)
 
     @staticmethod
     def type_data_folder(instance_type: str, system_folders: bool) -> Path:
         """
         Return OS specific data folder.
 
         Parameters
@@ -321,16 +298,15 @@
         ------
         AssertionError
             If the configuration manager is not initialized.
         """
         assert self.config_manager, \
             "Log file unkown as configuration manager not initialized"
         file_ = (Path(self.config_manager.name) /
-                 f"{type_}_{self.environment}_{self.scope}.log")
-
+                 f"{type_}_{self.scope}.log")
         return self.log_dir / file_
 
     @property
     def config_file_name(self) -> str:
         """Return the name of the configuration file.
 
         Returns
@@ -365,48 +341,15 @@
         ------
         AssertionError
             If the configuration file does not exist
         """
         assert Path(path).exists(), f"config {path} not found"
         self.__config_file = Path(path)
         self.config_manager = self.INST_CONFIG_MANAGER.from_file(path)
-
-    @property
-    def environment(self) -> str:
-        """Return the environment.
-
-        Returns
-        -------
-        str
-            Environment
-        """
-        return self.__environment
-
-    @environment.setter
-    def environment(self, env: str) -> None:
-        """
-        Set the environment.
-
-        Parameters
-        ----------
-        env: str
-            Environment
-
-        Raises
-        ------
-        AssertionError
-            If the environment is not found in the configuration or the
-            configuration manager is not initialized.
-        """
-        assert self.config_manager, \
-            "Environment set before ConfigurationManager is initialized..."
-        assert env in self.config_manager.available_environments, \
-            f"Requested environment {env} is not found in the configuration"
-        self.__environment = env
-        self.config: dict = self.config_manager.get(env)
+        self.config = self.config_manager.config
 
     @classmethod
     def find_config_file(
         cls, instance_type: str, instance_name: str, system_folders: bool,
         config_file: str | None = None, verbose: bool = True
     ) -> str:
         """
```

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/docker/addons.py` & `vantage6-common-4.0.0a2/vantage6/common/docker/addons.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/docker/network_manager.py` & `vantage6-common-4.0.0a2/vantage6/common/docker/network_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/encryption.py` & `vantage6-common-4.0.0a2/vantage6/common/encryption.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/log.py` & `vantage6-common-4.0.0a2/vantage6/common/log.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/task_status.py` & `vantage6-common-4.0.0a2/vantage6/common/task_status.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc4/vantage6/common/utest.py` & `vantage6-common-4.0.0a2/vantage6/common/utest.py`

 * *Files identical despite different names*

### Comparing `vantage6-common-3.9.0rc4/vantage6_common.egg-info/PKG-INFO` & `vantage6-common-4.0.0a2/vantage6_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-common
-Version: 3.9.0rc4
+Version: 4.0.0a2
 Summary: Vantage6 common
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-common Version: 3.9.0rc4 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-common Version: 4.0.0a2 Summary: Vantage6
 common Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
                                     ******
                                [vantage6] ******
           **** A privacy preserving federated learning solution ****
    ****  [![Release](https://github.com/vantage6/vantage6/actions/workflows/
 release.yml/badge.svg)](https://github.com/vantage6/vantage6/actions/workflows/
```

### Comparing `vantage6-common-3.9.0rc4/vantage6_common.egg-info/SOURCES.txt` & `vantage6-common-4.0.0a2/vantage6_common.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 vantage6/common/context.py
 vantage6/common/encryption.py
 vantage6/common/exceptions.py
 vantage6/common/globals.py
 vantage6/common/log.py
 vantage6/common/task_status.py
 vantage6/common/utest.py
+vantage6/common/client/client_base.py
+vantage6/common/client/deserialization.py
+vantage6/common/client/node_client.py
+vantage6/common/client/utils.py
 vantage6/common/docker/__init__.py
 vantage6/common/docker/addons.py
 vantage6/common/docker/network_manager.py
 vantage6_common.egg-info/PKG-INFO
 vantage6_common.egg-info/SOURCES.txt
 vantage6_common.egg-info/dependency_links.txt
 vantage6_common.egg-info/requires.txt
```

