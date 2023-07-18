# Comparing `tmp/grain-scheduler-0.17.0b2.tar.gz` & `tmp/grain-scheduler-0.17.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grain-scheduler-0.17.0b2.tar", last modified: Wed Oct 19 18:20:16 2022, max compression
+gzip compressed data, was "grain-scheduler-0.17.0b3.tar", last modified: Wed Nov  9 23:45:11 2022, max compression
```

## Comparing `grain-scheduler-0.17.0b2.tar` & `grain-scheduler-0.17.0b3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-10-19 18:20:16.130107 grain-scheduler-0.17.0b2/
--rw-r--r--   0 zhar     (13053) pl        (1102)     1071 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/LICENSE
--rw-r--r--   0 zhar     (13053) pl        (1102)     3736 2022-10-19 18:20:16.129096 grain-scheduler-0.17.0b2/PKG-INFO
--rw-r--r--   0 zhar     (13053) pl        (1102)     2968 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/README.md
-drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-10-19 18:20:16.038561 grain-scheduler-0.17.0b2/bench/
--rw-r--r--   0 zhar     (13053) pl        (1102)      318 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/bench/__init__.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     1115 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/bench/test_combine.py
--rw-r--r--   0 zhar     (13053) pl        (1102)      989 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/bench/test_delayed.py
--rw-r--r--   0 zhar     (13053) pl        (1102)      574 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/bench/test_head.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     2208 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/bench/test_worker.py
-drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-10-19 18:20:16.110839 grain-scheduler-0.17.0b2/grain/
--rw-r--r--   0 zhar     (13053) pl        (1102)      209 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/__init__.py
--rw-r--r--   0 zhar     (13053) pl        (1102)       25 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/_version.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     7498 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/cli.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     6429 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/combine.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     3429 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/config.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     7175 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/conn.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     6407 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/conn2.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     1291 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/conn_msgp.py
--rw-r--r--   0 zhar     (13053) pl        (1102)      567 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/contextvar.py
--rw-r--r--   0 zhar     (13053) pl        (1102)    14827 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/delayed.py
--rw-r--r--   0 zhar     (13053) pl        (1102)    18954 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/head.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     6929 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/pair.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     7898 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/remote_exer.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     9432 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/resource.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     2679 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/stat.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     4532 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/subproc.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     1571 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/subproc_worker.py
--rw-r--r--   0 zhar     (13053) pl        (1102)      723 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/test_combine.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     1457 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/test_conn2.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     3228 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/test_delayed.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     3481 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/test_head.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     1877 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/test_pair.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     3851 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/test_resource.py
--rw-r--r--   0 zhar     (13053) pl        (1102)      831 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/test_worker.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     7886 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/util.py
--rw-r--r--   0 zhar     (13053) pl        (1102)     5633 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/grain/worker.py
-drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-10-19 18:20:16.127078 grain-scheduler-0.17.0b2/grain_scheduler.egg-info/
--rw-r--r--   0 zhar     (13053) pl        (1102)     3736 2022-10-19 18:20:15.000000 grain-scheduler-0.17.0b2/grain_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 zhar     (13053) pl        (1102)      829 2022-10-19 18:20:16.000000 grain-scheduler-0.17.0b2/grain_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 zhar     (13053) pl        (1102)        1 2022-10-19 18:20:15.000000 grain-scheduler-0.17.0b2/grain_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 zhar     (13053) pl        (1102)       41 2022-10-19 18:20:15.000000 grain-scheduler-0.17.0b2/grain_scheduler.egg-info/entry_points.txt
--rw-r--r--   0 zhar     (13053) pl        (1102)      108 2022-10-19 18:20:16.000000 grain-scheduler-0.17.0b2/grain_scheduler.egg-info/requires.txt
--rw-r--r--   0 zhar     (13053) pl        (1102)       12 2022-10-19 18:20:16.000000 grain-scheduler-0.17.0b2/grain_scheduler.egg-info/top_level.txt
--rw-r--r--   0 zhar     (13053) pl        (1102)       38 2022-10-19 18:20:16.131111 grain-scheduler-0.17.0b2/setup.cfg
--rw-r--r--   0 zhar     (13053) pl        (1102)     2045 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b2/setup.py
+drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-11-09 23:45:11.034601 grain-scheduler-0.17.0b3/
+-rw-r--r--   0 zhar     (13053) pl        (1102)     1071 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/LICENSE
+-rw-r--r--   0 zhar     (13053) pl        (1102)     3787 2022-11-09 23:45:11.034601 grain-scheduler-0.17.0b3/PKG-INFO
+-rw-r--r--   0 zhar     (13053) pl        (1102)     2968 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/README.md
+drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-11-09 23:45:10.933935 grain-scheduler-0.17.0b3/bench/
+-rw-r--r--   0 zhar     (13053) pl        (1102)      318 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/bench/__init__.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     1115 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/bench/test_combine.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)      989 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/bench/test_delayed.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)      574 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/bench/test_head.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     2208 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/bench/test_worker.py
+drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-11-09 23:45:11.019510 grain-scheduler-0.17.0b3/grain/
+-rw-r--r--   0 zhar     (13053) pl        (1102)      209 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/__init__.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)       25 2022-11-09 23:22:01.000000 grain-scheduler-0.17.0b3/grain/_version.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     7513 2022-11-09 23:22:01.000000 grain-scheduler-0.17.0b3/grain/cli.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     6429 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/combine.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     3792 2022-11-09 23:22:01.000000 grain-scheduler-0.17.0b3/grain/config.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     7175 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/conn.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     6407 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/conn2.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     1291 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/conn_msgp.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)      567 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/contextvar.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)    14827 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/delayed.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)    19488 2022-11-09 23:22:01.000000 grain-scheduler-0.17.0b3/grain/head.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     6929 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/pair.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     8778 2022-11-09 23:22:01.000000 grain-scheduler-0.17.0b3/grain/remote_exer.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     9432 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/resource.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     2679 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/stat.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     4532 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/subproc.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     1571 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/subproc_worker.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)      723 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/test_combine.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     1457 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/test_conn2.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     3228 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/test_delayed.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     3481 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/test_head.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     1877 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/test_pair.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     3851 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/test_resource.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)      829 2022-11-09 23:22:01.000000 grain-scheduler-0.17.0b3/grain/test_worker.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     7886 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/util.py
+-rw-r--r--   0 zhar     (13053) pl        (1102)     5633 2022-10-19 18:18:08.000000 grain-scheduler-0.17.0b3/grain/worker.py
+drwxr-xr-x   0 zhar     (13053) pl        (1102)        0 2022-11-09 23:45:11.031580 grain-scheduler-0.17.0b3/grain_scheduler.egg-info/
+-rw-r--r--   0 zhar     (13053) pl        (1102)     3787 2022-11-09 23:45:10.000000 grain-scheduler-0.17.0b3/grain_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 zhar     (13053) pl        (1102)      829 2022-11-09 23:45:10.000000 grain-scheduler-0.17.0b3/grain_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 zhar     (13053) pl        (1102)        1 2022-11-09 23:45:10.000000 grain-scheduler-0.17.0b3/grain_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 zhar     (13053) pl        (1102)       41 2022-11-09 23:45:10.000000 grain-scheduler-0.17.0b3/grain_scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 zhar     (13053) pl        (1102)      108 2022-11-09 23:45:10.000000 grain-scheduler-0.17.0b3/grain_scheduler.egg-info/requires.txt
+-rw-r--r--   0 zhar     (13053) pl        (1102)       12 2022-11-09 23:45:10.000000 grain-scheduler-0.17.0b3/grain_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 zhar     (13053) pl        (1102)       38 2022-11-09 23:45:11.035606 grain-scheduler-0.17.0b3/setup.cfg
+-rw-r--r--   0 zhar     (13053) pl        (1102)     2095 2022-11-09 23:22:01.000000 grain-scheduler-0.17.0b3/setup.py
```

### Comparing `grain-scheduler-0.17.0b2/LICENSE` & `grain-scheduler-0.17.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/PKG-INFO` & `grain-scheduler-0.17.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: grain-scheduler
-Version: 0.17.0b2
+Version: 0.17.0b3
 Summary: A scheduler for resource-aware parallel computing on clusters.
 Home-page: https://github.com/Contextualist/grain
 Author: Harry Zhang
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Trio
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Grain
```

### Comparing `grain-scheduler-0.17.0b2/README.md` & `grain-scheduler-0.17.0b3/README.md`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/bench/test_combine.py` & `grain-scheduler-0.17.0b3/bench/test_combine.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/bench/test_delayed.py` & `grain-scheduler-0.17.0b3/bench/test_delayed.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/bench/test_head.py` & `grain-scheduler-0.17.0b3/bench/test_head.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/bench/test_worker.py` & `grain-scheduler-0.17.0b3/bench/test_worker.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/cli.py` & `grain-scheduler-0.17.0b3/grain/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,20 +121,20 @@
     def _wrapped(config, *args, **kwargs):
         return fn(conf=load_conf(config, conf_mode), *args, **kwargs)
     return _wrapped
 
 def gen_script(conf, is_worker=False):
     scriptc = conf.script
     rmem = int(scriptc.memory/15*14)
-    scriptc.walltime, rwalltime = norm_wtime(scriptc.walltime)
     if is_worker:
         res = dict()
         if scriptc.cores or rmem:
             res["Node"] = dict(N=scriptc.cores, M=rmem)
-        if rwalltime:
+        if scriptc.walltime:
+            scriptc.walltime, rwalltime = norm_wtime(scriptc.walltime)
             res["WTime"] = dict(T=rwalltime, countdown=True)
         scriptc.res_str = json.dumps(dict(
             **res,
             **conf.res,
         ))
     scriptc.setup, scriptc.cleanup = eval_defer(scriptc.setup_cleanup)
     if conf.custom_system:
```

