# Comparing `tmp/hoppr_nexus_bundler-0.4.9.tar.gz` & `tmp/hoppr_nexus_bundler-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_nexus_bundler-0.4.9.tar", max compression
+gzip compressed data, was "hoppr_nexus_bundler-0.5.0.tar", max compression
```

## Comparing `hoppr_nexus_bundler-0.4.9.tar` & `hoppr_nexus_bundler-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1084 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/LICENSE
--rw-r--r--   0        0        0     1694 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/README.md
--rw-r--r--   0        0        0       89 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/__init__.py
--rw-r--r--   0        0        0     7034 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/bundler.py
--rw-r--r--   0        0        0     1998 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/nexus_instance.py
--rw-r--r--   0        0        0        0 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/__init__.py
--rw-r--r--   0        0        0     4373 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/apt_publisher.py
--rw-r--r--   0        0        0     9569 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/base_publisher.py
--rw-r--r--   0        0        0     6265 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/docker_publisher.py
--rw-r--r--   0        0        0     2278 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/git_publisher.py
--rw-r--r--   0        0        0      833 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/helm_publisher.py
--rw-r--r--   0        0        0     1873 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/maven_publisher.py
--rw-r--r--   0        0        0        0 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/py.typed
--rw-r--r--   0        0        0      832 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/pypi_publisher.py
--rw-r--r--   0        0        0     1861 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/raw_publisher.py
--rw-r--r--   0        0        0     5741 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/yum_publisher.py
--rw-r--r--   0        0        0        0 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/nexus_bundler/py.typed
--rw-r--r--   0        0        0     1164 2023-04-26 20:09:28.000000 hoppr_nexus_bundler-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     2637 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1694 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/README.md
+-rw-r--r--   0        0        0       89 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/__init__.py
+-rw-r--r--   0        0        0     7356 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/bundler.py
+-rw-r--r--   0        0        0     1998 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/nexus_instance.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/__init__.py
+-rw-r--r--   0        0        0     4373 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/apt_publisher.py
+-rw-r--r--   0        0        0     9569 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/base_publisher.py
+-rw-r--r--   0        0        0     6485 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/docker_publisher.py
+-rw-r--r--   0        0        0     2278 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/git_publisher.py
+-rw-r--r--   0        0        0      833 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/helm_publisher.py
+-rw-r--r--   0        0        0     1873 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/maven_publisher.py
+-rw-r--r--   0        0        0      859 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/npm_publisher.py
+-rw-r--r--   0        0        0      871 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/nuget_publisher.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/py.typed
+-rw-r--r--   0        0        0      832 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/pypi_publisher.py
+-rw-r--r--   0        0        0     1861 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/raw_publisher.py
+-rw-r--r--   0        0        0     5741 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/yum_publisher.py
+-rw-r--r--   0        0        0        0 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/nexus_bundler/py.typed
+-rw-r--r--   0        0        0     1182 2023-07-18 16:05:08.000000 hoppr_nexus_bundler-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2676 1970-01-01 00:00:00.000000 hoppr_nexus_bundler-0.5.0/PKG-INFO
```

### Comparing `hoppr_nexus_bundler-0.4.9/LICENSE` & `hoppr_nexus_bundler-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/README.md` & `hoppr_nexus_bundler-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/bundler.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/bundler.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from nexus_bundler.publishers.base_publisher import Publisher
 from nexus_bundler.publishers.maven_publisher import MavenPublisher
 from nexus_bundler.publishers.git_publisher import GitPublisher
 from nexus_bundler.publishers.raw_publisher import RawPublisher
 from nexus_bundler.publishers.pypi_publisher import PypiPublisher
 from nexus_bundler.publishers.helm_publisher import HelmPublisher
 from nexus_bundler.publishers.docker_publisher import DockerPublisher
