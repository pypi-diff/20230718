# Comparing `tmp/spalloc_server-1!7.0.0a5.tar.gz` & `tmp/spalloc_server-1!7.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spalloc_server-1!7.0.0a5.tar", last modified: Wed Apr 26 12:08:27 2023, max compression
+gzip compressed data, was "spalloc_server-1!7.0.0a6.tar", last modified: Tue Jul 18 11:15:50 2023, max compression
```

## Comparing `spalloc_server-1!7.0.0a5.tar` & `spalloc_server-1!7.0.0a6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:27.659034 spalloc_server-1!7.0.0a5/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5082 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a5/CITATION.cff
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:36:59.000000 spalloc_server-1!7.0.0a5/LICENSE
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      967 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a5/LICENSE_POLICY.md
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       74 2023-04-11 11:02:16.000000 spalloc_server-1!7.0.0a5/MANIFEST.in
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2625 2023-04-26 12:08:27.659034 spalloc_server-1!7.0.0a5/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1406 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a5/README.rst
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:28:23.000000 spalloc_server-1!7.0.0a5/pyproject.toml
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1512 2023-04-26 12:08:27.659034 spalloc_server-1!7.0.0a5/setup.cfg
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1316 2023-04-11 11:05:20.000000 spalloc_server-1!7.0.0a5/setup.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:27.655034 spalloc_server-1!7.0.0a5/spalloc_server/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      660 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      735 2023-04-26 12:05:52.000000 spalloc_server-1!7.0.0a5/spalloc_server/_version.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    45607 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/allocator.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5891 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/area_to_rect.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    12605 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/async_bmp_controller.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    22151 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/configuration.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5164 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/configuration_reloader.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    58141 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/controller.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     9919 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/coordinates.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    21347 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/job_queue.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5478 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/links.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    14536 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/pack_tree.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5178 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/polling_server_core.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    45502 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a5/spalloc_server/server.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:27.659034 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2625 2023-04-26 12:08:27.000000 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1098 2023-04-26 12:08:27.000000 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/SOURCES.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:08:27.000000 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/dependency_links.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      106 2023-04-26 12:08:27.000000 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/entry_points.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       65 2023-04-26 12:08:27.000000 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/requires.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       15 2023-04-26 12:08:27.000000 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/top_level.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:08:27.000000 spalloc_server-1!7.0.0a5/spalloc_server.egg-info/zip-safe
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:08:27.659034 spalloc_server-1!7.0.0a5/tests/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    33475 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_allocator.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5859 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_area_to_rect.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11980 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_async_bmp_controller.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    10633 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_configuration.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    44669 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_controller.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5331 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_coordinates.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1069 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_import_all.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    17782 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_job_queue.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3198 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_links.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    22346 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_pack_tree.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1251 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_polling_server_core.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    34764 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a5/tests/test_server.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:50.846054 spalloc_server-1!7.0.0a6/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5082 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a6/CITATION.cff
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:36:59.000000 spalloc_server-1!7.0.0a6/LICENSE
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      967 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a6/LICENSE_POLICY.md
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       74 2023-04-11 11:02:16.000000 spalloc_server-1!7.0.0a6/MANIFEST.in
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2625 2023-07-18 11:15:50.846054 spalloc_server-1!7.0.0a6/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1406 2023-03-10 13:05:58.000000 spalloc_server-1!7.0.0a6/README.rst
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:28:23.000000 spalloc_server-1!7.0.0a6/pyproject.toml
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1512 2023-07-18 11:15:50.846054 spalloc_server-1!7.0.0a6/setup.cfg
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1316 2023-04-11 11:05:20.000000 spalloc_server-1!7.0.0a6/setup.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:50.842054 spalloc_server-1!7.0.0a6/spalloc_server/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      660 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      734 2023-07-18 11:15:48.000000 spalloc_server-1!7.0.0a6/spalloc_server/_version.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    45607 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/allocator.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5891 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/area_to_rect.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    12605 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/async_bmp_controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    22151 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/configuration.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5164 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/configuration_reloader.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    58141 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     9919 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/coordinates.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    21347 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/job_queue.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5478 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/links.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    14536 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/pack_tree.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5178 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/polling_server_core.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    45502 2023-04-04 07:01:31.000000 spalloc_server-1!7.0.0a6/spalloc_server/server.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:50.842054 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     2625 2023-07-18 11:15:50.000000 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1098 2023-07-18 11:15:50.000000 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/SOURCES.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:15:50.000000 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/dependency_links.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      106 2023-07-18 11:15:50.000000 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/entry_points.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       65 2023-07-18 11:15:50.000000 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/requires.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       15 2023-07-18 11:15:50.000000 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/top_level.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:15:50.000000 spalloc_server-1!7.0.0a6/spalloc_server.egg-info/zip-safe
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:15:50.846054 spalloc_server-1!7.0.0a6/tests/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    33475 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_allocator.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5859 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_area_to_rect.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11980 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_async_bmp_controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    10633 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_configuration.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    44669 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_controller.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5331 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_coordinates.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1069 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_import_all.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    17782 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_job_queue.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3198 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_links.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    22346 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_pack_tree.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1251 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_polling_server_core.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    34764 2023-03-08 14:14:30.000000 spalloc_server-1!7.0.0a6/tests/test_server.py
```

### Comparing `spalloc_server-1!7.0.0a5/CITATION.cff` & `spalloc_server-1!7.0.0a6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/LICENSE` & `spalloc_server-1!7.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/LICENSE_POLICY.md` & `spalloc_server-1!7.0.0a6/LICENSE_POLICY.md`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/PKG-INFO` & `spalloc_server-1!7.0.0a6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spalloc_server
-Version: 1!7.0.0a5
+Version: 1!7.0.0a6
 Summary: A tool for partitioning and allocating large SpiNNaker machines into smaller ones on demand.
 Home-page: https://github.com/SpiNNakerManchester/spalloc_server
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: Apache-2.0
 Keywords: spinnaker,allocation,packing management,supercomputer
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spalloc_server-1!7.0.0a5/README.rst` & `spalloc_server-1!7.0.0a6/README.rst`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/pyproject.toml` & `spalloc_server-1!7.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/setup.cfg` & `spalloc_server-1!7.0.0a6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 [options]
 python_requires = >=3.7, <4
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
 	pytz
