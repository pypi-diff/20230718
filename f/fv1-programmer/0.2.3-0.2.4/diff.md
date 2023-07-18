# Comparing `tmp/fv1_programmer-0.2.3.tar.gz` & `tmp/fv1_programmer-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fv1_programmer-0.2.3.tar", max compression
+gzip compressed data, was "fv1_programmer-0.2.4.tar", max compression
```

## Comparing `fv1_programmer-0.2.3.tar` & `fv1_programmer-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1065 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/LICENSE
--rw-r--r--   0        0        0      613 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/README.md
--rw-r--r--   0        0        0     1140 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/adaptor/adapter.py
--rw-r--r--   0        0        0     1083 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/adaptor/mcp2221.py
--rw-r--r--   0        0        0       30 2023-07-14 01:34:50.892645 fv1_programmer-0.2.3/asfv1/.git
--rw-r--r--   0        0        0     1157 2023-07-14 01:34:51.748662 fv1_programmer-0.2.3/asfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-07-14 01:34:51.748662 fv1_programmer-0.2.3/asfv1/LICENSE
--rw-r--r--   0        0        0    36334 2023-07-14 01:34:51.748662 fv1_programmer-0.2.3/asfv1/README.md
--rw-r--r--   0        0        0    54482 2023-07-14 01:34:51.752662 fv1_programmer-0.2.3/asfv1/asfv1.py
--rw-r--r--   0        0        0      561 2023-07-14 01:34:51.752662 fv1_programmer-0.2.3/asfv1/example.asm
--rw-r--r--   0        0        0      801 2023-07-14 01:34:51.752662 fv1_programmer-0.2.3/asfv1/setup.py
--rw-r--r--   0        0        0       31 2023-07-14 01:34:51.168650 fv1_programmer-0.2.3/disfv1/.git
--rw-r--r--   0        0        0     1157 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/.gitignore
--rw-r--r--   0        0        0     1075 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/LICENSE
--rw-r--r--   0        0        0     4816 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/README.md
--rw-r--r--   0        0        0    17532 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/disfv1.py
--rw-r--r--   0        0        0      512 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/example.bin
--rw-r--r--   0        0        0      798 2023-07-14 01:34:51.756662 fv1_programmer-0.2.3/disfv1/setup.py
--rw-r--r--   0        0        0     6747 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/eeprom/eeprom.py
--rw-r--r--   0        0        0     1780 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/fv1.py
--rw-r--r--   0        0        0     3429 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/main.py
--rw-r--r--   0        0        0     2906 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/tui.css
--rw-r--r--   0        0        0    13468 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/fv1_programmer/tui.py
--rw-r--r--   0        0        0     1274 2023-07-14 01:34:50.548638 fv1_programmer-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 fv1_programmer-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-18 02:11:22.176540 fv1_programmer-0.2.4/LICENSE
+-rw-r--r--   0        0        0      613 2023-07-18 02:11:22.176540 fv1_programmer-0.2.4/README.md
+-rw-r--r--   0        0        0     1140 2023-07-18 02:11:22.176540 fv1_programmer-0.2.4/adaptor/adapter.py
+-rw-r--r--   0        0        0     1083 2023-07-18 02:11:22.176540 fv1_programmer-0.2.4/adaptor/mcp2221.py
+-rw-r--r--   0        0        0       30 2023-07-18 02:11:22.524545 fv1_programmer-0.2.4/asfv1/.git
+-rw-r--r--   0        0        0     1157 2023-07-18 02:11:23.316540 fv1_programmer-0.2.4/asfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-07-18 02:11:23.316540 fv1_programmer-0.2.4/asfv1/LICENSE
+-rw-r--r--   0        0        0    36334 2023-07-18 02:11:23.316540 fv1_programmer-0.2.4/asfv1/README.md
+-rw-r--r--   0        0        0    54482 2023-07-18 02:11:23.316540 fv1_programmer-0.2.4/asfv1/asfv1.py
+-rw-r--r--   0        0        0      561 2023-07-18 02:11:23.316540 fv1_programmer-0.2.4/asfv1/example.asm
+-rw-r--r--   0        0        0      801 2023-07-18 02:11:23.316540 fv1_programmer-0.2.4/asfv1/setup.py
+-rw-r--r--   0        0        0       31 2023-07-18 02:11:22.792543 fv1_programmer-0.2.4/disfv1/.git
+-rw-r--r--   0        0        0     1157 2023-07-18 02:11:23.320540 fv1_programmer-0.2.4/disfv1/.gitignore
+-rw-r--r--   0        0        0     1075 2023-07-18 02:11:23.320540 fv1_programmer-0.2.4/disfv1/LICENSE
+-rw-r--r--   0        0        0     4816 2023-07-18 02:11:23.320540 fv1_programmer-0.2.4/disfv1/README.md
+-rw-r--r--   0        0        0    17532 2023-07-18 02:11:23.320540 fv1_programmer-0.2.4/disfv1/disfv1.py
+-rw-r--r--   0        0        0      512 2023-07-18 02:11:23.320540 fv1_programmer-0.2.4/disfv1/example.bin
+-rw-r--r--   0        0        0      798 2023-07-18 02:11:23.320540 fv1_programmer-0.2.4/disfv1/setup.py
+-rw-r--r--   0        0        0     6747 2023-07-18 02:11:22.180540 fv1_programmer-0.2.4/eeprom/eeprom.py
+-rw-r--r--   0        0        0     1780 2023-07-18 02:11:22.180540 fv1_programmer-0.2.4/fv1_programmer/fv1.py
+-rw-r--r--   0        0        0     3429 2023-07-18 02:11:22.180540 fv1_programmer-0.2.4/fv1_programmer/main.py
+-rw-r--r--   0        0        0     2709 2023-07-18 02:11:22.180540 fv1_programmer-0.2.4/fv1_programmer/tui.css
+-rw-r--r--   0        0        0    13652 2023-07-18 02:11:22.180540 fv1_programmer-0.2.4/fv1_programmer/tui.py
+-rw-r--r--   0        0        0     1274 2023-07-18 02:11:22.180540 fv1_programmer-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 fv1_programmer-0.2.4/PKG-INFO
```

### Comparing `fv1_programmer-0.2.3/LICENSE` & `fv1_programmer-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/README.md` & `fv1_programmer-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/adaptor/adapter.py` & `fv1_programmer-0.2.4/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/adaptor/mcp2221.py` & `fv1_programmer-0.2.4/adaptor/mcp2221.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/asfv1/.gitignore` & `fv1_programmer-0.2.4/asfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/asfv1/LICENSE` & `fv1_programmer-0.2.4/asfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/asfv1/README.md` & `fv1_programmer-0.2.4/asfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/asfv1/asfv1.py` & `fv1_programmer-0.2.4/asfv1/asfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/asfv1/example.asm` & `fv1_programmer-0.2.4/asfv1/example.asm`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/asfv1/setup.py` & `fv1_programmer-0.2.4/asfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/disfv1/.gitignore` & `fv1_programmer-0.2.4/disfv1/.gitignore`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/disfv1/LICENSE` & `fv1_programmer-0.2.4/disfv1/LICENSE`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/disfv1/README.md` & `fv1_programmer-0.2.4/disfv1/README.md`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/disfv1/disfv1.py` & `fv1_programmer-0.2.4/disfv1/disfv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/disfv1/setup.py` & `fv1_programmer-0.2.4/disfv1/setup.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/eeprom/eeprom.py` & `fv1_programmer-0.2.4/eeprom/eeprom.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/fv1_programmer/fv1.py` & `fv1_programmer-0.2.4/fv1_programmer/fv1.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/fv1_programmer/main.py` & `fv1_programmer-0.2.4/fv1_programmer/main.py`

 * *Files identical despite different names*

### Comparing `fv1_programmer-0.2.3/fv1_programmer/tui.css` & `fv1_programmer-0.2.4/fv1_programmer/tui.css`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 *  {
     transition: background 500ms in_out_cubic, color 500ms in_out_cubic;
 }
 
 Screen {
-    layers: base overlay top notifications;
+    layers: base overlay top;
     overflow: hidden;
 }
 
 Footer {
     layer: top;
 }
 
-Notification {
-    dock: bottom;
-    layer: notification;
-    width: auto;
-    margin: 2 4;
-    padding: 1 2;
-    background: $background;
-    color: $text;
-    height: auto;
-    
-}
-
 Sidebar {
     width: 40;
     background: $panel;
     transition: offset 500ms in_out_cubic;
     layer: overlay;
 
 }
```

