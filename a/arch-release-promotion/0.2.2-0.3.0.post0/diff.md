# Comparing `tmp/arch-release-promotion-0.2.2.tar.gz` & `tmp/arch_release_promotion-0.3.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch-release-promotion-0.2.2.tar", max compression
+gzip compressed data, was "arch_release_promotion-0.3.0.post0.tar", last modified: Tue Jul 18 06:51:28 2023, max compression
```

## Comparing `arch-release-promotion-0.2.2.tar` & `arch_release_promotion-0.3.0.post0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    35149 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/LICENSE
--rw-r--r--   0        0        0    10812 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/README.rst
--rw-r--r--   0        0        0        0 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/__init__.py
--rw-r--r--   0        0        0     3770 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/argparse.py
--rw-r--r--   0        0        0     5040 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/cli.py
--rw-r--r--   0        0        0    13558 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/config.py
--rw-r--r--   0        0        0    26345 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/files.py
--rw-r--r--   0        0        0     6811 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/gitlab.py
--rw-r--r--   0        0        0     1932 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/release.py
--rw-r--r--   0        0        0     1525 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/signature.py
--rw-r--r--   0        0        0     1777 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/arch_release_promotion/torrent.py
--rw-r--r--   0        0        0     3601 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/examples/example.toml
--rw-r--r--   0        0        0     1165 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/examples/projects.toml
--rw-r--r--   0        0        0     1133 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/examples/systemd/arch-release-sync.service
--rw-r--r--   0        0        0      184 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/examples/systemd/arch-release-sync.timer
--rw-r--r--   0        0        0       60 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/examples/sysusers.d/arch-release-promotion.conf
--rw-r--r--   0        0        0     2801 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1887 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/test_argparse.py
--rw-r--r--   0        0        0     6393 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/test_config.py
--rw-r--r--   0        0        0    28495 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/test_files.py
--rw-r--r--   0        0        0     6325 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/test_gitlab.py
--rw-r--r--   0        0        0      919 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/test_release.py
--rw-r--r--   0        0        0     1444 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/test_signature.py
--rw-r--r--   0        0        0      934 2022-04-14 17:18:13.075691 arch-release-promotion-0.2.2/tests/test_torrent.py
--rw-r--r--   0        0        0    12387 2022-04-14 17:18:18.886712 arch-release-promotion-0.2.2/setup.py
--rw-r--r--   0        0        0    12454 2022-04-14 17:18:18.887271 arch-release-promotion-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/LICENSE
+-rw-r--r--   0        0        0    35149 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/LICENSE
+-rw-r--r--   0        0        0      769 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/Makefile
+-rw-r--r--   0        0        0    10812 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/README.rst
+-rw-r--r--   0        0        0       46 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/__init__.py
+-rw-r--r--   0        0        0     3834 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/argparse.py
+-rw-r--r--   0        0        0     5224 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/cli.py
+-rw-r--r--   0        0        0    14783 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/config.py
+-rw-r--r--   0        0        0    26534 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/files.py
+-rw-r--r--   0        0        0     6877 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/gitlab.py
+-rw-r--r--   0        0        0     1973 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/release.py
+-rw-r--r--   0        0        0     1552 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/signature.py
+-rw-r--r--   0        0        0     1795 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/arch_release_promotion/torrent.py
+-rw-r--r--   0        0        0     3601 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/examples/example.toml
+-rw-r--r--   0        0        0     1165 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/examples/projects.toml
+-rw-r--r--   0        0        0     1133 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/examples/systemd/arch-release-sync.service
+-rw-r--r--   0        0        0      184 2023-07-17 21:24:52.499535 arch_release_promotion-0.3.0.post0/examples/systemd/arch-release-sync.timer
+-rw-r--r--   0        0        0       60 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/examples/sysusers.d/arch-release-promotion.conf
+-rw-r--r--   0        0        0     3923 2023-07-18 06:51:28.296553 arch_release_promotion-0.3.0.post0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/__init__.py
+-rw-r--r--   0        0        0     1887 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/test_argparse.py
+-rw-r--r--   0        0        0     6496 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/test_config.py
+-rw-r--r--   0        0        0    28174 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/test_files.py
+-rw-r--r--   0        0        0     6363 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/test_gitlab.py
+-rw-r--r--   0        0        0      919 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/test_release.py
+-rw-r--r--   0        0        0     1444 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/test_signature.py
+-rw-r--r--   0        0        0      976 2023-07-17 21:24:52.502868 arch_release_promotion-0.3.0.post0/tests/test_torrent.py
+-rw-r--r--   0        0        0    12378 1970-01-01 00:00:00.000000 arch_release_promotion-0.3.0.post0/PKG-INFO
```

### Comparing `arch-release-promotion-0.2.2/LICENSE` & `arch_release_promotion-0.3.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/README.rst` & `arch_release_promotion-0.3.0.post0/README.rst`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/argparse.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/argparse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+"""Argparse module for arch-release-promotion."""
+
 import argparse
 from importlib import metadata
 from sys import exit
 
 
 class ArgParseFactory:
-    """A factory class to create different types of argparse.ArgumentParser instances
+    """A factory class to create different types of argparse.ArgumentParser instances.
 
     Attributes
     ----------
     parser: argparse.ArgumentParser
         The instance's ArgumentParser instance, which is created with a default verbose argument
 
     """
 
     def __init__(self, prog: str = "program", description: str = "default") -> None:
+        """Initialize a new ArgParseFactory."""
         self.parser = argparse.ArgumentParser(prog=prog, description=description)
         self.parser.add_argument(
             "-v",
             "--verbose",
             action="store_true",
             help="verbose output",
         )
@@ -26,22 +29,21 @@
             "--version",
             action="store_true",
             help="version information",
         )
 
     @classmethod
     def promote(self) -> argparse.ArgumentParser:
-        """A class method to create an ArgumentParser for promotion
+        """Create an ArgumentParser for promotion.
 
         Returns
         -------
         argparse.ArgumentParser
             An ArgumentParser instance specific for promotion
         """
-
         instance = self(
             prog="arch-release-promotion",
             description="Download release artifacts from a project and promote them",
         )
         instance.parser.add_argument(
             "-p",
             "--project",
@@ -65,22 +67,21 @@
             print(f"{instance.parser.prog} {metadata.version('arch_release_promotion')}")
             exit(0)
 
         return instance.parser
 
     @classmethod
     def synchronize(self) -> argparse.ArgumentParser:
-        """A class method to create an ArgumentParser for synchronization
+        """Create an ArgumentParser for synchronization.
 
         Returns
         -------
         argparse.ArgumentParser
             An ArgumentParser instance specific for synchronization
         """
-
         instance = self(
             prog="arch-release-sync",
             description="Synchronize promoted releases of a project with a local directory",
         )
         instance.parser.add_argument(
             "-p",
             "--project",
@@ -96,15 +97,15 @@
             print(f"{instance.parser.prog} {metadata.version('arch_release_promotion')}")
             exit(0)
 
         return instance.parser
 
     @classmethod
     def non_zero_string(self, input_: str) -> str:
-        """Validate a string to be of non_zero length
+        """Validate a string to be of non_zero length.
 
         Parameters
         ----------
         input_: str
             A string
 
         Raises
@@ -113,11 +114,10 @@
             If a string is of zero length
 
         Returns
         -------
         str
             A string that is of non-zero length
         """
-
         if len(input_) < 1:
             raise argparse.ArgumentTypeError("the provided string can not be empty")
         return input_
```

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/cli.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""CLI handling."""
+
 from pathlib import Path
 from sys import exit
 from typing import Optional
 
 from arch_release_promotion import (
     argparse,
     config,
@@ -10,26 +12,25 @@
     release,
     signature,
     torrent,
 )
 
 
 def promote_project_release(project: config.ProjectConfig, release_version: Optional[str] = None) -> None:
-    """Promote a project's release
+    """Promote a project's release.
 
     Parameters
     ----------
     project: config.ProjectConfig
         The ProjectConfig object that describes the project's configuration
     release_version: Optional[str]
         The optional release version to promote. If None is provided, interactive user input is required (defaults to
         None)
     """
-
-    settings = config.Settings()
+    settings = config.Settings()  # type: ignore[call-arg]
     upstream = gitlab.Upstream(
         url=settings.GITLAB_URL,
         private_token=settings.PRIVATE_TOKEN,
         name=project.name,
     )
     upstream.auth()
 
@@ -106,33 +107,33 @@
         )
 
     files.remove_temp_dir(path=artifact_temp_dir)
     files.remove_temp_dir(path=promotion_temp_dir)
 
 
 def main() -> None:
+    """Run the main function."""
     args = argparse.ArgParseFactory.promote().parse_args()
     if args.project:
-        project = config.Projects().get_project(name=args.project)
+        project = config.Projects().get_project(name=args.project)  # type: ignore[call-arg]
         promote_project_release(project=project, release_version=args.release if args.release else None)
     else:
-        for project in config.Projects().projects:
+        for project in config.Projects().projects:  # type: ignore[call-arg]
             promote_project_release(project=project)
 
 
 def arch_release_sync() -> None:
-    """Synchronize releases
+    """Synchronize releases.
 
     If the argument parser contains a specific project to synchronize, only synchronize that, else all configured
     projects.
     """
-
     args = argparse.ArgParseFactory.synchronize().parse_args()
-    projects = config.Projects()
-    settings = config.Settings()
+    projects = config.Projects()  # type: ignore[call-arg]
+    settings = config.Settings()  # type: ignore[call-arg]
 
     if args.project:
         files.ProjectFiles.sync(
             project_config=projects.get_project(name=args.project),
             settings=settings,
         )
     else:
```

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/config.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,28 @@
+"""Configuration handling."""
+from __future__ import annotations
+
 from collections import Counter
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Type
+
+try:
+    import tomllib
+except ModuleNotFoundError:  # pragma: no cover
+    import tomli as tomllib  # type: ignore[no-redef]
 
-import toml
 from dotenv import dotenv_values
 from email_validator import EmailNotValidError, validate_email
-from pydantic import BaseModel, BaseSettings, Extra, root_validator, validator
-from pydantic.env_settings import SettingsSourceCallable
+from pydantic import BaseModel, field_validator, model_validator
+from pydantic.fields import FieldInfo
+from pydantic_settings import (
+    BaseSettings,
+    PydanticBaseSettingsSource,
+    SettingsConfigDict,
+)
 from xdg.BaseDirectory import xdg_config_home
 
 MAKEPKG_CONFIGS = [
     Path("/etc/makepkg.conf"),
     Path(f"{xdg_config_home}/pacman/makepkg.conf"),
     Path("~/.makepkg.conf"),
 ]
@@ -21,15 +33,15 @@
 ]
 
 PROJECTS_SYNC_DIR = Path("/var/lib/arch-release-sync/")
 PROJECTS_SYNC_BACKLOG = 3
 
 
 class ReleaseConfig(BaseModel):
-    """A pydantic model describing the configuration of a project's release
+    """A pydantic model describing the configuration of a project's release.
 
     Attributes
     ----------
     name: str
         The name of the release (type)
     version_metrics: Optional[List[str]]
         A list of names that identify labels in metric samples of type "info", that should be extracted from the
@@ -43,23 +55,23 @@
     extensions_to_sign: List[str]
         A list of file extensions for which to create detached signatures
     create_torrent: bool
         A bool indicating whether to create a torrent file for the release (defaults to False)
     """
 
     name: str
