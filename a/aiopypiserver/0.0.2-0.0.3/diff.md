# Comparing `tmp/aiopypiserver-0.0.2.tar.gz` & `tmp/aiopypiserver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopypiserver-0.0.2.tar", last modified: Tue Jul 18 00:47:21 2023, max compression
+gzip compressed data, was "aiopypiserver-0.0.3.tar", last modified: Tue Jul 18 18:53:24 2023, max compression
```

## Comparing `aiopypiserver-0.0.2.tar` & `aiopypiserver-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:47:21.141202 aiopypiserver-0.0.2/
--rw-r--r--   0 mscada    (1000) mscada    (1000)    35149 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/LICENSE
--rw-r--r--   0 mscada    (1000) mscada    (1000)       31 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/MANIFEST.in
--rw-r--r--   0 mscada    (1000) mscada    (1000)     2205 2023-07-18 00:47:21.141202 aiopypiserver-0.0.2/PKG-INFO
--rw-r--r--   0 mscada    (1000) mscada    (1000)     1587 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/README.md
--rw-r--r--   0 mscada    (1000) mscada    (1000)      789 2023-07-18 00:43:29.000000 aiopypiserver-0.0.2/pyproject.toml
--rw-r--r--   0 mscada    (1000) mscada    (1000)       38 2023-07-18 00:47:21.141202 aiopypiserver-0.0.2/setup.cfg
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:47:21.137202 aiopypiserver-0.0.2/src/
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:47:21.137202 aiopypiserver-0.0.2/src/aiopypiserver/
--rw-r--r--   0 mscada    (1000) mscada    (1000)      109 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/src/aiopypiserver/__init__.py
--rw-r--r--   0 mscada    (1000) mscada    (1000)      112 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/src/aiopypiserver/__main__.py
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:47:21.137202 aiopypiserver-0.0.2/src/aiopypiserver/assets/
--rw-r--r--   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:32:37.000000 aiopypiserver-0.0.2/src/aiopypiserver/assets/__init__.py
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:47:21.137202 aiopypiserver-0.0.2/src/aiopypiserver/assets/__pycache__/
--rw-r--r--   0 mscada    (1000) mscada    (1000)      154 2023-07-18 00:32:37.000000 aiopypiserver-0.0.2/src/aiopypiserver/assets/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 mscada    (1000) mscada    (1000)      505 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/src/aiopypiserver/assets/index.html
--rw-r--r--   0 mscada    (1000) mscada    (1000)      169 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/src/aiopypiserver/assets/list.html
--rw-r--r--   0 mscada    (1000) mscada    (1000)    10076 2023-07-17 19:52:39.000000 aiopypiserver-0.0.2/src/aiopypiserver/webserver.py
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:47:21.137202 aiopypiserver-0.0.2/src/aiopypiserver.egg-info/
--rw-r--r--   0 mscada    (1000) mscada    (1000)     2205 2023-07-18 00:47:21.000000 aiopypiserver-0.0.2/src/aiopypiserver.egg-info/PKG-INFO
--rw-r--r--   0 mscada    (1000) mscada    (1000)      573 2023-07-18 00:47:21.000000 aiopypiserver-0.0.2/src/aiopypiserver.egg-info/SOURCES.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)        1 2023-07-18 00:47:21.000000 aiopypiserver-0.0.2/src/aiopypiserver.egg-info/dependency_links.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)       64 2023-07-18 00:47:21.000000 aiopypiserver-0.0.2/src/aiopypiserver.egg-info/entry_points.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)       15 2023-07-18 00:47:21.000000 aiopypiserver-0.0.2/src/aiopypiserver.egg-info/requires.txt
--rw-r--r--   0 mscada    (1000) mscada    (1000)       14 2023-07-18 00:47:21.000000 aiopypiserver-0.0.2/src/aiopypiserver.egg-info/top_level.txt
-drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:47:21.141202 aiopypiserver-0.0.2/tests/
--rw-r--r--   0 mscada    (1000) mscada    (1000)      941 2023-07-17 18:22:11.000000 aiopypiserver-0.0.2/tests/test_server.py
+drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/
+-rw-r--r--   0 mscada    (1000) mscada    (1000)    35149 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/LICENSE
+-rw-r--r--   0 mscada    (1000) mscada    (1000)       31 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/MANIFEST.in
+-rw-r--r--   0 mscada    (1000) mscada    (1000)     2205 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/PKG-INFO
+-rw-r--r--   0 mscada    (1000) mscada    (1000)     1587 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/README.md
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      789 2023-07-18 18:52:18.000000 aiopypiserver-0.0.3/pyproject.toml
+-rw-r--r--   0 mscada    (1000) mscada    (1000)       38 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/setup.cfg
+drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.860734 aiopypiserver-0.0.3/src/
+drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.860734 aiopypiserver-0.0.3/src/aiopypiserver/
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      109 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/__init__.py
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      112 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/__main__.py
+drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/src/aiopypiserver/assets/
+-rw-r--r--   0 mscada    (1000) mscada    (1000)        0 2023-07-18 00:32:37.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/__init__.py
+drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/src/aiopypiserver/assets/__pycache__/
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      154 2023-07-18 00:32:37.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      505 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/index.html
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      169 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/src/aiopypiserver/assets/list.html
+-rw-r--r--   0 mscada    (1000) mscada    (1000)    10000 2023-07-18 18:41:05.000000 aiopypiserver-0.0.3/src/aiopypiserver/webserver.py
+drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/
+-rw-r--r--   0 mscada    (1000) mscada    (1000)     2205 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/PKG-INFO
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      573 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 mscada    (1000) mscada    (1000)        1 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 mscada    (1000) mscada    (1000)       64 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/entry_points.txt
+-rw-r--r--   0 mscada    (1000) mscada    (1000)       15 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/requires.txt
+-rw-r--r--   0 mscada    (1000) mscada    (1000)       14 2023-07-18 18:53:24.000000 aiopypiserver-0.0.3/src/aiopypiserver.egg-info/top_level.txt
+drwxr-xr-x   0 mscada    (1000) mscada    (1000)        0 2023-07-18 18:53:24.864734 aiopypiserver-0.0.3/tests/
+-rw-r--r--   0 mscada    (1000) mscada    (1000)      941 2023-07-17 18:22:11.000000 aiopypiserver-0.0.3/tests/test_server.py
```

### Comparing `aiopypiserver-0.0.2/LICENSE` & `aiopypiserver-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.2/PKG-INFO` & `aiopypiserver-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopypiserver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Do what pypiserver does, but with aiohttp.
 Author: Jamie Walton
 Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
 Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `aiopypiserver-0.0.2/README.md` & `aiopypiserver-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.2/pyproject.toml` & `aiopypiserver-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aiopypiserver"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name="Jamie Walton"}
 ]
 description = "Do what pypiserver does, but with aiohttp."
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
```

