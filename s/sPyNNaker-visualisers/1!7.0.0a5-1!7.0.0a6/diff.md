# Comparing `tmp/sPyNNaker_visualisers-1!7.0.0a5.tar.gz` & `tmp/sPyNNaker_visualisers-1!7.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sPyNNaker_visualisers-1!7.0.0a5.tar", last modified: Wed Apr 26 12:09:27 2023, max compression
+gzip compressed data, was "sPyNNaker_visualisers-1!7.0.0a6.tar", last modified: Tue Jul 18 11:17:15 2023, max compression
```

## Comparing `sPyNNaker_visualisers-1!7.0.0a5.tar` & `sPyNNaker_visualisers-1!7.0.0a6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:09:27.502040 sPyNNaker_visualisers-1!7.0.0a5/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5109 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a5/CITATION.cff
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:39:08.000000 sPyNNaker_visualisers-1!7.0.0a5/LICENSE
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      979 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a5/LICENSE_POLICY.md
--rw-r--r--   0 brenninc  (1000) brenninc  (1000)       63 2019-06-11 14:37:19.000000 sPyNNaker_visualisers-1!7.0.0a5/MANIFEST.in
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1361 2023-04-26 12:09:27.502040 sPyNNaker_visualisers-1!7.0.0a5/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      197 2023-04-26 12:06:27.000000 sPyNNaker_visualisers-1!7.0.0a5/README.md
--rw-r--r--   0 brenninc  (1000) brenninc  (1000)       90 2019-06-11 14:37:19.000000 sPyNNaker_visualisers-1!7.0.0a5/pypi_to_import
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:28:49.000000 sPyNNaker_visualisers-1!7.0.0a5/pyproject.toml
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:09:27.502040 sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1361 2023-04-26 12:09:27.000000 sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/PKG-INFO
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      733 2023-04-26 12:09:27.000000 sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/SOURCES.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:09:27.000000 sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/dependency_links.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       63 2023-04-26 12:09:27.000000 sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/requires.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       22 2023-04-26 12:09:27.000000 sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/top_level.txt
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-04-26 12:09:27.000000 sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/zip-safe
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1255 2023-04-26 12:09:27.502040 sPyNNaker_visualisers-1!7.0.0a5/setup.cfg
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1336 2023-04-11 13:16:45.000000 sPyNNaker_visualisers-1!7.0.0a5/setup.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:09:27.502040 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      866 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1052 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/_bigsurhack.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      735 2023-04-26 12:06:27.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/_version.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    13431 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/glut_framework.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3936 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/opengl_support.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:09:27.502040 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/raytrace/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      597 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/raytrace/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     7839 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/raytrace/drawer.py
-drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-04-26 12:09:27.502040 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/sudoku/
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      597 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/sudoku/__init__.py
--rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    15185 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/sudoku/sudoku_visualiser.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:17:15.092754 sPyNNaker_visualisers-1!7.0.0a6/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     5109 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a6/CITATION.cff
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    11360 2023-04-17 09:39:08.000000 sPyNNaker_visualisers-1!7.0.0a6/LICENSE
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      979 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a6/LICENSE_POLICY.md
+-rw-r--r--   0 brenninc  (1000) brenninc  (1000)       63 2019-06-11 14:37:19.000000 sPyNNaker_visualisers-1!7.0.0a6/MANIFEST.in
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1361 2023-07-18 11:17:15.092754 sPyNNaker_visualisers-1!7.0.0a6/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      197 2023-07-18 11:17:11.000000 sPyNNaker_visualisers-1!7.0.0a6/README.md
+-rw-r--r--   0 brenninc  (1000) brenninc  (1000)       90 2019-06-11 14:37:19.000000 sPyNNaker_visualisers-1!7.0.0a6/pypi_to_import
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      678 2023-04-18 10:28:49.000000 sPyNNaker_visualisers-1!7.0.0a6/pyproject.toml
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:17:15.088754 sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1361 2023-07-18 11:17:15.000000 sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/PKG-INFO
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      733 2023-07-18 11:17:15.000000 sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/SOURCES.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:17:15.000000 sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/dependency_links.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       63 2023-07-18 11:17:15.000000 sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/requires.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)       22 2023-07-18 11:17:15.000000 sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/top_level.txt
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)        1 2023-07-18 11:17:14.000000 sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/zip-safe
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1255 2023-07-18 11:17:15.092754 sPyNNaker_visualisers-1!7.0.0a6/setup.cfg
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1336 2023-04-11 13:16:45.000000 sPyNNaker_visualisers-1!7.0.0a6/setup.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:17:15.092754 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      866 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     1052 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/_bigsurhack.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      734 2023-07-18 11:17:11.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/_version.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    13431 2023-03-10 13:09:30.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/glut_framework.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     3936 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/opengl_support.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:17:15.092754 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/raytrace/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      597 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/raytrace/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)     7839 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/raytrace/drawer.py
+drwxrwxr-x   0 brenninc  (1000) brenninc  (1000)        0 2023-07-18 11:17:15.092754 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/sudoku/
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)      597 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/sudoku/__init__.py
+-rw-rw-r--   0 brenninc  (1000) brenninc  (1000)    15185 2023-03-08 14:17:47.000000 sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/sudoku/sudoku_visualiser.py
```

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/CITATION.cff` & `sPyNNaker_visualisers-1!7.0.0a6/CITATION.cff`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/LICENSE` & `sPyNNaker_visualisers-1!7.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/LICENSE_POLICY.md` & `sPyNNaker_visualisers-1!7.0.0a6/LICENSE_POLICY.md`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/PKG-INFO` & `sPyNNaker_visualisers-1!7.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sPyNNaker_visualisers
-Version: 1!7.0.0a5
+Version: 1!7.0.0a6
 Summary: Visualisation clients for special sPyNNaker networks.
 Home-page: https://github.com/SpiNNakerManchester/sPyNNakerVisualisersn
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: Apache-2.0
 Keywords: spinnaker,visualiser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/pyproject.toml` & `sPyNNaker_visualisers-1!7.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/PKG-INFO` & `sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sPyNNaker-visualisers
-Version: 1!7.0.0a5
+Version: 1!7.0.0a6
 Summary: Visualisation clients for special sPyNNaker networks.
 Home-page: https://github.com/SpiNNakerManchester/sPyNNakerVisualisersn
 Maintainer: SpiNNakerTeam
 Maintainer-email: spinnakerusers@googlegroups.com
 License: Apache-2.0
 Keywords: spinnaker,visualiser
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/sPyNNaker_visualisers.egg-info/SOURCES.txt` & `sPyNNaker_visualisers-1!7.0.0a6/sPyNNaker_visualisers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/setup.cfg` & `sPyNNaker_visualisers-1!7.0.0a6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 [options]
 python_requires = >=3.7, <4
 packages = find:
 zip_safe = True
 include_package_data = True
 install_requires = 
 	PyOpenGL
-	SpiNNFrontEndCommon == 1!7.0.0-a5
+	SpiNNFrontEndCommon == 1!7.0.0-a6
 
 [options.extras_require]
 test = 
 	flake8
 	pylint
 
 [egg_info]
```

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/setup.py` & `sPyNNaker_visualisers-1!7.0.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/__init__.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/__init__.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/_bigsurhack.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/_bigsurhack.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/_version.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/_version.py`

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

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/glut_framework.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/glut_framework.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/opengl_support.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/opengl_support.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/raytrace/__init__.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/raytrace/__init__.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/raytrace/drawer.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/raytrace/drawer.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/sudoku/__init__.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/sudoku/__init__.py`

 * *Files identical despite different names*

### Comparing `sPyNNaker_visualisers-1!7.0.0a5/spynnaker_visualisers/sudoku/sudoku_visualiser.py` & `sPyNNaker_visualisers-1!7.0.0a6/spynnaker_visualisers/sudoku/sudoku_visualiser.py`

 * *Files identical despite different names*

