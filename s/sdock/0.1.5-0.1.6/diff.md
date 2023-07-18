# Comparing `tmp/sdock-0.1.5.tar.gz` & `tmp/sdock-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdock-0.1.5.tar", last modified: Tue Jul 18 00:26:34 2023, max compression
+gzip compressed data, was "sdock-0.1.6.tar", last modified: Tue Jul 18 02:55:49 2023, max compression
```

## Comparing `sdock-0.1.5.tar` & `sdock-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:26:34.616262 sdock-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 00:26:30.000000 sdock-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 00:26:34.616262 sdock-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 00:26:30.000000 sdock-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:26:34.616262 sdock-0.1.5/sdock/
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-07-18 00:26:30.000000 sdock-0.1.5/sdock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-18 00:26:30.000000 sdock-0.1.5/sdock/vbgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:26:34.616262 sdock-0.1.5/sdock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 00:26:34.616262 sdock-0.1.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-18 00:26:30.000000 sdock-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:55:49.538637 sdock-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 02:55:45.000000 sdock-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 02:55:49.538637 sdock-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 02:55:45.000000 sdock-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:55:49.538637 sdock-0.1.6/sdock/
+-rw-r--r--   0 runner    (1001) docker     (123)    26199 2023-07-18 02:55:45.000000 sdock-0.1.6/sdock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-18 02:55:45.000000 sdock-0.1.6/sdock/vbgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:55:49.538637 sdock-0.1.6/sdock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 02:55:49.000000 sdock-0.1.6/sdock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 02:55:49.000000 sdock-0.1.6/sdock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:55:49.000000 sdock-0.1.6/sdock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 02:55:49.000000 sdock-0.1.6/sdock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 02:55:49.000000 sdock-0.1.6/sdock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:55:49.538637 sdock-0.1.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-18 02:55:45.000000 sdock-0.1.6/setup.py
```

### Comparing `sdock-0.1.5/LICENSE` & `sdock-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sdock-0.1.5/sdock/__init__.py` & `sdock-0.1.6/sdock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 		if use_lite:
 			output = output.replace(':latest','') + ":lite"
 		output = output.replace(':latest:latest',':latest').replace(':lite:lite',':lite')
 
 		if usebaredocker:
 			output = output.replace("{}/".format(docker_username),"")
 
-		return output
+		return ':'.join(text.split(":")[0:2]) #Fixes a problem where there's an output of :ui:latest
 	else:
 		return string
 
 @dataclass
 class dock:
 	"""Class for keeping track of an item in inventory."""
 	docker: str = "docker"
@@ -272,14 +272,17 @@
 			my_save_host_dir,
 			self.image,
 			cmd
 		]) + str(self.clean()+";" if self.postClean else "")
 
 	def __str__(self):
 		return self.string()
+	
+	def compose(self, output_file:str=""):
+		#https://docs.docker.com/compose/gettingstarted/
 
 @dataclass
 class vb:
 	"""Class for keeping track of an item in inventory."""
 	vmname: str = "takenname"
 	username: str = None
 	ovafile: str = None
```

### Comparing `sdock-0.1.5/sdock/vbgen.py` & `sdock-0.1.6/sdock/vbgen.py`

 * *Files identical despite different names*

### Comparing `sdock-0.1.5/setup.py` & `sdock-0.1.6/setup.py`

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
-VERSION = "0.1.5"
+VERSION = "0.1.6"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

