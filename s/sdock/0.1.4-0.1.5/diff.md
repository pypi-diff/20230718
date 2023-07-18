# Comparing `tmp/sdock-0.1.4.tar.gz` & `tmp/sdock-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdock-0.1.4.tar", last modified: Mon Jul 17 19:31:27 2023, max compression
+gzip compressed data, was "sdock-0.1.5.tar", last modified: Tue Jul 18 00:26:34 2023, max compression
```

## Comparing `sdock-0.1.4.tar` & `sdock-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:31:27.292322 sdock-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 19:31:23.000000 sdock-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 19:31:27.292322 sdock-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 19:31:23.000000 sdock-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:31:27.292322 sdock-0.1.4/sdock/
--rw-r--r--   0 runner    (1001) docker     (123)    26016 2023-07-17 19:31:23.000000 sdock-0.1.4/sdock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-17 19:31:23.000000 sdock-0.1.4/sdock/vbgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:31:27.292322 sdock-0.1.4/sdock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 19:31:27.000000 sdock-0.1.4/sdock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 19:31:27.000000 sdock-0.1.4/sdock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:31:27.000000 sdock-0.1.4/sdock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 19:31:27.000000 sdock-0.1.4/sdock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 19:31:27.000000 sdock-0.1.4/sdock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:31:27.292322 sdock-0.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-17 19:31:23.000000 sdock-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:26:34.616262 sdock-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 00:26:30.000000 sdock-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 00:26:34.616262 sdock-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 00:26:30.000000 sdock-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:26:34.616262 sdock-0.1.5/sdock/
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-07-18 00:26:30.000000 sdock-0.1.5/sdock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-18 00:26:30.000000 sdock-0.1.5/sdock/vbgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:26:34.616262 sdock-0.1.5/sdock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 00:26:34.000000 sdock-0.1.5/sdock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 00:26:34.616262 sdock-0.1.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-18 00:26:30.000000 sdock-0.1.5/setup.py
```

### Comparing `sdock-0.1.4/LICENSE` & `sdock-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sdock-0.1.4/sdock/__init__.py` & `sdock-0.1.5/sdock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 		return ' '.join([
 			f"{prefix} {port if checkPort(port) else open_port()}" for port in ports
 		])
 
 def cur_dir():
 	return '%cd%' if sys.platform in ['win32', 'cygwin'] else '`pwd`'
 
-def dockerImage(docker_username, string, usebaredocker=False):
+def dockerImage(string, usebaredocker=False, docker_username="frantzme"):
 	if not usebaredocker and "/" not in string:
 		use_lite = ":lite" in string
 		if "pydev" in string:
 			output = f"{docker_username}/pythondev:latest"
 		elif "pytest" in string:
 			output = f"{docker_username}/pythontesting:latest"
 		else:
```

### Comparing `sdock-0.1.4/sdock/vbgen.py` & `sdock-0.1.5/sdock/vbgen.py`

 * *Files identical despite different names*

### Comparing `sdock-0.1.4/setup.py` & `sdock-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.7.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

