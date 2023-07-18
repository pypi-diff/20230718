# Comparing `tmp/grai_cli-0.1.9.tar.gz` & `tmp/grai_cli-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_cli-0.1.9.tar", max compression
+gzip compressed data, was "grai_cli-0.2.0a1.tar", max compression
```

## Comparing `grai_cli-0.1.9.tar` & `grai_cli-0.2.0a1.tar`

### file list

```diff
@@ -1,29 +1,27 @@
--rw-r--r--   0        0        0        0 2022-07-19 07:50:36.524781 grai_cli-0.1.9/README.md
--rw-r--r--   0        0        0      293 2023-01-03 17:11:14.004310 grai_cli-0.1.9/grai_cli/__init__.py
--rw-r--r--   0        0        0       23 2023-01-03 17:11:14.004356 grai_cli-0.1.9/grai_cli/__version__.py
--rw-r--r--   0        0        0       63 2022-11-09 15:55:13.272679 grai_cli-0.1.9/grai_cli/api/__init__.py
--rw-r--r--   0        0        0       51 2022-07-24 08:00:09.094234 grai_cli-0.1.9/grai_cli/api/config/__init__.py
--rw-r--r--   0        0        0     2012 2023-03-19 22:15:28.568351 grai_cli-0.1.9/grai_cli/api/config/config.py
--rw-r--r--   0        0        0     2193 2023-03-16 04:12:39.224233 grai_cli-0.1.9/grai_cli/api/config/set.py
--rw-r--r--   0        0        0      463 2023-02-13 20:16:22.656762 grai_cli-0.1.9/grai_cli/api/config/setup.py
--rw-r--r--   0        0        0     1026 2023-02-13 20:16:22.656984 grai_cli-0.1.9/grai_cli/api/entrypoint.py
--rw-r--r--   0        0        0       49 2022-07-24 08:00:09.100216 grai_cli-0.1.9/grai_cli/api/server/__init__.py
--rw-r--r--   0        0        0     4372 2023-03-16 04:12:39.224788 grai_cli-0.1.9/grai_cli/api/server/endpoints.py
--rw-r--r--   0        0        0     1141 2023-03-16 04:12:39.225042 grai_cli-0.1.9/grai_cli/api/server/setup.py
--rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273574 grai_cli-0.1.9/grai_cli/api/telemetry/__init__.py
--rw-r--r--   0        0        0      300 2023-02-13 20:16:22.657393 grai_cli-0.1.9/grai_cli/api/telemetry/commands.py
--rw-r--r--   0        0        0       89 2023-03-16 04:12:39.225317 grai_cli-0.1.9/grai_cli/config_default.yaml
--rw-r--r--   0        0        0        0 2022-07-24 06:33:14.647347 grai_cli-0.1.9/grai_cli/py.typed
--rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273862 grai_cli-0.1.9/grai_cli/settings/__init__.py
--rw-r--r--   0        0        0     2098 2023-03-16 04:12:39.225733 grai_cli-0.1.9/grai_cli/settings/cache.py
--rw-r--r--   0        0        0     5772 2023-03-16 04:12:39.226132 grai_cli-0.1.9/grai_cli/settings/config.py
--rw-r--r--   0        0        0       88 2023-01-10 17:15:31.923336 grai_cli-0.1.9/grai_cli/utilities/__init__.py
--rw-r--r--   0        0        0     1233 2023-03-16 04:12:39.226578 grai_cli-0.1.9/grai_cli/utilities/headers.py
--rw-r--r--   0        0        0      783 2023-02-13 20:16:22.657964 grai_cli-0.1.9/grai_cli/utilities/styling.py
--rw-r--r--   0        0        0      541 2023-01-03 17:11:14.005048 grai_cli-0.1.9/grai_cli/utilities/telemetry.py
--rw-r--r--   0        0        0      488 2023-03-16 04:12:39.226900 grai_cli-0.1.9/grai_cli/utilities/test.py
--rw-r--r--   0        0        0     3529 2023-03-16 04:12:39.227159 grai_cli-0.1.9/grai_cli/utilities/utilities.py
--rw-r--r--   0        0        0     1663 2023-03-19 22:16:09.155405 grai_cli-0.1.9/grai_cli/utilities/validators.py
--rw-r--r--   0        0        0      861 2023-03-19 22:19:53.661091 grai_cli-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 grai_cli-0.1.9/setup.py
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 grai_cli-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      237 2023-05-19 11:07:12.863498 grai_cli-0.2.0a1/README.md
+-rw-r--r--   0        0        0      323 2023-07-18 02:25:32.298110 grai_cli-0.2.0a1/grai_cli/__init__.py
+-rw-r--r--   0        0        0       63 2022-11-09 15:55:13.272679 grai_cli-0.2.0a1/grai_cli/api/__init__.py
+-rw-r--r--   0        0        0       51 2022-07-24 08:00:09.094234 grai_cli-0.2.0a1/grai_cli/api/config/__init__.py
+-rw-r--r--   0        0        0     2024 2023-07-17 16:42:30.681148 grai_cli-0.2.0a1/grai_cli/api/config/config.py
+-rw-r--r--   0        0        0     3632 2023-06-14 21:02:53.335424 grai_cli-0.2.0a1/grai_cli/api/config/set.py
+-rw-r--r--   0        0        0      463 2023-06-14 21:02:53.375897 grai_cli-0.2.0a1/grai_cli/api/config/setup.py
+-rw-r--r--   0        0        0     1317 2023-06-14 21:02:53.291370 grai_cli-0.2.0a1/grai_cli/api/entrypoint.py
+-rw-r--r--   0        0        0       49 2022-07-24 08:00:09.100216 grai_cli-0.2.0a1/grai_cli/api/server/__init__.py
+-rw-r--r--   0        0        0     6030 2023-07-17 20:13:45.162367 grai_cli-0.2.0a1/grai_cli/api/server/endpoints.py
+-rw-r--r--   0        0        0     1094 2023-07-17 16:43:38.992726 grai_cli-0.2.0a1/grai_cli/api/server/setup.py
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273574 grai_cli-0.2.0a1/grai_cli/api/telemetry/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-14 21:02:53.379310 grai_cli-0.2.0a1/grai_cli/api/telemetry/commands.py
+-rw-r--r--   0        0        0       89 2023-03-16 04:12:39.225317 grai_cli-0.2.0a1/grai_cli/config_default.yaml
+-rw-r--r--   0        0        0        0 2022-07-24 06:33:14.647347 grai_cli-0.2.0a1/grai_cli/py.typed
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273862 grai_cli-0.2.0a1/grai_cli/settings/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-18 01:57:07.330038 grai_cli-0.2.0a1/grai_cli/settings/cache.py
+-rw-r--r--   0        0        0     6413 2023-07-18 02:21:27.966349 grai_cli-0.2.0a1/grai_cli/settings/config.py
+-rw-r--r--   0        0        0       88 2023-01-10 17:15:31.923336 grai_cli-0.2.0a1/grai_cli/utilities/__init__.py
+-rw-r--r--   0        0        0     1588 2023-06-01 16:01:43.233062 grai_cli-0.2.0a1/grai_cli/utilities/headers.py
+-rw-r--r--   0        0        0     1180 2023-06-01 16:01:43.233302 grai_cli-0.2.0a1/grai_cli/utilities/styling.py
+-rw-r--r--   0        0        0      796 2023-06-01 16:01:43.233445 grai_cli-0.2.0a1/grai_cli/utilities/telemetry.py
+-rw-r--r--   0        0        0      507 2023-07-17 16:42:57.404252 grai_cli-0.2.0a1/grai_cli/utilities/test.py
+-rw-r--r--   0        0        0     5013 2023-06-14 21:02:53.399455 grai_cli-0.2.0a1/grai_cli/utilities/utilities.py
+-rw-r--r--   0        0        0     2305 2023-06-14 21:02:53.362258 grai_cli-0.2.0a1/grai_cli/utilities/validators.py
+-rw-r--r--   0        0        0     1056 2023-07-18 02:25:32.292022 grai_cli-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 grai_cli-0.2.0a1/PKG-INFO
```

### Comparing `grai_cli-0.1.9/grai_cli/api/config/config.py` & `grai_cli-0.2.0a1/grai_cli/api/config/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,42 +21,43 @@
         ...,
         prompt=True,
         prompt_required=True,
         hide_input=True,
         confirmation_prompt=True,
         callback=strip_style(password_callback),
     ),