-    version_metrics: Optional[List[str]]
-    size_metrics: Optional[List[str]]
-    amount_metrics: Optional[List[str]]
+    version_metrics: Optional[List[str]] = None
+    size_metrics: Optional[List[str]] = None
+    amount_metrics: Optional[List[str]] = None
     extensions_to_sign: List[str]
     create_torrent: bool = False
 
 
 class SyncConfig(BaseModel):
-    """A pydantic model describing configuration for synchronization
+    """A pydantic model describing configuration for synchronization.
 
     Attributes
     ----------
     backlog: int
         The backlog of releases to retain at a maximum (defaults to PROJECTS_SYNC_BACKLOG when a SysConfig instance is
         used in a Projects instance or a ProjectConfig instance).
     directory: Path
@@ -69,22 +81,22 @@
         The optional path to a file, that is used to write a timestamp to, if the synchronization of a project leads to
         the changing of data on disk (defaults to None).
     temp_in_sync_dir: bool
         A bool specifying whether to download temporary data to temporary directories below sync_dir (defaults to True).
         If False is specified the temporary data is downloaded to the respective user's temporary directory.
     """
 
-    backlog: Optional[int]
-    directory: Optional[Path]
+    backlog: Optional[int] = None
+    directory: Optional[Path] = None
     last_updated_file: Optional[Path] = None
     temp_in_sync_dir: bool = True
 
 
 class ProjectConfig(BaseModel):
-    """A pydantic model describing the configuration of a project
+    """A pydantic model describing the configuration of a project.
 
     Attributes
     ----------
     name: str
         The name of the project
     job_name: str
         The project's job, that offers release artifacts
@@ -99,48 +111,50 @@
     """
 
     name: str
     job_name: str
     output_dir: Path
     metrics_file: Path
     releases: List[ReleaseConfig]
-    sync_config: Optional[SyncConfig]
+    sync_config: Optional[SyncConfig] = None
 
 
 class Projects(BaseSettings):
-    """A pydantic BaseSettings class to describe sets of project settings
+    """A pydantic BaseSettings class to describe sets of project settings.
 
     Attributes
     ----------
     projects: List[ProjectConfig]
         A list of project configurations
     sync_config: Optional[SyncConfig]
         An optional SyncConfig instance, which is used to override any implicit defaults and sets defaults for all
         ProjectConfig instances in projects.
     """
 
     projects: List[ProjectConfig]
-    sync_config: Optional[SyncConfig]
-
-    class Config:
+    sync_config: Optional[SyncConfig] = None
 
-        extra = Extra.ignore
+    model_config = SettingsConfigDict(extra="ignore")
 
-        @classmethod
-        def customise_sources(
-            cls,
-            init_settings: SettingsSourceCallable,
-            env_settings: SettingsSourceCallable,
-            file_secret_settings: SettingsSourceCallable,
-        ) -> Tuple[SettingsSourceCallable, ...]:
-            return (read_projects_conf,)
+    @classmethod
+    def settings_customise_sources(
+        cls,
+        settings_cls: Type[BaseSettings],
+        init_settings: PydanticBaseSettingsSource,
+        env_settings: PydanticBaseSettingsSource,
+        dotenv_settings: PydanticBaseSettingsSource,
+        file_secret_settings: PydanticBaseSettingsSource,
+    ) -> Tuple[PydanticBaseSettingsSource, ...]:
+        """Customize the configuration source assembly."""
+        return (TomlConfig(settings_cls),)
 
-    @validator("projects")
+    @field_validator("projects")
+    @classmethod
     def validate_project_releases_unique(cls, projects: List[ProjectConfig]) -> List[ProjectConfig]:
-        """Validate the list of ProjectConfig instances to only contain uniquely named ReleaseConfig instances
+        """Validate the list of ProjectConfig instances to only contain uniquely named ReleaseConfig instances.
 
         Parameters
         ----------
         projects: List[ProjectConfig]
             A list of ProjectConfig instances
 
         Raises
@@ -149,15 +163,14 @@
             If a non-unique name is encountered among any ReleaseConfig instance
 
         Returns
         -------
         List[ProjectConfig]
             The unmodified list of ProjectConfig instances
         """
-
         release_types: List[ReleaseConfig] = []
         for project in projects:
             release_types += project.releases
         names = [release_type.name for release_type in release_types]
 
         if len(set(names)) < len(names):
             duplicates = [name for name, count in Counter(names).items() if count > 1]
@@ -165,17 +178,17 @@
                 f"The following release type {'name' if len(duplicates) == 1 else 'names'} "
                 f"{'is' if len(duplicates) == 1 else 'are'} not unique: "
                 f"{duplicates[0] if len(duplicates) == 1 else duplicates}"
             )
 
         return projects
 
-    @root_validator
+    @model_validator(mode="before")
     def validate_projects(cls, values: Dict[str, Any]) -> Dict[str, Any]:
-        """Validate the list of ProjectConfig instances and override defaults
+        """Validate the list of ProjectConfig instances and override defaults.
 
         If a ProjectConfig does not specify a SysConfig, override it with the global SysConfig. If a global SysConfig
         does not exist, override with an implicit default where directory defaults to PROJECTS_SYNC_DIR and backlog to
         PROJECTS_SYNC_BACKLOG.
 
         Parameters
         ----------
@@ -183,54 +196,39 @@
             A dict with all values of the Projects instance
 
         Returns
         -------
         values: Dict[str, Any]
             The (potentially modified) dict with all values of the Projects instance
         """
-
         default_sync_config = SyncConfig(
             directory=PROJECTS_SYNC_DIR,
             backlog=PROJECTS_SYNC_BACKLOG,
             last_updated_file=None,
         )
 
-        projects: List[ProjectConfig] = values.get("projects")  # type: ignore
-        sync_config: Optional[SyncConfig] = values.get("sync_config")
+        projects: List[Dict[str, Any]] = values.get("projects") or []
+        sync_config: Optional[Dict[str, Any]] = values.get("sync_config")
 
         # merge global sync_config with defaults
         if sync_config:
-            global_sync_config = SyncConfig(
-                directory=sync_config.directory or default_sync_config.directory,
-                backlog=sync_config.backlog or default_sync_config.backlog,
-                last_updated_file=sync_config.last_updated_file or default_sync_config.last_updated_file,
-                temp_in_sync_dir=False if not sync_config.temp_in_sync_dir else default_sync_config.temp_in_sync_dir,
-            )
+            global_sync_config = sync_config | default_sync_config.model_dump()
         else:
-            global_sync_config = default_sync_config
+            global_sync_config = default_sync_config.model_dump()
 
         for project in projects:
-            if not project.sync_config:
-                project.sync_config = global_sync_config
+            if not project.get("sync_config"):
+                project["sync_config"] = global_sync_config
             else:
-                project.sync_config = SyncConfig(
-                    directory=project.sync_config.directory or global_sync_config.directory,
-                    backlog=project.sync_config.backlog or global_sync_config.backlog,
-                    last_updated_file=project.sync_config.last_updated_file or global_sync_config.last_updated_file,
-                    temp_in_sync_dir=False
-                    if not project.sync_config.temp_in_sync_dir
-                    else global_sync_config.temp_in_sync_dir,
-                )
-
-        values["projects"] = projects
+                project["sync_config"] = project.get("sync_config") | global_sync_config  # type: ignore[operator]
 
-        return values
+        return {"projects": projects, "sync_config": sync_config}
 
     def get_project(self, name: str) -> ProjectConfig:
-        """Return a ProjectConfig by name
+        """Return a ProjectConfig by name.
 
         Parameters
         ----------
         name: str
             A string that matches the name attribute of a ProjectConfig
 
         Raises
@@ -239,51 +237,87 @@
             If no ProjectConfig instance of the given name can be found
 
         Returns
         -------
         ProjectConfig
             The configuration identified by the provided name
         """
-
         for project in self.projects:
             if project.name == name:
                 return project
 
         raise RuntimeError(f"No project configuration of the name '{name}' can be found!")
 
 
-def read_projects_conf(settings: BaseSettings) -> Dict[str, Any]:
-    """Read all available projects.toml files"""
+class TomlConfig(PydanticBaseSettingsSource):
+    """A TOML config reader."""
+
+    def get_field_value(self, field: FieldInfo, field_name: str) -> Any:  # pragma: no cover
+        """
+        Get the value, the key for model creation, and a flag to determine whether value is complex.
 
-    config: Dict[str, Any] = {}
-    config_files: List[str] = []
-    for config_file in PROJECTS_CONFIGS:
-        if config_file.exists():
-            config_files += [str(config_file)]
+        Parameters
+        ----------
+            field: The field.
+            field_name: The field name.
 
-    if config_files:
-        config.update(toml.load(config_files))
-    else:
-        raise RuntimeError("There are no project configuration files!")
+        Returns
+        -------
+            A tuple containing the key, value and a boolean to determine whether value is complex.
+        """
+        pass
 
-    return config
+    def __call__(self) -> dict[str, Any]:
+        """Read all available projects.toml files."""
+        output_dict: dict[str, Any] = {}
+        config_files: List[Path] = []
+        for config_file in PROJECTS_CONFIGS:
+            if config_file.exists():
+                config_files += [config_file]
 
+        if not config_files:
+            raise RuntimeError("There are no project configuration files!")
 
-def read_makepkg_conf(settings: BaseSettings) -> Dict[str, Any]:
-    """Read all available makepkg.conf files"""
+        for config_file in config_files:
+            with open(config_file, "rb") as file:
+                file_dict = tomllib.load(file)
+                output_dict = output_dict | file_dict
 
-    config: Dict[str, Optional[str]] = {}
-    for config_file in MAKEPKG_CONFIGS:
-        config.update(dotenv_values(config_file.expanduser()))
+        return output_dict
 
-    return config
+
+class MakepkgConfig(PydanticBaseSettingsSource):
+    """A makepkg config reader."""
+
+    def get_field_value(self, field: FieldInfo, field_name: str) -> Any:  # pragma: no cover
+        """
+        Get the value, the key for model creation, and a flag to determine whether value is complex.
+
+        Parameters
+        ----------
+            field: The field.
+            field_name: The field name.
+
+        Returns
+        -------
+            A tuple containing the key, value and a boolean to determine whether value is complex.
+        """
+        pass
+
+    def __call__(self) -> dict[str, Any]:
+        """Read all available projects.toml files."""
+        config: Dict[str, Optional[str]] = {}
+        for config_file in MAKEPKG_CONFIGS:
+            config.update(dotenv_values(config_file.expanduser()))
+
+        return config
 
 
 class Settings(BaseSettings):
-    """A class to describe configuration
+    """A class to describe configuration.
 
     Attributes
     ----------
     GITLAB_URL: str
         A URL for a GitLab upstream (defaults to "https://gitlab.archlinux.org")
     GPGKEY: str
         The PGP key id to use for artifact signatures
