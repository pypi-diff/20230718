# Comparing `tmp/polimedia_client-0.0.2.tar.gz` & `tmp/polimedia_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polimedia_client-0.0.2.tar", last modified: Wed Oct 26 12:07:28 2022, max compression
+gzip compressed data, was "polimedia_client-0.0.3.tar", last modified: Tue Jul 18 07:43:15 2023, max compression
```

## Comparing `polimedia_client-0.0.2.tar` & `polimedia_client-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2022-10-26 12:07:28.102962 polimedia_client-0.0.2/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      425 2022-10-26 12:07:28.102962 polimedia_client-0.0.2/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      142 2022-10-26 08:18:15.000000 polimedia_client-0.0.2/README.md
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2022-10-26 12:07:28.098962 polimedia_client-0.0.2/polimedia/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     8220 2022-10-26 11:59:43.000000 polimedia_client-0.0.2/polimedia/__init__.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2022-10-26 12:07:28.102962 polimedia_client-0.0.2/polimedia_client.egg-info/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      425 2022-10-26 12:07:28.000000 polimedia_client-0.0.2/polimedia_client.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      239 2022-10-26 12:07:28.000000 polimedia_client-0.0.2/polimedia_client.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2022-10-26 12:07:28.000000 polimedia_client-0.0.2/polimedia_client.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2022-10-26 12:07:28.000000 polimedia_client-0.0.2/polimedia_client.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       10 2022-10-26 12:07:28.000000 polimedia_client-0.0.2/polimedia_client.egg-info/top_level.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2022-10-26 12:07:28.102962 polimedia_client-0.0.2/setup.cfg
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      967 2022-10-26 08:39:43.000000 polimedia_client-0.0.2/setup.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-18 07:43:15.834180 polimedia_client-0.0.3/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      425 2023-07-18 07:43:15.834180 polimedia_client-0.0.3/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      142 2022-10-26 08:18:15.000000 polimedia_client-0.0.3/README.md
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-18 07:43:15.826181 polimedia_client-0.0.3/polimedia/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     9301 2023-07-18 07:40:15.000000 polimedia_client-0.0.3/polimedia/__init__.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2023-07-18 07:43:15.834180 polimedia_client-0.0.3/polimedia_client.egg-info/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      425 2023-07-18 07:43:15.000000 polimedia_client-0.0.3/polimedia_client.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      239 2023-07-18 07:43:15.000000 polimedia_client-0.0.3/polimedia_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2023-07-18 07:43:15.000000 polimedia_client-0.0.3/polimedia_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2023-07-18 07:43:15.000000 polimedia_client-0.0.3/polimedia_client.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       10 2023-07-18 07:43:15.000000 polimedia_client-0.0.3/polimedia_client.egg-info/top_level.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2023-07-18 07:43:15.834180 polimedia_client-0.0.3/setup.cfg
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      967 2022-10-26 08:39:43.000000 polimedia_client-0.0.3/setup.py
```

### Comparing `polimedia_client-0.0.2/polimedia/__init__.py` & `polimedia_client-0.0.3/polimedia/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 import pymongo
 import pprint
 from datetime import datetime
 from loguru import logger
 from pathlib import Path
 from typing import Optional, List
@@ -202,7 +202,33 @@
             repoinfo["server"]
             + repoinfo["endpoint"]
             + videoId
             + "/polimedia/"
             + video_json["source"]["videos"][0]["src"]
         )
         return videoFileURL
+
+    # Channels
+    def get_mongo_entry_for_channel(self, channel_id: str) -> Optional[dict]:
+        """
+        Given the ID of a channel, returns the info stored in the PoliMedia Mongo DB
+        about that channel.
+
+        :param channel_id: Channel video id (e.g. e98845a0-0298-11ed-abaa-3f7da180bcf7)
+        :returns: JSON/dict-like object with information about the video
+        """
+
+        filt = {"_id": channel_id}
+        return self.db.videos.find_one(filt)
+
+    def get_channel_videos(self, channel_id, recursion_level=0, max_recursion=5):
+        channel_videos = []
+        recursion_level += 1
+        channel_info = self.db.channels.find_one({"_id": channel_id})
+        if not channel_info:
+            raise Exception(f"No channel with ID {channel_id} could be found")
+        for v in channel_info["videos"]:
+            channel_videos.append(v)
+        if recursion_level <= max_recursion:
+            for c in channel_info["children"]:
+                channel_videos += self.get_channel_videos(c, recursion_level)
+        return list(set(channel_videos))
```

### Comparing `polimedia_client-0.0.2/setup.py` & `polimedia_client-0.0.3/setup.py`

 * *Files identical despite different names*

