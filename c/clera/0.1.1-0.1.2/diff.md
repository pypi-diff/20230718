# Comparing `tmp/clera-0.1.1.tar.gz` & `tmp/clera-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clera-0.1.1.tar", last modified: Tue Jul 11 01:05:44 2023, max compression
+gzip compressed data, was "clera-0.1.2.tar", last modified: Tue Jul 18 10:41:16 2023, max compression
```

## Comparing `clera-0.1.1.tar` & `clera-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,37 @@
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.432115 clera-0.1.1/
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1622 2023-07-11 00:59:12.000000 clera-0.1.1/CHANGELOG.md
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-04-23 00:22:42.000000 clera-0.1.1/LICENCE.txt
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)       42 2023-07-11 00:59:20.000000 clera-0.1.1/MANIFEST.in
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3539 2023-07-11 01:05:44.432115 clera-0.1.1/PKG-INFO
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1279 2023-07-08 18:13:25.000000 clera-0.1.1/README.md
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.416115 clera-0.1.1/clera/
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      161 2023-07-11 01:01:47.000000 clera-0.1.1/clera/__init__.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    61327 2023-07-11 01:03:32.000000 clera-0.1.1/clera/core.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.428115 clera-0.1.1/clera/icons/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       65 2023-07-04 11:49:49.000000 clera-0.1.1/clera/icons/__init__.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16293 2023-06-19 11:40:22.000000 clera-0.1.1/clera/icons/add-file.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13782 2023-06-19 03:37:40.000000 clera-0.1.1/clera/icons/close.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13430 2023-06-19 11:40:48.000000 clera-0.1.1/clera/icons/document.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16420 2023-06-19 03:41:00.000000 clera-0.1.1/clera/icons/documents.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15098 2023-06-19 03:38:16.000000 clera-0.1.1/clera/icons/gear.png
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)   290225 2023-02-13 13:07:36.000000 clera-0.1.1/clera/icons/hand-drawn-icon.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13536 2023-06-19 03:36:08.000000 clera-0.1.1/clera/icons/off.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    14518 2023-06-19 03:36:42.000000 clera-0.1.1/clera/icons/on.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    15585 2023-06-19 03:38:52.000000 clera-0.1.1/clera/icons/save-as.png
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    13421 2023-06-19 03:38:40.000000 clera-0.1.1/clera/icons/save.png
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)    41561 2023-04-25 04:20:56.000000 clera-0.1.1/clera/icons/toon-icon.ico
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.428115 clera-0.1.1/clera/scripts/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       21 2023-07-11 01:02:09.000000 clera-0.1.1/clera/scripts/__init__.py
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16531 2023-07-11 00:26:54.000000 clera-0.1.1/clera/scripts/editor.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.432115 clera-0.1.1/clera/utils/
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      120 2023-07-04 11:49:58.000000 clera-0.1.1/clera/utils/__init__.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      129 2023-03-24 12:03:54.000000 clera-0.1.1/clera/utils/exceptions.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    19722 2023-07-05 13:58:59.000000 clera-0.1.1/clera/utils/handlers.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     1071 2023-03-19 13:17:06.000000 clera-0.1.1/clera/utils/keys.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     6431 2023-07-02 16:17:50.000000 clera-0.1.1/clera/utils/procr.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     4295 2023-07-03 00:25:19.000000 clera-0.1.1/clera/utils/style.py
--rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    27822 2023-07-09 13:18:50.000000 clera-0.1.1/clera/widgets.py
-drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-11 01:05:44.420115 clera-0.1.1/clera.egg-info/
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     3539 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/PKG-INFO
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      751 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/SOURCES.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/dependency_links.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       46 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/entry_points.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        8 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/requires.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        6 2023-07-11 01:05:43.000000 clera-0.1.1/clera.egg-info/top_level.txt
--rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-11 01:05:44.432115 clera-0.1.1/setup.cfg
--rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1340 2023-07-11 00:58:31.000000 clera-0.1.1/setup.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 10:41:16.807504 clera-0.1.2/
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1622 2023-07-11 00:59:12.000000 clera-0.1.2/CHANGELOG.md
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     7651 2023-04-23 00:22:42.000000 clera-0.1.2/LICENCE.txt
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)       42 2023-07-11 00:59:20.000000 clera-0.1.2/MANIFEST.in
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2264 2023-07-18 10:41:16.807504 clera-0.1.2/PKG-INFO
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1629 2023-07-18 10:38:24.000000 clera-0.1.2/README.md
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 10:41:16.667555 clera-0.1.2/clera/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      194 2023-07-18 10:15:06.000000 clera-0.1.2/clera/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    61352 2023-07-18 10:21:42.000000 clera-0.1.2/clera/core.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 10:41:16.727533 clera-0.1.2/clera/icons/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      696 2023-07-18 09:59:04.000000 clera-0.1.2/clera/icons/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)   618709 2023-07-14 03:30:33.000000 clera-0.1.2/clera/icons/data.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 10:41:16.731532 clera-0.1.2/clera/scripts/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       21 2023-07-14 02:43:52.000000 clera-0.1.2/clera/scripts/__init__.py
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    16940 2023-07-18 10:12:43.000000 clera-0.1.2/clera/scripts/editor.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 10:41:16.803506 clera-0.1.2/clera/stubs/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       43 2023-07-03 14:47:26.000000 clera-0.1.2/clera/stubs/__init__.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)    11965 2023-07-18 10:19:27.000000 clera-0.1.2/clera/stubs/core.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     1272 2023-07-18 10:17:55.000000 clera-0.1.2/clera/stubs/handlers.pyi
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     7669 2023-07-08 14:35:34.000000 clera-0.1.2/clera/stubs/widgets.pyi
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 10:41:16.807504 clera-0.1.2/clera/utils/
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      120 2023-07-04 11:49:58.000000 clera-0.1.2/clera/utils/__init__.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)      129 2023-03-24 12:03:54.000000 clera-0.1.2/clera/utils/exceptions.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    20153 2023-07-18 09:56:45.000000 clera-0.1.2/clera/utils/handlers.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     1071 2023-03-19 13:17:06.000000 clera-0.1.2/clera/utils/keys.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     6431 2023-07-02 16:17:50.000000 clera-0.1.2/clera/utils/procr.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)     4295 2023-07-03 00:25:19.000000 clera-0.1.2/clera/utils/style.py
+-rw-rw-r--   0 eirasmx   (1000) eirasmx   (1000)    27822 2023-07-09 13:18:50.000000 clera-0.1.2/clera/widgets.py
+drwxr-xr-x   0 eirasmx   (1000) eirasmx   (1000)        0 2023-07-18 10:41:16.727533 clera-0.1.2/clera.egg-info/
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)     2264 2023-07-18 10:41:15.000000 clera-0.1.2/clera.egg-info/PKG-INFO
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)      605 2023-07-18 10:41:15.000000 clera-0.1.2/clera.egg-info/SOURCES.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        1 2023-07-18 10:41:15.000000 clera-0.1.2/clera.egg-info/dependency_links.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       46 2023-07-18 10:41:15.000000 clera-0.1.2/clera.egg-info/entry_points.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)        8 2023-07-18 10:41:15.000000 clera-0.1.2/clera.egg-info/requires.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       56 2023-07-18 10:41:15.000000 clera-0.1.2/clera.egg-info/top_level.txt
+-rw-r--r--   0 eirasmx   (1000) eirasmx   (1000)       38 2023-07-18 10:41:16.807504 clera-0.1.2/setup.cfg
+-rwxrwxrwx   0 eirasmx   (1000) eirasmx   (1000)     1994 2023-07-18 00:27:57.000000 clera-0.1.2/setup.py
```

### Comparing `clera-0.1.1/CHANGELOG.md` & `clera-0.1.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `clera-0.1.1/LICENCE.txt` & `clera-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `clera-0.1.1/README.md` & `clera-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 
 ---
 
 Clera provides platform for developing python GUI quickly and simply with low learning curve.
 
 <br>
 
