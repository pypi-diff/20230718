# Comparing `tmp/dt-cli-1.6.7.tar.gz` & `tmp/dt-cli-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-cli-1.6.7.tar", max compression
+gzip compressed data, was "dt-cli-1.6.9.tar", max compression
```

## Comparing `dt-cli-1.6.7.tar` & `dt-cli-1.6.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11342 2022-08-02 14:56:21.000000 dt-cli-1.6.7/LICENSE
--rw-r--r--   0        0        0     3232 2022-08-02 14:56:21.000000 dt-cli-1.6.7/README.md
--rw-r--r--   0        0        0      638 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/__init__.py
--rw-r--r--   0        0        0       95 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/__main__.py
--rw-r--r--   0        0        0     5579 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/api.py
--rw-r--r--   0        0        0     5130 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/building.py
--rw-r--r--   0        0        0     2396 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/click_helpers.py
--rw-r--r--   0        0        0     1726 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/constants.py
--rw-r--r--   0        0        0     5246 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/delete_extension.py
--rw-r--r--   0        0        0     1769 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/dev.py
--rw-r--r--   0        0        0      607 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/scripts/__init__.py
--rw-r--r--   0        0        0    30537 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/scripts/dt.py
--rw-r--r--   0        0        0      926 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/scripts/utility.py
--rw-r--r--   0        0        0     2009 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/server_api.py
--rw-r--r--   0        0        0      464 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/shim.py
--rw-r--r--   0        0        0    11263 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/signing.py
--rw-r--r--   0        0        0     2940 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/utils.py
--rw-r--r--   0        0        0     2672 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/validate_schema.py
--rw-r--r--   0        0        0      600 2022-08-02 14:56:21.000000 dt-cli-1.6.7/dtcli/version.py
--rw-r--r--   0        0        0     1511 2022-08-02 14:56:21.000000 dt-cli-1.6.7/pyproject.toml
--rw-r--r--   0        0        0     4311 2022-08-02 14:57:24.468305 dt-cli-1.6.7/setup.py
--rw-r--r--   0        0        0     4318 2022-08-02 14:57:24.468914 dt-cli-1.6.7/PKG-INFO
+-rw-r--r--   0        0        0    11342 2022-09-29 14:50:40.000000 dt-cli-1.6.9/LICENSE
+-rw-r--r--   0        0        0     3232 2022-09-29 14:50:40.000000 dt-cli-1.6.9/README.md
+-rw-r--r--   0        0        0      638 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/__init__.py
+-rw-r--r--   0        0        0       95 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/__main__.py
+-rw-r--r--   0        0        0     5969 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/api.py
+-rw-r--r--   0        0        0     5130 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/building.py
+-rw-r--r--   0        0        0     2395 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/click_helpers.py
+-rw-r--r--   0        0        0     1726 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/constants.py
+-rw-r--r--   0        0        0     5055 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/delete_extension.py
+-rw-r--r--   0        0        0     1769 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/dev.py
+-rw-r--r--   0        0        0      607 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/scripts/__init__.py
+-rw-r--r--   0        0        0    30251 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/scripts/dt.py
+-rw-r--r--   0        0        0      926 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/scripts/utility.py
+-rw-r--r--   0        0        0     2009 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/server_api.py
+-rw-r--r--   0        0        0      464 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/shim.py
+-rw-r--r--   0        0        0    11263 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/signing.py
+-rw-r--r--   0        0        0     2940 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/utils.py
+-rw-r--r--   0        0        0     2672 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/validate_schema.py
+-rw-r--r--   0        0        0      600 2022-09-29 14:50:40.000000 dt-cli-1.6.9/dtcli/version.py
+-rw-r--r--   0        0        0     1513 2022-09-29 14:50:40.000000 dt-cli-1.6.9/pyproject.toml
+-rw-r--r--   0        0        0     4315 1970-01-01 00:00:00.000000 dt-cli-1.6.9/setup.py
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 dt-cli-1.6.9/PKG-INFO
```

### Comparing `dt-cli-1.6.7/LICENSE` & `dt-cli-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/README.md` & `dt-cli-1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/__init__.py` & `dt-cli-1.6.9/dtcli/__init__.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/api.py` & `dt-cli-1.6.9/dtcli/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,19 @@
             return
 
         r.raise_for_status()
         return r.json()
 
     def acquire_extensions(self):
         r = self.requests.get(f"{self.url_base}/api/v2/extensions", headers=self.headers)
