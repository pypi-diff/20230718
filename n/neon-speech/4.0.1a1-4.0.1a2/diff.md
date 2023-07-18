# Comparing `tmp/neon_speech-4.0.1a1.tar.gz` & `tmp/neon_speech-4.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_speech-4.0.1a1.tar", last modified: Tue Jun 27 21:42:56 2023, max compression
+gzip compressed data, was "neon_speech-4.0.1a2.tar", last modified: Tue Jul 18 19:00:22 2023, max compression
```

## Comparing `neon_speech-4.0.1a1.tar` & `neon_speech-4.0.1a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:42:56.564944 neon_speech-4.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-27 21:42:56.564944 neon_speech-4.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:42:56.560944 neon_speech-4.0.1a1/neon_speech/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/neon_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/neon_speech/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/neon_speech/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/neon_speech/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/neon_speech/stt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/neon_speech/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 21:42:56.564944 neon_speech-4.0.1a1/neon_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-27 21:42:56.000000 neon_speech-4.0.1a1/neon_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-27 21:42:56.000000 neon_speech-4.0.1a1/neon_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 21:42:56.000000 neon_speech-4.0.1a1/neon_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 21:42:56.000000 neon_speech-4.0.1a1/neon_speech.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-27 21:42:56.000000 neon_speech-4.0.1a1/neon_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-27 21:42:56.000000 neon_speech-4.0.1a1/neon_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 21:42:56.564944 neon_speech-4.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-27 21:42:51.000000 neon_speech-4.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:22.726611 neon_speech-4.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-18 19:00:22.726611 neon_speech-4.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:22.722612 neon_speech-4.0.1a2/neon_speech/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/neon_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/neon_speech/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/neon_speech/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20934 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/neon_speech/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/neon_speech/stt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/neon_speech/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:00:22.726611 neon_speech-4.0.1a2/neon_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-18 19:00:22.000000 neon_speech-4.0.1a2/neon_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-18 19:00:22.000000 neon_speech-4.0.1a2/neon_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:00:22.000000 neon_speech-4.0.1a2/neon_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 19:00:22.000000 neon_speech-4.0.1a2/neon_speech.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-18 19:00:22.000000 neon_speech-4.0.1a2/neon_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 19:00:22.000000 neon_speech-4.0.1a2/neon_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:00:22.726611 neon_speech-4.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-18 19:00:18.000000 neon_speech-4.0.1a2/setup.py
```

### Comparing `neon_speech-4.0.1a1/LICENSE.md` & `neon_speech-4.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.0.1a1/PKG-INFO` & `neon_speech-4.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_speech
-Version: 4.0.1a1
+Version: 4.0.1a2
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.0.1a1/README.md` & `neon_speech-4.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon_speech-4.0.1a1/neon_speech/__init__.py` & `neon_speech-4.0.1a2/neon_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.0.1a1/neon_speech/__main__.py` & `neon_speech-4.0.1a2/neon_speech/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,9 +51,16 @@
         try:
             print_malloc(snapshot_malloc())
         except Exception as e:
             LOG.error(e)
     service.shutdown()
 
 
+def deprecated_entrypoint():
+    from ovos_utils.log import log_deprecation
+    log_deprecation("Use `neon-speech run` in place of `neon_speech_client`",
+                    "2.0.0")
+    main()
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `neon_speech-4.0.1a1/neon_speech/cli.py` & `neon_speech-4.0.1a2/neon_speech/cli.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.0.1a1/neon_speech/service.py` & `neon_speech-4.0.1a2/neon_speech/service.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.0.1a1/neon_speech/stt.py` & `neon_speech-4.0.1a2/neon_speech/stt.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.0.1a1/neon_speech/utils.py` & `neon_speech-4.0.1a2/neon_speech/utils.py`

 * *Files identical despite different names*

### Comparing `neon_speech-4.0.1a1/neon_speech.egg-info/PKG-INFO` & `neon_speech-4.0.1a2/neon_speech.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-speech
-Version: 4.0.1a1
+Version: 4.0.1a2
 Summary: Neon Speech Module
 Home-page: https://github.com/NeonGeckoCom/neon_speech
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon_speech-4.0.1a1/setup.py` & `neon_speech-4.0.1a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,12 +75,12 @@
     author_email='developers@neon.ai',
     description="Neon Speech Module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
             # TODO: Deprecate `neon_speech_client` entrypoint
-            'neon_speech_client=neon_speech.__main__:main',
+            'neon_speech_client=neon_speech.__main__:deprecated_entrypoint',
             'neon-speech=neon_speech.cli:neon_speech_cli'
         ]
     }
 )
```

