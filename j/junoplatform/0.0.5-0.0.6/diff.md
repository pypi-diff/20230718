# Comparing `tmp/junoplatform-0.0.5.tar.gz` & `tmp/junoplatform-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junoplatform-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "junoplatform-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `junoplatform-0.0.5.tar` & `junoplatform-0.0.6.tar`

### file list

```diff
@@ -1,6 +1,23 @@
--rw-r--r--   0        0        0        0 2023-07-10 07:45:23.535265 junoplatform-0.0.5/README.md
--rw-r--r--   0        0        0      609 2023-07-10 08:44:22.805652 junoplatform-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.5/src/junoplatform/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 07:47:41.758337 junoplatform-0.0.5/src/junoplatform/io/__init__.py
--rw-r--r--   0        0        0       26 2023-07-10 07:59:43.895947 junoplatform-0.0.5/src/junoplatform/io/input.py
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 junoplatform-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       31 2023-07-12 03:20:16.720150 junoplatform-0.0.6/.gitignore
+-rw-r--r--   0        0        0        0 2023-07-10 07:45:23.535265 junoplatform-0.0.6/README.md
+-rw-r--r--   0        0        0      859 2023-07-18 03:26:45.512854 junoplatform-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 08:03:40.679259 junoplatform-0.0.6/src/junoplatform/__init__.py
+-rw-r--r--   0        0        0     1229 2023-07-17 07:58:35.111276 junoplatform-0.0.6/src/junoplatform/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-13 11:17:07.122874 junoplatform-0.0.6/src/junoplatform/io/_input/__init__.py
+-rw-r--r--   0        0        0      408 2023-07-14 01:45:21.929460 junoplatform-0.0.6/src/junoplatform/io/_input/clickhouse.py
+-rw-r--r--   0        0        0      237 2023-07-10 09:06:31.429958 junoplatform-0.0.6/src/junoplatform/io/_input/reader.py
+-rw-r--r--   0        0        0      816 2023-07-13 12:43:43.305443 junoplatform-0.0.6/src/junoplatform/io/_output/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 02:04:06.922936 junoplatform-0.0.6/src/junoplatform/meta/__init__.py
+-rw-r--r--   0        0        0     2142 2023-07-17 09:03:42.085651 junoplatform-0.0.6/src/junoplatform/meta/decorators.py
+-rw-r--r--   0        0        0      866 2023-07-17 09:07:03.410699 junoplatform-0.0.6/src/junoplatform/templates/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 08:39:47.775803 junoplatform-0.0.6/src/junoplatform/tools/__init__.py
+-rw-r--r--   0        0        0     3470 2023-07-18 03:18:44.190852 junoplatform-0.0.6/src/junoplatform/tools/cmd.py
+-rw-r--r--   0        0        0      163 2023-07-13 05:56:20.979580 junoplatform-0.0.6/tests/fputs.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-07-13 05:56:20.999580 junoplatform-0.0.6/tests/fputs.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2023-07-13 05:56:20.979580 junoplatform-0.0.6/tests/fputs.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        6 2023-07-13 05:56:20.979580 junoplatform-0.0.6/tests/fputs.egg-info/top_level.txt
+-rw-r--r--   0        0        0       76 2023-07-17 08:32:09.175206 junoplatform-0.0.6/tests/input.json
+-rw-r--r--   0        0        0      363 2023-07-13 05:55:54.568005 junoplatform-0.0.6/tests/setup.py
+-rw-r--r--   0        0        0      866 2023-07-17 09:02:41.334545 junoplatform-0.0.6/tests/test.py
+-rw-r--r--   0        0        0      782 2023-07-17 09:02:02.959111 junoplatform-0.0.6/tests/test_module.c
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 junoplatform-0.0.6/PKG-INFO
```

