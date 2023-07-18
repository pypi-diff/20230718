# Comparing `tmp/nrcpy-1.2.2.tar.gz` & `tmp/nrcpy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrcpy-1.2.2.tar", last modified: Tue Jul 18 20:53:29 2023, max compression
+gzip compressed data, was "nrcpy-1.2.3.tar", last modified: Tue Jul 18 21:02:23 2023, max compression
```

## Comparing `nrcpy-1.2.2.tar` & `nrcpy-1.2.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 20:53:29.419016 nrcpy-1.2.2/
--rw-rw-rw-   0        0        0     1431 2023-07-18 20:53:29.419016 nrcpy-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1188 2023-07-18 20:17:31.000000 nrcpy-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 20:53:29.352135 nrcpy-1.2.2/nrcpy/
--rw-rw-rw-   0        0        0     2376 2023-07-18 19:52:29.000000 nrcpy-1.2.2/nrcpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 20:53:29.416412 nrcpy-1.2.2/nrcpy.egg-info/
--rw-rw-rw-   0        0        0     1431 2023-07-18 20:53:29.000000 nrcpy-1.2.2/nrcpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-07-18 20:53:29.000000 nrcpy-1.2.2/nrcpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 20:53:29.000000 nrcpy-1.2.2/nrcpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 20:53:29.000000 nrcpy-1.2.2/nrcpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 20:53:29.000000 nrcpy-1.2.2/nrcpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 20:53:29.419016 nrcpy-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      533 2023-07-18 20:53:23.000000 nrcpy-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:02:23.906363 nrcpy-1.2.3/
+-rw-rw-rw-   0        0        0     1450 2023-07-18 21:02:23.898354 nrcpy-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1200 2023-07-18 21:00:46.000000 nrcpy-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 21:02:23.868268 nrcpy-1.2.3/nrcpy/
+-rw-rw-rw-   0        0        0     2376 2023-07-18 20:58:31.000000 nrcpy-1.2.3/nrcpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:02:23.898354 nrcpy-1.2.3/nrcpy.egg-info/
+-rw-rw-rw-   0        0        0     1450 2023-07-18 21:02:23.000000 nrcpy-1.2.3/nrcpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-07-18 21:02:23.000000 nrcpy-1.2.3/nrcpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:02:23.000000 nrcpy-1.2.3/nrcpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 21:02:23.000000 nrcpy-1.2.3/nrcpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 21:02:23.906363 nrcpy-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      525 2023-07-18 21:01:41.000000 nrcpy-1.2.3/setup.py
```

### Comparing `nrcpy-1.2.2/PKG-INFO` & `nrcpy-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: nrcpy
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package for NRC devices
 Home-page: https://github.com/Rebox98/nrcpy
 Author: Hossein Ghaheri
 Author-email: hosseinghaheri@yahoo.com
 Description-Content-Type: text/markdown
 
 # Nrcpy
 
 Nrcpy is a Python package for working with NRC devices. It provides a convenient interface to connect to an NRC device, send commands, and retrieve information from the device.
 
-## Installation
+## ðŸ”¥ Installation
 
 You can install `nrcpy` using pip:
 
 ```shell
 pip install nrcpy
 ```
-## Usage
+## ðŸª§ Usage
 Here is an example of how to use nrcpy to connect to an NRC device and control the relays:
 ```python
 from nrcpy import NrcDevice
 
 # Configure the device
 ip = '192.168.1.200'
 port = 23
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nrcpy-1.2.2/README.md` & `nrcpy-1.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Nrcpy
 
 Nrcpy is a Python package for working with NRC devices. It provides a convenient interface to connect to an NRC device, send commands, and retrieve information from the device.
 
-## Installation
+## 🔥 Installation
 
 You can install `nrcpy` using pip:
 
 ```shell
 pip install nrcpy
 ```
-## Usage
+## 🪧 Usage
 Here is an example of how to use nrcpy to connect to an NRC device and control the relays:
 ```python
 from nrcpy import NrcDevice
 
 # Configure the device
 ip = '192.168.1.200'
 port = 23
@@ -44,8 +44,8 @@
     print(f'Relay 2 Status: {relay_2_status}')
 else:
     print('Error in login')
 
 # Close connection
 nrc.disconnect()
 
-```
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nrcpy-1.2.2/nrcpy/__init__.py` & `nrcpy-1.2.3/nrcpy/__init__.py`

 * *Files identical despite different names*

### Comparing `nrcpy-1.2.2/nrcpy.egg-info/PKG-INFO` & `nrcpy-1.2.3/nrcpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: nrcpy
-Version: 1.2.2
+Version: 1.2.3
 Summary: A package for NRC devices
 Home-page: https://github.com/Rebox98/nrcpy
 Author: Hossein Ghaheri
 Author-email: hosseinghaheri@yahoo.com
 Description-Content-Type: text/markdown
 
 # Nrcpy
 
 Nrcpy is a Python package for working with NRC devices. It provides a convenient interface to connect to an NRC device, send commands, and retrieve information from the device.
 
-## Installation
+## ðŸ”¥ Installation
 
 You can install `nrcpy` using pip:
 
 ```shell
 pip install nrcpy
 ```
-## Usage
+## ðŸª§ Usage
 Here is an example of how to use nrcpy to connect to an NRC device and control the relays:
 ```python
 from nrcpy import NrcDevice
 
 # Configure the device
 ip = '192.168.1.200'
 port = 23
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nrcpy-1.2.2/setup.py` & `nrcpy-1.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.md").read_text()
 
 setup(
     name='nrcpy',
-    version='1.2.2',
+    version='1.2.3',
     description='A package for NRC devices',
     author='Hossein Ghaheri',
     author_email='hosseinghaheri@yahoo.com',
     url='https://github.com/Rebox98/nrcpy',
     packages=['nrcpy'],
-    install_requires=['socket'],
+    install_requires=[],
     long_description = long_description,
     long_description_content_type="text/markdown"
 )
```