+        # Temporary solution. It can cause too much data usage.
+        # Also we can hit a hard backend limit wrg to page size.
+        # Which can cause false negatives.
+        ext_num_tot = r.json()["totalCount"]
+        r = self.requests.get(f"{self.url_base}/api/v2/extensions?pageSize={ext_num_tot}", headers=self.headers)
         r.raise_for_status()
         return r.json()["extensions"]
 
     def acquire_extension_versions(self, fqdn: str):
         r = self.requests.get(self.url_base + f"/api/v2/extensions/{fqdn}", headers=self.headers)
 
         r.raise_for_status()
@@ -101,25 +106,26 @@
         matches = [v for v in versions if v.startswith(target_version)]
         if matches:
             return matches[0]
 
         raise SystemExit(f"Target version {target_version} does not exist. \nAvailable versions: {versions}")
 
     def download_schemas(self, target_version: str, download_dir: str):
-        """Downloads schemas from choosen version."""
+        """Downloads schemas from chosen version."""
         version = self.get_schema_target_version(target_version)
 
         if not os.path.exists(download_dir):
             os.makedirs(download_dir)
 
         header = self.headers
         header["accept"] = "application/octet-stream"
-        file = self.requests.get(self.url_base + f"/api/v2/extensions/schemas/{version}", headers=header, stream=True)
-        file.raise_for_status()
-        zfile = zipfile.ZipFile(io.BytesIO(file.content))
+        schema_file = self.requests.get(self.url_base + f"/api/v2/extensions/schemas/{version}",
+                                        headers=header, stream=True)
+        schema_file.raise_for_status()
+        zfile = zipfile.ZipFile(io.BytesIO(schema_file.content))
 
         THRESHOLD_ENTRIES = 10000
         THRESHOLD_SIZE = 1000000000
         THRESHOLD_RATIO = 10
 
         totalSizeArchive = 0
         totalEntryArchive = 0
```

### Comparing `dt-cli-1.6.7/dtcli/building.py` & `dt-cli-1.6.9/dtcli/building.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/click_helpers.py` & `dt-cli-1.6.9/dtcli/click_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
 def deprecated(alternative: Optional[str], alternative_help: Optional[str] = None):
     """
     This has to happen this way.
 
     Click decorator registers the function automatically, so I'd need to track where it's registered or something [so
-    the acutal function that's run could be decorated], instead I've opted for spawining 2 decorators and just doing
+    the actual function that's run could be decorated], instead I've opted for spawning 2 decorators and just doing
     it the hacky way.
     """
     if alternative:
         alt_text = f"\nPlease consider using {click.style(alternative,fg='bright_cyan')} instead." \
                    f"{' ' + alternative_help.capitalize() + '.' if alternative_help else ''}\n"
     else:
         alt_text = ""
```

### Comparing `dt-cli-1.6.7/dtcli/constants.py` & `dt-cli-1.6.9/dtcli/constants.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/delete_extension.py` & `dt-cli-1.6.9/dtcli/delete_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,19 +54,14 @@
                 extensions[extension][mc["value"]["version"]]["monitoring_configurations"].append(mc)
 
     s = State(extensions)
     return s
 
 
 def acquire_state_for_extension(client: DynatraceAPIClient, extension: str) -> State:
-    extensions_listing = list(map(lambda e: e["extensionName"], client.acquire_extensions()))
-
-    if extension not in extensions_listing:
-        raise Exception("Extension doesn't exist")
-
     versions = client.acquire_extension_versions(extension)
     # TODO: is this really any?
     extension_data: Dict[str, Dict[str, Any]] = defaultdict(dict)
     for e in versions:
         name, version = e["extensionName"], e["version"]
         extension_data[name][version] = {"monitoring_configurations": []}
