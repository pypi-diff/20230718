# Comparing `tmp/ffmpeg_quality_metrics-3.2.1.tar.gz` & `tmp/ffmpeg_quality_metrics-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg_quality_metrics-3.2.1.tar", last modified: Mon Mar  6 09:42:39 2023, max compression
+gzip compressed data, was "ffmpeg_quality_metrics-3.3.0.tar", last modified: Tue Jul 18 07:35:29 2023, max compression
```

## Comparing `ffmpeg_quality_metrics-3.2.1.tar` & `ffmpeg_quality_metrics-3.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-06 09:42:39.013845 ffmpeg_quality_metrics-3.2.1/
--rw-r--r--   0 werner     (501) staff       (20)    27429 2023-03-06 09:42:39.013973 ffmpeg_quality_metrics-3.2.1/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)    26664 2023-03-06 09:18:53.000000 ffmpeg_quality_metrics-3.2.1/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-06 09:42:39.010147 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/
--rw-r--r--   0 werner     (501) staff       (20)      444 2023-03-06 09:42:32.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     6503 2023-03-06 09:20:09.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)    29447 2023-03-06 09:40:56.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/ffmpeg_quality_metrics.py
--rw-r--r--   0 werner     (501) staff       (20)      871 2023-01-03 13:45:47.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/log.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:51:28.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/py.typed
--rw-r--r--   0 werner     (501) staff       (20)     2321 2023-01-03 13:45:49.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/utils.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-06 09:42:39.013367 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/vmaf_models/
--rw-r--r--   0 werner     (501) staff       (20)    22910 2021-02-09 19:33:31.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/vmaf_models/vmaf_4k_v0.6.1.json
--rw-r--r--   0 werner     (501) staff       (20)    19101 2021-02-09 19:33:31.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1.json
--rw-r--r--   0 werner     (501) staff       (20)    19519 2021-02-09 19:33:31.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1neg.json
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-06 09:42:39.011125 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)    27429 2023-03-06 09:42:38.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      694 2023-03-06 09:42:38.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-03-06 09:42:38.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       80 2023-03-06 09:42:38.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)       41 2023-03-06 09:42:38.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/requires.txt
--rw-r--r--   0 werner     (501) staff       (20)       23 2023-03-06 09:42:38.000000 ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      280 2023-03-06 09:42:39.014253 ffmpeg_quality_metrics-3.2.1/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1810 2023-01-03 13:48:53.000000 ffmpeg_quality_metrics-3.2.1/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-03-06 09:42:39.013587 ffmpeg_quality_metrics-3.2.1/test/
--rw-r--r--   0 werner     (501) staff       (20)     4344 2023-02-19 12:59:58.000000 ffmpeg_quality_metrics-3.2.1/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-18 07:35:29.175938 ffmpeg_quality_metrics-3.3.0/
+-rw-r--r--   0 werner     (501) staff       (20)    27814 2023-07-18 07:35:29.176139 ffmpeg_quality_metrics-3.3.0/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)    27049 2023-07-18 07:35:08.000000 ffmpeg_quality_metrics-3.3.0/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-18 07:35:29.168659 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/
+-rw-r--r--   0 werner     (501) staff       (20)      444 2023-07-18 07:35:24.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     6730 2023-07-18 07:34:03.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)    29703 2023-07-18 07:32:25.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/ffmpeg_quality_metrics.py
+-rw-r--r--   0 werner     (501) staff       (20)      871 2023-01-03 13:45:47.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/log.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:51:28.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/py.typed
+-rw-r--r--   0 werner     (501) staff       (20)     2321 2023-01-03 13:45:49.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/utils.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-18 07:35:29.175394 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/vmaf_models/
+-rw-r--r--   0 werner     (501) staff       (20)    22910 2021-02-09 19:33:31.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/vmaf_models/vmaf_4k_v0.6.1.json
+-rw-r--r--   0 werner     (501) staff       (20)    19101 2021-02-09 19:33:31.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1.json
+-rw-r--r--   0 werner     (501) staff       (20)    19519 2021-02-09 19:33:31.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1neg.json
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-18 07:35:29.174215 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    27814 2023-07-18 07:35:29.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      694 2023-07-18 07:35:29.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-07-18 07:35:29.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       80 2023-07-18 07:35:29.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)       41 2023-07-18 07:35:29.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/requires.txt
+-rw-r--r--   0 werner     (501) staff       (20)       23 2023-07-18 07:35:29.000000 ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      280 2023-07-18 07:35:29.176998 ffmpeg_quality_metrics-3.3.0/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1852 2023-07-18 07:29:59.000000 ffmpeg_quality_metrics-3.3.0/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-07-18 07:35:29.175766 ffmpeg_quality_metrics-3.3.0/test/
+-rw-r--r--   0 werner     (501) staff       (20)     4344 2023-02-19 12:59:58.000000 ffmpeg_quality_metrics-3.3.0/test/test.py
```

### Comparing `ffmpeg_quality_metrics-3.2.1/PKG-INFO` & `ffmpeg_quality_metrics-3.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg_quality_metrics
-Version: 3.2.1
+Version: 3.3.0
 Summary: Calculate video quality metrics with FFmpeg (SSIM, PSNR, VMAF)
 Home-page: https://github.com/slhck/ffmpeg-quality-metrics
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -90,14 +90,16 @@
 
 ```
 ffmpeg-quality-metrics distorted.mp4 reference.avi
 ```
 
 The distorted file will be automatically scaled to the resolution of the reference, and the default metrics (PSNR, SSIM) will be computed.
 
