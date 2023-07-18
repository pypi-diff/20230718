# Comparing `tmp/zipline.py-0.6.1.tar.gz` & `tmp/zipline.py-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zipline.py-0.6.1.tar", last modified: Sun Apr  2 05:38:08 2023, max compression
+gzip compressed data, was "zipline.py-0.7.0.tar", last modified: Tue Jul 18 18:13:23 2023, max compression
```

## Comparing `zipline.py-0.6.1.tar` & `zipline.py-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-04-02 05:38:08.441025 zipline.py-0.6.1/
--rw-r--r--   0 rdrescher   (501) staff       (20)     1046 2023-03-27 21:55:25.000000 zipline.py-0.6.1/LICENSE
--rw-r--r--   0 rdrescher   (501) staff       (20)     2012 2023-04-02 05:38:08.440846 zipline.py-0.6.1/PKG-INFO
--rw-r--r--   0 rdrescher   (501) staff       (20)      319 2023-03-29 21:28:07.000000 zipline.py-0.6.1/README.md
--rw-r--r--   0 rdrescher   (501) staff       (20)      884 2023-04-02 05:37:51.000000 zipline.py-0.6.1/pyproject.toml
--rw-r--r--   0 rdrescher   (501) staff       (20)       38 2023-04-02 05:38:08.441070 zipline.py-0.6.1/setup.cfg
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-04-02 05:38:08.439624 zipline.py-0.6.1/zipline/
--rw-r--r--   0 rdrescher   (501) staff       (20)     1274 2023-04-02 05:37:44.000000 zipline.py-0.6.1/zipline/__init__.py
--rw-r--r--   0 rdrescher   (501) staff       (20)    22933 2023-04-01 00:45:04.000000 zipline.py-0.6.1/zipline/client.py
--rw-r--r--   0 rdrescher   (501) staff       (20)     1261 2023-04-01 00:12:46.000000 zipline.py-0.6.1/zipline/enums.py
--rw-r--r--   0 rdrescher   (501) staff       (20)     1851 2023-04-01 00:12:32.000000 zipline.py-0.6.1/zipline/errors.py
--rw-r--r--   0 rdrescher   (501) staff       (20)    15314 2023-04-02 05:37:15.000000 zipline.py-0.6.1/zipline/models.py
-drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-04-02 05:38:08.440583 zipline.py-0.6.1/zipline.py.egg-info/
--rw-r--r--   0 rdrescher   (501) staff       (20)     2012 2023-04-02 05:38:08.000000 zipline.py-0.6.1/zipline.py.egg-info/PKG-INFO
--rw-r--r--   0 rdrescher   (501) staff       (20)      292 2023-04-02 05:38:08.000000 zipline.py-0.6.1/zipline.py.egg-info/SOURCES.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)        1 2023-04-02 05:38:08.000000 zipline.py-0.6.1/zipline.py.egg-info/dependency_links.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)       55 2023-04-02 05:38:08.000000 zipline.py-0.6.1/zipline.py.egg-info/requires.txt
--rw-r--r--   0 rdrescher   (501) staff       (20)        8 2023-04-02 05:38:08.000000 zipline.py-0.6.1/zipline.py.egg-info/top_level.txt
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-18 18:13:23.624610 zipline.py-0.7.0/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1046 2023-03-27 21:55:25.000000 zipline.py-0.7.0/LICENSE
+-rw-r--r--   0 rdrescher   (501) staff       (20)     2012 2023-07-18 18:13:23.624488 zipline.py-0.7.0/PKG-INFO
+-rw-r--r--   0 rdrescher   (501) staff       (20)      319 2023-03-29 21:28:07.000000 zipline.py-0.7.0/README.md
+-rw-r--r--   0 rdrescher   (501) staff       (20)      884 2023-07-18 18:13:05.000000 zipline.py-0.7.0/pyproject.toml
+-rw-r--r--   0 rdrescher   (501) staff       (20)       38 2023-07-18 18:13:23.624642 zipline.py-0.7.0/setup.cfg
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-18 18:13:23.623711 zipline.py-0.7.0/zipline/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1274 2023-07-18 18:13:01.000000 zipline.py-0.7.0/zipline/__init__.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)    22944 2023-07-18 18:11:47.000000 zipline.py-0.7.0/zipline/client.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1261 2023-07-18 18:11:05.000000 zipline.py-0.7.0/zipline/enums.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)     1851 2023-07-18 18:11:05.000000 zipline.py-0.7.0/zipline/errors.py
+-rw-r--r--   0 rdrescher   (501) staff       (20)    15314 2023-07-18 18:11:05.000000 zipline.py-0.7.0/zipline/models.py
+drwxr-xr-x   0 rdrescher   (501) staff       (20)        0 2023-07-18 18:13:23.624303 zipline.py-0.7.0/zipline.py.egg-info/
+-rw-r--r--   0 rdrescher   (501) staff       (20)     2012 2023-07-18 18:13:23.000000 zipline.py-0.7.0/zipline.py.egg-info/PKG-INFO
+-rw-r--r--   0 rdrescher   (501) staff       (20)      292 2023-07-18 18:13:23.000000 zipline.py-0.7.0/zipline.py.egg-info/SOURCES.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)        1 2023-07-18 18:13:23.000000 zipline.py-0.7.0/zipline.py.egg-info/dependency_links.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)       55 2023-07-18 18:13:23.000000 zipline.py-0.7.0/zipline.py.egg-info/requires.txt
+-rw-r--r--   0 rdrescher   (501) staff       (20)        8 2023-07-18 18:13:23.000000 zipline.py-0.7.0/zipline.py.egg-info/top_level.txt
```

### Comparing `zipline.py-0.6.1/LICENSE` & `zipline.py-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zipline.py-0.6.1/PKG-INFO` & `zipline.py-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline.py
-Version: 0.6.1
+Version: 0.7.0
 Summary: An async wrapper for the Zipline api.
 Author-email: fretgfr <fretgfr@sudomail.com>
 License: Copyright 2023 fretgfr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `zipline.py-0.6.1/pyproject.toml` & `zipline.py-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zipline.py"
-version = "0.6.1"
+version = "0.7.0"
 description = "An async wrapper for the Zipline api."
 readme = "README.md"
 authors = [{ name = "fretgfr", email = "fretgfr@sudomail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `zipline.py-0.6.1/zipline/__init__.py` & `zipline.py-0.7.0/zipline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 from .errors import *
 from .models import *
 
 __title__ = "zipline.py"
 __author__ = "fretgfr"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 fretgfr"