### Comparing `grain-scheduler-0.17.0b2/grain/combine.py` & `grain-scheduler-0.17.0b3/grain/combine.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/config.py` & `grain-scheduler-0.17.0b3/grain/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,29 +16,34 @@
 @define(slots=False)
 class Script:
     cores:         int = 0
     memory:        int = 0
     setup_cleanup: str = ""
     shebang:       str = "#!/bin/bash"
     queue:         str = "''"
-    walltime:      str = "12:00:00"
+    walltime:      str = ""
     extra_args:    List[str] = Factory(list)
 
 @define
 class CustomSystem:
     submit_cmd: str
     directory:  str
     template:   str
 
 @define
 class Config:
     system:        str = ""
     script:        Script = Factory(Script)
     contextmod:    str = ""
     custom_system: Optional[CustomSystem] = None
+    address:       str = ""
+    def __attrs_post_init__(self):
+        if not self.address:
+            (_local_share := Path.home()/".local/share").mkdir(mode=0o755, parents=True, exist_ok=True)
+            self.address = f"edge://{_local_share}/edge-file-default"
 
 @define
 class Gnaw:
     enabled:    bool = True
     log_file:   str = ""
     max_conn:   int = 8
     idle_quit:  str = "30m"
@@ -46,42 +51,44 @@
     extra_args: List[str] = Factory(list)
 
 @define
 class Head(Config):
     name:          str = "grain_head"
     main_log_file: str = "/dev/null"
     log_file:      str = ""
