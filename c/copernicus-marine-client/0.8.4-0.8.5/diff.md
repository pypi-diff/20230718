# Comparing `tmp/copernicus_marine_client-0.8.4.tar.gz` & `tmp/copernicus_marine_client-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.8.4.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.8.5.tar", max compression
```

## Comparing `copernicus_marine_client-0.8.4.tar` & `copernicus_marine_client-0.8.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     9742 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.4/README.md
--rw-r--r--   0        0        0     3171 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.4/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    22196 2023-07-11 15:10:39.591359 copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0     6162 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/request_structure.py
--rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      994 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     3797 2023-07-11 08:16:13.394928 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     4823 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_login.py
--rw-r--r--   0        0        0     8870 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0    17026 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     5550 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/configuration_files_creator.py
--rw-r--r--   0        0        0     7868 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     4616 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0     8748 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_opendap.py
--rw-r--r--   0        0        0     8501 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_s3native.py
--rw-r--r--   0        0        0     4397 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_zarr.py
--rw-r--r--   0        0        0     4456 2023-07-13 15:58:15.755707 copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/subset_xarray.py
--rw-r--r--   0        0        0      768 2023-07-04 12:33:19.408010 copernicus_marine_client-0.8.4/copernicus_marine_client/logging_conf.json
--rw-r--r--   0        0        0      623 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.4/copernicus_marine_client/utils.py
--rw-r--r--   0        0        0      887 2023-07-17 09:15:30.602198 copernicus_marine_client-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    11278 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.4/setup.py
--rw-r--r--   0        0        0    10677 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     9742 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.5/README.md
+-rw-r--r--   0        0        0     3171 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.5/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.5/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    22039 2023-07-17 14:28:06.899037 copernicus_marine_client-0.8.5/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     6162 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.5/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       10 2023-02-28 13:18:03.224455 copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      994 2023-07-06 14:45:40.213214 copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3539 2023-07-17 16:09:12.015945 copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4829 2023-07-17 13:45:09.276750 copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_login.py
+-rw-r--r--   0        0        0     8870 2023-07-17 09:14:07.365808 copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0    17026 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     5883 2023-07-17 13:45:09.280750 copernicus_marine_client-0.8.5/copernicus_marine_client/configuration_files_creator.py
+-rw-r--r--   0        0        0     7642 2023-07-17 16:09:12.027945 copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     4207 2023-07-17 13:45:09.280750 copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0     1328 2023-07-17 16:09:12.027945 copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_native.py
+-rw-r--r--   0        0        0     8748 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0     7938 2023-07-17 16:09:12.027945 copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_s3native.py
+-rw-r--r--   0        0        0     4395 2023-07-17 16:09:12.027945 copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_zarr.py
+-rw-r--r--   0        0        0     4456 2023-07-13 15:58:15.755707 copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/subset_xarray.py
+-rw-r--r--   0        0        0      768 2023-07-04 12:33:19.408010 copernicus_marine_client-0.8.5/copernicus_marine_client/logging_conf.json
+-rw-r--r--   0        0        0      623 2023-07-13 06:55:20.799279 copernicus_marine_client-0.8.5/copernicus_marine_client/utils.py
+-rw-r--r--   0        0        0      887 2023-07-18 12:04:37.403009 copernicus_marine_client-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0    11278 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.5/setup.py
+-rw-r--r--   0        0        0    10677 1970-01-01 00:00:00.000000 copernicus_marine_client-0.8.5/PKG-INFO
```

### Comparing `copernicus_marine_client-0.8.4/README.md` & `copernicus_marine_client-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/__init__.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/catalogue_parser.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/catalogue_parser/catalogue_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,21 +107,18 @@
 ) -> CopernicusMarineCatalogue:
     return merge_catalogues(
         parse_dissemination_unit_catalogue(overwrite_cache=overwrite_cache),
         parse_marine_data_store_catalogue(overwrite_cache=overwrite_cache),
     )
 
 
