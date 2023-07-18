# Comparing `tmp/neon-enclosure-1.5.2a1.tar.gz` & `tmp/neon-enclosure-1.5.2a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-enclosure-1.5.2a1.tar", last modified: Tue Jun 27 18:49:09 2023, max compression
+gzip compressed data, was "neon-enclosure-1.5.2a2.tar", last modified: Tue Jul 18 18:22:53 2023, max compression
```

## Comparing `neon-enclosure-1.5.2a1.tar` & `neon-enclosure-1.5.2a2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:49:09.001495 neon-enclosure-1.5.2a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-27 18:49:09.001495 neon-enclosure-1.5.2a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:49:08.997495 neon-enclosure-1.5.2a1/neon_enclosure/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/neon_enclosure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/neon_enclosure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:49:09.001495 neon-enclosure-1.5.2a1/neon_enclosure/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/neon_enclosure/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/neon_enclosure/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/neon_enclosure/admin/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/neon_enclosure/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/neon_enclosure/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:49:08.997495 neon-enclosure-1.5.2a1/neon_enclosure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-27 18:49:08.000000 neon-enclosure-1.5.2a1/neon_enclosure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-27 18:49:08.000000 neon-enclosure-1.5.2a1/neon_enclosure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:49:08.000000 neon-enclosure-1.5.2a1/neon_enclosure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-27 18:49:08.000000 neon-enclosure-1.5.2a1/neon_enclosure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-27 18:49:08.000000 neon-enclosure-1.5.2a1/neon_enclosure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-27 18:49:08.000000 neon-enclosure-1.5.2a1/neon_enclosure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:49:09.001495 neon-enclosure-1.5.2a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-27 18:49:05.000000 neon-enclosure-1.5.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:53.419732 neon-enclosure-1.5.2a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-18 18:22:53.419732 neon-enclosure-1.5.2a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:53.419732 neon-enclosure-1.5.2a2/neon_enclosure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/neon_enclosure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/neon_enclosure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:53.419732 neon-enclosure-1.5.2a2/neon_enclosure/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/neon_enclosure/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/neon_enclosure/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/neon_enclosure/admin/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/neon_enclosure/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/neon_enclosure/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:22:53.419732 neon-enclosure-1.5.2a2/neon_enclosure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-07-18 18:22:53.000000 neon-enclosure-1.5.2a2/neon_enclosure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-18 18:22:53.000000 neon-enclosure-1.5.2a2/neon_enclosure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:22:53.000000 neon-enclosure-1.5.2a2/neon_enclosure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 18:22:53.000000 neon-enclosure-1.5.2a2/neon_enclosure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-18 18:22:53.000000 neon-enclosure-1.5.2a2/neon_enclosure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 18:22:53.000000 neon-enclosure-1.5.2a2/neon_enclosure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:22:53.419732 neon-enclosure-1.5.2a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-18 18:22:49.000000 neon-enclosure-1.5.2a2/setup.py
```

### Comparing `neon-enclosure-1.5.2a1/LICENSE.md` & `neon-enclosure-1.5.2a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.5.2a1/PKG-INFO` & `neon-enclosure-1.5.2a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.5.2a1
+Version: 1.5.2a2
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.5.2a1/README.md` & `neon-enclosure-1.5.2a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure/__init__.py` & `neon-enclosure-1.5.2a2/neon_enclosure/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure/__main__.py` & `neon-enclosure-1.5.2a2/neon_enclosure/admin/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,30 +27,31 @@
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
 from neon_utils.signal_utils import init_signal_bus, init_signal_handlers
 from ovos_utils.messagebus import get_mycroft_bus
 from ovos_utils.process_utils import reset_sigint_handler
-from ovos_utils.log import LOG
 from ovos_utils import wait_for_exit_signal
+from ovos_utils.log import LOG
 
-from neon_enclosure.service import NeonHardwareAbstractionLayer
+from neon_enclosure.admin.service import NeonAdminHardwareAbstractionLayer
 
 
 def main(*args, **kwargs):
-    init_log(log_name="enclosure")
+    init_log(log_name="admin")
     malloc_running = start_malloc(stack_depth=4)
+
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
 
     init_signal_bus(bus)
     init_signal_handlers()
     reset_sigint_handler()
-    service = NeonHardwareAbstractionLayer(*args, **kwargs)
+    service = NeonAdminHardwareAbstractionLayer(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     if malloc_running:
         try:
             print_malloc(snapshot_malloc())
         except Exception as e:
             LOG.error(e)
```

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure/admin/__init__.py` & `neon-enclosure-1.5.2a2/neon_enclosure/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure/admin/__main__.py` & `neon-enclosure-1.5.2a2/neon_enclosure/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,36 +27,42 @@
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
 from neon_utils.signal_utils import init_signal_bus, init_signal_handlers
 from ovos_utils.messagebus import get_mycroft_bus
 from ovos_utils.process_utils import reset_sigint_handler
-from ovos_utils import wait_for_exit_signal
 from ovos_utils.log import LOG
+from ovos_utils import wait_for_exit_signal
 
-from neon_enclosure.admin.service import NeonAdminHardwareAbstractionLayer
+from neon_enclosure.service import NeonHardwareAbstractionLayer
 
 
 def main(*args, **kwargs):
-    init_log(log_name="admin")
+    init_log(log_name="enclosure")
     malloc_running = start_malloc(stack_depth=4)
-
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
 
     init_signal_bus(bus)
     init_signal_handlers()
     reset_sigint_handler()
-    service = NeonAdminHardwareAbstractionLayer(*args, **kwargs)
+    service = NeonHardwareAbstractionLayer(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     if malloc_running:
         try:
             print_malloc(snapshot_malloc())
         except Exception as e:
             LOG.error(e)
     service.shutdown()
 
 
+def deprecated_entrypoint():
+    from ovos_utils.log import log_deprecation
+    log_deprecation("Use `neon-enclosure run` in place of "
+                    "`neon_enclosure_client`", "2.0.0")
+    main()
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure/admin/service.py` & `neon-enclosure-1.5.2a2/neon_enclosure/admin/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure/cli.py` & `neon-enclosure-1.5.2a2/neon_enclosure/cli.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure/service.py` & `neon-enclosure-1.5.2a2/neon_enclosure/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.5.2a1/neon_enclosure.egg-info/PKG-INFO` & `neon-enclosure-1.5.2a2/neon_enclosure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.5.2a1
+Version: 1.5.2a2
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.5.2a1/setup.py` & `neon-enclosure-1.5.2a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,12 +62,13 @@
     author='Neongecko',
     author_email='developers@neon.ai',
     description="Neon Enclosure Module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         'console_scripts': [
-            'neon_enclosure_client=neon_enclosure.__main__:main',
+            # TODO: deprecate `neon_enclosure_client` entrypoint
+            'neon_enclosure_client=neon_enclosure.__main__:deprecated_entrypoint',
             'neon-enclosure=neon_enclosure.cli:neon_enclosure_cli'
         ]
     }
 )
```

