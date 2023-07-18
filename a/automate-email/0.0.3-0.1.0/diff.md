# Comparing `tmp/automate_email-0.0.3.tar.gz` & `tmp/automate_email-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/xavierh/automate_email/dist/.tmp-330o2suq/automate_email-0.0.3.tar", last modified: Tue Jul 18 02:36:29 2023, max compression
+gzip compressed data, was "/Users/xavierh/automate_email/dist/.tmp-nlrp7q6s/automate_email-0.1.0.tar", last modified: Tue Jul 18 02:38:43 2023, max compression
```

## Comparing `automate_email-0.0.3.tar` & `automate_email-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:36:29.623397 automate_email-0.0.3/
--rw-r--r--   0 xavierh    (501) staff       (20)     1070 2023-07-17 23:22:26.000000 automate_email-0.0.3/LICENSE
--rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 02:36:29.623553 automate_email-0.0.3/PKG-INFO
-drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:36:29.621151 automate_email-0.0.3/automate_email/
--rw-r--r--   0 xavierh    (501) staff       (20)     1360 2023-07-18 02:32:39.000000 automate_email-0.0.3/automate_email/__init__.py
-drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:36:29.623031 automate_email-0.0.3/automate_email.egg-info/
--rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 02:36:29.000000 automate_email-0.0.3/automate_email.egg-info/PKG-INFO
--rw-r--r--   0 xavierh    (501) staff       (20)      211 2023-07-18 02:36:29.000000 automate_email-0.0.3/automate_email.egg-info/SOURCES.txt
--rw-r--r--   0 xavierh    (501) staff       (20)        1 2023-07-18 02:36:29.000000 automate_email-0.0.3/automate_email.egg-info/dependency_links.txt
--rw-r--r--   0 xavierh    (501) staff       (20)       15 2023-07-18 02:36:29.000000 automate_email-0.0.3/automate_email.egg-info/top_level.txt
--rw-r--r--   0 xavierh    (501) staff       (20)       93 2023-07-18 00:39:07.000000 automate_email-0.0.3/pyproject.toml
--rw-r--r--   0 xavierh    (501) staff       (20)      454 2023-07-18 02:36:29.624201 automate_email-0.0.3/setup.cfg
+drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:38:43.097476 automate_email-0.1.0/
+-rw-r--r--   0 xavierh    (501) staff       (20)     1070 2023-07-17 23:22:26.000000 automate_email-0.1.0/LICENSE
+-rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 02:38:43.097607 automate_email-0.1.0/PKG-INFO
+drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:38:43.095162 automate_email-0.1.0/automate_email/
+-rw-r--r--   0 xavierh    (501) staff       (20)     1360 2023-07-18 02:32:39.000000 automate_email-0.1.0/automate_email/__init__.py
+drwxr-xr-x   0 xavierh    (501) staff       (20)        0 2023-07-18 02:38:43.097106 automate_email-0.1.0/automate_email.egg-info/
+-rw-r--r--   0 xavierh    (501) staff       (20)      387 2023-07-18 02:38:43.000000 automate_email-0.1.0/automate_email.egg-info/PKG-INFO
+-rw-r--r--   0 xavierh    (501) staff       (20)      211 2023-07-18 02:38:43.000000 automate_email-0.1.0/automate_email.egg-info/SOURCES.txt
+-rw-r--r--   0 xavierh    (501) staff       (20)        1 2023-07-18 02:38:43.000000 automate_email-0.1.0/automate_email.egg-info/dependency_links.txt
+-rw-r--r--   0 xavierh    (501) staff       (20)       15 2023-07-18 02:38:43.000000 automate_email-0.1.0/automate_email.egg-info/top_level.txt
+-rw-r--r--   0 xavierh    (501) staff       (20)       93 2023-07-18 00:39:07.000000 automate_email-0.1.0/pyproject.toml
+-rw-r--r--   0 xavierh    (501) staff       (20)      454 2023-07-18 02:38:43.098132 automate_email-0.1.0/setup.cfg
```

### Comparing `automate_email-0.0.3/LICENSE` & `automate_email-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `automate_email-0.0.3/automate_email/__init__.py` & `automate_email-0.1.0/automate_email/__init__.py`

 * *Files identical despite different names*

