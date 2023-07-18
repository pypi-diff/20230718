# Comparing `tmp/hspylib-setman-0.9.8.tar.gz` & `tmp/hspylib-setman-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-setman-0.9.8.tar", last modified: Thu Jul  6 22:57:59 2023, max compression
+gzip compressed data, was "hspylib-setman-0.9.9.tar", last modified: Fri Jul  7 18:28:10 2023, max compression
```

## Comparing `hspylib-setman-0.9.8.tar` & `hspylib-setman-0.9.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.335534 hspylib-setman-0.9.8/
--rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.8/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 22:57:59.334661 hspylib-setman-0.9.8/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.302679 hspylib-setman-0.9.8/hspylib_setman.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-06 22:57:59.000000 hspylib-setman-0.9.8/hspylib_setman.egg-info/top_level.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.312377 hspylib-setman-0.9.8/setman/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      718 2023-07-05 21:55:00.000000 hspylib-setman-0.9.8/setman/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/__init__.py
--rwxr-xr-x   0 hjunior    (504) staff       (20)     4904 2023-07-06 20:31:12.000000 hspylib-setman-0.9.8/setman/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.320701 hspylib-setman-0.9.8/setman/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     7715 2023-07-06 20:30:14.000000 hspylib-setman-0.9.8/setman/core/setman.py
--rw-r--r--   0 hjunior    (504) staff       (20)      823 2023-07-05 22:10:34.000000 hspylib-setman-0.9.8/setman/core/setman_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.8/setman/core/setman_enums.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-06 22:57:59.333242 hspylib-setman-0.9.8/setman/settings/
--rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-06 22:57:58.000000 hspylib-setman-0.9.8/setman/settings/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     9772 2023-07-06 19:29:15.000000 hspylib-setman-0.9.8/setman/settings/settings.py
--rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.8/setman/settings/settings_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3446 2023-07-05 22:08:41.000000 hspylib-setman-0.9.8/setman/settings/settings_entry.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4135 2023-07-06 19:23:54.000000 hspylib-setman-0.9.8/setman/settings/settings_repository.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2154 2023-07-06 19:24:40.000000 hspylib-setman-0.9.8/setman/settings/settings_service.py
--rw-r--r--   0 hjunior    (504) staff       (20)      232 2023-07-06 19:46:06.000000 hspylib-setman-0.9.8/setman/welcome.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-06 22:57:59.335710 hspylib-setman-0.9.8/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.8/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:28:10.586367 hspylib-setman-0.9.9/
+-rw-r--r--   0 hjunior    (504) staff       (20)       51 2023-07-06 16:29:29.000000 hspylib-setman-0.9.9/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-07 18:28:10.585264 hspylib-setman-0.9.9/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      672 2023-07-07 18:28:09.000000 hspylib-setman-0.9.9/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:28:10.549710 hspylib-setman-0.9.9/hspylib_setman.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1675 2023-07-07 18:28:10.000000 hspylib-setman-0.9.9/hspylib_setman.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      619 2023-07-07 18:28:10.000000 hspylib-setman-0.9.9/hspylib_setman.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-07-07 18:28:10.000000 hspylib-setman-0.9.9/hspylib_setman.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       41 2023-07-07 18:28:10.000000 hspylib-setman-0.9.9/hspylib_setman.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        7 2023-07-07 18:28:10.000000 hspylib-setman-0.9.9/hspylib_setman.egg-info/top_level.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:28:10.560732 hspylib-setman-0.9.9/setman/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-07-07 18:28:09.000000 hspylib-setman-0.9.9/setman/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      785 2023-07-07 16:00:13.000000 hspylib-setman-0.9.9/setman/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      166 2023-07-07 18:28:09.000000 hspylib-setman-0.9.9/setman/__init__.py
+-rwxr-xr-x   0 hjunior    (504) staff       (20)     4904 2023-07-07 16:14:44.000000 hspylib-setman-0.9.9/setman/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:28:10.570693 hspylib-setman-0.9.9/setman/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      197 2023-07-07 18:28:09.000000 hspylib-setman-0.9.9/setman/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     7742 2023-07-07 18:23:30.000000 hspylib-setman-0.9.9/setman/core/setman.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      822 2023-07-07 16:14:17.000000 hspylib-setman-0.9.9/setman/core/setman_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1406 2023-07-05 22:27:05.000000 hspylib-setman-0.9.9/setman/core/setman_enums.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-07-07 18:28:10.583726 hspylib-setman-0.9.9/setman/settings/
+-rw-r--r--   0 hjunior    (504) staff       (20)      256 2023-07-07 18:28:09.000000 hspylib-setman-0.9.9/setman/settings/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     9717 2023-07-07 18:23:30.000000 hspylib-setman-0.9.9/setman/settings/settings.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     1404 2023-07-05 17:37:53.000000 hspylib-setman-0.9.9/setman/settings/settings_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3427 2023-07-07 18:18:38.000000 hspylib-setman-0.9.9/setman/settings/settings_entry.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4106 2023-07-07 18:15:51.000000 hspylib-setman-0.9.9/setman/settings/settings_repository.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2119 2023-07-07 18:16:06.000000 hspylib-setman-0.9.9/setman/settings/settings_service.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      232 2023-07-06 19:46:06.000000 hspylib-setman-0.9.9/setman/welcome.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-07-07 18:28:10.586521 hspylib-setman-0.9.9/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     2067 2023-07-05 21:51:13.000000 hspylib-setman-0.9.9/setup.py
```

### Comparing `hspylib-setman-0.9.8/PKG-INFO` & `hspylib-setman-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.8
+Version: 0.9.9
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.8/README.md` & `hspylib-setman-0.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.8/hspylib_setman.egg-info/PKG-INFO` & `hspylib-setman-0.9.9/hspylib_setman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-setman
-Version: 0.9.8
+Version: 0.9.9
 Summary: HsPyLib - Settings Manager
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-setman/
@@ -26,12 +26,12 @@
 Description-Content-Type: text/markdown
 
 # HsPyLib - Settings Manager
 
 ## Manage your terminal settings
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.8/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.9/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-setman)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-setman-0.9.8/hspylib_setman.egg-info/SOURCES.txt` & `hspylib-setman-0.9.9/hspylib_setman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.8/setman/__classpath__.py` & `hspylib-setman-0.9.9/setman/__classpath__.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,8 +21,8 @@
     """TODO"""
 
     def __init__(self):
         super().__init__(get_path(__file__), get_path(run_dir()), (get_path(__file__) / "resources"))
 
 
 # Instantiate the classpath singleton
