# Comparing `tmp/XStatic-Angular-lrdragndrop-1.0.2.4.tar.gz` & `tmp/XStatic-Angular-lrdragndrop-1.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/XStatic-Angular-lrdragndrop-1.0.2.4.tar", last modified: Thu Feb 14 06:34:03 2019, max compression
+gzip compressed data, was "XStatic-Angular-lrdragndrop-1.0.2.5.tar", last modified: Tue Jul 18 12:36:47 2023, max compression
```

## Comparing `XStatic-Angular-lrdragndrop-1.0.2.4.tar` & `XStatic-Angular-lrdragndrop-1.0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      157 2019-02-14 06:31:39.000000 XStatic-Angular-lrdragndrop-1.0.2.4/MANIFEST.in
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      755 2019-02-14 06:31:39.000000 XStatic-Angular-lrdragndrop-1.0.2.4/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/namespace_packages.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/angular_lrdragndrop/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-02-14 06:34:03.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/angular_lrdragndrop/data/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6797 2019-02-14 06:31:39.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/angular_lrdragndrop/data/lrdragndrop.js
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1969 2019-02-14 06:31:39.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/angular_lrdragndrop/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       56 2019-02-14 06:31:39.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       56 2019-02-14 06:31:39.000000 XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      489 2019-02-14 06:31:39.000000 XStatic-Angular-lrdragndrop-1.0.2.4/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-18 12:36:47.431283 XStatic-Angular-lrdragndrop-1.0.2.5/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-07-18 12:36:25.000000 XStatic-Angular-lrdragndrop-1.0.2.5/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2023-07-18 12:36:47.431283 XStatic-Angular-lrdragndrop-1.0.2.5/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2023-07-18 12:36:25.000000 XStatic-Angular-lrdragndrop-1.0.2.5/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-18 12:36:47.427283 XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2023-07-18 12:36:47.000000 XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-07-18 12:36:47.000000 XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-18 12:36:47.000000 XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       20 2023-07-18 12:36:47.000000 XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-18 12:36:47.000000 XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2023-07-18 12:36:47.000000 XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       38 2023-07-18 12:36:47.431283 XStatic-Angular-lrdragndrop-1.0.2.5/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2023-07-18 12:36:25.000000 XStatic-Angular-lrdragndrop-1.0.2.5/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-18 12:36:47.431283 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-07-18 12:36:25.000000 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-18 12:36:47.431283 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2023-07-18 12:36:25.000000 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-18 12:36:47.431283 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/angular_lrdragndrop/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1969 2023-07-18 12:36:25.000000 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/angular_lrdragndrop/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-18 12:36:47.431283 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/angular_lrdragndrop/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7396 2023-07-18 12:36:25.000000 XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/angular_lrdragndrop/data/lrdragndrop.js
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `XStatic-Angular-lrdragndrop-1.0.2.4/setup.py` & `XStatic-Angular-lrdragndrop-1.0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `XStatic-Angular-lrdragndrop-1.0.2.4/XStatic_Angular_lrdragndrop.egg-info/PKG-INFO` & `XStatic-Angular-lrdragndrop-1.0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: XStatic-Angular-lrdragndrop
-Version: 1.0.2.4
+Version: 1.0.2.5
 Summary: Angular-lrdragndrop 1.0.2 (XStatic packaging standard)
 Home-page: https://github.com/lorenzofox3/lrDragNDrop
 Maintainer: Thai Tran
 Maintainer-email: tqtran@us.ibm.com
 License: MIT
 Description: XStatic-Angular-lrdragndrop
         ---------------------------
```

### Comparing `XStatic-Angular-lrdragndrop-1.0.2.4/PKG-INFO` & `XStatic-Angular-lrdragndrop-1.0.2.5/XStatic_Angular_lrdragndrop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: XStatic-Angular-lrdragndrop
-Version: 1.0.2.4
+Version: 1.0.2.5
 Summary: Angular-lrdragndrop 1.0.2 (XStatic packaging standard)
 Home-page: https://github.com/lorenzofox3/lrDragNDrop
 Maintainer: Thai Tran
 Maintainer-email: tqtran@us.ibm.com
 License: MIT
 Description: XStatic-Angular-lrdragndrop
         ---------------------------
```

### Comparing `XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/angular_lrdragndrop/data/lrdragndrop.js` & `XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/angular_lrdragndrop/data/lrdragndrop.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,27 @@
 (function(ng) {
     'use strict';
 
     function isJqueryEventDataTransfer() {
-        return window.jQuery && (-1 == window.jQuery.event.props.indexOf('dataTransfer'));
+        return window.jQuery && (!window.jQuery.event.special.dataTransfer ||
+            !window.jQuery.event.special.dataTransfer.props || -1 ===
+            window.jQuery.event.special.dataTransfer.props.indexOf('dataTransfer'));
+        /
     }
 
     if (isJqueryEventDataTransfer()) {
-        window.jQuery.event.props.push('dataTransfer');
+        if (!window.jQuery.event.special.dataTransfer) {
+            window.jQuery.event.special.dataTransfer = {
+                props: ['dataTransfer']
+            };
+        } else if (!window.jQuery.event.special.dataTransfer.props) {
+            window.jQuery.event.special.dataTransfer.props = ['dataTransfer'];
+        } else if (-1 === window.jQuery.event.special.dataTransfer.props.indexOf('dataTransfer')) {
+            window.jQuery.event.special.dataTransfer.props.push('dataTransfer');
+        }
     }
 
     var module = ng.module('lrDragNDrop', []);
 
     module.service('lrDragStore', ['$document', function(document) {
 
         var store = {};
```

### Comparing `XStatic-Angular-lrdragndrop-1.0.2.4/xstatic/pkg/angular_lrdragndrop/__init__.py` & `XStatic-Angular-lrdragndrop-1.0.2.5/xstatic/pkg/angular_lrdragndrop/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 NAME = __name__.split('.')[-1] # package name (e.g. 'foo' or 'foo_bar')
                                # please use a all-lowercase valid python
                                # package name
 
 VERSION = '1.0.2' # version of the packaged files, please use the upstream
                   # version number
-BUILD = '4' # our package build number, so we can release new builds
+BUILD = '5' # our package build number, so we can release new builds
              # with fixes for xstatic stuff.
 PACKAGE_VERSION = VERSION + '.' + BUILD # version used for PyPi
 
 DESCRIPTION = "%s %s (XStatic packaging standard)" % (DISPLAY_NAME, VERSION)
 
 PLATFORMS = 'any'
 CLASSIFIERS = []
```

