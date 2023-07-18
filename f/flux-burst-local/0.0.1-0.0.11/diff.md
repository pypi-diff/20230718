# Comparing `tmp/flux-burst-local-0.0.1.tar.gz` & `tmp/flux-burst-local-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-local-0.0.1.tar", last modified: Sat Jul 15 03:16:52 2023, max compression
+gzip compressed data, was "flux-burst-local-0.0.11.tar", last modified: Tue Jul 18 06:30:44 2023, max compression
```

## Comparing `flux-burst-local-0.0.1.tar` & `flux-burst-local-0.0.11.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:16:52.142841 flux-burst-local-0.0.1/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-07-13 11:43:03.000000 flux-burst-local-0.0.1/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-07-13 11:43:03.000000 flux-burst-local-0.0.1/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      219 2023-07-13 11:43:58.000000 flux-burst-local-0.0.1/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-07-13 11:43:03.000000 flux-burst-local-0.0.1/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2096 2023-07-15 03:16:52.142841 flux-burst-local-0.0.1/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1247 2023-07-14 07:00:03.000000 flux-burst-local-0.0.1/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:16:52.142841 flux-burst-local-0.0.1/flux_burst_local.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2096 2023-07-15 03:16:52.000000 flux-burst-local-0.0.1/flux_burst_local.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      495 2023-07-15 03:16:52.000000 flux-burst-local-0.0.1/flux_burst_local.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-15 03:16:52.000000 flux-burst-local-0.0.1/flux_burst_local.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       64 2023-07-15 03:16:52.000000 flux-burst-local-0.0.1/flux_burst_local.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-14 04:18:59.000000 flux-burst-local-0.0.1/flux_burst_local.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       95 2023-07-15 03:16:52.000000 flux-burst-local-0.0.1/flux_burst_local.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       16 2023-07-15 03:16:52.000000 flux-burst-local-0.0.1/flux_burst_local.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:16:52.142841 flux-burst-local-0.0.1/fluxburst_local/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      900 2023-07-14 07:36:06.000000 flux-burst-local-0.0.1/fluxburst_local/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2055 2023-07-15 03:16:49.000000 flux-burst-local-0.0.1/fluxburst_local/flux.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11637 2023-07-15 03:16:49.000000 flux-burst-local-0.0.1/fluxburst_local/plugin.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1407 2023-07-15 00:05:07.000000 flux-burst-local-0.0.1/fluxburst_local/templates.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1122 2023-07-14 18:25:26.000000 flux-burst-local-0.0.1/fluxburst_local/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-07-13 11:43:03.000000 flux-burst-local-0.0.1/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      159 2023-07-15 03:16:52.142841 flux-burst-local-0.0.1/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3276 2023-07-14 07:36:06.000000 flux-burst-local-0.0.1/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:44.344816 flux-burst-local-0.0.11/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-07-13 11:43:03.000000 flux-burst-local-0.0.11/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-07-13 11:43:03.000000 flux-burst-local-0.0.11/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      219 2023-07-13 11:43:58.000000 flux-burst-local-0.0.11/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-07-13 11:43:03.000000 flux-burst-local-0.0.11/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2097 2023-07-18 06:30:44.344816 flux-burst-local-0.0.11/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1247 2023-07-14 07:00:03.000000 flux-burst-local-0.0.11/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:44.344816 flux-burst-local-0.0.11/flux_burst_local.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2097 2023-07-18 06:30:44.000000 flux-burst-local-0.0.11/flux_burst_local.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      495 2023-07-18 06:30:44.000000 flux-burst-local-0.0.11/flux_burst_local.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-18 06:30:44.000000 flux-burst-local-0.0.11/flux_burst_local.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       64 2023-07-18 06:30:44.000000 flux-burst-local-0.0.11/flux_burst_local.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-14 04:18:59.000000 flux-burst-local-0.0.11/flux_burst_local.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       95 2023-07-18 06:30:44.000000 flux-burst-local-0.0.11/flux_burst_local.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       16 2023-07-18 06:30:44.000000 flux-burst-local-0.0.11/flux_burst_local.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:44.344816 flux-burst-local-0.0.11/fluxburst_local/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      854 2023-07-18 06:30:40.000000 flux-burst-local-0.0.11/fluxburst_local/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2653 2023-07-18 06:30:40.000000 flux-burst-local-0.0.11/fluxburst_local/flux.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13020 2023-07-18 06:30:40.000000 flux-burst-local-0.0.11/fluxburst_local/plugin.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1407 2023-07-15 00:05:07.000000 flux-burst-local-0.0.11/fluxburst_local/templates.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1123 2023-07-18 06:30:40.000000 flux-burst-local-0.0.11/fluxburst_local/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-07-13 11:43:03.000000 flux-burst-local-0.0.11/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      159 2023-07-18 06:30:44.344816 flux-burst-local-0.0.11/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3276 2023-07-14 07:36:06.000000 flux-burst-local-0.0.11/setup.py
```

### Comparing `flux-burst-local-0.0.1/LICENSE` & `flux-burst-local-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-local-0.0.1/NOTICE` & `flux-burst-local-0.0.11/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-local-0.0.1/PKG-INFO` & `flux-burst-local-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-local
-Version: 0.0.1
+Version: 0.0.11
 Summary: A bursting plugin for Flux and Compute Engine on Google Cloud
 Home-page: https://github.com/converged-computing/flux-burst-local
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-local-0.0.1/README.md` & `flux-burst-local-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `flux-burst-local-0.0.1/flux_burst_local.egg-info/PKG-INFO` & `flux-burst-local-0.0.11/flux_burst_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst-local
-Version: 0.0.1
+Version: 0.0.11
 Summary: A bursting plugin for Flux and Compute Engine on Google Cloud
 Home-page: https://github.com/converged-computing/flux-burst-local
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: flux,flux-framework,workflow,example,plugin
```

