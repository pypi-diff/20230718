# Comparing `tmp/systembridgegui-3.8.0.dev8.tar.gz` & `tmp/systembridgegui-3.8.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgegui-3.8.0.dev8.tar", last modified: Tue Jul 18 10:20:51 2023, max compression
+gzip compressed data, was "systembridgegui-3.8.0.dev9.tar", last modified: Tue Jul 18 14:39:18 2023, max compression
```

## Comparing `systembridgegui-3.8.0.dev8.tar` & `systembridgegui-3.8.0.dev9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui/
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 10:20:49.000000 systembridgegui-3.8.0.dev8/systembridgegui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/system_tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/widgets/timed_message_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui/window/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:39:18.542544 systembridgegui-3.8.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 14:39:18.542544 systembridgegui-3.8.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:39:18.542544 systembridgegui-3.8.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:39:18.538544 systembridgegui-3.8.0.dev9/systembridgegui/
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 14:39:14.000000 systembridgegui-3.8.0.dev9/systembridgegui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/system_tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:39:18.542544 systembridgegui-3.8.0.dev9/systembridgegui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/widgets/timed_message_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:39:18.542544 systembridgegui-3.8.0.dev9/systembridgegui/window/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/window/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/window/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 14:38:11.000000 systembridgegui-3.8.0.dev9/systembridgegui/window/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:39:18.542544 systembridgegui-3.8.0.dev9/systembridgegui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 14:39:18.000000 systembridgegui-3.8.0.dev9/systembridgegui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 14:39:18.000000 systembridgegui-3.8.0.dev9/systembridgegui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:39:18.000000 systembridgegui-3.8.0.dev9/systembridgegui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-18 14:39:18.000000 systembridgegui-3.8.0.dev9/systembridgegui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 14:39:18.000000 systembridgegui-3.8.0.dev9/systembridgegui.egg-info/top_level.txt
```

### Comparing `systembridgegui-3.8.0.dev8/pyproject.toml` & `systembridgegui-3.8.0.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/setup.py` & `systembridgegui-3.8.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/__init__.py` & `systembridgegui-3.8.0.dev9/systembridgegui/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/__main__.py` & `systembridgegui-3.8.0.dev9/systembridgegui/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/icon.png` & `systembridgegui-3.8.0.dev9/systembridgegui/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/system_tray.py` & `systembridgegui-3.8.0.dev9/systembridgegui/system_tray.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/widgets/timed_message_box.py` & `systembridgegui-3.8.0.dev9/systembridgegui/widgets/timed_message_box.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/window/main.py` & `systembridgegui-3.8.0.dev9/systembridgegui/window/main.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/window/notification.py` & `systembridgegui-3.8.0.dev9/systembridgegui/window/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui/window/player.py` & `systembridgegui-3.8.0.dev9/systembridgegui/window/player.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.8.0.dev8/systembridgegui.egg-info/SOURCES.txt` & `systembridgegui-3.8.0.dev9/systembridgegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

