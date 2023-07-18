# Comparing `tmp/outplan-2.1.1.tar.gz` & `tmp/outplan-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/outplan-2.1.1.tar", last modified: Mon Apr  3 08:50:04 2023, max compression
+gzip compressed data, was "dist/outplan-2.1.2.tar", last modified: Tue Jul 18 11:15:46 2023, max compression
```

## Comparing `outplan-2.1.1.tar` & `outplan-2.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-03 08:50:04.000000 outplan-2.1.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1067 2023-04-03 08:49:05.000000 outplan-2.1.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-04-03 08:50:04.000000 outplan-2.1.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2023-04-03 08:49:05.000000 outplan-2.1.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-03 08:50:04.000000 outplan-2.1.1/outplan/
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2023-04-03 08:49:05.000000 outplan-2.1.1/outplan/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12285 2023-04-03 08:49:05.000000 outplan-2.1.1/outplan/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      256 2023-04-03 08:49:05.000000 outplan-2.1.1/outplan/const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2023-04-03 08:49:05.000000 outplan-2.1.1/outplan/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13747 2023-04-03 08:49:05.000000 outplan-2.1.1/outplan/experiment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1952 2023-04-03 08:49:05.000000 outplan-2.1.1/outplan/local.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-03 08:50:04.000000 outplan-2.1.1/outplan.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-04-03 08:50:04.000000 outplan-2.1.1/outplan.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2023-04-03 08:50:04.000000 outplan-2.1.1/outplan.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-03 08:50:04.000000 outplan-2.1.1/outplan.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2023-04-03 08:50:04.000000 outplan-2.1.1/outplan.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-03 08:50:04.000000 outplan-2.1.1/outplan.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-04-03 08:49:05.000000 outplan-2.1.1/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-04-03 08:50:04.000000 outplan-2.1.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1258 2023-04-03 08:49:05.000000 outplan-2.1.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-03 08:50:04.000000 outplan-2.1.1/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    28361 2023-04-03 08:49:05.000000 outplan-2.1.1/tests/test_experiment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1416 2023-04-03 08:49:05.000000 outplan-2.1.1/tests/test_local.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1067 2023-07-18 11:14:46.000000 outplan-2.1.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-07-18 11:15:46.000000 outplan-2.1.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2023-07-18 11:14:46.000000 outplan-2.1.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      300 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12861 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      256 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/const.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      195 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14078 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/experiment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1952 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/local.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      366 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       82 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-07-18 11:14:46.000000 outplan-2.1.2/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-07-18 11:15:46.000000 outplan-2.1.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1258 2023-07-18 11:14:46.000000 outplan-2.1.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    28361 2023-07-18 11:14:46.000000 outplan-2.1.2/tests/test_experiment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1416 2023-07-18 11:14:46.000000 outplan-2.1.2/tests/test_local.py
```

### Comparing `outplan-2.1.1/LICENSE` & `outplan-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `outplan-2.1.1/PKG-INFO` & `outplan-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outplan
-Version: 2.1.1
+Version: 2.1.2
 Summary: Support nested experiment/namespace base on Facebook Planout
 Home-page: https://github.com/xiachufang/outplan
 Author: x1ah
 Author-email: gaoxiaoqiang@xiachufang.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `outplan-2.1.1/README.md` & `outplan-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `outplan-2.1.1/outplan/client.py` & `outplan-2.1.2/outplan/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,14 +137,24 @@
         if unit and allow_specify_group and callable(self._get_specified_group_func):
             group = self._get_specified_group_func(
                 experiment_context, namespace_name, unit, user_id=user_id, pdid=pdid, **params
             )
             if group:
                 _tracking_group = self.get_tracking_group_by_group_name(namespace_name, group)
                 if _tracking_group:
+                    if self.tracking_client and track:
+                        self.tracking_client.track(
+                            user_id=user_id or 0,
+                            pdid=pdid or "",
+                            event_name="user_experiment_group_info",
+                            properties=dict(
+                                experiment=_tracking_group.experiment_trace(),
+                                group=_tracking_group.group_trace(),
+                            ),
+                        )
                     return _tracking_group
 
         key = "tracking_group{%s}{%s}" % (namespace_name, unit)
 
         if unit and cache and key in cached_group:
             return cached_group[key]
 
@@ -185,19 +195,20 @@
         return tracking_group.last_group
 
     def get_tracking_group_by_group_name(
         self, namespace_name: str, group_name: str
     ) -> Optional[TrackingGroup]:
         """ 根据实验组名获取tracking_group """
         namespace_item = self.get_namespace_item(namespace_name)  # type: NamespaceItem
-        group = namespace_item.get_group_by_name(group_name)
-        if group:
+        result = namespace_item.get_experiment_and_group_by_name(group_name)
+        if result:
+            exp, group = result
             return TrackingGroup(
                 group_name=group.name,
-                experiment_name="",
+                experiment_name=exp.name,
                 group_extra_params=group.extra_params,
             )
         return None
 
     def add_namespace(self, namespace_item: NamespaceItem):
         if namespace_item.name in self.namespaces:
             raise ExperimentValidateError("namespace name 冲突")
```

