# Comparing `tmp/eons-2.7.2.tar.gz` & `tmp/eons-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.7.2.tar", last modified: Mon Jul 17 15:15:20 2023, max compression
+gzip compressed data, was "eons-2.7.3.tar", last modified: Tue Jul 18 04:45:08 2023, max compression
```

## Comparing `eons-2.7.2.tar` & `eons-2.7.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.355358 eons-2.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 15:15:20.355358 eons-2.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-17 15:14:53.000000 eons-2.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.347358 eons-2.7.2/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.351358 eons-2.7.2/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99076 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.351358 eons-2.7.2/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.355358 eons-2.7.2/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:15:11.000000 eons-2.7.2/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-17 15:14:41.000000 eons-2.7.2/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:15:20.351358 eons-2.7.2/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 15:15:20.000000 eons-2.7.2/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-17 15:15:11.000000 eons-2.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 15:15:20.355358 eons-2.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-18 04:45:08.520157 eons-2.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-07-18 04:44:50.000000 eons-2.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.516157 eons-2.7.3/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99533 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:44:59.000000 eons-2.7.3/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 04:44:42.000000 eons-2.7.3/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:45:08.520157 eons-2.7.3/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25510 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 04:45:08.000000 eons-2.7.3/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-18 04:44:59.000000 eons-2.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-18 04:45:08.520157 eons-2.7.3/setup.cfg
```

### Comparing `eons-2.7.2/PKG-INFO` & `eons-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.2
+Version: 2.7.3
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.7.2/README.md` & `eons-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.7.2/pkg/eons/eons.py` & `eons-2.7.3/pkg/eons/eons.py`

 * *Files 1% similar despite different names*

```diff
@@ -885,15 +885,16 @@
 	def PrepareNext(this, next):
 		pass
 
 
 	# Call the next Functor.
 	# RETURN the result of the next Functor or None.
 	def CallNext(this):
-		if (not this.next):
+		# TODO: Why would next ever not be a list This should be the same as the FIXME below.s
+		if (not this.next or not isinstance(this.next, list) or len(this.next) == 0):
 			return None
 		
 		# Something odd happens here; we've been getting:
 		# AttributeError("'builtin_function_or_method' object has no attribute 'pop'")
 		# But that implies we're getting a valid next object that is not a list.
 		# FIXME: Debug this.
 		proceedToNext = False
@@ -1712,23 +1713,27 @@
 							functor,
 							arg.default.parameters,
 							source,
 							ctor
 						)
 						shouldMapArg = False
 					else:
-						ctor.source.append(f"this.optionalKWArgs['{arg.name}'] = {arg.default}")
+						defaultValue = arg.default
+						if (isinstance(arg.default, str)):
+							defaultValue = f"'{arg.default}'"
+						ctor.source.append(f"this.optionalKWArgs['{arg.name}'] = {defaultValue}")
 				else:
 					ctor.source.append(f"this.requiredKWArgs.append('{arg.name}')")
 
 				if (shouldMapArg):
 					ctor.source.append(f"this.argMapping.append('{arg.name}')")
 
 			# Source mangling
-			source = source.replace(arg.name, replaceWith)
+			# TODO: Expand as we have more solid test cases.
+			source = re.sub(fr"{arg.name}([\s\[\]\.\(\)\}}\*\+/-=%])", fr"{replaceWith}\1", source)
 			
 		return functor, source, ctor
 
 	def FunctionToFunctor(function):
 		executor = ExecutorTracker.GetLatest()
 		shouldLog = executor and executor.verbosity > 3
 
@@ -1745,16 +1750,16 @@
 		)
 
 		if ('name' not in kwargs):
 			kwargs['name'] = function.__name__
 	
 		args = inspect.signature(function).parameters
 		source = inspect.getsource(function)
