# Comparing `tmp/mama-0.8.0.tar.gz` & `tmp/mama-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.8.0.tar", last modified: Mon Jul 17 21:31:56 2023, max compression
+gzip compressed data, was "mama-0.8.1.tar", last modified: Tue Jul 18 11:14:33 2023, max compression
```

## Comparing `mama-0.8.0.tar` & `mama-0.8.1.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.8.0/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-17 21:31:56.420707 mama-0.8.0/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11354 2023-07-17 21:28:34.000000 mama-0.8.0/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.8.0/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12572 2023-03-08 20:41:13.000000 mama-0.8.0/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    38745 2023-07-17 19:15:48.000000 mama-0.8.0/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    23348 2023-07-14 21:51:07.000000 mama-0.8.0/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    51121 2023-07-17 21:14:34.000000 mama-0.8.0/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    13639 2023-07-17 13:34:28.000000 mama-0.8.0/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    14557 2023-07-17 12:51:12.000000 mama-0.8.0/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.8.0/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11372 2023-07-17 12:54:02.000000 mama-0.8.0/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.8.0/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7828 2023-04-07 22:30:06.000000 mama-0.8.0/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     6773 2023-03-08 20:52:02.000000 mama-0.8.0/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-31 19:23:36.000000 mama-0.8.0/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.8.0/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3348 2023-07-17 21:12:25.000000 mama-0.8.0/mama/platforms/mips.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     4765 2023-07-17 19:14:06.000000 mama-0.8.0/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.8.0/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.8.0/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2022-10-13 07:46:30.000000 mama-0.8.0/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.8.0/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12615 2023-07-14 21:38:06.000000 mama-0.8.0/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.8.0/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15666 2023-05-09 09:22:21.000000 mama-0.8.0/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.8.0/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.8.0/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9784 2023-04-09 16:20:29.000000 mama-0.8.0/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1439 2023-03-06 14:41:17.000000 mama-0.8.0/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      793 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2023-07-17 21:29:07.000000 mama-0.8.0/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-07-17 21:31:56.420707 mama-0.8.0/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.8.1/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-18 11:14:33.541546 mama-0.8.1/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11354 2023-07-17 21:28:34.000000 mama-0.8.1/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.8.1/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12572 2023-03-08 20:41:13.000000 mama-0.8.1/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    38745 2023-07-17 19:15:48.000000 mama-0.8.1/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    23348 2023-07-14 21:51:07.000000 mama-0.8.1/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    50914 2023-07-18 11:13:23.000000 mama-0.8.1/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    13639 2023-07-17 13:34:28.000000 mama-0.8.1/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    14557 2023-07-17 12:51:12.000000 mama-0.8.1/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.8.1/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11372 2023-07-17 12:54:02.000000 mama-0.8.1/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.8.1/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     8133 2023-07-18 10:47:43.000000 mama-0.8.1/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     6773 2023-03-08 20:52:02.000000 mama-0.8.1/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-31 19:23:36.000000 mama-0.8.1/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.8.1/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3348 2023-07-17 21:12:25.000000 mama-0.8.1/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     4765 2023-07-17 19:14:06.000000 mama-0.8.1/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.8.1/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.8.1/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2022-10-13 07:46:30.000000 mama-0.8.1/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.8.1/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12615 2023-07-14 21:38:06.000000 mama-0.8.1/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.8.1/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15932 2023-07-18 10:46:30.000000 mama-0.8.1/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.8.1/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1795 2023-07-18 10:55:23.000000 mama-0.8.1/mama/utils/gdb.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      922 2023-07-18 10:56:31.000000 mama-0.8.1/mama/utils/gtest.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.8.1/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1002 2023-07-18 10:52:29.000000 mama-0.8.1/mama/utils/run.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9784 2023-07-18 10:24:21.000000 mama-0.8.1/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1439 2023-03-06 14:41:17.000000 mama-0.8.1/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      849 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1181 2023-07-18 11:13:12.000000 mama-0.8.1/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-07-18 11:14:33.541546 mama-0.8.1/setup.cfg
```

### Comparing `mama-0.8.0/LICENSE` & `mama-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/PKG-INFO` & `mama-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.8.0
+Version: 0.8.1
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.8.0/README.md` & `mama-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/artifactory.py` & `mama-0.8.1/mama/artifactory.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/build_config.py` & `mama-0.8.1/mama/build_config.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/build_dependency.py` & `mama-0.8.1/mama/build_dependency.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/build_target.py` & `mama-0.8.1/mama/build_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from .types.git import Git
 from .types.local_source import LocalSource
 from .types.asset import Asset
 from .types.artifactory_pkg import ArtifactoryPkg
 
 from .artifactory import artifactory_fetch_and_reconfigure
 from .utils.system import System, console