@@ -296,35 +330,37 @@
         An optional private token to use for authenticating against an upstream
     """
 
     GITLAB_URL: str = "https://gitlab.archlinux.org"
     GPGKEY: str
     MIRRORLIST_URL: str = "https://archlinux.org/mirrorlist/?country=all&protocol=http&protocol=https"
     PACKAGER: str
-    PRIVATE_TOKEN: Optional[str]
+    PRIVATE_TOKEN: Optional[str] = None
 
-    class Config:
+    model_config = SettingsConfigDict(extra="ignore")
 
-        extra = Extra.ignore
-
-        @classmethod
-        def customise_sources(
-            cls,
-            init_settings: SettingsSourceCallable,
-            env_settings: SettingsSourceCallable,
-            file_secret_settings: SettingsSourceCallable,
-        ) -> Tuple[SettingsSourceCallable, ...]:
-            return (
-                read_makepkg_conf,
-                env_settings,
-            )
+    @classmethod
+    def settings_customise_sources(
+        cls,
+        settings_cls: Type[BaseSettings],
+        init_settings: PydanticBaseSettingsSource,
+        env_settings: PydanticBaseSettingsSource,
+        dotenv_settings: PydanticBaseSettingsSource,
+        file_secret_settings: PydanticBaseSettingsSource,
+    ) -> Tuple[PydanticBaseSettingsSource, ...]:
+        """Customize the sources for configuration."""
+        return (
+            MakepkgConfig(settings_cls),
+            env_settings,
+        )
 
-    @validator("PACKAGER")
+    @field_validator("PACKAGER")
+    @classmethod
     def validate_packager(cls, packager: str) -> str:
-        """A validator for the PACKAGER attribute
+        """Validate the PACKAGER attribute.
 
         Parameters
         ----------
         packager: str
             The packager string to validate
 
         Raises
@@ -333,32 +369,32 @@
             If the packager string is not valid
 
         Returns
         -------
         str
             A valid packager string
         """
-
         if len(packager) == 0:
             raise ValueError("The PACKAGER string can not be empty.")
         if not ("<" in packager and ">" in packager):
             raise ValueError(f"The PACKAGER string has to define a mail address: {packager}")
         split_packager = packager.replace(">", "").split("<")
         if len(split_packager[0]) < 1:
             raise ValueError(f"The PACKAGER string has to define a name: {packager}")
         try:
             validate_email(split_packager[1])
         except EmailNotValidError as e:
             raise ValueError(f"The PACKAGER string has to define a valid mail address: {packager}\n{e}")
 
         return packager
 
-    @validator("GPGKEY")
+    @field_validator("GPGKEY")
+    @classmethod
     def validate_gpgkey(cls, gpgkey: str) -> str:
-        """A validator for the GPGKEY attribute
+        """Validate the GPGKEY attribute.
 
         Parameters
         ----------
         gpgkey: str
             The packager string to validate
 
         Raises
@@ -367,23 +403,23 @@
             If the gpgkey string is not valid
 
         Returns
         -------
         str
             A gpgkey string in long-format
         """
-
         if len(gpgkey) < 40:
             raise ValueError(f"The GPGKEY string has to represent a PGP key ID in long format (40 chars): {gpgkey}")
 
         return gpgkey
 
-    @validator("PRIVATE_TOKEN")
+    @field_validator("PRIVATE_TOKEN")
+    @classmethod
     def validate_private_token(cls, private_token: Optional[str]) -> Optional[str]:
-        """A validator for the PRIVATE_TOKEN attribute
+        """Validate the PRIVATE_TOKEN attribute.
 
         Parameters
         ----------
         private_token: str
             The private token string to validate
 
         Raises
@@ -392,15 +428,14 @@
             If the private token string is not valid
 
         Returns
         -------
         str
             A gpgkey string in long-format
         """
-
         if private_token is None:
             return None
 
         if len(private_token) < 20:
             raise ValueError("The PRIVATE_TOKEN string has to represent a valid private token (20 chars).")
 
         return private_token