### Comparing `aiopypiserver-0.0.2/src/aiopypiserver/webserver.py` & `aiopypiserver-0.0.3/src/aiopypiserver/webserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,21 +18,22 @@
         prog='aiopypiserver',
         description='Private PyPi server.',
         epilog='Browse index at http://localhost:8080/.'
     )
     parser.add_argument('package_path', type=str, nargs='?',
                         default='packages', help='path to packages')
     parser.add_argument('-p', '--port', metavar='port', type=int,
-                        nargs=1, default=8080, help='Listen on port')
+                        nargs='?', default=8080, help='Listen on port')
     parser.add_argument('-i', '--interface', metavar='address', type=str,
-                        nargs=1, default='localhost', help='Listen on address')
+                        nargs='?', default='localhost',
+                        help='Listen on address')
     parser.add_argument('-u', '--username', metavar='username', type=str,
-                        nargs=1, help='For uploading packages')
+                        nargs='?', help='For uploading packages')
     parser.add_argument('-P', '--password', metavar='password', type=str,
-                        nargs=1, help='...')
+                        nargs='?', help='...')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='set debug level')
     parser.add_argument('-q', '--quiet', action='store_true',
                         help='turn off access logging')
     return parser.parse_args()
 
 
@@ -121,19 +122,16 @@
 
     def __init__(self, config):
         """Initialise with an argparse NameSpace."""
         self.ip = config.interface
         self.port = config.port
         self.packages = config.package_path
         self.pkg_path = Path('.').joinpath(self.packages).resolve()
-        try:
-            self.username = config.username[0]
-            self.password = config.password[0]
-        except IndexError:
-            self.username, self.password = None, None
+        self.username = config.username
+        self.password = config.password
         self.info = get_package_details(self.pkg_path)
         if not self.pkg_path.is_dir():
             raise RuntimeError(f"{self.pkg_path} bad package directory")
         self.webapp = web.Application()
         routes = [web.get('/', self.index_handler),
                   web.get('/index.html', self.index_handler),
                   web.get('/packages/', self.packages_handler),
```

### Comparing `aiopypiserver-0.0.2/src/aiopypiserver.egg-info/PKG-INFO` & `aiopypiserver-0.0.3/src/aiopypiserver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopypiserver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Do what pypiserver does, but with aiohttp.
 Author: Jamie Walton
 Project-URL: Homepage, https://github.com/jamie0walton/aiopypiserver
 Project-URL: Bug Tracker, https://github.com/jamie0walton/aiopypiserver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `aiopypiserver-0.0.2/src/aiopypiserver.egg-info/SOURCES.txt` & `aiopypiserver-0.0.3/src/aiopypiserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiopypiserver-0.0.2/tests/test_server.py` & `aiopypiserver-0.0.3/tests/test_server.py`

 * *Files identical despite different names*

