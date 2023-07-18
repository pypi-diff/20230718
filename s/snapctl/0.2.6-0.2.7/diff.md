# Comparing `tmp/snapctl-0.2.6.tar.gz` & `tmp/snapctl-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapctl-0.2.6.tar", max compression
+gzip compressed data, was "snapctl-0.2.7.tar", max compression
```

## Comparing `snapctl-0.2.6.tar` & `snapctl-0.2.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      971 2023-07-17 16:26:27.384137 snapctl-0.2.6/README.md
--rw-r--r--   0        0        0      399 2023-07-17 15:31:21.284704 snapctl-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-17 15:14:31.467451 snapctl-0.2.6/snapctl/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.6/snapctl/__main__.py
--rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.6/snapctl/commands/__init__.py
--rw-r--r--   0        0        0     8886 2023-07-17 14:24:47.287813 snapctl-0.2.6/snapctl/commands/byosnap.py
--rw-r--r--   0        0        0     1575 2023-07-17 16:24:55.892589 snapctl-0.2.6/snapctl/main.py
--rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.6/snapctl/types/__init__.py
--rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.6/snapctl/types/definitions.py
--rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.6/snapctl/utils/__init__.py
--rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.6/snapctl/utils/echo.py
--rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 snapctl-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      971 2023-07-17 16:26:27.384137 snapctl-0.2.7/README.md
+-rw-r--r--   0        0        0      399 2023-07-18 17:51:11.107192 snapctl-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 15:14:31.467451 snapctl-0.2.7/snapctl/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.7/snapctl/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.7/snapctl/commands/__init__.py
+-rw-r--r--   0        0        0     9102 2023-07-18 18:54:09.906072 snapctl-0.2.7/snapctl/commands/byosnap.py
+-rw-r--r--   0        0        0     1599 2023-07-18 17:53:10.590362 snapctl-0.2.7/snapctl/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.7/snapctl/types/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.7/snapctl/types/definitions.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.7/snapctl/utils/__init__.py
+-rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.7/snapctl/utils/echo.py
+-rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 snapctl-0.2.7/PKG-INFO
```

### Comparing `snapctl-0.2.6/README.md` & `snapctl-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `snapctl-0.2.6/snapctl/commands/byosnap.py` & `snapctl-0.2.7/snapctl/commands/byosnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from sys import platform
 
 from snapctl.types.definitions import ResponseType
 from snapctl.utils.echo import error, success, info
 
 class ByoSnap:
   COMMANDS = ['build', 'push', 'upload-docs', 'publish']
+  DEFAULT_BUILD_PLATFORM = 'linux/arm64'
 
   def __init__(self, command: str, path: str, tag: str, token: str, dockerfile: str = 'Dockerfile') -> None:
     self.command: str = command
     self.path: str = path
     self.tag: str = tag
     self.token: str = token
     self.token_parts: list = ByoSnap.get_token_values(token)
@@ -27,15 +28,16 @@
       # url|web_app_token|service_id|ecr_repo_url|ecr_repo_username|ecr_repo_token
       # url = self.token_parts[0]
       # web_app_token = self.token_parts[1]
       # service_id = self.token_parts[2]
       # ecr_repo_url = self.token_parts[3]
       # ecr_repo_username = self.token_parts[4]
       # ecr_repo_token = self.token_parts[5]
-      if len(token_parts) == 6:
+      # platform = self.token_parts[6]
+      if len(token_parts) >= 6:
         return token_parts
     except Exception:
       pass
     return None
 
   def validate_input(self) -> ResponseType:
     response: ResponseType = {
@@ -69,14 +71,17 @@
     # web_app_token = self.token_parts[1]
     service_id = self.token_parts[2]
     ecr_repo_url = self.token_parts[3]
     ecr_repo_username = self.token_parts[4]
     ecr_repo_token = self.token_parts[5]
     image_tag = f'{service_id}.{self.tag}'
     full_ecr_repo_url = f'{ecr_repo_url}:{image_tag}'
+    build_platform = ByoSnap.DEFAULT_BUILD_PLATFORM
+    if len(self.token_parts) == 7:
+      build_platform = self.token_parts[6]
     try:
       # Check dependencies
       with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
       ) as progress:
@@ -116,20 +121,20 @@
         TextColumn("[progress.description]{task.description}"),
         transient=True,
       ) as progress:
         progress.add_task(description=f'Building your snap...', total=None)
         if platform == "win32":
           response = subprocess.run([
             #f"docker build --no-cache -t {tag} {path}"
-            'docker', 'build', '--platform', 'linux/arm64', '-t', image_tag, self.path
+            'docker', 'build', '--platform', build_platform, '-t', image_tag, self.path
           ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         else:
           response = subprocess.run([
             #f"docker build --no-cache -t {tag} {path}"
-            f"docker build --platform linux/arm64 -t {image_tag} {self.path}"
+            f"docker build --platform {build_platform} -t {image_tag} {self.path}"
           ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         if response.returncode:
           error('Unable to build docker.')
           return False
       success('Build Successfull')
 
       # Tag the repo
```

### Comparing `snapctl-0.2.6/snapctl/main.py` & `snapctl-0.2.7/snapctl/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import typer
 
 from snapctl.commands.byosnap import ByoSnap
 from snapctl.types.definitions import ResponseType
 from snapctl.utils.echo import error, success, info
 
-__version__ = '0.2.6'
+__version__ = '0.2.7'
 
 app = typer.Typer()
 
 def version_callback(value: bool = True):
   if value:
     typer.echo(f"Snapctl version: {__version__}")
     raise typer.Exit()
 
+# Presently in typer this is the only way we can expose the `--version`
 @app.callback()
 def common(
     ctx: typer.Context,
     version: bool = typer.Option(
       None, "--version",
       help="Get the Snapctl version.",
       callback=version_callback
     ),
 ):
     pass
 
-# command: Optional[str] = typer.Argument(None)
 @app.command()
 def byosnap(
   command: str = typer.Argument(..., help="BYOSnap Commands: " + ", ".join(ByoSnap.COMMANDS) + "."),
   path: str = typer.Argument(..., help="Path to your snap code"),
   tag: str = typer.Argument(..., help="Tag for your snap"),
   token: str = typer.Argument(..., help="Copy the token from the Web App"),
   docker_file: str = typer.Option("Dockerfile", help="Dockerfile name to use")
```

### Comparing `snapctl-0.2.6/PKG-INFO` & `snapctl-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapctl
-Version: 0.2.6
+Version: 0.2.7
 Summary: Snapser CLI Tool
 Author: Ajinkya Apte
 Author-email: aj@snapser.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