-_Classpath()
+assert _Classpath().INSTANCE is not None, "Failed to create Classpath instance"
```

### Comparing `hspylib-setman-0.9.8/setman/__main__.py` & `hspylib-setman-0.9.9/setman/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,27 @@
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-import logging as log
-import sys
-from textwrap import dedent
-
 from clitt.core.tui.tui_application import TUIApplication
 from hspylib.core.enums.charset import Charset
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.application.argparse.parser_action import ParserAction
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
-
 from setman.__classpath__ import _Classpath
 from setman.core.setman import Setman
 from setman.core.setman_enums import SetmanOps, SettingsType
+from textwrap import dedent
+
+import logging as log
+import sys
 
 
 class Main(TUIApplication):
     """HsPyLib CLI Terminal Tools - Create professional CLI applications."""
 
     # The welcome message
     DESCRIPTION = _Classpath.get_source_path("welcome.txt").read_text(encoding=Charset.UTF_8.val)
@@ -95,15 +94,15 @@
         st = self.get_arg("type")
         self._setman.execute(
             SetmanOps.of_value(op) if op else None,
             self.get_arg("name"),
             self.get_arg("value"),
             SettingsType.of_value(st) if st else None,
             self.get_arg("simple"),
-            self.get_arg("file")
+            self.get_arg("file"),
         )
 
         return ExitStatus.SUCCESS
 
 
 # Application entry point
 if __name__ == "__main__":
```

### Comparing `hspylib-setman-0.9.8/setman/core/setman.py` & `hspylib-setman-0.9.9/setman/core/setman.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,40 +8,39 @@
    @created: Fri, 29 May 2023
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-import atexit
-import logging as log
-import os
-from typing import Any
-
 from clitt.core.tui.table.table_enums import TextAlignment
 from clitt.core.tui.table.table_renderer import TableRenderer
 from hspylib.core.enums.charset import Charset
 from hspylib.core.exception.exceptions import InvalidArgumentError
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_state
 from hspylib.core.tools.commons import file_is_not_empty, syserr, sysout
 from hspylib.modules.application.application import Application
 from hspylib.modules.cli.keyboard import Keyboard
