# Comparing `tmp/pytorch-perf-0.0.1.dev0.tar.gz` & `tmp/pytorch-perf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-perf-0.0.1.dev0.tar", last modified: Sun Jul  2 23:03:53 2023, max compression
+gzip compressed data, was "pytorch-perf-0.0.2.tar", last modified: Tue Jul 18 05:13:36 2023, max compression
```

## Comparing `pytorch-perf-0.0.1.dev0.tar` & `pytorch-perf-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-02 23:03:53.255428 pytorch-perf-0.0.1.dev0/
--rw-rw-r--   0 yren      (1000) yren      (1000)     1488 2023-07-02 21:44:16.000000 pytorch-perf-0.0.1.dev0/LICENSE
--rw-rw-r--   0 yren      (1000) yren      (1000)     1000 2023-07-02 23:03:53.255428 pytorch-perf-0.0.1.dev0/PKG-INFO
--rw-r--r--   0 yren      (1000) yren      (1000)      365 2023-07-02 22:44:42.000000 pytorch-perf-0.0.1.dev0/README.md
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-02 23:03:53.255428 pytorch-perf-0.0.1.dev0/pytorch_perf.egg-info/
--rw-rw-r--   0 yren      (1000) yren      (1000)     1000 2023-07-02 23:03:53.000000 pytorch-perf-0.0.1.dev0/pytorch_perf.egg-info/PKG-INFO
--rw-rw-r--   0 yren      (1000) yren      (1000)      271 2023-07-02 23:03:53.000000 pytorch-perf-0.0.1.dev0/pytorch_perf.egg-info/SOURCES.txt
--rw-rw-r--   0 yren      (1000) yren      (1000)        1 2023-07-02 23:03:53.000000 pytorch-perf-0.0.1.dev0/pytorch_perf.egg-info/dependency_links.txt
--rw-rw-r--   0 yren      (1000) yren      (1000)       10 2023-07-02 23:03:53.000000 pytorch-perf-0.0.1.dev0/pytorch_perf.egg-info/top_level.txt
--rw-rw-r--   0 yren      (1000) yren      (1000)       38 2023-07-02 23:03:53.255428 pytorch-perf-0.0.1.dev0/setup.cfg
--rw-r--r--   0 yren      (1000) yren      (1000)     1576 2023-07-02 23:02:37.000000 pytorch-perf-0.0.1.dev0/setup.py
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-02 23:03:53.255428 pytorch-perf-0.0.1.dev0/tests/
--rw-r--r--   0 yren      (1000) yren      (1000)      650 2023-07-02 21:41:19.000000 pytorch-perf-0.0.1.dev0/tests/test_basics.py
--rw-r--r--   0 yren      (1000) yren      (1000)       62 2023-07-02 22:38:17.000000 pytorch-perf-0.0.1.dev0/tests/test_info.py
-drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-02 23:03:53.255428 pytorch-perf-0.0.1.dev0/torchperf/
--rw-r--r--   0 yren      (1000) yren      (1000)       99 2023-06-25 02:11:17.000000 pytorch-perf-0.0.1.dev0/torchperf/__init__.py
--rw-r--r--   0 yren      (1000) yren      (1000)     1173 2023-07-02 22:42:32.000000 pytorch-perf-0.0.1.dev0/torchperf/info.py
--rw-rw-r--   0 yren      (1000) yren      (1000)      757 2023-07-02 22:45:23.000000 pytorch-perf-0.0.1.dev0/torchperf/measure.py
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1488 2023-07-02 21:44:16.000000 pytorch-perf-0.0.2/LICENSE
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1764 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/PKG-INFO
+-rw-r--r--   0 yren      (1000) yren      (1000)     1134 2023-07-18 04:45:11.000000 pytorch-perf-0.0.2/README.md
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.809395 pytorch-perf-0.0.2/pytorch_perf.egg-info/
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1764 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/PKG-INFO
+-rw-rw-r--   0 yren      (1000) yren      (1000)      347 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/SOURCES.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)        1 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/dependency_links.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)        6 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/requires.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)       10 2023-07-18 05:13:36.000000 pytorch-perf-0.0.2/pytorch_perf.egg-info/top_level.txt
+-rw-rw-r--   0 yren      (1000) yren      (1000)       38 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/setup.cfg
+-rw-r--r--   0 yren      (1000) yren      (1000)     1565 2023-07-18 04:48:19.000000 pytorch-perf-0.0.2/setup.py
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.809395 pytorch-perf-0.0.2/tests/
+-rw-r--r--   0 yren      (1000) yren      (1000)      810 2023-07-18 02:40:40.000000 pytorch-perf-0.0.2/tests/test_basics.py
+-rw-r--r--   0 yren      (1000) yren      (1000)      129 2023-07-18 04:27:37.000000 pytorch-perf-0.0.2/tests/test_info.py
+-rw-r--r--   0 yren      (1000) yren      (1000)     1137 2023-07-18 04:25:12.000000 pytorch-perf-0.0.2/tests/test_recipe.py
+drwxrwxr-x   0 yren      (1000) yren      (1000)        0 2023-07-18 05:13:36.813395 pytorch-perf-0.0.2/torchperf/
+-rw-r--r--   0 yren      (1000) yren      (1000)      160 2023-07-18 04:46:24.000000 pytorch-perf-0.0.2/torchperf/__init__.py
+-rw-r--r--   0 yren      (1000) yren      (1000)     1225 2023-07-18 02:30:25.000000 pytorch-perf-0.0.2/torchperf/info.py
+-rw-rw-r--   0 yren      (1000) yren      (1000)     1188 2023-07-18 02:39:48.000000 pytorch-perf-0.0.2/torchperf/measure.py
+-rw-r--r--   0 yren      (1000) yren      (1000)     2589 2023-07-18 04:30:41.000000 pytorch-perf-0.0.2/torchperf/recipe.py
```

### Comparing `pytorch-perf-0.0.1.dev0/LICENSE` & `pytorch-perf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-perf-0.0.1.dev0/setup.py` & `pytorch-perf-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,20 +24,20 @@
         license="BSD-3",
         long_description=LONG_DESC,
         long_description_content_type="text/markdown",
         url="https://github.com/yhren/torchperf",
         keywords="decorator cuda performance perf pytorch",
         packages=find_namespace_packages(include=["torchperf", "torchperf.*"]),
         include_package_data=True,
