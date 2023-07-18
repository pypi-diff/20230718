# Comparing `tmp/advert_cafe-0.0.1.tar.gz` & `tmp/advert_cafe-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "advert_cafe-0.0.1.tar", max compression
+gzip compressed data, was "advert_cafe-0.1.0.tar", max compression
```

## Comparing `advert_cafe-0.0.1.tar` & `advert_cafe-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      287 2023-07-18 20:53:00.020245 advert_cafe-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-18 20:44:29.794617 advert_cafe-0.0.1/advert_cafe/__init__.py
--rw-r--r--   0        0        0     1712 2023-07-18 20:47:23.357219 advert_cafe-0.0.1/advert_cafe/main.py
--rw-r--r--   0        0        0      372 2023-07-18 20:53:48.773831 advert_cafe-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 advert_cafe-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 21:06:17.652569 advert_cafe-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 21:06:17.652569 advert_cafe-0.1.0/advert_cafe/__init__.py
+-rw-r--r--   0        0        0     1713 2023-07-18 20:54:18.195501 advert_cafe-0.1.0/advert_cafe/main.py
+-rw-r--r--   0        0        0      335 2023-07-18 21:09:47.143908 advert_cafe-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      388 1970-01-01 00:00:00.000000 advert_cafe-0.1.0/PKG-INFO
```

### Comparing `advert_cafe-0.0.1/advert_cafe/main.py` & `advert_cafe-0.1.0/advert_cafe/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import netifaces as nif
 import logging
 import uuid
 import copy
 import json
+
 logger = logging.getLogger("advertcafe")
 
 
 def mac_for_ip(ip):
     "Returns a list of MACs for interfaces that have given IP, returns None if not found"
     for i in nif.interfaces():
         addrs = nif.ifaddresses(i)
```