-    listen:        str = "tcp://:4242"
+    listen:        str = ""
     cmd:           str = ""
     gnaw:          Gnaw = Factory(Gnaw)
+    def __attrs_post_init__(self):
+        Config.__attrs_post_init__(self)
+        if not self.listen:
+            self.listen = self.address
 
 @define
 class Worker(Config):
     specialized_type: str = ""
     name:             str = "w{{HHMMSS}}"
     log_file:         str = "w{{HHMMSS}}.log"
-    dial:             str = "UNSET"
+    dial:             str = ""
     cli_dial:         str = ""
     res:              Dict[str, Any] = Factory(dict)
     def __attrs_post_init__(self):
-        if self.dial == "UNSET":
-            raise ValueError("Config `worker.dial` is not set")
+        Config.__attrs_post_init__(self)
+        if not self.dial:
+            self.dial = self.address
         if not self.cli_dial:
             self.cli_dial = self.dial
 
 @define
 class GenericConfig:
     head:   Head
     worker: Worker
 
 _loose_filler = dict(
-    system="",
     head=dict(gnaw=dict(enabled=False)), # disable gnaw for test purpose
-    worker=dict(dial=""),
-    script=dict(cores=0, memory=0, setup_cleanup=""),
 )
 
 def ChainMapNested(d0, d1):
     for k in set(d0.keys()) & set(d1.keys()):
         if type(d0[k]) is dict and type(d1[k]) is dict:
             d0[k] = ChainMapNested(d0[k], d1[k])
     return ChainMap(d0, d1)
