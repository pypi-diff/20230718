# Comparing `tmp/linkplay-cli-0.0.4.tar.gz` & `tmp/linkplay-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkplay-cli-0.0.4.tar", last modified: Mon Jul 17 17:29:39 2023, max compression
+gzip compressed data, was "linkplay-cli-0.0.5.tar", last modified: Tue Jul 18 07:56:12 2023, max compression
```

## Comparing `linkplay-cli-0.0.4.tar` & `linkplay-cli-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/linkplay_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21069 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/firmware_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/linkplay_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/linkplay_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-17 17:29:39.000000 linkplay-cli-0.0.4/linkplay_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 17:29:39.602148 linkplay-cli-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-17 17:29:28.000000 linkplay-cli-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:12.234609 linkplay-cli-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-18 07:56:12.234609 linkplay-cli-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:12.234609 linkplay-cli-0.0.5/linkplay_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/linkplay_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21069 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/linkplay_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/linkplay_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/linkplay_cli/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/linkplay_cli/firmware_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/linkplay_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:12.234609 linkplay-cli-0.0.5/linkplay_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-18 07:56:12.000000 linkplay-cli-0.0.5/linkplay_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 07:56:12.000000 linkplay-cli-0.0.5/linkplay_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:56:12.000000 linkplay-cli-0.0.5/linkplay_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 07:56:12.000000 linkplay-cli-0.0.5/linkplay_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 07:56:12.000000 linkplay-cli-0.0.5/linkplay_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 07:56:12.000000 linkplay-cli-0.0.5/linkplay_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:56:12.234609 linkplay-cli-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-18 07:56:03.000000 linkplay-cli-0.0.5/setup.py
```

### Comparing `linkplay-cli-0.0.4/LICENSE` & `linkplay-cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.4/PKG-INFO` & `linkplay-cli-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkplay-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Control Linkplay devices from the comfort of your shell
 Home-page: https://github.com/ramikg/linkplay-cli
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linkplay CLI
```

### Comparing `linkplay-cli-0.0.4/README.md` & `linkplay-cli-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.4/linkplay_cli/cli.py` & `linkplay-cli-0.0.5/linkplay_cli/cli.py`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.4/linkplay_cli/discovery.py` & `linkplay-cli-0.0.5/linkplay_cli/discovery.py`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.4/linkplay_cli/firmware_update.py` & `linkplay-cli-0.0.5/linkplay_cli/firmware_update.py`

 * *Files identical despite different names*

### Comparing `linkplay-cli-0.0.4/linkplay_cli/utils.py` & `linkplay-cli-0.0.5/linkplay_cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 def _supress_openssl_warning_when_importing_requests():
     """
     Invoking the CLI on a system without OpenSSL (e.g. one with LibreSSL) may result in a warning we'd like to supress.
     This warning is raised when importing urllib3 >= 2.0.3 (which the requests library may do).
     """
     with warnings.catch_warnings(record=True) as caught_warnings:
-        from urllib3.exceptions import NotOpenSSLWarning
+        try:
+            from urllib3.exceptions import NotOpenSSLWarning
+        except ImportError:
+            return
 
     for w in caught_warnings:
         if w.category is NotOpenSSLWarning:
             continue
         else:
             warnings.warn(message=w.message, category=w.category, source=w.source)
```

### Comparing `linkplay-cli-0.0.4/linkplay_cli.egg-info/PKG-INFO` & `linkplay-cli-0.0.5/linkplay_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkplay-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Control Linkplay devices from the comfort of your shell
 Home-page: https://github.com/ramikg/linkplay-cli
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Linkplay CLI
```

### Comparing `linkplay-cli-0.0.4/setup.py` & `linkplay-cli-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = readme.read()
 
 setup(name='linkplay-cli',
       description='Control Linkplay devices from the comfort of your shell',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ramikg/linkplay-cli',
-      version='0.0.4',
+      version='0.0.5',
       packages=find_packages(),
       install_requires=[
           'async_upnp_client',
           'beautifulsoup4',
           'lxml',
           'prettytable',
           'pycryptodome',
```