### Comparing `flux-burst-local-0.0.1/fluxburst_local/__init__.py` & `flux-burst-local-0.0.11/fluxburst_local/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,13 @@
     Parse custom arguments and return the Burst client.
 
     We use this section to create (and enter) the initial
     FluxBurst local setup. If this is running on top of Flux,
     this means starting another flux instance with the resources.
     If SLURM we assume we are inside a SLURM allocation.
     """
-    from .plugin import FluxBurstLocal, FluxBurstSlurm, SlurmBurstParameters
+    from .plugin import BurstParameters, FluxBurstHPC
 
-    if isinstance(dataclass, SlurmBurstParameters):
-        # Set variables from slurm
-        FluxBurstSlurm.setup(dataclass)
-        return FluxBurstSlurm(dataclass, **kwargs)
-    return FluxBurstLocal(dataclass, **kwargs)
+    if not isinstance(dataclass, BurstParameters):
+        raise ValueError("Current support is only for BurstParameters")
+    FluxBurstHPC.setup(dataclass)
+    return FluxBurstHPC(dataclass, **kwargs)
```

### Comparing `flux-burst-local-0.0.1/fluxburst_local/flux.py` & `flux-burst-local-0.0.11/fluxburst_local/flux.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,17 +54,34 @@
     # If we weren't, we would add them via:
     # client.set_ordering()
     # client.set_selector()
 
     # Here is how we can see the jobs that are contenders to burst!
     # client.select_jobs()
 
+    # This isn't supported (or needed) for top level flux-burst yet, so
+    # we interact directly with the plugin
+    plugin = client.plugins["local"]
+
     # Continue running the burst until no more burstable
-    # This likely needs to be adjusted
     while True:
         print("Running burst...")
+
+        # This will hit the plugin->run to flux proxy to start brokers
         client.run_burst()
+
+        # This is a bit buggy - we have to wait for the brokers to start
+        time.sleep(10)
+
+        # Bursted job ids associated with brokers are here
+        if plugin.jobids:
+            # Ask client to wait for all jobs to be finished (in state cancel or fail)
+            client.wait_for_jobs()
+
+            # When they are done, we cleanup the jobs (and clear jobids
+            client.run_unburst()
+
         time.sleep(5)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `flux-burst-local-0.0.1/fluxburst_local/plugin.py` & `flux-burst-local-0.0.11/fluxburst_local/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     curve_cert: Optional[str] = None
     flux_root: Optional[str] = None
     config_dir: Optional[str] = None
     flux_uri: Optional[str] = None
 
     # Flux log level
     log_level: Optional[int] = 7
-    regenerate: bool = False
+    regenerate: bool = True
 
     # Custom flux user (defaults to running user)
     flux_user: Optional[str] = None
 
     @property
     def system_dir(self):
         return os.path.join(self.config_dir, "system")
@@ -54,14 +54,28 @@
     def lib_dir(self):
         return os.path.join(self.config_dir, "lib")
 
     @property
     def fluxcmd(self):
         return f"{self.flux_root}/bin/flux"
 
+    def set_hostnames(self):
+        """
+        Ensure we have hostnames from a variable or environment.
+        """
+        self.hostnames = (
+            self.hostnames
+            or os.environ.get("SLURM_JOB_HOSTLIST")
+            or os.environ.get("SLURM_NODELIST")
+        )
+        if not self.hostnames:
+            raise ValueError(
+                "The 'hostnames' parameter or environment variable SLURM_JOB_HOSTLIST must be defined."
+            )
+
     def generate_flux_config(self):
         """
         Generate a bursted broked config.
         """
         template = templates.system_toml
         system_toml = os.path.join(self.system_dir, "system.toml")
         if os.path.exists(system_toml) and not self.regenerate:
@@ -102,14 +116,18 @@
     def set_config_dir(self):
         """
         Setup the local config directory
 
         We also create paths for run, lib, and system.
         """
         self.config_dir = os.path.abspath(self.config_dir or utils.get_tmpdir())
+        if self.regenerate and os.path.exists(self.config_dir):
+            logger.info("Cleaning up previous config directory...")
+            shutil.rmtree(self.config_dir)
+
         for path in [self.lib_dir, self.run_dir, self.system_dir]:
             utils.mkdir_p(path)
 
     def write_curve_cert(self):
         """
         Ensure we have a curve cert string and write to file.
         """
@@ -149,41 +167,21 @@
             [self.fluxcmd, "R", "encode", "--hosts", self.hostnames, "--local"]
         )
         if res["return_code"] != 0:
             raise ValueError("Issue generating R")
         utils.write_file(res["message"], rpath)
 
 
-@dataclass
-class SlurmBurstParameters(BurstParameters):
-    """
-    Custom parameters for SLURM.
-
-    We can get the hostnames from the environment. This dataclass
-    is used to trigger getting the needed parameters from the environment.
-    """
-
-    def set_hostnames(self):
-        """
-        Ensure we have hostnames from a variable or environment.
-        """
-        self.hostnames = (
-            self.hostnames
-            or os.environ.get("SLURM_JOB_HOSTLIST")
-            or os.environ.get("SLURM_NODELIST")
-        )
-        if not self.hostnames:
-            raise ValueError(
-                "The 'hostnames' parameter or environment variable SLURM_JOB_HOSTLIST must be defined."
-            )
-
-
 class FluxBurstLocal(BurstPlugin):
     _param_dataclass = BurstParameters
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.jobids = []
+
     def run(self, request_burst=False, nodes=None, **kwargs):
         """
         Given some set of scheduled jobs, run bursting.
         """
         try:
             import flux
             import flux.resource
@@ -228,30 +226,71 @@
         logger.debug(f"{nodes_needed} are needed.")
 
         # Note that this assumes flux in the same install location, and the rank 0 of the second instance == rank 0 of the first
         # Aside from that, we let flux choose the nodes. We need to exclude the lead (the requires didn't parse well with spaces)
         command = [
             self.params.fluxcmd,
             "proxy",
+            "--force",
             self.params.flux_uri,
             self.params.fluxcmd,
             "submit",
             "-N",
             str(nodes_needed),
             # TODO need a way to specify this
             # '--requires=\"not rank:0\"',
             self.params.fluxcmd,
             "start",
             "--broker-opts",
             "--config",
             self.params.system_dir,
         ]
-        # This likely can be improved
         print(" ".join(command))
-        os.system(" ".join(command))
+        res = utils.run_command(command)
+
+        # Tell the user about any issues
+        if res["return_code"] != 0:
+            command = " ".join(command)
+            logger.warning(f'Issue running {command}: res["message"]')
+            return
+
+        # 'f3YXvFkgX\n'
+        jobid = res["message"].strip()
+        logger.debug(f"Adding jobid {jobid} to bursted proxy jobs.")
+        self.jobids.append(jobid)
+
+    def unburst(self):
+        """
+        Given a set of jobids that started brokers, cancel them.
+
+        This gets called by flux burst when the original job is determined
+        to be done.
+        """
+        if not self.jobids:
+            logger.debug("There are no jobs to unburst.")
+            return
+
+        command = [
+            self.params.fluxcmd,
+            "proxy",
+            "--force",
+            self.params.flux_uri,
+            self.params.fluxcmd,
+            "job",
+            "cancel",
+        ] + self.jobids
+        print(" ".join(command))
+        res = utils.run_command(command)
+
+        # Tell the user about any issues
+        if res["return_code"] != 0:
+            command = " ".join(command)
+            logger.warning(f'Issue running {command}: res["message"]')
+            return
+        self.jobids = []
 
     def validate_params(self):
         """
         Validate parameters provided as BurstParameters.
 
         This includes checking to see if we have an isolated burst,
         and if a script is provided for any boot script, ensuring that