-# --------------------------------------------------------
-# --- Function specific for cmems-be.lobelia catalogue ---
-# --------------------------------------------------------
 @cachier(stale_after=timedelta(hours=3))
 def _fetch_raw_products() -> list[dict[str, Any]]:
     response = requests.post(
-        "https://cmems-be.lobelia.earth/api/datasets",
+        "https://data-be-prd.marine.copernicus.eu/api/datasets",
         json={"size": 1000, "includeOmis": True},
     )
     assert response.ok, response.text
     raw_catalogue: dict[str, Any] = loads(response.text)
     return map_parallel(
         _fetch_raw_product,
         tqdm(
@@ -135,15 +132,15 @@
     response = requests.get(product_url(product_id))
     assert response.ok, response.text
     return loads(response.text)
 
 
 def product_url(product_id: str) -> str:
     return (
-        f"https://cmems-be.lobelia.earth/api/dataset/{product_id}"
+        f"https://data-be-prd.marine.copernicus.eu/api/dataset/{product_id}"
         + "?variant=detailed-v2"
     )
 
 
 def variable_title_to_standard_name(variable_title: str) -> str:
     return variable_title.lower().replace(" ", "_")
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/catalogue_parser/request_structure.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/catalogue_parser/request_structure.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,21 +37,14 @@
     > copernicus-marine describe --contains METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 --include-datasets
 
     \b
     > copernicus-marine describe -c METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
     """,  # noqa
 )
 @click.option(
-    "--one-line",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Output JSON on one line",
-)
-@click.option(
     "--include-description",
     type=bool,
     is_flag=True,
     default=False,
     help="Include product description in output",
 )
 @click.option(
@@ -92,15 +85,14 @@
         "(based on standard logging library)."
     ),
 )
 def describe(
     include_description: bool,
     include_datasets: bool,
     include_keywords: bool,
-    one_line: bool,
     contains: list[str],
     overwrite_cache: bool,
     log_level: str = "INFO",
 ) -> None:
     if log_level == "QUIET":
         logging.root.disabled = True
         logging.root.setLevel(level="CRITICAL")
@@ -124,20 +116,16 @@
             attributes.pop("description", None)
         if not include_datasets:
             attributes.pop("datasets", None)
         if not include_keywords:
             attributes.pop("keywords", None)
         return obj.__dict__
 
-    json_dump = (
-        dumps(catalogue, default=default_filter, sort_keys=False)
-        if one_line
-        else dumps(
-            catalogue, default=default_filter, sort_keys=False, indent=2
-        )
+    json_dump = dumps(
+        catalogue, default=default_filter, sort_keys=False, indent=2
     )
     logger = logging.getLogger("blank_logger")
     logger.warn(json_dump)
 
 
 if __name__ == "__main__":
     cli_group_describe()
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_login.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     password = get_credential(
         password,
         "password",
         hide_input=True,
         config_file_directory=config_file_directory,
     )
     result_check = check_copernicus_marine_credentials(username, password)
-    if result_check:
+    if result_check.error:
         logging.warning(
             "Invalid credentials, your download will not be authenticated"
         )
     return (username, password)
 
 
 if __name__ == "__main__":
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_native.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_native.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/configuration_files_creator.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/configuration_files_creator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import base64
 import configparser
 import logging
 import os
+from dataclasses import dataclass
+from datetime import timedelta
 from netrc import netrc
 from typing import Literal, Optional
 
 import click
 import lxml.html
 import requests
+from cachier import cachier
 
 
 def load_credential_from_copernicus_marine_config_file(
     credential_type: Literal["username", "password"],
     config_filename: str,
 ) -> Optional[str]:
     config_file = open(config_filename)
@@ -109,17 +112,23 @@
     config_string = base64.b64encode(
         "".join(config_lines).encode("ascii", "strict")
     ).decode("utf8")
     config_file.write(config_string)
     config_file.close()
 
 
+@dataclass
+class CheckCredentialsResponse:
+    error: Optional[ConnectionRefusedError]
+
+
+@cachier(stale_after=timedelta(hours=5))
 def check_copernicus_marine_credentials(
     username: Optional[str], password: Optional[str]
-) -> Optional[ConnectionRefusedError]:
+) -> CheckCredentialsResponse:
     """
     Check provided Copernicus Marine Credentials are correct.
 
     Parameters
     ----------
     username : str
         Copernicus Marine Username, provided for free from https://marine.copernicus.eu
@@ -138,23 +147,25 @@
         he.attrib["name"]: he.attrib["value"]
         for he in hidden_elements_from_html
     }
     playload["username"] = username
     playload["password"] = password
     response = conn_session.post(cmems_cas_url, data=playload)
     if response.text.find("success") == -1:
-        credential_error_message = ConnectionRefusedError(
-            "Incorrect username or password.\n"
-            "Learn how to recover your credentials at: "
-            "https://help.marine.copernicus.eu/en/articles/"
-            "4444552-i-forgot-my-username-or-my-password-what-should-i-do"
+        check_credentials_response = CheckCredentialsResponse(
+            error=ConnectionRefusedError(
+                "Incorrect username or password.\n"
+                "Learn how to recover your credentials at: "
+                "https://help.marine.copernicus.eu/en/articles/"
+                "4444552-i-forgot-my-username-or-my-password-what-should-i-do"
+            )
         )
-        logging.error(credential_error_message)
-        return credential_error_message
-    return None
+        logging.error(check_credentials_response.error)
+        return check_credentials_response
+    return CheckCredentialsResponse(error=None)
 
 
 def main(
     username: str,
     password: str,
     config_file_directory: str,
     force_download: bool,
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 import logging
 import os
 import re
 from ftplib import FTP
 from itertools import chain
 from multiprocessing.pool import ThreadPool
-from typing import Any, Optional, Tuple
+from typing import Any, List, Optional, Tuple
 
-import click
 from numpy import append, arange
 from tqdm import tqdm
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
 )
-from copernicus_marine_client.utils import (
-    FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
-    get_unique_filename,
+from copernicus_marine_client.download_functions.download_native import (
+    download_native,
 )
+from copernicus_marine_client.utils import get_unique_filename
 
 # /////////////////////////////
 # ---Using ftplib
 # /////////////////////////////
 
 
 def download_ftp(
     username: str,
     password: str,
     native_request: NativeRequest,
 ) -> str:
-    message, host, filenames_in = download_header(
-        str(native_request.dataset_url),
-        native_request.regex,
+    filenames_in, filenames_out, host = download_native(
         username,
         password,
+        native_request,
+        download_header,
+        create_filenames_out,
     )
-    filenames_out = create_filenames_out(
-        filenames_in=filenames_in,
-        output_directory=native_request.output_directory,
-        no_directories=native_request.no_directories,
-        overwrite=native_request.overwrite,
-    )
-    logging.info(message)
-    if native_request.show_outputnames:
-        logging.info("Output filenames:")
-        for filename_out in filenames_out:
-            logging.info(filename_out)
-    if not native_request.force_download:
-        click.confirm(FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True)
+    return download_files(
+        host, username, password, filenames_in, filenames_out
+    )
+
 
+def download_files(
+    host: str,
+    username: str,
+    password: str,
+    filenames_in: List[str],
+    filenames_out: List[str],
+) -> str:
     pool = ThreadPool()
     nfiles_per_process, nfiles = 1, len(filenames_in)
     indexes = append(
         arange(0, nfiles, nfiles_per_process, dtype=int),
         nfiles,
     )
     groups_in_files = [
@@ -60,31 +58,30 @@
     ]
     groups_out_files = [
         filenames_out[indexes[i] : indexes[i + 1]]
         for i in range(len(indexes) - 1)
     ]
     groups_in_files_count = len(groups_in_files)
     download_summary_list = pool.map(
-        download_files,
+        _download_files,
         zip(
             [host] * groups_in_files_count,
             [username] * groups_in_files_count,
             [password] * groups_in_files_count,
             groups_in_files,
             groups_out_files,
         ),
     )
     download_summary = "".join(map(str, download_summary_list))
     return download_summary
 
 
 def download_header(
     data_path: str, regex: Optional[str], username: str, password: str
-) -> Tuple[str, str, list[str]]:
-
+) -> Tuple[str, str, list[str], float]:
     (host, path) = parse_ftp_dataset_url(data_path)
     message = "You requested the download of the following files:\n"
     total_size = 0
     with FTP(host) as ftp:
         ftp.login(user=username, passwd=password)
         raw_filenames = get_filenames_recursively(ftp, path)
         if regex:
@@ -116,15 +113,15 @@
         message += str(result[0])
         message += f" - {format_file_size(float(result[1]))}\n"
     if len(flattened_results) > 20:
         message += f"Printed 20 out of {len(flattened_results)} files\n"
     message += (
         f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
     )
-    return (message, host, filenames)
+    return (message, host, filenames, total_size)
 
 
 def get_filenames_recursively(
     ftp: FTP, path: str, extensions: list[str] = [".nc"]
 ) -> list[str]:
     if any(extension in path for extension in extensions):
         # path is a file
@@ -152,15 +149,15 @@
         ftp.login(user=username, passwd=password)
         list_tuples = [
             (filename, ftp.size(filename)) for filename in filenames
         ]
     return list_tuples
 
 
-def download_files(
+def _download_files(
     tuple_ftp_filename: Tuple[str, str, str, list[str], list[str]],
 ) -> str:
     def _ftp_file_download(ftp, file_in, file_out):
         """
         Download ONE file and return a string of the result
         """
         os.makedirs(os.path.dirname(file_out), exist_ok=True)
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_motu.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_motu.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-import logging
-import xml.dom.minidom
+import os
 from os import path
 from subprocess import run
 from typing import Optional
 
 import click
 
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
     CopernicusMarineCatalogue,
     get_product_from_url,
     parse_catalogue,
 )
 from copernicus_marine_client.catalogue_parser.request_structure import (
     SubsetRequest,
 )
-from copernicus_marine_client.utils import FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE
+from copernicus_marine_client.utils import (
+    FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
+    get_unique_filename,
+)
 
 
 def parse_motu_dataset_url(data_path: str) -> str:
     host = data_path.split("/motu-web/Motu")[0] + "/motu-web/Motu"
     return host
 
 
@@ -45,25 +47,35 @@
         output_filename = "data.nc"
     else:
         output_filename = subset_request.output_filename
     if not subset_request.output_directory:
         output_directory = "."
     else:
         output_directory = subset_request.output_directory
+
+    if not subset_request.force_download:
+        click.confirm(FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True)
+
+    output_filepath = path.join(output_directory, output_filename)
+
+    if os.path.exists(output_filepath):
+        if not subset_request.overwrite:
+            output_filepath = get_unique_filename(filepath=output_filepath)
+
     options_list = [
         "--motu",
         parse_motu_dataset_url(str(subset_request.dataset_url)),
         "--service-id",
         product_id + "-TDS",
         "--product-id",
         dataset_id,
         "--out-dir",
-        output_directory,
+        os.path.dirname(output_filepath),
         "--out-name",
-        output_filename,
+        os.path.basename(output_filepath),
         "--user",
         username,
         "--pwd",
         password,
     ]
 
     if subset_request.minimal_longitude is not None:
@@ -127,37 +139,15 @@
         options_list.extend(
             [
                 flat
                 for var in subset_request.variables
                 for flat in ["--variable", var]
             ]
         )
-    description_xml = run(
-        [
-            "motuclient",
-        ]
-        + options_list
-        + ["--quiet", "--describe-product", "-o", "console"],
-        capture_output=True,
-    )
-    description_dom = xml.dom.minidom.parseString(description_xml.stdout)
-    logger = logging.getLogger("blank_logger")
-    logger.warn(description_dom.toprettyxml(newl=""))
-    size_xml = run(
-        [
-            "motuclient",
-        ]
-        + options_list
-        + ["--quiet", "--size", "-o", "console"],
-        capture_output=True,
-    )
-    size_dom = xml.dom.minidom.parseString(size_xml.stdout)
-    logger.warn(size_dom.toprettyxml(newl=""))
-    if not subset_request.force_download:
-        click.confirm(FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True)
+
     run(
         [
             "motuclient",
         ]
         + options_list
     )
-    return path.join(output_directory, output_filename)
+    return output_filepath
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_opendap.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_opendap.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_s3native.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_s3native.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-import logging
 import os
 import re
 from multiprocessing.pool import ThreadPool
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import boto3
 import botocore
-import click
 from numpy import append, arange
 from tqdm import tqdm
 
 from copernicus_marine_client.catalogue_parser.request_structure import (
     NativeRequest,
 )
-from copernicus_marine_client.utils import (
-    FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE,
-    get_unique_filename,
+from copernicus_marine_client.download_functions.download_native import (
+    download_native,
 )
+from copernicus_marine_client.utils import get_unique_filename
 
 MARINE_DATA_LAKE_LISTING_ENDPOINT = "https://marine.copernicus.eu"
 MARINE_DATA_LAKE_LISTING_NATIVE_BUCKET = "mdl-native-list"
 MARINE_DATA_LAKE_DOWNLOAD_NATIVE_BUCKET = "mdl-native"
 MARINE_DATA_LAKE_S3_LISTING_NATIVE_ROOT_URI = (
     f"{MARINE_DATA_LAKE_LISTING_NATIVE_BUCKET}/native"
 )
@@ -31,34 +29,29 @@
 
 
 def download_s3native(
     username: str,
     password: str,
     native_request: NativeRequest,
 ) -> str:
-    message, endpoint_url, filenames_in = download_header(
-        [str(native_request.dataset_url)],
-        native_request.regex,
+    filenames_in, filenames_out, endpoint_url = download_native(
         username,
         password,
+        native_request,
+        download_header,
+        create_filenames_out,
     )
-    filenames_out = create_filenames_out(
-        filenames_in=filenames_in,
-        output_directory=native_request.output_directory,
-        no_directories=native_request.no_directories,
-        overwrite=native_request.overwrite,
-    )
-    logging.info(message)
-    if native_request.show_outputnames:
-        logging.info("Output filenames:")
-        for filename_out in filenames_out:
-            logging.info(filename_out)
-    if not native_request.force_download:
-        click.confirm(FORCE_DOWNLOAD_CLI_PROMPT_MESSAGE, abort=True)
+    return download_files(endpoint_url, filenames_in, filenames_out)
 
+
+def download_files(
+    endpoint_url: str,
+    filenames_in: List[str],
+    filenames_out: List[str],
+) -> str:
     pool = ThreadPool()
     nfiles_per_process, nfiles = 1, len(filenames_in)
     indexes = append(
         arange(0, nfiles, nfiles_per_process, dtype=int),
         nfiles,
     )
     groups_in_files = [
@@ -72,52 +65,50 @@
 
     for groups_out_file in groups_out_files:
         parent_dir = Path(groups_out_file[0]).parent
         if not os.path.isdir(parent_dir):
             os.makedirs(parent_dir)
 
     download_summary_list = pool.imap(
-        download_files,
+        _download_files,
         zip(
             [endpoint_url] * len(groups_in_files),
             groups_in_files,
             groups_out_files,
         ),
     )
     list(tqdm(download_summary_list, total=len(groups_in_files)))
     download_summary = "Download complete"
     return download_summary
 
 
 def download_header(
-    data_paths: list[str], regex: Optional[str], username: str, password: str
-) -> Tuple[str, str, list[str]]:
-    path_dict = parse_s3native_dataset_url(data_paths)
+    data_path: str, regex: Optional[str], username: str, password: str
+) -> Tuple[str, str, list[str], float]:
+    (endpoint_url, path) = parse_s3native_dataset_url(data_path)
     message = "You requested the download of the following files:\n"
     filenames, sizes, total_size = [], [], 0.0
-    for endpoint_url, paths in path_dict.items():
-        for path in paths:
-            raw_filenames = list_files_on_marine_data_lake_s3(path)
-            filename_filtered = []
-            for filename, size in raw_filenames:
-                if not regex or re.match(regex, filename):
-                    filenames += [filename]
-                    sizes += [float(size)]
-                    total_size += float(size)
-                    filename_filtered.append((filename, size))
+    raw_filenames = list_files_on_marine_data_lake_s3(path)
+    filename_filtered = []
+    for filename, size in raw_filenames:
+        if not regex or re.match(regex, filename):
+            filenames += [filename]
+            sizes += [float(size)]
+            total_size += float(size)
+            filename_filtered.append((filename, size))
 
     for filename, size in filename_filtered[:20]:
         message += str(filename)
         message += f" - {format_file_size(float(size))}\n"
     if len(filenames) > 20:
         message += f"Printed 20 out of {len(filenames)} files\n"
     message += (
         f"\nTotal size of the download: {format_file_size(total_size)}\n\n"
     )
-    return (message, endpoint_url, filenames)
+    return (message, endpoint_url, filenames, total_size)
 
 
 def list_files_on_marine_data_lake_s3(
     path: str,
     files_already_found: list[tuple[str, int]] = [],
 ) -> list[tuple[str, int]]:
     # In order to list S3 native files, we are using CDN functionnalities using the following endpoint_url and path  # noqa
@@ -155,15 +146,15 @@
                     file.size,
                 )
             ]
         )
     return files_already_found
 
 
-def download_files(
+def _download_files(
     tuple_s3native_filename: Tuple[str, list[str], list[str]],
 ) -> str:
     def _s3native_file_download(
         endpoint_url: str, file_in: str, file_out: str
     ) -> str:
         """
         Download ONE file and return a string of the result
@@ -196,21 +187,18 @@
 
 
 # /////////////////////////////
 # --- Tools
 # /////////////////////////////
 
 
-def parse_s3native_dataset_url(data_paths: list[str]) -> dict:
-    path_dict: dict[str, list[str]] = {}
-    for data_path in data_paths:
-        endpoint_url, path = data_path.split("/mdl-native/", maxsplit=1)
-        path = "s3://mdl-native/" + path
-        path_dict.setdefault(endpoint_url, []).append(path)
-    return path_dict
+def parse_s3native_dataset_url(data_path: str) -> Tuple[str, str]:
+    endpoint_url, path = data_path.split("/mdl-native/", maxsplit=1)
+    path = "s3://mdl-native/" + path
+    return (endpoint_url, path)
 
 
 def create_filenames_out(
     filenames_in: list[str],
     overwrite: bool,
     output_directory: str = "",
     no_directories=False,
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/download_zarr.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/download_zarr.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     dataset_url: str,
     output_directory: str,
     output_filename: str,
     variables: Optional[list[str]],
     force_download: bool = False,
     overwrite: bool = False,
 ):
-
     dataset = xr.open_zarr(dataset_url)
     dataset = subset(
         dataset, variables, geographical_subset, temporal_subset, depth_range
     )
     dataset = dataset.chunk(chunks="auto")
 
     output_path = path.join(output_directory, output_filename)
@@ -97,15 +96,14 @@
 
 
 def download_zarr(
     username: str,
     password: str,
     subset_request: SubsetRequest,
 ):
-
     geographical_subset = (
         subset_request.minimal_latitude,
         subset_request.maximal_latitude,
         subset_request.minimal_longitude,
         subset_request.maximal_longitude,
     )
     temporal_subset = (
```

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/download_functions/subset_xarray.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/download_functions/subset_xarray.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/logging_conf.json` & `copernicus_marine_client-0.8.5/copernicus_marine_client/logging_conf.json`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/copernicus_marine_client/utils.py` & `copernicus_marine_client-0.8.5/copernicus_marine_client/utils.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.8.4/pyproject.toml` & `copernicus_marine_client-0.8.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.8.4"
+version = "0.8.5"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `copernicus_marine_client-0.8.4/setup.py` & `copernicus_marine_client-0.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.8.4',
+    'version': '0.8.5',
     'description': '',
     'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\n\nRetrieve information about all products as JSON:\n\n```txt\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```txt\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n```\n\n### Command *login*\n\nCreate the configuration files for access to the copernicus marine service:\n\'.dodsrc\', \'.netrc\', \'.motuclient-python.ini\'.\nThe directory to store these configuration files can be modified by the user using the "config-file-directory" option\nbut beware as it should also be passed to the *subset* and *native* command afterwards.\nBy default, if the configuration files already exist, the user is asked for confirmation to overwrite them.\n\nExample:\n\'\'\'\n> copernicus marine login\n< Username :\n< Password :\n> INFO     - root - Configuration files stored in ${HOME}\\.copernicus_marine_client\n\'\'\'\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```txt\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Username:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.{nc/zarr} if not specified otherwise (through -o/--output-directory and -f/--output-filename options). If the output-filename argument ends with \'.nc\' suffix, the file will be downloaded as a netCDF file.\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n\n```txt\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Username:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to proceed with download? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nOption `--filter TEXT` allows to specify a Unix shell-style wildcard pattern (see [fnmatch — Unix filename pattern matching](https://docs.python.org/3/library/fnmatch.html)) and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n\nOption `--regex TEXT` allows to specify a regular expression and select specific files. It work with both `--dataset-id` and `--dataset-url` options.\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m --regex ".*2022(08|09|10).nc"\nPassword:\nYou requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\n\nTotal size of the download: 9.82 MB\n\n\nDo you want to proceed with download? [y/N]:\n```\n\n### The overwrite option\n\nBoth `native` and `subset` commands provide an `--overwrite-ouput-data` option.\nWhen not provided (default behavior), once the download has been accepted (or if the `--force-download` option was provided), if the file already exists on destination, then a new one with a unique index will be created.\nOn the other hand, if the `--overwrite-ouput-data` option is provided and the file already exists, then it\'ll be overwritten.\n\n### The `--help` argument\n\nIn any case, please remember that you can call the `--help` argument on any CLI option. This may save you some time or find what you need.\n\n## Python functions\n\nThe library also provide python functions to help with catalogue\nbrowsing and datasets download in scripts.\n\n### Basic example\n\nIn this example 4 steps are performed:\n  1- Fetch the catalogue to select a dataset\n  2- Construct a SubsetRequest for this dataset\n  3- Download the subset as a zarr store\n  4- Open the subset as an xarray dataset\n\n```python\nimport copernicus_marine_client as cmc\n\n# Step 1: Fetch catalogue and parse information on dataset\ncatalogue = cmc.fetch_catalogue()\ndataset_id = "cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m"\nassert dataset_id in cmc.get_all_dataset_ids()\ndataset = catalogue.filter([dataset_id]).products[0].datasets[0]\n# Object "dataset" can be used to display all the metadata necessary to build a SubsetRequest\nvariable = [\n    variable for variable in dataset.variables if variable.short_name in ["zooc"]\n][0]\ncoordinates = {\n    coordinate.coordinates_id: (coordinate.minimum_value, coordinate.maximum_value)\n    for coordinate in variable.coordinates\n}\n\n# Step 2: Construct the request based on parsed information\nsubset_request = cmc.SubsetRequest(\n    dataset_id="cmems_mod_ibi_bgc_anfc_0.027deg-3D_P1D-m",\n    start_datetime="2023-04-20",\n    end_datetime="2023-04-21",\n    minimal_latitude=30.0,\n    maximal_latitude=30.1,\n    minimal_longitude=0.1,\n    maximal_longitude=0.2,\n    minimal_depth=100,\n    maximal_depth=1000,\n    variables=["zooc"],\n    force_protocol="zarr-map",\n    output_directory="data_folder",\n    output_filename="datastore.zarr",\n    force_download=True,\n)\n\n# Step 3: Download the subset based on request content\nfilename = cmc.download_subset(\n    login="FAKE_LOGIN", password="FAKE_PASSWORD", subset_request=subset_request\n)\n\n# Step 4: Open the downloaded subset as an xarray dataset\nsubset = cmc.open_dataset(filepath=filename, engine="zarr", out_type="xarray")\n```\n\n## Installation\n\nUsing pip, for example:\n\n```shell\npip install copernicus-marine-client\n```\n\n## Technical details\n\nThis module is organized around two capabilities:\n\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```python\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    force_download: Optional[bool] = None\n    force_protocol: Optional[str] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `copernicus_marine_client-0.8.4/PKG-INFO` & `copernicus_marine_client-0.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.8.4
+Version: 0.8.5
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

