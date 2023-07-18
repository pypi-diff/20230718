# Comparing `tmp/nodered.py-0.2.6.post4.tar.gz` & `tmp/nodered.py-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.2.6.post4.tar", last modified: Tue Jul 11 12:41:26 2023, max compression
+gzip compressed data, was "nodered.py-0.2.7.tar", last modified: Tue Jul 18 09:12:28 2023, max compression
```

## Comparing `nodered.py-0.2.6.post4.tar` & `nodered.py-0.2.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 12:41:26.830000 nodered.py-0.2.6.post4/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.6.post4/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2581 2023-07-11 12:41:26.970000 nodered.py-0.2.6.post4/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2259 2023-07-10 09:05:46.000000 nodered.py-0.2.6.post4/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 12:41:26.830000 nodered.py-0.2.6.post4/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2581 2023-07-11 12:41:26.000000 nodered.py-0.2.6.post4/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-11 12:41:26.000000 nodered.py-0.2.6.post4/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-11 12:41:26.000000 nodered.py-0.2.6.post4/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-11 12:41:26.000000 nodered.py-0.2.6.post4/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-11 12:41:26.000000 nodered.py-0.2.6.post4/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.6.post4/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 12:41:26.830000 nodered.py-0.2.6.post4/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      480 2023-07-11 12:34:48.000000 nodered.py-0.2.6.post4/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    19358 2023-07-11 12:39:53.000000 nodered.py-0.2.6.post4/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.6.post4/noderedpy/_property.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 12:41:26.830000 nodered.py-0.2.6.post4/noderedpy/assets/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.6.post4/noderedpy/assets/python-logo.png
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.6.post4/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 12:41:26.830000 nodered.py-0.2.6.post4/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.6.post4/noderedpy/node-red-starter/editorTheme.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1589 2023-07-03 06:05:35.000000 nodered.py-0.2.6.post4/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-07-10 08:42:28.000000 nodered.py-0.2.6.post4/noderedpy/node-red-starter/package.json
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-11 12:41:26.830000 nodered.py-0.2.6.post4/noderedpy/templates/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.6.post4/noderedpy/templates/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.6.post4/noderedpy/templates/template.html
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5788 2023-07-11 11:51:18.000000 nodered.py-0.2.6.post4/noderedpy/templates/template.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.6.post4/noderedpy/templates/template.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-11 12:41:26.970000 nodered.py-0.2.6.post4/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.6.post4/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.2.7/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2780 2023-07-18 09:12:28.880000 nodered.py-0.2.7/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2464 2023-07-18 09:07:11.000000 nodered.py-0.2.7/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2780 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      599 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       74 2023-07-18 09:12:28.000000 nodered.py-0.2.7/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.2.7/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      474 2023-07-18 08:37:06.000000 nodered.py-0.2.7/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)    19526 2023-07-18 09:07:30.000000 nodered.py-0.2.7/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4807 2023-07-10 01:12:44.000000 nodered.py-0.2.7/noderedpy/_property.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/noderedpy/assets/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)   453665 2023-05-07 01:22:45.000000 nodered.py-0.2.7/noderedpy/assets/python-logo.png
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1260 2023-05-10 10:41:49.000000 nodered.py-0.2.7/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.790000 nodered.py-0.2.7/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        8 2023-05-07 00:47:00.000000 nodered.py-0.2.7/noderedpy/node-red-starter/editorTheme.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1583 2023-07-18 08:40:46.000000 nodered.py-0.2.7/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      266 2023-07-10 08:42:28.000000 nodered.py-0.2.7/noderedpy/node-red-starter/package.json
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-07-18 09:12:28.800000 nodered.py-0.2.7/noderedpy/templates/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     9689 2023-07-10 01:17:43.000000 nodered.py-0.2.7/noderedpy/templates/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      969 2023-05-10 10:44:16.000000 nodered.py-0.2.7/noderedpy/templates/template.html
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     5788 2023-07-11 11:51:18.000000 nodered.py-0.2.7/noderedpy/templates/template.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      290 2023-05-10 09:24:21.000000 nodered.py-0.2.7/noderedpy/templates/template.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-07-18 09:12:28.880000 nodered.py-0.2.7/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1106 2023-06-02 04:28:29.000000 nodered.py-0.2.7/setup.py
```

### Comparing `nodered.py-0.2.6.post4/LICENSE` & `nodered.py-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/PKG-INFO` & `nodered.py-0.2.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.6.post4
+Version: 0.2.7
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -28,14 +28,21 @@
 </div>
 <br/><br/>
 
 ## 🎛️ requirements
 - node.js 18.16.1 or higher(latest stable)
   - nodered.py 0.2.6 or higher, automatically download from internet if no node.js installed
 - python 3.7 or higher