@@ -285,26 +324,32 @@
             return True
 
         # Add to self.jobs and return True!
         self.jobs[job["id"]] = job
         return True
 
 
-class FluxBurstSlurm(FluxBurstLocal):
+class FluxBurstHPC(FluxBurstLocal):
     # Set our custom dataclass, otherwise empty
     _param_dataclass = BurstParameters
 
     @classmethod
     def setup(cls, dataclass):
         """
         Finish populating the dataclass with SLURM environment variables.
         """
         dataclass.validate()
         dataclass.set_hostnames()
         dataclass.set_config_dir()
+
+        # If we aren't regenerating, don't show this
+        if not dataclass.regenerate:
+            return
+
+        # Write configs
         dataclass.write_curve_cert()
         dataclass.write_resource_spec()
         dataclass.generate_flux_config()
 
         # Flux URI is required
         if not dataclass.flux_uri:
             raise ValueError(
```

### Comparing `flux-burst-local-0.0.1/fluxburst_local/templates.py` & `flux-burst-local-0.0.11/fluxburst_local/templates.py`

 * *Files identical despite different names*

### Comparing `flux-burst-local-0.0.1/fluxburst_local/version.py` & `flux-burst-local-0.0.11/fluxburst_local/version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.1"
+__version__ = "0.0.11"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst-local"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst-local"
 KEYWORDS = "flux, flux-framework, workflow, example, plugin"
 DESCRIPTION = "A bursting plugin for Flux and Compute Engine on Google Cloud"
 LICENSE = "LICENSE"
```

### Comparing `flux-burst-local-0.0.1/setup.py` & `flux-burst-local-0.0.11/setup.py`

 * *Files identical despite different names*