-
 from setman.core.setman_config import SetmanConfig
 from setman.core.setman_enums import SetmanOps, SettingsType
 from setman.settings.settings import Settings
+from typing import Any
+
+import atexit
+import logging as log
+import os
 
 
 class Setman(metaclass=Singleton):
     """HsPyLib application that helps managing system settings."""
 
     RESOURCE_DIR = os.environ.get("HHS_DIR", os.environ.get("HOME", "~/"))
 
-    SETMAN_CONFIG_FILE = f"setman.properties"
+    SETMAN_CONFIG_FILE = "setman.properties"
 
     SETMAN_DB_FILE = f"{RESOURCE_DIR}/.setman-db"
 
     def __init__(self, parent_app: Application) -> None:
         self._parent_app = parent_app
         cfg_file = f"{self.RESOURCE_DIR}/{self.SETMAN_CONFIG_FILE}"
         if not file_is_not_empty(cfg_file):
@@ -70,18 +69,18 @@
     def execute(
         self,
         operation: SetmanOps,
         name: str | None,
         value: Any | None,
         stype: SettingsType = None,
         simple_fmt: bool = False,
-        filepath: str = None
+        filepath: str = None,
     ) -> None:
         """Execute the specified operation."""
-        log.debug(f"{operation} Name: {name or '*'} Value: {value or '-'} SettingsType: {stype or '*'}")
+        log.debug("%s Name: %s Value: %s SettingsType: %s", operation, name or "*", "-", stype or "*")
         atexit.register(self.settings.close)
         with self.settings.open():
             match operation:
                 case SetmanOps.LIST:
                     self._list_settings(name, stype)
                 case SetmanOps.SEARCH:
                     self._search_settings(name or "*", stype, simple_fmt)
@@ -143,32 +142,36 @@
     def _search_settings(self, name: str | None, stype: SettingsType | None, simple_fmt: bool) -> None:
         """Search and display all settings matching criteria.
         :param name: the settings name to filter.
         :param stype: the settings type to filter.
         :param simple_fmt: whether to display simple or formatted.
         """
         data = list(map(lambda e: e.to_string(simple_fmt), self.settings.search(name, stype)))
-        sysout(os.linesep.join(data)) \
-            if data \
-            else sysout("%EOL%%YELLOW%No settings found matching: %WHITE%",
-                        f"[name={name or '*'}, stype={stype or '*'}]", "%EOL%")
+        sysout(
+            os.linesep.join(data) if data else "%EOL%%YELLOW%No settings found matching: %WHITE%",
+            f"[name={name or '*'}, stype={stype or '*'}]",
+            "%EOL%",
+        )
 
     def _clear_settings(self, name: str | None, stype: SettingsType | None) -> None:
         """Clear all settings.
         :param name: clear settings matching name.
         """
         if not name and not stype:
             sysout("%EOL%%ORANGE%All settings will be removed. Are you sure (y/[n])? ")
             if (keystroke := Keyboard.wait_keystroke()) and keystroke in [Keyboard.VK_y, Keyboard.VK_Y]:
                 self.settings.clear("*", stype)
                 sysout("%EOL%%ORANGE%!!! All settings have been removed !!!%EOL%")
         else:
             self.settings.clear(name, stype)
-            sysout("%EOL%%ORANGE%Removed settings matching: %WHITE%",
-                   f"[name={name or '*'}, stype={stype or '*'}]", "%EOL%")
+            sysout(
+                "%EOL%%ORANGE%Removed settings matching: %WHITE%",
+                f"[name={name or '*'}, stype={stype or '*'}]",
+                "%EOL%",
+            )
 
     def _import_settings(self, filepath: str) -> None:
         """Import settings from CSV file."""
         count = self.settings.import_csv(filepath)
         sysout(f"%EOL%%GREEN%Imported {count} settings from {filepath}! %EOL%")
 
     def _export_settings(self, filepath: str, name: str | None = None, stype: SettingsType | None = None) -> None:
@@ -176,9 +179,9 @@
         count = self.settings.export_csv(filepath, name, stype)
         sysout(f"%EOL%%GREEN%Exported {count} settings to {filepath}! %EOL%")
 
     def _setup(self, filepath: str) -> None:
         """Setup SetMan on the system."""
         with open(filepath, "w+", encoding=Charset.UTF_8.val) as f_configs:
             f_configs.write(f"hhs.setman.database = {self.SETMAN_DB_FILE} {os.linesep}")
