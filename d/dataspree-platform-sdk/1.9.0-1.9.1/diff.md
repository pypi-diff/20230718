# Comparing `tmp/dataspree-platform-sdk-1.9.0.tar.gz` & `tmp/dataspree-platform-sdk-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspree-platform-sdk-1.9.0.tar", last modified: Fri Oct 28 14:05:00 2022, max compression
+gzip compressed data, was "dataspree-platform-sdk-1.9.1.tar", last modified: Thu Dec  1 14:12:56 2022, max compression
```

## Comparing `dataspree-platform-sdk-1.9.0.tar` & `dataspree-platform-sdk-1.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-10-28 14:05:00.189891 dataspree-platform-sdk-1.9.0/
--rw-rw-rw-   0        0        0     9760 2022-04-29 09:52:06.000000 dataspree-platform-sdk-1.9.0/LICENSE
--rw-rw-rw-   0        0        0       26 2022-04-29 13:09:12.000000 dataspree-platform-sdk-1.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3353 2022-10-28 14:05:00.188884 dataspree-platform-sdk-1.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     2291 2022-10-28 14:04:51.000000 dataspree-platform-sdk-1.9.0/README.md
-drwxrwxrwx   0        0        0        0 2022-10-28 14:05:00.141891 dataspree-platform-sdk-1.9.0/dataspree/
-drwxrwxrwx   0        0        0        0 2022-10-28 14:05:00.160892 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/
--rw-rw-rw-   0        0        0      628 2022-10-28 14:04:51.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/__init__.py
--rw-rw-rw-   0        0        0     9651 2022-10-28 14:04:51.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/base_model.py
--rw-rw-rw-   0        0        0    12429 2022-07-28 08:08:10.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/cli.py
--rw-rw-rw-   0        0        0    80054 2022-10-28 14:04:51.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/client.py
--rw-rw-rw-   0        0        0    21021 2022-10-28 14:04:51.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/data_loader.py
-drwxrwxrwx   0        0        0        0 2022-10-28 14:05:00.167930 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/
--rw-rw-rw-   0        0        0      642 2022-04-29 11:46:44.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/__init__.py
--rw-rw-rw-   0        0        0     1401 2022-04-29 11:26:51.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/base_decoder.py
--rw-rw-rw-   0        0        0     4181 2022-05-20 09:48:17.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/opencv_decoder.py
--rw-rw-rw-   0        0        0     2019 2022-04-29 12:11:43.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/pcd_decoder.py
--rw-rw-rw-   0        0        0     6892 2022-07-04 15:21:06.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/serializer.py
--rw-rw-rw-   0        0        0      973 2022-04-29 09:52:06.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/http_token_authentication.py
--rw-rw-rw-   0        0        0     4888 2022-04-29 09:52:06.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/query.py
--rw-rw-rw-   0        0        0    33806 2022-07-06 13:49:32.000000 dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/worker.py
-drwxrwxrwx   0        0        0        0 2022-10-28 14:05:00.187887 dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/
--rw-rw-rw-   0        0        0     3353 2022-10-28 14:04:59.000000 dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2022-10-28 14:04:59.000000 dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-28 14:04:59.000000 dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2022-10-28 14:04:59.000000 dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      161 2022-10-28 14:04:59.000000 dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-10-28 14:04:59.000000 dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      130 2022-04-29 09:52:06.000000 dataspree-platform-sdk-1.9.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-10-28 14:05:00.189891 dataspree-platform-sdk-1.9.0/setup.cfg
--rw-rw-rw-   0        0        0     2408 2022-07-04 13:57:08.000000 dataspree-platform-sdk-1.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-01 14:12:56.650026 dataspree-platform-sdk-1.9.1/
+-rw-rw-rw-   0        0        0     9760 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2840 2022-12-01 14:12:56.649028 dataspree-platform-sdk-1.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2291 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/README.md
+drwxrwxrwx   0        0        0        0 2022-12-01 14:12:56.522315 dataspree-platform-sdk-1.9.1/dataspree/
+drwxrwxrwx   0        0        0        0 2022-12-01 14:12:56.576025 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/
+-rw-rw-rw-   0        0        0      628 2022-12-01 14:06:57.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/__init__.py
+-rw-rw-rw-   0        0        0     9837 2022-12-01 12:30:42.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/base_model.py
+-rw-rw-rw-   0        0        0    12429 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/cli.py
+-rw-rw-rw-   0        0        0    80054 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/client.py
+-rw-rw-rw-   0        0        0    21274 2022-12-01 13:43:06.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/data_loader.py
+drwxrwxrwx   0        0        0        0 2022-12-01 14:12:56.620025 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/
+-rw-rw-rw-   0        0        0      642 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/__init__.py
+-rw-rw-rw-   0        0        0     1401 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/base_decoder.py
+-rw-rw-rw-   0        0        0     4181 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/opencv_decoder.py
+-rw-rw-rw-   0        0        0     2019 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/pcd_decoder.py
+-rw-rw-rw-   0        0        0     6892 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/serializer.py
+-rw-rw-rw-   0        0        0      973 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/http_token_authentication.py
+-rw-rw-rw-   0        0        0     4888 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/query.py
+-rw-rw-rw-   0        0        0    33806 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/worker.py
+drwxrwxrwx   0        0        0        0 2022-12-01 14:12:56.648025 dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2840 2022-12-01 14:12:56.000000 dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2022-12-01 14:12:56.000000 dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-01 14:12:56.000000 dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2022-12-01 14:12:56.000000 dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      161 2022-12-01 14:12:56.000000 dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-12-01 14:12:56.000000 dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      130 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-12-01 14:12:56.650026 dataspree-platform-sdk-1.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     2408 2022-11-24 15:21:01.000000 dataspree-platform-sdk-1.9.1/setup.py
```

### Comparing `dataspree-platform-sdk-1.9.0/LICENSE` & `dataspree-platform-sdk-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/PKG-INFO` & `dataspree-platform-sdk-1.9.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,63 @@
-Metadata-Version: 2.1
-Name: dataspree-platform-sdk
-Version: 1.9.0
-Summary: Python SDK Data Spree AI Platform
-Home-page: https://data-spree.com/ai
-Author: Data Spree GmbH
-Author-email: info@data-spree.com
-License: Apache-2.0
-Description: # Data Spree AI Platform SDK
-        The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
-        custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
-        * Data Spree
-        * KITTI
-        * COCO
-        
-        Furthermore, it is possible to export datasets from the platform.
-        
-        ## Usage
-        
-        ### General Usage
-        ```
-        Usage: ds [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          --help  Show this message and exit.
-        
-        Commands:
-          export
-          import
-        ```
-        
-        ### Dataset Import
-        ```
-        Usage: ds import [OPTIONS]
-        
-        Options:
-          --format [dataspree|kitti|coco]  Dataset format to import
-          --dataset_name TEXT         Name of the newly created dataset.
-          --dataset_id INTEGER        ID of the dataset to which new items should be
-                                      imported. If set to '-1', a new dataset will be
-                                      created
-          --images PATH               Directory containing the images to import.
-                                      [required]
-          --annotations PATH          Directory or file containing the annotations to
-                                      import.  [required]
-          --http_retries INTEGER      Number of HTTP retries.  [default: 10]
-          --username TEXT             Username for data spree vision platform.
-          --password TEXT             Password for data spree vision platform.
-          --url TEXT                  URL to the API of the platform.
-          --help                      Show this message and exit.
-        ```
-        
-        ### Dataset Export
-        ```
-        Usage: ds export [OPTIONS]
-        
-        Options:
-          -o, --output_dir DIRECTORY   Output directory.  [required]
-          -i, --id INTEGER             ID of the dataset to download.
-          -n, --n_items INTEGER        Number of items to download. Download all
-                                       items: '-1'  [default: -1]
-          --http_retries INTEGER       Number of HTTP retries.  [default: 10]
-          --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
-          --username TEXT              Username for data spree vision platform.
-          --password TEXT              Password for data spree vision platform.
-          --url TEXT                   URL to the API of the platform.
-          --help                       Show this message and exit.
-        ```
-        
-        ## License
-        Apache License 2.0
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: kitti
-Provides-Extra: worker
-Provides-Extra: build
+# Data Spree AI Platform SDK
+The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
+custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
+* Data Spree
+* KITTI
+* COCO
+
+Furthermore, it is possible to export datasets from the platform.
+
+## Usage
+
+### General Usage
+```
+Usage: ds [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  export
+  import
+```
+
+### Dataset Import
+```
+Usage: ds import [OPTIONS]
+
+Options:
+  --format [dataspree|kitti|coco]  Dataset format to import
+  --dataset_name TEXT         Name of the newly created dataset.
+  --dataset_id INTEGER        ID of the dataset to which new items should be
+                              imported. If set to '-1', a new dataset will be
+                              created
+  --images PATH               Directory containing the images to import.
+                              [required]
+  --annotations PATH          Directory or file containing the annotations to
+                              import.  [required]
+  --http_retries INTEGER      Number of HTTP retries.  [default: 10]
+  --username TEXT             Username for data spree vision platform.
+  --password TEXT             Password for data spree vision platform.
+  --url TEXT                  URL to the API of the platform.
+  --help                      Show this message and exit.
+```
+
+### Dataset Export
+```
+Usage: ds export [OPTIONS]
+
+Options:
+  -o, --output_dir DIRECTORY   Output directory.  [required]
+  -i, --id INTEGER             ID of the dataset to download.
+  -n, --n_items INTEGER        Number of items to download. Download all
+                               items: '-1'  [default: -1]
+  --http_retries INTEGER       Number of HTTP retries.  [default: 10]
+  --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
+  --username TEXT              Username for data spree vision platform.
+  --password TEXT              Password for data spree vision platform.
+  --url TEXT                   URL to the API of the platform.
+  --help                       Show this message and exit.
+```
+
+## License
+Apache License 2.0
```

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/__init__.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = '1.9.0'
+__version__ = '1.9.1'
```

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/base_model.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/base_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,20 +126,23 @@
             return
 
         # load model information
         model_id = job.get('model').get('id')
         platform_model = client.get_model(model_id)
         model_class_labels = client.get_model_class_labels(model_id)
         target_class_labels = []