-	SpiNNMan == 1!7.0.0-a5
+	SpiNNMan == 1!7.0.0-a6
 
 [options.packages.find]
 include = 
 	spalloc_server
 	spalloc_server.*
 
 [options.extras_require]
```

### Comparing `spalloc_server-1!7.0.0a5/setup.py` & `spalloc_server-1!7.0.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/__init__.py` & `spalloc_server-1!7.0.0a6/spalloc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/_version.py` & `spalloc_server-1!7.0.0a6/spalloc_server/_version.py`

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

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/allocator.py` & `spalloc_server-1!7.0.0a6/spalloc_server/allocator.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/area_to_rect.py` & `spalloc_server-1!7.0.0a6/spalloc_server/area_to_rect.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/async_bmp_controller.py` & `spalloc_server-1!7.0.0a6/spalloc_server/async_bmp_controller.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/configuration.py` & `spalloc_server-1!7.0.0a6/spalloc_server/configuration.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/configuration_reloader.py` & `spalloc_server-1!7.0.0a6/spalloc_server/configuration_reloader.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/controller.py` & `spalloc_server-1!7.0.0a6/spalloc_server/controller.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/coordinates.py` & `spalloc_server-1!7.0.0a6/spalloc_server/coordinates.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/job_queue.py` & `spalloc_server-1!7.0.0a6/spalloc_server/job_queue.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/links.py` & `spalloc_server-1!7.0.0a6/spalloc_server/links.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/pack_tree.py` & `spalloc_server-1!7.0.0a6/spalloc_server/pack_tree.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/polling_server_core.py` & `spalloc_server-1!7.0.0a6/spalloc_server/polling_server_core.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server/server.py` & `spalloc_server-1!7.0.0a6/spalloc_server/server.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server.egg-info/PKG-INFO` & `spalloc_server-1!7.0.0a6/spalloc_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spalloc-server
-Version: 1!7.0.0a5
+Version: 1!7.0.0a6
 Summary: A tool for partitioning and allocating large SpiNNaker machines into smaller ones on demand.
 Home-page: https://github.com/SpiNNakerManchester/spalloc_server
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: Apache-2.0
 Keywords: spinnaker,allocation,packing management,supercomputer
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `spalloc_server-1!7.0.0a5/spalloc_server.egg-info/SOURCES.txt` & `spalloc_server-1!7.0.0a6/spalloc_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_allocator.py` & `spalloc_server-1!7.0.0a6/tests/test_allocator.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_area_to_rect.py` & `spalloc_server-1!7.0.0a6/tests/test_area_to_rect.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_async_bmp_controller.py` & `spalloc_server-1!7.0.0a6/tests/test_async_bmp_controller.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_configuration.py` & `spalloc_server-1!7.0.0a6/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_controller.py` & `spalloc_server-1!7.0.0a6/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_coordinates.py` & `spalloc_server-1!7.0.0a6/tests/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_import_all.py` & `spalloc_server-1!7.0.0a6/tests/test_import_all.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_job_queue.py` & `spalloc_server-1!7.0.0a6/tests/test_job_queue.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_links.py` & `spalloc_server-1!7.0.0a6/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_pack_tree.py` & `spalloc_server-1!7.0.0a6/tests/test_pack_tree.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_polling_server_core.py` & `spalloc_server-1!7.0.0a6/tests/test_polling_server_core.py`

 * *Files identical despite different names*

### Comparing `spalloc_server-1!7.0.0a5/tests/test_server.py` & `spalloc_server-1!7.0.0a6/tests/test_server.py`

 * *Files identical despite different names*