+Note that if your distorted file is not in time sync with the reference, you can use the `--dist-delay` option to delay the distorted file by a certain amount of seconds (positive or negative).
+
 ### Metrics
 
 The following metrics are available in this tool:
 
 | Metric | Description                                                                            | Scale                    | Components/Submetrics                                                                                                                                                                                                                       | Calculated by default? |
 | ------ | -------------------------------------------------------------------------------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- |
 | PSNR   | [Peak Signal to Noise Ratio](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio) | dB                       | `mse_avg`, `mse_y`, `mse_u`, `mse_v`, `psnr_avg`, `psnr_y`, `psnr_u`, `psnr_v`                                                                                                                                                              | ✔️                      |
@@ -123,22 +125,22 @@
 
 See `ffmpeg-quality-metrics -h`:
 
 ```
 usage: ffmpeg-quality-metrics [-h] [-n] [-v] [-p] [-k] [--tmp-dir TMP_DIR]
                               [-m {vmaf,psnr,ssim,vif} [{vmaf,psnr,ssim,vif} ...]]
                               [-s {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}]
-                              [-r FRAMERATE] [-t THREADS] [-of {json,csv}]
+                              [-r FRAMERATE] [--dist-delay DIST_DELAY] [-t THREADS] [-of {json,csv}]
                               [--vmaf-model-path VMAF_MODEL_PATH]
                               [--vmaf-model-params VMAF_MODEL_PARAMS [VMAF_MODEL_PARAMS ...]]
                               [--vmaf-threads VMAF_THREADS] [--vmaf-subsample VMAF_SUBSAMPLE]
                               [--vmaf-features VMAF_FEATURES [VMAF_FEATURES ...]]
                               dist ref
 
-ffmpeg-quality-metrics v3.2.0
+ffmpeg-quality-metrics v3.2.1
 
 positional arguments:
   dist                                  input file, distorted
   ref                                   input file, reference
 
 options:
   -h, --help                            show this help message and exit
@@ -157,14 +159,16 @@
                                         Metrics to calculate. Specify multiple metrics like '--
                                         metrics ssim vmaf' (default: ['psnr', 'ssim'])
 
 FFmpeg options:
   -s {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}, --scaling-algorithm {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}
                                         Scaling algorithm for ffmpeg (default: bicubic)
   -r FRAMERATE, --framerate FRAMERATE   Force an input framerate (default: None)
+  --dist-delay DIST_DELAY               Delay the distorted video against the reference by this many
+                                        seconds (default: 0.0)
   -t THREADS, --threads THREADS         Number of threads to do the calculations (default: 0)
 
 Output options:
   -of {json,csv}, --output-format {json,csv}
                                         Output format for the metrics (default: json)
 
 VMAF options:
```