-    host: str = typer.Option(
-        default=default_styler(config.server.host),
-        prompt="Server host",
+    url: str = typer.Option(
+        default=default_styler(config.server.url),
+        prompt="Server URL",
         prompt_required=True,
         callback=strip_style(host_callback),
     ),
-    port: str = typer.Option(
-        default=default_styler(config.server.port),
-        prompt="Server port",
-        prompt_required=True,
-        callback=strip_style(port_callback),
-    ),
-    insecure: str = typer.Option(
-        default=default_styler("False"),
-        prompt="Insecure connection (i.e. http)?",
-        prompt_required=True,
-        callback=strip_style(insecure_callback),
-    ),
     workspace: str = typer.Option(
         default=default_styler(config.server.workspace),
         prompt="The Grai workspace for this config",
         prompt_required=True,
         callback=strip_style(workspace_callback),
     ),
 ):
-    """Initialize a new config file"""
+    """Initialize a new config file
+
+    Args:
+        username:  (Default value = typer.Option(..., prompt=True, callback=username_callback, prompt_required=True))
+        password:  (Default value = typer.Option(...,prompt=True,prompt_required=True,hide_input=True,confirmation_prompt=True,callback=strip_style(password_callback))
+        ):
+        url:
+        workspace:  (Default value = typer.Option(default=default_styler(config.server.workspace))
+
+    Returns:
+
+    Raises:
+
+    """
     config.auth = BasicAuthSettings(username=username, password=password)
