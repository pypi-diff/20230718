# Comparing `tmp/talkytimes_package-0.3.5.tar.gz` & `tmp/talkytimes_package-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.3.5.tar", last modified: Tue Jul 18 01:15:01 2023, max compression
+gzip compressed data, was "talkytimes_package-0.3.6.tar", last modified: Tue Jul 18 01:35:23 2023, max compression
```

## Comparing `talkytimes_package-0.3.5.tar` & `talkytimes_package-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.207677 talkytimes_package-0.3.5/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.5/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.5/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-18 01:15:01.207677 talkytimes_package-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.5/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.5/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-18 01:15:01.212676 talkytimes_package-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.184673 talkytimes_package-0.3.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.190673 talkytimes_package-0.3.5/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.5/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.5/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2040 2023-07-18 01:13:02.000000 talkytimes_package-0.3.5/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.193674 talkytimes_package-0.3.5/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-18 01:12:48.000000 talkytimes_package-0.3.5/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.5/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     4004 2023-07-18 01:11:05.000000 talkytimes_package-0.3.5/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:15:01.206676 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-18 01:15:01.000000 talkytimes_package-0.3.5/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 01:35:23.776806 talkytimes_package-0.3.6/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-18 01:35:23.776806 talkytimes_package-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.3.6/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.3.6/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-18 01:35:23.780806 talkytimes_package-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:35:23.748379 talkytimes_package-0.3.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 01:35:23.755263 talkytimes_package-0.3.6/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.3.6/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.3.6/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     1955 2023-07-18 01:34:40.000000 talkytimes_package-0.3.6/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:35:23.758264 talkytimes_package-0.3.6/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-18 01:35:21.000000 talkytimes_package-0.3.6/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.3.6/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     4004 2023-07-18 01:11:05.000000 talkytimes_package-0.3.6/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-18 01:35:23.775810 talkytimes_package-0.3.6/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-18 01:35:23.000000 talkytimes_package-0.3.6/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-18 01:35:23.000000 talkytimes_package-0.3.6/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 01:35:23.000000 talkytimes_package-0.3.6/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-18 01:35:23.000000 talkytimes_package-0.3.6/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 01:35:23.000000 talkytimes_package-0.3.6/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.3.5/LICENSE` & `talkytimes_package-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.5/src/dynamodb/dynamodb.py` & `talkytimes_package-0.3.6/src/dynamodb/dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,12 @@
                 ':user_info': {
                     'S': new_user_info,
                 },
             },
             Key={
                 'external_id': {
                     'S': external_id,
-                },
-                "user_info": {
-                    'S': user_info
                 }
             },
             ReturnValues='UPDATED_NEW',
             UpdateExpression='SET #UI = :user_info',
         )
```

### Comparing `talkytimes_package-0.3.5/src/talkytimes/base.py` & `talkytimes_package-0.3.6/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.3.5/src/talkytimes/talkytimes.py` & `talkytimes_package-0.3.6/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