+> **NOTE:** Clera is still in the **alpha** stage which means development is not complete its undergoing internal tests and development.
+
+<br>
+
 ## **THE BASICS**
 
 ### **Installation**
 
 ```bash
 pip install clera
 ```
@@ -58,12 +62,16 @@
 
 - Windows
 - Mac
 - Linux
 
 <br>
 
-> INFO: Visit https://cleragui.github.io/ for documentation and more information.
+To run the clera style editor, run "**clera-editor**" in the terminal or command prompt. Also to see a sample of what clera is capable of, check out the editor. Its developed with clera!
+
+<br>
+
+> **INFO:** Visit https://cleragui.github.io/ for documentation and more information.
 
 <br>
 
 ---
```

### Comparing `clera-0.1.1/clera/core.py` & `clera-0.1.2/clera/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     'Textarea', 'textarea', 'item', 'empty', 'separator', 'Exit', 'exit', 'Copy', 'copy', 'Cut', 'cut',
     'Paste', 'paste', 'Undo', 'undo', 'Redo', 'redo', 'link', 'ListWidget', 'listwidget', 'ListItem',
     'tab', 'TabWidget', 'tabwidget', 'Select', 'select', 'option', 'ProgressBar', 'progressbar',
     'Slider', 'slider', 'Dial', 'dial', 'Popup', 'popup', 'call', 'Titlebar', 'titlebar', 'File', 'file',
     'Folder', 'folder', 'ScrollArea', 'scrollarea', 'minimize', 'maximize', 'close', 'title', 'Highlight',
     'r', 'Stack', 'expand', 'fixed', 'vertical', 'horizontal', 'top', 'bottom', 'left', 'right', 'center',
     'vcenter', 'hcenter', 'justify', 'static', 'normal', 'standard', 'password', 'noecho', 'extended',