-    config.server = ServerSettingsV1(host=host, port=port, insecure=insecure, workspace=workspace)
+    config.server = ServerSettingsV1(url=url, workspace=workspace)
     config.save()
 
 
 @config_app.command(help="Print config to console")
 def view():
     """View the current config file"""
     utilities.print(config.view())
```

### Comparing `grai_cli-0.1.9/grai_cli/api/entrypoint.py` & `grai_cli-0.2.0a1/grai_cli/api/entrypoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,25 @@
 import typer
 
 from grai_cli.utilities.telemetry import Telemetry
 from grai_cli.utilities.utilities import HAS_RICH, default_callback
 
 
 def result_callback(*args, **kwargs):
+    """
+
+    Args:
+        *args:
+        **kwargs:
+
+    Returns:
+
+    Raises:
+
+    """
     ctx = click.get_current_context()
     command_path = ctx.meta["command_path"]
     if command_path and command_path[0] != "telemetry":
         command = f"grai {' '.join(command_path)}"
         Telemetry.capture(command)
 
 
@@ -26,16 +37,24 @@
 
 
 @app.callback()
 def callback(
     ctx: typer.Context,
     telemetry: Optional[bool] = typer.Option(None, show_default=False, help="Enable or disable telemetry"),
 ):
-    """
-    Grai CLI
+    """Grai CLI
+
+    Args:
+        ctx (typer.Context):
+        telemetry (Optional[bool], optional):  (Default value = typer.Option(None, show_default=False, help="Enable or disable telemetry"))
+
+    Returns:
+
+    Raises:
+
     """
 
     if telemetry is not None:
         from grai_cli.settings.cache import cache
 
         cache.set("telemetry_consent", telemetry)
```

### Comparing `grai_cli-0.1.9/grai_cli/api/server/endpoints.py` & `grai_cli-0.2.0a1/grai_cli/api/server/endpoints.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,44 +4,50 @@
 import typer
 
 from grai_cli.api.entrypoint import app
 from grai_cli.api.server.setup import client_app, client_get_app, get_default_client
 from grai_cli.utilities import utilities
 from grai_cli.utilities.styling import default_styler
 from grai_cli.utilities.utilities import merge_dicts, write_yaml
+from grai_client.schemas.schema import validate_file
 
 
 @client_app.command("is_authenticated", help="Verify auth credentials are valid")
 def is_authenticated():
+    """ """
     client = get_default_client()
     authentication_status = client.check_authentication()
     if authentication_status.status_code == 200:
         utilities.print("Authenticated")
     else:
         utilities.print(
             f"Failed to Authenticate: Code {authentication_status.status_code}, {authentication_status.content}"
         )
 
 
 def get_nodes(
-    name: Optional[str] = None,
-    namespace: Optional[str] = None,
     print: bool = True,
     to_file: Optional[Path] = None,
+    **kwargs
 ):
+    """
+
+    Args:
+        name (Optional[str], optional):  (Default value = None)
+        namespace (Optional[str], optional):  (Default value = None)
+        print (bool, optional):  (Default value = True)
+        to_file (Optional[Path], optional):  (Default value = None)
+
+    Returns:
+
+    Raises:
+
+    """
     client = get_default_client()
-    if name is None:
-        if namespace is None:
-            result = client.get("Node")
-        else:
-            result = client.get("Node", "*", namespace)
-    elif namespace is None:
-        result = client.get("Node", name)
-    else:
-        result = client.get("Node", name, namespace)
+    result = client.get("Node", **kwargs)
 
     if print:
         utilities.print(result)
     if isinstance(to_file, Path):
         write_yaml(result, to_file)
 
     return result
@@ -50,22 +56,46 @@
 @client_get_app.command("nodes", help=f"Grab active {default_styler('nodes')} from the guide.")
 def get_nodes_cli(
     name: Optional[str] = typer.Argument(None),
     namespace: Optional[str] = typer.Option(None, "--namespace", "-n", help="Namespace of node"),
     print: bool = typer.Option(True, "--p", help=f"Print nodes to console"),
     to_file: Optional[Path] = typer.Option(None, "--f", help="Write nodes to file"),
 ):
+    """
+
+    Args:
+        name (Optional[str], optional):  (Default value = typer.Argument(None))
+        namespace (Optional[str], optional):  (Default value = typer.Option(None, "--namespace", "-n", help="Namespace of node"))
+        print (bool, optional):  (Default value = typer.Option(True, "--p", help=f"Print nodes to console"))
+        to_file (Optional[Path], optional):  (Default value = typer.Option(None, "--f", help="Write nodes to file"))
+
+    Returns:
+
+    Raises:
+
+    """
     return get_nodes(name=name, namespace=namespace, print=print, to_file=to_file)
 
 
 @client_get_app.command("edges", help=f"Grab active {default_styler('edges')} from the guide.")
 def get_edges(
     print: bool = typer.Option(True, "--p", help=f"Print edges to console"),
     to_file: Optional[Path] = typer.Option(None, "--f", help="Write edges to file"),
 ):
+    """
+
+    Args:
+        print (bool, optional):  (Default value = typer.Option(True, "--p", help=f"Print edges to console"))
+        to_file (Optional[Path], optional):  (Default value = typer.Option(None, "--f", help="Write edges to file"))
+
+    Returns:
+
+    Raises:
+
+    """
     client = get_default_client()
     result = client.get("Edge")
 
     if print:
         utilities.print(result)
     if to_file:
         write_yaml(result, to_file)
@@ -75,59 +105,96 @@
 
 @client_get_app.command("workspaces", help=f"Grab active {default_styler('workspaces')} from the guide.")
 def get_workspaces(
     name: str = typer.Argument(None),
     print: bool = typer.Option(True, "--p", help=f"Print workspaces to console"),
     to_file: Optional[Path] = typer.Option(None, "--f", help="Write workspaces to file"),
 ):
+    """
+
+    Args:
+        name (str, optional):  (Default value = typer.Argument(None))
+        print (bool, optional):  (Default value = typer.Option(True, "--p", help=f"Print workspaces to console"))
+        to_file (Optional[Path], optional):  (Default value = typer.Option(None, "--f", help="Write workspaces to file"))
+
+    Returns:
+
+    Raises:
+
+    """
     client = get_default_client()
     if name is None:
         result = client.get("workspaces")
     else:
-        result = client.get("workspaces", name)
+        result = client.get("workspaces", name=name)
 
     if print:
         utilities.print(result)
     if to_file:
         write_yaml(result, to_file)
 
     return result
 
 
 @app.command("apply", help="Apply a configuration to The Guide by file name")
 def apply(
     file: Path = typer.Argument(...),
     dry_run: bool = typer.Option(False, "--d", help="Dry run of file application"),
 ):
-    from grai_client.schemas.schema import validate_file
+    """
+
+    Args:
+        file:  (Default value = typer.Argument(...))
+        dry_run:  (Default value = typer.Option(False, "--d", help="Dry run of file application"))
+
+    Returns:
+
+    Raises:
+
+    """
 
     # TODO: Edges don't have a human readable unique identifier
     client = get_default_client()
     specs = validate_file(file)
 
     if dry_run:
         for spec in specs:
             utilities.print(spec)
         typer.Exit()
 
     for spec in specs:
-        record = client.get(spec)
+        try:
+            record = client.get(spec)
+        except:
+            record = None
+
         if record is None:
             client.post(spec)
         else:
             provided_values = {k: v for k, v in spec.spec.dict().items() if v}
             updated_record = record.update(provided_values)
             client.patch(updated_record)
 
 
 @app.command("delete", help="Delete a configuration from The Guide by file name")
 def delete(
     file: Path = typer.Argument(...),
     dry_run: bool = typer.Option(False, "--d", help="Dry run of file application"),
 ):
+    """
+
+    Args:
+        file (Path, optional):  (Default value = typer.Argument(...))
+        dry_run (bool, optional):  (Default value = typer.Option(False, "--d", help="Dry run of file application"))
+
+    Returns:
+
+    Raises:
+
+    """
     from grai_client.schemas.schema import validate_file
 
     # TODO: Edges don't have a human readable unique identifier
     client = get_default_client()
     specs = validate_file(file)
     if dry_run:
         for spec in specs:
```

### Comparing `grai_cli-0.1.9/grai_cli/api/server/setup.py` & `grai_cli-0.2.0a1/grai_cli/api/server/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,27 +10,34 @@
 from grai_cli.utilities.utilities import default_callback
 
 if TYPE_CHECKING:
     from grai_client.endpoints.client import BaseClient
 
 
 def get_default_client() -> BaseClient:
+    """
+
+    Args:
+
+    Returns:
+
+    Raises:
+
+    """
     from grai_client.endpoints.v1.client import ClientV1
 
     _clients: Dict[str, Type[BaseClient]] = {
         "v1": ClientV1,
     }
-    host = config.server.host
-    port = config.server.port
+    url = config.server.url
     workspace = config.server.workspace
-    insecure = config.server.insecure
-
-    client = _clients[config.server.api_version](host=host, port=port, workspace=workspace, insecure=insecure)
 
+    client = _clients[config.server.api_version](url=url, workspace=workspace)
     authenticate(client)
+
     return client
 
 
 client_app = typer.Typer(no_args_is_help=True, help="Interact with The Guide", callback=default_callback)
 app.add_typer(client_app, name="client")
```

### Comparing `grai_cli-0.1.9/grai_cli/settings/cache.py` & `grai_cli-0.2.0a1/grai_cli/settings/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import os
 import shelve
+import tempfile
 import uuid
+import warnings
 
 import typer
 
 from grai_cli.settings.config import config
-
+from tempfile import NamedTemporaryFile
 
 class GraiCache:
+    """ """
+
     def __init__(self):
         self.cache_filename = "cache"
-        self.cache_file = os.path.join(config.handler.config_dir, self.cache_filename)
+
+        cache_dir = config.handler.config_dir if config.handler.config_dir else tempfile.gettempdir()
+        self.cache_file = os.path.join(cache_dir, self.cache_filename)
 
         with self.cache as cache:
             self.first_install = cache.get("first_install", True)
             self.run_config_init = cache.get("run_config_init", True)
 
             self.has_telemetry_alert = cache.get("has_telemetry_alert", False)
             self.telemetry_consent = cache.get("telemetry_consent", True)
@@ -39,23 +45,56 @@
                 )
                 typer.echo(message)
                 cache["has_telemetry_alert"] = True
             self.has_telemetry_alert = cache["has_telemetry_alert"]
 
     @property
     def cache(self):
+        """ """
+        try:
+            return shelve.open(self.cache_file)
+        except Exception as e:
+            message = (
+                f"Failed to open the cli cache file located at {self.cache_file}. This sometimes indicates cache"
+                f" corruption. We've moved your cache file to {self.cache_file}.bak and replaced it with an empty file."
+            )
+            warnings.warn(message)
+            os.rename(self.cache_file, f"{self.cache_file}.bak")
+
         return shelve.open(self.cache_file)
 
     def set(self, key, value):
+        """
+
+        Args:
+            key:
+            value:
+
+        Returns:
+
+        Raises:
+
+        """
         super().__setattr__(key, value)
 
         with self.cache as cache:
             cache[key] = value
 
     def get(self, key, default=None):
+        """
+
+        Args:
+            key:
+            default:  (Default value = None)
+
+        Returns:
+
+        Raises:
+
+        """
         with self.cache as cache:
             if default:
                 return cache[key]
             else:
                 return cache.get(key, default)
```

### Comparing `grai_cli-0.1.9/grai_cli/settings/config.py` & `grai_cli-0.2.0a1/grai_cli/settings/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,160 +1,210 @@
 import os
 import platform
 import warnings
 from typing import Any, Dict, Literal, Optional, Union
 
 import yaml
 from pydantic import BaseModel, BaseSettings, SecretStr
-from pydantic_yaml import YamlModel, YamlModelMixin, YamlStrEnum
+import warnings
+
+OS = platform.system()
+if OS == "Darwin":
+    _HOME_PATH = os.path.expanduser("~")
+    DEFAULT_CONFIG_PATHS = [f"{_HOME_PATH}/.config/grai"]
+elif OS == "Linux":
+    _HOME_PATH = os.path.expanduser("~")
+    DEFAULT_CONFIG_PATHS = [f"{_HOME_PATH}/.config/grai"]
+elif OS == "Windows":
+    _HOME_PATH = os.getenv("APPDATA")
+    DEFAULT_CONFIG_PATHS = [f"{_HOME_PATH}/grai"]
+elif OS == "":
+    raise Exception("Python could not detect the type of your operating system. ")
+else:
+    warnings.warn(f"Operating system {OS} not recognized. Expected either 'Darwin', 'Windows', or 'Linux'")
+    _HOME_PATH = os.path.expanduser("~")
+    DEFAULT_CONFIG_PATHS = [f"{_HOME_PATH}/.config/grai"]
 
+DEFAULT_CONFIG_PATH = DEFAULT_CONFIG_PATHS[0]
 
 class ConfigDirHandler:
+    """ """
+    DEFAULT_CONFIG_PATHS = DEFAULT_CONFIG_PATHS
+    DEFAULT_CONFIG_PATH = DEFAULT_CONFIG_PATHS[0]
     DEFAULT_CONFIG_FILE_NAMES = ["config.yaml", "config.yml"]
 
     def __init__(self):
-        self.os = platform.system()
-        if self.os == "Darwin":
-            _HOME_PATH = os.path.expanduser("~")
-            config_paths = [f"{_HOME_PATH}/.config/grai"]
-        elif self.os == "Linux":
-            _HOME_PATH = os.path.expanduser("~")
-            config_paths = [f"{_HOME_PATH}/.config/grai"]
-        elif self.os == "Windows":
-            _HOME_PATH = os.getenv("APPDATA")
-            config_paths = [f"{_HOME_PATH}/grai"]
-        elif self.os == "":
-            raise Exception("Python could not detect the type of your operating system. ")
-        else:
-            warnings.warn(f"Operating system {self.os} not recognized. Expected either 'Darwin', 'Windows', or 'Linux'")
-            _HOME_PATH = os.path.expanduser("~")
-            config_paths = [f"{_HOME_PATH}/.config/grai"]
-
-        self.config_paths = config_paths
-        self.default_config_path = self.config_paths[0]
-        self.default_config_file = os.path.join(self.default_config_path, self.DEFAULT_CONFIG_FILE_NAMES[0])
-        self.has_config_file = False
-
-        self.config_dir = self.get_config_dir()
-        self.config_file = self.get_config_file()
-        self._config_content = None
+        path = os.environ.get("GRAI_CLI_CONFIG_DIR", None)
+        self.config_paths = [path, *self.DEFAULT_CONFIG_PATHS] if path is not None else [*self.DEFAULT_CONFIG_PATHS]
+        self.default_config_file = os.path.join(self.DEFAULT_CONFIG_PATH, self.DEFAULT_CONFIG_FILE_NAMES[0])
+
+        self.config_file: str = self.get_config_file()
+        self.has_config_file: bool = self.config_file is not None
+        self.config_dir: Optional[str] = os.path.dirname(self.config_file) if self.has_config_file else None
+
+        self._config_content: Dict = None
+    def get_config_file(self) -> Optional[str]:
+        for path in self.config_paths:
+            for filename in self.DEFAULT_CONFIG_FILE_NAMES:
+                config_file = os.path.join(path, filename)
+                if os.path.exists(config_file):
+                    return config_file
+
+        return None
 
     @property
-    def config_content(self):
+    def config_content(self) -> Dict:
+        """ """
         if isinstance(self._config_content, dict):
             return self._config_content
         elif not self.has_config_file:
             return {}
 
         with open(self.config_file, "r") as file:
-            self._config_content = yaml.safe_load(file)
+            self._config_content= yaml.safe_load(file)
         return self._config_content
 
     @config_content.setter
     def config_content(self, value: Dict):
+        """
+
+        Args:
+            value (Dict):
+
+        Returns:
+
+        Raises:
+
+        """
         if not isinstance(value, dict):
             raise Exception("config_content must be a dictionary")
         self._config_content = value
 
     def save_content(self):
+        """ """
         with open(self.config_file, "w") as file:
             yaml.safe_dump(self._config_content, file)
 
-    def get_config_dir(self) -> str:
-        env_config_dir = os.environ.get("GRAI_CLI_CONFIG_DIR", None)
-
-        if env_config_dir is not None and os.path.exists(env_config_dir):
-            return env_config_dir
-
-        for path in self.config_paths:
-            if os.path.exists(path):
-                return path
-
-        os.mkdir(self.default_config_path)
-        return self.default_config_path
+def unredact(obj: Any) -> Any:
+    """
 