-__version__ = "0.6.1"
+__version__ = "0.7.0"
```

### Comparing `zipline.py-0.6.1/zipline/client.py` & `zipline.py-0.7.0/zipline/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         """Creates user invites.
 
         Parameters
         ----------
         count : int, optional
             The number of invites to create, by default 1
         expires_at : Optional[datetime], optional
-            When the creates invite(s) should expire, by default None
+            When the created invite(s) should expire, by default None
 
         Returns
         -------
         List[PartialInvite]
             The created invites.
 
         Raises
@@ -181,20 +181,20 @@
         ZiplineError
             The server returned the invites in an unexpected format.
         BadRequest
             The server could not process the request.
         Forbidden
             You are not an administrator and cannot use this method.
         """
-        data = {"count": count, "expiresAt": expires_at.isoformat() if expires_at is not None else None}
+        data = {"count": count, "expiresAt": f"date={expires_at.isoformat()}" if expires_at is not None else None}
         async with self._session.post("/api/auth/invite", json=data) as resp:
             status = resp.status
             if status == 200:
                 js = await resp.json()
-                # Endpoint cant return a list of invites or just a single one if you only request one
+                # Endpoint can't return a list of invites or just a single one if you only request one
                 # Endpoint *should* return a full Invite, however it only returns three fields currently,
                 # hence the PartialInvite return type.
                 if isinstance(js, list):
                     return [PartialInvite._from_data(data) for data in js]
 
                 elif isinstance(js, dict):
                     return [PartialInvite._from_data(js)]
```

### Comparing `zipline.py-0.6.1/zipline/enums.py` & `zipline.py-0.7.0/zipline/enums.py`

 * *Files identical despite different names*

### Comparing `zipline.py-0.6.1/zipline/errors.py` & `zipline.py-0.7.0/zipline/errors.py`

 * *Files identical despite different names*

### Comparing `zipline.py-0.6.1/zipline/models.py` & `zipline.py-0.7.0/zipline/models.py`

 * *Files identical despite different names*

### Comparing `zipline.py-0.6.1/zipline.py.egg-info/PKG-INFO` & `zipline.py-0.7.0/zipline.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline.py
-Version: 0.6.1
+Version: 0.7.0
 Summary: An async wrapper for the Zipline api.
 Author-email: fretgfr <fretgfr@sudomail.com>
 License: Copyright 2023 fretgfr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

