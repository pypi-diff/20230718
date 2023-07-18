# Comparing `tmp/repository-updater-1.2.5.tar.gz` & `tmp/repository-updater-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repository-updater-1.2.5.tar", last modified: Tue Mar 14 10:27:44 2023, max compression
+gzip compressed data, was "repository-updater-1.3.0.tar", last modified: Tue Jul 18 18:26:55 2023, max compression
```

## Comparing `repository-updater-1.2.5.tar` & `repository-updater-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 frenck    (1000) frenck    (1000)        0 2023-03-14 10:27:44.127370 repository-updater-1.2.5/
--rwxr-xr-x   0 frenck    (1000) frenck    (1000)     1077 2023-03-13 10:56:30.000000 repository-updater-1.2.5/LICENSE.md
--rw-r--r--   0 frenck    (1000) frenck    (1000)     1129 2023-03-14 10:27:44.127370 repository-updater-1.2.5/PKG-INFO
--rwxr-xr-x   0 frenck    (1000) frenck    (1000)    12628 2023-03-13 10:56:30.000000 repository-updater-1.2.5/README.md
-drwxr-xr-x   0 frenck    (1000) frenck    (1000)        0 2023-03-14 10:27:44.123370 repository-updater-1.2.5/repository_updater.egg-info/
--rw-r--r--   0 frenck    (1000) frenck    (1000)     1129 2023-03-14 10:27:44.000000 repository-updater-1.2.5/repository_updater.egg-info/PKG-INFO
--rw-r--r--   0 frenck    (1000) frenck    (1000)      482 2023-03-14 10:27:44.000000 repository-updater-1.2.5/repository_updater.egg-info/SOURCES.txt
--rw-r--r--   0 frenck    (1000) frenck    (1000)        1 2023-03-14 10:27:44.000000 repository-updater-1.2.5/repository_updater.egg-info/dependency_links.txt
--rw-r--r--   0 frenck    (1000) frenck    (1000)      147 2023-03-14 10:27:44.000000 repository-updater-1.2.5/repository_updater.egg-info/entry_points.txt
--rw-r--r--   0 frenck    (1000) frenck    (1000)      140 2023-03-14 10:27:44.000000 repository-updater-1.2.5/repository_updater.egg-info/requires.txt
--rw-r--r--   0 frenck    (1000) frenck    (1000)       18 2023-03-14 10:27:44.000000 repository-updater-1.2.5/repository_updater.egg-info/top_level.txt
-drwxr-xr-x   0 frenck    (1000) frenck    (1000)        0 2023-03-14 10:27:44.127370 repository-updater-1.2.5/repositoryupdater/
--rw-r--r--   0 frenck    (1000) frenck    (1000)      543 2023-03-14 10:27:37.000000 repository-updater-1.2.5/repositoryupdater/__init__.py
--rw-r--r--   0 frenck    (1000) frenck    (1000)      133 2021-01-13 17:56:41.000000 repository-updater-1.2.5/repositoryupdater/__main__.py
--rw-r--r--   0 frenck    (1000) frenck    (1000)    15774 2023-03-14 10:18:29.000000 repository-updater-1.2.5/repositoryupdater/addon.py
--rw-r--r--   0 frenck    (1000) frenck    (1000)     1847 2023-03-13 10:56:27.000000 repository-updater-1.2.5/repositoryupdater/cli.py
--rw-r--r--   0 frenck    (1000) frenck    (1000)      183 2021-01-13 17:57:03.000000 repository-updater-1.2.5/repositoryupdater/const.py
--rw-r--r--   0 frenck    (1000) frenck    (1000)     1174 2023-03-13 10:56:27.000000 repository-updater-1.2.5/repositoryupdater/github.py
--rw-r--r--   0 frenck    (1000) frenck    (1000)     7372 2023-03-13 10:56:27.000000 repository-updater-1.2.5/repositoryupdater/repository.py
--rw-r--r--   0 frenck    (1000) frenck    (1000)       38 2023-03-14 10:27:44.127370 repository-updater-1.2.5/setup.cfg
--rw-r--r--   0 frenck    (1000) frenck    (1000)     1610 2023-03-13 12:08:52.000000 repository-updater-1.2.5/setup.py
+drwxr-xr-x   0 frenck    (1000) frenck    (1000)        0 2023-07-18 18:26:55.463341 repository-updater-1.3.0/
+-rwxr-xr-x   0 frenck    (1000) frenck    (1000)     1077 2023-03-13 10:56:30.000000 repository-updater-1.3.0/LICENSE.md
+-rw-r--r--   0 frenck    (1000) frenck    (1000)     1129 2023-07-18 18:26:55.463341 repository-updater-1.3.0/PKG-INFO
+-rwxr-xr-x   0 frenck    (1000) frenck    (1000)    12626 2023-07-18 18:24:05.000000 repository-updater-1.3.0/README.md
+drwxr-xr-x   0 frenck    (1000) frenck    (1000)        0 2023-07-18 18:26:55.463341 repository-updater-1.3.0/repository_updater.egg-info/
+-rw-r--r--   0 frenck    (1000) frenck    (1000)     1129 2023-07-18 18:26:55.000000 repository-updater-1.3.0/repository_updater.egg-info/PKG-INFO
+-rw-r--r--   0 frenck    (1000) frenck    (1000)      482 2023-07-18 18:26:55.000000 repository-updater-1.3.0/repository_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 frenck    (1000) frenck    (1000)        1 2023-07-18 18:26:55.000000 repository-updater-1.3.0/repository_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 frenck    (1000) frenck    (1000)      147 2023-07-18 18:26:55.000000 repository-updater-1.3.0/repository_updater.egg-info/entry_points.txt
+-rw-r--r--   0 frenck    (1000) frenck    (1000)      141 2023-07-18 18:26:55.000000 repository-updater-1.3.0/repository_updater.egg-info/requires.txt
+-rw-r--r--   0 frenck    (1000) frenck    (1000)       18 2023-07-18 18:26:55.000000 repository-updater-1.3.0/repository_updater.egg-info/top_level.txt
+drwxr-xr-x   0 frenck    (1000) frenck    (1000)        0 2023-07-18 18:26:55.463341 repository-updater-1.3.0/repositoryupdater/
+-rw-r--r--   0 frenck    (1000) frenck    (1000)      543 2023-07-18 18:26:49.000000 repository-updater-1.3.0/repositoryupdater/__init__.py
+-rw-r--r--   0 frenck    (1000) frenck    (1000)      133 2021-01-13 17:56:41.000000 repository-updater-1.3.0/repositoryupdater/__main__.py
+-rw-r--r--   0 frenck    (1000) frenck    (1000)    15774 2023-03-14 10:28:27.000000 repository-updater-1.3.0/repositoryupdater/addon.py
+-rw-r--r--   0 frenck    (1000) frenck    (1000)     1847 2023-03-13 10:56:27.000000 repository-updater-1.3.0/repositoryupdater/cli.py
+-rw-r--r--   0 frenck    (1000) frenck    (1000)      183 2021-01-13 17:57:03.000000 repository-updater-1.3.0/repositoryupdater/const.py
+-rw-r--r--   0 frenck    (1000) frenck    (1000)     1174 2023-03-13 10:56:27.000000 repository-updater-1.3.0/repositoryupdater/github.py
+-rw-r--r--   0 frenck    (1000) frenck    (1000)     7372 2023-03-13 10:56:27.000000 repository-updater-1.3.0/repositoryupdater/repository.py
+-rw-r--r--   0 frenck    (1000) frenck    (1000)       38 2023-07-18 18:26:55.463341 repository-updater-1.3.0/setup.cfg
+-rw-r--r--   0 frenck    (1000) frenck    (1000)     1611 2023-07-18 18:24:05.000000 repository-updater-1.3.0/setup.py
```

### Comparing `repository-updater-1.2.5/LICENSE.md` & `repository-updater-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `repository-updater-1.2.5/PKG-INFO` & `repository-updater-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-updater
-Version: 1.2.5
+Version: 1.3.0
 Home-page: https://github.com/hassio-addons/repository-updater
 Author: Franck Nijhof
 Author-email: frenck@addons.community
 License: MIT
 Keywords: addons,repository,home assistant,home-assistant,add-ons,frenck
 Platform: any
 Classifier: Environment :: Console
```

