# Comparing `tmp/pyhids-0.5.0.tar.gz` & `tmp/pyhids-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhids-0.5.0.tar", max compression
+gzip compressed data, was "pyhids-0.5.1.tar", max compression
```

## Comparing `pyhids-0.5.0.tar` & `pyhids-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rwxr-xr-x   0        0        0     3293 2023-07-17 17:14:36.982829 pyhids-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-07-17 16:49:42.208696 pyhids-0.5.0/pyhids/__init__.py
--rwxr-xr-x   0        0        0     4484 2023-07-17 16:54:13.611030 pyhids-0.5.0/pyhids/genBase.py
--rwxr-xr-x   0        0        0     1794 2023-07-17 16:53:16.896992 pyhids-0.5.0/pyhids/genKeys.py
--rwxr-xr-x   0        0        0    11025 2023-07-17 17:26:39.395501 pyhids-0.5.0/pyhids/pyHIDS.py
--rw-r--r--   0        0        0      950 2023-07-17 17:27:00.970601 pyhids-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4110 1970-01-01 00:00:00.000000 pyhids-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35146 2023-07-16 10:30:39.177836 pyhids-0.5.1/COPYING
+-rwxr-xr-x   0        0        0     3293 2023-07-17 17:14:36.982829 pyhids-0.5.1/README.md
+-rwxr-xr-x   0        0        0     3088 2023-07-18 20:17:49.255292 pyhids-0.5.1/conf.py
+-rw-r--r--   0        0        0        0 2023-07-17 16:49:42.208696 pyhids-0.5.1/pyhids/__init__.py
+-rwxr-xr-x   0        0        0     4484 2023-07-17 22:18:35.631711 pyhids-0.5.1/pyhids/genBase.py
+-rwxr-xr-x   0        0        0     1794 2023-07-17 16:53:16.896992 pyhids-0.5.1/pyhids/genKeys.py
+-rwxr-xr-x   0        0        0    11025 2023-07-17 22:18:21.663851 pyhids-0.5.1/pyhids/pyHIDS.py
+-rw-r--r--   0        0        0     1154 2023-07-18 20:19:44.056505 pyhids-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4228 1970-01-01 00:00:00.000000 pyhids-0.5.1/PKG-INFO
```

### Comparing `pyhids-0.5.0/README.md` & `pyhids-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyhids-0.5.0/pyhids/genBase.py` & `pyhids-0.5.1/pyhids/genBase.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.5.0/pyhids/genKeys.py` & `pyhids-0.5.1/pyhids/genKeys.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.5.0/pyhids/pyHIDS.py` & `pyhids-0.5.1/pyhids/pyHIDS.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-pyHIDS Copyright (C) 2010-2018 Cedric Bonhomme
+pyHIDS Copyright (C) 2010-2023 Cedric Bonhomme
 This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
 This is free software, and you are welcome to redistribute it
 under certain conditions; type `show c' for details.
 """
 
 __author__ = "Cedric Bonhomme"
 __version__ = "$Revision: 0.5 $"
```

### Comparing `pyhids-0.5.0/pyproject.toml` & `pyhids-0.5.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 [tool.poetry]
 name = "pyHIDS"
-version = "0.5.0"
+version = "0.5.1"
 description = "A host-based intrusion detection system."
 authors = ["Cédric Bonhomme <cedric@cedricbonhomme.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
+homepage = "https://github.com/cedricbonhomme/pyHIDS"
+repository = "https://github.com/cedricbonhomme/pyHIDS"
+
 keywords = ["hids", "security"]
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Security",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
 ]
 
+include = [
+    "README.md",
+    "COPYING",
+    "conf.py",
+]
+
 [tool.poetry.scripts]
 pyhids-genKeys = "pyhids.genKeys:main"
 pyhids-genBase = "pyhids.genBase:main"
 pyhids-run = "pyhids.pyHIDS:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 rsa = "^4.9"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
```

### Comparing `pyhids-0.5.0/PKG-INFO` & `pyhids-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: pyhids
-Version: 0.5.0
+Version: 0.5.1
 Summary: A host-based intrusion detection system.
+Home-page: https://github.com/cedricbonhomme/pyHIDS
 License: GPL-3.0-or-later
 Keywords: hids,security
 Author: Cédric Bonhomme
 Author-email: cedric@cedricbonhomme.org
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -14,14 +15,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security
 Requires-Dist: rsa (>=4.9,<5.0)
+Project-URL: Repository, https://github.com/cedricbonhomme/pyHIDS
 Description-Content-Type: text/markdown
 
 ## pyHIDS
 
 
 ### Presentation
```