@@ -96,14 +103,16 @@
             config_s = Path(config).read_bytes().decode() if type(config) is str else config.read()
             conf = tomllib.loads(config_s)
         except FileNotFoundError:
             logger.error(f"Cannot find Grain config file {config!r}")
             exit(1)
         if type(config) is StringIO: # internal config fragment
             conf = ChainMap(conf, _loose_filler)
+    conf.setdefault('head', {})
+    conf.setdefault('worker', {})
     if mode == 'worker':
         return cattr.structure(ChainMapNested(conf['worker'], conf), Worker)
     elif mode == 'head':
         return cattr.structure(ChainMapNested(conf['head'], conf), Head)
     return GenericConfig(
         worker=cattr.structure(ChainMapNested(conf['worker'], conf), Worker),
         head=cattr.structure(ChainMapNested(conf['head'], conf), Head),
```

### Comparing `grain-scheduler-0.17.0b2/grain/conn.py` & `grain-scheduler-0.17.0b3/grain/conn.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/conn2.py` & `grain-scheduler-0.17.0b3/grain/conn2.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/conn_msgp.py` & `grain-scheduler-0.17.0b3/grain/conn_msgp.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/contextvar.py` & `grain-scheduler-0.17.0b3/grain/contextvar.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/delayed.py` & `grain-scheduler-0.17.0b3/grain/delayed.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/head.py` & `grain-scheduler-0.17.0b3/grain/head.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fnmatch import fnmatchcase
 import logging
 logger = logging.getLogger(__name__)
 
 from .contextvar import GVAR
 from .util import timeblock, pickle_dumps, pickle_loads, WaitGroup, nullacontext, optional_cm, make_prependable, load_contextmod, load_mod, as_daemon
 from .resource import Resource, ZERO, Reject
-from .pair import SocketChannel, SocketChannelAcceptor
+from .pair import SocketChannel, SocketChannelAcceptor, notify
 from .subproc import subprocess_pool_daemon, BrokenSubprocessError
 from .stat import log_event, log_timestart, log_timeend, stat_logger, ls_worker_res, reg_probe, collect_probe
 
 FULL_HEALTH = 3
 STATSPAN = 15 # minutes
 HEARTBEAT_INTERVAL, HEARTBEAT_TOLERANCE = 10, 3 # 10s * 3
 
@@ -239,32 +239,14 @@
         async with self.cond_res:
             for _,w in self._match_workers(pattern):
                 if type(w.res) is Reject: continue
                 logger.info(f"worker {w.name} is going to leave")
                 w.res = Reject(w.res)
                 self._n.start_soon(_wait_n_unreg, w)
 
-    async def backendless_sworker_manager(self, task_status=trio.TASK_STATUS_IGNORED):
-        registered_stype = set()
-        async with trio.open_nursery() as self.backendless_sworker_n:
-            for sw_conf in self.sworker_config:
-                stype = sw_conf.specialized_type
-                registered_stype.add(stype)
-                sw_mod = load_mod(stype)
-                if not sw_mod.GRAIN_SWORKER_CONFIG.get("BACKENDLESS", False):
-                    continue
-                sw_info = await self.backendless_sworker_n.start(as_daemon, sw_mod.grain_run_sworker())
-                res = Resource.from_dict({
-                    'Node': dict(N=sw_conf.script.cores, M=sw_conf.script.memory),
-                    'WTime': dict(T=sw_conf.script.walltime),
-                    **sw_conf.res,
-                })
-                self.pool.append(GrainSpecializedRemote(sw_info.pop("name"), res, None, dict(_stype=stype, **sw_info)))
-            task_status.started(registered_stype)
-
     async def worker_manager(self, registered_stype, task_status=trio.TASK_STATUS_IGNORED):
         async with trio.open_nursery() as _n, \
                    SocketChannelAcceptor(self.listen_addr, _n=_n) as self.soacceptor:
             for w in self.pool:
                 await w.connect(_n)
             task_status.started()
             async for _c in self.soacceptor:
@@ -300,15 +282,18 @@
                     elif cmd == "TRM": # graceful termination
                         pattern = msg['name']
                         await self.terminate(pattern)
                     else:
                         logger.warning(f"worker manager received unknown command {cmd} from {_c.host}")
 
     async def __aenter__(self):
-        registered_stype = await self._n.start(self.backendless_sworker_manager)
+        registered_stype, _, self.backendless_sworker_n = await self._n.start(
+            backendless_sworker_manager,
+            self.sworker_config, self.listen_addr,
+        )
         await self._n.start(self.worker_manager, registered_stype)
 
     async def aclose(self):
         with trio.move_on_after(10) as cleanup_scope: # 10s cleanup
             cleanup_scope.shield = True
             self.backendless_sworker_n.cancel_scope.cancel()
             for w in self.pool:
@@ -316,14 +301,44 @@
             await self.soacceptor.aclose()
 
     async def __aexit__(self, *exc):
         await self.aclose()
         return False
 
 
+async def backendless_sworker_manager(sworker_config, manager_api, task_status=trio.TASK_STATUS_IGNORED):
+    registered_stype = set()
+    backendless_stype = set()
+    async with trio.open_nursery() as backendless_sworker_n:
+        for sw_conf in sworker_config:
+            stype = sw_conf.specialized_type
+            registered_stype.add(stype)
+            sw_mod = load_mod(stype)
+            if not sw_mod.GRAIN_SWORKER_CONFIG.get("BACKENDLESS", False):
+                continue
+            backendless_stype.add(stype)
+            # Backendless sworker's `grain_run_sworker` should be a trivial context for returning `sw_info`
+            sw_info = await backendless_sworker_n.start(as_daemon, sw_mod.grain_run_sworker())
+            resd = dict()
+            if sw_conf.script.cores or sw_conf.script.memory:
+                resd["Node"] = dict(N=sw_conf.script.cores, M=sw_conf.script.memory)
+            if sw_conf.script.walltime:
+                resd["WTime"] = dict(T=sw_conf.script.walltime, countdown=True)
+            res = Resource.from_dict({
+                **resd,
+                **sw_conf.res,
+            })
+            await notify(
+                manager_api,
+                dict(cmd="SRG", name=sw_info.pop("name"), res=res, obj=dict(_stype=stype, **sw_info)),
+                seg=True,
+            )
+        task_status.started((registered_stype, backendless_stype, backendless_sworker_n))
+
+
 class GrainExecutor:
     """There are two ways to use GrainExecutor: sync and async:
     sync: TODO
     async: TODO
     """
     def __init__(
         self,
```

### Comparing `grain-scheduler-0.17.0b2/grain/pair.py` & `grain-scheduler-0.17.0b3/grain/pair.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/remote_exer.py` & `grain-scheduler-0.17.0b3/grain/remote_exer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import trio
 import psutil
 
 from .conn_msgp import send_packet
 from .pair import SocketChannel
-from .head import GrainSpecializedRemote
+from .head import GrainSpecializedRemote, backendless_sworker_manager
 from .util import WaitGroup, pickle_dumps, pickle_loads, timeblock
 
 import secrets
 from functools import partial
 from math import inf as INFIN
 import getpass
 import argparse
@@ -26,24 +26,25 @@
         executor is a managed daemon process.
     """
     def __init__(self, _n=None, config=None, gnaw=DAEMON, name="", prioritized=False, sworker_config=(), **kwargs):
         if kwargs:
             logger.warning(f"kwargs {kwargs} are ignored")
         self.gnaw = gnaw
         self.name = name + ("-p" if prioritized else "")
+        self.sworker_config = sworker_config
         self.push_job, self.pull_job = trio.open_memory_channel(INFIN)
         self.push_result, self.resultq = trio.open_memory_channel(INFIN)
         self.jobn = 0
         assert _n is not None
         self._n = _n
         self._c = None
         self._cs = None
         self._wg = WaitGroup() # track the entire lifetime of each job
+        self.listen = config.listen
         if gnaw is DAEMON:
-            self.listen = config.listen
             self.gnaw_conf = config.gnaw
         self.side_c = None
         self.fnd = {}
 
 
     def submit(self, res, fn, *args, **kwargs):
         tid = self.jobn = self.jobn+1
@@ -102,15 +103,17 @@
                     raise RuntimeError("Gnaw took too long to start")
         with timeblock("all jobs"):
             async with SocketChannel(self.gnaw, dial=True, _n=self._n) as self._c, \
                        self.push_result:
                 # handshake
                 await send_packet(self._c._so, dict(cmd="chTaskResult", name=self.name))
                 hsmsg = await self._c.receive()
-                await self._n.start(self.run_sworker_clients, hsmsg)
+                assert hsmsg["cmd"] == "hsSynAck"
+                # self.run_sworker_clients will create chApprovalRStatus and start all required clients before reporting started
+                await self._n.start(self.run_sworker_clients, hsmsg["name"])
                 self._n.start_soon(self._sender)
                 task_status.started()
                 async for x in self._c:
                     if x['exception']: # display exception
                         tb, exp = pickle_loads(x['result'])
                         logger.error(f"Exception from task: {x['exception']}: {exp}\n{tb}")
                         continue
@@ -122,21 +125,22 @@
         await self._n.start(self.run)
         return self
     async def __aexit__(self, *exc):
         if any(exc):
             return False
         self._n.start_soon(self.sealer)
 
-    # TODO: backendless sworker
-    async def run_sworker_clients(self, hsmsg, task_status=trio.TASK_STATUS_IGNORED):
-        assert hsmsg["cmd"] == "hsSynAck"
+    async def run_sworker_clients(self, dock_id, task_status=trio.TASK_STATUS_IGNORED):
         pool = dict()
+        started = False
 
         async def _reg(name, kwargs):
             logger.info(f"client for specialized worker {name} started")
+            if backendless_stype:
+                backendless_stype.discard(kwargs.get("_stype", None))
             # We don't need to manage resource or connection here
             sr = GrainSpecializedRemote(name, None, None, kwargs)
             await sr.connect(_n)
             pool[name] = sr
         async def _unreg(name):
             if (sr := pool.pop(name, None)) is not None:
                 await sr.aclose()
@@ -150,26 +154,35 @@
                 del self.fnd[tid]
             else:
                 # TODO: buffered exp
                 exp, tb = r
                 logger.error(f"Exception from task: {exp}\n{tb}")
 
         async with trio.open_nursery() as _n:
-            for name, kwargs in hsmsg["obj"].items():
-                await _reg(name, kwargs)
+            _, backendless_stype, _backendless_sworker_n = await _n.start(backendless_sworker_manager, self.sworker_config, self.listen)
             async with SocketChannel(self.gnaw, dial=True, _n=_n) as self.side_c:
-                await send_packet(self.side_c._so, dict(cmd="chApprovalRStatus", name=str(hsmsg["name"])))
-                assert (await self.side_c.receive())["cmd"] == "hsAck"
-                task_status.started()
+                await send_packet(self.side_c._so, dict(cmd="chApprovalRStatus", name=dock_id))
+                hsmsg = await self.side_c.receive()
+                assert hsmsg["cmd"] == "hsAck"
+                for name, kwargs in hsmsg["obj"].items():
+                    await _reg(name, kwargs)
+                if not started and not backendless_stype:
+                    started = True
+                    task_status.started()
+                # otherwise there is any pending backendless sworker, wait until registered
                 async for x in self.side_c:
                     cmd = x.get("cmd", "")
                     if cmd == "":
                         tid, res, client_name = x["tid"], x["res"], x["func"]
                         _n.start_soon(_run_task, tid, res, client_name)
                     elif cmd == "pushSWorker":
                         await _reg(x["name"], x["obj"])
+                        if not started and not backendless_stype:
+                            started = True
+                            task_status.started()
                     elif cmd == "quitSWorker":
                         await _unreg(x["name"])
                     else:
                         logger.warning(f"specialized worker client manager received unknown command {cmd}")
             for sr in pool.values():
                 await sr.aclose()
+            _backendless_sworker_n.cancel_scope.cancel()
```

### Comparing `grain-scheduler-0.17.0b2/grain/resource.py` & `grain-scheduler-0.17.0b3/grain/resource.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/stat.py` & `grain-scheduler-0.17.0b3/grain/stat.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/subproc.py` & `grain-scheduler-0.17.0b3/grain/subproc.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/subproc_worker.py` & `grain-scheduler-0.17.0b3/grain/subproc_worker.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/test_combine.py` & `grain-scheduler-0.17.0b3/grain/test_combine.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/test_conn2.py` & `grain-scheduler-0.17.0b3/grain/test_conn2.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/test_delayed.py` & `grain-scheduler-0.17.0b3/grain/test_delayed.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/test_head.py` & `grain-scheduler-0.17.0b3/grain/test_head.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/test_pair.py` & `grain-scheduler-0.17.0b3/grain/test_pair.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/test_resource.py` & `grain-scheduler-0.17.0b3/grain/test_resource.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/test_worker.py` & `grain-scheduler-0.17.0b3/grain/test_worker.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return x+1
 
 async def test_worker():
     N = 3
     async with trio.open_nursery() as _n, \
                GrainExecutor(_n=_n, nolocal=True) as exer:
         GVAR.instance = "test-worker-A"
-        _n.start_soon(grain_worker, Memory(4)&WTime(T=10,countdown=True), "tcp://localhost:4242")
+        _n.start_soon(grain_worker, Memory(4)&WTime(T=10,countdown=True), exer.mgr.listen_addr)
         for i in range(N):
             exer.submit(Memory(2), addone, i)
     results = [None] * N
     async with exer.resultq:
         async for i, r in exer.resultq:
             results[i-1] = r
     assert results == list(range(1,N+1))
```

### Comparing `grain-scheduler-0.17.0b2/grain/util.py` & `grain-scheduler-0.17.0b3/grain/util.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain/worker.py` & `grain-scheduler-0.17.0b3/grain/worker.py`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/grain_scheduler.egg-info/PKG-INFO` & `grain-scheduler-0.17.0b3/grain_scheduler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: grain-scheduler
-Version: 0.17.0b2
+Version: 0.17.0b3
 Summary: A scheduler for resource-aware parallel computing on clusters.
 Home-page: https://github.com/Contextualist/grain
 Author: Harry Zhang
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Trio
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: System :: Distributed Computing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Grain
```

### Comparing `grain-scheduler-0.17.0b2/grain_scheduler.egg-info/SOURCES.txt` & `grain-scheduler-0.17.0b3/grain_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grain-scheduler-0.17.0b2/setup.py` & `grain-scheduler-0.17.0b3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,11 +61,12 @@
         "Framework :: Trio",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: System :: Distributed Computing",
     ],
 )
```

