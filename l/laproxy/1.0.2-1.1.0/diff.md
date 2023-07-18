# Comparing `tmp/laproxy-1.0.2.tar.gz` & `tmp/laproxy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "laproxy-1.0.2.tar", max compression
+gzip compressed data, was "laproxy-1.1.0.tar", max compression
```

## Comparing `laproxy-1.0.2.tar` & `laproxy-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      406 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/__init__.py
--rw-r--r--   0        0        0     5086 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/_http.py
--rw-r--r--   0        0        0      501 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/_laproxy.py
--rw-r--r--   0        0        0     2898 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/_tcp.py
--rw-r--r--   0        0        0        0 2023-06-02 09:55:34.707128 laproxy-1.0.2/laproxy/py.typed
--rw-r--r--   0        0        0      485 2023-06-02 09:55:34.707128 laproxy-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 laproxy-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1461 2023-07-18 08:44:52.443900 laproxy-1.1.0/README.md
+-rw-r--r--   0        0        0     1914 2023-07-18 08:44:52.443900 laproxy-1.1.0/laproxy/__init__.py
+-rw-r--r--   0        0        0     8704 2023-07-18 08:44:52.443900 laproxy-1.1.0/laproxy/_http.py
+-rw-r--r--   0        0        0     1527 2023-07-18 08:44:52.443900 laproxy-1.1.0/laproxy/_laproxy.py
+-rw-r--r--   0        0        0     6581 2023-07-18 08:44:52.443900 laproxy-1.1.0/laproxy/_tcp.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:44:52.443900 laproxy-1.1.0/laproxy/py.typed
+-rw-r--r--   0        0        0     1105 2023-07-18 08:44:52.443900 laproxy-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2664 1970-01-01 00:00:00.000000 laproxy-1.1.0/PKG-INFO
```

