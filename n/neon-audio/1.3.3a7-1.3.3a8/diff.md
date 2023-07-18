# Comparing `tmp/neon-audio-1.3.3a7.tar.gz` & `tmp/neon-audio-1.3.3a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-audio-1.3.3a7.tar", last modified: Wed Jul 12 01:51:55 2023, max compression
+gzip compressed data, was "neon-audio-1.3.3a8.tar", last modified: Tue Jul 18 19:17:31 2023, max compression
```

## Comparing `neon-audio-1.3.3a7.tar` & `neon-audio-1.3.3a8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.496967 neon-audio-1.3.3a7/neon_audio/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.496967 neon-audio-1.3.3a7/neon_audio/tts/
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/tts/neon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/neon_audio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.496967 neon-audio-1.3.3a7/neon_audio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:51:55.000000 neon-audio-1.3.3a7/neon_audio.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/api_method_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:51:55.500967 neon-audio-1.3.3a7/tests/test_objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/test_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-12 01:51:46.000000 neon-audio-1.3.3a7/tests/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:17:31.211421 neon-audio-1.3.3a8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-18 19:17:31.211421 neon-audio-1.3.3a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:17:31.207421 neon-audio-1.3.3a8/neon_audio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/neon_audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/neon_audio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/neon_audio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/neon_audio/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:17:31.211421 neon-audio-1.3.3a8/neon_audio/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/neon_audio/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/neon_audio/tts/neon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/neon_audio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:17:31.211421 neon-audio-1.3.3a8/neon_audio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-18 19:17:31.000000 neon-audio-1.3.3a8/neon_audio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-18 19:17:31.000000 neon-audio-1.3.3a8/neon_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:17:31.000000 neon-audio-1.3.3a8/neon_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 19:17:31.000000 neon-audio-1.3.3a8/neon_audio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-18 19:17:31.000000 neon-audio-1.3.3a8/neon_audio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 19:17:31.000000 neon-audio-1.3.3a8/neon_audio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:17:31.000000 neon-audio-1.3.3a8/neon_audio.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:17:31.211421 neon-audio-1.3.3a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:17:31.211421 neon-audio-1.3.3a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10567 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/tests/api_method_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:17:31.211421 neon-audio-1.3.3a8/tests/test_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/tests/test_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-18 19:17:26.000000 neon-audio-1.3.3a8/tests/unit_tests.py
```

### Comparing `neon-audio-1.3.3a7/LICENSE.md` & `neon-audio-1.3.3a8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/PKG-INFO` & `neon-audio-1.3.3a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.3.3a7
+Version: 1.3.3a8
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.3.3a7/README.md` & `neon-audio-1.3.3a8/README.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/neon_audio/__init__.py` & `neon-audio-1.3.3a8/neon_audio/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/neon_audio/__main__.py` & `neon-audio-1.3.3a8/neon_audio/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,9 +65,16 @@
         try:
             print_malloc(snapshot_malloc())
         except Exception as e:
             LOG.error(e)
     service.shutdown()
 
 
+def deprecated_entrypoint():
+    from ovos_utils.log import log_deprecation
+    log_deprecation("Use `neon-audio run` in place of "
+                    "`neon_audio_client`", "2.0.0")
+    main()
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `neon-audio-1.3.3a7/neon_audio/cli.py` & `neon-audio-1.3.3a8/neon_audio/cli.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/neon_audio/service.py` & `neon-audio-1.3.3a8/neon_audio/service.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/neon_audio/tts/__init__.py` & `neon-audio-1.3.3a8/neon_audio/tts/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/neon_audio/tts/neon.py` & `neon-audio-1.3.3a8/neon_audio/tts/neon.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/neon_audio/utils.py` & `neon-audio-1.3.3a8/neon_audio/utils.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/neon_audio.egg-info/PKG-INFO` & `neon-audio-1.3.3a8/neon_audio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.3.3a7
+Version: 1.3.3a8
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.3.3a7/neon_audio.egg-info/SOURCES.txt` & `neon-audio-1.3.3a8/neon_audio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/setup.py` & `neon-audio-1.3.3a8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,12 +81,12 @@
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
     ],
     entry_points={
         'console_scripts': [
             # TODO: Deprecate neon_audio_client entrypoint
-            'neon_audio_client=neon_audio.__main__:main',
+            'neon_audio_client=neon_audio.__main__:deprecated_entrypoint',
             'neon-audio=neon_audio.cli:neon_audio_cli'
         ]
     }
 )
```

### Comparing `neon-audio-1.3.3a7/tests/__init__.py` & `neon-audio-1.3.3a8/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/tests/api_method_tests.py` & `neon-audio-1.3.3a8/tests/api_method_tests.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/tests/test_objects/__init__.py` & `neon-audio-1.3.3a8/tests/test_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.3.3a7/tests/unit_tests.py` & `neon-audio-1.3.3a8/tests/unit_tests.py`

 * *Files identical despite different names*