-    def get_config_file(self) -> Optional[str]:
-        for file_name in self.DEFAULT_CONFIG_FILE_NAMES:
-            file = os.path.join(self.config_dir, file_name)
-            if os.path.exists(file):
-                self.has_config_file = True
-                return file
+    Args:
+        obj (Any):
 
-        return self.default_config_file
+    Returns:
 
+    Raises:
 
-def unredact(obj: Any) -> Any:
+    """
     if isinstance(obj, dict):
         return {k: unredact(v) for k, v in obj.items()}
     elif isinstance(obj, SecretStr):
         return obj.get_secret_value()
     else:
         return obj
 
 
 config_handler = ConfigDirHandler()
 
 
 def yaml_config_settings_source(settings: BaseSettings) -> dict[str, Any]:
-    if not config_handler.has_config_file:
-        return {}
-    file = config_handler.config_file
-    with open(file, "r") as file:
-        result = yaml.safe_load(file)
-    return result if result is not None else {}
+    """
+
+    Args:
+        settings:
+
+    Returns:
+
+    Raises:
+
+    """
+    print('yaml loader', config_handler.config_content)
+    return config_handler.config_content
+
 
 
 class ServerSettingsV1(BaseModel):
+    """ """
+
     api_version: Literal["v1"] = "v1"
-    host: str = "localhost"
-    port: str = "8000"
+    url: str
     workspace: str
-    insecure: bool = False
 
     class Config:
+        """ """
+
         validate_assignment = True
 
 
 class AuthModeSettings(BaseModel):
+    """ """
+
     authentication_mode: str
 
     class Config:
+        """ """
+
         validate_assignment = True
 
 
 class BasicAuthSettings(AuthModeSettings):
+    """ """
+
     authentication_mode: Literal["username"] = "username"
     username: str
     password: SecretStr
 
 
 class ApiKeySettings(AuthModeSettings):
+    """ """
+
     authentication_mode: Literal["api_key"] = "api_key"
     api_key: SecretStr
 
 
 class ContextSettings(BaseModel):
+    """ """
+
     namespace: str = "default"
 
 
-class GraiConfig(YamlModelMixin, BaseSettings):
+class GraiConfig(BaseSettings):
+    """ """
+
     server: Union[ServerSettingsV1]
     auth: Union[BasicAuthSettings, ApiKeySettings]
     # context: Optional[ContextSettings]
     handler: ConfigDirHandler = config_handler
 
     def save(self):
+        """ """
         values = unredact(self.dict(exclude={"handler"}))
         with open(self.handler.config_file, "w") as f:
             yaml.dump(values, f)
 
     def view(self):
+        """ """
         return self.yaml(exclude={"handler"})
 
+    @classmethod
+    def default_config(cls):
+        server = ServerSettingsV1(url="http://localhost:8000", workspace="default/default")
+        auth = BasicAuthSettings(username="null@grai.io", password="super_secret")
+        return cls(server=server, auth=auth)
+
+    @classmethod
+    def from_file(cls, file):
+        with open(file, "r") as file:
+            content = yaml.safe_load(file)
+
+        return cls(**content)
+
     class Config:
+        """ """
+
         env_prefix = "grai_"
         validate_assignment = True
         fields = {"server": {}, "auth": {"exclude": {"authentication_mode"}}, "context": {}}
 
         @classmethod
         def customise_sources(
             cls,
@@ -165,27 +215,23 @@
             return (
                 init_settings,
                 env_settings,
                 yaml_config_settings_source,
             )
 
 
-if config_handler.has_config_file:
-    try:
-        config = GraiConfig()
-    except Exception as e:
-        message = f"Unable to construct a complete config file from provided environment variables and/or the config file located at {config_handler.config_file}"
-        raise Exception(message) from e
-else:
-    _default_config = {
-        "auth": {
-            "username": "null@grai.io",
-            "password": "super_secret",
-        },
-        "server": {
-            "host": "localhost",
-            "port": "8000",
-            "insecure": True,
-            "workspace": "default",
-        },
-    }
-    config = GraiConfig(**_default_config)
+try:
+    config = GraiConfig()
+
+except Exception as e:
+    message = (
+        f"We were unable to construct a complete config file from provided environment variables and/or the config file "
+        f"located at {config_handler.config_file}. This most likely means either \n"
+        f"1) The config file is malformed, in which case you can edit it or execute `grai config init` to recreate it.\n"
+        f"2) The config directory is incorrect. We've attempted looking in the following directories: "
+        f"{config_handler.DEFAULT_CONFIG_PATHS} based on our operating system and the `GRAI_CLI_CONFIG_DIR` env var. \n"
+        f"3) You may have made a mistake configuring your environment based purely on environment variables. \n"
+        f"{os.environ.get('GRAI_CLI_CONFIG_DIR')}"
+    )
+    warnings.warn(message)
+    config = GraiConfig.default_config()
+
```

### Comparing `grai_cli-0.1.9/grai_cli/utilities/headers.py` & `grai_cli-0.2.0a1/grai_cli/utilities/headers.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,35 +7,76 @@
 if TYPE_CHECKING:
     from grai_client.endpoints.client import BaseClient
 
 json_headers = {"accept": "application/json", "Content-Type": "application/json"}
 
 
 def get_jwt(self, username: str, password: str) -> Dict:
+    """
+
+    Args:
+        username (str):
+        password (str):
+
+    Returns:
+
+    Raises:
+
+    """
     import requests
 
     response = requests.post(f"{self.api}/token/", headers=self.json_headers, params=self.user_auth_params)
     if response.status_code != 200:
         raise
 
     return response.json()
 
 
 def authenticate_with_username(client: BaseClient) -> BaseClient:
+    """
+
+    Args:
+        client (BaseClient):
+
+    Returns:
+
+    Raises:
+
+    """
     client.authenticate(username=config.auth.username, password=config.auth.password.get_secret_value())
     return client
 
 
 def authenticate_with_api_key(client: BaseClient) -> BaseClient:
+    """
+
+    Args:
+        client (BaseClient):
+
+    Returns:
+
+    Raises:
+
+    """
     client.authenticate(api_key=config.auth.api_key.get_secret_value())
     return client
 
 
 # TODO Switch to pydantic
 def authenticate(client: BaseClient) -> BaseClient:
+    """
+
+    Args:
+        client (BaseClient):
+
+    Returns:
+
+    Raises:
+
+    """
     auth_modes = {
         "username": authenticate_with_username,
         "api_key": authenticate_with_api_key,
     }
 
     auth_mode_id = config.auth.authentication_mode
     auth_mode = auth_modes[auth_mode_id]
```

### Comparing `grai_cli-0.1.9/grai_cli/utilities/telemetry.py` & `grai_cli-0.2.0a1/grai_cli/utilities/telemetry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,54 @@
 import subprocess
 
 from grai_cli.settings.cache import cache
 
 
 def prep_posthog(posthog):
+    """
+
+    Args:
+        posthog:
+
+    Returns:
+
+    Raises:
+
+    """
     posthog.project_api_key = "phc_Q8OCDm0JpCwt4Akk3pMybuBWniWPfOsJzRrdxWjAnjE"
     posthog.host = "https://app.posthog.com"
     posthog.disabled = not cache.telemetry_consent
 
 
 def capture(event):
+    """
+
+    Args:
+        event:
+
+    Returns:
+
+    Raises:
+
+    """
     import posthog
 
     prep_posthog(posthog)
     posthog.capture(cache.telemetry_id, event, groups={"package": "grai-cli"})
 
 
 class Telemetry:
+    """ """
+
     @staticmethod
     def capture(event: str):
+        """
+
+        Args:
+            event (str):
+
+        Returns:
+
+        Raises:
+
+        """
         subprocess.Popen(["grai", "telemetry", "log", event])
```

### Comparing `grai_cli-0.1.9/pyproject.toml` & `grai_cli-0.2.0a1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [tool.poetry]
 name = "grai-cli"
-version = "0.1.9"
+version = "0.2.0-alpha1"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 readme = "README.md"
 packages = [{include = "grai_cli"}]
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-cli"
+documentation = "https://docs.grai.io/"
 
 [tool.poetry.scripts]
 grai = "grai_cli.api.entrypoint:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 multimethod = "^1.9"
 typer = "^0.7.0"
 confuse = "^2.0.0"
 requests = "^2.28.1"
-pydantic = "^1.10.2"
-grai-client = "^0.2.4"
+pydantic = "^1.10.11"
+grai-client = "^0.3.0-alpha25"
 posthog = "^2.2.0"
 rich = "^12.6.0"
-grai-schemas = "^0.1.5"
-pydantic-yaml = "^0.11.1"
+grai-schemas = "^0.2.0a10"
 
 [tool.isort]
 profile = "black"
 known_first_party = "grai_cli"
 
 [tool.black]
 line-length = 120
@@ -38,7 +40,9 @@
 mypy = "^0.991"
 pre-commit = "^2.21.0"
 devtools = "^0.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."grai_cli/__init__.py"]
```

