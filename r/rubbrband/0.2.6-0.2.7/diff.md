# Comparing `tmp/rubbrband-0.2.6.tar.gz` & `tmp/rubbrband-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubbrband-0.2.6.tar", last modified: Fri Jun 23 04:42:24 2023, max compression
+gzip compressed data, was "rubbrband-0.2.7.tar", last modified: Tue Jul 18 03:17:46 2023, max compression
```

## Comparing `rubbrband-0.2.6.tar` & `rubbrband-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-23 04:42:24.686425 rubbrband-0.2.6/
--rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.6/LICENSE
--rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.6/MANIFEST.in
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-23 04:42:24.686481 rubbrband-0.2.6/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.6/README.md
--rw-r--r--   0 llewyn     (501) staff       (20)      103 2023-06-19 21:09:40.000000 rubbrband-0.2.6/pyproject.toml
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-23 04:42:24.685709 rubbrband-0.2.6/rubbrband/
--rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.6/rubbrband/__init__.py
--rw-r--r--   0 llewyn     (501) staff       (20)     1473 2023-06-23 04:41:52.000000 rubbrband-0.2.6/rubbrband/main.py
-drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-06-23 04:42:24.686318 rubbrband-0.2.6/rubbrband.egg-info/
--rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/PKG-INFO
--rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/SOURCES.txt
--rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/dependency_links.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       16 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/requires.txt
--rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-06-23 04:42:24.000000 rubbrband-0.2.6/rubbrband.egg-info/top_level.txt
--rw-r--r--   0 llewyn     (501) staff       (20)      259 2023-06-23 04:42:24.686703 rubbrband-0.2.6/setup.cfg
--rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-06-19 21:09:40.000000 rubbrband-0.2.6/setup.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-07-18 03:17:46.047404 rubbrband-0.2.7/
+-rw-r--r--   0 llewyn     (501) staff       (20)    11357 2023-03-07 10:22:28.000000 rubbrband-0.2.7/LICENSE
+-rw-r--r--   0 llewyn     (501) staff       (20)       48 2023-02-24 08:26:52.000000 rubbrband-0.2.7/MANIFEST.in
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-07-18 03:17:46.047470 rubbrband-0.2.7/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)       54 2023-06-07 21:39:04.000000 rubbrband-0.2.7/README.md
+-rw-r--r--   0 llewyn     (501) staff       (20)      103 2023-06-19 21:09:40.000000 rubbrband-0.2.7/pyproject.toml
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-07-18 03:17:46.046405 rubbrband-0.2.7/rubbrband/
+-rw-r--r--   0 llewyn     (501) staff       (20)       61 2023-06-07 21:45:01.000000 rubbrband-0.2.7/rubbrband/__init__.py
+-rw-r--r--   0 llewyn     (501) staff       (20)     1206 2023-07-18 03:16:46.000000 rubbrband-0.2.7/rubbrband/main.py
+drwxr-xr-x   0 llewyn     (501) staff       (20)        0 2023-07-18 03:17:46.047264 rubbrband-0.2.7/rubbrband.egg-info/
+-rw-r--r--   0 llewyn     (501) staff       (20)      125 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/PKG-INFO
+-rw-r--r--   0 llewyn     (501) staff       (20)      267 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/SOURCES.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)        1 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/dependency_links.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       16 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/requires.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)       10 2023-07-18 03:17:46.000000 rubbrband-0.2.7/rubbrband.egg-info/top_level.txt
+-rw-r--r--   0 llewyn     (501) staff       (20)      259 2023-07-18 03:17:46.047746 rubbrband-0.2.7/setup.cfg
+-rw-r--r--   0 llewyn     (501) staff       (20)      182 2023-06-19 21:09:40.000000 rubbrband-0.2.7/setup.py
```

### Comparing `rubbrband-0.2.6/LICENSE` & `rubbrband-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rubbrband-0.2.6/rubbrband/main.py` & `rubbrband-0.2.7/rubbrband/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,10 @@
 
     if "url" not in response:
         return False
 
     response = response["url"]
 
     files = {"file": (name, image)}
-    http_response = requests.post(response["url"], data=response["fields"], files=files)
-
-    image_url = f"https://rubbrband-image-bucket.s3.amazonaws.com/{api_key}/{name}"
-    block_req = requests.post(
-        f"https://block.rubbrband.com/process_img?api_key={api_key}&image_url={image_url}",
-        json={"metadata": metadata},
-    )
+    requests.post(response["url"], data=response["fields"], files=files)
 
     return True
```

