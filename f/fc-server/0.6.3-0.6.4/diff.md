# Comparing `tmp/fc-server-0.6.3.tar.gz` & `tmp/fc-server-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-server-0.6.3.tar", last modified: Tue Jul 18 04:27:04 2023, max compression
+gzip compressed data, was "dist/fc-server-0.6.4.tar", last modified: Tue Jul 18 05:39:55 2023, max compression
```

## Comparing `fc-server-0.6.3.tar` & `fc-server-0.6.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 04:26:21.000000 fc-server-0.6.3/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:04.000000 fc-server-0.6.3/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 04:26:21.000000 fc-server-0.6.3/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/version.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/__init__.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/config/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      530 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/config/sample_cfg.yaml
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       82 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/config/sample_lavacli.yaml
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/core/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      935 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     7751 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/api_svr.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     4093 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    12190 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/coordinator.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1990 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/decorators.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      623 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/plugin.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/management/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/management/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2498 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/management/cmd_online_lava_devices.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      212 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/management/common.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/plugins/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     8138 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/labgrid.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    17708 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/lava.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/plugins/utils/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/utils/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2819 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/utils/labgrid.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     5264 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/utils/lava.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1113 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/server.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      993 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      157 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/requires.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server_daemon/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server_daemon/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2185 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server_daemon/server_daemon.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 04:27:04.000000 fc-server-0.6.3/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 04:26:21.000000 fc-server-0.6.3/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 05:39:49.000000 fc-server-0.6.4/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 05:39:55.000000 fc-server-0.6.4/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 05:39:49.000000 fc-server-0.6.4/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_common/version.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/__init__.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server/config/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      530 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/config/sample_cfg.yaml
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       82 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/config/sample_lavacli.yaml
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server/core/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      935 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/core/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     7888 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/core/api_svr.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     4093 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/core/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    12190 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/core/coordinator.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1990 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/core/decorators.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      623 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/core/plugin.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server/management/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/management/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2498 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/management/cmd_online_lava_devices.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      212 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/management/common.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server/plugins/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/plugins/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     8138 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/plugins/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    17708 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/plugins/lava.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server/plugins/utils/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/plugins/utils/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2819 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/plugins/utils/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     5264 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/plugins/utils/lava.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1113 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server/server.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 05:39:54.000000 fc-server-0.6.4/fc_server.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      993 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 05:39:54.000000 fc-server-0.6.4/fc_server.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-18 05:39:54.000000 fc-server-0.6.4/fc_server.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      157 2023-07-18 05:39:54.000000 fc-server-0.6.4/fc_server.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-18 05:39:54.000000 fc-server-0.6.4/fc_server.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:55.000000 fc-server-0.6.4/fc_server_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server_daemon/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2185 2023-07-18 05:39:49.000000 fc-server-0.6.4/fc_server_daemon/server_daemon.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 05:39:55.000000 fc-server-0.6.4/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 05:39:49.000000 fc-server-0.6.4/setup.py
```

### Comparing `fc-server-0.6.3/LICENSE` & `fc-server-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/PKG-INFO` & `fc-server-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.6.3
+Version: 0.6.4
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-server-0.6.3/README.rst` & `fc-server-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_common/config.py` & `fc-server-0.6.4/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_common/etcd.py` & `fc-server-0.6.4/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_common/logger.py` & `fc-server-0.6.4/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_common/version.py` & `fc-server-0.6.4/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/config/sample_cfg.yaml` & `fc-server-0.6.4/fc_server/config/sample_cfg.yaml`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/core/__init__.py` & `fc-server-0.6.4/fc_server/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/core/api_svr.py` & `fc-server-0.6.4/fc_server/core/api_svr.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,19 @@
 
                 if self.external_info_tool:
                     # fetch external resource info if needed
                     fc_resource = res
                     fc_farm_type = Config.managed_resources_farm_types.get(res, "")
                     template = Template(self.external_info_tool)
                     tool_command = template.substitute(
-                        {"fc_resource": fc_resource, "fc_farm_type": fc_farm_type}
+                        {
+                            "fc_resource": fc_resource,
+                            "fc_farm_type": fc_farm_type,
+                            "fc_peripheral_info": "",
+                        }
                     )
                     ret, info, _ = await self._run_cmd(tool_command)
 
                     if ret == 0:
                         item.append(info)
                     else:
                         item.append("NA")
```

### Comparing `fc-server-0.6.3/fc_server/core/config.py` & `fc-server-0.6.4/fc_server/core/config.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/core/coordinator.py` & `fc-server-0.6.4/fc_server/core/coordinator.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/core/decorators.py` & `fc-server-0.6.4/fc_server/core/decorators.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/core/plugin.py` & `fc-server-0.6.4/fc_server/core/plugin.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/management/cmd_online_lava_devices.py` & `fc-server-0.6.4/fc_server/management/cmd_online_lava_devices.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/plugins/labgrid.py` & `fc-server-0.6.4/fc_server/plugins/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/plugins/lava.py` & `fc-server-0.6.4/fc_server/plugins/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/plugins/utils/labgrid.py` & `fc-server-0.6.4/fc_server/plugins/utils/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/plugins/utils/lava.py` & `fc-server-0.6.4/fc_server/plugins/utils/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server/server.py` & `fc-server-0.6.4/fc_server/server.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server.egg-info/PKG-INFO` & `fc-server-0.6.4/fc_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.6.3
+Version: 0.6.4
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-server-0.6.3/fc_server.egg-info/SOURCES.txt` & `fc-server-0.6.4/fc_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/fc_server_daemon/server_daemon.py` & `fc-server-0.6.4/fc_server_daemon/server_daemon.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/setup.cfg` & `fc-server-0.6.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.3/setup.py` & `fc-server-0.6.4/setup.py`

 * *Files identical despite different names*