### Comparing `ffmpeg_quality_metrics-3.2.1/README.md` & `ffmpeg_quality_metrics-3.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,16 @@
 
 ```
 ffmpeg-quality-metrics distorted.mp4 reference.avi
 ```
 
 The distorted file will be automatically scaled to the resolution of the reference, and the default metrics (PSNR, SSIM) will be computed.
 
+Note that if your distorted file is not in time sync with the reference, you can use the `--dist-delay` option to delay the distorted file by a certain amount of seconds (positive or negative).
+
 ### Metrics
 
 The following metrics are available in this tool:
 
 | Metric | Description                                                                            | Scale                    | Components/Submetrics                                                                                                                                                                                                                       | Calculated by default? |
 | ------ | -------------------------------------------------------------------------------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- |
 | PSNR   | [Peak Signal to Noise Ratio](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio) | dB                       | `mse_avg`, `mse_y`, `mse_u`, `mse_v`, `psnr_avg`, `psnr_y`, `psnr_u`, `psnr_v`                                                                                                                                                              | ✔️                      |
@@ -103,22 +105,22 @@
 
 See `ffmpeg-quality-metrics -h`:
 
 ```
 usage: ffmpeg-quality-metrics [-h] [-n] [-v] [-p] [-k] [--tmp-dir TMP_DIR]
                               [-m {vmaf,psnr,ssim,vif} [{vmaf,psnr,ssim,vif} ...]]
                               [-s {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}]
-                              [-r FRAMERATE] [-t THREADS] [-of {json,csv}]
+                              [-r FRAMERATE] [--dist-delay DIST_DELAY] [-t THREADS] [-of {json,csv}]
                               [--vmaf-model-path VMAF_MODEL_PATH]
                               [--vmaf-model-params VMAF_MODEL_PARAMS [VMAF_MODEL_PARAMS ...]]
                               [--vmaf-threads VMAF_THREADS] [--vmaf-subsample VMAF_SUBSAMPLE]
                               [--vmaf-features VMAF_FEATURES [VMAF_FEATURES ...]]
                               dist ref
 
-ffmpeg-quality-metrics v3.2.0
+ffmpeg-quality-metrics v3.2.1
 
 positional arguments:
   dist                                  input file, distorted
   ref                                   input file, reference
 
 options:
   -h, --help                            show this help message and exit
@@ -137,14 +139,16 @@
                                         Metrics to calculate. Specify multiple metrics like '--
                                         metrics ssim vmaf' (default: ['psnr', 'ssim'])
 
 FFmpeg options:
   -s {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}, --scaling-algorithm {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}
                                         Scaling algorithm for ffmpeg (default: bicubic)
   -r FRAMERATE, --framerate FRAMERATE   Force an input framerate (default: None)
+  --dist-delay DIST_DELAY               Delay the distorted video against the reference by this many
+                                        seconds (default: 0.0)
   -t THREADS, --threads THREADS         Number of threads to do the calculations (default: 0)
 
 Output options:
   -of {json,csv}, --output-format {json,csv}
                                         Output format for the metrics (default: json)
 
 VMAF options:
```

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/__main__.py` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,21 @@
         "-r",
         "--framerate",
         type=float,
         help="Force an input framerate",
     )
 
     ffmpeg_opts.add_argument(
+        "--dist-delay",
+        type=float,
+        default=0.0,
+        help="Delay the distorted video against the reference by this many seconds",
+    )
+
+    ffmpeg_opts.add_argument(
         "-t",
         "--threads",
         type=int,
         default=FfmpegQualityMetrics.DEFAULT_THREADS,
         help="Number of threads to do the calculations",
     )
 
@@ -166,14 +173,15 @@
     setup_logger(logging.DEBUG if cli_args.verbose else logging.INFO)
 
     ffqm = FfmpegQualityMetrics(
         ref=cli_args.ref,
         dist=cli_args.dist,
         scaling_algorithm=cli_args.scaling_algorithm,
         framerate=cli_args.framerate,
+        dist_delay=cli_args.dist_delay,
         dry_run=cli_args.dry_run,
         verbose=cli_args.verbose,
         threads=cli_args.threads,
         progress=cli_args.progress,
         keep_tmp_files=cli_args.keep_tmp,
         tmp_dir=cli_args.tmp_dir,
     )
```

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/ffmpeg_quality_metrics.py` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/ffmpeg_quality_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,42 +128,45 @@
 
     def __init__(
         self,
         ref: str,
         dist: str,
         scaling_algorithm: str = DEFAULT_SCALER,
         framerate: Union[float, None] = None,
+        dist_delay: float = 0,
         dry_run: Union[bool, None] = False,
         verbose: Union[bool, None] = False,
         threads: int = DEFAULT_THREADS,
         progress: Union[bool, None] = False,
         keep_tmp_files: Union[bool, None] = False,
         tmp_dir: Union[str, None] = None,
     ):
         """Instantiate a new FfmpegQualityMetrics
 
         Args:
             ref (str): reference file
             dist (str): distorted file
             scaling_algorithm (str, optional): A scaling algorithm. Must be one of the following: ["fast_bilinear", "bilinear", "bicubic", "experimental", "neighbor", "area", "bicublin", "gauss", "sinc", "lanczos", "spline"]. Defaults to "bicubic"
             framerate (float, optional): Force a frame rate. Defaults to None.
+            dist_delay (float): Delay the distorted file against the reference by this amount of seconds. Defaults to 0.
             dry_run (bool, optional): Don't run anything, just print commands. Defaults to False.
             verbose (bool, optional): Show more output. Defaults to False.
             threads (int, optional): Number of ffmpeg threads. Defaults to 0 (auto).
             progress (bool, optional): Show a progress bar. Defaults to False.
             keep_tmp_files (bool, optional): Keep temporary files for debugging purposes. Defaults to False.
             tmp_dir (str, optional): Directory to store temporary files. Will use system default if not specified. Defaults to None.
 
         Raises:
             FfmpegQualityMetricsError: A generic error
         """
         self.ref = str(ref)
         self.dist = str(dist)
         self.scaling_algorithm = str(scaling_algorithm)
         self.framerate = float(framerate) if framerate is not None else None
+        self.dist_delay = float(dist_delay)
         self.dry_run = bool(dry_run)
         self.verbose = bool(verbose)
         self.threads = int(threads)
         self.progress = bool(progress)
         self.keep_tmp_files = bool(keep_tmp_files)
         self.tmp_dir = str(tmp_dir) if tmp_dir is not None else tempfile.gettempdir()
 
@@ -569,14 +572,16 @@
             "-y",
             "-threads",
             str(self.threads),
             "-r",
             str(ref_framerate),
             "-i",
             self.ref,
+            "-itsoffset",
+            str(self.dist_delay),
             "-r",
             str(dist_framerate),
             "-i",
             self.dist,
             "-filter_complex",
             ";".join(filter_chains),
             "-an",
```

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/log.py` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/log.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/utils.py` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/vmaf_models/vmaf_4k_v0.6.1.json` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/vmaf_models/vmaf_4k_v0.6.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1.json` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1neg.json` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics/vmaf_models/vmaf_v0.6.1neg.json`

 * *Files identical despite different names*

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/PKG-INFO` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-quality-metrics
-Version: 3.2.1
+Version: 3.3.0
 Summary: Calculate video quality metrics with FFmpeg (SSIM, PSNR, VMAF)
 Home-page: https://github.com/slhck/ffmpeg-quality-metrics
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -90,14 +90,16 @@
 
 ```
 ffmpeg-quality-metrics distorted.mp4 reference.avi
 ```
 
 The distorted file will be automatically scaled to the resolution of the reference, and the default metrics (PSNR, SSIM) will be computed.
 
+Note that if your distorted file is not in time sync with the reference, you can use the `--dist-delay` option to delay the distorted file by a certain amount of seconds (positive or negative).
+
 ### Metrics
 
 The following metrics are available in this tool:
 
 | Metric | Description                                                                            | Scale                    | Components/Submetrics                                                                                                                                                                                                                       | Calculated by default? |
 | ------ | -------------------------------------------------------------------------------------- | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- |
 | PSNR   | [Peak Signal to Noise Ratio](https://en.wikipedia.org/wiki/Peak_signal-to-noise_ratio) | dB                       | `mse_avg`, `mse_y`, `mse_u`, `mse_v`, `psnr_avg`, `psnr_y`, `psnr_u`, `psnr_v`                                                                                                                                                              | ✔️                      |
@@ -123,22 +125,22 @@
 
 See `ffmpeg-quality-metrics -h`:
 
 ```
 usage: ffmpeg-quality-metrics [-h] [-n] [-v] [-p] [-k] [--tmp-dir TMP_DIR]
                               [-m {vmaf,psnr,ssim,vif} [{vmaf,psnr,ssim,vif} ...]]
                               [-s {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}]
