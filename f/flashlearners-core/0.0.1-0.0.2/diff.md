# Comparing `tmp/flashlearners_core-0.0.1.tar.gz` & `tmp/flashlearners_core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flashlearners_core-0.0.1.tar", last modified: Wed Jun 14 10:59:56 2023, max compression
+gzip compressed data, was "flashlearners_core-0.0.2.tar", last modified: Tue Jul 18 12:42:05 2023, max compression
```

## Comparing `flashlearners_core-0.0.1.tar` & `flashlearners_core-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-14 10:59:56.650338 flashlearners_core-0.0.1/
--rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 flashlearners_core-0.0.1/LICENSE
--rw-r--r--   0 macbookpro   (501) staff       (20)      447 2023-06-14 10:59:56.650131 flashlearners_core-0.0.1/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     6195 2023-06-02 12:38:27.000000 flashlearners_core-0.0.1/README.md
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-14 10:59:56.620698 flashlearners_core-0.0.1/flashlearners_core/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-06-02 12:40:26.000000 flashlearners_core-0.0.1/flashlearners_core/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-14 10:59:56.622963 flashlearners_core-0.0.1/flashlearners_core/app/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-05-31 22:47:47.000000 flashlearners_core-0.0.1/flashlearners_core/app/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1495 2023-06-12 18:40:33.000000 flashlearners_core-0.0.1/flashlearners_core/app/admin.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      122 2023-06-12 15:57:05.000000 flashlearners_core-0.0.1/flashlearners_core/app/apps.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-14 10:59:56.623516 flashlearners_core-0.0.1/flashlearners_core/app/migrations/
--rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-05-31 22:47:47.000000 flashlearners_core-0.0.1/flashlearners_core/app/migrations/__init__.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-14 10:59:56.649641 flashlearners_core-0.0.1/flashlearners_core/app/models/
--rw-r--r--   0 macbookpro   (501) staff       (20)      486 2023-06-12 16:16:55.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/__init__.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      505 2023-06-01 00:40:45.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/base.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      347 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/bookmark.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      265 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/faq.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      314 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/feedback.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/flashcard.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      738 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/guide.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      547 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/media.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      506 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/notification.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      661 2023-06-14 10:26:50.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/payment.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      443 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/performance.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      821 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/quiz.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      458 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/subject.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      553 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/subscription.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      354 2023-06-14 10:26:09.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/topic.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      626 2023-06-14 10:40:55.000000 flashlearners_core-0.0.1/flashlearners_core/app/models/user.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     1337 2023-06-01 20:50:00.000000 flashlearners_core-0.0.1/flashlearners_core/constants.py
--rw-r--r--   0 macbookpro   (501) staff       (20)     5127 2023-06-02 13:07:30.000000 flashlearners_core-0.0.1/flashlearners_core/settings.py
--rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 flashlearners_core-0.0.1/flashlearners_core/utils.py
-drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-06-14 10:59:56.622106 flashlearners_core-0.0.1/flashlearners_core.egg-info/
--rw-r--r--   0 macbookpro   (501) staff       (20)      447 2023-06-14 10:59:56.000000 flashlearners_core-0.0.1/flashlearners_core.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (501) staff       (20)     1172 2023-06-14 10:59:56.000000 flashlearners_core-0.0.1/flashlearners_core.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-06-14 10:59:56.000000 flashlearners_core-0.0.1/flashlearners_core.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)      128 2023-06-14 10:59:56.000000 flashlearners_core-0.0.1/flashlearners_core.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       19 2023-06-14 10:59:56.000000 flashlearners_core-0.0.1/flashlearners_core.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 flashlearners_core-0.0.1/pyproject.toml
--rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-06-14 10:59:56.650417 flashlearners_core-0.0.1/setup.cfg
--rw-r--r--   0 macbookpro   (501) staff       (20)     1161 2023-06-14 10:57:15.000000 flashlearners_core-0.0.1/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-18 12:42:05.066321 flashlearners_core-0.0.2/
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1073 2022-06-15 18:33:30.000000 flashlearners_core-0.0.2/LICENSE
+-rw-r--r--   0 macbookpro   (501) staff       (20)      447 2023-07-18 12:42:05.066145 flashlearners_core-0.0.2/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     6195 2023-06-02 12:38:27.000000 flashlearners_core-0.0.2/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-18 12:42:05.060701 flashlearners_core-0.0.2/flashlearners_core/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-06-02 12:40:26.000000 flashlearners_core-0.0.2/flashlearners_core/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-18 12:42:05.062020 flashlearners_core-0.0.2/flashlearners_core/app/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-05-31 22:47:47.000000 flashlearners_core-0.0.2/flashlearners_core/app/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1495 2023-06-12 18:40:33.000000 flashlearners_core-0.0.2/flashlearners_core/app/admin.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      122 2023-06-12 15:57:05.000000 flashlearners_core-0.0.2/flashlearners_core/app/apps.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-18 12:42:05.062289 flashlearners_core-0.0.2/flashlearners_core/app/migrations/
+-rw-r--r--   0 macbookpro   (501) staff       (20)        0 2023-05-31 22:47:47.000000 flashlearners_core-0.0.2/flashlearners_core/app/migrations/__init__.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-18 12:42:05.065850 flashlearners_core-0.0.2/flashlearners_core/app/models/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      486 2023-06-12 16:16:55.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      505 2023-06-01 00:40:45.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/base.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      347 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/bookmark.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      265 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/faq.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      314 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/feedback.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      373 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/flashcard.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      738 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/guide.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      547 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/media.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      506 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/notification.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      661 2023-06-14 10:26:50.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/payment.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      443 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/performance.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      821 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/quiz.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      458 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/subject.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      553 2023-06-14 10:26:09.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/subscription.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      432 2023-07-18 08:06:39.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/topic.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     3697 2023-07-18 12:41:13.000000 flashlearners_core-0.0.2/flashlearners_core/app/models/user.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1337 2023-06-01 20:50:00.000000 flashlearners_core-0.0.2/flashlearners_core/constants.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     5127 2023-06-02 13:07:30.000000 flashlearners_core-0.0.2/flashlearners_core/settings.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)      942 2023-04-30 10:17:16.000000 flashlearners_core-0.0.2/flashlearners_core/utils.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-07-18 12:42:05.061488 flashlearners_core-0.0.2/flashlearners_core.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)      447 2023-07-18 12:42:05.000000 flashlearners_core-0.0.2/flashlearners_core.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1172 2023-07-18 12:42:05.000000 flashlearners_core-0.0.2/flashlearners_core.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-07-18 12:42:05.000000 flashlearners_core-0.0.2/flashlearners_core.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      128 2023-07-18 12:42:05.000000 flashlearners_core-0.0.2/flashlearners_core.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       19 2023-07-18 12:42:05.000000 flashlearners_core-0.0.2/flashlearners_core.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       84 2022-06-15 18:10:36.000000 flashlearners_core-0.0.2/pyproject.toml
+-rw-r--r--   0 macbookpro   (501) staff       (20)       38 2023-07-18 12:42:05.066373 flashlearners_core-0.0.2/setup.cfg
+-rw-r--r--   0 macbookpro   (501) staff       (20)     1161 2023-07-18 12:41:30.000000 flashlearners_core-0.0.2/setup.py
```

### Comparing `flashlearners_core-0.0.1/LICENSE` & `flashlearners_core-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/README.md` & `flashlearners_core-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/app/admin.py` & `flashlearners_core-0.0.2/flashlearners_core/app/admin.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/app/models/guide.py` & `flashlearners_core-0.0.2/flashlearners_core/app/models/guide.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/app/models/media.py` & `flashlearners_core-0.0.2/flashlearners_core/app/models/media.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/app/models/payment.py` & `flashlearners_core-0.0.2/flashlearners_core/app/models/payment.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/app/models/quiz.py` & `flashlearners_core-0.0.2/flashlearners_core/app/models/quiz.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/app/models/subscription.py` & `flashlearners_core-0.0.2/flashlearners_core/app/models/subscription.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/constants.py` & `flashlearners_core-0.0.2/flashlearners_core/constants.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/settings.py` & `flashlearners_core-0.0.2/flashlearners_core/settings.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core/utils.py` & `flashlearners_core-0.0.2/flashlearners_core/utils.py`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/flashlearners_core.egg-info/SOURCES.txt` & `flashlearners_core-0.0.2/flashlearners_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flashlearners_core-0.0.1/setup.py` & `flashlearners_core-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'FlashLearners core package'
 LONG_DESCRIPTION = 'Package that holds all models and core functions/classes of FlashLearners project'
 
 # Setting up
 setup(
     # the name must match the folder name 'verysimplemodule'
     name="flashlearners_core",
```