-from .utils.sub_process import execute, execute_echo
+from .utils.gdb import run_gdb
+from .utils.gtest import run_gtest
+from .utils.run import run_in_project_dir, run_in_working_dir
 from .papa_deploy import papa_deploy_to, papa_upload_to
 import mama.msbuild as msbuild
 import mama.util as util
 import mama.cmake_configure as cmake
 import mama.package as package
 
 if TYPE_CHECKING:
@@ -478,15 +480,15 @@
         self.export_asset('extras/csharp/NanoMesh.cs', category='dotnet')
             --> {deploy}/dotnet/NanoMesh.cs
         ```
         """
         return package.export_asset(self, asset, category, src_dir)
 
 
-    def export_assets(self, assets_path, pattern_substrings = [], category=None, src_dir=True):
+    def export_assets(self, assets_path: str, pattern_substrings = [], category=None, src_dir=True):
         """
         Performs a GLOB recurse, using specific pattern substrings.
         This can be later used when creating a deployment
 
         category -- (optional) Can be used for grouping the assets and flattening folder structure
         
         Example:
@@ -497,15 +499,15 @@
         self.export_assets('extras/csharp', ['.cs'], category='dotnet')
             --> {deploy}/dotnet/NanoMesh.cs
         ```
         """
         return package.export_assets(self, assets_path, pattern_substrings, category, src_dir)
 
 
-    def export_syslib(self, name, apt='', required=True):
+    def export_syslib(self, name: str, apt='', required=True):
         """
         For UNIX: Find and export system libraries so they are automatically linked with mamabuild.
 
         :returns: TRUE if syslib was exported; FALSE if required=False and syslib not found
         ```
             self.export_syslib('uuid')
             # will attempt to find system library in this order:
@@ -651,15 +653,15 @@
             self.add_cmake_options(['ZLIB_STATIC=TRUE', 'NO_GUI=1'])
         ```
         """
         for option in options:
             if isinstance(option, list): self.cmake_opts += option
             else:                        self.cmake_opts.append(option)
 
-    
+
     def add_platform_options(self, windows=None, linux=None, macos=None, ios=None, android=None):
         """
         Selectively applies CMake options depending on configuration platform.
         ```
             self.add_platform_options(windows='ZLIB_STATIC=TRUE')
         ```
         """
@@ -745,68 +747,68 @@
 
     def is_enabled_cxx11(self):
         if 'CXX11' in self.args: return True
         std = self._get_cxx_std()
         return 'c++11' in std
 
 
-    def copy(self, src, dst):
+    def copy(self, src: str, dst: str):
         """
         Utility for copying files and folders
         ```
             # copies built .so into an android archive
             self.copy(self.build_dir('libAwesome.so'), 
                       self.source_dir('deploy/Awesome.aar/jni/armeabi-v7a'))
         ```
         """
         if util.copy_if_needed(src, dst):
             if self.config.verbose: console(f'copy {src} --> {dst}')
 
 
-    def copy_built_file(self, builtFile, copyToFolder):
+    def copy_built_file(self, builtFile: str, copyToFolder: str):
         """
         Utility for copying files within the build directory.
         ```
             self.copy_built_file('RelWithDebInfo/libawesome.a', 'lib')
         ```
         """
         src = f'{self.build_dir()}/{builtFile}'
         dst = f'{self.build_dir()}/{copyToFolder}/{os.path.basename(builtFile)}'
         if not os.path.exists(src) and os.path.exists(dst):
             return # src is missing, but dst exists, ignore error
         if util.copy_if_needed(src, dst):
             if self.config.verbose: console(f'copy_built_file {src} --> {dst}')
 
 
-    def copy_deployed_folder(self, src_dir, dst_dir):
+    def copy_deployed_folder(self, src_dir: str, dst_dir: str):
         """
         Utility for copying folders from source dir.
         ```
             self.copy_deployed_folder('deploy/NanoMesh', 'C:/Projects/Game/Plugins')
             # --> 'C:/Projects/Game/Plugins/NanoMesh
         ```
         """
         src = self.source_dir(src_dir)
         dst = dst_dir
         if util.copy_if_needed(src, dst):
             if self.config.verbose: console(f'copy_deployed_folder {src} --> {dst}')
 
 
-    def download_file(self, remote_url, local_dir, force=False):
+    def download_file(self, remote_url: str, local_dir: str, force=False):
         """
         Downloads a file if it doesn't already exist.
         ```
             self.download_file('http://example.com/file1', 'bin')
             # --> 'bin/file1'
         ```
         """
         return util.download_file(remote_url, local_dir, force)
 
 
-    def download_and_unzip(self, remote_zip, extract_dir, unless_file_exists=None):
+    def download_and_unzip(self, remote_zip: str, extract_dir: str, unless_file_exists=None):
         """
         Downloads and unzips an archive if it doesn't already exist.
 
         unless_file_exists -- If the specified file exists, then download and unzip steps are skipped.
         ```
             self.download_and_unzip('http://example.com/archive.zip', 
                                     'bin', 'bin/unzipped_file.txt')
@@ -872,78 +874,63 @@
                 self.nothing_to_build()
         ```
         """
         self.dep.nothing_to_build = True
         self.dep.should_rebuild = False
 
 
-    def run(self, command, src_dir=False, exit_on_fail=True):
+    def run(self, command: str, src_dir=False, exit_on_fail=True):
         """
         Run a command in the build or source folder.
         Can be used for any custom commands or custom build systems.
         src_dir -- [False] If true, then command is relative to source directory.
         ```
-            self.run('./configure')
-            self.run('make release -j7')
+            self.run('./configure', src_dir=True)
+            self.run('make release -j7') # run in build dir
         ```
         """
-        dir = self.source_dir() if src_dir else self.build_dir()
-        res = execute(f'cd {dir} && {command}', echo=True, throw=not exit_on_fail)
-        if res != 0 and exit_on_fail:
-            exit(res)
+        run_in_project_dir(self, command, src_dir, exit_on_fail)
 
 
-    def run_program(self, working_dir, command):
+    def run_program(self, working_dir: str, command: str, exit_on_fail=True):
         """
         Run any program in any directory. Can be used for custom tools.
         ```
             self.run_program(self.source_dir('bin'), 
                              self.source_dir('bin/DbTool'))
         ```
         """
-        execute_echo(working_dir, command, exit_on_fail=True)
+        run_in_working_dir(self, working_dir, command, exit_on_fail=exit_on_fail)
 
 
-    ## TODO: Move this into a new utility
-    def gdb(self, command, src_dir=True):
+    def gdb(self, command: str, src_dir=True):
         """
         Run a command with gdb in the build folder.
         ```
             self.gdb('bin/NanoMeshTests')
         ```
         """
-        if self.android or self.ios or self.raspi or self.oclea or self.mips:
-            console('Cannot run tests for Android, iOS, Raspi, Oclea, MIPS builds.')
-            return # nothing to run
-
-        split = command.split(' ', 1)
-        cmd = split[0].lstrip('.')
-        args = split[1] if len(split) >= 2 else ''
-        path = self.source_dir() if src_dir else self.build_dir()
-        path = f"{path}/{os.path.dirname(cmd).lstrip('/')}"
-        exe = os.path.basename(cmd)
-
-        if System.windows and self.windows and '.exe' not in exe:
-            exe += '.exe'
-
-        if self.windows:
-            if not src_dir: path = f'{path}/{self.cmake_build_type}'
-            gdb = f'{path}/{exe} {args}'
-        elif self.macos:
-            # b: batch, q: quiet, -o r: run
-            # -k bt: on crash, backtrace
-            # -k q: on crash, quit 
-            gdb = f'lldb -b -o r -k bt -k q  -- ./{exe} {args}'
-        else: # linux
-            # r: run;  bt: give backtrace;  q: quit when done;
-            gdb = f'gdb -batch -return-child-result -ex=r -ex=bt -ex=q --args ./{exe} {args}'
-
-        if not os.path.exists(f'{path}/{exe}'):
-            raise IOError(f'Could not find {path}/{exe}')
-        execute_echo(cwd=path, cmd=gdb)
+        return run_gdb(self, command, src_dir)
+
+
+    def gtest(self, executable: str, args: str, src_dir=True):
+        """
+        Runs a gtest executable with gdb by default.
+        The gtest report is written to $src_dir/test/report.xml.
+        Arguments
+        - executable -- which executable to run
+        - args -- a string of options separated by spaces, 
+          'gdb', 'nogdb' or gtest fixture/test partial name
+        - src_dir -- [True] If true, then executable is relative to source directory.
+        ```
+            self.gtest("bin/MyAppGtests", "nogdb", src_dir=True)
+            self.gtest("bin/MyAppGtests", "MyFixtureName.TheTestName", src_dir=True)
+        ```
+        """
+        run_gtest(self, executable, args, src_dir)
 
 
     ########## Customization Points ###########
 
 
     def settings(self):
         """
