# Comparing `tmp/kfpx-0.2.3.tar.gz` & `tmp/kfpx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfpx-0.2.3.tar", max compression
+gzip compressed data, was "kfpx-0.3.0.tar", max compression
```

## Comparing `kfpx-0.2.3.tar` & `kfpx-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1064 2022-05-31 04:06:19.563397 kfpx-0.2.3/LICENSE
--rw-r--r--   0        0        0       40 2022-06-14 07:54:25.417725 kfpx-0.2.3/kfpx/__init__.py
--rw-r--r--   0        0        0     2108 2022-09-08 08:53:17.783088 kfpx-0.2.3/kfpx/client.py
--rw-r--r--   0        0        0        0 2022-05-31 04:13:08.826978 kfpx-0.2.3/kfpx/compiler.py
--rw-r--r--   0        0        0      517 2023-05-10 09:05:22.373335 kfpx-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      593 1970-01-01 00:00:00.000000 kfpx-0.2.3/setup.py
--rw-r--r--   0        0        0      337 1970-01-01 00:00:00.000000 kfpx-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-05-31 04:06:19.563397 kfpx-0.3.0/LICENSE
+-rw-r--r--   0        0        0       40 2022-06-14 07:54:25.417725 kfpx-0.3.0/kfpx/__init__.py
+-rw-r--r--   0        0        0     2108 2022-09-08 08:53:17.783088 kfpx-0.3.0/kfpx/client.py
+-rw-r--r--   0        0        0        0 2022-05-31 04:13:08.826978 kfpx-0.3.0/kfpx/compiler.py
+-rw-r--r--   0        0        0      488 2023-07-18 12:28:58.576429 kfpx-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      339 1970-01-01 00:00:00.000000 kfpx-0.3.0/PKG-INFO
```

### Comparing `kfpx-0.2.3/LICENSE` & `kfpx-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kfpx-0.2.3/kfpx/client.py` & `kfpx-0.3.0/kfpx/client.py`

 * *Files identical despite different names*