+- tested on
+
+|        OS       | Tested | Pass |
+| --------------- | ------ | ---- |
+| Mac 13(Ventura) |   ✅   |  ✅  |
+| Windows 10      |   ✅   |  ✅  |
+| Linux(WSL)      |   🚫   |      |
 
 <br/><br/>
 
 ## 🌐 install
 ### - using pip
 ```zsh
 python -m pip install nodered.py
@@ -52,15 +59,15 @@
 ### Node-RED initialize
 ```python
 from noderedpy import RED
 
 red = RED(
     os.path.join(__dirname, ".node-red"),
     os.path.join(__dirname, "node_red_dir"),
-    "/node-red", 1880
+    "/node-red", "/", 1880
 )
 ```
 
 <br/>
 
 ### register Node
 - register as decorator
@@ -89,15 +96,15 @@
 ### start Node-RED
 ```python
 red.start({debug:bool}, {callback:MethodType})
 ```
 <br/><br/>
 
 ## Todos
-[x] type support for "list" and "dict"
+✅ type support for "list" and "dict"
 
 <br/><br/>
 
 ## Roadmap To 2.0
-[x] remove aiohttp server
+✅ remove aiohttp server
 
-[ ] flexible property ui
+🟩 flexible property ui
```

#### html2text {}

```diff
@@ -1,35 +1,37 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6.post4 Summary: make
-python function to Node-RED node Home-page: https://github.com/oyajiDev/
-NodeRED.py Author: oyajiDev Author-email: this.dev.somehit@gmail.com License:
-MIT license Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.7 Summary: make python
+function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
+Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
 ## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
 0.2.6 or higher, automatically download from internet if no node.js installed -
-python 3.7 or higher
+python 3.7 or higher - tested on | OS | Tested | Pass | | --------------- | ---
+--- | ---- | | Mac 13(Ventura) | â | â | | Windows 10 | â | â | | Linux
+(WSL) | ð« | |
 
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
 ## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
-"node_red_dir"), "/node-red", 1880 ) ```
+"node_red_dir"), "/node-red", "/", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
 function for details ```python from noderedpy import Node from
 noderedpy.decorator import register @register("test") def test(node:Node,
 props:dict, msg:dict) -> dict: # user codes here return msg ``` - register from
 Node-RED object - See noredpy.decorator.register_function for details ```python
 api = API() red.register("test", api.test) ``` - See noderedpy._property for
 details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
-## Todos [x] type support for "list" and "dict"
+## Todos â type support for "list" and "dict"
 
-## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
+## Roadmap To 2.0 â remove aiohttp server ð© flexible property ui
```

### Comparing `nodered.py-0.2.6.post4/README.md` & `nodered.py-0.2.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,21 @@
 </div>
 <br/><br/>
 
 ## 🎛️ requirements
 - node.js 18.16.1 or higher(latest stable)
   - nodered.py 0.2.6 or higher, automatically download from internet if no node.js installed
 - python 3.7 or higher
+- tested on
+
+|        OS       | Tested | Pass |
+| --------------- | ------ | ---- |
+| Mac 13(Ventura) |   ✅   |  ✅  |
+| Windows 10      |   ✅   |  ✅  |
+| Linux(WSL)      |   🚫   |      |
 
 <br/><br/>
 
 ## 🌐 install
 ### - using pip
 ```zsh
 python -m pip install nodered.py
@@ -40,15 +47,15 @@
 ### Node-RED initialize
 ```python
 from noderedpy import RED
 
 red = RED(
     os.path.join(__dirname, ".node-red"),
     os.path.join(__dirname, "node_red_dir"),
-    "/node-red", 1880
+    "/node-red", "/", 1880
 )
 ```
 
 <br/>
 
 ### register Node
 - register as decorator
@@ -77,15 +84,15 @@
 ### start Node-RED
 ```python
 red.start({debug:bool}, {callback:MethodType})
 ```
 <br/><br/>
 
 ## Todos
-[x] type support for "list" and "dict"
+✅ type support for "list" and "dict"
 
 <br/><br/>
 
 ## Roadmap To 2.0
-[x] remove aiohttp server
+✅ remove aiohttp server
 
-[ ] flexible property ui
+🟩 flexible property ui
```