### Comparing `outplan-2.1.1/outplan/experiment.py` & `outplan-2.1.2/outplan/experiment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # coding: utf-8
 from collections import namedtuple
 from decimal import Decimal
-from typing import Any, Callable, Dict, List, Optional  # noqa
+from typing import Any, Callable, Dict, List, Optional, Tuple # noqa
 
 import simplejson
 from planout.experiment import DefaultExperiment
 from planout.namespace import SimpleNamespace
 from planout.ops.random import WeightedChoice
 
 from .const import GroupResultType, UserTagFilterType
@@ -135,19 +135,27 @@
         group_names = get_namespace_group_names(self)
 
         if len(group_names) != len(set(group_names)):
             raise ExperimentValidateError("实验({}) group name 重复".format(self.name))
 
     def get_group_by_name(self, group_name):
         # type: (str) -> Optional[GroupItem]
+        result = self.get_experiment_and_group_by_name(group_name)
+        if result is None:
+            return None
+        _, group_object = result
+        return group_object
+
+    def get_experiment_and_group_by_name(self, group_name):
+        # type: (str) -> Optional[Tuple[ExperimentItem, GroupItem]]
         for experiment_item in self.experiment_items:
             for group in experiment_item.group_items:
                 group_object = group.get_group_by_name(group_name)
                 if group_object:
-                    return group_object
+                    return experiment_item, group_object
         return None
 
     def get_group(self, unit="", **params):
         if not unit:
             unit = params.get(self.unit_type, "")
 
         valid_experiment_items = []
```

### Comparing `outplan-2.1.1/outplan/local.py` & `outplan-2.1.2/outplan/local.py`

 * *Files identical despite different names*

### Comparing `outplan-2.1.1/outplan.egg-info/PKG-INFO` & `outplan-2.1.2/outplan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outplan
-Version: 2.1.1
+Version: 2.1.2
 Summary: Support nested experiment/namespace base on Facebook Planout
 Home-page: https://github.com/xiachufang/outplan
 Author: x1ah
 Author-email: gaoxiaoqiang@xiachufang.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `outplan-2.1.1/setup.py` & `outplan-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with io.open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="outplan",
-    version="2.1.1",
+    version="2.1.2",
     description="Support nested experiment/namespace base on Facebook Planout",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xiachufang/outplan",
     author="x1ah",
     author_email="gaoxiaoqiang@xiachufang.com",
     packages=find_packages(exclude=["docs", "tests*"]),
```

### Comparing `outplan-2.1.1/tests/test_experiment.py` & `outplan-2.1.2/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `outplan-2.1.1/tests/test_local.py` & `outplan-2.1.2/tests/test_local.py`

 * *Files identical despite different names*

