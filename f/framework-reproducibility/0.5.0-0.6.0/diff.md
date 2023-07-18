# Comparing `tmp/framework-reproducibility-0.5.0.tar.gz` & `tmp/framework-reproducibility-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/framework-reproducibility-0.5.0.tar", last modified: Thu Jun 22 22:45:43 2023, max compression
+gzip compressed data, was "dist/framework-reproducibility-0.6.0.tar", last modified: Mon Jul 17 23:45:27 2023, max compression
```

## Comparing `framework-reproducibility-0.5.0.tar` & `framework-reproducibility-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2846 2023-04-27 19:27:49.000000 framework-reproducibility-0.5.0/setup.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/seeder/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2007 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/seed_gen.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2965 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/pyt.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3135 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/tf.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2960 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/seeder/paddle.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      777 2023-02-28 05:04:37.000000 framework-reproducibility-0.5.0/fwr13y/seeder/__init__.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      701 2023-06-22 22:44:48.000000 framework-reproducibility-0.5.0/fwr13y/version.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/d9m/
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2687 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_segment_sum.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3080 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2923 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_bias_add.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     2904 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/enable_determinism.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3260 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      955 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/__init__.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     3752 2023-02-27 20:42:41.000000 framework-reproducibility-0.5.0/fwr13y/d9m/utils.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      789 2023-04-27 19:27:49.000000 framework-reproducibility-0.5.0/fwr13y/d9m/__init__.py
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      823 2023-04-27 19:27:49.000000 framework-reproducibility-0.5.0/fwr13y/__init__.py
-drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/
--rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/PKG-INFO
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        7 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/top_level.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/dependency_links.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)      667 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/framework_reproducibility.egg-info/SOURCES.txt
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       67 2023-06-22 22:45:43.000000 framework-reproducibility-0.5.0/setup.cfg
--rw-rw-r--   0 duncan    (1000) duncan    (1000)       18 2023-02-28 05:04:37.000000 framework-reproducibility-0.5.0/MANIFEST.in
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2967 2023-07-17 23:45:20.000000 framework-reproducibility-0.6.0/setup.py
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/fwr13y/
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/fwr13y/seeder/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2007 2023-06-22 22:44:48.000000 framework-reproducibility-0.6.0/fwr13y/seeder/seed_gen.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2965 2023-06-22 22:44:48.000000 framework-reproducibility-0.6.0/fwr13y/seeder/pyt.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3135 2023-06-22 22:44:48.000000 framework-reproducibility-0.6.0/fwr13y/seeder/tf.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2960 2023-06-22 22:44:48.000000 framework-reproducibility-0.6.0/fwr13y/seeder/paddle.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      777 2023-02-28 05:04:37.000000 framework-reproducibility-0.6.0/fwr13y/seeder/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      701 2023-07-17 23:08:12.000000 framework-reproducibility-0.6.0/fwr13y/version.py
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/fwr13y/d9m/
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2687 2023-02-27 20:42:41.000000 framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch_segment_sum.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3080 2023-02-27 20:42:41.000000 framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2923 2023-02-27 20:42:41.000000 framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch_bias_add.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     2904 2023-02-27 20:42:41.000000 framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/enable_determinism.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3260 2023-02-27 20:42:41.000000 framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      955 2023-02-27 20:42:41.000000 framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     3752 2023-02-27 20:42:41.000000 framework-reproducibility-0.6.0/fwr13y/d9m/utils.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      789 2023-04-27 19:27:49.000000 framework-reproducibility-0.6.0/fwr13y/d9m/__init__.py
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      823 2023-04-27 19:27:49.000000 framework-reproducibility-0.6.0/fwr13y/__init__.py
+drwxrwxr-x   0 duncan    (1000) duncan    (1000)        0 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/framework_reproducibility.egg-info/
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)     1378 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/framework_reproducibility.egg-info/PKG-INFO
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)        7 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/framework_reproducibility.egg-info/top_level.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)        1 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/framework_reproducibility.egg-info/dependency_links.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)      667 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/framework_reproducibility.egg-info/SOURCES.txt
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       67 2023-07-17 23:45:27.000000 framework-reproducibility-0.6.0/setup.cfg
+-rw-rw-r--   0 duncan    (1000) duncan    (1000)       18 2023-02-28 05:04:37.000000 framework-reproducibility-0.6.0/MANIFEST.in
```

### Comparing `framework-reproducibility-0.5.0/PKG-INFO` & `framework-reproducibility-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framework-reproducibility
-Version: 0.5.0
+Version: 0.6.0
 Summary: Providing reproducibility in deep learning frameworks
 Home-page: https://github.com/NVIDIA/framework-reproducibility
 Author: NVIDIA
 Author-email: duncan@nvidia.com
 License: Apache 2.0
 Description: This package provides patches and tools related to determinism
         (bit-accurate, run-to-run reproducibility) in deep learning frameworks, with a
