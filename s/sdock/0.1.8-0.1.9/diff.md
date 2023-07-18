# Comparing `tmp/sdock-0.1.8.tar.gz` & `tmp/sdock-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdock-0.1.8.tar", last modified: Tue Jul 18 03:06:34 2023, max compression
+gzip compressed data, was "sdock-0.1.9.tar", last modified: Tue Jul 18 04:08:41 2023, max compression
```

## Comparing `sdock-0.1.8.tar` & `sdock-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:06:34.317528 sdock-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 03:06:30.000000 sdock-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:06:34.317528 sdock-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 03:06:30.000000 sdock-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:06:34.317528 sdock-0.1.8/sdock/
--rw-r--r--   0 runner    (1001) docker     (123)    26210 2023-07-18 03:06:30.000000 sdock-0.1.8/sdock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-18 03:06:30.000000 sdock-0.1.8/sdock/vbgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:06:34.317528 sdock-0.1.8/sdock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 03:06:34.000000 sdock-0.1.8/sdock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:06:34.317528 sdock-0.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-18 03:06:30.000000 sdock-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:41.592350 sdock-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 04:08:37.000000 sdock-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 04:08:41.592350 sdock-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 04:08:37.000000 sdock-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:41.592350 sdock-0.1.9/sdock/
+-rw-r--r--   0 runner    (1001) docker     (123)    26367 2023-07-18 04:08:37.000000 sdock-0.1.9/sdock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-18 04:08:37.000000 sdock-0.1.9/sdock/vbgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:08:41.592350 sdock-0.1.9/sdock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 04:08:41.000000 sdock-0.1.9/sdock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-18 04:08:41.000000 sdock-0.1.9/sdock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:08:41.000000 sdock-0.1.9/sdock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 04:08:41.000000 sdock-0.1.9/sdock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 04:08:41.000000 sdock-0.1.9/sdock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:08:41.592350 sdock-0.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-18 04:08:37.000000 sdock-0.1.9/setup.py
```

### Comparing `sdock-0.1.8/LICENSE` & `sdock-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sdock-0.1.8/sdock/__init__.py` & `sdock-0.1.9/sdock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,14 +123,15 @@
 	login: bool = False
 	loggout: bool = False
 	logg: bool = False
 	macaddress: str = None
 	postClean: bool = False
 	preClean: bool = False
 	extra: str = None
+	raw: str = None
 	save_host_dir: bool = False
 	docker_username:str="frantzme"
 	docker_id:str=None
 
 	@staticmethod
 	def cur_dir():
 		return '%cd%' if sys.platform in ['win32', 'cygwin'] else '`pwd`'
@@ -255,25 +256,33 @@
 		if self.save_host_dir:
 			if 'HOSTDIR' in os.environ:
 				past_dir,current_dir = os.environ['HOSTDIR'], os.path.abspath(os.curdir).replace('/sync/','')
 				my_save_host_dir = '--env="HOSTDIR={0}/{1}"'.format(past_dir,current_dir)
 			else:
 				my_save_host_dir = '--env="HOSTDIR={0}"'.format(dir)
 
+		raw_input = ''
+		if raw:
+			if isinstance(raw, list):
+				raw_input = ' '.join(self.raw)
+			else:
+				raw_input = self.raw
+
 		return str(self.clean()+";" if self.preClean else "") + "{0} run ".format(self.docker) + " ".join([
 			dockerInDocker,
 			'--rm' if self.remove else '',
 			'-d' if self.detach else '-it',
 			'' if no_mount else '-v "{0}:{1}"'.format(use_dir, self.mountto),
 			exchanged,
 			network,
 			getPort(self.ports),
 			'--mac-address ' + str(self.macaddress) if self.macaddress else '',
 			self.extra if self.extra else '',
 			my_save_host_dir,
+			raw_input,
 			self.image,
 			cmd
 		]) + str(self.clean()+";" if self.postClean else "")
 
 	def __str__(self):
 		return self.string()
```

### Comparing `sdock-0.1.8/sdock/vbgen.py` & `sdock-0.1.9/sdock/vbgen.py`

 * *Files identical despite different names*

### Comparing `sdock-0.1.8/setup.py` & `sdock-0.1.9/setup.py`

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
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