### Comparing `fv1_programmer-0.2.3/fv1_programmer/tui.py` & `fv1_programmer-0.2.4/fv1_programmer/tui.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         markdown = '# No program specified (leave this slot untouched)'
         if new_program is not None:
             markdown = new_program.as_markdown()
 
         self.query_one(Markdown).update(markdown)
 
     def on_mount(self) -> None:
-        self.query_one(Markdown).tooltip = """Ctrl+C - Copy to clipboard\nCtrl+T - Paste from clipboard\nCtrl+D - Delete this program"""
+        self.query_one(Markdown).tooltip = """Ctrl+C - Copy to clipboard\nCtrl+V/Ctrl+T - Paste from clipboard\nCtrl+D - Delete this program"""
 
 class ProgramTabs(Widget):
     def compose(self) -> ComposeResult:  
         with TabbedContent():
             with TabPane("Program 1", id="prog1"):
                 yield FV1ProgramPane(id="fv1prog1")
             with TabPane("Program 2", id="prog2"):
@@ -180,14 +180,15 @@
     BINDINGS = [
         # ("ctrl+l", "load_file", "Load File"),
         # ("ctrl+r", "read_eeprom", "Read EEPROM"),
         ("ctrl+w", "write_eeprom", "Write EEPROM"),
         ("f1", "app.toggle_class('TextLog', '-hidden')", "Show Log"),
         ("f2", "toggle_sidebar", "Settings"),
         ("ctrl+q", "request_quit", "Quit"),
+        Binding("ctrl+v", "paste", "Paste", show=False, priority=True),
         Binding("ctrl+t", "paste", "Paste", show=False, priority=True),
         Binding("ctrl+d", "delete", "Delete Program", show=False, priority=True),
     ]
 
     show_sidebar = reactive(False)
 
     def compose(self) -> ComposeResult:
@@ -239,53 +240,54 @@
             program_pane = self.query_one(f"#fv1prog{i}", FV1ProgramPane)
             if program_pane.program is not None:
                 bin_array, warnings, errors = program_pane.program.assemble(
                                                             clamp=self.app.setting_asfv1_clamp,
                                                             spinreals=self.app.setting_asfv1_spinreals)
                 programs.append({"program": i, "address" : (i - 1)*512, "data" : bin_array})
         if len(programs) == 0:
-            self.app.notify("Nothing to do!")
+            self.app.show_toast("Nothing to do!", severity="warning")
         else:
             eeprom = None
             if self.app.setting_simulate:
                 from eeprom.eeprom import DummyEEPROM
                 eeprom = DummyEEPROM(Path('sim.bin'), 4096)
             else:
                 from adaptor.mcp2221 import MCP2221I2CAdaptor
                 from eeprom.eeprom import I2CEEPROM
                 adaptor = MCP2221I2CAdaptor(0x50, i2c_clock_speed=100000)
                 try:
                     adaptor.open()
                     eeprom = I2CEEPROM(adaptor, 4096, page_size_in_bytes=32)
-                except:
-                    self.app.notify("Failed to find an FV-1 programmer!")
+                except Exception as e:
+                    self.app.logger.error(str(e))
+                    self.app.show_toast("Failed to find Easy Spin! See log for details.", title="Error", severity="error")
 
             if eeprom is not None:
                 total_bytes = 0
                 for program in programs:
                     addr = program["address"]
                     data = program["data"]
                     eeprom.write_bytes(addr, data)
                     total_bytes += len(data)
-                    self.app.notify(f"Wrote {len(data)} bytes to program {addr // 512 + 1}")
+                    # self.app.show_toast(f"Wrote {len(data)} bytes to program {addr // 512 + 1}")
 