#### html2text {}

```diff
@@ -2,29 +2,31 @@
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
 ## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
 0.2.6 or higher, automatically download from internet if no node.js installed -
-python 3.7 or higher
+python 3.7 or higher - tested on | OS | Tested | Pass | | --------------- | ---
+--- | ---- | | Mac 13(Ventura) | â | â | | Windows 10 | â | â | | Linux
+(WSL) | ð« | |
 
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
 ## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
-"node_red_dir"), "/node-red", 1880 ) ```
+"node_red_dir"), "/node-red", "/", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
 function for details ```python from noderedpy import Node from
 noderedpy.decorator import register @register("test") def test(node:Node,
 props:dict, msg:dict) -> dict: # user codes here return msg ``` - register from
 Node-RED object - See noredpy.decorator.register_function for details ```python
 api = API() red.register("test", api.test) ``` - See noderedpy._property for
 details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
-## Todos [x] type support for "list" and "dict"
+## Todos â type support for "list" and "dict"
 
-## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
+## Roadmap To 2.0 â remove aiohttp server ð© flexible property ui
```

### Comparing `nodered.py-0.2.6.post4/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.2.7/nodered.py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.2.6.post4
+Version: 0.2.7
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -28,14 +28,21 @@
 </div>
 <br/><br/>
 
 ## 🎛️ requirements
 - node.js 18.16.1 or higher(latest stable)
   - nodered.py 0.2.6 or higher, automatically download from internet if no node.js installed
 - python 3.7 or higher
+- tested on
+
+|        OS       | Tested | Pass |
+| --------------- | ------ | ---- |
+| Mac 13(Ventura) |   ✅   |  ✅  |
+| Windows 10      |   ✅   |  ✅  |
+| Linux(WSL)      |   🚫   |      |
 
 <br/><br/>
 
 ## 🌐 install
 ### - using pip
 ```zsh
 python -m pip install nodered.py
@@ -52,15 +59,15 @@
 ### Node-RED initialize
 ```python
 from noderedpy import RED
 
 red = RED(
     os.path.join(__dirname, ".node-red"),
     os.path.join(__dirname, "node_red_dir"),
-    "/node-red", 1880
+    "/node-red", "/", 1880
 )
 ```
 
 <br/>
 
 ### register Node
 - register as decorator
@@ -89,15 +96,15 @@
 ### start Node-RED
 ```python
 red.start({debug:bool}, {callback:MethodType})
 ```
 <br/><br/>
 
 ## Todos
-[x] type support for "list" and "dict"
+✅ type support for "list" and "dict"
 
 <br/><br/>
 
 ## Roadmap To 2.0
-[x] remove aiohttp server
+✅ remove aiohttp server
 
-[ ] flexible property ui
+🟩 flexible property ui
```

#### html2text {}

```diff
@@ -1,35 +1,37 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.2.6.post4 Summary: make
-python function to Node-RED node Home-page: https://github.com/oyajiDev/
-NodeRED.py Author: oyajiDev Author-email: this.dev.somehit@gmail.com License:
-MIT license Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE
+Metadata-Version: 2.1 Name: nodered.py Version: 0.2.7 Summary: make python
+function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
+Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
                              [MIT_License] [pypi]
 
 
 ## ðï¸ requirements - node.js 18.16.1 or higher(latest stable) - nodered.py
 0.2.6 or higher, automatically download from internet if no node.js installed -
-python 3.7 or higher
+python 3.7 or higher - tested on | OS | Tested | Pass | | --------------- | ---
+--- | ---- | | Mac 13(Ventura) | â | â | | Windows 10 | â | â | | Linux
+(WSL) | ð« | |
 
 ## ð install ### - using pip ```zsh python -m pip install nodered.py ``` ###
 - using git(dev) ```zsh python -m pip install git+https://github.com/oyajiDev/
 NodeRED.py.git ```
 
 ## ð  usage ### Node-RED initialize ```python from noderedpy import RED red =
 RED( os.path.join(__dirname, ".node-red"), os.path.join(__dirname,
-"node_red_dir"), "/node-red", 1880 ) ```
+"node_red_dir"), "/node-red", "/", 1880 ) ```
 ### register Node - register as decorator - See noredpy.decorator.register
 function for details ```python from noderedpy import Node from
 noderedpy.decorator import register @register("test") def test(node:Node,
 props:dict, msg:dict) -> dict: # user codes here return msg ``` - register from
 Node-RED object - See noredpy.decorator.register_function for details ```python
 api = API() red.register("test", api.test) ``` - See noderedpy._property for
 details of "Property" - See example for details.
 ### start Node-RED ```python red.start({debug:bool}, {callback:MethodType}) ```
 
 
