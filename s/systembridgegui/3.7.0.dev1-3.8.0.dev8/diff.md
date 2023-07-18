# Comparing `tmp/systembridgegui-3.7.0.dev1.tar.gz` & `tmp/systembridgegui-3.8.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgegui-3.7.0.dev1.tar", last modified: Mon Jul  3 08:35:32 2023, max compression
+gzip compressed data, was "systembridgegui-3.8.0.dev8.tar", last modified: Tue Jul 18 10:20:51 2023, max compression
```

## Comparing `systembridgegui-3.7.0.dev1.tar` & `systembridgegui-3.8.0.dev8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.581477 systembridgegui-3.7.0.dev1/systembridgegui/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-03 08:35:30.000000 systembridgegui-3.7.0.dev1/systembridgegui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/system_tray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/systembridgegui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/widgets/timed_message_box.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/systembridgegui/window/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-03 08:35:14.000000 systembridgegui-3.7.0.dev1/systembridgegui/window/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:35:32.585477 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-03 08:35:32.000000 systembridgegui-3.7.0.dev1/systembridgegui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui/
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 10:20:49.000000 systembridgegui-3.8.0.dev8/systembridgegui/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/system_tray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/widgets/timed_message_box.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui/window/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-18 10:20:02.000000 systembridgegui-3.8.0.dev8/systembridgegui/window/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:20:51.899648 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 10:20:51.000000 systembridgegui-3.8.0.dev8/systembridgegui.egg-info/top_level.txt
```

### Comparing `systembridgegui-3.7.0.dev1/pyproject.toml` & `systembridgegui-3.8.0.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/setup.py` & `systembridgegui-3.8.0.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui/__main__.py` & `systembridgegui-3.8.0.dev8/systembridgegui/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-"""System Bridge GUI: Main"""
+"""System Bridge GUI"""
 from __future__ import annotations
 
 import asyncio
-import json
 import os
 import sys
 from typing import Optional
 
 import async_timeout
 from PySide6.QtCore import QUrl
 from PySide6.QtGui import QIcon
 from PySide6.QtMultimedia import QAudioOutput, QMediaPlayer
 from PySide6.QtWidgets import QApplication, QMessageBox
 from systembridgeshared.base import Base
-from systembridgeshared.const import SETTING_LOG_LEVEL
 from systembridgeshared.database import Database
 from systembridgeshared.exceptions import ConnectionErrorException
-from systembridgeshared.logger import setup_logger
 from systembridgeshared.models.media_play import MediaPlay
 from systembridgeshared.models.notification import Notification as NotificationData
 from systembridgeshared.settings import Settings
 from systembridgeshared.websocket_client import WebSocketClient
-from typer import Typer
 
 from ._version import __version__
 from .system_tray import SystemTray
 from .widgets.timed_message_box import TimedMessageBox
 from .window.main import MainWindow
 from .window.notification import NotificationWindow
 from .window.player import PlayerWindow
 
 
-class Main(Base):
-    """Main"""
+class Application(Base):
+    """Application"""
 
     def __init__(
         self,
+        database: Database,
+        settings: Settings,
         command: str = "main",
         gui_only: bool = False,
         data: Optional[dict] = None,
     ) -> None:
         """Initialize"""
         super().__init__()
         self._logger.info("System Bridge GUI %s: Startup", __version__.public())
@@ -225,47 +223,7 @@
                 await self._websocket_client.connect()
         except ConnectionErrorException as exception:
             self._logger.error("Could not connect to WebSocket: %s", exception)
             self._startup_error("Could not connect to WebSocket!")
         except asyncio.TimeoutError as exception:
             self._logger.error("Connection timeout to WebSocket: %s", exception)
             self._startup_error("Connection timeout to WebSocket!")
-
-
-app = Typer()
-
-
-@app.command(name="main", help="Run the main application")
-def main(
-    gui_only: bool = False,
-) -> None:
-    """Run the main application"""
-    Main(command="main", gui_only=gui_only)
-
-
-@app.command(name="media-player", help="Run the media player")
-def media_player(
-    media_type: str,
-    data: str,
-) -> None:
-    """Run the media player"""
-    Main(command=f"media-player-{media_type}", data=json.loads(data))
-
-
-@app.command(name="notification", help="Show a notification")
-def notification(
-    data: str,
-) -> None:
-    """Show a notification"""
-    Main(command="notification", data=json.loads(data))
-
-
-if __name__ == "__main__":
-    asyncio.set_event_loop(asyncio.new_event_loop())
-    database = Database()
-    settings = Settings(database)
-
-    log_level: str = str(settings.get(SETTING_LOG_LEVEL))
-
-    setup_logger(log_level, "system-bridge-gui")
-
-    app()
```

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui/icon.png` & `systembridgegui-3.8.0.dev8/systembridgegui/icon.png`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui/system_tray.py` & `systembridgegui-3.8.0.dev8/systembridgegui/system_tray.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui/widgets/timed_message_box.py` & `systembridgegui-3.8.0.dev8/systembridgegui/widgets/timed_message_box.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui/window/main.py` & `systembridgegui-3.8.0.dev8/systembridgegui/window/main.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui/window/notification.py` & `systembridgegui-3.8.0.dev8/systembridgegui/window/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui/window/player.py` & `systembridgegui-3.8.0.dev8/systembridgegui/window/player.py`

 * *Files identical despite different names*

### Comparing `systembridgegui-3.7.0.dev1/systembridgegui.egg-info/SOURCES.txt` & `systembridgegui-3.8.0.dev8/systembridgegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