-                              [-r FRAMERATE] [-t THREADS] [-of {json,csv}]
+                              [-r FRAMERATE] [--dist-delay DIST_DELAY] [-t THREADS] [-of {json,csv}]
                               [--vmaf-model-path VMAF_MODEL_PATH]
                               [--vmaf-model-params VMAF_MODEL_PARAMS [VMAF_MODEL_PARAMS ...]]
                               [--vmaf-threads VMAF_THREADS] [--vmaf-subsample VMAF_SUBSAMPLE]
                               [--vmaf-features VMAF_FEATURES [VMAF_FEATURES ...]]
                               dist ref
 
-ffmpeg-quality-metrics v3.2.0
+ffmpeg-quality-metrics v3.2.1
 
 positional arguments:
   dist                                  input file, distorted
   ref                                   input file, reference
 
 options:
   -h, --help                            show this help message and exit
@@ -157,14 +159,16 @@
                                         Metrics to calculate. Specify multiple metrics like '--
                                         metrics ssim vmaf' (default: ['psnr', 'ssim'])
 
 FFmpeg options:
   -s {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}, --scaling-algorithm {fast_bilinear,bilinear,bicubic,experimental,neighbor,area,bicublin,gauss,sinc,lanczos,spline}
                                         Scaling algorithm for ffmpeg (default: bicubic)
   -r FRAMERATE, --framerate FRAMERATE   Force an input framerate (default: None)