-## Todos [x] type support for "list" and "dict"
+## Todos â type support for "list" and "dict"
 
-## Roadmap To 2.0 [x] remove aiohttp server [ ] flexible property ui
+## Roadmap To 2.0 â remove aiohttp server ð© flexible property ui
```

### Comparing `nodered.py-0.2.6.post4/nodered.py.egg-info/SOURCES.txt` & `nodered.py-0.2.7/nodered.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/noderedpy/_nodered.py` & `nodered.py-0.2.7/noderedpy/_nodered.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,42 +10,49 @@
 
 class RED:
     """
     Node-RED manager class
     """
     registered_nodes:List["Node"] = []
 
-    def __init__(self, user_dir:str, node_red_dir:str = None, admin_root:str = "/node-red-py", port:int = 1880, show_default_category:bool = True, editor_theme:dict = {}, auths:List[dict] = []):
+    def __init__(self, user_dir:str, node_red_dir:str = None, admin_root:str = "/node-red-py", node_root:str = "/", port:int = 1880, enable_remote_access:bool = True, show_default_category:bool = True, editor_theme:dict = {}, auths:List[dict] = []):
         """
         Set configs of Node-RED and setup
 
         Parameters
         ----------
         user_dir: str, required
             userDir of Node-RED settings
         node_red_dir: str, default None
             directory for Node-RED starter
         admin_root: str, default "/node-red-py"
             httpAdminRoot of Node-RED settings
+        node_root: str, default "/"
+            httpNodeRoot of Node-RED settings
         port: int, default 1880
             port of Node-RED server
+        enable_remote_access: bool, default True
+            enable remote access of Node-RED or not
         show_default_category: bool, default True
             show default categories of Node-RED or not
         editor_theme: dict, default {}
             editorTheme of Node-RED server (for detail information, see https://github.com/node-red/node-red/wiki/Design:-Editor-Themes)
         auths: List[dict], default []
             auth list for Node-RED
         """
-        self.user_dir, self.admin_root, self.port, self.show_default_category, self.editor_theme =\
-            user_dir, admin_root, port, show_default_category, self.__default_editor_theme(editor_theme)
+        self.user_dir, self.admin_root, self.node_root, self.port, self.enable_remote_access, self.show_default_category, self.editor_theme =\
+            user_dir, admin_root, node_root, port, enable_remote_access, show_default_category, self.__default_editor_theme(editor_theme)
         self.__temp_dir, self.__node_dir =\
             os.path.join(__path__[0], ".temp"), os.path.join(__path__[0], ".nodejs")
 
         if not self.admin_root.startswith("/"):
-            self.admin_root = f"/{self.admin_root}"
+            raise SyntaxError("`admin_root` must starts with '/'!")
+
+        if not self.node_root.startswith("/"):
+            raise SyntaxError("`node_root` must starts with '/'!")
 
         self.node_auths = self.__default_node_auth(auths)
 
         # check node.js exists
         try:
             subprocess.call(
                 [ "npm.cmd" if sys.platform == "win32" else "npm", "--version" ],
@@ -181,14 +188,28 @@
                     "username": node_auth["username"],
                     "password": node_auth["password"],
                     "permissions": node_auth.pop("permissions", "*")
                 })
 
         return new_node_auths
     