-            f_configs.write(f"hhs.setman.encode.database = True")
+            f_configs.write("hhs.setman.encode.database = True")
             check_state(os.path.exists(filepath), "Unable to create Setman configuration file: " + filepath)
```

### Comparing `hspylib-setman-0.9.8/setman/core/setman_config.py` & `hspylib-setman-0.9.9/setman/core/setman_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
 from hspylib.core.tools.commons import str_to_bool
-
 from setman.settings.settings_config import SettingsConfig
 
 
 class SetmanConfig(SettingsConfig):
     """Holds the SetMan configurations."""
 
     def __init__(self, resource_dir: str, filename: str):
```

### Comparing `hspylib-setman-0.9.8/setman/core/setman_enums.py` & `hspylib-setman-0.9.9/setman/core/setman_enums.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.8/setman/settings/settings.py` & `hspylib-setman-0.9.9/setman/settings/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,35 +8,34 @@
    @created: Thu, 04 Jul 2023
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-import binascii
-import contextlib
-import csv
-import logging as log
-import os
-import uuid
-from functools import lru_cache
-from typing import Any, List, Optional, Tuple
-
 from datasource.identity import Identity
+from functools import lru_cache
 from hspylib.core.exception.exceptions import ApplicationError
 from hspylib.core.preconditions import check_argument, check_state
 from hspylib.core.tools.commons import dirname, file_is_not_empty, safe_delete_file, touch_file
 from hspylib.core.tools.text_tools import ensure_endswith
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.security.security import decode_file, encode_file
-
 from setman.core.setman_enums import SettingsType
 from setman.settings.settings_config import SettingsConfig
 from setman.settings.settings_entry import SettingsEntry
 from setman.settings.settings_service import SettingsService
+from typing import Any, List, Optional, Tuple
+
+import binascii
+import contextlib
+import csv
+import logging as log
+import os
+import uuid
 
 
 class Settings:
     """Class to provide settings interactions."""
 
     HEADERS = ["uuid", "name", "value", "settings type", "modified"]
 
@@ -46,20 +45,16 @@
         self._service = SettingsService(self.configs)
         if not file_is_not_empty(self.configs.database):
             self._create_db()
         self._limit = 500
         self._offset = 0
 
     def __str__(self):
-        entries = f",{os.linesep}  ".join(list(map(lambda s: str(s), self.search())))
-        return (
-            f"Settings: [{os.linesep + '  ' if entries else ''}"
-            f"{entries}"
-            f"{os.linesep if entries else ''}]"
-        )
+        entries = f",{os.linesep}  ".join(list(map(str, self.search())))
+        return f"Settings: [{os.linesep + '  ' if entries else ''}" f"{entries}" f"{os.linesep if entries else ''}]"
 
     def __repr__(self):
         return str(self)
 
     def __getitem__(self, name: str) -> SettingsEntry:
         return self.get(name)
 
@@ -85,15 +80,15 @@
     @property
     def is_open(self) -> bool:
         return self._is_open
 
     @is_open.setter
     def is_open(self, new_is_open: bool) -> None:
         self._is_open = new_is_open
-        log.debug(f"Settings database open: {self.configs.database}")
+        log.debug("Settings database open: %s", self.configs.database)
 
     @contextlib.contextmanager
     def open(self) -> None:
         """Decode and open the SQL lite database file. Return the context to manipulate it."""
         try:
             if not self.is_open:
                 self.is_open = True
@@ -113,15 +108,15 @@
     def close(self) -> None:
         """Encode and open the SQL lite database file. Return the context to manipulate it."""
         try:
             if self._is_open:
                 if self.configs.is_db_encoded:
                     self._encode_db_file()
                 self._is_open = False
-                log.debug(f"Settings database closed: {self.configs.database}")
+                log.debug("Settings database closed: %s", self.configs.database)
         except (UnicodeDecodeError, binascii.Error) as err:
             err_msg = f"Failed to close settings file => {self.configs.database}"
             raise ApplicationError(err_msg, err) from err
         except Exception as err:
             err_msg = f"Unable to close settings file => {self.configs.database}"
             raise ApplicationError(err_msg, err) from err
         finally:
