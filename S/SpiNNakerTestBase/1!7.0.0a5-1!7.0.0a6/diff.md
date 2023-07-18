# Comparing `tmp/SpiNNakerTestBase-1!7.0.0a5.tar.gz` & `tmp/SpiNNakerTestBase-1!7.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpiNNakerTestBase-1!7.0.0a5.tar", last modified: Wed Apr 26 12:08:54 2023, max compression
+gzip compressed data, was "SpiNNakerTestBase-1!7.0.0a6.tar", last modified: Tue Jul 18 11:16:21 2023, max compression
```

## Comparing `SpiNNakerTestBase-1!7.0.0a5.tar` & `SpiNNakerTestBase-1!7.0.0a6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5054 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a5/CITATION.cff
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:37:33.000000 SpiNNakerTestBase-1!7.0.0a5/LICENSE
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      957 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a5/LICENSE_POLICY.md
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       56 2023-04-11 13:07:45.000000 SpiNNakerTestBase-1!7.0.0a5/MANIFEST.in
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1299 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      167 2023-04-26 12:06:32.000000 SpiNNakerTestBase-1!7.0.0a5/README.md
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:54.222593 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1299 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      630 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/SOURCES.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/dependency_links.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       92 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/requires.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       19 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/top_level.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:08:54.000000 SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/zip-safe
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:30:41.000000 SpiNNakerTestBase-1!7.0.0a5/pyproject.toml
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1380 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/setup.cfg
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1319 2023-04-13 14:09:56.000000 SpiNNakerTestBase-1!7.0.0a5/setup.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:54.226593 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      798 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      735 2023-04-26 12:06:32.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/_version.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3359 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/base_test_case.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     6113 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_script_builder.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     4903 2023-04-11 13:07:45.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_test_case.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2822 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/script_checker.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1033 2023-04-14 09:55:13.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_no_job_destroy.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1022 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_scripts_header
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:16:21.677578 SpiNNakerTestBase-1!7.0.0a6/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5054 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a6/CITATION.cff
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:37:33.000000 SpiNNakerTestBase-1!7.0.0a6/LICENSE
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      957 2023-03-10 13:09:34.000000 SpiNNakerTestBase-1!7.0.0a6/LICENSE_POLICY.md
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       56 2023-04-11 13:07:45.000000 SpiNNakerTestBase-1!7.0.0a6/MANIFEST.in
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1512 2023-07-18 11:16:21.677578 SpiNNakerTestBase-1!7.0.0a6/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      380 2023-07-18 11:16:18.000000 SpiNNakerTestBase-1!7.0.0a6/README.md
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:16:21.673578 SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1512 2023-07-18 11:16:21.000000 SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      630 2023-07-18 11:16:21.000000 SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/SOURCES.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:16:21.000000 SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/dependency_links.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       92 2023-07-18 11:16:21.000000 SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/requires.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       19 2023-07-18 11:16:21.000000 SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/top_level.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:16:21.000000 SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/zip-safe
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:30:41.000000 SpiNNakerTestBase-1!7.0.0a6/pyproject.toml
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1380 2023-07-18 11:16:21.677578 SpiNNakerTestBase-1!7.0.0a6/setup.cfg
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1319 2023-04-13 14:09:56.000000 SpiNNakerTestBase-1!7.0.0a6/setup.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:16:21.677578 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      798 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      734 2023-07-18 11:16:18.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/_version.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2318 2023-05-16 07:22:18.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/base_test_case.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     6113 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/root_script_builder.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5173 2023-06-19 09:58:26.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/root_test_case.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2822 2023-04-11 10:14:59.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/script_checker.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1033 2023-04-14 09:55:13.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/test_no_job_destroy.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1022 2023-03-08 14:17:55.000000 SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/test_scripts_header
```

### Comparing `SpiNNakerTestBase-1!7.0.0a5/CITATION.cff` & `SpiNNakerTestBase-1!7.0.0a6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/LICENSE` & `SpiNNakerTestBase-1!7.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/LICENSE_POLICY.md` & `SpiNNakerTestBase-1!7.0.0a6/LICENSE_POLICY.md`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/SpiNNakerTestBase.egg-info/SOURCES.txt` & `SpiNNakerTestBase-1!7.0.0a6/SpiNNakerTestBase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/pyproject.toml` & `SpiNNakerTestBase-1!7.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/setup.cfg` & `SpiNNakerTestBase-1!7.0.0a6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 [options]
 python_requires = >=3.7, <4
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
-	SpiNNFrontEndCommon == 1!7.0.0-a5
+	SpiNNFrontEndCommon == 1!7.0.0-a6
 	matplotlib
 
 [options.packages.find]
 include = 
 	spinnaker_testbase
 	spinnaker_testbase.*
```

