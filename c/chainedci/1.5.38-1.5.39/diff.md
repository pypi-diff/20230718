# Comparing `tmp/chainedci-1.5.38.tar.gz` & `tmp/chainedci-1.5.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainedci-1.5.38.tar", last modified: Mon Jul 10 19:16:19 2023, max compression
+gzip compressed data, was "chainedci-1.5.39.tar", last modified: Tue Jul 18 04:12:03 2023, max compression
```

## Comparing `chainedci-1.5.38.tar` & `chainedci-1.5.39.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:16:19.033878 chainedci-1.5.38/
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-10 19:16:01.000000 chainedci-1.5.38/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      923 2023-07-10 19:16:19.033878 chainedci-1.5.38/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-10 19:16:01.000000 chainedci-1.5.38/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:16:19.030878 chainedci-1.5.38/chainedci/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11472 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/artifact.py
--rw-rw-rw-   0 root         (0) root         (0)     9356 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/artifact_src.py
--rwxrwxrwx   0 root         (0) root         (0)      131 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/chainedci
--rw-rw-rw-   0 root         (0) root         (0)     6338 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     6819 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3663 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/default_chainedci.yml
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/env_vars.py
--rw-rw-rw-   0 root         (0) root         (0)     2924 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/http_adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/init_project.py
--rw-rw-rw-   0 root         (0) root         (0)     4174 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/log.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/options.py
--rw-rw-rw-   0 root         (0) root         (0)     3888 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/parser.py
--rw-rw-rw-   0 root         (0) root         (0)    10532 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     4890 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:16:19.032878 chainedci-1.5.38/chainedci/static/
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/static/inventory
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/static/projectA.yml
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/static/projectA_config1.yml
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/static/projectA_config2.yml
--rw-rw-rw-   0 root         (0) root         (0)    15020 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:16:19.032878 chainedci-1.5.38/chainedci/templates/
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/templates/all.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     3974 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/templates/main.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/templates/scenario.yml.tpl
--rw-rw-rw-   0 root         (0) root         (0)     2782 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/tools.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-10 19:16:01.000000 chainedci-1.5.38/chainedci/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:16:19.031878 chainedci-1.5.38/chainedci.egg-info/
--rw-r--r--   0 root         (0) root         (0)      923 2023-07-10 19:16:19.000000 chainedci-1.5.38/chainedci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      924 2023-07-10 19:16:19.000000 chainedci-1.5.38/chainedci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:16:19.000000 chainedci-1.5.38/chainedci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 19:16:19.000000 chainedci-1.5.38/chainedci.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       99 2023-07-10 19:16:19.000000 chainedci-1.5.38/chainedci.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-10 19:16:19.000000 chainedci-1.5.38/chainedci.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-10 19:16:19.033878 chainedci-1.5.38/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-07-10 19:16:01.000000 chainedci-1.5.38/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 19:16:19.033878 chainedci-1.5.38/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-10 19:16:01.000000 chainedci-1.5.38/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2023-07-10 19:16:01.000000 chainedci-1.5.38/tests/tests_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:12:03.813439 chainedci-1.5.39/
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-07-18 04:11:46.000000 chainedci-1.5.39/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      923 2023-07-18 04:12:03.813439 chainedci-1.5.39/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-18 04:11:46.000000 chainedci-1.5.39/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:12:03.810439 chainedci-1.5.39/chainedci/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11472 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/artifact.py
+-rw-rw-rw-   0 root         (0) root         (0)     9356 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/artifact_src.py
+-rwxrwxrwx   0 root         (0) root         (0)      131 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/chainedci
+-rw-rw-rw-   0 root         (0) root         (0)     6338 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     6819 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3663 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/default_chainedci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3926 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/env_vars.py
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/http_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/init_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     4174 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     3888 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    10532 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     4890 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:12:03.812439 chainedci-1.5.39/chainedci/static/
+-rw-rw-rw-   0 root         (0) root         (0)        8 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/static/inventory
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/static/projectA.yml
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/static/projectA_config1.yml
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/static/projectA_config2.yml
+-rw-rw-rw-   0 root         (0) root         (0)    15020 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:12:03.812439 chainedci-1.5.39/chainedci/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/templates/all.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     3974 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/templates/main.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/templates/scenario.yml.tpl
+-rw-rw-rw-   0 root         (0) root         (0)     2782 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-18 04:11:46.000000 chainedci-1.5.39/chainedci/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:12:03.811439 chainedci-1.5.39/chainedci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      923 2023-07-18 04:12:03.000000 chainedci-1.5.39/chainedci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      924 2023-07-18 04:12:03.000000 chainedci-1.5.39/chainedci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 04:12:03.000000 chainedci-1.5.39/chainedci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 04:12:03.000000 chainedci-1.5.39/chainedci.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-18 04:12:03.000000 chainedci-1.5.39/chainedci.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-18 04:12:03.000000 chainedci-1.5.39/chainedci.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-18 04:12:03.813439 chainedci-1.5.39/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-07-18 04:11:46.000000 chainedci-1.5.39/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 04:12:03.812439 chainedci-1.5.39/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 04:11:46.000000 chainedci-1.5.39/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-07-18 04:11:46.000000 chainedci-1.5.39/tests/tests_lib.py
```

### Comparing `chainedci-1.5.38/PKG-INFO` & `chainedci-1.5.39/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.38
+Version: 1.5.39
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.38/README.md` & `chainedci-1.5.39/README.md`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/artifact.py` & `chainedci-1.5.39/chainedci/artifact.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/artifact_src.py` & `chainedci-1.5.39/chainedci/artifact_src.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/cli.py` & `chainedci-1.5.39/chainedci/cli.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/config.py` & `chainedci-1.5.39/chainedci/config.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/default_chainedci.yml` & `chainedci-1.5.39/chainedci/default_chainedci.yml`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/env_vars.py` & `chainedci-1.5.39/chainedci/env_vars.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/http_adapter.py` & `chainedci-1.5.39/chainedci/http_adapter.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/init_project.py` & `chainedci-1.5.39/chainedci/init_project.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/inventory.py` & `chainedci-1.5.39/chainedci/inventory.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/log.py` & `chainedci-1.5.39/chainedci/log.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/options.py` & `chainedci-1.5.39/chainedci/options.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/parser.py` & `chainedci-1.5.39/chainedci/parser.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/pipeline.py` & `chainedci-1.5.39/chainedci/pipeline.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/scenario.py` & `chainedci-1.5.39/chainedci/scenario.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/step.py` & `chainedci-1.5.39/chainedci/step.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/templates/all.yml.tpl` & `chainedci-1.5.39/chainedci/templates/all.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/templates/main.yml.tpl` & `chainedci-1.5.39/chainedci/templates/main.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/templates/scenario.yml.tpl` & `chainedci-1.5.39/chainedci/templates/scenario.yml.tpl`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/tools.py` & `chainedci-1.5.39/chainedci/tools.py`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/chainedci/version.py` & `chainedci-1.5.39/chainedci/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 """Version module."""
 
