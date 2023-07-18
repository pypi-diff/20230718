# Comparing `tmp/sdss_archon-0.9.0.tar.gz` & `tmp/sdss_archon-0.9.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_archon-0.9.0.tar", max compression
+gzip compressed data, was "sdss_archon-0.9.0b1.tar", max compression
```

## Comparing `sdss_archon-0.9.0.tar` & `sdss_archon-0.9.0b1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1504 2023-04-13 21:21:49.985286 sdss_archon-0.9.0/LICENSE.md
--rw-r--r--   0        0        0     4187 2023-04-13 21:21:49.985486 sdss_archon-0.9.0/README.md
--rw-r--r--   0        0        0      515 2023-04-13 21:21:49.985737 sdss_archon-0.9.0/archon/__init__.py
--rw-r--r--   0        0        0      351 2023-04-13 21:21:49.986025 sdss_archon-0.9.0/archon/actor/__init__.py
--rw-r--r--   0        0        0     7078 2023-04-13 21:21:49.986313 sdss_archon-0.9.0/archon/actor/actor.py
--rw-r--r--   0        0        0     1079 2023-04-13 21:21:49.986718 sdss_archon-0.9.0/archon/actor/commands/__init__.py
--rw-r--r--   0        0        0     3396 2023-04-13 21:21:49.987031 sdss_archon-0.9.0/archon/actor/commands/config.py
--rw-r--r--   0        0        0     1072 2023-04-13 21:21:49.987292 sdss_archon-0.9.0/archon/actor/commands/disconnect.py
--rw-r--r--   0        0        0     6649 2023-04-13 21:21:49.987530 sdss_archon-0.9.0/archon/actor/commands/expose.py
--rw-r--r--   0        0        0     1025 2023-04-13 21:21:49.987784 sdss_archon-0.9.0/archon/actor/commands/flush.py
--rw-r--r--   0        0        0     4039 2023-04-13 21:21:49.987939 sdss_archon-0.9.0/archon/actor/commands/frame.py
--rw-r--r--   0        0        0     5326 2023-04-13 21:21:49.988322 sdss_archon-0.9.0/archon/actor/commands/init.py
--rw-r--r--   0        0        0     2824 2023-04-13 21:21:49.988510 sdss_archon-0.9.0/archon/actor/commands/power.py
--rw-r--r--   0        0        0     1607 2023-04-13 21:21:49.988700 sdss_archon-0.9.0/archon/actor/commands/reconnect.py
--rw-r--r--   0        0        0      929 2023-04-13 21:21:49.989040 sdss_archon-0.9.0/archon/actor/commands/reset.py
--rw-r--r--   0        0        0     1713 2023-04-13 21:21:49.989308 sdss_archon-0.9.0/archon/actor/commands/status.py
--rw-r--r--   0        0        0      920 2023-04-13 21:21:49.989537 sdss_archon-0.9.0/archon/actor/commands/system.py
--rw-r--r--   0        0        0     1261 2023-04-13 21:21:49.989760 sdss_archon-0.9.0/archon/actor/commands/talk.py
--rw-r--r--   0        0        0     3150 2023-04-13 21:21:49.989972 sdss_archon-0.9.0/archon/actor/commands/window.py
--rw-r--r--   0        0        0    27832 2023-04-13 21:21:49.990294 sdss_archon-0.9.0/archon/actor/delegate.py
--rw-r--r--   0        0        0     5379 2023-04-13 21:21:49.990560 sdss_archon-0.9.0/archon/actor/tools.py
--rw-r--r--   0        0        0      587 2023-04-13 21:21:49.990850 sdss_archon-0.9.0/archon/controller/__init__.py
--rw-r--r--   0        0        0     7430 2023-04-13 21:21:49.991128 sdss_archon-0.9.0/archon/controller/command.py
--rw-r--r--   0        0        0    47092 2023-04-13 21:21:49.991579 sdss_archon-0.9.0/archon/controller/controller.py
--rw-r--r--   0        0        0     1334 2023-04-13 21:21:49.991811 sdss_archon-0.9.0/archon/controller/maskbits.py
--rw-r--r--   0        0        0      427 2023-04-13 21:21:49.992150 sdss_archon-0.9.0/archon/etc/archon.yml
--rw-r--r--   0        0        0     3191 2023-04-13 21:21:49.992349 sdss_archon-0.9.0/archon/etc/schema.json
--rw-r--r--   0        0        0     2078 2023-04-13 21:21:49.992613 sdss_archon-0.9.0/archon/exceptions.py
--rw-r--r--   0        0        0     3861 2023-04-13 21:21:49.992842 sdss_archon-0.9.0/archon/tools.py
--rw-r--r--   0        0        0     2375 2023-04-13 21:21:49.999972 sdss_archon-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5580 1970-01-01 00:00:00.000000 sdss_archon-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-03-10 18:16:19.653045 sdss_archon-0.9.0b1/LICENSE.md
+-rw-r--r--   0        0        0     4187 2023-03-10 18:16:19.734734 sdss_archon-0.9.0b1/README.md
+-rw-r--r--   0        0        0      515 2023-03-10 18:16:19.775521 sdss_archon-0.9.0b1/archon/__init__.py
+-rw-r--r--   0        0        0      351 2023-03-10 18:16:19.857788 sdss_archon-0.9.0b1/archon/actor/__init__.py
+-rw-r--r--   0        0        0     7078 2023-03-10 18:16:19.898989 sdss_archon-0.9.0b1/archon/actor/actor.py
+-rw-r--r--   0        0        0     1079 2023-03-10 18:16:19.980152 sdss_archon-0.9.0b1/archon/actor/commands/__init__.py
+-rw-r--r--   0        0        0     3396 2023-03-10 18:16:20.021530 sdss_archon-0.9.0b1/archon/actor/commands/config.py
+-rw-r--r--   0        0        0     1072 2023-03-10 18:16:20.102933 sdss_archon-0.9.0b1/archon/actor/commands/disconnect.py
+-rw-r--r--   0        0        0     6649 2023-03-10 18:16:20.143760 sdss_archon-0.9.0b1/archon/actor/commands/expose.py
+-rw-r--r--   0        0        0     1025 2023-03-10 18:16:20.224926 sdss_archon-0.9.0b1/archon/actor/commands/flush.py
+-rw-r--r--   0        0        0     4039 2023-03-10 18:16:20.265383 sdss_archon-0.9.0b1/archon/actor/commands/frame.py
+-rw-r--r--   0        0        0     5326 2023-03-10 18:16:20.346906 sdss_archon-0.9.0b1/archon/actor/commands/init.py
+-rw-r--r--   0        0        0     2824 2023-03-10 18:16:20.387852 sdss_archon-0.9.0b1/archon/actor/commands/power.py
+-rw-r--r--   0        0        0     1607 2023-03-10 18:16:20.469360 sdss_archon-0.9.0b1/archon/actor/commands/reconnect.py
+-rw-r--r--   0        0        0      929 2023-03-10 18:16:20.510327 sdss_archon-0.9.0b1/archon/actor/commands/reset.py
+-rw-r--r--   0        0        0     1713 2023-03-10 18:16:20.591600 sdss_archon-0.9.0b1/archon/actor/commands/status.py
+-rw-r--r--   0        0        0      920 2023-03-10 18:16:20.632566 sdss_archon-0.9.0b1/archon/actor/commands/system.py
+-rw-r--r--   0        0        0     1261 2023-03-10 18:16:20.713376 sdss_archon-0.9.0b1/archon/actor/commands/talk.py
+-rw-r--r--   0        0        0     3150 2023-03-10 18:16:20.754420 sdss_archon-0.9.0b1/archon/actor/commands/window.py
+-rw-r--r--   0        0        0    26217 2023-03-10 18:16:20.835933 sdss_archon-0.9.0b1/archon/actor/delegate.py
+-rw-r--r--   0        0        0     5379 2023-03-10 18:16:20.877632 sdss_archon-0.9.0b1/archon/actor/tools.py
+-rw-r--r--   0        0        0      587 2023-03-10 18:16:20.959768 sdss_archon-0.9.0b1/archon/controller/__init__.py
+-rw-r--r--   0        0        0     7430 2023-03-10 18:16:21.000823 sdss_archon-0.9.0b1/archon/controller/command.py
+-rw-r--r--   0        0        0    47092 2023-03-10 18:16:21.082026 sdss_archon-0.9.0b1/archon/controller/controller.py
+-rw-r--r--   0        0        0     1334 2023-03-10 18:16:21.123127 sdss_archon-0.9.0b1/archon/controller/maskbits.py
+-rw-r--r--   0        0        0      427 2023-03-10 18:16:21.204242 sdss_archon-0.9.0b1/archon/etc/archon.yml
+-rw-r--r--   0        0        0     3191 2023-03-10 18:16:21.245234 sdss_archon-0.9.0b1/archon/etc/schema.json
+-rw-r--r--   0        0        0     2078 2023-03-10 18:16:21.325934 sdss_archon-0.9.0b1/archon/exceptions.py
+-rw-r--r--   0        0        0     3830 2023-03-10 18:16:21.367337 sdss_archon-0.9.0b1/archon/tools.py
+-rw-r--r--   0        0        0     2398 2023-03-10 18:16:21.814897 sdss_archon-0.9.0b1/pyproject.toml
+-rw-r--r--   0        0        0     5582 1970-01-01 00:00:00.000000 sdss_archon-0.9.0b1/PKG-INFO
```

### Comparing `sdss_archon-0.9.0/LICENSE.md` & `sdss_archon-0.9.0b1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/README.md` & `sdss_archon-0.9.0b1/README.md`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/__init__.py` & `sdss_archon-0.9.0b1/archon/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/actor.py` & `sdss_archon-0.9.0b1/archon/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/__init__.py` & `sdss_archon-0.9.0b1/archon/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/config.py` & `sdss_archon-0.9.0b1/archon/actor/commands/config.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/disconnect.py` & `sdss_archon-0.9.0b1/archon/actor/commands/disconnect.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/expose.py` & `sdss_archon-0.9.0b1/archon/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/flush.py` & `sdss_archon-0.9.0b1/archon/actor/commands/flush.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/frame.py` & `sdss_archon-0.9.0b1/archon/actor/commands/frame.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/init.py` & `sdss_archon-0.9.0b1/archon/actor/commands/init.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/power.py` & `sdss_archon-0.9.0b1/archon/actor/commands/power.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/reconnect.py` & `sdss_archon-0.9.0b1/archon/actor/commands/reconnect.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/reset.py` & `sdss_archon-0.9.0b1/archon/actor/commands/reset.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/status.py` & `sdss_archon-0.9.0b1/archon/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/system.py` & `sdss_archon-0.9.0b1/archon/actor/commands/system.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/talk.py` & `sdss_archon-0.9.0b1/archon/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/commands/window.py` & `sdss_archon-0.9.0b1/archon/actor/commands/window.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/actor/delegate.py` & `sdss_archon-0.9.0b1/archon/actor/delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from astropy.io import fits
 
 from sdsstools.time import get_sjd
 
 from archon import __version__
 from archon.controller.controller import ArchonController
 from archon.controller.maskbits import ControllerStatus
-from archon.tools import gzip_async, subprocess_run_async
+from archon.tools import gzip_async
 
 
 if TYPE_CHECKING:  # pragma: no cover
     from clu import Command
 
     from .actor import ArchonBaseActor
 
@@ -302,16 +302,14 @@
         return True
 
     async def expose_cotasks(self):
         """Tasks that will be executed concurrently with readout.
 
         There is no guarantee that this coroutine will be waited or that
         it will complete before the shutter closes and the readout begins.
-        To ensure that the expose tasks have completed, await the task
-        in ``self._expose_cotasks``.
 
         """
 
         return
 
     async def readout_cotasks(self):
         """Tasks that will be executed concurrently with readout.
@@ -389,16 +387,14 @@
 
         if len(valid) != len(filenames):
             for fn in filenames:
                 if isinstance(fn, Exception):
                     self.command.error(f"HDUs failed to write to disk: {fn!s}")
                     return False
 
-        await self._generate_checksum(valid)
-
         return True
 
     async def _write_to_file(self, hdu: fits.PrimaryHDU, file_path: str):
         """Writes the HDU to file using an executor.
 
         The file is first written to a temporary file with the same path and
         name as the final file but with a random suffix, and then renamed.
@@ -433,53 +429,14 @@
                 f"Failed renaming temporary file {temp_file}. "
                 "The original file is still available."
             )
             return
 
         return file_path
 
-    async def _generate_checksum(self, filenames: list[str]):
-        """Generates a checksum file for the images written to disk."""
-
-        write_checksum = False
-        if self.actor.config.get("checksum", None):
-            if self.actor.config["checksum"].get("write", False):
-                write_checksum = True
-
-        if not write_checksum:
-            return
-
-        checksum_config = self.actor.config["checksum"]
-
-        checksum_mode = checksum_config.get("mode", "md5")
-        if checksum_mode.startswith("sha1"):
-            sum_command = "sha1sum"
-        elif checksum_mode.startswith("md5"):
-            sum_command = "md5sum"
-        else:
-            self.command.warning(f"Invalid checksum mode {checksum_mode!r}.")
-            return
-
-        checksum_basefile = checksum_config.get("file", f"{{SJD}}.{checksum_mode}sum")
-        checksum_basefile = checksum_basefile.format(SJD=get_sjd())
-
-        for filename in filenames:
-            filename = str(filename)
-            dirname = os.path.dirname(os.path.realpath(filename))
-            basename = os.path.basename(filename)
-
-            try:
-                await subprocess_run_async(
-                    f"{sum_command} {basename} >> {checksum_basefile}",
-                    shell=True,
-                    cwd=dirname,
-                )
-            except Exception as err:
-                self.command.warning(f"Failed to generate checksum: {err}")
-
     async def post_process(
         self,
         controller: ArchonController,
         hdus: list[fits.PrimaryHDU],
     ) -> tuple[ArchonController, list[fits.PrimaryHDU]]:
         """Custom post-processing."""
```

