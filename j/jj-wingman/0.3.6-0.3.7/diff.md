# Comparing `tmp/jj_wingman-0.3.6.tar.gz` & `tmp/jj_wingman-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.3.6.tar", last modified: Thu Jun 22 17:56:44 2023, max compression
+gzip compressed data, was "jj_wingman-0.3.7.tar", last modified: Mon Jul 17 22:29:13 2023, max compression
```

## Comparing `jj_wingman-0.3.6.tar` & `jj_wingman-0.3.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-22 17:56:44.752318 jj_wingman-0.3.6/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.3.6/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)    15275 2023-06-22 17:56:44.752318 jj_wingman-0.3.6/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)    13579 2023-06-21 18:39:48.000000 jj_wingman-0.3.6/README.md
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-22 17:56:44.752318 jj_wingman-0.3.6/jj_wingman.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)    15275 2023-06-22 17:56:44.000000 jj_wingman-0.3.6/jj_wingman.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-06-22 17:56:44.000000 jj_wingman-0.3.6/jj_wingman.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-06-22 17:56:44.000000 jj_wingman-0.3.6/jj_wingman.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-06-22 17:56:44.000000 jj_wingman-0.3.6/jj_wingman.egg-info/entry_points.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-06-22 17:56:44.000000 jj_wingman-0.3.6/jj_wingman.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-06-22 17:56:44.000000 jj_wingman-0.3.6/jj_wingman.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-06-22 17:56:30.000000 jj_wingman-0.3.6/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-06-22 17:56:44.752318 jj_wingman-0.3.6/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.3.6/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-22 17:56:44.752318 jj_wingman-0.3.6/test/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.3.6/test/test_replay_buffer.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-06-22 17:56:44.752318 jj_wingman-0.3.6/wingman/
--rw-rw-r--   0 jet       (1000) jet       (1000)      218 2023-06-02 11:46:07.000000 jj_wingman-0.3.6/wingman/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.3.6/wingman/cli_scripts.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      306 2023-06-21 18:19:17.000000 jj_wingman-0.3.6/wingman/config.yaml
--rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-06-02 11:46:40.000000 jj_wingman-0.3.6/wingman/neural_blocks.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1113 2023-06-21 18:59:06.000000 jj_wingman-0.3.6/wingman/print_utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.3.6/wingman/replay_buffer.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1025 2023-06-22 17:56:22.000000 jj_wingman-0.3.6/wingman/utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15817 2023-06-21 18:43:26.000000 jj_wingman-0.3.6/wingman/wingman.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 22:29:13.076057 jj_wingman-0.3.7/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.3.7/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15275 2023-07-17 22:29:13.076057 jj_wingman-0.3.7/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)    13579 2023-06-21 18:39:48.000000 jj_wingman-0.3.7/README.md
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 22:29:13.076057 jj_wingman-0.3.7/jj_wingman.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15275 2023-07-17 22:29:13.000000 jj_wingman-0.3.7/jj_wingman.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-07-17 22:29:13.000000 jj_wingman-0.3.7/jj_wingman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-17 22:29:13.000000 jj_wingman-0.3.7/jj_wingman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-07-17 22:29:13.000000 jj_wingman-0.3.7/jj_wingman.egg-info/entry_points.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-07-17 22:29:13.000000 jj_wingman-0.3.7/jj_wingman.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-07-17 22:29:13.000000 jj_wingman-0.3.7/jj_wingman.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-07-17 22:29:08.000000 jj_wingman-0.3.7/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-17 22:29:13.076057 jj_wingman-0.3.7/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.3.7/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 22:29:13.076057 jj_wingman-0.3.7/test/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3917 2023-05-29 12:52:26.000000 jj_wingman-0.3.7/test/test_replay_buffer.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-17 22:29:13.076057 jj_wingman-0.3.7/wingman/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      218 2023-06-02 11:46:07.000000 jj_wingman-0.3.7/wingman/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.3.7/wingman/cli_scripts.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      306 2023-06-21 18:19:17.000000 jj_wingman-0.3.7/wingman/config.yaml
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10283 2023-06-02 11:46:40.000000 jj_wingman-0.3.7/wingman/neural_blocks.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1113 2023-06-21 18:59:06.000000 jj_wingman-0.3.7/wingman/print_utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5617 2023-05-21 21:59:51.000000 jj_wingman-0.3.7/wingman/replay_buffer.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1099 2023-07-17 22:29:03.000000 jj_wingman-0.3.7/wingman/utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15817 2023-06-21 18:43:26.000000 jj_wingman-0.3.7/wingman/wingman.py
```

### Comparing `jj_wingman-0.3.6/LICENSE.txt` & `jj_wingman-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.6/PKG-INFO` & `jj_wingman-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.3.6
+Version: 0.3.7
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.3.6/README.md` & `jj_wingman-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.6/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.3.7/jj_wingman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jj-wingman
-Version: 0.3.6
+Version: 0.3.7
 Summary: Wingman library for AI projects.
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `jj_wingman-0.3.6/pyproject.toml` & `jj_wingman-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jj_wingman-0.3.6/test/test_replay_buffer.py` & `jj_wingman-0.3.7/test/test_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.6/wingman/cli_scripts.py` & `jj_wingman-0.3.7/wingman/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.6/wingman/neural_blocks.py` & `jj_wingman-0.3.7/wingman/neural_blocks.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.6/wingman/print_utils.py` & `jj_wingman-0.3.7/wingman/print_utils.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.6/wingman/replay_buffer.py` & `jj_wingman-0.3.7/wingman/replay_buffer.py`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.3.6/wingman/utils.py` & `jj_wingman-0.3.7/wingman/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,26 +7,24 @@
     import torch
 except ImportError as e:
     raise ImportError(
         "Could not import torch, this is not bundled as part of Wingman and has to be installed manually."
     ) from e
 
 
-def gpuize(input, device: str = "cuda:0") -> torch.Tensor:
+def gpuize(input, device: str = "cuda:0", keeptype: bool = False) -> torch.Tensor:
     """gpuize.
 
     Args:
         input: the array that we want to gpuize
         device: a string of the device we want to move the thing to
+        keeptype: a boolean on whether to keep the original dtype, otherwise, the tensor is converted to torch.float64
     """
-    if torch.is_tensor(input):
-        if input.device == device:
-            return input
-        return input.to(device)
-    return torch.tensor(input).to(device)
+    dtype = input.dtype if keeptype else torch.float64
+    return input.to(device, dtype=dtype)
 
 
 def cpuize(input) -> np.ndarray:
     """cpuize.
 
     Args:
         input: the array of the thing we want to put on the cpu
```

### Comparing `jj_wingman-0.3.6/wingman/wingman.py` & `jj_wingman-0.3.7/wingman/wingman.py`

 * *Files identical despite different names*