+  --dist-delay DIST_DELAY               Delay the distorted video against the reference by this many
+                                        seconds (default: 0.0)
   -t THREADS, --threads THREADS         Number of threads to do the calculations (default: 0)
 
 Output options:
   -of {json,csv}, --output-format {json,csv}
                                         Output format for the metrics (default: json)
 
 VMAF options:
```

### Comparing `ffmpeg_quality_metrics-3.2.1/ffmpeg_quality_metrics.egg-info/SOURCES.txt` & `ffmpeg_quality_metrics-3.3.0/ffmpeg_quality_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffmpeg_quality_metrics-3.2.1/setup.py` & `ffmpeg_quality_metrics-3.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 import os
 
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Versioning
-with open(os.path.join(here, "ffmpeg_quality_metrics", "__init__.py")) as version_file:
+with open(
+    os.path.join(here, "ffmpeg_quality_metrics", "__init__.py"), encoding="utf-8"
+) as version_file:
     # parse the string that looks like '__version__ = "3.1.2"'
     for line in version_file:
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().strip('"')
             break
 
 # Get the long description from the README file
-with open(os.path.join(here, "README.md")) as f:
+with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ffmpeg_quality_metrics",
     version=version,
     description="Calculate video quality metrics with FFmpeg (SSIM, PSNR, VMAF)",
     long_description=long_description,
```

### Comparing `ffmpeg_quality_metrics-3.2.1/test/test.py` & `ffmpeg_quality_metrics-3.3.0/test/test.py`

 * *Files identical despite different names*