### Comparing `repository-updater-1.2.5/README.md` & `repository-updater-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 [commits-shield]: https://img.shields.io/github/commit-activity/y/hassio-addons/repository-updater.svg
-[commits]: https://github.com/hassio-addons/repository-updater/commits/master
+[commits]: https://github.com/hassio-addons/repository-updater/commits/main
 [contributors]: https://github.com/hassio-addons/repository-updater/graphs/contributors
 [discord-shield]: https://img.shields.io/discord/330944238910963714.svg
 [discord]: https://discord.gg/c5DvZ4e
 [forum-shield]: https://img.shields.io/badge/community-forum-brightgreen.svg
 [forum]: https://community.home-assistant.io?u=frenck
 [frenck]: https://github.com/frenck
 [issue]: https://github.com/hassio-addons/repository-updater/issues
```

### Comparing `repository-updater-1.2.5/repository_updater.egg-info/PKG-INFO` & `repository-updater-1.3.0/repository_updater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-updater
-Version: 1.2.5
+Version: 1.3.0
 Home-page: https://github.com/hassio-addons/repository-updater
 Author: Franck Nijhof
 Author-email: frenck@addons.community
 License: MIT
 Keywords: addons,repository,home assistant,home-assistant,add-ons,frenck
 Platform: any
 Classifier: Environment :: Console