+    def __save_config(self, is_ready:bool):
+        with open(os.path.join(self.node_red_dir, "config.json"), "w", encoding = "utf-8") as cfw:
+            json.dump({
+                "userDir": self.user_dir,
+                "adminRoot": self.admin_root,
+                "nodeRoot": self.node_root,
+                "port": self.port,
+                "enableRemoteAccess": self.enable_remote_access,
+                "showDefaultCategory": self.show_default_category,
+                "userCategory": list(set([ node.category for node in RED.registered_nodes ])),
+                "editorTheme": self.editor_theme,
+                "adminAuth": [] if is_ready else self.node_auths
+            }, cfw, indent = 4)
+    
     def register(self, node_func:MethodType, name:str, category:str = "nodered_py", version:str = "1.0.0", description:str = "", author:str = "nodered.py", keywords:List[str] = [], icon:str = "function.png", properties:List[Property] = []):
         """
         Function to register Node function
 
         Parameters
         ----------
         node_func: MethodType, required
@@ -277,24 +298,15 @@
         self.__cache_dir = os.path.join(self.user_dir, ".cache")
         if os.path.exists(self.__cache_dir):
             shutil.rmtree(self.__cache_dir)
 
         os.mkdir(self.__cache_dir)
 
         # save configs
-        with open(os.path.join(self.node_red_dir, "config.json"), "w", encoding = "utf-8") as cfw:
-            json.dump({
-                "userDir": self.user_dir,
-                "adminRoot": self.admin_root,
-                "port": self.port,
-                "showDefaultCategory": self.show_default_category,
-                "userCategory": list(set([ node.category for node in RED.registered_nodes ])),
-                "editorTheme": self.editor_theme,
-                "adminAuth": self.node_auths
-            }, cfw, indent = 4)
+        self.__save_config(True)
 
         # remove existing nodes
         for node_dir in glob(os.path.join(self.user_dir, "node_modules", "nodered-py-*")):
             shutil.rmtree(node_dir)
 
         # create custom nodes
         for node in RED.registered_nodes:
@@ -329,24 +341,15 @@
         import time
 
         self.__started_file = os.path.join(self.node_red_dir, "started")
         if os.path.exists(self.__started_file):
             os.remove(self.__started_file)
 
         # save configs
-        with open(os.path.join(self.node_red_dir, "config.json"), "w", encoding = "utf-8") as cfw:
-            json.dump({
-                "userDir": self.user_dir,
-                "adminRoot": self.admin_root,
-                "port": self.port,
-                "showDefaultCategory": self.show_default_category,
-                "userCategory": list(set([ node.category for node in RED.registered_nodes ])),
-                "editorTheme": self.editor_theme,
-                "adminAuth": []
-            }, cfw, indent = 4)
+        self.__save_config(False)
 
         subprocess.Popen([
             self.__node_path,
             "index.js"
         ], shell = False, stdout = subprocess.DEVNULL, stderr = subprocess.STDOUT, cwd = self.node_red_dir)
 
         while True:
```

### Comparing `nodered.py-0.2.6.post4/noderedpy/_property.py` & `nodered.py-0.2.7/noderedpy/_property.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/noderedpy/assets/python-logo.png` & `nodered.py-0.2.7/noderedpy/assets/python-logo.png`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/noderedpy/decorator.py` & `nodered.py-0.2.7/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/noderedpy/node-red-starter/index.js` & `nodered.py-0.2.7/noderedpy/node-red-starter/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -13,16 +13,16 @@
 // create express and node-red server
 const exapp = express();
 const RED_server = http.createServer(exapp);
 
 // set start options
 let opts = {
     editorTheme: configs.editorTheme,
-    httpAdminRoot: configs.adminRoot.startsWith("/") ? configs.adminRoot : `/${configs.adminRoot}`,
-    httpNodeRoot: "/",
+    httpAdminRoot: configs.adminRoot,
+    httpNodeRoot: configs.nodeRoot,
     flowFile: "noderedpy.json",
     userDir: configs.userDir,
     paletteCategories: configs.showDefaultCategory ? configs.userCategory.concat(["subflows", "common", "function", "network", "sequence", "parser", "storage"]) : configs.userCategory
 };
 // set auth
 if (Array.isArray(configs.adminAuth) && configs.adminAuth.length > 0) {
     var realAuth = [];
@@ -42,11 +42,11 @@
 // node-red default routes
 exapp.use("/", express.static("web"));
 exapp.use(RED.settings.httpAdminRoot, RED.httpAdmin);
 exapp.use(RED.settings.httpNodeRoot, RED.httpNode);
 
 // start node-red
 RED.start().then(() => {
-    RED_server.listen(configs.port, "0.0.0.0", () => {
+    RED_server.listen(configs.port, configs.enableRemoteAccess ? "0.0.0.0" : "127.0.0.1", () => {
         fs.writeFileSync(path.join(__dirname, "started"), "");
     });
 });
```

### Comparing `nodered.py-0.2.6.post4/noderedpy/templates/__init__.py` & `nodered.py-0.2.7/noderedpy/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/noderedpy/templates/template.html` & `nodered.py-0.2.7/noderedpy/templates/template.html`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/noderedpy/templates/template.js` & `nodered.py-0.2.7/noderedpy/templates/template.js`

 * *Files identical despite different names*

### Comparing `nodered.py-0.2.6.post4/setup.py` & `nodered.py-0.2.7/setup.py`

 * *Files identical despite different names*