-        python_requires = ">=3.9",
+        python_requires=">=3.9",
         classifiers=[
             "License :: OSI Approved :: BSD License",
             "Development Status :: 2 - Pre-Alpha",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Operating System :: POSIX :: Linux",
         ],
-        # install_requires=install_requires,
+        install_requires=["numpy"],
         # Install development dependencies with
         # pip install -r requirements/dev.txt -e .
     )
```

### Comparing `pytorch-perf-0.0.1.dev0/tests/test_basics.py` & `pytorch-perf-0.0.2/tests/test_basics.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,7 +41,18 @@
 
     @perf(o=rst, n=10)
     def mul(x, y):
         return x * y
 
     _ = mul(x, y)
     assert len(rst) > 0
+
+
+def test_output_repeat_warmup():
+    rst = []
+
+    @perf(o=rst, n=10, w=3)
+    def mul(x, y):
+        return x * y
+
+    _ = mul(x, y)
+    assert len(rst) > 0
```

### Comparing `pytorch-perf-0.0.1.dev0/torchperf/info.py` & `pytorch-perf-0.0.2/torchperf/info.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,22 +15,25 @@
         ["nvidia-smi", "--query-gpu=driver_version", "--format=csv", "-i", "0"],
         stdout=PIPE,
     )
     rst = check_output(["tail", "-n1"], stdin=p.stdout)
     return rst.decode("utf-8").strip()
 
 
+def get_linux_kernel():
+    return subprocess.check_output(["uname", "-r"]).decode("utf-8").strip()
+
+
 def show():
     def ver2str(x):
         return ".".join(map(str, x))
 
-    kernel_ver = subprocess.check_output(["uname", "-r"])
     print("python     ver|", ver2str(sys.version_info[:3]))
     print("pytorch    ver|", torch.__version__)
     print("CUDA       ver|", torch.version.cuda)
     print("cuDNN      ver|", torch.backends.cudnn.version() / 1000)
     print("nccl       ver|", ver2str(torch.cuda.nccl.version()))
     print("GPU Driver ver|", get_gpu_driver())
-    print("Kernel     ver|", kernel_ver)
+    print("Kernel     ver|", get_linux_kernel())
     print("Device Name   |", torch.cuda.get_device_name(0))
     print("OS name       |", get_os_name())
     print("num GPUs      |", torch.cuda.device_count())
```

### Comparing `pytorch-perf-0.0.1.dev0/torchperf/measure.py` & `pytorch-perf-0.0.2/torchperf/measure.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 import torch
 from functools import wraps, partial
 
 
-def perf(_func=None, *, o=None, n=1):
+def perf(_func=None, *, o=None, n=1, w=1):
+    r"""performance measurement decorator
+
+    o : List, optional [=None]
+        "output" elapsed times per run are stored in the list.
+        If `o` is `None`, an averaged result is printed.
+    n : int, optional [=1]
+        "number of runs"
+    w : int, optional [=1]
+        "warmup", number of warmup runs.
+    """
+
     if not _func:
-        return partial(perf, o=o, n=n)
+        return partial(perf, o=o, n=n, w=w)
 
     @wraps(_func)
     def measure_time(*args, **kwargs):
+        # warmup
+        for _ in range(w):
+            rst = _func(*args, **kwargs)
+
+        # recording
         tot, cnt = 0.0, 0
+        stt = torch.cuda.Event(enable_timing=True)
+        end = torch.cuda.Event(enable_timing=True)
         for _ in range(n):
-            stt = torch.cuda.Event(enable_timing=True)
-            end = torch.cuda.Event(enable_timing=True)
             stt.record()
             rst = _func(*args, **kwargs)
             end.record()
             torch.cuda.synchronize()
             tim = stt.elapsed_time(end)
             if o is None:
                 tot += tim
```

