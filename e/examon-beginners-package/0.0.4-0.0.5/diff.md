# Comparing `tmp/examon_beginners_package-0.0.4.tar.gz` & `tmp/examon_beginners_package-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_beginners_package-0.0.4.tar", max compression
+gzip compressed data, was "examon_beginners_package-0.0.5.tar", max compression
```

## Comparing `examon_beginners_package-0.0.4.tar` & `examon_beginners_package-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.0.4/examon_beginners_package/__init__.py
--rw-r--r--   0        0        0     1082 2023-07-16 21:28:12.657199 examon_beginners_package-0.0.4/examon_beginners_package/beginners.py
--rw-r--r--   0        0        0      338 2023-07-17 15:53:44.205408 examon_beginners_package-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 examon_beginners_package-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.0.5/examon_beginners_package/__init__.py
+-rw-r--r--   0        0        0      548 2023-07-18 14:37:44.540369 examon_beginners_package-0.0.5/examon_beginners_package/beginners.py
+-rw-r--r--   0        0        0      338 2023-07-18 14:31:44.760096 examon_beginners_package-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 examon_beginners_package-0.0.5/PKG-INFO
```

