# Comparing `tmp/SherLocking-0.0.2.tar.gz` & `tmp/SherLocking-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SherLocking-0.0.2.tar", last modified: Tue Jul 18 17:39:28 2023, max compression
+gzip compressed data, was "SherLocking-0.0.3.tar", last modified: Tue Jul 18 18:00:35 2023, max compression
```

## Comparing `SherLocking-0.0.2.tar` & `SherLocking-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:39:28.304547 SherLocking-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-07-18 04:42:39.000000 SherLocking-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      558 2023-07-18 17:39:28.304547 SherLocking-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-18 04:42:44.000000 SherLocking-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 17:39:28.237273 SherLocking-0.0.2/SherLocking/
--rw-rw-rw-   0        0        0       24 2023-07-18 05:28:28.000000 SherLocking-0.0.2/SherLocking/__init__.py
--rw-rw-rw-   0        0        0     5154 2023-07-18 17:37:47.000000 SherLocking-0.0.2/SherLocking/activation.py
--rw-rw-rw-   0        0        0     1286 2023-07-18 06:53:24.000000 SherLocking-0.0.2/SherLocking/config.py
--rw-rw-rw-   0        0        0     2140 2023-07-18 17:36:22.000000 SherLocking-0.0.2/SherLocking/file.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:39:28.304547 SherLocking-0.0.2/SherLocking.egg-info/
--rw-rw-rw-   0        0        0      558 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-18 17:39:28.000000 SherLocking-0.0.2/SherLocking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-18 17:39:27.000000 SherLocking-0.0.2/SherLocking.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 17:39:28.314688 SherLocking-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      849 2023-07-18 17:38:28.000000 SherLocking-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:00:35.933387 SherLocking-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-07-18 04:42:39.000000 SherLocking-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      558 2023-07-18 18:00:35.933387 SherLocking-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 04:42:44.000000 SherLocking-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 18:00:35.885917 SherLocking-0.0.3/SherLocking/
+-rw-rw-rw-   0        0        0       24 2023-07-18 05:28:28.000000 SherLocking-0.0.3/SherLocking/__init__.py
+-rw-rw-rw-   0        0        0     5218 2023-07-18 17:50:11.000000 SherLocking-0.0.3/SherLocking/activation.py
+-rw-rw-rw-   0        0        0     1286 2023-07-18 06:53:24.000000 SherLocking-0.0.3/SherLocking/config.py
+-rw-rw-rw-   0        0        0     1824 2023-07-18 17:58:37.000000 SherLocking-0.0.3/SherLocking/file.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:00:35.933387 SherLocking-0.0.3/SherLocking.egg-info/
+-rw-rw-rw-   0        0        0      558 2023-07-18 18:00:35.000000 SherLocking-0.0.3/SherLocking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-18 18:00:35.000000 SherLocking-0.0.3/SherLocking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:00:35.000000 SherLocking-0.0.3/SherLocking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 18:00:35.000000 SherLocking-0.0.3/SherLocking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-18 18:00:35.000000 SherLocking-0.0.3/SherLocking.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 18:00:35.933387 SherLocking-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-07-18 18:00:31.000000 SherLocking-0.0.3/setup.py
```

### Comparing `SherLocking-0.0.2/PKG-INFO` & `SherLocking-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SherLocking
-Version: 0.0.2
+Version: 0.0.3
 Summary: Applies activation for any program.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python,locking,activation,trial,license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SherLocking-0.0.2/SherLocking/activation.py` & `SherLocking-0.0.3/SherLocking/activation.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,23 +43,28 @@
         index_a = CHARACTERS.index(character)
         index_b = CHARACTERS.index(offset)
         index_c = (index_a - index_b) % len(CHARACTERS)
         result += CHARACTERS[index_c]
     return result
 
 
+class StatusBar(ttk.Frame):
+    def __init__(self, master: ttk.Frame, **kwargs):
+        super().__init__(master, **kwargs)
+
+
 class ActivateLicense(ttk.Window):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         # PROPERTIES
         self.variable = 'USERPROFILE'
         self.directory = os.path.join(os.environ[self.variable], 'desktop') 
         self.config_path = os.path.join(self.directory, 'NTMAF.json')
