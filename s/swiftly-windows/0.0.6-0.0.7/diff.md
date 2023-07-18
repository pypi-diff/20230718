# Comparing `tmp/swiftly-windows-0.0.6.tar.gz` & `tmp/swiftly-windows-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftly-windows-0.0.6.tar", last modified: Tue Jul 18 20:56:52 2023, max compression
+gzip compressed data, was "swiftly-windows-0.0.7.tar", last modified: Tue Jul 18 21:00:47 2023, max compression
```

## Comparing `swiftly-windows-0.0.6.tar` & `swiftly-windows-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:56:52.673809 swiftly-windows-0.0.6/
--rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-18 20:18:06.000000 swiftly-windows-0.0.6/LICENSE
--rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 20:56:52.673683 swiftly-windows-0.0.6/PKG-INFO
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:56:52.672272 swiftly-windows-0.0.6/scripts/
--rw-r--r--   0 brainspoof   (501) staff       (20)     6133 2023-07-18 20:55:45.000000 swiftly-windows-0.0.6/scripts/swiftly.bat
--rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-18 20:56:52.673844 swiftly-windows-0.0.6/setup.cfg
--rw-r--r--   0 brainspoof   (501) staff       (20)      169 2023-07-18 20:56:48.000000 swiftly-windows-0.0.6/setup.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:56:52.673075 swiftly-windows-0.0.6/swiftly_windows/
--rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:18:06.000000 swiftly-windows-0.0.6/swiftly_windows/__init__.py
--rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-18 20:18:06.000000 swiftly-windows-0.0.6/swiftly_windows/config.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-18 20:18:06.000000 swiftly-windows-0.0.6/swiftly_windows/gitignore.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     3299 2023-07-18 20:18:06.000000 swiftly-windows-0.0.6/swiftly_windows/init.py
--rw-r--r--   0 brainspoof   (501) staff       (20)     2172 2023-07-18 20:18:06.000000 swiftly-windows-0.0.6/swiftly_windows/makeapp.py
--rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-18 20:18:06.000000 swiftly-windows-0.0.6/swiftly_windows/runapp.py
-drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:56:52.673523 swiftly-windows-0.0.6/swiftly_windows.egg-info/
--rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 20:56:52.000000 swiftly-windows-0.0.6/swiftly_windows.egg-info/PKG-INFO
--rw-r--r--   0 brainspoof   (501) staff       (20)      352 2023-07-18 20:56:52.000000 swiftly-windows-0.0.6/swiftly_windows.egg-info/SOURCES.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-18 20:56:52.000000 swiftly-windows-0.0.6/swiftly_windows.egg-info/dependency_links.txt
--rw-r--r--   0 brainspoof   (501) staff       (20)       16 2023-07-18 20:56:52.000000 swiftly-windows-0.0.6/swiftly_windows.egg-info/top_level.txt
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:00:47.736164 swiftly-windows-0.0.7/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     1500 2023-07-18 20:18:06.000000 swiftly-windows-0.0.7/LICENSE
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 21:00:47.735840 swiftly-windows-0.0.7/PKG-INFO
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:00:47.726544 swiftly-windows-0.0.7/scripts/
+-rw-r--r--   0 brainspoof   (501) staff       (20)     6132 2023-07-18 21:00:34.000000 swiftly-windows-0.0.7/scripts/swiftly.bat
+-rw-r--r--   0 brainspoof   (501) staff       (20)       38 2023-07-18 21:00:47.737577 swiftly-windows-0.0.7/setup.cfg
+-rw-r--r--   0 brainspoof   (501) staff       (20)      169 2023-07-18 21:00:45.000000 swiftly-windows-0.0.7/setup.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:00:47.727499 swiftly-windows-0.0.7/swiftly_windows/
+-rw-r--r--   0 brainspoof   (501) staff       (20)        0 2023-07-18 20:18:06.000000 swiftly-windows-0.0.7/swiftly_windows/__init__.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)       30 2023-07-18 20:18:06.000000 swiftly-windows-0.0.7/swiftly_windows/config.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3104 2023-07-18 20:18:06.000000 swiftly-windows-0.0.7/swiftly_windows/gitignore.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     3299 2023-07-18 20:18:06.000000 swiftly-windows-0.0.7/swiftly_windows/init.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)     2172 2023-07-18 20:18:06.000000 swiftly-windows-0.0.7/swiftly_windows/makeapp.py
+-rw-r--r--   0 brainspoof   (501) staff       (20)      177 2023-07-18 20:18:06.000000 swiftly-windows-0.0.7/swiftly_windows/runapp.py
+drwxr-xr-x   0 brainspoof   (501) staff       (20)        0 2023-07-18 21:00:47.730598 swiftly-windows-0.0.7/swiftly_windows.egg-info/
+-rw-r--r--   0 brainspoof   (501) staff       (20)       81 2023-07-18 21:00:47.000000 swiftly-windows-0.0.7/swiftly_windows.egg-info/PKG-INFO
+-rw-r--r--   0 brainspoof   (501) staff       (20)      352 2023-07-18 21:00:47.000000 swiftly-windows-0.0.7/swiftly_windows.egg-info/SOURCES.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)        1 2023-07-18 21:00:47.000000 swiftly-windows-0.0.7/swiftly_windows.egg-info/dependency_links.txt
+-rw-r--r--   0 brainspoof   (501) staff       (20)       16 2023-07-18 21:00:47.000000 swiftly-windows-0.0.7/swiftly_windows.egg-info/top_level.txt
```

### Comparing `swiftly-windows-0.0.6/LICENSE` & `swiftly-windows-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.6/scripts/swiftly.bat` & `swiftly-windows-0.0.7/scripts/swiftly.bat`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-@echo off
+@echo on
 REM Disable echo
 
 REM Check if the first argument is 'init', 'makeapp', 'run', 'install', 'uninstall', or 'push'
 IF NOT "%~1"=="init" IF NOT "%~1"=="makeapp" IF NOT "%~1"=="run" IF NOT "%~1"=="install" IF NOT "%~1"=="uninstall" IF NOT "%~1"=="push" (
     echo Invalid command.
     exit /b
 )
```

### Comparing `swiftly-windows-0.0.6/swiftly_windows/gitignore.py` & `swiftly-windows-0.0.7/swiftly_windows/gitignore.py`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.6/swiftly_windows/init.py` & `swiftly-windows-0.0.7/swiftly_windows/init.py`

 * *Files identical despite different names*

### Comparing `swiftly-windows-0.0.6/swiftly_windows/makeapp.py` & `swiftly-windows-0.0.7/swiftly_windows/makeapp.py`

 * *Files identical despite different names*