-__version__ = "1.5.38"
+__version__ = "1.5.39"
```

### Comparing `chainedci-1.5.38/chainedci.egg-info/PKG-INFO` & `chainedci-1.5.39/chainedci.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainedci
-Version: 1.5.38
+Version: 1.5.39
 Summary: Chaine Gitlab CI pipelines
 Home-page: https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci
 Author: Orange OpenSource
 License: Apache 2.0
 Description-Content-Type: text/markdown
 
 # Chained-ci-py
```

### Comparing `chainedci-1.5.38/chainedci.egg-info/SOURCES.txt` & `chainedci-1.5.39/chainedci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainedci-1.5.38/setup.py` & `chainedci-1.5.39/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 def readme():
     """Set Readme from file."""
     with open('README.md', encoding="utf-8") as f:
         return f.read()
 
 
 setup(name='chainedci',
-      version='1.5.38',
+      version='1.5.39',
       description='Chaine Gitlab CI pipelines',
       long_description=readme(),
       long_description_content_type='text/markdown',
       url='https://gitlab.com/Orange-OpenSource/lfn/ci_cd/chained-ci',
       author='Orange OpenSource',
       license='Apache 2.0',
       packages=find_packages(),
       py_modules=[splitext(basename(path))[0] for path in glob('*.py')],
       include_package_data=True,
       scripts=["chainedci/chainedci"],
       install_requires=[
-          "ansible-core==2.15.1",
+          "ansible-core==2.15.2",
           "GitPython==3.1.32",
           "Jinja2==3.1.2",
           "requests==2.31.0",
           "schema==0.7.5",
           "urllib3 ==2.0.3"
       ],
       setup_requires=["pytest-runner"],
```

### Comparing `chainedci-1.5.38/tests/tests_lib.py` & `chainedci-1.5.39/tests/tests_lib.py`

 * *Files identical despite different names*