```

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/files.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,34 @@
+"""Local file handling."""
+
 import shutil
 import tempfile
 import time
 import zipfile
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 import orjson
 from prometheus_client.parser import text_fd_to_metric_families
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from arch_release_promotion.config import ProjectConfig, Settings
 from arch_release_promotion.gitlab import Upstream
 from arch_release_promotion.release import (
     AmountMetric,
     Release,
     SizeMetric,
     VersionMetric,
 )
 
 TEMP_DIR_PREFIX = "arp-"
 
 
 def files_in_dir(path: Path) -> List[str]:
-    """Return the files in a directory as a list of strings
+    """Return the files in a directory as a list of strings.
 
     Parameters
     ----------
     path: Path
         The path for which to list files
 
     Raises
@@ -35,23 +37,22 @@
         If the provided path is not a directory
 
     Returns
     -------
     List[str]
         A list of strings representing the files in a directory
     """
-
     if not path.is_dir():
         raise RuntimeError(f"The path is not a path: {path}")
 
     return [child.name for child in path.iterdir()]
 
 
 def get_version_from_artifact_release_dir(path: Path) -> str:
-    """Extrapolate the version of a given release path
+    """Extrapolate the version of a given release path.
 
     Parameters
     ----------
     path: Path
         The path to a release
 
     Raises
@@ -60,108 +61,103 @@
         If the provided path is not a directory
 
     Returns
     -------
     str
         The version string for the release
     """
-
     if not path.is_dir():
         raise RuntimeError(f"The path for the release is not a directory: {path}")
 
     version = path.name.split("-")[1]
     if len(version) < 1:
         raise RuntimeError(f"The extracted version string '{version}' from path '{path}' is not valid.")
 
     return version
 
 
 def create_temp_dir() -> Path:
-    """Create a temporary directory
+    """Create a temporary directory.
 
     Returns
     -------
     Path
         The path to the directory
     """
-
     return Path(tempfile.mkdtemp(prefix=TEMP_DIR_PREFIX))
 
 
 def remove_temp_dir(path: Path) -> None:
-    """Remove a temporary directory recursively
+    """Remove a temporary directory recursively.
 
     Parameters
     ----------
     path: Path
         The path to a directory to remove
 
     Raises
     ------
     RuntimeError
         If the to be removed path is not a directory or if its name does not contain TEMP_DIR_PREFIX
     """
-
     if not path.is_dir():
         raise RuntimeError(f"The path to remove is not a directory: {path}")
 
     if TEMP_DIR_PREFIX not in path.name:
         raise RuntimeError(f"Can not remove a temporary directory, that is not created by the same tool: {path}")
 
     shutil.rmtree(path=path)
 
 
 def extract_zip_file_to_parent_dir(path: Path) -> None:
-    """Extract the contents of a ZIP file to the parent directory of that file
+    """Extract the contents of a ZIP file to the parent directory of that file.
 
     Parameters
     ----------
     path: Path
         The path to a ZIP file
 
     Raises
     ------
     RuntimeError
         If the path does not specify a valid zip file
     """
-
     if not zipfile.is_zipfile(path):
         raise RuntimeError(f"The file is not a ZIP file: {path}")
 
     with zipfile.ZipFile(file=path, mode="r") as zip_file:
         zip_file.extractall(path=path.parent)
 
 
 def copy_signatures(source: Path, destination: Path) -> None:
-    """Copy any signature files from a source directory to a destination directory
+    """Copy any signature files from a source directory to a destination directory.
 
     Parameters
     ----------
     source: Path
         The source directory to copy signature files from
     destination: Path
         The destination directory to copy signature files to
 
     Raises
     ------
     RuntimeError
         If either source or destination is not a directory
     """
-
     for path in [source, destination]:
         if not path.is_dir():
             raise RuntimeError("The specified path is not a directory: {path}")
 
     for file in source.iterdir():
         if file.suffix in [".sig"]:
             shutil.copy(src=file, dst=destination)
 
 
 def write_release_info_to_file(release: Release, path: Path) -> None:
-    """Write a Release instance to a JSON file
+    """Write a Release instance to a JSON file.
 
     Parameters
     ----------
     release: Release
         A release instance that will be serialized to JSON
     path: Path
         The file to write the JSON string to
@@ -169,52 +165,51 @@
     Raises
     ------
     IsADirectoryError:
         If the path is a directory
     OSError:
         If the file path is not writable
     """
-
     with open(path, "wb") as file:
         file.write(
-            orjson.dumps(release.dict(), option=orjson.OPT_INDENT_2 | orjson.OPT_APPEND_NEWLINE | orjson.OPT_SORT_KEYS)
+            orjson.dumps(
+                release.model_dump(), option=orjson.OPT_INDENT_2 | orjson.OPT_APPEND_NEWLINE | orjson.OPT_SORT_KEYS
+            )
         )
 
 
 def load_release_from_json_payload(path: Path) -> Release:
-    """Read a JSON payload and return it as a Release instance
+    """Read a JSON payload and return it as a Release instance.
 
     Parameters
     ----------
     path: Path
         The path to a file containing a JSON payload
 
     Returns
     -------
     Release
         A Release instance reflecting the data from the JSON payload
     """
-
     with open(path, "r") as file:
         return Release(**orjson.loads(file.read()))
 
 
 def write_zip_file_to_parent_dir(path: Path, name: str = "promotion", format: str = "zip") -> None:
-    """Create ZIP file of all contents in a directory and write it to the directory's parent
+    """Create ZIP file of all contents in a directory and write it to the directory's parent.
 
     Parameters
     ----------
     path: Path
         The path to add to the ZIP file
     name: str
         The name to use for the compressed file (defaults to "promotion")
     format: str
         The compressed file format to use (defaults to "zip")
     """
-
     known_formats = ["zip", "tar", "gztar", "bztar", "xztar"]
     if len(name) < 1:
         raise RuntimeError("The file name has to be at least one char long, but empty string was provided.")
     if format not in known_formats:
         raise RuntimeError(f"The format must be one of {known_formats}, but {format} is provided.")
 
     shutil.make_archive(base_name=str(path.parent / Path(name)), format=format, root_dir=path)
@@ -222,15 +217,15 @@
 
 def read_metrics_file(
     path: Path,
     version_metrics_names: Optional[List[str]],
     size_metrics_names: Optional[List[str]],
     amount_metrics_names: Optional[List[str]],
 ) -> Tuple[List[AmountMetric], List[SizeMetric], List[VersionMetric]]:
-    """Read a metrics file that contains openmetrics based metrics and return those that match the respective keywords
+    """Read a metrics file that contains openmetrics based metrics and return those that match the respective keywords.
 
     Parameters
     ----------
     path: Path
         The path of the file to read
     version_metrics_names: Optional[List[str]]
         A list of metric names to search for in the labels of metric samples of type "info"
@@ -240,74 +235,73 @@
         A list of metric names to search for in the labels of metric samples of type "summary"
 
     Returns
     -------
     Tuple[List[AmountMetric], List[SizeMetric], List[VersionMetric]]:
         A Tuple with lists of AmountMetric, SizeMetric and VersionMetric instances derived from the input file
     """
-
     amount_metrics: List[AmountMetric] = []
     size_metrics: List[SizeMetric] = []
     version_metrics: List[VersionMetric] = []
 
     if path.exists():
         with open(path, "r") as file:
-            for metric in text_fd_to_metric_families(file):  # type: ignore[no-untyped-call]
+            for metric in text_fd_to_metric_families(file):
                 for sample in metric.samples:
                     if (
                         version_metrics_names
                         and metric.type == "info"
                         and metric.name == "version_info"
                         and sample.labels.get("name") in version_metrics_names
                         and sample.labels.get("description")
                         and sample.labels.get("version")
                     ):
                         version_metrics += [
                             VersionMetric(
-                                name=sample.labels.get("name"),
-                                description=sample.labels.get("description"),
-                                version=sample.labels.get("version"),
+                                name=sample.labels.get("name"),  # type: ignore[arg-type]
+                                description=sample.labels.get("description"),  # type: ignore[arg-type]
+                                version=sample.labels.get("version"),  # type: ignore[arg-type]
                             )
                         ]
                     if (
                         size_metrics_names
                         and metric.type == "gauge"
                         and metric.name == "artifact_bytes"
                         and sample.labels.get("name") in size_metrics_names
                         and sample.labels.get("description")
                         and sample.value
                     ):
                         size_metrics += [
                             SizeMetric(
-                                name=sample.labels.get("name"),
-                                description=sample.labels.get("description"),
+                                name=sample.labels.get("name"),  # type: ignore[arg-type]
+                                description=sample.labels.get("description"),  # type: ignore[arg-type]
                                 size=sample.value,
                             )
                         ]
                     if (
                         amount_metrics_names
                         and metric.type == "summary"
                         and metric.name == "data_count"
                         and sample.labels.get("name") in amount_metrics_names
                         and sample.labels.get("description")
                         and sample.value
                     ):
                         amount_metrics += [
                             AmountMetric(
-                                name=sample.labels.get("name"),
-                                description=sample.labels.get("description"),
-                                amount=sample.value,
+                                name=sample.labels.get("name"),  # type: ignore[arg-type]
+                                description=sample.labels.get("description"),  # type: ignore[arg-type]
+                                amount=int(sample.value),
                             )
                         ]
 
     return (amount_metrics, size_metrics, version_metrics)
 
 
 def create_dir(path: Path) -> Path:
-    """Create a directory
+    """Create a directory.
 
     Parameters
     ----------
     path: Path
         The path for which to create a directory
 
     Raises
@@ -316,59 +310,55 @@
         If the path exists but is not a directory
 
     Returns
     -------
     Path
         The path representing the existing, absolute directory
     """
-
     path = path.resolve(strict=False)
 
     if path.exists() and not path.is_dir():
         raise RuntimeError(f"The provided path is not a directory: {path}")
     else:
         path.mkdir(parents=True, exist_ok=True)
 
     return path
 
 
 class ProjectFiles(BaseModel):
-    """A pydantic model to operate on a project's files and releases
+    """A pydantic model to operate on a project's files and releases.
 
     Attributes
     ----------
     project_config: ProjectConfig
         A ProjectConfig instance describing the project
     upstream: Upstream
         An Upstream instance used for queries to releases of a project
     promoted_releases: List[str]
         A list of version strings
     """
 
     project_config: ProjectConfig
     upstream: Upstream
     promoted_releases: List[str]
-
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def __init__(self, project_config: ProjectConfig, settings: Settings) -> None:
-        """A custom constructor to initialize an instance of ProjectFiles
+        """Initialize an instance of ProjectFiles.
 
         The names of the configured maximum number of promoted releases is retrieved using an Upstream instance.
         If the project's sync_dir does not exist, it will be created.
 
         Parameters
         ----------
         project_config: ProjectConfig
             A ProjectConfig instance describing the project
         settings: Settings
             A Settings instance used to initialize an Upstream instance
         """
-
         upstream = Upstream(
             url=settings.GITLAB_URL,
             private_token=None,
             name=project_config.name,
         )
         promoted_releases = upstream.get_releases(
             max_releases=project_config.sync_config.backlog,  # type: ignore
@@ -382,24 +372,23 @@
             project_config=project_config,
             upstream=upstream,
             promoted_releases=promoted_releases,
         )
 
     @classmethod
     def sync(self, project_config: ProjectConfig, settings: Settings) -> None:
-        """A factory method to initialize an instance of ProjectFiles and synchronize all of its promoted_releases
+        """Initialize an instance of ProjectFiles and synchronize all of its promoted_releases.
 
         Parameters
         ----------
         project_config: ProjectConfig
             A ProjectConfig instance describing the project
         settings: Settings
             A Settings instance used to initialize an Upstream instance
         """
-
         change_state: List[bool] = []
 
         project_files = self(
             project_config=project_config,
             settings=settings,
         )
 
@@ -422,26 +411,24 @@
         change_state += [project_files._set_latest_version_symlink()]
         change_state += [project_files._remove_obsolete_releases()]
 
         if any(change_state):
             project_files._set_last_update_file_timestamp()
 
     def _set_last_update_file_timestamp(self) -> None:
-        """Write the current seconds since the epoch to a "last update file" if it is configured"""
-
+        """Write the current seconds since the epoch to a "last update file" if it is configured."""
         if self.project_config.sync_config.last_updated_file:  # type: ignore
             print(f"Updating timestamp in {self.project_config.sync_config.last_updated_file}...")  # type: ignore
             with open(self.project_config.sync_config.last_updated_file, "w") as file:  # type: ignore
                 file.write(f"{int(time.time())}")
 
             print("Done!")
 
     def _remove_obsolete_releases(self) -> bool:
-        """Remove obsolete releases of a project from its sync_dir"""
-
+        """Remove obsolete releases of a project from its sync_dir."""
         state: List[bool] = []
         expected_dirs: List[Path] = []
         expected_files: List[Path] = []
 
         for release_type in self.project_config.releases:
             release_type_dir = self.project_config.sync_config.directory / Path(release_type.name)  # type: ignore
             print(f"Removing obsolete release files from '{release_type_dir}'...")
@@ -468,16 +455,15 @@
                     state += [True]
 
             print("Done!")
 
         return any(state)
 
     def _set_latest_version_symlink(self) -> bool:
-        """Set the symlink to the latest version in a project's sync_dir"""
-
+        """Set the symlink to the latest version in a project's sync_dir."""
         state: List[bool] = []
 
         if self.promoted_releases:
             latest_version = sorted(self.promoted_releases)[-1]
 
             for release_type in self.project_config.releases:
                 latest_link = (
@@ -496,15 +482,15 @@
                     state += [True]
 
             print("Done!")
 
         return any(state)
 
     def _sync_version(self, temp_dir_base: Optional[Path], version: str) -> bool:
-        """Synchronize a project's (release) version
+        """Synchronize a project's (release) version.
 
         Download a project release's promotion artifact and use it to establish whether the release version has been
         synchronized fully to the project's sync_dir.
         Download the project release's build artifact, if the release version is not yet (fully) synchronized and move
         the combined artifacts to the project's sync_dir.
 
         Parameters
@@ -515,15 +501,14 @@
             The project's release version
 
         Returns
         -------
         bool
             True if the synchronization introduced changes in the synchronization directory, False otherwise
         """
-
         with tempfile.TemporaryDirectory(prefix=TEMP_DIR_PREFIX, dir=temp_dir_base) as promotion_temp_dir_name:
             promotion_temp_dir = Path(promotion_temp_dir_name)
             extract_zip_file_to_parent_dir(
                 path=self.upstream.download_promotion_artifact(
                     tag_name=version,
                     temp_dir=promotion_temp_dir,
                 )
@@ -559,29 +544,28 @@
                         )
 
                     return True
 
             return False
 
     def _is_release_type_synced(self, name: str, version: str) -> bool:
-        """Check whether a release type of a project's release version is synchronized fully already
+        """Check whether a release type of a project's release version is synchronized fully already.
 
         Parameters
         ----------
         name: str
             The release name
         version: str
             The release version
 
         Returns
         -------
         bool
             True if the project's release type in the specified version is fully synchronized, False otherwise
         """
-
         release_base = self.project_config.sync_config.directory / Path(name)  # type: ignore
         release_json = release_base / Path(f"{name}-{version}.json")
         if not release_json.exists():
             return False
 
         release = load_release_from_json_payload(path=release_json)
 
@@ -595,27 +579,26 @@
 
         return True
 
     def _project_version_requires_sync(
         self,
         version: str,
     ) -> bool:
-        """Evaluate whether a project's release requires syncing
+        """Evaluate whether a project's release requires syncing.
 
         Parameters
         ----------
         version: str
             The version of the project's release
 
         Returns
         -------
         bool
             True if any of the release types of the project are not yet fully synchronized, False otherwise
         """
-
         release_type_states: List[bool] = []
         for project_release_type in self.project_config.releases:
             if not self._is_release_type_synced(
                 name=project_release_type.name,
                 version=version,
             ):
                 release_type_states += [True]
@@ -627,26 +610,25 @@
     @classmethod
     def copy_release_type_promotion_artifacts_to_build_dir(
         self,
         release_type: Release,
         source_base: Path,
         destination_base: Path,
     ) -> None:
-        """Copy promotion artifacts of a release type to its respective build artifact directory
+        """Copy promotion artifacts of a release type to its respective build artifact directory.
 
         Parameters
         ----------
         release_type: Release
             The Release instance describing the files to copy
         source_base: Path
             The base directory in which the promotion artifacts of the release type are located
         destination_base: Path
             The base directory in which the build artifacts of the release type are located
         """
-
         copy_signatures(
             source=source_base / Path(f"{release_type.name}/{release_type.name}-{release_type.version}"),
             destination=destination_base / Path(f"{release_type.name}/{release_type.name}-{release_type.version}"),
         )
         # move torrent file if it exists
         if release_type.torrent_file:
             (source_base / Path(f"{release_type.name}/{release_type.torrent_file}")).rename(
@@ -655,29 +637,28 @@
         # move JSON payload
         (source_base / Path(f"{release_type.name}/{release_type.name}-{release_type.version}.json")).rename(
             (destination_base / Path(f"{release_type.name}/{release_type.name}-{release_type.version}.json"))
         )
 
     @classmethod
     def validate_release_type_files(self, release_type: Release, path: Path) -> None:
-        """Validate the files of a release type
+        """Validate the files of a release type.
 
         Parameters
         ----------
         release_type: Release
             The Release instance describing the release type
         path: Path
             The directory in which the files for the release type are located
 
         Raises
         ------
         RuntimeError
             If one of the files is missing
         """
-
         print(f"Validating release type '{release_type.name}' version '{release_type.version}'...")
 
         json_payload = Path(f"{release_type.name}/{release_type.name}-{release_type.version}.json")
         if not (path / json_payload).exists():
             raise RuntimeError(f"The file '{json_payload}' does not exist.")
 
         torrent_file = Path(f"{release_type.name}/{release_type.name}-{release_type.version}.torrent")
@@ -689,26 +670,25 @@
             if not (path / file_path).exists():
                 raise RuntimeError(f"The file '{file_path}' does not exist.")
 
         print("Done!")
 
     @classmethod
     def move_release_type_to_sync_dir(self, release: Release, source_base: Path, sync_dir: Path) -> None:
-        """Move a validated version of a release type to a sync directory
+        """Move a validated version of a release type to a sync directory.
 
         Parameters
         ----------
         release_type: Release
             The Release instance describing the release type
         source_base: Path
             The directory in which the files for the release type are located
         sync_dir: Path
             The directory to which the release type files are moved
         """
-
         print(f"Moving release type '{release.name}' version '{release.version}' to '{sync_dir}'...")
 
         release_type_base = sync_dir / Path(f"{release.name}")
         create_dir(release_type_base)
         destination_release_dir = release_type_base / Path(f"{release.name}-{release.version}")
 
         # if the destination exists already, remove it first
```

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/gitlab.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/gitlab.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,79 +1,78 @@
+"""GitLab interaction."""
+
 from pathlib import Path
 from typing import List, Optional
 from urllib import request
 
 import gitlab
 
 
 class Upstream(gitlab.Gitlab):
