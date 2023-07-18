# Comparing `tmp/backgroundremover-0.2.3.tar.gz` & `tmp/backgroundremover-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backgroundremover-0.2.3.tar", last modified: Mon May 29 01:29:12 2023, max compression
+gzip compressed data, was "backgroundremover-0.2.4.tar", last modified: Tue Jul 18 15:33:46 2023, max compression
```

## Comparing `backgroundremover-0.2.3.tar` & `backgroundremover-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.3/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.3/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     6191 2023-05-15 23:12:59.000000 backgroundremover-0.2.3/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover/
--rw-rw-r--   0 john      (1000) john      (1000)      175 2023-05-29 01:28:23.000000 backgroundremover-0.2.3/backgroundremover/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     6964 2023-05-29 01:24:44.000000 backgroundremover-0.2.3/backgroundremover/bg.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover/cmd/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/cmd/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/cmd/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/cmd/server.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover/u2net/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/data_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/detect.py
--rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/u2net.py
--rw-rw-r--   0 john      (1000) john      (1000)    12628 2023-05-15 23:12:59.000000 backgroundremover-0.2.3/backgroundremover/utilities.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      654 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       18 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.3/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-06 14:07:42.000000 backgroundremover-0.2.3/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1027 2023-05-29 01:28:23.000000 backgroundremover-0.2.3/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-18 15:33:46.233898 backgroundremover-0.2.4/
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      183 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     6690 2023-07-18 15:33:46.233898 backgroundremover-0.2.4/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     6191 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-18 15:33:46.229898 backgroundremover-0.2.4/backgroundremover/
+-rw-rw-r--   0 john      (1000) john      (1000)      175 2023-07-18 15:27:25.000000 backgroundremover-0.2.4/backgroundremover/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6964 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/bg.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-18 15:33:46.233898 backgroundremover-0.2.4/backgroundremover/cmd/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/cmd/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/cmd/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/cmd/server.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-18 15:33:46.233898 backgroundremover-0.2.4/backgroundremover/u2net/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/u2net/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/u2net/data_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/u2net/detect.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-07-01 21:34:29.000000 backgroundremover-0.2.4/backgroundremover/u2net/u2net.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12541 2023-07-18 15:25:35.000000 backgroundremover-0.2.4/backgroundremover/utilities.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-07-18 15:33:46.233898 backgroundremover-0.2.4/backgroundremover.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     6690 2023-07-18 15:33:46.000000 backgroundremover-0.2.4/backgroundremover.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      654 2023-07-18 15:33:46.000000 backgroundremover-0.2.4/backgroundremover.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-07-18 15:33:46.000000 backgroundremover-0.2.4/backgroundremover.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       69 2023-07-18 15:33:46.000000 backgroundremover-0.2.4/backgroundremover.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      350 2023-07-18 15:33:46.000000 backgroundremover-0.2.4/backgroundremover.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       18 2023-07-18 15:33:46.000000 backgroundremover-0.2.4/backgroundremover.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      230 2023-07-01 21:34:32.000000 backgroundremover-0.2.4/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)      350 2023-07-01 21:34:32.000000 backgroundremover-0.2.4/requirements.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       78 2023-07-18 15:33:46.233898 backgroundremover-0.2.4/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1027 2023-07-18 15:27:25.000000 backgroundremover-0.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backgroundremover-0.2.3/LICENSE.txt` & `backgroundremover-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/README.md` & `backgroundremover-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/backgroundremover/bg.py` & `backgroundremover-0.2.4/backgroundremover/bg.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/backgroundremover/cmd/cli.py` & `backgroundremover-0.2.4/backgroundremover/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/backgroundremover/cmd/server.py` & `backgroundremover-0.2.4/backgroundremover/cmd/server.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/backgroundremover/u2net/data_loader.py` & `backgroundremover-0.2.4/backgroundremover/u2net/data_loader.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/backgroundremover/u2net/detect.py` & `backgroundremover-0.2.4/backgroundremover/u2net/detect.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/backgroundremover/u2net/u2net.py` & `backgroundremover-0.2.4/backgroundremover/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/backgroundremover/utilities.py` & `backgroundremover-0.2.4/backgroundremover/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,15 +180,15 @@
     matte_key(temp_file, file_path,
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
-    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest '%s'" % (
+    cmd = "ffmpeg -y -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest '%s'" % (
         file_path, temp_file, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
 
     return
 
 
@@ -206,15 +206,15 @@
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[fg];[2][fg]overlay=(main_w-overlay_w)/2:(main_h-overlay_h)/2:format=auto,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest '%s'" % (
+    cmd = "ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[fg];[2][fg]overlay=(main_w-overlay_w)/2:(main_h-overlay_h)/2:format=auto,fps=10,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse' -shortest '%s'" % (
         file_path, temp_file, overlay, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
@@ -235,22 +235,17 @@
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -nostats -loglevel 0 -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1' -c:v qtrle -shortest '%s'" % (
+    cmd = "ffmpeg -y -nostats -loglevel 0 -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1' -c:v qtrle -shortest '%s'" % (
         file_path, temp_file, output)
-    process = sp.Popen(cmd, shell=True, stdout=sp.PIPE, stderr=sp.PIPE)
-    stdout, stderr = process.communicate()
-    print('after call')
-
-    if stderr:
-        return "ERROR: %s" % stderr.decode("utf-8")
+    sp.run(shlex.split(cmd))
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
     return
 
@@ -269,15 +264,15 @@
               worker_nodes,
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[vid];[vid][2:v]scale2ref[fg][bg];[bg][fg]overlay=shortest=1[out]' -map [out] -shortest '%s'" % (
+    cmd = "ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[1][0]scale2ref[mask][main];[main][mask]alphamerge=shortest=1[vid];[vid][2:v]scale2ref[fg][bg];[bg][fg]overlay=shortest=1[out]' -map [out] -shortest '%s'" % (
         file_path, temp_file, overlay, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
@@ -299,45 +294,46 @@
               gpu_batchsize,
               model_name,
               frame_limit,
               prefetched_batches,
               framerate)
     print("Scale image")
     temp_image = os.path.abspath("%s/new.jpg" % tmpdirname)
-    cmd = "nice -10 ffmpeg -i '%s' -i '%s' -filter_complex 'scale2ref[img][vid];[img]setsar=1;[vid]nullsink' -q:v 2 '%s'" % (
+    cmd = "ffmpeg -i '%s' -i '%s' -filter_complex 'scale2ref[img][vid];[img]setsar=1;[vid]nullsink' -q:v 2 '%s'" % (
         overlay, file_path, temp_image)
     sp.run(shlex.split(cmd))
     print("Starting alphamerge")
-    cmd = "nice -10 ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[0:v]scale2ref=oh*mdar:ih[bg];[1:v]scale2ref=oh*mdar:ih[fg];[bg][fg]overlay=(W-w)/2:(H-h)/2:shortest=1[out]' -map [out] -shortest '%s'" % (
+    cmd = "ffmpeg -y -i '%s' -i '%s' -i '%s' -filter_complex '[0:v]scale2ref=oh*mdar:ih[bg];[1:v]scale2ref=oh*mdar:ih[fg];[bg][fg]overlay=(W-w)/2:(H-h)/2:shortest=1[out]' -map [out] -shortest '%s'" % (
         temp_image, file_path, temp_file, output)
     sp.run(shlex.split(cmd))
     print("Process finished")
     try:
         temp_dir.cleanup()
     except PermissionError:
         pass
     return
 
 def download_files_from_github(path, model_name):
-    if model_name not in ["u2net", "u2net_human_seg"]:
-        print("Invalid model name, please use 'u2net' or 'u2net_human_seg'")
+    if model_name not in ["u2net", "u2net_human_seg", "u2netp"]:
+        print("Invalid model name, please use 'u2net' or 'u2net_human_seg' or 'u2netp'")
         return
     print(f"downloading model [{model_name}] to {path} ...")
     urls = []
     if model_name == "u2net":
         urls = ['https://github.com/nadermx/backgroundremover/raw/main/models/u2aa',
                 'https://github.com/nadermx/backgroundremover/raw/main/models/u2ab',
                 'https://github.com/nadermx/backgroundremover/raw/main/models/u2ac',
                 'https://github.com/nadermx/backgroundremover/raw/main/models/u2ad']
     elif model_name == "u2net_human_seg":
         urls = ['https://github.com/nadermx/backgroundremover/raw/main/models/u2haa',
                 'https://github.com/nadermx/backgroundremover/raw/main/models/u2hab',
                 'https://github.com/nadermx/backgroundremover/raw/main/models/u2hac',
                 'https://github.com/nadermx/backgroundremover/raw/main/models/u2had']
-
+    elif model_name == 'u2netp':
+        urls = ['https://github.com/nadermx/backgroundremover/raw/main/models/u2netp.pth']
     try:
         os.makedirs(os.path.expanduser("~/.u2net"), exist_ok=True)
     except Exception as e:
         print(f"Error creating directory: {e}")
         return
 
     try:
```

### Comparing `backgroundremover-0.2.3/backgroundremover.egg-info/SOURCES.txt` & `backgroundremover-0.2.4/backgroundremover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.3/setup.py` & `backgroundremover-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 with open("requirements.txt") as f:
     requireds = f.read().splitlines()
 
 setup(
     name="backgroundremover",
-    version="0.2.3",
+    version="0.2.4",
     description="Background remover from image and video using AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nadermx/backgroundremover",
     author="Johnathan Nader",
     author_email="john@nader.mx",
     classifiers=[
```

