# Comparing `tmp/gorilla-cli-0.0.8.tar.gz` & `tmp/gorilla-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gorilla-cli-0.0.8.tar", last modified: Thu Jun 29 18:03:12 2023, max compression
+gzip compressed data, was "gorilla-cli-0.0.9.tar", last modified: Tue Jul 18 06:46:43 2023, max compression
```

## Comparing `gorilla-cli-0.0.8.tar` & `gorilla-cli-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.807590 gorilla-cli-0.0.8/
--rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/LICENSE
--rw-r--r--   0 shishir    (501) staff       (20)     2581 2023-06-29 18:03:12.807271 gorilla-cli-0.0.8/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)     2075 2023-06-29 17:39:11.000000 gorilla-cli-0.0.8/README.md
--rw-r--r--   0 shishir    (501) staff       (20)     6804 2023-06-29 18:03:01.000000 gorilla-cli-0.0.8/go_cli.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.804568 gorilla-cli-0.0.8/go_questionary/
--rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/constants.py
--rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/form.py
--rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompt.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.806196 gorilla-cli-0.0.8/go_questionary/prompts/
--rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/autocomplete.py
--rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/checkbox.py
--rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/common.py
--rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/confirm.py
--rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/password.py
--rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/path.py
--rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/rawselect.py
--rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/select.py
--rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/prompts/text.py
--rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/question.py
--rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/utils.py
--rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-20 08:46:02.000000 gorilla-cli-0.0.8/go_questionary/version.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-29 18:03:12.807044 gorilla-cli-0.0.8/gorilla_cli.egg-info/
--rw-r--r--   0 shishir    (501) staff       (20)     2581 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/SOURCES.txt
--rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/dependency_links.txt
--rw-r--r--   0 shishir    (501) staff       (20)       41 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/entry_points.txt
--rw-r--r--   0 shishir    (501) staff       (20)       29 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/requires.txt
--rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-29 18:03:12.000000 gorilla-cli-0.0.8/gorilla_cli.egg-info/top_level.txt
--rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-29 18:03:12.807642 gorilla-cli-0.0.8/setup.cfg
--rw-r--r--   0 shishir    (501) staff       (20)     1507 2023-06-29 18:02:23.000000 gorilla-cli-0.0.8/setup.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-07-18 06:46:43.285856 gorilla-cli-0.0.9/
+-rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/LICENSE
+-rw-r--r--   0 shishir    (501) staff       (20)     3515 2023-07-18 06:46:43.285672 gorilla-cli-0.0.9/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)     3009 2023-07-18 06:41:36.000000 gorilla-cli-0.0.9/README.md
+-rw-r--r--   0 shishir    (501) staff       (20)     7006 2023-07-18 06:42:50.000000 gorilla-cli-0.0.9/go_cli.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-07-18 06:46:43.283200 gorilla-cli-0.0.9/go_questionary/
+-rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/constants.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/form.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompt.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-07-18 06:46:43.284798 gorilla-cli-0.0.9/go_questionary/prompts/
+-rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/autocomplete.py
+-rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/checkbox.py
+-rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/common.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/confirm.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/password.py
+-rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/path.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/rawselect.py
+-rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/select.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/prompts/text.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/question.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/utils.py
+-rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-20 08:46:02.000000 gorilla-cli-0.0.9/go_questionary/version.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-07-18 06:46:43.285484 gorilla-cli-0.0.9/gorilla_cli.egg-info/
+-rw-r--r--   0 shishir    (501) staff       (20)     3515 2023-07-18 06:46:43.000000 gorilla-cli-0.0.9/gorilla_cli.egg-info/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)      770 2023-07-18 06:46:43.000000 gorilla-cli-0.0.9/gorilla_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 shishir    (501) staff       (20)        1 2023-07-18 06:46:43.000000 gorilla-cli-0.0.9/gorilla_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       41 2023-07-18 06:46:43.000000 gorilla-cli-0.0.9/gorilla_cli.egg-info/entry_points.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       29 2023-07-18 06:46:43.000000 gorilla-cli-0.0.9/gorilla_cli.egg-info/requires.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       22 2023-07-18 06:46:43.000000 gorilla-cli-0.0.9/gorilla_cli.egg-info/top_level.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       38 2023-07-18 06:46:43.285977 gorilla-cli-0.0.9/setup.cfg
+-rw-r--r--   0 shishir    (501) staff       (20)     1530 2023-07-18 05:43:36.000000 gorilla-cli-0.0.9/setup.py
```

### Comparing `gorilla-cli-0.0.8/LICENSE` & `gorilla-cli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_cli.py` & `gorilla-cli-0.0.9/go_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 import requests
 import subprocess
 import urllib.parse
 import sys
 from halo import Halo
 import go_questionary
 