+from nexus_bundler.publishers.nuget_publisher import NugetPublisher
+from nexus_bundler.publishers.npm_publisher import NpmPublisher
 from nexus_bundler.nexus_instance import NexusInstance
 from nexus_bundler.publishers.yum_publisher import YumPublisher
 
 
 def _publish(publisher: Publisher, path: Path) -> Result:
     pub_instance = publisher.__class__(
         publisher.nexus_instance, publisher.context, publisher.config
@@ -119,14 +121,18 @@
                 publisher = retrieve_publisher("helm", HelmPublisher)
             case "docker":
                 publisher = retrieve_publisher("docker", DockerPublisher)
             case "rpm" | "yum":
                 publisher = retrieve_publisher("yum", YumPublisher)
             case "deb":
                 publisher = retrieve_publisher("apt", AptPublisher)
+            case "nuget":
+                publisher = retrieve_publisher("nuget", NugetPublisher)
+            case "npm":
+                publisher = retrieve_publisher("npm", NpmPublisher)
 
         if publisher is None:
             raise HopprPluginError(
                 f"No Nexus Publisher defined for purl type {purl_type}"
             )
 
         return publisher
```

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/nexus_instance.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/nexus_instance.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/apt_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/apt_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/base_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/base_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/docker_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/docker_publisher.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 Nexus publisher for docker artifacts
 """
 import json
-from pathlib import Path
 import re
+
+from pathlib import Path
 from typing import Any, Dict
+
 import requests
 
-from hoppr import HopprContext, Result, hoppr_rerunner
+from hoppr import HopprContext, Result, __version__, hoppr_rerunner
 from hoppr.exceptions import HopprError
+from semver.version import Version
 
-from nexus_bundler.publishers.base_publisher import Publisher
 from nexus_bundler.nexus_instance import NexusInstance
+from nexus_bundler.publishers.base_publisher import Publisher
 
 
 class DockerPublisher(Publisher):
     """
     Nexus publisher for docker artifacts
     """
 
@@ -23,48 +26,51 @@
     required_tools = ["skopeo"]
 
     def __init__(
         self, nexus_instance: NexusInstance, context: HopprContext, config: Any = None
     ) -> None:
         super().__init__(nexus_instance, context, config)
 
-        if self.config is not None:
-            if "skopeo_command" in self.config:
-                self.required_tools = [self.config["skopeo_command"]]
+        if self.config is not None and "skopeo_command" in self.config:
+            self.required_tools = [self.config["skopeo_command"]]
 
     @hoppr_rerunner
     def push_artifact(self, path: Path) -> Result:
         """
         Publishes the artifact at the specified path to Nexus
         """
 
         path_from_root = path.absolute().relative_to(self.root_dir)
         dest = "/".join(path_from_root.parts[2:])
         docker_url = re.sub(
             r"https?://", "docker://", str(self.nexus_instance.docker_url)
         )
-        dest = docker_url + re.sub(r"(.*)_(.*)", r"\1:\2", dest)
+
+        hoppr_version = Version.parse(__version__.removeprefix("v"))
+        if hoppr_version < Version.parse("1.8.6"):
+            dest = docker_url + re.sub(r"(.*)_(.*)", r"\1:\2", dest)
+        else:
+            dest = docker_url + re.sub(r"(.*)@(.*)", r"\1:\2", dest)
+
         src = f"docker-archive:{path}"
 
         command = [
             self.required_tools[0],
             "copy",
             "--dest-creds",
-            self.nexus_instance.userid + ":" + self.nexus_instance.password,
+            f"{self.nexus_instance.userid}:{self.nexus_instance.password}",
         ]
 
         if (
             re.match("^http://", str(self.nexus_instance.docker_url))
             or self.nexus_instance.force_http
         ):
             command.append("--dest-tls-verify=false")
 
-        command.append(src)
-        command.append(dest)
-
+        command.extend((src, dest))
         proc = self.run_command(command, [self.nexus_instance.password])
 
         if proc.returncode != 0:
             msg = (
                 f"Skopeo failed to copy docker image to {dest}, "
                 + f"return_code={proc.returncode}"
             )
```

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/git_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/git_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/helm_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/helm_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/maven_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/maven_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/pypi_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/pypi_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/raw_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/raw_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/nexus_bundler/publishers/yum_publisher.py` & `hoppr_nexus_bundler-0.5.0/nexus_bundler/publishers/yum_publisher.py`

 * *Files identical despite different names*

### Comparing `hoppr_nexus_bundler-0.4.9/pyproject.toml` & `hoppr_nexus_bundler-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr_nexus_bundler"
-version = "0.4.9"
+version = "0.5.0"
 description = "Plug-in for Hoppr to bundle artifacts into a Nexus Repository"
 authors = ["LMCO Open Source <open.source@lmco.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hoppr.dev/"
 repository = "https://gitlab.com/-/ide/project/lmco/hoppr/plugins/hoppr-nexus-bundler"
 
@@ -25,15 +25,16 @@
 packages = [
     { include = "nexus_bundler" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-hoppr = "^1.8.0"
+hoppr = "^1.9.0"
+semver = "^3.0.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 pylint = "^2.14.4"
 mypy = "^0.961"
 coverage = "^7.0.0"
 pytest = "^7.1.2"
```

### Comparing `hoppr_nexus_bundler-0.4.9/PKG-INFO` & `hoppr_nexus_bundler-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-nexus-bundler
-Version: 0.4.9
+Version: 0.5.0
 Summary: Plug-in for Hoppr to bundle artifacts into a Nexus Repository
 Home-page: https://hoppr.dev/
 License: MIT
 Keywords: hoppr,plugin,nexus
 Author: LMCO Open Source
 Author-email: open.source@lmco.com
 Requires-Python: >=3.10,<4.0
@@ -13,15 +13,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Software Distribution
-Requires-Dist: hoppr (>=1.8.0,<2.0.0)
+Requires-Dist: hoppr (>=1.9.0,<2.0.0)
+Requires-Dist: semver (>=3.0.1,<4.0.0)
 Project-URL: Repository, https://gitlab.com/-/ide/project/lmco/hoppr/plugins/hoppr-nexus-bundler
 Description-Content-Type: text/markdown
 
 # Nexus Bundler for Hoppr
 
 The Nexus Bundler is a plug-in for [Hoppr](https://gitlab.com/lmco/hoppr/hoppr) to package the collected artifacts into an existing Nexus instance.
```

