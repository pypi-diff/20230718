# Comparing `tmp/neon-mana-utils-0.2.0.tar.gz` & `tmp/neon-mana-utils-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-mana-utils-0.2.0.tar", last modified: Tue Jun 27 18:27:42 2023, max compression
+gzip compressed data, was "neon-mana-utils-0.2.1a1.tar", last modified: Tue Jul 18 16:10:59 2023, max compression
```

## Comparing `neon-mana-utils-0.2.0.tar` & `neon-mana-utils-0.2.1a1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:27:42.086214 neon-mana-utils-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-27 18:27:42.086214 neon-mana-utils-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:27:42.086214 neon-mana-utils-0.2.0/neon_mana_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/bus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/core_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/skills.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/neon_mana_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 18:27:42.086214 neon-mana-utils-0.2.0/neon_mana_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-27 18:27:42.000000 neon-mana-utils-0.2.0/neon_mana_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-27 18:27:42.000000 neon-mana-utils-0.2.0/neon_mana_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 18:27:42.000000 neon-mana-utils-0.2.0/neon_mana_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-27 18:27:42.000000 neon-mana-utils-0.2.0/neon_mana_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-27 18:27:42.000000 neon-mana-utils-0.2.0/neon_mana_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 18:27:42.000000 neon-mana-utils-0.2.0/neon_mana_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 18:27:42.086214 neon-mana-utils-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-27 18:27:36.000000 neon-mana-utils-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:10:59.804478 neon-mana-utils-0.2.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-18 16:10:59.804478 neon-mana-utils-0.2.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:10:59.804478 neon-mana-utils-0.2.1a1/neon_mana_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/bus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/core_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/skills.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/neon_mana_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:10:59.804478 neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-18 16:10:59.000000 neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-18 16:10:59.000000 neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:10:59.000000 neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 16:10:59.000000 neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 16:10:59.000000 neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 16:10:59.000000 neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:10:59.804478 neon-mana-utils-0.2.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-18 16:10:56.000000 neon-mana-utils-0.2.1a1/setup.py
```

### Comparing `neon-mana-utils-0.2.0/LICENSE.md` & `neon-mana-utils-0.2.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/PKG-INFO` & `neon-mana-utils-0.2.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mana-utils
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: Message Application for Neon AI
 Home-page: https://github.com/neongeckocom/neon-mana-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-mana-utils-0.2.0/README.md` & `neon-mana-utils-0.2.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/__init__.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/bus_api.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/bus_api.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/cli.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/cli.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/config.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/config.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/constants.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/constants.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/core_commands.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/core_commands.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/messagebus.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/messagebus.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/skills.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/skills.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/status.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/status.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils/version.py` & `neon-mana-utils-0.2.1a1/neon_mana_utils/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.2.0"
+__version__ = "0.2.1a1"
```

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils.egg-info/PKG-INFO` & `neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mana-utils
-Version: 0.2.0
+Version: 0.2.1a1
 Summary: Message Application for Neon AI
 Home-page: https://github.com/neongeckocom/neon-mana-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-mana-utils-0.2.0/neon_mana_utils.egg-info/SOURCES.txt` & `neon-mana-utils-0.2.1a1/neon_mana_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.0/setup.py` & `neon-mana-utils-0.2.1a1/setup.py`

 * *Files identical despite different names*