-        self.config_file = HiddenConfig(self.config_path, auto_save=False)
+        self.config_file = HiddenConfig(self.config_path)
 
         # VARIABLES
         today = self.get_today().strftime('%x')
         intervals = [
             '1 Day', '1 Week', '2 Weeks', '3 Weeks',
             '1 Month', '2 Months', '3 Months', '4 Months', '5 Months', '6 Months',
             '7 Months', '8 Months', '9 Months', '10 Months', '11 Months',
@@ -81,15 +86,14 @@
         info_frame.pack(expand=True, fill='x', padx=10, pady=(0, 10), ipady=5)
         ttk.Label(info_frame, text='Program seed: ').grid(row=0, column=0, padx=20, sticky='w')
         self.seed_entry = ttk.Entry(info_frame, width=20, state='disabled')
         self.seed_entry.grid(row=0, column=1, padx=(0, 20), sticky='w', pady=5)
         ttk.Label(info_frame, text='Program name: ').grid(row=1, column=0, padx=20, sticky='w')
         self.program_name = ttk.Entry(info_frame, width=20)
         self.program_name.grid(row=1, column=1, padx=(0, 20), sticky='w')
-        self.program_name.insert(0, 'ORGANIZER')
 
         ttk.Button(self, text='Activate...', bootstyle='success', command=self.activate).pack(fill='x', padx=10, pady=(0, 10))
 
         # BINDS
         self.wm_protocol('WM_DELETE_WINDOW', self.leave)
         self.program_name.bind('<KeyRelease>', self.update_seed)
```

### Comparing `SherLocking-0.0.2/SherLocking/config.py` & `SherLocking-0.0.3/SherLocking/config.py`

 * *Files identical despite different names*

### Comparing `SherLocking-0.0.2/SherLocking/file.py` & `SherLocking-0.0.3/SherLocking/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,48 +32,38 @@
 
         # PROPERTIES
         self.path = path
         self.delay = delay
     
     def hide_file(self) -> bool:
         """Makes the file no visible"""
-        print('Hiding file...')
-        if not os.path.isfile(self.path):
-            print('File doesnt exist...')
-            return False
+        if not os.path.isfile(self.path): return False
         os.system(f'attrib +h {self.path}')
         time.sleep(self.delay)
-        print('File hidden...')
         return True
 
     def show_file(self) -> bool:
         """Makes the file visible"""
-        print('Showing file...')
-        if not os.path.isfile(self.path):
-            print('File doesnt exist..')
-            return False
+        if not os.path.isfile(self.path): return False
         os.system(f'attrib -h {self.path}')
         time.sleep(self.delay)
-        print('File visible...')
         return True
 
 
 class HiddenConfig(HiddenFile, Config):
     def __init__(self, path: str, auto_save=True):
         HiddenFile.__init__(self, path)
         Config.__init__(self, path, auto_save=auto_save)
     
     def get(self, key: str='') -> dict:
         """Returns the content of the config"""
         self.show_file()
-        print('Getting config...')
         config = super().get(key)
         self.hide_file()
         return config
 
     def save(self) -> None:
         """Saves the config"""
         self.show_file()
-        print('Saving config...')
         super().save()
         self.hide_file()
```

### Comparing `SherLocking-0.0.2/SherLocking.egg-info/PKG-INFO` & `SherLocking-0.0.3/SherLocking.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SherLocking
-Version: 0.0.2
+Version: 0.0.3
 Summary: Applies activation for any program.
 Author: Armando Chaparro
 Author-email: <pylejandria@gmail.com>
 Keywords: python,locking,activation,trial,license
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `SherLocking-0.0.2/setup.py` & `SherLocking-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Applies activation for any program.'
 LONG_DESCRIPTION = 'A package to apply activation required to run any program, like a license.'
 
 setup(
     name="SherLocking",
     version=VERSION,
     author="Armando Chaparro",
```