-                self.app.notify(f"Wrote {total_bytes} bytes to program slots {[w['program'] for w in programs]}{' (simulation)' if self.app.setting_simulate else ''}")
+                self.app.show_toast(f"Wrote {total_bytes} bytes to program slots {[w['program'] for w in programs]}{' (simulation)' if self.app.setting_simulate else ''}")
 
     def action_paste(self) -> None:
         # Validate program
         new_program = FV1Program(pyperclip.paste())
         bin_array, warnings, errors = new_program.assemble(clamp=self.app.setting_asfv1_clamp,
                                                            spinreals=self.app.setting_asfv1_spinreals)
         [self.app.logger.info(w) for w in warnings]
         [self.app.logger.info(e) for e in errors]
         if len(errors) == 0:
             active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
             active_program_pane.program = FV1Program(pyperclip.paste())
         else:
-            self.app.notify("Ignoring invalid clipboard contents")
+            self.app.show_toast("Ignoring invalid clipboard contents. See log for details.")
 
     def action_delete(self) -> None:
         active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
         active_program_pane.program = None
 
 
 from dataclasses import dataclass
@@ -301,22 +303,14 @@
     load_File:Path
     save_File:Path
     verify:bool
     debug:bool
     sim:bool
 
 
-class Notification(Static):
-    def on_mount(self) -> None:
-        self.set_timer(3, self.remove)
-
-    def on_click(self) -> None:
-        self.remove()
-
-
 class FV1App(App[None]):
     CSS_PATH = "tui.css"
     SCREENS = {"main" : MainScreen()}
 
     def __init__(self, cmdline_args=None, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         self.cmdline_args = cmdline_args
@@ -360,18 +354,18 @@
 
     # Intercept the app exit (the only thing connected to this should be Ctrl+C)
     # and make it behave like Copy
     def exit(self, result = None) -> None:
         active_program_pane = self.query_one(f"#fv1{self.query_one(TabbedContent).active}", FV1ProgramPane)
         if active_program_pane.program is not None:
             pyperclip.copy(active_program_pane.program.asm)
-            self.notify("Current program copied to clipboard")
+            self.show_toast("Current program copied to clipboard")
 
     def do_exit(self, result = None) -> None:
         super().exit(result)
 
     def on_mount(self) -> None:
         self.push_screen("main")
 
-    def notify(self, message) -> None:
+    def show_toast(self, message, title=None, severity="information", timeout=4.0) -> None:
         self.logger.info(message)
-        self.screen.mount(Notification(message))
+        self.notify(message, title=title, severity=severity, timeout=timeout)
```

### Comparing `fv1_programmer-0.2.3/pyproject.toml` & `fv1_programmer-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fv1-programmer"
-version = "0.2.3"
+version = "0.2.4"
 description = "An EEPROM programming tool for the FV-1 DSP"
 authors = ["Mark Melvin <mark.melvin@audiofab.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
@@ -25,15 +25,15 @@
     {include = "adaptor"},
     {include = "asfv1"},
     {include = "disfv1"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-textual = {extras = ["dev"], version = "^0.28.1"}
+textual = {extras = ["dev"], version = "^0.30.0"}
 easymcp2221 = "^1.6.2"
 intelhex = "^2.3.0"
 pyperclip = "^1.8.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
```

### Comparing `fv1_programmer-0.2.3/PKG-INFO` & `fv1_programmer-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fv1-programmer
-Version: 0.2.3
+Version: 0.2.4
 Summary: An EEPROM programming tool for the FV-1 DSP
 License: MIT
 Author: Mark Melvin
 Author-email: mark.melvin@audiofab.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: easymcp2221 (>=1.6.2,<2.0.0)
 Requires-Dist: intelhex (>=2.3.0,<3.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
-Requires-Dist: textual[dev] (>=0.28.1,<0.29.0)
+Requires-Dist: textual[dev] (>=0.30.0,<0.31.0)
 Description-Content-Type: text/markdown
 
 # FV-1 Programmer
 
 An EEPROM programming tool for the FV-1 DSP.
 
 # Installation
```

