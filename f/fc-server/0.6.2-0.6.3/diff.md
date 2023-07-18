# Comparing `tmp/fc-server-0.6.2.tar.gz` & `tmp/fc-server-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fc-server-0.6.2.tar", last modified: Thu Jul  6 08:49:04 2023, max compression
+gzip compressed data, was "dist/fc-server-0.6.3.tar", last modified: Tue Jul 18 04:27:04 2023, max compression
```

## Comparing `fc-server-0.6.2.tar` & `fc-server-0.6.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-06 08:48:52.000000 fc-server-0.6.2/LICENSE
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 08:49:04.000000 fc-server-0.6.2/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-06 08:48:52.000000 fc-server-0.6.2/README.rst
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_common/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_common/VERSION
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_common/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_common/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_common/etcd.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_common/logger.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_common/version.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/__init__.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server/config/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      530 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/config/sample_cfg.yaml
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       82 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/config/sample_lavacli.yaml
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server/core/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      935 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/core/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     6461 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/core/api_svr.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     4093 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/core/config.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    12190 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/core/coordinator.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1990 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/core/decorators.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      623 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/core/plugin.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server/management/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/management/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2498 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/management/cmd_online_lava_devices.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      212 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/management/common.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server/plugins/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/plugins/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     8138 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/plugins/labgrid.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)    17708 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/plugins/lava.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server/plugins/utils/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/plugins/utils/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2819 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/plugins/utils/labgrid.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     5264 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/plugins/utils/lava.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     1113 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server/server.py
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server.egg-info/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server.egg-info/PKG-INFO
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      993 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server.egg-info/SOURCES.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server.egg-info/dependency_links.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server.egg-info/entry_points.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      157 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server.egg-info/requires.txt
--rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server.egg-info/top_level.txt
-drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:49:04.000000 fc-server-0.6.2/fc_server_daemon/
--rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server_daemon/__init__.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     2185 2023-07-06 08:48:52.000000 fc-server-0.6.2/fc_server_daemon/server_daemon.py
--rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-06 08:49:04.000000 fc-server-0.6.2/setup.cfg
--rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-06 08:48:52.000000 fc-server-0.6.2/setup.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1071 2023-07-18 04:26:21.000000 fc-server-0.6.3/LICENSE
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:04.000000 fc-server-0.6.3/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2535 2023-07-18 04:26:21.000000 fc-server-0.6.3/README.rst
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_common/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        6 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/VERSION
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      482 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      930 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1607 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/etcd.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1501 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/logger.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      712 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_common/version.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/__init__.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/config/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      530 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/config/sample_cfg.yaml
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       82 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/config/sample_lavacli.yaml
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/core/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      935 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     7751 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/api_svr.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     4093 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/config.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    12190 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/coordinator.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1990 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/decorators.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      623 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/core/plugin.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/management/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/management/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2498 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/management/cmd_online_lava_devices.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      212 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/management/common.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/plugins/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     8138 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)    17708 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/lava.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server/plugins/utils/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/utils/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2819 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/utils/labgrid.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     5264 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/plugins/utils/lava.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     1113 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server/server.py
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      670 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/PKG-INFO
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      993 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/SOURCES.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        1 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/dependency_links.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       52 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/entry_points.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      157 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/requires.txt
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)       37 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server.egg-info/top_level.txt
+drwxr-xr-x   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:27:04.000000 fc-server-0.6.3/fc_server_daemon/
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)        0 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server_daemon/__init__.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     2185 2023-07-18 04:26:21.000000 fc-server-0.6.3/fc_server_daemon/server_daemon.py
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)      614 2023-07-18 04:27:04.000000 fc-server-0.6.3/setup.cfg
+-rw-r--r--   0 nxa13855  (1001) atg       (1001)     3882 2023-07-18 04:26:21.000000 fc-server-0.6.3/setup.py
```

### Comparing `fc-server-0.6.2/LICENSE` & `fc-server-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/PKG-INFO` & `fc-server-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-server-0.6.2/README.rst` & `fc-server-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_common/config.py` & `fc-server-0.6.3/fc_common/config.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_common/etcd.py` & `fc-server-0.6.3/fc_common/etcd.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_common/logger.py` & `fc-server-0.6.3/fc_common/logger.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_common/version.py` & `fc-server-0.6.3/fc_common/version.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/config/sample_cfg.yaml` & `fc-server-0.6.3/fc_server/config/sample_cfg.yaml`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/core/__init__.py` & `fc-server-0.6.3/fc_server/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/core/api_svr.py` & `fc-server-0.6.3/fc_server/core/api_svr.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,47 +43,51 @@
                 labgrid_managed_resources = framework.managed_resources
                 break
 
         res = request.match_info.get("res", "")
 
         resources_info = []
         if res:
-            item = []
-            item.append(res)
-            item.append(Config.managed_resources_farm_types.get(res, ""))
-            item.append(
-                ApiSvr.friendly_status(
-                    self.context.managed_resources_status.get(res, "")
+            if res in Config.managed_resources:
+                item = []
+                item.append(res)
+                item.append(Config.managed_resources_farm_types.get(res, ""))
+                item.append(
+                    ApiSvr.friendly_status(
+                        self.context.managed_resources_status.get(res, "")
+                    )
                 )
-            )
-            if res not in labgrid_managed_resources:
-                item.append("non-debuggable")
-            else:
-                item.append("")
+                if res not in labgrid_managed_resources:
+                    item.append("non-debuggable")
+                else:
+                    item.append("")
 
-            # fetch external resource info if needed
-            if self.external_info_tool:
-                fc_resource = res
-                fc_farm_type = Config.managed_resources_farm_types.get(res, "")
-                template = Template(self.external_info_tool)
-                tool_command = template.substitute(
-                    {"fc_resource": fc_resource, "fc_farm_type": fc_farm_type}
-                )
-                ret, info, _ = await self._run_cmd(tool_command)
+                if self.external_info_tool:
+                    # fetch external resource info if needed
+                    fc_resource = res
+                    fc_farm_type = Config.managed_resources_farm_types.get(res, "")
+                    template = Template(self.external_info_tool)
+                    tool_command = template.substitute(
+                        {"fc_resource": fc_resource, "fc_farm_type": fc_farm_type}
+                    )
+                    ret, info, _ = await self._run_cmd(tool_command)
 
-                if ret == 0:
-                    item.append(info)
+                    if ret == 0:
+                        item.append(info)
+                    else:
+                        item.append("NA")
                 else:
-                    item.append("NA")
+                    item.append([])
 
-            resources_info.append(item)
+                resources_info.append(item)
         else:
             params = request.rel_url.query
             farm_type = params.get("farmtype", "")
             device_type = params.get("devicetype", "")
+            peripheral_info = params.get("peripheralinfo", "")
 
             if device_type and farm_type:
                 scope = Config.raw_managed_resources.get(farm_type, {}).get(
                     device_type, []
                 )
             elif device_type:
                 scope = []
@@ -114,24 +118,47 @@
 
                 # fetch external resource info if needed
                 if self.external_info_tool and device_type:
                     fc_resource = resource
                     fc_farm_type = Config.managed_resources_farm_types.get(resource, "")
                     template = Template(self.external_info_tool)
                     tool_command = template.substitute(
-                        {"fc_resource": fc_resource, "fc_farm_type": fc_farm_type}
+                        {
+                            "fc_resource": fc_resource,
+                            "fc_farm_type": fc_farm_type,
+                            "fc_peripheral_info": peripheral_info,
+                        }
                     )
                     tool_command_list.append(self._run_cmd(tool_command))
 
-            external_info_list = await asyncio.gather(*tool_command_list)
-            for index, value in enumerate(external_info_list):
-                if value[0] == 0:
-                    resources_info[index].append(value[1])
-                else:
-                    resources_info[index].append("NA")
+            fc_not_match_list = []
+            if self.external_info_tool and device_type:
+                external_info_list = await asyncio.gather(*tool_command_list)
+                for index, value in enumerate(external_info_list):
+                    if value[0] == 0:
+                        resources_info[index].append(value[1])
+                        if value[1].strip() == "FC_NOT_MATCH":
+                            fc_not_match_list.append(index)
+                    else:
+                        resources_info[index].append("NA")
+            elif (
+                device_type
+            ):  # for fc instance which doesn't configure external_info_tool
+                for index, resource in enumerate(resources_info):
+                    resource.append([])
+                    if (
+                        peripheral_info
+                    ):  # external_info_tool not specified instance defintly not match anything
+                        fc_not_match_list.append(index)
+
+            resources_info = [
+                item
+                for index, item in enumerate(resources_info)
+                if index not in fc_not_match_list
+            ]
 
         return web.json_response(resources_info)
 
     @staticmethod
     async def pong(_):
         return web.Response(text="pong")
```