```

### Comparing `framework-reproducibility-0.5.0/setup.py` & `framework-reproducibility-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 # all the supported frameworks have not been installed. By temporarility
 # appending to sys.path, it's possible to just import from the version module.
 import sys
 sys.path.append(package_name)
 from version import __version__ as version
 sys.path.remove(package_name)
 
+packages = (
+    ['fwr13y'] + ['fwr13y.' +
+                  subpackage for subpackage in find_packages(where='fwr13y')])
+
 readme = os.path.join(os.path.dirname(os.path.realpath(__file__)),
                       "pypi_description.md")
 with open(readme, "r") as fp:
   long_description = fp.read()
 
 description = ("Providing reproducibility in deep learning frameworks")
 url = "https://github.com/NVIDIA/%s" % distribution_name
@@ -49,15 +53,15 @@
             "reproducibility pytorch seed seeder noise noise-reduction "
             "variance-reduction atomics ngc gpu-determinism deterministic-ops "
             "frameworks gpu-support d9m r13y fwr13y")
 
 setup(
   name                          = distribution_name,
   version                       = version,
-  packages                      = ['fwr13y'],
+  packages                      = packages,
   url                           = url,
   license                       = 'Apache 2.0',
   author                        = 'NVIDIA',
   author_email                  = 'duncan@nvidia.com',
   description                   = description,
   long_description              = long_description,
   long_description_content_type = 'text/markdown',
```

### Comparing `framework-reproducibility-0.5.0/fwr13y/seeder/seed_gen.py` & `framework-reproducibility-0.6.0/fwr13y/seeder/seed_gen.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/seeder/pyt.py` & `framework-reproducibility-0.6.0/fwr13y/seeder/pyt.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/seeder/tf.py` & `framework-reproducibility-0.6.0/fwr13y/seeder/tf.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/seeder/paddle.py` & `framework-reproducibility-0.6.0/fwr13y/seeder/paddle.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/seeder/__init__.py` & `framework-reproducibility-0.6.0/fwr13y/seeder/__init__.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/version.py` & `framework-reproducibility-0.6.0/fwr13y/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ========================================================================
 
-__version__ = "0.5.0"
+__version__ = "0.6.0"
```

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_segment_sum.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch_segment_sum.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch_unsorted_segment_sum.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch_bias_add.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch_bias_add.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/enable_determinism.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/enable_determinism.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/patch.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/patch.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/tensorflow/__init__.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/utils.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/utils.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/d9m/__init__.py` & `framework-reproducibility-0.6.0/fwr13y/d9m/__init__.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/fwr13y/__init__.py` & `framework-reproducibility-0.6.0/fwr13y/__init__.py`

 * *Files identical despite different names*

### Comparing `framework-reproducibility-0.5.0/framework_reproducibility.egg-info/PKG-INFO` & `framework-reproducibility-0.6.0/framework_reproducibility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framework-reproducibility
-Version: 0.5.0
+Version: 0.6.0
 Summary: Providing reproducibility in deep learning frameworks
 Home-page: https://github.com/NVIDIA/framework-reproducibility
 Author: NVIDIA
 Author-email: duncan@nvidia.com
 License: Apache 2.0
 Description: This package provides patches and tools related to determinism
         (bit-accurate, run-to-run reproducibility) in deep learning frameworks, with a
```

### Comparing `framework-reproducibility-0.5.0/framework_reproducibility.egg-info/SOURCES.txt` & `framework-reproducibility-0.6.0/framework_reproducibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