-    'noselection', 'multi', 'single', 'windows', 'fusion', 'curve', 'breeze', 'oxygen','circle', 'square'
+    'noselection', 'multi', 'single', 'windows', 'fusion', 'curve', 'breeze', 'oxygen','circle', 'square',
+    'encode', 'decode',
 ]
 
 
 app = start()
 
 DEFAULT_WINDOW_LAYOUT = QWidget()
```

### Comparing `clera-0.1.1/clera/scripts/editor.py` & `clera-0.1.2/clera/scripts/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,17 +204,23 @@
     window = Window(content_margin=0, frame=False, movable=True, fixed_size=(420, 270), spacing=0)
     line_width = make_line_width()
 
     settings_styling = f'''
         font-size: {MAIN['size']}px;
         font-family: {MAIN['font_family']};
     '''
-
+    win_color = 'rgb(19, 19, 19)'
+    txt_color = 'rgb(23, 23, 23)'
     css = f'''
+    window [
+        background: {win_color};
+    ]
+
     button [
+        color: white;
         border: 0px solid;
         padding: 3px 2px;
     ]
 
     select [
         height: 25px;
     ]
@@ -239,24 +245,32 @@
         height: 0px;
     ]
 
     scrollbar::sub-line:vertical [
         height: 0px;
     ]
 
+    popup [
+        color: white;
+        background: {win_color};
+    ]
+
     line [
         max-width: {line_width};
         border: 0px solid;
         background: rgb(19, 19, 19);
         color: rgb(131, 130, 130);
         {settings_styling}
     ]
 
     txt [
+        color: white;
         {settings_styling}
+        background: {txt_color};
+        border: 0px;
     ]
 
     scrollbar:horizontal [
         background: rgba(0, 0, 0, 0);
         margin: 0;
         max-height: 5px;
     ]
@@ -311,15 +325,15 @@
             file, format = File.save(filter=allow)
             file_path[0] = file
             if file.strip().endswith('cx'):
                 ...
             else:
                 file = f'{file.strip()}.cx'
 
-            if len(file) != 0:
+            if len(file.removesuffix('.cx')) != 0:
                 with open(file, 'w') as file:
                     file.write(str(textarea))
                     editor_state[0] = False
                     GET('line').style('border-right: 0px;')
                     return True
             else:
                 return False
@@ -373,22 +387,23 @@
                 else:
                     if action == 'open':
                         handle_open()
                     elif action == 'exit':
                         window.quit()
 
             warning = [
-                [Text('Do you want to Save Document?')],
+                [Text('Do you want to Save Document?', id='save-msg')],
                 [Button('Save', save, id='popup-save'), Button("Don't Save", dont_save, id='popup-d-save'), Button('Cancel', cancel,id='popup-cancel', shortcut='Esc')]
             ]
 
             Popup('Notification', warning, modal=True, id='warning-popup', lock=True)
             GET('popup-save').style(POPUP_STYLING)
             GET('popup-d-save').style(POPUP_STYLING)
             GET('popup-cancel').style(POPUP_STYLING)
+            GET('save-msg').style('color: white;')
 
 
         
         def handle_save():
             if file_path[0] != None and len(file_path[0])  != 0:
                 with open(file_path[0], 'w') as file:
                     file.write(str(textarea))
@@ -443,19 +458,19 @@
 
     def switch():
         current_state = state[0]
         _switch = GET('switch')
         _textarea = GET('txt')
 
         if current_state == 'on':
-            _switch.icon('icons/off.png')
+            _switch.icon(f'{DIR_NAME}/../icons/off.png')
             state[0] = 'off'
             _textarea.disable()
         elif current_state == 'off':
-            _switch.icon('icons/on.png')
+            _switch.icon(f'{DIR_NAME}/../icons/on.png')
             state[0] = 'on'
             _textarea.enable()
 
     def settings():
         def pop_action(action):
             popup = GET('settings')
 
@@ -535,14 +550,15 @@
     # Textarea('line', disabled=True, value='1'), 
 
     Box([[Textarea('line', disabled=True, value='1'), Textarea('txt', text_changed=changed, wordwrap=False)]])
 
     GET('txt').scrollbar(GET('line').scrollbar(id='scroll'))
     GET('line').alignment('right')
 
+
     keywords = [
         'button', 
         'text', 
         'input', 
         'checkbox', 
         'radiobutton',
         'toolbar',
```

### Comparing `clera-0.1.1/clera/utils/handlers.py` & `clera-0.1.2/clera/utils/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import os.path as path
 import sys
 import inspect
+import base64 
 import re
 
 from PySide6.QtGui import QAction, QIcon, Qt, QTextCharFormat, QColor,QKeyEvent
 from PySide6.QtWidgets import QSizePolicy, QApplication
 from PySide6.QtWidgets import QListWidgetItem, QAbstractItemView, QComboBox
 
 from ..icons import *
@@ -757,7 +758,25 @@
             format.setBackground(background)
             
     return format
 
 def r(list: list = None):
     if list != None:
         return '|'.join([fr'\b{list[i]}\b' for i in range(len(list))])
+
+def encode(path):
+    path = str(path)
+    
+    if os.path.isfile(path):
+        with open(path, 'rb') as image:
+            BASE_64 = base64.b64encode(image.read())
+
+        return BASE_64
+
+def decode(byte, path: str = 'image.png', write: bool = False):
+    BASE_64 = base64.b64decode(byte)
+    
+    if write == True:
+        with open(path, 'wb') as image:
+                image.write(BASE_64)
+
+    return BASE_64
```

### Comparing `clera-0.1.1/clera/utils/keys.py` & `clera-0.1.2/clera/utils/keys.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.1/clera/utils/procr.py` & `clera-0.1.2/clera/utils/procr.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.1/clera/utils/style.py` & `clera-0.1.2/clera/utils/style.py`

 * *Files identical despite different names*

### Comparing `clera-0.1.1/clera/widgets.py` & `clera-0.1.2/clera/widgets.py`

 * *Files identical despite different names*

