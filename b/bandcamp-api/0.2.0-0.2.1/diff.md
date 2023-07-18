# Comparing `tmp/bandcamp_api-0.2.0.tar.gz` & `tmp/bandcamp_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bandcamp_api-0.2.0.tar", last modified: Tue Jul 18 19:07:04 2023, max compression
+gzip compressed data, was "bandcamp_api-0.2.1.tar", last modified: Tue Jul 18 19:34:55 2023, max compression
```

## Comparing `bandcamp_api-0.2.0.tar` & `bandcamp_api-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:07:04.022663 bandcamp_api-0.2.0/
--rwxr-xr-x   0 rin        (501) staff       (20)    35149 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/LICENSE
--rw-r--r--   0 rin        (501) staff       (20)      218 2023-07-18 19:07:04.022485 bandcamp_api-0.2.0/PKG-INFO
--rwxr-xr-x   0 rin        (501) staff       (20)      678 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/README.md
-drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:07:04.021474 bandcamp_api-0.2.0/bandcamp_api/
--rwxr-xr-x   0 rin        (501) staff       (20)       34 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/bandcamp_api/__init__.py
--rw-r--r--   0 rin        (501) staff       (20)     9181 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/album.py
--rw-r--r--   0 rin        (501) staff       (20)     1363 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/artist.py
--rw-r--r--   0 rin        (501) staff       (20)     7118 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/bandcamp_api.py
--rwxr-xr-x   0 rin        (501) staff       (20)     1615 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/bandcamp_api/bandcampjson.py
--rwxr-xr-x   0 rin        (501) staff       (20)    10654 2023-05-26 17:47:35.000000 bandcamp_api-0.2.0/bandcamp_api/daily.py
--rwxr-xr-x   0 rin        (501) staff       (20)     1846 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/genres.py
--rwxr-xr-x   0 rin        (501) staff       (20)    14004 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/homepage.py
--rwxr-xr-x   0 rin        (501) staff       (20)     2618 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/label.py
--rw-r--r--   0 rin        (501) staff       (20)     6226 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/search.py
--rwxr-xr-x   0 rin        (501) staff       (20)     5540 2023-07-18 18:48:37.000000 bandcamp_api-0.2.0/bandcamp_api/track.py
-drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:07:04.022274 bandcamp_api-0.2.0/bandcamp_api.egg-info/
--rw-r--r--   0 rin        (501) staff       (20)      218 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/PKG-INFO
--rw-r--r--   0 rin        (501) staff       (20)      505 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/SOURCES.txt
--rw-r--r--   0 rin        (501) staff       (20)        1 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/dependency_links.txt
--rw-r--r--   0 rin        (501) staff       (20)        1 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/not-zip-safe
--rw-r--r--   0 rin        (501) staff       (20)       58 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/requires.txt
--rw-r--r--   0 rin        (501) staff       (20)       13 2023-07-18 19:07:03.000000 bandcamp_api-0.2.0/bandcamp_api.egg-info/top_level.txt
--rw-r--r--   0 rin        (501) staff       (20)       38 2023-07-18 19:07:04.022704 bandcamp_api-0.2.0/setup.cfg
--rwxr-xr-x   0 rin        (501) staff       (20)      401 2023-07-18 19:06:41.000000 bandcamp_api-0.2.0/setup.py
+drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:34:55.675122 bandcamp_api-0.2.1/
+-rwxr-xr-x   0 rin        (501) staff       (20)    35149 2023-05-26 17:47:35.000000 bandcamp_api-0.2.1/LICENSE
+-rw-r--r--   0 rin        (501) staff       (20)      218 2023-07-18 19:34:55.674997 bandcamp_api-0.2.1/PKG-INFO
+-rwxr-xr-x   0 rin        (501) staff       (20)      680 2023-07-18 19:16:56.000000 bandcamp_api-0.2.1/README.md
+drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:34:55.673784 bandcamp_api-0.2.1/bandcamp_api/
+-rwxr-xr-x   0 rin        (501) staff       (20)       34 2023-05-26 17:47:35.000000 bandcamp_api-0.2.1/bandcamp_api/__init__.py
+-rw-r--r--   0 rin        (501) staff       (20)     9181 2023-07-18 18:48:37.000000 bandcamp_api-0.2.1/bandcamp_api/album.py
+-rw-r--r--   0 rin        (501) staff       (20)     1363 2023-07-18 18:48:37.000000 bandcamp_api-0.2.1/bandcamp_api/artist.py
+-rw-r--r--   0 rin        (501) staff       (20)     7413 2023-07-18 19:21:36.000000 bandcamp_api-0.2.1/bandcamp_api/bandcamp_api.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     1615 2023-05-26 17:47:35.000000 bandcamp_api-0.2.1/bandcamp_api/bandcampjson.py
+-rwxr-xr-x   0 rin        (501) staff       (20)    10654 2023-05-26 17:47:35.000000 bandcamp_api-0.2.1/bandcamp_api/daily.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     1846 2023-07-18 18:48:37.000000 bandcamp_api-0.2.1/bandcamp_api/genres.py
+-rwxr-xr-x   0 rin        (501) staff       (20)    14004 2023-07-18 18:48:37.000000 bandcamp_api-0.2.1/bandcamp_api/homepage.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     2618 2023-07-18 18:48:37.000000 bandcamp_api-0.2.1/bandcamp_api/label.py
+-rw-r--r--   0 rin        (501) staff       (20)     6226 2023-07-18 18:48:37.000000 bandcamp_api-0.2.1/bandcamp_api/search.py
+-rwxr-xr-x   0 rin        (501) staff       (20)     5540 2023-07-18 18:48:37.000000 bandcamp_api-0.2.1/bandcamp_api/track.py
+drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:34:55.674580 bandcamp_api-0.2.1/bandcamp_api.egg-info/
+-rw-r--r--   0 rin        (501) staff       (20)      218 2023-07-18 19:34:55.000000 bandcamp_api-0.2.1/bandcamp_api.egg-info/PKG-INFO
+-rw-r--r--   0 rin        (501) staff       (20)      520 2023-07-18 19:34:55.000000 bandcamp_api-0.2.1/bandcamp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 rin        (501) staff       (20)        1 2023-07-18 19:34:55.000000 bandcamp_api-0.2.1/bandcamp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 rin        (501) staff       (20)        1 2023-07-18 19:34:55.000000 bandcamp_api-0.2.1/bandcamp_api.egg-info/not-zip-safe
+-rw-r--r--   0 rin        (501) staff       (20)       58 2023-07-18 19:34:55.000000 bandcamp_api-0.2.1/bandcamp_api.egg-info/requires.txt
+-rw-r--r--   0 rin        (501) staff       (20)       13 2023-07-18 19:34:55.000000 bandcamp_api-0.2.1/bandcamp_api.egg-info/top_level.txt
+-rw-r--r--   0 rin        (501) staff       (20)       38 2023-07-18 19:34:55.675164 bandcamp_api-0.2.1/setup.cfg
+-rwxr-xr-x   0 rin        (501) staff       (20)      402 2023-07-18 19:34:30.000000 bandcamp_api-0.2.1/setup.py
+drwxr-xr-x   0 rin        (501) staff       (20)        0 2023-07-18 19:34:55.674721 bandcamp_api-0.2.1/tests/
+-rw-r--r--   0 rin        (501) staff       (20)      513 2023-07-18 19:32:17.000000 bandcamp_api-0.2.1/tests/test1.py
```

### Comparing `bandcamp_api-0.2.0/LICENSE` & `bandcamp_api-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/README.md` & `bandcamp_api-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 ```python
 from bandcamp_api import Bandcamp
 
 bc = Bandcamp()
 
 album = bc.get_album(album_url="https://c418.bandcamp.com/album/minecraft-volume-alpha")
 
-print("Album title:", album.album_title)
+print("Album title: " + album.album_title)
 ```
 
 For more information on the functions available see the [functions wiki](https://github.com/RustyRin/bandcamp-api/wiki/Functions) or the [object wiki](https://github.com/RustyRin/bandcamp-api/wiki/Bandcamp-api-Objects)
```

### Comparing `bandcamp_api-0.2.0/bandcamp_api/album.py` & `bandcamp_api-0.2.1/bandcamp_api/album.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/artist.py` & `bandcamp_api-0.2.1/bandcamp_api/artist.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/bandcamp_api.py` & `bandcamp_api-0.2.1/bandcamp_api/bandcamp_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,25 +39,31 @@
 
 class Bandcamp:
     def __init__(self):
         self.headers = {'User-Agent': 'bandcamp-api/0 (https://github.com/RustyRin/bandcamp-api)'}
         self.soup = None
         self.tracks = None
 
-    def get_album(self, album_url: str, advanced: bool = False) -> Album | Track:
+    def get_album(self, album_url: str = None,
+                  album_id: int | str = None,
+                  artist_id: int | str = None,
+                  advanced: bool = False) -> Album | Track:
         """Returns information for a given album URL"""
         # split by /album/
         # take first
 
-        if '/album/' in album_url:
-            search_term = album_url.split('/album/')[1]
-        elif '/track/' in album_url:
-            search_term = album_url.split('/track/')[1]
+        if album_id is not None and artist_id is not None:
+            return Album(album_id=album_id, artist_id=artist_id, advanced=advanced)
+        else:
+            if '/album/' in album_url:
+                search_term = album_url.split('/album/')[1]
+            elif '/track/' in album_url:
+                search_term = album_url.split('/track/')[1]
 
-        results = search(search_string=search_term.rstrip("//"))
+            results = search(search_string=search_term.rstrip("//"))
 
         for item in results:
             if item.url == album_url.rstrip('//'):
                 return Album(album_id=item.album_id, artist_id=item.artist_id, advanced=advanced)
 
     def get_track(self, track_url: str, advanced: bool = False) -> Track:
         """Returns information for a given track URL"""
```

### Comparing `bandcamp_api-0.2.0/bandcamp_api/bandcampjson.py` & `bandcamp_api-0.2.1/bandcamp_api/bandcampjson.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/daily.py` & `bandcamp_api-0.2.1/bandcamp_api/daily.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/genres.py` & `bandcamp_api-0.2.1/bandcamp_api/genres.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/homepage.py` & `bandcamp_api-0.2.1/bandcamp_api/homepage.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/label.py` & `bandcamp_api-0.2.1/bandcamp_api/label.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/search.py` & `bandcamp_api-0.2.1/bandcamp_api/search.py`

 * *Files identical despite different names*

### Comparing `bandcamp_api-0.2.0/bandcamp_api/track.py` & `bandcamp_api-0.2.1/bandcamp_api/track.py`

 * *Files identical despite different names*