@@ -131,29 +126,27 @@
     @lru_cache
     def get(self, name: str) -> Optional[SettingsEntry]:
         """Get setting matching the specified name.
         :param name: the settings name to get.
         """
         check_state(self.is_open, "Settings database is not open")
         if name:
-            return self._service.get(name)
+            return self._service.get_by_name(name)
         return None
 
     def upsert(
-        self,
-        name: str | None = None,
-        value: Any | None = None,
-        stype: SettingsType | None = None) -> Tuple[Optional[SettingsEntry], Optional[SettingsEntry]]:
+        self, name: str | None = None, value: Any | None = None, stype: SettingsType | None = None
+    ) -> Tuple[Optional[SettingsEntry], Optional[SettingsEntry]]:
         """Upsert the specified setting.
         :param name: the settings name.
         :param value: the settings value.
         :param stype: the settings type.
         """
         check_state(self.is_open, "Settings database is not open")
-        found = self._service.get(name)
+        found = self._service.get_by_name(name)
         entry = found or SettingsEntry(Identity(SettingsEntry.SetmanId(uuid.uuid4().hex)), name, value, stype)
         if not name or not value or not stype:
             entry = SettingsEntry.prompt(entry)
         if entry:
             entry.modified = now()
             self._service.save(entry)
             self._clear_caches()
@@ -161,15 +154,15 @@
 
     def remove(self, name: str) -> Optional[SettingsEntry]:
         """Delete the specified setting.
         :param name: the settings name to delete.
         """
         check_state(self.is_open, "Settings database is not open")
         if name:
-            found = self._service.get(name)
+            found = self._service.get_by_name(name)
             if found:
                 self._service.remove(found)
                 self._clear_caches()
                 return found
         return None
 
     @lru_cache(maxsize=500)
@@ -193,15 +186,15 @@
     def import_csv(self, filepath: str) -> int:
         """Upsert settings from CSV file into the database.
         :param filepath: the path of the CSV file to be imported.
         """
         count, csv_file = 0, ensure_endswith(filepath, ".csv")
         check_argument(os.path.exists(filepath), "CSV file does not exist: " + csv_file)
         with open(csv_file, encoding="UTF8") as f_csv:
-            csv_reader = csv.reader(f_csv, delimiter=',')
+            csv_reader = csv.reader(f_csv, delimiter=",")
             for row in csv_reader:
                 if row == self.HEADERS:
                     continue
                 uid, name, value, stype = str(row[0]), str(row[1]), str(row[2]), SettingsType.of_value(row[3])
                 entry = SettingsEntry(Identity(SettingsEntry.SetmanId(uid)), name, value, stype)
                 self._service.save(entry)
                 count += 1
