# Comparing `tmp/sdock-0.1.7.tar.gz` & `tmp/sdock-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdock-0.1.7.tar", last modified: Tue Jul 18 03:04:17 2023, max compression
+gzip compressed data, was "sdock-0.1.8.tar", last modified: Tue Jul 18 03:06:34 2023, max compression
```

## Comparing `sdock-0.1.7.tar` & `sdock-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:04:17.215017 sdock-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 03:04:13.000000 sdock-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:04:17.215017 sdock-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 03:04:13.000000 sdock-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:04:17.215017 sdock-0.1.7/sdock/
--rw-r--r--   0 runner    (1001) docker     (123)    26201 2023-07-18 03:04:13.000000 sdock-0.1.7/sdock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-18 03:04:13.000000 sdock-0.1.7/sdock/vbgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:04:17.215017 sdock-0.1.7/sdock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:04:17.000000 sdock-0.1.7/sdock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 03:04:17.000000 sdock-0.1.7/sdock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:04:17.000000 sdock-0.1.7/sdock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 03:04:17.000000 sdock-0.1.7/sdock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 03:04:17.000000 sdock-0.1.7/sdock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:04:17.215017 sdock-0.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-18 03:04:13.000000 sdock-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:06:34.317528 sdock-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 03:06:30.000000 sdock-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:06:34.317528 sdock-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 03:06:30.000000 sdock-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:06:34.317528 sdock-0.1.8/sdock/
+-rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-18 03:06:30.000000 sdock-0.1.8/sdock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-18 03:06:30.000000 sdock-0.1.8/sdock/vbgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:06:34.317528 sdock-0.1.8/sdock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:06:34.317528 sdock-0.1.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-18 03:06:30.000000 sdock-0.1.8/setup.py
```

### Comparing `sdock-0.1.7/LICENSE` & `sdock-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sdock-0.1.7/sdock/__init__.py` & `sdock-0.1.8/sdock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,15 @@
 		]) + str(self.clean()+";" if self.postClean else "")
 
 	def __str__(self):
 		return self.string()
 	
 	def compose(self, output_file:str=""):
 		#https://docs.docker.com/compose/gettingstarted/
+		return
 
 @dataclass
 class vb:
 	"""Class for keeping track of an item in inventory."""
 	vmname: str = "takenname"
 	username: str = None
 	ovafile: str = None
```

### Comparing `sdock-0.1.7/sdock/vbgen.py` & `sdock-0.1.8/sdock/vbgen.py`

 * *Files identical despite different names*

### Comparing `sdock-0.1.7/setup.py` & `sdock-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.7.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

