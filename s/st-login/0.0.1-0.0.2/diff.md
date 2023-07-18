# Comparing `tmp/st_login-0.0.1.tar.gz` & `tmp/st_login-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_login-0.0.1.tar", last modified: Mon Jul 17 07:18:37 2023, max compression
+gzip compressed data, was "st_login-0.0.2.tar", last modified: Tue Jul 18 08:59:45 2023, max compression
```

## Comparing `st_login-0.0.1.tar` & `st_login-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.580529 st_login-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-07-17 06:41:41.000000 st_login-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6211 2023-07-17 07:18:37.580529 st_login-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5600 2023-07-17 07:15:36.000000 st_login-0.0.1/README.md
--rw-rw-rw-   0        0        0      906 2023-07-17 07:18:37.583530 st_login-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       79 2023-07-17 06:39:35.000000 st_login-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.536546 st_login-0.0.1/st_login/
--rw-rw-rw-   0        0        0       36 2023-07-17 07:06:31.000000 st_login-0.0.1/st_login/__init__.py
--rw-rw-rw-   0        0        0     6963 2023-07-17 06:41:41.000000 st_login-0.0.1/st_login/utils.py
--rw-rw-rw-   0        0        0    13979 2023-07-17 07:06:23.000000 st_login-0.0.1/st_login/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.572533 st_login-0.0.1/st_login.egg-info/
--rw-rw-rw-   0        0        0     6211 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 07:18:37.000000 st_login-0.0.1/st_login.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-07-17 07:18:37.576617 st_login-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-17 06:41:41.000000 st_login-0.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:59:45.495564 st_login-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-07-17 06:41:41.000000 st_login-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     6211 2023-07-18 08:59:45.496564 st_login-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5600 2023-07-17 07:15:36.000000 st_login-0.0.2/README.md
+-rw-rw-rw-   0        0        0      919 2023-07-18 08:59:45.499569 st_login-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       79 2023-07-17 06:39:35.000000 st_login-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:59:45.436564 st_login-0.0.2/st_login/
+-rw-rw-rw-   0        0        0       36 2023-07-17 07:06:31.000000 st_login-0.0.2/st_login/__init__.py
+-rw-rw-rw-   0        0        0     6963 2023-07-17 06:41:41.000000 st_login-0.0.2/st_login/utils.py
+-rw-rw-rw-   0        0        0    13979 2023-07-17 07:06:23.000000 st_login-0.0.2/st_login/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-18 08:59:45.485564 st_login-0.0.2/st_login.egg-info/
+-rw-rw-rw-   0        0        0     6211 2023-07-18 08:59:45.000000 st_login-0.0.2/st_login.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-07-18 08:59:45.000000 st_login-0.0.2/st_login.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 08:59:45.000000 st_login-0.0.2/st_login.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-07-18 08:59:45.000000 st_login-0.0.2/st_login.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-18 08:59:45.000000 st_login-0.0.2/st_login.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 07:18:37.000000 st_login-0.0.2/st_login.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-07-18 08:59:45.491564 st_login-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 06:41:41.000000 st_login-0.0.2/tests/__init__.py
```

### Comparing `st_login-0.0.1/LICENSE` & `st_login-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_login-0.0.1/PKG-INFO` & `st_login-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_login
-Version: 0.0.1
+Version: 0.0.2
 Summary: The st_login library is meant for streamlit application developers. It lets you connect your streamlit application to a pre-built and secure Login/ Sign-Up page
 Home-page: https://github.com/lijiacaigit/st_login
 Author: Lijiacai
 Author-email: 1050518702@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `st_login-0.0.1/README.md` & `st_login-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `st_login-0.0.1/setup.cfg` & `st_login-0.0.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 745f 6c6f 6769 6e0d 0a76 6572   = st_login..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e31 0d0a 6465  sion = 0.0.1..de
+00000020: 7369 6f6e 203d 2030 2e30 2e32 0d0a 6465  sion = 0.0.2..de
 00000030: 7363 7269 7074 696f 6e20 3d20 5468 6520  scription = The 
 00000040: 7374 5f6c 6f67 696e 206c 6962 7261 7279  st_login library
 00000050: 2069 7320 6d65 616e 7420 666f 7220 7374   is meant for st
 00000060: 7265 616d 6c69 7420 6170 706c 6963 6174  reamlit applicat
 00000070: 696f 6e20 6465 7665 6c6f 7065 7273 2e20  ion developers. 
 00000080: 4974 206c 6574 7320 796f 7520 636f 6e6e  It lets you conn
 00000090: 6563 7420 796f 7572 2073 7472 6561 6d6c  ect your streaml
@@ -44,14 +44,15 @@
 000002b0: 6172 676f 6e32 2d63 6666 690d 0a09 6172  argon2-cffi...ar
 000002c0: 676f 6e32 2d63 6666 692d 6269 6e64 696e  gon2-cffi-bindin
 000002d0: 6773 0d0a 0973 7472 6561 6d6c 6974 0d0a  gs...streamlit..
 000002e0: 0973 7472 6561 6d6c 6974 2d63 6f6f 6b69  .streamlit-cooki
 000002f0: 6573 2d6d 616e 6167 6572 0d0a 0973 7472  es-manager...str
 00000300: 6561 6d6c 6974 2d6c 6f74 7469 650d 0a09  eamlit-lottie...
 00000310: 7374 7265 616d 6c69 742d 6f70 7469 6f6e  streamlit-option
-00000320: 2d6d 656e 750d 0a0d 0a5b 6f70 7469 6f6e  -menu....[option
-00000330: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000340: 0d0a 6578 636c 7564 6520 3d20 0d0a 0974  ..exclude = ...t
-00000350: 6573 740d 0a09 7465 7374 2e2a 0d0a 0d0a  est...test.*....
-00000360: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000370: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000380: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000320: 2d6d 656e 750d 0a09 7472 7963 6f75 7269  -menu...trycouri
+00000330: 6572 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  er....[options.p
+00000340: 6163 6b61 6765 732e 6669 6e64 5d0d 0a65  ackages.find]..e
+00000350: 7863 6c75 6465 203d 200d 0a09 7465 7374  xclude = ...test
+00000360: 0d0a 0974 6573 742e 2a0d 0a0d 0a5b 6567  ...test.*....[eg
+00000370: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000380: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000390: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `st_login-0.0.1/st_login/utils.py` & `st_login-0.0.2/st_login/utils.py`

 * *Files identical despite different names*

### Comparing `st_login-0.0.1/st_login/widgets.py` & `st_login-0.0.2/st_login/widgets.py`

 * *Files identical despite different names*

### Comparing `st_login-0.0.1/st_login.egg-info/PKG-INFO` & `st_login-0.0.2/st_login.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-login
-Version: 0.0.1
+Version: 0.0.2
 Summary: The st_login library is meant for streamlit application developers. It lets you connect your streamlit application to a pre-built and secure Login/ Sign-Up page
 Home-page: https://github.com/lijiacaigit/st_login
 Author: Lijiacai
 Author-email: 1050518702@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

