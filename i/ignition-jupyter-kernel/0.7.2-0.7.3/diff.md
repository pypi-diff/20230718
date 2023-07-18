# Comparing `tmp/ignition_jupyter_kernel-0.7.2.tar.gz` & `tmp/ignition_jupyter_kernel-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignition_jupyter_kernel-0.7.2.tar", last modified: Tue Jul 18 00:40:18 2023, max compression
+gzip compressed data, was "ignition_jupyter_kernel-0.7.3.tar", last modified: Tue Jul 18 00:58:43 2023, max compression
```

## Comparing `ignition_jupyter_kernel-0.7.2.tar` & `ignition_jupyter_kernel-0.7.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 00:40:18.018153 ignition_jupyter_kernel-0.7.2/
--rw-rw-rw-   0        0        0    11558 2022-06-17 13:24:02.000000 ignition_jupyter_kernel-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     1132 2023-07-18 00:40:18.016163 ignition_jupyter_kernel-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-07-18 00:22:06.000000 ignition_jupyter_kernel-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 00:40:18.008152 ignition_jupyter_kernel-0.7.2/ignition_jupyter_kernel.egg-info/
--rw-rw-rw-   0        0        0     1132 2023-07-18 00:40:17.000000 ignition_jupyter_kernel-0.7.2/ignition_jupyter_kernel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-07-18 00:40:17.000000 ignition_jupyter_kernel-0.7.2/ignition_jupyter_kernel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 00:40:17.000000 ignition_jupyter_kernel-0.7.2/ignition_jupyter_kernel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      121 2023-07-18 00:40:17.000000 ignition_jupyter_kernel-0.7.2/ignition_jupyter_kernel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 00:40:17.000000 ignition_jupyter_kernel-0.7.2/ignition_jupyter_kernel.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 00:40:18.014154 ignition_jupyter_kernel-0.7.2/ignition_kernel/
--rw-rw-rw-   0        0        0       79 2023-07-18 00:22:13.000000 ignition_jupyter_kernel-0.7.2/ignition_kernel/__init__.py
--rw-rw-rw-   0        0        0    11224 2023-07-13 15:02:44.000000 ignition_jupyter_kernel-0.7.2/ignition_kernel/__main__.py
--rw-rw-rw-   0        0        0    14121 2023-07-13 14:07:20.000000 ignition_jupyter_kernel-0.7.2/ignition_kernel/provisioner.py
--rw-rw-rw-   0        0        0      941 2023-07-18 00:21:22.000000 ignition_jupyter_kernel-0.7.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 00:40:18.018153 ignition_jupyter_kernel-0.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 00:58:43.778968 ignition_jupyter_kernel-0.7.3/
+-rw-rw-rw-   0        0        0    11558 2022-06-17 13:24:02.000000 ignition_jupyter_kernel-0.7.3/LICENSE
+-rw-rw-rw-   0        0        0     1981 2023-07-18 00:58:43.777967 ignition_jupyter_kernel-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1321 2023-07-18 00:55:48.000000 ignition_jupyter_kernel-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 00:58:43.771968 ignition_jupyter_kernel-0.7.3/ignition_jupyter_kernel.egg-info/
+-rw-rw-rw-   0        0        0     1981 2023-07-18 00:58:43.000000 ignition_jupyter_kernel-0.7.3/ignition_jupyter_kernel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-07-18 00:58:43.000000 ignition_jupyter_kernel-0.7.3/ignition_jupyter_kernel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 00:58:43.000000 ignition_jupyter_kernel-0.7.3/ignition_jupyter_kernel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-07-18 00:58:43.000000 ignition_jupyter_kernel-0.7.3/ignition_jupyter_kernel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 00:58:43.000000 ignition_jupyter_kernel-0.7.3/ignition_jupyter_kernel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 00:58:43.776969 ignition_jupyter_kernel-0.7.3/ignition_kernel/
+-rw-rw-rw-   0        0        0       79 2023-07-18 00:55:58.000000 ignition_jupyter_kernel-0.7.3/ignition_kernel/__init__.py
+-rw-rw-rw-   0        0        0    11224 2023-07-13 15:02:44.000000 ignition_jupyter_kernel-0.7.3/ignition_kernel/__main__.py
+-rw-rw-rw-   0        0        0    14375 2023-07-18 00:51:20.000000 ignition_jupyter_kernel-0.7.3/ignition_kernel/provisioner.py
+-rw-rw-rw-   0        0        0      941 2023-07-18 00:52:33.000000 ignition_jupyter_kernel-0.7.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 00:58:43.778968 ignition_jupyter_kernel-0.7.3/setup.cfg
```

### Comparing `ignition_jupyter_kernel-0.7.2/LICENSE` & `ignition_jupyter_kernel-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ignition_jupyter_kernel-0.7.2/ignition_kernel/__main__.py` & `ignition_jupyter_kernel-0.7.3/ignition_kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `ignition_jupyter_kernel-0.7.2/ignition_kernel/provisioner.py` & `ignition_jupyter_kernel-0.7.3/ignition_kernel/provisioner.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
     for when the `ignition_kernel_id` is None because the kernel is torn down.
     """
 
 
     # defaults
     host_url: Union[str, Unicode] = Unicode(config=True)
     endpoint: Union[str, Unicode] = Unicode("system/webdev/jupyter/kernel", config=True)
+    username: Union[str, Unicode] = Unicode(config=True)
+    password: Union[str, Unicode] = Unicode("keyring", config=True)
+
     connection_info: KernelConnectionInfo = {}
 
     ignition_kernel_id: str = Unicode(None, allow_none=True)
 
     
     ## TODO: port caching for preventing messy race stuff
     # for compatibility with the usual usage
@@ -241,14 +244,15 @@
         start kernel sequence.
 
         Returns the (potentially updated) keyword arguments that are passed to
         :meth:`launch_kernel()`.
         """
 
         # grab the auth password from keyring
+        assert self.password == 'keyring', "Only keyring password storage is currently supported. At least, not plaintext."
         self._keyring_password = keyring.get_password("Jupyter-Kernel", self._keyring_identifier)
 
 
         # Kernel Manager will be generating the connection info
         # (TODO: At least for this PoC testing...)
         km = self.parent
         if km:
```

### Comparing `ignition_jupyter_kernel-0.7.2/pyproject.toml` & `ignition_jupyter_kernel-0.7.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools]
 packages = ["ignition_kernel"]
 
 
 [project]
 name = "ignition_jupyter_kernel"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
 	{ name="Andrew Geiger", email="andrew@corsosystems.com" },
 ]
 
 description = "Allow Jupyter to connect to a kernel running on a configured Ignition instance."
 readme = "README.md"
```