-__version__ = "0.0.8"  # current version
+__version__ = "0.0.9"  # current version
 SERVER_URL = "http://34.135.112.197:8000"
 UPDATE_CHECK_FILE = os.path.expanduser("~/.gorilla-cli-last-update-check")
 USERID_FILE = os.path.expanduser("~/.gorilla-cli-userid")
 ISSUE_URL = f"https://github.com/gorilla-llm/gorilla-cli/issues/new"
 WELCOME_TEXT = """🦍 Welcome to Gorilla-CLI! Enhance your Command Line with the power of LLMs! 
 
 Simply use `gorilla <your desired operation>` and Gorilla will do the rest. For instance:
-    gorilla what is the path of my current directory
+    gorilla generate 100 random characters into a file called test.txt
+    gorilla get the image ids of all pods running in all namespaces in kubernetes
     gorilla list all my GCP instances
 
-Created as a research prototype by UC Berkeley, Gorilla-CLI ensures user control and privacy:
+A research prototype from UC Berkeley, Gorilla-CLI ensures user control and privacy:
  - Commands are executed only with explicit user approval.
  - While queries and error (stderr) logs are used to refine our model, we NEVER gather output (stdout) data.
 
-Visit us at github.com/gorilla-llm/gorilla-cli and start talking to your CLI!"""
+Visit github.com/gorilla-llm/gorilla-cli for examples and to learn more!"""
 
 
 def check_for_updates():
     # Check if a new version of gorilla-cli is available once a day
     try:
         with open(UPDATE_CHECK_FILE, "r") as f:
             last_check_date = datetime.datetime.strptime(f.read(), "%Y-%m-%d")
@@ -69,15 +70,17 @@
     # Gorilla-CLI is hosted by UC Berkeley Sky lab for FREE as a
     #  research prototype. Please don't spam the system or use it
     #  for commercial serving. If you would like to request rate
     #  limit increases for your GitHub handle, please raise an issue.
     try:
         with open(USERID_FILE, "r") as f:
             user_id = str(f.read())
-            assert user_id != ""
+            # If file found and user_id is blank. User hasn't setup github
+            if user_id == "":
+                user_id = str(uuid.uuid4())
         return user_id
     except FileNotFoundError:
         try:
             user_id = (
                 subprocess.check_output(["git", "config", "--global", "user.email"])
                 .decode("utf-8")
                 .strip()
```

### Comparing `gorilla-cli-0.0.8/go_questionary/__init__.py` & `gorilla-cli-0.0.9/go_questionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/constants.py` & `gorilla-cli-0.0.9/go_questionary/constants.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/form.py` & `gorilla-cli-0.0.9/go_questionary/form.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompt.py` & `gorilla-cli-0.0.9/go_questionary/prompt.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/__init__.py` & `gorilla-cli-0.0.9/go_questionary/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/autocomplete.py` & `gorilla-cli-0.0.9/go_questionary/prompts/autocomplete.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/checkbox.py` & `gorilla-cli-0.0.9/go_questionary/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/common.py` & `gorilla-cli-0.0.9/go_questionary/prompts/common.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/confirm.py` & `gorilla-cli-0.0.9/go_questionary/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/password.py` & `gorilla-cli-0.0.9/go_questionary/prompts/password.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/path.py` & `gorilla-cli-0.0.9/go_questionary/prompts/path.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/rawselect.py` & `gorilla-cli-0.0.9/go_questionary/prompts/rawselect.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/select.py` & `gorilla-cli-0.0.9/go_questionary/prompts/select.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/prompts/text.py` & `gorilla-cli-0.0.9/go_questionary/prompts/text.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/question.py` & `gorilla-cli-0.0.9/go_questionary/question.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/go_questionary/utils.py` & `gorilla-cli-0.0.9/go_questionary/utils.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/gorilla_cli.egg-info/SOURCES.txt` & `gorilla-cli-0.0.9/gorilla_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.8/setup.py` & `gorilla-cli-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup, find_packages
 
 setup(
     name="gorilla-cli",
-    version="0.0.8",
+    version="0.0.9",
     url="https://github.com/gorilla-llm/gorilla-cli",
     author="Shishir Patil, Tianjun Zhang",
     author_email="sgp@berkeley.edu, tianjunz@berkeley.edu",
     description="LLMs for CLI",
-    long_description=open("README.md").read(),
+    long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["go_cli"],
     packages=find_packages(include=["*", "go_questionary.*"]),
     install_requires=[
         "requests",
         "halo",
         "prompt-toolkit",
```