```

### Comparing `dt-cli-1.6.7/dtcli/dev.py` & `dt-cli-1.6.9/dtcli/dev.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/scripts/__init__.py` & `dt-cli-1.6.9/dtcli/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/scripts/dt.py` & `dt-cli-1.6.9/dtcli/scripts/dt.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 from dtcli import signing
 from dtcli.click_helpers import deprecated, compose_click_decorators_2, mk_click_callback
 from dtcli.scripts.utility import app as utility_app
 from dtcli.shim import _Path_is_relative
 
 
 CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
+FORCE_OPTION = typer.Option(False,
+                            "--force", "-f",
+                            help="Ignore subtleties, overwrite without prompt, when in doubt - advance!")
 
 
 def validate_parse_subject(ctx, param, value):
     if value is None:
         return None
 
     def split_pair_and_verify_key(pair):
@@ -506,18 +509,23 @@
         kwargs["dev_subject"],
         datetime.datetime.today() + datetime.timedelta(days=kwargs["days_valid"]),
         kwargs["ca_passphrase"],
         kwargs["dev_passphrase"],
     )
 
 
+_deprecate_above, _deprecate_below = deprecated("dt ext assemble or dt ext sign")
+
+
+@_deprecate_above
 @extension.command(
     help=f"Build and sign extension package from the given extension directory (default: {const.DEFAULT_EXTENSION_DIR})"
          f" that contains extension.yaml and additional asset directories"
 )
+@_deprecate_below
 @click.option(
     "--extension-directory",
     default=const.DEFAULT_EXTENSION_DIR,
     show_default=True,
     help="Directory where the `extension.yaml' and other extension files are located",
 )
 @click.option(
@@ -601,44 +609,31 @@
         certificate_file_path,
         private_key_file_path,
         kwargs["dev_passphrase"],
         kwargs["keep_intermediate_files"],
     )
 
 
-@extension.command()
-@click.option(
-    "--src",
-    "--source",
-    "source",
-    default=const.DEFAULT_EXTENSION_DIR2,
-    type=click.Path(exists=True, file_okay=False),
-    callback=mk_click_callback(Path),
-    show_default=True,
-    help="Directory where the `extension.yaml' and other extension files are located",
-)
-@click.option(
-    "-o",
-    "--output",
-    "destination",
-    type=click.Path(writable=True, dir_okay=False),
-    default=str(const.DEFAULT_BUILD_OUTPUT),
-    callback=mk_click_callback(Path),
-    show_default=True,
-    help="Location where the extension package will be written",
-)
-@click.option(
-    "-f",
-    "--force",
-    is_flag=True,
-    default=False,
-    show_default=True,
-    help="Ignore subtleties, overwrite without prompt, when in doubt - advance!",
-)
-def assemble(source, destination, force):
+@typer_extension.command()
+def assemble(
+        source: Path = typer.Option(
+            const.DEFAULT_EXTENSION_DIR2,
+            "--src", "--source",
+            exists=True, dir_okay=True,
+            readable=True,
+            help="Directory where the `extension.yaml' and other extension files are located",
+        ),
+        destination: Path = typer.Option(
+            str(const.DEFAULT_BUILD_OUTPUT),
+            "-o", "--output",
+            writable=True, dir_okay=False,
+            help="Location where the extension package will be written",
+        ),
+        force: bool = FORCE_OPTION
+):
     """
     Build extension package.
     """
     if destination.exists() and not force:
         raise click.BadParameter(f"destination {destination} already exists, please try again with --force to proceed "
                                  f"irregardless", param_hint="--source")
 
@@ -665,19 +660,15 @@
     ),
     certkey: Path = typer.Option(
         const.DEFAULT_KEYCERT_PATH,
         "--key",
         exists=True, dir_okay=False,
         help="Location of the fused key-certificate for signing with",
     ),