### Comparing `SpiNNakerTestBase-1!7.0.0a5/setup.py` & `SpiNNakerTestBase-1!7.0.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/__init__.py` & `SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/__init__.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/_version.py` & `SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1!7.0.0-a5"
-__version_month__ = "April"
+__version__ = "1!7.0.0-a6"
+__version_month__ = "July"
 __version_year__ = "2023"
-__version_day__ = "17"
+__version_day__ = "18"
 __version_name__ = "Revisionist"
```

### Comparing `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_script_builder.py` & `SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/root_script_builder.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/root_test_case.py` & `SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/root_test_case.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 # limitations under the License.
 
 import os
 import sys
 import time
 import unittest
 from unittest import SkipTest
+from spinn_utilities.exceptions import NotSetupException
 from spinnman.exceptions import SpinnmanException
 from spinn_utilities.config_holder import (
     get_config_bool, get_config_str, has_config_option)
 from pacman.exceptions import PacmanPartitionException, PacmanValueError
 from spalloc_client.job import JobDestroyedError
+from spinn_front_end_common.data import FecDataView
 
 if os.environ.get('CONTINUOUS_INTEGRATION', 'false').lower() == 'true':
     max_tries = 3
 else:
     max_tries = 1
 
 
@@ -63,24 +65,29 @@
         test_base_directory = os.path.dirname(__file__)
         test_dir = os.path.dirname(test_base_directory)
         return os.path.join(test_dir, "ErrorFile.txt")
 
     def report(self, message, file_name):
         if not message.endswith("\n"):
             message += "\n"
-        test_base_directory = os.path.dirname(__file__)
-        test_dir = os.path.dirname(test_base_directory)
-        report_dir = os.path.join(test_dir, "global_reports")
-        if not os.path.exists(report_dir):
+        global_reports = os.environ.get("GLOBAL_REPORTS", None)
+        if not global_reports:
+            try:
+                global_reports = FecDataView.get_timestamp_dir_path()
+            except NotSetupException:
+                # This may happen if you are running none script fiels locally
+                return
+
+        if not os.path.exists(global_reports):
             # It might now exist if run in parallel
             try:
-                os.makedirs(report_dir)
+                os.makedirs(global_reports)
             except Exception:  # pylint: disable=broad-except
                 pass
-        report_path = os.path.join(report_dir, file_name)
+        report_path = os.path.join(global_reports, file_name)
         with open(report_path, "a", encoding="utf-8") as report_file:
             report_file.write(message)
 
     def runsafe(self, method, retry_delay=3.0, skip_exceptions=None):
         """
         Will run the method possibly a few times
```

### Comparing `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/script_checker.py` & `SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/script_checker.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_no_job_destroy.py` & `SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/test_no_job_destroy.py`

 * *Files identical despite different names*

### Comparing `SpiNNakerTestBase-1!7.0.0a5/spinnaker_testbase/test_scripts_header` & `SpiNNakerTestBase-1!7.0.0a6/spinnaker_testbase/test_scripts_header`

 * *Files identical despite different names*

