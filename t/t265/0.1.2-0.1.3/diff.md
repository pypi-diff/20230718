# Comparing `tmp/t265-0.1.2.tar.gz` & `tmp/t265-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t265-0.1.2.tar", last modified: Wed Jul  5 17:53:46 2023, max compression
+gzip compressed data, was "t265-0.1.3.tar", last modified: Tue Jul 18 01:32:23 2023, max compression
```

## Comparing `t265-0.1.2.tar` & `t265-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 17:53:46.695465 t265-0.1.2/
--rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 t265-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      563 2023-07-05 17:53:46.694462 t265-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-07-05 00:15:37.000000 t265-0.1.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 17:53:46.695465 t265-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-07-05 07:51:14.000000 t265-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 17:53:46.689960 t265-0.1.2/t265/
--rw-rw-rw-   0        0        0     2528 2023-07-05 01:41:09.000000 t265-0.1.2/t265/Tracking.py
--rw-rw-rw-   0        0        0       32 2023-07-05 01:41:09.000000 t265-0.1.2/t265/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 17:53:46.694462 t265-0.1.2/t265.egg-info/
--rw-rw-rw-   0        0        0      563 2023-07-05 17:53:46.000000 t265-0.1.2/t265.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-05 17:53:46.000000 t265-0.1.2/t265.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 17:53:46.000000 t265-0.1.2/t265.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-05 17:53:46.000000 t265-0.1.2/t265.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-05 17:53:46.000000 t265-0.1.2/t265.egg-info/top_level.txt
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-18 01:32:23.037089 t265-0.1.3/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       25 2023-07-18 00:54:55.000000 t265-0.1.3/MANIFEST.in
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-18 01:32:23.037089 t265-0.1.3/PKG-INFO
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:21:38.000000 t265-0.1.3/requirements.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       38 2023-07-18 01:32:23.037089 t265-0.1.3/setup.cfg
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     1008 2023-07-18 01:29:33.000000 t265-0.1.3/setup.py
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-18 01:32:23.037089 t265-0.1.3/t265/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     2560 2023-07-18 01:17:25.000000 t265-0.1.3/t265/Tracking.py
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       31 2023-07-18 00:54:55.000000 t265-0.1.3/t265/__init__.py
+drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-18 01:32:23.037089 t265-0.1.3/t265.egg-info/
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/PKG-INFO
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      210 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/SOURCES.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        1 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/dependency_links.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/requires.txt
+-rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        5 2023-07-18 01:32:23.000000 t265-0.1.3/t265.egg-info/top_level.txt
```

### Comparing `t265-0.1.2/PKG-INFO` & `t265-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: t265
-Version: 0.1.2
-Summary: t265 Tracking camera API wrapper
-Author: Yusuke Tanaka
-License: LGPLv3
-Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Robot Framework
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1
+Name: t265
+Version: 0.1.3
+Summary: t265 Tracking camera API wrapper
+Author: Yusuke Tanaka
+License: LGPLv3
+Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Robot Framework
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
```

### Comparing `t265-0.1.2/t265.egg-info/PKG-INFO` & `t265-0.1.3/t265.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: t265
-Version: 0.1.2
-Summary: t265 Tracking camera API wrapper
-Author: Yusuke Tanaka
-License: LGPLv3
-Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Robot Framework
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1
+Name: t265
+Version: 0.1.3
+Summary: t265 Tracking camera API wrapper
+Author: Yusuke Tanaka
+License: LGPLv3
+Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Robot Framework
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
```