@@ -214,15 +207,15 @@
         :param name: the settings name to filter.
         :param stype: the settings type to filter.
         """
         dest_dir, csv_file = dirname(filepath), ensure_endswith(filepath, ".csv")
         check_argument(os.path.exists(dest_dir), "Destination dir does not exist: " + dest_dir)
         settings = self.search(name, stype)
         with open(csv_file, "w", encoding="UTF8") as f_csv:
-            writer = csv.writer(f_csv, delimiter=',')
+            writer = csv.writer(f_csv, delimiter=",")
             writer.writerow(self.HEADERS)
             writer.writerows(list(map(lambda s: s.values, settings)))
             return len(settings)
 
     def _create_db(self) -> bool:
         """Create the settings SQLite DB file."""
         touch_file(self.configs.database)
```

### Comparing `hspylib-setman-0.9.8/setman/settings/settings_config.py` & `hspylib-setman-0.9.9/setman/settings/settings_config.py`

 * *Files identical despite different names*

### Comparing `hspylib-setman-0.9.8/setman/settings/settings_entry.py` & `hspylib-setman-0.9.9/setman/settings/settings_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,18 @@
 from clitt.core.tui.minput.menu_input import MenuInput
 from clitt.core.tui.minput.minput import minput
 from collections import namedtuple
 from datasource.crud_entity import CrudEntity
 from datasource.identity import Identity
 from hspylib.core.tools.text_tools import environ_name
 from hspylib.core.zoned_datetime import now
+from setman.core.setman_enums import SettingsType
 from textwrap import dedent
 from typing import Any, Optional, Union
 
-from setman.core.setman_enums import SettingsType
-
 
 class SettingsEntry(CrudEntity):
     """Represents the Settings domain object."""
 
     SetmanId = namedtuple("SetmanId", ["uuid"])
 
     # Setman entry display format.
@@ -101,9 +100,8 @@
         """Return the string representation of this entry."""
         if simple:
             return (
                 self._SIMPLE_FORMAT.format(environ_name(self.name), self.value)
                 if self.stype == SettingsType.ENVIRONMENT.val
                 else self._SIMPLE_FORMAT.format(self.name, self.value)
             )
-        else:
-            return self._DISPLAY_FORMAT.format(self.name, self.stype, self.value, self.modified)
+        return self._DISPLAY_FORMAT.format(self.name, self.stype, self.value, self.modified)
```

### Comparing `hspylib-setman-0.9.8/setman/settings/settings_repository.py` & `hspylib-setman-0.9.9/setman/settings/settings_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,41 +10,37 @@
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
 from datasource.identity import Identity
 from datasource.sqlite.sqlite_repository import SQLiteRepository
-from textwrap import dedent
-from typing import List, Optional
-
 from setman.core.setman_enums import SettingsType
 from setman.settings.settings_entry import SettingsEntry
+from textwrap import dedent
+from typing import List, Optional
 
 
 class SettingsRepository(SQLiteRepository[SettingsEntry]):
     """Provide CRUD operations for the Settings."""
 
     @property
     def database(self) -> str:
         return self._config.database
 
     def find_by_name(self, name: str) -> Optional[SettingsEntry]:
         """Find settings by name."""
-        sql = f"SELECT * FROM SETTINGS WHERE name = ? ORDER BY name"
+        sql = "SELECT * FROM SETTINGS WHERE name = ? ORDER BY name"
         result = next((e for e in self.execute(sql, name=name)[1]), None)
 
         return self.to_entity_type(result) if result else None
 
     def search(
-        self,
-        name: str | None = None,
-        stype: SettingsType | None = None,
-        limit: int = 500,
-        offset: int = 0) -> List[SettingsEntry]:
+        self, name: str | None = None, stype: SettingsType | None = None, limit: int = 500, offset: int = 0
+    ) -> List[SettingsEntry]:
         """Search settings by settings type."""
         search_name = name.replace("*", "%") if name else "%"
         if stype:
             sql = f"SELECT * FROM SETTINGS WHERE name LIKE ? AND stype = ? ORDER BY name LIMIT {limit} OFFSET {offset}"
             result = self.execute(sql, name=search_name, stype=stype.val)[1] or []
         else:
             sql = f"SELECT * FROM SETTINGS WHERE name LIKE ? ORDER BY name LIMIT {limit} OFFSET {offset}"
```

### Comparing `hspylib-setman-0.9.8/setman/settings/settings_service.py` & `hspylib-setman-0.9.9/setman/settings/settings_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,42 +8,35 @@
    @created: Mon, 5 Jun 2023
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
    Copyright 2023, HsPyLib team
 """
-from typing import List, Optional
-
 from datasource.crud_service import CrudService
-
 from setman.core.setman_enums import SettingsType
 from setman.settings.settings_config import SettingsConfig
 from setman.settings.settings_entry import SettingsEntry
 from setman.settings.settings_repository import SettingsRepository
+from typing import List, Optional
 
 
 class SettingsService(CrudService[SettingsRepository, SettingsEntry]):
     """Provides a CRUD service for the Setman application."""
 
     def __init__(self, setman_config: SettingsConfig):
         super().__init__(SettingsRepository(setman_config))
 
-    def get(self, name: str) -> Optional[SettingsEntry]:
+    def get_by_name(self, name: str) -> Optional[SettingsEntry]:
         """Get settings entry matching the specified name.
         :param name: the setting name to get.
         """
         return self.repository.find_by_name(name)
 
-    def search(
-        self,
-        name: str,
-        stype: SettingsType = None,
-        limit: int = 500,
-        offset: int = 0) -> List[SettingsEntry]:
+    def search(self, name: str, stype: SettingsType = None, limit: int = 500, offset: int = 0) -> List[SettingsEntry]:
         """Search settings matching the specified name.
         :param name: the settings name to filter.
         :param stype: the settings type to filter.
         :param limit: the max amount of records to search.
         :param offset: the records offset from which to search.
         """
         return self.repository.search(name, stype, limit, offset)
```

### Comparing `hspylib-setman-0.9.8/setup.py` & `hspylib-setman-0.9.9/setup.py`

 * *Files identical despite different names*