-    """A class to interact with a gitlab instance
+    """A class to interact with a gitlab instance.
 
     Upstream is derived from gitlab.Gitlab, but implements a few additional convenience methods such as
     self.select_release(), self.download_release() and self.promote_release().
     """
 
     def __init__(self, url: str, private_token: Optional[str], name: str):
-        """Create an instance of Upstream
+        """Create an instance of Upstream.
 
         Parameters
         ----------
         url: str
             The URL of the gitlab instance to interact with
         private_token: Optional[str]
             An API token to use to interact with the gitlab instance
         name: str
             The name of the project to interact with
         """
-
         super().__init__(url=url, private_token=private_token)
         self.name = name
         if "/" in name:
             self.project_name = name.split("/")[-1]
 
     def select_release(self, max_releases: int = 3) -> Optional[str]:
-        """Select one release from a project, that is not yet promoted
+        """Select one release from a project, that is not yet promoted.
 
         Parameters
         ----------
         max_releases: int
             How many releases to show at maximum
 
         Returns
         -------
         str
             The tag_name of the selected release
         """
-
         release_tags = self.get_releases(max_releases=max_releases, promoted=False)
 
         if release_tags:
             selection_string = "".join([f"{index}) {value}\n" for index, value in enumerate(release_tags)])
             selection = input(f"Select a release for {self.name}:\n{selection_string}")
             return release_tags[int(selection)]
         else:
             print("There are no releases to promote!")
             return None
 
     def get_releases(self, max_releases: int, promoted: bool = False) -> List[str]:
-        """Get a list of releases of a project
+        """Get a list of releases of a project.
 
         Parameters
         ----------
         max_releases: int
             The maximum amount of releases to list
         promoted: bool
             Whether to only consider promoted releases (defaults to False)
 
         Returns
         -------
         List[str]
             A list of strings representing release tags of the project
         """
-
         project = self.projects.get(self.name)
 
         release_tags: List[str] = []
 
         for release in project.releases.list():
             if promoted:
                 # only select releases that are promoted
@@ -89,15 +88,15 @@
                     and len(release_tags) < max_releases
                 ):
                     release_tags += [release.tag_name]
 
         return release_tags
 
     def download_release(self, tag_name: str, temp_dir: Path, job_name: str) -> Path:
-        """Download the build artifacts of a project's release as a compressed file
+        """Download the build artifacts of a project's release as a compressed file.
 
         Parameters
         ----------
         tag_name: str
             The tag_name of the release to download
         temp_dir: Path
             The directory into which to download
@@ -105,15 +104,14 @@
             The name of the job that provides the release artifacts
 
         Returns
         -------
         Path
             The file path of the downloaded compressed file
         """
-
         project = self.projects.get(self.name)
         artifact_zip = temp_dir / Path(f"{self.project_name}-{tag_name}.zip")
         try:
             print(f"Downloading build artifacts of release '{tag_name}' for '{self.name}'...")
             with open(artifact_zip, "wb") as download:
                 project.artifacts(
                     ref_name=tag_name,
@@ -124,29 +122,28 @@
             print("Done!")
         except gitlab.exceptions.GitlabGetError:
             print(f"Skipping release {tag_name} as there are no artifacts to download")
 
         return artifact_zip
 
     def download_promotion_artifact(self, tag_name: str, temp_dir: Path) -> Path:
-        """Download the promotion artifact of a project's release
+        """Download the promotion artifact of a project's release.
 
         Parameters
         ----------
         tag_name: str
             The tag_name of the release to download
         temp_dir: Path
             The directory into which to download
 
         Returns
         -------
         Path
             The file path of the downloaded file
         """
-
         project = self.projects.get(self.name)
         artifact_links: List[str] = []
 
         for release in project.releases.list():
             # only select releases that are promoted
             if release.tag_name == tag_name and any(link.name == "Promotion artifact" for link in release.links.list()):
                 artifact_links += [link.url for link in release.links.list() if link.name == "Promotion artifact"]
@@ -158,30 +155,31 @@
         if len(artifact_links) > 1:
             raise RuntimeError(
                 f"There is more than one promotion artifact to download for the release '{tag_name}' "
                 f"of project '{project.name}'. Something is wrong!"
             )
 
         print(f"Downloading promotion artifact of release '{tag_name}' for '{self.name}'...")
-        filename, headers = request.urlretrieve(artifact_links[0], filename=temp_dir / Path("promotion.zip"))
+        filename, headers = request.urlretrieve(  # ignore: B310
+            artifact_links[0], filename=temp_dir / Path("promotion.zip")
+        )
         print("Done!")
 
         return Path(filename)
 
     def promote_release(self, tag_name: str, file: str) -> None:
-        """Upload a promotion file to the project and add it as a link to a release
+        """Upload a promotion file to the project and add it as a link to a release.
 
         Parameters
         ----------
         tag_name: str
             The tag_name of the project's release to attach a link to
         file: str
             The file path for a file to upload to the project
         """
-
         project = self.projects.get(self.name)
         print(f"Project '{self.name}': Uploading file {file}...")
         uploaded_file = project.upload(filename="promotion.zip", filepath=file)
         print(f"Project '{self.name}': Linking file {file} to release {tag_name}...")
         for release in project.releases.list():
             if release.tag_name == tag_name:
                 release.links.create(
```

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/release.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/release.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,64 @@
+"""Release handling."""
+
 from typing import List, Optional
 
 from pydantic import BaseModel
 
 
 class Metric(BaseModel):
-    """A pydantic model describing a metric
+    """A pydantic model describing a metric.
 
     Attributes
     ----------
     name: str
         A name for the metric
     description: str
         A description for the metric
     """
 
     name: str
     description: str
 
 
 class SizeMetric(Metric):
-    """A pydantic model describing a size metric
+    """A pydantic model describing a size metric.
 
     Attributes
     ----------
-    size: int
+    size: float
     """
 
-    size: int
+    size: float
 
 
 class AmountMetric(Metric):
-    """A pydantic model describing an amount metric
+    """A pydantic model describing an amount metric.
 
     Attributes
     ----------
     amount: int
     """
 
     amount: int
 
 
 class VersionMetric(Metric):
-    """A pydantic model describing a version metric
+    """A pydantic model describing a version metric.
 
     Attributes
     ----------
     version: str
     """
 
     version: str
 
 
 class Release(BaseModel):
-    """A pydantic model describing a release
+    """A pydantic model describing a release.
 
     Attributes
     ----------
     name: str
         The name of the artifact type
     version: str
         The version of the artifact
@@ -78,10 +80,10 @@
 
     name: str
     version: str
     files: List[str]
     amount_metrics: List[AmountMetric]
     size_metrics: List[SizeMetric]
     version_metrics: List[VersionMetric]
-    torrent_file: Optional[str]
+    torrent_file: Optional[str] = None
     developer: str
     pgp_public_key: str
```

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/signature.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/signature.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
+"""Signature handling."""
+
 from pathlib import Path
 from subprocess import run
 from typing import List
 
 
 def sign_files_in_dir(path: Path, developer: str, gpgkey: str, file_extensions: List[str] = []) -> None:
-    """Create a detached PGP signature for one or more files in a release
+    """Create a detached PGP signature for one or more files in a release.
 
     Parameters
     ----------
     path: Path
         The path to the release
     developer: str
         The developer mbox (i.e. "First Last <user@domain.tld>")
     gpgkey: str
         The PGP key to sign with
     """
-
     for _file in path.iterdir():
         if _file.suffix in file_extensions:
             print(f"Creating signature for {_file}...")
             return_code = 255
             while return_code != 0:
                 return_code = sign_file(path=_file.resolve(), developer=developer, gpgkey=gpgkey)
             print("Done!")
 
 
 def sign_file(path: Path, developer: str, gpgkey: str) -> int:
-    """Sign a file and return the status code of gpg
+    """Sign a file and return the status code of gpg.
 
     Parameters
     ----------
     path: Path
         The path to a file to sign
     developer: str
         The developer mbox (i.e. "First Last <user@domain.tld>")
@@ -38,15 +39,14 @@
         The PGP key to sign with
 
     Returns
     -------
     int
         The returncode of the gpg process
     """
-
     return run(
         [
             "gpg",
             "--batch",
             "--no-armor",
             "--no-include-key-block",
             "--sender",
```

### Comparing `arch-release-promotion-0.2.2/arch_release_promotion/torrent.py` & `arch_release_promotion-0.3.0.post0/arch_release_promotion/torrent.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""Torrent handling."""
+
 from pathlib import Path
 from typing import List
 from urllib.request import urlopen
 
 from torrentool.api import Torrent
 
 
 def create_torrent_file(path: Path, webseeds: List[str], output: Path) -> str:
-    """Create a torrent file for a path and write it to an output directory
+    """Create a torrent file for a path and write it to an output directory.
 
     Parameters
     ----------
     path: Path
         The path for which to create a torrent file
     webseeds: List[str]
         The list of webseeds to add to the torrent file
@@ -18,29 +20,27 @@
         A path to write the .torrent file to
 
     Returns
     -------
     str
         A string representing the name of the torrent file
     """
-
     torrent = Torrent.create_from(path)
     torrent.webseeds = webseeds
     torrent.to_file(output)
 
     return output.name
 
 
 def get_webseeds(
     artifact_type: str,
     mirrorlist_url: str,
     version: str,
 ) -> List[str]:
-    """Read available mirrors from a remote URL and return them in a formatted list representing the webseeds for a
-    given artifact type
+    """Assemble webseeds for an artifact type by querying a mirrorlist URL.
 
     Parameters
     ----------
     artifact_type: str
         The artifact type to create the webseeds for
     mirrorlist_url: str
         A URL used to retrieve the list of mirrors
@@ -48,20 +48,22 @@
         The version of the artifact type to create the webseeds for
 
     Returns
     -------
     List[str]
         A list of strings representing webseeds for an artifact type in a specific version
     """