### Comparing `fc-server-0.6.2/fc_server/core/config.py` & `fc-server-0.6.3/fc_server/core/config.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/core/coordinator.py` & `fc-server-0.6.3/fc_server/core/coordinator.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/core/decorators.py` & `fc-server-0.6.3/fc_server/core/decorators.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/core/plugin.py` & `fc-server-0.6.3/fc_server/core/plugin.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/management/cmd_online_lava_devices.py` & `fc-server-0.6.3/fc_server/management/cmd_online_lava_devices.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/plugins/labgrid.py` & `fc-server-0.6.3/fc_server/plugins/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/plugins/lava.py` & `fc-server-0.6.3/fc_server/plugins/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/plugins/utils/labgrid.py` & `fc-server-0.6.3/fc_server/plugins/utils/labgrid.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/plugins/utils/lava.py` & `fc-server-0.6.3/fc_server/plugins/utils/lava.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server/server.py` & `fc-server-0.6.3/fc_server/server.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server.egg-info/PKG-INFO` & `fc-server-0.6.3/fc_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fc-server
-Version: 0.6.2
+Version: 0.6.3
 Home-page: https://fc.readthedocs.io/
 Author: Larry Shen
 Author-email: larry.shen@nxp.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `fc-server-0.6.2/fc_server.egg-info/SOURCES.txt` & `fc-server-0.6.3/fc_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/fc_server_daemon/server_daemon.py` & `fc-server-0.6.3/fc_server_daemon/server_daemon.py`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/setup.cfg` & `fc-server-0.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `fc-server-0.6.2/setup.py` & `fc-server-0.6.3/setup.py`

 * *Files identical despite different names*