+        target_class_label_ids = []
         for c in model_class_labels:
             target_class_label = c['target_class_label']
             if target_class_label is None:
                 # old class labels have no target (they are the target/there is no remapping)
                 target_class_label = c['class_label']
-            target_class_labels.append(target_class_label)
+            if target_class_label['id'] not in target_class_label_ids:
+                target_class_label_ids.append(target_class_label['id'])
+                target_class_labels.append(target_class_label)
 
         # "class_labels" contains the original and the target class labels
         platform_model['class_labels'] = model_class_labels
 
         # the "target_class_labels" contain only those labels that are predicted by the model
         platform_model['target_class_labels'] = target_class_labels
```

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/cli.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/cli.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/client.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/client.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/data_loader.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,27 @@
 
         self._items = {}
 
         # load class label ids and names that are used within this model
         self._model_class_labels: List[Dict] = client.get_model_class_labels(network_model['id'])
         self._mapped_class_labels: Dict[int, List[int]] = dict()
         self._target_class_labels: List[Dict] = []
+        target_class_label_ids = []
         for c in self._model_class_labels:
             target_class_label = c['target_class_label']
             if target_class_label is None:
                 # old class labels have no target (they are the target/there is no remapping)
                 target_class_label = c['class_label']
-            self._target_class_labels.append(target_class_label)
+            if target_class_label['id'] not in target_class_label_ids:
+                target_class_label_ids.append(target_class_label['id'])
+                self._target_class_labels.append(target_class_label)
             class_label = c['class_label']
             mapped_labels = self._mapped_class_labels.setdefault(class_label['id'], [])
-            mapped_labels.append(target_class_label['id'])
+            if target_class_label['id'] not in mapped_labels:
+                mapped_labels.append(target_class_label['id'])
 
         # get all categories and aggregate the respective subset IDs
         self._subsets_ids_by_category = {}
         for entry in network_model['data_subsets']:
             if entry['category'] not in self._subsets_ids_by_category.keys():
                 self._subsets_ids_by_category[entry['category']] = []
             if entry['data_subset']['id'] not in self._subsets_ids_by_category[entry['category']]:
```

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/__init__.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/base_decoder.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/base_decoder.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/opencv_decoder.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/opencv_decoder.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/pcd_decoder.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/pcd_decoder.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/decoder/serializer.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/decoder/serializer.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/http_token_authentication.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/http_token_authentication.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/query.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/query.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree/platform_sdk/worker.py` & `dataspree-platform-sdk-1.9.1/dataspree/platform_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/dataspree_platform_sdk.egg-info/SOURCES.txt` & `dataspree-platform-sdk-1.9.1/dataspree_platform_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataspree-platform-sdk-1.9.0/setup.py` & `dataspree-platform-sdk-1.9.1/setup.py`

 * *Files identical despite different names*