-
     webseeds: List[str] = []
     url = urlopen(mirrorlist_url)
     for line in url.read().decode("utf-8").split("\n"):
         if "#Server = " in line:
             webseeds += [
-                line.replace("#Server = ", "",).replace(
+                line.replace(
+                    "#Server = ",
+                    "",
+                ).replace(
                     "$repo/os/$arch",
                     f"releases/{artifact_type}/{version}/",
                 )
             ]
 
     return webseeds
```

### Comparing `arch-release-promotion-0.2.2/examples/example.toml` & `arch_release_promotion-0.3.0.post0/examples/example.toml`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/examples/projects.toml` & `arch_release_promotion-0.3.0.post0/examples/projects.toml`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/examples/systemd/arch-release-sync.service` & `arch_release_promotion-0.3.0.post0/examples/systemd/arch-release-sync.service`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/tests/test_argparse.py` & `arch_release_promotion-0.3.0.post0/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/tests/test_config.py` & `arch_release_promotion-0.3.0.post0/tests/test_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     conf.write(f"PACKAGER='{packager}'\n")
     if private_token:
         conf.write(f"PRIVATE_TOKEN={private_token}\n")
     conf.close()
 
     with patch("arch_release_promotion.config.MAKEPKG_CONFIGS", [Path(conf.name)]):
         with expectation:
-            assert config.Settings()
+            assert config.Settings()  # type: ignore[call-arg]
     Path(conf.name).unlink()
 
 
 @mark.parametrize(
     "create_config, config_rows, name, expectation",
     [
         (
@@ -150,31 +150,32 @@
             [
                 "[[projects]]",
                 'name = "foo/bar"',
                 'job_name = "build"',
                 'metrics_file = "metrics.txt"',
                 'output_dir = "output"',
                 "releases = [",
-                '{name = "test",extensions_to_sign = [".baz"]}',
-                '{name = "test",extensions_to_sign = [".bar"]}]',
+                '  {name = "test", extensions_to_sign = [".baz"]},',
+                '  {name = "test", extensions_to_sign = [".bar"]},',
+                "]",
             ],
             "foo/bar",
             raises(ValidationError),
         ),
         (
             False,
             [],
             "",
             raises(RuntimeError),
         ),
         (
             True,
             [],
             "",
-            raises(ValidationError),
+            raises(RuntimeError),
         ),
     ],
 )
 def test_projects(
     create_config: bool,
     config_rows: List[str],
     name: str,
@@ -184,16 +185,16 @@
         conf = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", suffix=".conf", delete=False)
         for row in config_rows:
             conf.write(f"{row}\n")
         conf.close()
 
         with patch("arch_release_promotion.config.PROJECTS_CONFIGS", [Path(conf.name)]):
             with expectation:
-                projects = config.Projects()
+                projects = config.Projects()  # type: ignore[call-arg]
                 assert projects
                 assert isinstance(projects.get_project(name=name), config.ProjectConfig)
 
         Path(conf.name).unlink()
     else:
         with patch("arch_release_promotion.config.PROJECTS_CONFIGS", [Path("foo.bar")]):
             with expectation:
-                assert config.Projects()
+                assert config.Projects()  # type: ignore[call-arg]
```

### Comparing `arch-release-promotion-0.2.2/tests/test_files.py` & `arch_release_promotion-0.3.0.post0/tests/test_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
 
 @fixture
 def project_config() -> Iterator[config.ProjectConfig]:
     yield config.ProjectConfig(
         name="foo",
         job_name="bar",
-        output_dir="out",
-        metrics_file="metrics.txt",
+        output_dir=Path("out"),
+        metrics_file=Path("metrics.txt"),
         releases=[],
         sync_config=config.SyncConfig(),
     )
 
 
 @fixture
 def project_files(project_config: config.ProjectConfig) -> Iterator[files.ProjectFiles]:
@@ -419,22 +419,20 @@
     version_dir = Path(f"{name}-{version}")
     (release_type_dir / version_dir).mkdir()
 
     if has_promoted_releases:
         project_files.promoted_releases = ["0.1.0"]
         project_files.project_config.releases = [
             config.ReleaseConfig(
-                **{
-                    "amount_metrics": [],
-                    "create_torrent": False,
-                    "extensions_to_sign": [],
-                    "name": name,
-                    "size_metrics": [],
-                    "version_metrics": [],
-                }
+                amount_metrics=[],
+                create_torrent=False,
+                extensions_to_sign=[],
+                name=name,
+                size_metrics=[],
+                version_metrics=[],
             )
         ]
     else:
         project_files.promoted_releases = []
 
     if create_files:
         other_version_dir = release_type_dir / Path(f"{name}-{other_version}")
@@ -475,22 +473,20 @@
     version_dir = Path(f"{name}-{version}")
     (release_type_dir / version_dir).mkdir()
 
     if has_promoted_releases:
         project_files.promoted_releases = ["0.1.0"]
         project_files.project_config.releases = [
             config.ReleaseConfig(
-                **{
-                    "amount_metrics": [],
-                    "create_torrent": False,
-                    "extensions_to_sign": [],
-                    "name": name,
-                    "size_metrics": [],
-                    "version_metrics": [],
-                }
+                amount_metrics=[],
+                create_torrent=False,
+                extensions_to_sign=[],
+                name=name,
+                size_metrics=[],
+                version_metrics=[],
             )
         ]
     else:
         project_files.promoted_releases = []
 
     if link_target == "same_version":
         latest_path.symlink_to(version_dir)
@@ -601,25 +597,23 @@
     if create_json:
         (
             project_files.project_config.sync_config.directory / Path(f"{name}/{name}-{version}.json")  # type: ignore
         ).touch()
 
     load_release_from_json_payload_mock.return_value = (
         files.Release(
-            **{
-                "name": name,
-                "version": version,
-                "files": [file],
-                "amount_metrics": [],
-                "size_metrics": [],
-                "version_metrics": [],
-                "torrent_file": f"{name}-{version}.torrent" if has_torrent else None,
-                "developer": "Foobar McFooface <foobar@mcfooface.com>",
-                "pgp_public_key": "SOMEONESKEY",
-            }
+            name=name,
+            version=version,
+            files=[file],
+            amount_metrics=[],
+            size_metrics=[],
+            version_metrics=[],
+            torrent_file=f"{name}-{version}.torrent" if has_torrent else None,
+            developer="Foobar McFooface <foobar@mcfooface.com>",
+            pgp_public_key="SOMEONESKEY",
         )
         if create_json
         else None
     )
 
     if create_torrent_file:
         (
@@ -656,22 +650,20 @@
     project_files: files.ProjectFiles,
 ) -> None:
     name = "foo"
     version = "0.1.0"
     if has_release_type:
         project_files.project_config.releases = [
             config.ReleaseConfig(
-                **{
-                    "amount_metrics": [],
-                    "create_torrent": False,
-                    "extensions_to_sign": [],
-                    "name": name,
-                    "size_metrics": [],
-                    "version_metrics": [],
-                }
+                amount_metrics=[],
+                create_torrent=False,
+                extensions_to_sign=[],
+                name=name,
+                size_metrics=[],
+                version_metrics=[],
             )
         ]
 
     _is_release_type_synced_mock.return_value = release_type_synced
 
     assert project_files._project_version_requires_sync(version=version) is return_value
```

### Comparing `arch-release-promotion-0.2.2/tests/test_gitlab.py` & `arch_release_promotion-0.3.0.post0/tests/test_gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,18 @@
     project = Mock()
     project.releases = releases
 
     projects = Mock()
     projects.get.return_value = project
     upstream.projects = projects
     assert upstream.select_release() == output
+    if output is not None:
+        input_mock.assert_called_once()
+    else:
+        input_mock.assert_not_called()
 
 
 @mark.parametrize(
     "releases_available, tag_name, link_name, max_releases, promoted, output",
     [
         (True, "0.1.0", "Build artifacts", 1, False, ["0.1.0"]),
         (False, "0.1.0", "Build artifacts", 1, False, []),
@@ -127,45 +131,42 @@
     projects = Mock()
     projects.get.return_value = project
     upstream.projects = projects
     upstream.download_release(tag_name="0.1.0", temp_dir=Path("/tmp"), job_name="job")
 
 
 @mark.parametrize(
-    "releases_available, tag_name, multi_promotion, has_link, link_name, link_url, expectation",
+    "releases_available, tag_name, multi_promotion, link_name, link_url, expectation",
     [
-        (True, "0.1.0", False, True, "Promotion artifact", "https://foo.bar/download/this/file.zip", does_not_raise()),
-        (True, "0.1.0", False, True, "Foo artifact", "https://foo.bar/download/this/file.zip", raises(RuntimeError)),
+        (True, "0.1.0", False, "Promotion artifact", "https://foo.bar/download/this/file.zip", does_not_raise()),
+        (True, "0.1.0", False, "Foo artifact", "https://foo.bar/download/this/file.zip", raises(RuntimeError)),
         (
             False,
             "0.1.0",
             False,
-            True,
             "Promotion artifact",
             "https://foo.bar/download/this/file.zip",
             raises(RuntimeError),
         ),
         (
             True,
             "0.1.0",
             True,
-            True,
             "Promotion artifact",
             "https://foo.bar/download/this/file.zip",
             raises(RuntimeError),
         ),
     ],
 )
 @patch("arch_release_promotion.gitlab.request.urlretrieve")
 def test_gitlab_download_promotion_artifact(
     urlretrieve_mock: Mock,
     releases_available: bool,
     tag_name: str,
     multi_promotion: bool,
-    has_link: bool,
     link_name: str,
     link_url: str,
     expectation: ContextManager[str],
 ) -> None:
     urlretrieve_mock.return_value = ("foo", None)
     upstream = gitlab.Upstream(
         url="https://foo.bar-mc.foo",
```

### Comparing `arch-release-promotion-0.2.2/tests/test_release.py` & `arch_release_promotion-0.3.0.post0/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/tests/test_signature.py` & `arch_release_promotion-0.3.0.post0/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `arch-release-promotion-0.2.2/tests/test_torrent.py` & `arch_release_promotion-0.3.0.post0/tests/test_torrent.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from arch_release_promotion import torrent
 
 
 @patch("arch_release_promotion.torrent.Torrent.create_from")
 def test_creat_torrent_file(create_from_mock: Mock) -> None:
     torrent.create_torrent_file(path=Path("foo"), webseeds=["foo"], output=Path("bar"))
+    create_from_mock.assert_called_once()
 
 
 @patch("arch_release_promotion.torrent.urlopen")
 def test_get_webseeds(urlopen_mock: Mock) -> None:
     artifact_type = "foo"
     mirrorlist_url = "https://foo.bar/mirrorlist"
     version = "0.1.0"
```

### Comparing `arch-release-promotion-0.2.2/setup.py` & `arch_release_promotion-0.3.0.post0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,344 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: arch-release-promotion
+Version: 0.3.0.post0
+Summary: Promote official Arch Linux releases and synchronize them
+Keywords: arch linux releases pgp signature synchronization torrent
+Home-page: https://gitlab.archlinux.org/archlinux/arch-release-promotion
+Author-Email: David Runge <dvzrv@archlinux.org>
+License: GPL-3.0-or-later
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Security :: Cryptography
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Operating System
+Classifier: Topic :: Utilities
+Project-URL: Bug tracker, https://gitlab.archlinux.org/archlinux/arch-release-promotion/-/issues/
+Project-URL: Homepage, https://gitlab.archlinux.org/archlinux/arch-release-promotion
+Project-URL: Repository, https://gitlab.archlinux.org/archlinux/arch-release-promotion
+Project-URL: Documentation, https://gitlab.archlinux.org/archlinux/arch-release-promotion/-/blob/master/README.rst
+Requires-Python: <4.0,>=3.10
+Requires-Dist: pydantic<3.0.0,>=2.0.0
+Requires-Dist: python-dotenv<2.0.0,>=1.0.0
+Requires-Dist: pyxdg<1.0,>=0.27
+Requires-Dist: email-validator<3.0.0,>=2.0.0
+Requires-Dist: torrentool<2.0.0,>=1.1.1
+Requires-Dist: python-gitlab<4.0.0,>=3.0.0
+Requires-Dist: orjson<4.0.0,>=3.6.1
+Requires-Dist: prometheus-client<1.0.0,>=0.14.1
+Requires-Dist: tomli>=2.0.1; python_version < "3.11"
+Requires-Dist: pydantic-settings>=2.0.2
+Description-Content-Type: text/x-rst
 
-packages = \
-['arch_release_promotion']
+======================
+arch-release-promotion
+======================
 
-package_data = \
-{'': ['*']}
+This project allows for promotion and synchronization of existing releases of a
+project in Arch Linux's Gitlab instance.
 
-install_requires = \
-['email-validator>=1.1.3,<2.0.0',
- 'orjson>=3.6.1,<4.0.0',
- 'prometheus-client>=0.14.1,<0.15.0',
- 'pydantic>=1.8.2,<2.0.0',
- 'python-dotenv>=0.20.0,<0.21.0',
- 'python-gitlab>=3.0.0,<4.0.0',
- 'pyxdg>=0.27,<0.28',
- 'toml>=0.10.2,<0.11.0',
- 'torrentool>=1.1.1,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['arch-release-promotion = arch_release_promotion.cli:main',
-                     'arch-release-sync = '
-                     'arch_release_promotion.cli:arch_release_sync']}
-
-setup_kwargs = {
-    'name': 'arch-release-promotion',
-    'version': '0.2.2',
-    'description': 'Promote official Arch Linux releases and synchronize them',
-    'long_description': '======================\narch-release-promotion\n======================\n\nThis project allows for promotion and synchronization of existing releases of a\nproject in Arch Linux\'s Gitlab instance.\n\nReleases of a project (e.g. ``project``) may consist of several release types\n(e.g. ``image_a`` and ``image_b``), which are addressed separately.\n\nA promotion encompasses - per release type - PGP signatures for relevant\nartifacts (optional), a torrent file (optional) and a JSON payload which can be\nused by `archweb <https://github.com/archlinux/archweb>`_ to display\ninformation about each release type.\n\nSynchronization with a local directory can be achieved for a configurable\nmaximum amount of release versions (each consisting of their respective\nconfigured release types) of a project.\n\nRequirements\n============\n\nArch-release-promotion is Python based. All language specific requirements are\nspecified in its `pyproject.toml <pyproject.toml>`_.\n\nAdditionally, ``arch-release-promotion`` requires `gnupg <https://gnupg.org/>`_\nto handle detached PGP signatures.\n\nUse\n===\n\nAfter installation, refer to the output of ``arch-release-promotion -h`` and\n``arch-release-sync -h``.\n\nConfiguration\n=============\n\nThe command-line tools ``arch-release-promotion`` and ``arch-release-sync``\nmake use of two sources of configuration:\n\n* `makepkg.conf <https://man.archlinux.org/man/makepkg.conf.5>`_ is read from\n  any of its locations in the same priority as `makepkg\n  <https://man.archlinux.org/man/makepkg.8>`_ does.\n  All of the below can also be passed to the tool via environment variables:\n\n  * ``GPGKEY`` is recognized for establishing which PGP key to use for signing\n  * ``PACKAGER`` is recognized for establishing who is doing the signature and\n    is important for `WKD\n    <https://wiki.archlinux.org/title/GnuPG#Web_Key_Directory>`_ lookup\n  * ``MIRRORLIST_URL`` (not used by makepkg) is used during the generation of\n    torrent files to add webseeds (defaults to\n    ``"https://archlinux.org/mirrorlist/?country=all&protocol=http&protocol=https"``)\n  * ``GITLAB_URL`` (not used by makepkg) is used to connect to a GitLab\n    instance to select, download and promote releases of a project (defaults to\n    ``"https://gitlab.archlinux.org"``)\n  * ``PRIVATE_TOKEN`` (not used by makepkg) is used to authenticate against the\n    GitLab instance. The `personal access token\n    <https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html>`_\n    needs to provide write access for the target project.\n\n* ``projects.toml`` is a configuration file that provides the configuration for a\n  project and its releases. Configuration files are read and merged with\n  descending priority from ``/etc/arch-release-promotion/projects.toml`` and\n  ``$XDG_CONFIG_HOME/arch-release-promotion/projects.toml`` (which defaults to\n  ``$HOME/.config/arch-release-promotion/projects.toml`` if\n  ``$XDG_CONFIG_HOME`` is unset).\n  Please refer to `examples/example.toml <examples/example.toml>`_ for further\n  reference in regards to the available options\n\nOpenmetrics\n-----------\n\nIf the upstream project offers an `openmetrics <https://openmetrics.io/>`_\nbased metrics file, the data from it can be used as additional information in\nthe JSON payload.\n\nThe following metrics are considered.\n\nVersion metrics\n^^^^^^^^^^^^^^^\n\nDescription and version information about e.g. packages can be derived from\n``version_info`` metrics of type ``info``, that define a ``name``,\n``description`` and ``version`` label.\n\nFor the metrics to be considered, they have to be configured by adding a\n``version_metrics`` list (a list of names to look for) to a release of a\nproject.\n\n.. code::\n\n   # TYPE version_info info\n   # HELP version_info Package description and version information\n   version_info{name="my-package",description="Version of my-package used for build",version="1.0.0-1"} 1\n\nThe above metrics entry would result in the following JSON representation:\n\n.. code:: json\n\n   "version_metrics": [\n     {\n       "name": "my-package",\n       "description": "Version of my-package used for build",\n       "version": "1.0.0-1"\n     }\n   ]\n\nSize metrics\n^^^^^^^^^^^^\n\nArtifact size information in MebiBytes (MiB) and description can be derived\nfrom ``artifact_bytes`` metrics of type ``gauge``, that define a ``name`` and a\n``description`` label.\n\nFor the metrics to be considered, they have to be configured by adding a\n``size_metrics`` list (a list of names to look for) to a release of a\nproject.\n\n.. code::\n\n   # TYPE artifact_bytes gauge\n   # HELP artifact_bytes Artifact sizes in Bytes\n   artifact_bytes{name="foo",description="Size of foo in MiB"} 832\n\nThe above metrics entry would result in the following JSON representation:\n\n.. code:: json\n\n   "size_metrics": [\n     {\n       "name": "foo",\n       "description": "Size of foo in MiB",\n       "size": 832\n     }\n   ]\n\nAmount metrics\n^^^^^^^^^^^^^^\n\nInformation on the amount of something (e.g. packages) and description can be\nderived from ``data_count`` metrics of type ``summary``, that define a ``name``\nand a ``description`` label.\n\nFor the metrics to be considered, they have to be configured by adding a\n``amount_metrics`` list (a list of names to look for) to a release of a\nproject.\n\n.. code::\n\n   # TYPE data_count summary\n   # HELP data_count The amount of something used in some context\n   data_count{name="foo",description="The amount of packages in foo"} 369\n\nThe above metrics entry would result in the following JSON representation:\n\n.. code:: json\n\n   "amount_metrics": [\n     {\n       "name": "foo",\n       "description": "The amount of packages in foo",\n       "amount": 369\n     }\n   ]\n\nPromotion artifact\n==================\n\nThe promotion artifact is a ZIP compressed file (``promotion.zip``), that is\nuploaded to the project before its link is added to the release that it is\npromoting.\n\nThe file contains one directory for each release type that the project offers.\nIn each release type directory there are is a **JSON payload**\n(``<release_type>-<version>.json``), a directory\n(``<release_type>-<version>/``) containing signatures for any files that have\nbeen setup for detached signatures and optionally a torrent file\n(``<release_type>-<version>.json``) that is created for the release type\'s\nbuild artifacts *and* the detached signatures contained in the promotion\nartifact.\n\n.. code::\n\n   example\n   ├── example-0.1.0\n   │\xa0\xa0 └── artifact.tar.gz.sig\n   ├── example-0.1.0.json\n   └── example-0.1.0.torrent\n\nJSON payload\n------------\n\nThe promotion of a release encompasses one or more JSON payloads, that describe\neach release type in the release.\n\n.. code:: json\n\n   {\n     "amount_metrics": [\n       {\n         "name": "foo",\n         "description": "The amount of packages in foo",\n         "size": 369\n       }\n     ],\n     "developer": "Foobar McFooface <foobar@mcfooface.com>",\n     "files": ["something.txt", "something.txt.sig"],\n     "name": "foo",\n     "pgp_public_key": "SOMEONESPGPKEYID",\n     "size_metrics": [\n       {\n         "name": "foo",\n         "description": "Size of foo in MiB",\n         "size": 832\n       }\n     ],\n     "torrent_file": "foo-0.1.0.torrent",\n     "version_metrics": [\n       {\n         "name": "my-package",\n         "description": "Version of my-package used for build",\n         "version": "1.0.0-1"\n       }\n     ],\n     "version": "0.1.0"\n   }\n\n* ``amount_metrics``: A list of objects that describe the amount of something\n  (optional). The list depends on whether the project\'s configuration defines\n  ``amount_metrics`` and whether those metrics are available in the specific\n  release.\n* ``developer``: The full uid of the person promoting (and optionally signing\n  artifacts in) the release type.\n* ``files``: A list of files in the release type.\n* ``name``: The name of the release type.\n* ``pgp_public_key``: The PGP key ID of the key signing files in the release\n  type.\n* ``size_metrics``: A list of objects that describe the size of something\n  (optional). The list depends on whether the project\'s configuration defines\n  ``size_metrics`` and whether those metrics are available in the specific\n  release.\n* ``torrent_file`` (optional): The name of a torrent file created for the\n  release type. The value depends on whether the configuration for the release\n  type sets ``create_torrent`` to ``True``.\n* ``version_metrics``: A list of objects that describe the version of something\n  (optional). The list depends on whether the project\'s configuration defines\n  ``version_metrics`` and whether those metrics are available in the specific\n  release.\n* ``version``: The version of the release type.\n\nSynchronization\n===============\n\nThe synchronization of releases works by retrieving the list of promoted\nreleases of the project from the remote. For each promoted release version, the\npromotion artifact is downloaded and used to establish whether all of the\nconfigured release types are fully synchronized.\n\nLocation and cleanup\n--------------------\n\nAll release types for each release version are synchronized to a local\ndirectory. The directory and and the maximum amount of synchronized release\nversions are configurable globally or per project.\n\n.. code::\n\n   sync_dir\n   ├── example_a\n   │\xa0\xa0 ├── example_a-0.1.0\n   │\xa0\xa0 │\xa0\xa0 ├── foo.txt\n   │\xa0\xa0 │\xa0\xa0 └── foo.txt.sig\n   │\xa0\xa0 ├── example_a-0.1.0.json\n   │\xa0\xa0 ├── example_a-0.1.0.torrent\n   │\xa0\xa0 └── latest -> example_a-0.1.0\n   └── example_b\n       ├── example_b-0.1.0\n       │\xa0\xa0 ├── bar.txt\n       │\xa0\xa0 └── bar.txt.sig\n       ├── example_b-0.1.0.json\n       ├── example_b-0.1.0.torrent\n       └── latest -> example_b-0.1.0\n\nA ``latest`` symlink is created to point at the currently latest version of\neach release type.\n\nAny files and directories that are not owned by versions of release types of\nthe currently synchronized release versions are removed from the\nsynchronization directory.\n\nIf changes are introduced to files in the target directory (due to a\nsynchronization action), it is possible to write a Unix timestamp to a file\nthat is configurable globally or per project (the directory in which the file\nresides in has to exist).\n\nSystem integration\n------------------\n\nFor systemd based systems there are example systemd system service and timer\nfiles that are provided in `examples/systemd/ <examples/systemd/>`_.\nThe provided service file relies on the user ``arch-release-sync`` which may be\ncreated using the `sysusers.d\n<https://man.archlinux.org/man/core/systemd/sysusers.d.5.en>`_ integration\nprovided in `examples/sysusers.d/ <examples/sysusers.d/>`_.\n\nLicense\n=======\n\nArch-release-promotion is licensed under the terms of the **GPL-3.0-or-later**\n(see `LICENSE <LICENSE>`_).\n\n',
-    'author': 'David Runge',
-    'author_email': 'dvzrv@archlinux.org',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://gitlab.archlinux.org/archlinux/arch-release-promotion',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+Releases of a project (e.g. ``project``) may consist of several release types
+(e.g. ``image_a`` and ``image_b``), which are addressed separately.
 
+A promotion encompasses - per release type - PGP signatures for relevant
+artifacts (optional), a torrent file (optional) and a JSON payload which can be
+used by `archweb <https://github.com/archlinux/archweb>`_ to display
+information about each release type.
+
+Synchronization with a local directory can be achieved for a configurable
+maximum amount of release versions (each consisting of their respective
+configured release types) of a project.
+
+Requirements
+============
+
+Arch-release-promotion is Python based. All language specific requirements are
+specified in its `pyproject.toml <pyproject.toml>`_.
+
+Additionally, ``arch-release-promotion`` requires `gnupg <https://gnupg.org/>`_
+to handle detached PGP signatures.
+
+Use
+===
+
+After installation, refer to the output of ``arch-release-promotion -h`` and
+``arch-release-sync -h``.
+
+Configuration
+=============
+
+The command-line tools ``arch-release-promotion`` and ``arch-release-sync``
+make use of two sources of configuration:
+
+* `makepkg.conf <https://man.archlinux.org/man/makepkg.conf.5>`_ is read from
+  any of its locations in the same priority as `makepkg
+  <https://man.archlinux.org/man/makepkg.8>`_ does.
+  All of the below can also be passed to the tool via environment variables:
+
+  * ``GPGKEY`` is recognized for establishing which PGP key to use for signing
+  * ``PACKAGER`` is recognized for establishing who is doing the signature and
+    is important for `WKD
+    <https://wiki.archlinux.org/title/GnuPG#Web_Key_Directory>`_ lookup
+  * ``MIRRORLIST_URL`` (not used by makepkg) is used during the generation of
+    torrent files to add webseeds (defaults to
+    ``"https://archlinux.org/mirrorlist/?country=all&protocol=http&protocol=https"``)
+  * ``GITLAB_URL`` (not used by makepkg) is used to connect to a GitLab
+    instance to select, download and promote releases of a project (defaults to
+    ``"https://gitlab.archlinux.org"``)
+  * ``PRIVATE_TOKEN`` (not used by makepkg) is used to authenticate against the
+    GitLab instance. The `personal access token
+    <https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html>`_
+    needs to provide write access for the target project.
+
+* ``projects.toml`` is a configuration file that provides the configuration for a
+  project and its releases. Configuration files are read and merged with
+  descending priority from ``/etc/arch-release-promotion/projects.toml`` and
+  ``$XDG_CONFIG_HOME/arch-release-promotion/projects.toml`` (which defaults to
+  ``$HOME/.config/arch-release-promotion/projects.toml`` if
+  ``$XDG_CONFIG_HOME`` is unset).
+  Please refer to `examples/example.toml <examples/example.toml>`_ for further
+  reference in regards to the available options
+
+Openmetrics
+-----------
+
+If the upstream project offers an `openmetrics <https://openmetrics.io/>`_
+based metrics file, the data from it can be used as additional information in
+the JSON payload.
+
+The following metrics are considered.
+
+Version metrics
+^^^^^^^^^^^^^^^
+
+Description and version information about e.g. packages can be derived from
+``version_info`` metrics of type ``info``, that define a ``name``,
+``description`` and ``version`` label.
+
+For the metrics to be considered, they have to be configured by adding a
+``version_metrics`` list (a list of names to look for) to a release of a
+project.
+
+.. code::
+
+   # TYPE version_info info
+   # HELP version_info Package description and version information
+   version_info{name="my-package",description="Version of my-package used for build",version="1.0.0-1"} 1
+
+The above metrics entry would result in the following JSON representation:
+
+.. code:: json
+
+   "version_metrics": [
+     {
+       "name": "my-package",
+       "description": "Version of my-package used for build",
+       "version": "1.0.0-1"
+     }
+   ]
+
+Size metrics
+^^^^^^^^^^^^
+
+Artifact size information in MebiBytes (MiB) and description can be derived
+from ``artifact_bytes`` metrics of type ``gauge``, that define a ``name`` and a
+``description`` label.
+
+For the metrics to be considered, they have to be configured by adding a
+``size_metrics`` list (a list of names to look for) to a release of a
+project.
+
+.. code::
+
+   # TYPE artifact_bytes gauge
+   # HELP artifact_bytes Artifact sizes in Bytes
+   artifact_bytes{name="foo",description="Size of foo in MiB"} 832
+
+The above metrics entry would result in the following JSON representation:
+
+.. code:: json
+
+   "size_metrics": [
+     {
+       "name": "foo",
+       "description": "Size of foo in MiB",
+       "size": 832
+     }
+   ]
+
+Amount metrics
+^^^^^^^^^^^^^^
+
+Information on the amount of something (e.g. packages) and description can be
+derived from ``data_count`` metrics of type ``summary``, that define a ``name``
+and a ``description`` label.
+
+For the metrics to be considered, they have to be configured by adding a
+``amount_metrics`` list (a list of names to look for) to a release of a
+project.
+
+.. code::
+
+   # TYPE data_count summary
+   # HELP data_count The amount of something used in some context
+   data_count{name="foo",description="The amount of packages in foo"} 369
+
+The above metrics entry would result in the following JSON representation:
+
+.. code:: json
+
+   "amount_metrics": [
+     {
+       "name": "foo",
+       "description": "The amount of packages in foo",
+       "amount": 369
+     }
+   ]
+
+Promotion artifact
+==================
+
+The promotion artifact is a ZIP compressed file (``promotion.zip``), that is
+uploaded to the project before its link is added to the release that it is
+promoting.
+
+The file contains one directory for each release type that the project offers.
+In each release type directory there are is a **JSON payload**
+(``<release_type>-<version>.json``), a directory
+(``<release_type>-<version>/``) containing signatures for any files that have
+been setup for detached signatures and optionally a torrent file
+(``<release_type>-<version>.json``) that is created for the release type's
+build artifacts *and* the detached signatures contained in the promotion
+artifact.
+
+.. code::
+
+   example
+   ├── example-0.1.0
+   │   └── artifact.tar.gz.sig
+   ├── example-0.1.0.json
+   └── example-0.1.0.torrent
+
+JSON payload
+------------
+
+The promotion of a release encompasses one or more JSON payloads, that describe
+each release type in the release.
+
+.. code:: json
+
+   {
+     "amount_metrics": [
+       {
+         "name": "foo",
+         "description": "The amount of packages in foo",
+         "size": 369
+       }
+     ],
+     "developer": "Foobar McFooface <foobar@mcfooface.com>",
+     "files": ["something.txt", "something.txt.sig"],
+     "name": "foo",
+     "pgp_public_key": "SOMEONESPGPKEYID",
+     "size_metrics": [
+       {
+         "name": "foo",
+         "description": "Size of foo in MiB",
+         "size": 832
+       }
+     ],
+     "torrent_file": "foo-0.1.0.torrent",
+     "version_metrics": [
+       {
+         "name": "my-package",
+         "description": "Version of my-package used for build",
+         "version": "1.0.0-1"
+       }
+     ],
+     "version": "0.1.0"
+   }
+
+* ``amount_metrics``: A list of objects that describe the amount of something
+  (optional). The list depends on whether the project's configuration defines
+  ``amount_metrics`` and whether those metrics are available in the specific
+  release.
+* ``developer``: The full uid of the person promoting (and optionally signing
+  artifacts in) the release type.
+* ``files``: A list of files in the release type.
+* ``name``: The name of the release type.
+* ``pgp_public_key``: The PGP key ID of the key signing files in the release
+  type.
+* ``size_metrics``: A list of objects that describe the size of something
+  (optional). The list depends on whether the project's configuration defines
+  ``size_metrics`` and whether those metrics are available in the specific
+  release.
+* ``torrent_file`` (optional): The name of a torrent file created for the
+  release type. The value depends on whether the configuration for the release
+  type sets ``create_torrent`` to ``True``.
+* ``version_metrics``: A list of objects that describe the version of something
+  (optional). The list depends on whether the project's configuration defines
+  ``version_metrics`` and whether those metrics are available in the specific
+  release.
+* ``version``: The version of the release type.
+
+Synchronization
+===============
+
+The synchronization of releases works by retrieving the list of promoted
+releases of the project from the remote. For each promoted release version, the
+promotion artifact is downloaded and used to establish whether all of the
+configured release types are fully synchronized.
+
+Location and cleanup
+--------------------
+
+All release types for each release version are synchronized to a local
+directory. The directory and and the maximum amount of synchronized release
+versions are configurable globally or per project.
+
+.. code::
+
+   sync_dir
+   ├── example_a
+   │   ├── example_a-0.1.0
+   │   │   ├── foo.txt
+   │   │   └── foo.txt.sig
+   │   ├── example_a-0.1.0.json
+   │   ├── example_a-0.1.0.torrent
+   │   └── latest -> example_a-0.1.0
+   └── example_b
+       ├── example_b-0.1.0
+       │   ├── bar.txt
+       │   └── bar.txt.sig
+       ├── example_b-0.1.0.json
+       ├── example_b-0.1.0.torrent
+       └── latest -> example_b-0.1.0
+
+A ``latest`` symlink is created to point at the currently latest version of
+each release type.
+
+Any files and directories that are not owned by versions of release types of
+the currently synchronized release versions are removed from the
+synchronization directory.
+
+If changes are introduced to files in the target directory (due to a
+synchronization action), it is possible to write a Unix timestamp to a file
+that is configurable globally or per project (the directory in which the file
+resides in has to exist).
+
+System integration
+------------------
+
+For systemd based systems there are example systemd system service and timer
+files that are provided in `examples/systemd/ <examples/systemd/>`_.
+The provided service file relies on the user ``arch-release-sync`` which may be
+created using the `sysusers.d
+<https://man.archlinux.org/man/core/systemd/sysusers.d.5.en>`_ integration
+provided in `examples/sysusers.d/ <examples/sysusers.d/>`_.
+
+License
+=======
+
+Arch-release-promotion is licensed under the terms of the **GPL-3.0-or-later**
+(see `LICENSE <LICENSE>`_).
 
-setup(**setup_kwargs)
```