```

### Comparing `repository-updater-1.2.5/repositoryupdater/__init__.py` & `repository-updater-1.3.0/repositoryupdater/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 Please note, this program cannot be used with the general documented
 Home Assistant add-on repository approach.
 """
 
 APP_NAME = "repository-updater"
 APP_FULL_NAME = "Community Home Assistant Add-ons Repository Updater"
-APP_VERSION = "1.2.5"
+APP_VERSION = "1.3.0"
 APP_DESCRIPTION = __doc__
 
 __version__ = APP_VERSION
```

### Comparing `repository-updater-1.2.5/repositoryupdater/addon.py` & `repository-updater-1.3.0/repositoryupdater/addon.py`

 * *Files identical despite different names*

### Comparing `repository-updater-1.2.5/repositoryupdater/cli.py` & `repository-updater-1.3.0/repositoryupdater/cli.py`

 * *Files identical despite different names*

### Comparing `repository-updater-1.2.5/repositoryupdater/github.py` & `repository-updater-1.3.0/repositoryupdater/github.py`

 * *Files identical despite different names*

### Comparing `repository-updater-1.2.5/repositoryupdater/repository.py` & `repository-updater-1.3.0/repositoryupdater/repository.py`

 * *Files identical despite different names*

### Comparing `repository-updater-1.2.5/setup.py` & `repository-updater-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,23 +31,23 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Utilities",
     ],
     packages=find_packages(),
     install_requires=[
-        "click==8.1.3",
+        "click==8.1.5",
         "crayons==0.4.0",
-        "emoji==2.2.0",
-        "GitPython==3.1.31",
+        "emoji==2.6.0",
+        "GitPython==3.1.32",
         "Jinja2==3.1.2",
-        "PyGithub==1.58.0",
+        "PyGithub==1.59.0",
         "python-dateutil==2.8.2",
-        "PyYAML==6.0",
-        "semver==2.13.0",
+        "PyYAML==6.0.1",
+        "semver==3.0.1",
     ],
     entry_points="""
         [console_scripts]
             repository-updater=repositoryupdater.cli:repository_updater
             repository-updater-git-askpass=repositoryupdater.cli:git_askpass
     """,
 )
```