### Comparing `sdss_archon-0.9.0/archon/actor/tools.py` & `sdss_archon-0.9.0b1/archon/actor/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/controller/__init__.py` & `sdss_archon-0.9.0b1/archon/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/controller/command.py` & `sdss_archon-0.9.0b1/archon/controller/command.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/controller/controller.py` & `sdss_archon-0.9.0b1/archon/controller/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/controller/maskbits.py` & `sdss_archon-0.9.0b1/archon/controller/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/etc/schema.json` & `sdss_archon-0.9.0b1/archon/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/exceptions.py` & `sdss_archon-0.9.0b1/archon/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_archon-0.9.0/archon/tools.py` & `sdss_archon-0.9.0b1/archon/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,28 +52,27 @@
     def reset(self):
         """Reset the count."""
 
         self.cancel()
         self._task = self._loop.create_task(self._job())
 
 
-async def subprocess_run_async(*args, shell=False, cwd=None):
+async def subprocess_run_async(*args, shell=False):
     """Runs a command asynchronously.
 
     If ``shell=True`` the command will be executed through the shell. In that case
     the argument must be a single string with the full command. Otherwise, must receive
     a list of program arguments. Returns the output of stdout.
     """
 
     if shell:
         cmd = await asyncio.create_subprocess_shell(
             args[0],
             stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE,
-            cwd=cwd,
         )
         cmd_str = args[0]
 
     else:
         cmd = await asyncio.create_subprocess_exec(
             *args,
             stdout=asyncio.subprocess.PIPE,
```

### Comparing `sdss_archon-0.9.0/pyproject.toml` & `sdss_archon-0.9.0b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-archon"
-version = "0.9.0"
+version = "0.9.0b1"
 description = "A library and actor to communicate with an STA Archon controller."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/archon"
 repository = "https://github.com/sdss/archon"
 documentation = "https://sdss-archon.readthedocs.org"
@@ -37,14 +37,15 @@
 doc8 = ">=0.8.0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
 pytest-sugar = ">=0.9.2"
 isort = ">=4.3.21"
+codecov = ">=2.0.15"
 coverage = {version = ">=5.0", extras = ["toml"]}
 ipdb = ">=0.12.3"
 rstcheck = ">=3.3.1"
 Sphinx = ">=3.0.0"
 black = ">=20.8b1"
 jedi = "0.17.2"
 sphinx-click = ">=2.6.0"
```

### Comparing `sdss_archon-0.9.0/PKG-INFO` & `sdss_archon-0.9.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-archon
-Version: 0.9.0
+Version: 0.9.0b1
 Summary: A library and actor to communicate with an STA Archon controller.
 Home-page: https://github.com/sdss/archon
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<3.12
```