-		source = source[source.find(':')+1:].strip()
-		source = source.replace('caller', 'this.caller')
+		source = source[source.find(':\n')+1:].strip() # Will fail if an arg has ':\n' in it
+		source = re.sub(r'caller([\s\[\]\.\(\)\}\*\+/-=%])', r'this.caller\1', source)
 
 		ctor = util.DotDict()
 		ctor.source = []
 		ctor.additions = ""
 
 		functor, source, ctor = ParseParameters(functor, args, source, ctor)
 
@@ -2068,17 +2073,17 @@
 		this.enableAutoReturn = False
 
 		this.resolveErrors = True
 		this.errorRecursionDepth = 0
 		this.errorResolutionStack = {}
 		this.resolveErrorsWith = [ # order matters: FIFO (first is first).
 			'find_by_fetch',
+			'import_module',
 			'install_from_repo_with_default_package_type',
 			'install_from_repo',
-			'import_module',
 			'install_with_pip'
 		]
 
 		# Caching is required for Functor's staticKWArgs and other static features to be effective.
 		# This is used in Execute().
 		this.cachedFunctors = {}
 
@@ -2694,24 +2699,24 @@
 
 		return registered
 
 
 	# Non-static override of the SelfRegistering method.
 	# Needed for errorObject resolution.
 	@recoverable
-	def RegisterAllClassesInDirectory(this, directory):
+	def RegisterAllClassesInDirectory(this, directory, recurse=True):
 		path = Path(directory)
 		if (not path.exists()):
 			logging.debug(f"Making path for SelfRegitering classes: {str(path)}")
 			path.mkdir(parents=True, exist_ok=True)
 
 		if (directory not in this.syspath):
 			this.syspath.append(directory)
 
-		SelfRegistering.RegisterAllClassesInDirectory(directory)
+		SelfRegistering.RegisterAllClassesInDirectory(directory, recurse=recurse)
 
 
 	# Utility method. may not be useful.
 	@staticmethod
 	def SplitNameOnpackageType(name):
 		splitName = name.split('_')
 		if (len(splitName)>1):
```

### Comparing `eons-2.7.2/pkg/eons/method/External.py` & `eons-2.7.3/pkg/eons/method/External.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,18 +29,32 @@
 
 		# To allow this.functor to be called with *args, we must also allow this to be called with *args.
 		this.argMapping = this.functor.argMapping
 
 	def PopulateFrom(this, function):
 		this.functorName = function.__name__
 
-	def Function(this):
+	def GetKWArgsForMethod(this):
 		kwargs = this.kwargs
 		kwargs.update({
 			'executor': this.executor,
 			'precursor': this,
 		})
-		
 		this.functor.caller = this.caller
-		
-		return this.functor(*this.args, **kwargs)
-	
+		return kwargs
+
+	def Function(this):
+		ret = this.functor(*this.args, **this.GetKWArgsForMethod())
+		this.result = this.functor.result
+		return ret
+
+	def Rollback(this):
+		this.functor.WarmUp(*this.args, **this.GetKWArgsForMethod())
+		ret = this.functor.Rollback()
+		this.result = this.functor.result
+		return ret
+	
+	def DidFunctionSucceed(this):
+		return this.functor.DidFunctionSucceed()
+	
+	def DidRollbackSucceed(this):
+		return this.functor.DidRollbackSucceed()
```

### Comparing `eons-2.7.2/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.7.3/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.2/pkg/eons/resolve/resolve_import_module.py` & `eons-2.7.3/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.2/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.7.3/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.7.2/pkg/eons.egg-info/PKG-INFO` & `eons-2.7.3/pkg/eons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.7.2
+Version: 2.7.3
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.7.2/pkg/eons.egg-info/SOURCES.txt` & `eons-2.7.3/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.7.2/setup.cfg` & `eons-2.7.3/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.7.2
+version = 2.7.3
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -19,19 +19,19 @@
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	requests_futures
+	tqdm
 	eot
 	jsonpickle
-	requests
 	pyyaml
-	tqdm
+	requests
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