@@ -1153,15 +1140,19 @@
 
     def test(self, args):
         """
         Perform test steps here with test args.
         `mama test arg1 arg2 arg3`
         ```
             def test(self, args):
+                # simply runs an executable with GDB
                 self.gdb(f'RppTests {args}')
+                # or run gtest executable, with GDB by default
+                # or you can provide `nogdb` argument to disable GDB
+                self.gtest(f'bin/project_gtests', args, src_dir=True)
         ```
         """
         pass
 
 
     def start(self, args):
         """
```

### Comparing `mama-0.8.0/mama/cmake_configure.py` & `mama-0.8.1/mama/cmake_configure.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/dependency_chain.py` & `mama-0.8.1/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/init_project.py` & `mama-0.8.1/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/main.py` & `mama-0.8.1/mama/main.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/msbuild.py` & `mama-0.8.1/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/package.py` & `mama-0.8.1/mama/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,114 +1,114 @@
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import List, TYPE_CHECKING
 import os
 from .utils.system import console
 from .util import normalized_path, glob_with_name_match
 from .types.asset import Asset
 
 if TYPE_CHECKING:
     from .build_target import BuildTarget
 
-def is_a_static_library(lib):
+def is_a_static_library(lib: str):
     return lib.endswith('.a') or lib.endswith('.lib')
 
 
-def is_a_dynamic_library(lib):
+def is_a_dynamic_library(lib: str):
     return lib.endswith('.dll')    or lib.endswith('.pdb') \
         or lib.endswith('.dylib')  or lib.endswith('.so')  \
         or lib.endswith('.bundle') or lib.endswith('.framework') \
         or lib.endswith('.aar')
 
 
-def is_a_library(lib):
+def is_a_library(lib: str):
     return is_a_static_library(lib) or is_a_dynamic_library(lib)
 
 
-def target_root_path(target, path, src_dir):
+def target_root_path(target: BuildTarget, path: str, src_dir: bool):
     root = target.source_dir() if src_dir else target.build_dir()
     return normalized_path(os.path.join(root, path))
 
 
-def get_lib_basename(lib):
+def get_lib_basename(lib: str|tuple):
     if isinstance(lib, tuple):
         return os.path.basename(lib[0])
     elif lib.startswith('-framework '):
         return lib.split(' ', 1)[1]
     else:
         return os.path.basename(lib)
 
 
-def get_unique_basenames(items):
+def get_unique_basenames(items: list):
     unique = dict()
     for item in items:
         basename = get_lib_basename(item)
         unique[basename] = item
     return list(unique.values())
 
 
-def export_include(target, include_path, build_dir):
+def export_include(target: BuildTarget, include_path: str, build_dir: bool):
     include_path = target_root_path(target, include_path, not build_dir)
     #console(f'export_include={include_path}')
     if os.path.exists(include_path):
         if not include_path in target.exported_includes:
             target.exported_includes.append(include_path)
         return True
     return False
 
 
-def export_includes(target, include_paths, build_dir):
+def export_includes(target: BuildTarget, include_paths: list, build_dir: bool):
     added = False
     for include_path in include_paths:
         added |= target.export_include(include_path, build_dir)
     return added
 
 
-def export_lib(target, relative_path, src_dir):
+def export_lib(target: BuildTarget, relative_path: str, src_dir: str):
     path = target_root_path(target, relative_path, src_dir)
     if os.path.exists(path):
         target.exported_libs.append(path)
         target.exported_libs = get_unique_basenames(target.exported_libs)
     else:
         console(f'export_lib failed to find: {path}')
 
 
-def set_export_libs_and_products(target, libs_and_deps:list):
+def set_export_libs_and_products(target: BuildTarget, libs_and_deps: List[str]):
     """
     Sets target's exported_libs and build_products from previously serialized
     list of libraries and dependencies
     """
     libs_and_deps = cleanup_libs_list(libs_and_deps)
     only_libs = []
     for lib in libs_and_deps:
         if os.path.exists(lib) and is_a_library(lib):
             only_libs.append(lib)
     target.exported_libs = get_unique_basenames(only_libs)
     target.build_products = get_unique_basenames(libs_and_deps)
 
 
-def cleanup_libs_list(libs):
+def cleanup_libs_list(libs: List[str]):
     """Cleans up libs list by removing invalid entries"""
     cleaned = []
     for lib in libs:
         lib = lib.strip()
         if not lib.endswith('.lib.recipe'):
             cleaned.append(lib)
     return cleaned
 
 
-def clean_intermediate_files(target):
+def clean_intermediate_files(target: BuildTarget):
     files_to_clean = glob_with_name_match(target.build_dir(), ['.obj', '.o'])
     if files_to_clean:
         if target.config.print:
             print(f'Cleaning {len(files_to_clean)} intermediate files in {target.build_dir()}')
         for file in files_to_clean:
             os.remove(file)
 
 
-def export_libs(target, path, pattern_substrings, src_dir, order):
+def export_libs(target: BuildTarget, path, pattern_substrings: List[str], src_dir: bool, order: list):
     root_path = target_root_path(target, path, src_dir)
     libs = glob_with_name_match(root_path, pattern_substrings)
     libs = cleanup_libs_list(libs)
 
     # ignore root_path/deploy
     root_deploy = root_path + '/deploy/'
     libs = [l for l in libs if not l.startswith(root_deploy)]
@@ -122,35 +122,35 @@
             return lib_index(lib)
         libs.sort(key=sort_key)
     target.exported_libs += libs
     target.exported_libs = get_unique_basenames(target.exported_libs)
     return len(target.exported_libs) > 0
 
 
-def export_asset(target, asset, category=None, src_dir=True):
+def export_asset(target: BuildTarget, asset: str, category=None, src_dir=True):
     full_asset = target_root_path(target, asset, src_dir)
     if os.path.exists(full_asset):
         target.exported_assets.append(Asset(asset, full_asset, category))
         return True
     else:
         console(f'export_asset failed to find: {full_asset}')
         return False
 
 
-def export_assets(target, assets_path, pattern_substrings, category=None, src_dir=True):
+def export_assets(target: BuildTarget, assets_path: str, pattern_substrings: list, category=None, src_dir=True):
     assets_path += '/'
     assets = glob_with_name_match(target_root_path(target, assets_path, src_dir), pattern_substrings, match_dirs=False)
     if assets:
         for full_asset in assets:
             target.exported_assets.append(Asset(assets_path, full_asset, category))
         return True
     return False
 
 
-def find_syslib(target: BuildTarget, name, apt, required: bool):
+def find_syslib(target: BuildTarget, name: str, apt: bool, required: bool):
     if target.ios or target.macos:
         if not name.startswith('-framework '):
             raise EnvironmentError(f'Expected "-framework name" but got "{name}"')
         return name # '-framework Foundation'
     elif target.linux:
         for candidate in [
             lambda: f'/usr/lib/x86_64-linux-gnu/{name}',
@@ -163,15 +163,15 @@
         if not required: return None
         if apt: raise IOError(f'Error {target.name} failed to find REQUIRED SysLib: {name}  Try `sudo apt install {apt}`')
         raise IOError(f'Error {target.name} failed to find REQUIRED SysLib: {name}  Try installing it with apt.')
     else:
         return name # just export it. expect system linker to find it.
 
 
-def export_syslib(target: BuildTarget, name, apt: bool, required: bool):
+def export_syslib(target: BuildTarget, name: str, apt: bool, required: bool):
     """
     - target: The build target where to add the export syslib
     - name: Name of the system library, eg: lzma
     - apt: if true, then apt suggestion is given
     - required: if true, then an exception is thrown if syslib is not found
     """
     try:
@@ -188,32 +188,32 @@
             target.exported_syslibs = get_unique_basenames(target.exported_syslibs)
             return True
         else:
             raise
     return False
 
 
-def get_lib_basename(syslib):
+def get_lib_basename(syslib: str):
     if syslib.startswith('-framework '):
         return syslib
     return os.path.basename(syslib)
 
 
-def _reset_syslib_name(syslib):
+def _reset_syslib_name(syslib: str):
     """ Resets the syslib name from `/usr/lib/x86_64-linux-gnu/liblzma.so` to `lzma` """
     fname = os.path.basename(syslib)
     if fname.startswith('lib'):
         if fname.endswith('.so'):
             return fname[3:-3]  # pop 'lib'(3) from front and '.so'(3) from back
         if fname.endswith('.a'):
             return fname[3:-2]  # pop 'lib' and '.a'
     return fname
 
 
-def reload_syslibs(target, syslibs):
+def reload_syslibs(target: BuildTarget, syslibs: List[str]):
     reloaded = []
     for syslib in syslibs:
         if syslib.startswith('-framework '):
             reloaded.append(syslib)
         else:
             libname = _reset_syslib_name(syslib)
             lib = find_syslib(target, libname, apt=None, required=False)
```

### Comparing `mama-0.8.0/mama/papa_deploy.py` & `mama-0.8.1/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/parse_mamafile.py` & `mama-0.8.1/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/platforms/mips.py` & `mama-0.8.1/mama/platforms/mips.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/platforms/oclea.py` & `mama-0.8.1/mama/platforms/oclea.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/types/artifactory_pkg.py` & `mama-0.8.1/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/types/asset.py` & `mama-0.8.1/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/types/dep_source.py` & `mama-0.8.1/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/types/git.py` & `mama-0.8.1/mama/types/git.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/types/local_source.py` & `mama-0.8.1/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/util.py` & `mama-0.8.1/mama/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import time, ssl, pathlib, random
 from .utils.system import System, console
 from .utils.sub_process import execute
 from urllib import request
 from datetime import datetime
 from dateutil import tz
 
-def is_file_modified(src, dst):
+def is_file_modified(src: str, dst: str):
     return os.path.getmtime(src) == os.path.getmtime(dst) and\
            os.path.getsize(src) == os.path.getsize(dst)
 
 
-def find_executable_from_system(name):
+def find_executable_from_system(name: str):
     if not name: return ''
     output = shutil.which(name)
     if not output: return ''
     return output if os.path.isfile(output) else ''
 
 
-def copy_files(fromFolder, toFolder, fileNames):
+def copy_files(fromFolder: str, toFolder: str, fileNames: List[str]):
     for file in fileNames:
         sourceFile = os.path.join(fromFolder, file)
         if not os.path.exists(sourceFile):
             continue
         destFile = os.path.join(toFolder, os.path.basename(file))
         destFileExists = os.path.exists(destFile)
         if destFileExists and is_file_modified(sourceFile, destFile):
@@ -36,15 +36,15 @@
             try:
                 os.remove(tempCopy)
             except Exception:
                 pass
         shutil.copy2(sourceFile, destFile) # copy while preserving metadata
 
 
-def deploy_framework(framework, deployFolder):
+def deploy_framework(framework: str, deployFolder: str):
     if not os.path.exists(framework):
         raise IOError(f'no framework found at: {framework}') 
     if os.path.exists(deployFolder):
         name = os.path.basename(framework)
         deployPath = os.path.join(deployFolder, name)
         console(f'Deploying framework to {deployPath}')
         execute(f'rm -rf {deployPath}')
@@ -91,37 +91,37 @@
 
 
 def normalized_join(path1: str, *pathsN) -> str:
     """ Joins N paths and the calls normalized_path() """
     return normalized_path(os.path.join(path1, *pathsN))
 
 
-def glob_with_extensions(rootdir, extensions):
+def glob_with_extensions(rootdir: str, extensions: List[str]) -> List[str]:
     results = []
     for dirpath, _, dirfiles in os.walk(rootdir):
         for file in dirfiles:
             _, fext = os.path.splitext(file)
             if fext in extensions:
                 pathstring = os.path.join(dirpath, file)
                 pathstring = normalized_path(pathstring)
                 results.append(pathstring)
     return results
 
 
-def strstr_multi(s, substrings):
+def strstr_multi(s: str, substrings: List[str]) -> bool:
     #console(f'file: {s} matches: {substrings}')
     if not substrings: # if no substrings, then match everything
         return True
     for substr in substrings:
         if substr in s:
             return True
     return False
 
 
-def glob_with_name_match(rootdir, pattern_substrings, match_dirs=True):
+def glob_with_name_match(rootdir: str, pattern_substrings: list, match_dirs=True) -> List[str]:
     results = []
     for dirpath, dirnames, dirfiles in os.walk(rootdir):
         if match_dirs:
             for dir in dirnames:
                 if strstr_multi(dir, pattern_substrings):
                     pathstring = os.path.join(dirpath, dir)
                     pathstring = normalized_path(pathstring)
@@ -130,51 +130,51 @@
             if strstr_multi(file, pattern_substrings):
                 pathstring = os.path.join(dirpath, file)
                 pathstring = normalized_path(pathstring)
                 results.append(pathstring)
     return results
 
 
-def glob_folders_with_name_match(rootdir, pattern_substrings):
+def glob_folders_with_name_match(rootdir: str, pattern_substrings: List[str]):
     results = []
     for dirpath, _, _ in os.walk(rootdir):
         if strstr_multi(dirpath, pattern_substrings):
             results.append(normalized_path(dirpath))
     return results
 
 
-def is_dir_empty(dir): # no files?
+def is_dir_empty(dir: str): # no files?
     if not os.path.exists(dir): return True
     _, _, filenames = next(os.walk(dir))
     return len(filenames) == 0
 
 
-def has_tag_changed(old_tag_file, new_tag):
+def has_tag_changed(old_tag_file: str, new_tag: str):
     if not os.path.exists(old_tag_file):
         return True
     old_tag = read_text_from(old_tag_file)
     if old_tag != new_tag:
         console(f" tagchange '{old_tag.strip()}'\n"+
                 f"      ---> '{new_tag.strip()}'")
         return True
     return False
 
 
-def read_text_from(file_path) -> str:
+def read_text_from(file_path: str) -> str:
     return pathlib.Path(file_path).read_text()
 
 
-def write_text_to(file, text):
+def write_text_to(file: str, text: str):
     dirname = os.path.dirname(file)
     if not os.path.exists(dirname):
         os.makedirs(dirname, exist_ok=True)
     pathlib.Path(file).write_text(text, encoding='utf-8')
 
 
-def read_lines_from(file) -> List[str]:
+def read_lines_from(file: str) -> List[str]:
     if not os.path.exists(file):
         return []
     with pathlib.Path(file).open(encoding='utf-8') as f:
         return f.readlines()
 
 
 def get_file_size_str(size):
@@ -245,15 +245,15 @@
     # report actual percent here, just incase something goes wrong
     elapsed = time.time() - start
     percent = int((transferred / size) * 100.0)
     print(f'\r    |<{"="*50}| {percent:>3}% ({get_time_str(elapsed)})')
     return local_file
 
 
-def unzip(local_zip, extract_dir, pwd=None):
+def unzip(local_zip: str, extract_dir: str, pwd: str = None):
     """
     Attempts to unzip an archive, throws on failure.
     Only extracts the files if their current size or modified time mismatches.
     Always sets modified time from the zipfile info.
     Preserves symlinks. And sets the correct file permission attributes.
     Returns # of files actually extracted.
     """
@@ -342,15 +342,15 @@
     if not local_file:
         return None
     unzip(local_file, extract_dir)
     console(f'Extracted {local_file} to {extract_dir}')
     return extract_dir
 
 
-def _should_copy(src, dst):
+def _should_copy(src: str, dst: str):
     src_stat = None
     try:
         src_stat = os.stat(src)
     except (OSError, ValueError):
         return False # does not exist, nothing to copy
 
     dst_stat = None
@@ -365,35 +365,35 @@
     if src_stat.st_mtime != dst_stat.st_mtime:
         #console(f'_should_copy true src.mtime != dst.mtime\n┌<──{src}\n└──> {dst}')
         return True
     #console(f'skip {dst}')
     return False
 
 
-def _passes_filter(src_file, filter):
+def _passes_filter(src_file: str, filter: List[str]) -> bool:
     if not filter: return True
     for f in filter:
         if src_file.endswith(f):
             return True
     return False
 
 
-def copy_file(src, dst, filter) -> bool:
+def copy_file(src: str, dst: str, filter: List[str]) -> bool:
     """
         Copies a single file if it passes the filter and
         if it has changed, returns TRUE if copied
     """
     if _passes_filter(src, filter) and _should_copy(src, dst):
         #console(f'copy {src}\n --> {dst}')
         shutil.copy2(src, dst)
         return True
     return False
 
 
-def copy_dir(src_dir, out_dir, filter=None) -> bool:
+def copy_dir(src_dir: str, out_dir: str, filter=None) -> bool:
     """
         Copies an entire dir if it passes the filter and
         if the individual files have changed.
         Returns TRUE if any files were copied.
     """
     if not os.path.exists(src_dir):
         raise RuntimeError(f'copy_dir: {src_dir} does not exist!')
@@ -409,15 +409,15 @@
         for file in files:
             src_file = os.path.join(fulldir, file)
             dst_file = os.path.join(dst_folder, file)
             copied |= copy_file(src_file, dst_file, filter)
     return copied
 
 
-def copy_if_needed(src, dst, filter=None) -> bool:
+def copy_if_needed(src: str, dst: str, filter=None) -> bool:
     """ Copies src -> dst  dir/file  if needed and returns TRUE if anything was copied """
     #console(f'COPY {src} --> {dst}')
     if os.path.isdir(src):
         return copy_dir(src, dst, filter)
     else:
         return copy_file(src, dst, filter)
```

### Comparing `mama-0.8.0/mama/utils/nonblocking_io.py` & `mama-0.8.1/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/utils/sub_process.py` & `mama-0.8.1/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama/utils/system.py` & `mama-0.8.1/mama/utils/system.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.0/mama.egg-info/PKG-INFO` & `mama-0.8.1/mama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.8.0
+Version: 0.8.1
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.8.0/mama.egg-info/SOURCES.txt` & `mama-0.8.1/mama.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -27,10 +27,13 @@
 mama/types/__init__.py
 mama/types/artifactory_pkg.py
 mama/types/asset.py
 mama/types/dep_source.py
 mama/types/git.py
 mama/types/local_source.py
 mama/utils/__init__.py
+mama/utils/gdb.py
+mama/utils/gtest.py
 mama/utils/nonblocking_io.py
+mama/utils/run.py
 mama/utils/sub_process.py
 mama/utils/system.py
```

### Comparing `mama-0.8.0/pyproject.toml` & `mama-0.8.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.8.0"
+version = "0.8.01"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```