-    # TODO: extract this as a common option
-    force: bool = typer.Option(
-        False,
-        "--force", "-f",
-        help="Ignore subtleties, overwrite without prompt, when in doubt - advance!")
+    force: bool = FORCE_OPTION
 ):
     """
     Produce signed extension package.
 
     Certificates with passphrase are currently not supported as if you required that kind of level of security it
     wouldn't be wise to use this command in it's current form. If you'd like this feature to be implemented sooner
     please visit https://github.com/dynatrace-oss/dt-cli/issues/81 and upvote.
@@ -789,15 +780,21 @@
 def delete(**kwargs):
     """
     Delete extension from Dynatrace Cluster.
 
     Example: custom:com.dynatrace.extension.extension-name
     """
     token = kwargs["api_token_path"]
-    delete_extension.wipe(fqdn=kwargs["extension"], tenant=kwargs["tenant_url"], token=token)
+    try:
+        delete_extension.wipe(fqdn=kwargs["extension"], tenant=kwargs["tenant_url"], token=token)
+    except requests.exceptions.HTTPError as err:
+        if err.response.status_code == 404:
+            raise click.BadParameter(err, param_hint="EXTENSION")
+        else:
+            raise
 
 
 @extension.command(
     help="Validate extension with schemas"
 )
 @click.option(
     "--instance",
@@ -850,24 +847,12 @@
     extension_directory = kwargs["extension_directory"]
 
     return dev.pack_python_extension(
         setup_path=path_to_setup_py, target_path=extension_directory, additional_path=additional_libraries_dir
     )
 
 
-# becasue of how typer works there has to be at least 2 commands for it to create a group
-# TODO: remove this after another command is migrated
-# https://typer.tiangolo.com/tutorial/using-click/#how-typer-works
-@typer_extension.command()
-def please_remove_this_later():
-    pass
-
-
 for name, cmd in typer.main.get_command(typer_extension).commands.items():
-    # TODO: remove this after another command is migrated
-    if name == "please-remove-this-later":
-        continue
-
     extension.add_command(cmd, name)
 
 
 main.add_command(typer.main.get_command(utility_app), "utility")
```

### Comparing `dt-cli-1.6.7/dtcli/scripts/utility.py` & `dt-cli-1.6.9/dtcli/scripts/utility.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/server_api.py` & `dt-cli-1.6.9/dtcli/server_api.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/signing.py` & `dt-cli-1.6.9/dtcli/signing.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/utils.py` & `dt-cli-1.6.9/dtcli/utils.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/validate_schema.py` & `dt-cli-1.6.9/dtcli/validate_schema.py`

 * *Files identical despite different names*

### Comparing `dt-cli-1.6.7/dtcli/version.py` & `dt-cli-1.6.9/dtcli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.6.7"
+__version__ = "1.6.9"
```

### Comparing `dt-cli-1.6.7/pyproject.toml` & `dt-cli-1.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 maintainers = ["Wiktor Bachnik <wiktor.bachnik@dynatrace.com>", "Vagiz Duseev <vagiz.duseev@dynatrace.com>"]
 name = "dt-cli"
 packages = [
   {include = "dtcli"},
 ]
 readme = "README.md"
 repository = "https://github.com/dynatrace-oss/dt-cli"
-version = "1.6.7"
+version = "1.6.9"
 
 
 [tool.poetry.dependencies]
 PyYAML = "^5.4"
 asn1crypto = "^1.4"
 click-aliases = "^1.0"
 cryptography = "^3.4"
 python = "^3.8"
-wheel = "^0.36"
+wheel = "^0.37.1"
 requests = "^2.26"
 jsonschema = "^4.7.2"
 typer = "^0.6.1"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^3.5"
 black = {version = "^20.8b1", allow-prereleases = true}
```

### Comparing `dt-cli-1.6.7/setup.py` & `dt-cli-1.6.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 ['PyYAML>=5.4,<6.0',
  'asn1crypto>=1.4,<2.0',
  'click-aliases>=1.0,<2.0',
  'cryptography>=3.4,<4.0',
  'jsonschema>=4.7.2,<5.0.0',
  'requests>=2.26,<3.0',
  'typer>=0.6.1,<0.7.0',
- 'wheel>=0.36,<0.37']
+ 'wheel>=0.37.1,<0.38.0']
 
 entry_points = \
 {'console_scripts': ['dt = dtcli.__main__:main']}
 
 setup_kwargs = {
     'name': 'dt-cli',
-    'version': '1.6.7',
+    'version': '1.6.9',
     'description': 'Dynatrace CLI',
     'long_description': '# dt-cli — Dynatrace developer\'s toolbox\n\nDynatrace CLI is a command line utility that assists in signing, building and uploading\nextensions for Dynatrace Extension Framework 2.0.\n\n<p>\n  <a href="https://pypi.org/project/dt-cli/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dt-cli?color=blue&logo=python&logoColor=white"></a>\n  <a href="https://pypi.org/project/dt-cli/"><img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/dt-cli?logo=python&logoColor=white"></a>\n  <a href="https://github.com/dynatrace-oss/dt-cli/actions/workflows/built-test-release.yml"><img alt="GitHub Workflow Status (main branch)" src="https://img.shields.io/github/workflow/status/dynatrace-oss/dt-cli/Build%20Test%20Release/main?logo=github"></a>\n</p>\n\n\n### Features\n\n* Build and sign extensions from source\n* Generate development certificates for extension signing\n* Generate CA certificates for development\n* Validate and upload extension to Dynatrace Extension Framework 2.0.\n\n## Installation\n\n```shell\npip install dt-cli\n```\n\n## Usage\n\n1. Generate certificates\n```sh\n  dt extension gencerts\n```\n2. Upload your `ca.pem` certificate to the Dynatrace credential vault\n\nSee: [Add your root certificate to the Dynatrace credential vault](https://www.dynatrace.com/support/help/extend-dynatrace/extensions20/sign-extension/#add-your-root-certificate-to-the-dynatrace-credential-vault)\n\n3. Build and sign, then upload extension\n```sh\n  dt extension build\n  dt extension upload\n```\nUse `dt extension --help` to learn more\n\n4. Download extension schemas\n```sh\n  dt extension schemas\n```\n_API permissions needed: `extensions.read`_\n\nThis script should only be needed once, whenever schema files are missing or you want to target a different version than what you already have. It does the following:\n* Downloads all the extension schema files of a specific version\n* Schemas are downloaded to `schemas` folder\n\n5. Wipes out extension from Dynatrace Cluster\n```sh\n  dt extension delete\n```\nUse `dt extension --help` to learn more\n\n\n## Using dt-cli from your Python code\n\nYou may want to use some commands implemented by `dt-cli` directly in your Python code, e.g. to automatically sign your extension in a CI environment.\nHere\'s an example of building an extension programatically, it assumes `dtcli` package is already installed and available in your working environment.\n\n\n```python\nfrom dtcli import building\n\n\nbuilding.build_extension(\n    extension_dir_path = \'./extension\',\n    extension_zip_path = \'./extension.zip\',\n    extension_zip_sig_path = \'./extension.zip.sig\',\n    target_dir_path = \'./dist\',\n    certificate_file_path = \'./developer.crt\',\n    private_key_file_path = \'./developer.key\',\n    dev_passphrase=None,\n    keep_intermediate_files=False,\n)\n```\n\n## Development\n\nSee our [CONTRIBUTING](CONTRIBUTING.md) guidelines and instructions.\n\n## Contributions\n\nYou are welcome to contribute using Pull Requests to the respective\nrepository. Before contributing, please read our\n[Code of Conduct](https://github.com/dynatrace-oss/dt-cli/blob/main/CODE_OF_CONDUCT.md).\n\n## License\n\n`dt-cli` is an Open Source Project. Please see\n[LICENSE](https://github.com/dynatrace-oss/dt-cli/blob/main/LICENSE) for more information.',
     'author': 'Wiktor Bachnik',
     'author_email': 'wiktor.bachnik@dynatrace.com',
     'maintainer': 'Wiktor Bachnik',
     'maintainer_email': 'wiktor.bachnik@dynatrace.com',
     'url': 'https://github.com/dynatrace-oss/dt-cli',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['dtcli',
 'dtcli.scripts'] package_data = \ {'': ['*']} install_requires = \
 ['PyYAML>=5.4,<6.0', 'asn1crypto>=1.4,<2.0', 'click-aliases>=1.0,<2.0',
 'cryptography>=3.4,<4.0', 'jsonschema>=4.7.2,<5.0.0', 'requests>=2.26,<3.0',
-'typer>=0.6.1,<0.7.0', 'wheel>=0.36,<0.37'] entry_points = \
+'typer>=0.6.1,<0.7.0', 'wheel>=0.37.1,<0.38.0'] entry_points = \
 {'console_scripts': ['dt = dtcli.__main__:main']} setup_kwargs = { 'name': 'dt-
-cli', 'version': '1.6.7', 'description': 'Dynatrace CLI', 'long_description':
+cli', 'version': '1.6.9', 'description': 'Dynatrace CLI', 'long_description':
 '# dt-cli â Dynatrace developer\'s toolbox\n\nDynatrace CLI is a command line
 utility that assists in signing, building and uploading\nextensions for
 Dynatrace Extension Framework 2.0.\n\n
 \n [PyPI]\n [PyPI_-_Python_Version]\n [GitHub_Workflow_Status_(main_branch)]\n
 \n\n\n### Features\n\n* Build and sign extensions from source\n* Generate
 development certificates for extension signing\n* Generate CA certificates for
 development\n* Validate and upload extension to Dynatrace Extension Framework
```

### Comparing `dt-cli-1.6.7/PKG-INFO` & `dt-cli-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: dt-cli
-Version: 1.6.7
+Version: 1.6.9
 Summary: Dynatrace CLI
 Home-page: https://github.com/dynatrace-oss/dt-cli
 License: Apache-2.0
 Keywords: dynatrace,cli,extensions
 Author: Wiktor Bachnik
 Author-email: wiktor.bachnik@dynatrace.com
 Maintainer: Wiktor Bachnik
 Maintainer-email: wiktor.bachnik@dynatrace.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=5.4,<6.0)
 Requires-Dist: asn1crypto (>=1.4,<2.0)
 Requires-Dist: click-aliases (>=1.0,<2.0)
 Requires-Dist: cryptography (>=3.4,<4.0)
 Requires-Dist: jsonschema (>=4.7.2,<5.0.0)
 Requires-Dist: requests (>=2.26,<3.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
-Requires-Dist: wheel (>=0.36,<0.37)
+Requires-Dist: wheel (>=0.37.1,<0.38.0)
 Project-URL: Documentation, https://dt-cli.readthedocs.io
 Project-URL: Repository, https://github.com/dynatrace-oss/dt-cli
 Description-Content-Type: text/markdown
 
 # dt-cli — Dynatrace developer's toolbox
 
 Dynatrace CLI is a command line utility that assists in signing, building and uploading
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: dt-cli Version: 1.6.7 Summary: Dynatrace CLI Home-
+Metadata-Version: 2.1 Name: dt-cli Version: 1.6.9 Summary: Dynatrace CLI Home-
 page: https://github.com/dynatrace-oss/dt-cli License: Apache-2.0 Keywords:
 dynatrace,cli,extensions Author: Wiktor Bachnik Author-email:
 wiktor.bachnik@dynatrace.com Maintainer: Wiktor Bachnik Maintainer-email:
 wiktor.bachnik@dynatrace.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Requires-Dist: PyYAML (>=5.4,<6.0) Requires-Dist: asn1crypto
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Requires-Dist: PyYAML (>=5.4,<6.0) Requires-Dist: asn1crypto
 (>=1.4,<2.0) Requires-Dist: click-aliases (>=1.0,<2.0) Requires-Dist:
 cryptography (>=3.4,<4.0) Requires-Dist: jsonschema (>=4.7.2,<5.0.0) Requires-
 Dist: requests (>=2.26,<3.0) Requires-Dist: typer (>=0.6.1,<0.7.0) Requires-
-Dist: wheel (>=0.36,<0.37) Project-URL: Documentation, https://dt-
+Dist: wheel (>=0.37.1,<0.38.0) Project-URL: Documentation, https://dt-
 cli.readthedocs.io Project-URL: Repository, https://github.com/dynatrace-oss/
 dt-cli Description-Content-Type: text/markdown # dt-cli â Dynatrace
 developer's toolbox Dynatrace CLI is a command line utility that assists in
 signing, building and uploading extensions for Dynatrace Extension Framework
 2.0.
 [PyPI] [PyPI_-_Python_Version] [GitHub_Workflow_Status_(main_branch)]
 ### Features * Build and sign extensions from source * Generate development
```

