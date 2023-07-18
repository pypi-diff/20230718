# Comparing `tmp/mkdocs-redirects-1.1.0.tar.gz` & `tmp/mkdocs-redirects-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-redirects-1.1.0.tar", last modified: Mon Aug 22 17:25:12 2022, max compression
+gzip compressed data, was "mkdocs-redirects-1.2.0.tar", last modified: Sun Sep 18 12:17:04 2022, max compression
```

## Comparing `mkdocs-redirects-1.1.0.tar` & `mkdocs-redirects-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-08-22 17:25:12.178368 mkdocs-redirects-1.1.0/
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     1071 2022-03-30 19:04:52.000000 mkdocs-redirects-1.1.0/LICENSE
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     4335 2022-08-22 17:25:12.178368 mkdocs-redirects-1.1.0/PKG-INFO
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     3241 2022-08-03 15:51:23.000000 mkdocs-redirects-1.1.0/README.md
-drwxr-xr-x   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-08-22 17:25:12.178368 mkdocs-redirects-1.1.0/mkdocs_redirects/
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-03-29 17:54:34.000000 mkdocs-redirects-1.1.0/mkdocs_redirects/__init__.py
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     6229 2022-08-22 17:23:02.000000 mkdocs-redirects-1.1.0/mkdocs_redirects/plugin.py
-drwxr-xr-x   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-08-22 17:25:12.178368 mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     4335 2022-08-22 17:25:11.000000 mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/PKG-INFO
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)      334 2022-08-22 17:25:11.000000 mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/SOURCES.txt
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)        1 2022-08-22 17:25:11.000000 mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/dependency_links.txt
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)       68 2022-08-22 17:25:11.000000 mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/entry_points.txt
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)      232 2022-08-22 17:25:11.000000 mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/requires.txt
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)       17 2022-08-22 17:25:11.000000 mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/top_level.txt
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)      134 2022-08-22 17:25:12.178368 mkdocs-redirects-1.1.0/setup.cfg
--rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     1908 2022-08-22 17:24:36.000000 mkdocs-redirects-1.1.0/setup.py
+drwxr-xr-x   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-09-18 12:17:04.689235 mkdocs-redirects-1.2.0/
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     1071 2022-03-30 19:04:52.000000 mkdocs-redirects-1.2.0/LICENSE
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     4217 2022-09-18 12:17:04.689235 mkdocs-redirects-1.2.0/PKG-INFO
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     3241 2022-08-03 15:51:23.000000 mkdocs-redirects-1.2.0/README.md
+drwxr-xr-x   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-09-18 12:17:04.689235 mkdocs-redirects-1.2.0/mkdocs_redirects/
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-03-29 17:54:34.000000 mkdocs-redirects-1.2.0/mkdocs_redirects/__init__.py
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     4777 2022-09-18 10:48:48.000000 mkdocs-redirects-1.2.0/mkdocs_redirects/plugin.py
+drwxr-xr-x   0 blaxpirit  (1000) blaxpirit  (1000)        0 2022-09-18 12:17:04.689235 mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     4217 2022-09-18 12:17:04.000000 mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/PKG-INFO
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)      334 2022-09-18 12:17:04.000000 mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/SOURCES.txt
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)        1 2022-09-18 12:17:04.000000 mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/dependency_links.txt
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)       68 2022-09-18 12:17:04.000000 mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/entry_points.txt
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)      126 2022-09-18 12:17:04.000000 mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/requires.txt
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)       17 2022-09-18 12:17:04.000000 mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/top_level.txt
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)      134 2022-09-18 12:17:04.689235 mkdocs-redirects-1.2.0/setup.cfg
+-rw-r--r--   0 blaxpirit  (1000) blaxpirit  (1000)     1763 2022-09-18 12:16:14.000000 mkdocs-redirects-1.2.0/setup.py
```

### Comparing `mkdocs-redirects-1.1.0/LICENSE` & `mkdocs-redirects-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-redirects-1.1.0/PKG-INFO` & `mkdocs-redirects-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: mkdocs-redirects
-Version: 1.1.0
+Version: 1.2.0
 Summary: A MkDocs plugin for dynamic page redirects to prevent broken links.
 Home-page: https://github.com/datarobot/mkdocs-redirects
 Author: Dustin Burke
 Author-email: dustin@datarobot.com
 License: MIT
 Keywords: mkdocs redirect
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: release
 License-File: LICENSE
 
 # mkdocs-redirects
@@ -117,9 +114,7 @@
 
 It will prompt you for your PyPI user and password.
 
 See:
 
 - <https://packaging.python.org/tutorials/packaging-projects/>
 - <https://packaging.python.org/guides/migrating-to-pypi-org/>
-
-
```

### Comparing `mkdocs-redirects-1.1.0/README.md` & `mkdocs-redirects-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-redirects-1.1.0/mkdocs_redirects/plugin.py` & `mkdocs-redirects-1.2.0/mkdocs_redirects/plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,119 +1,89 @@
 """
 Copyright 2019-2022 DataRobot, Inc. and its affiliates.
 All rights reserved.
 """
 import logging
 import os
 import posixpath
-import textwrap
 
 from mkdocs import utils
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
+from mkdocs.structure.files import File
 
 log = logging.getLogger('mkdocs.plugin.redirects')
 log.addFilter(utils.warning_filter)
 
 
+HTML_TEMPLATE = """
+<!doctype html>
+<html lang="en">
+<head>
+    <meta charset="utf-8">
+    <title>Redirecting...</title>
+    <link rel="canonical" href="{url}">
+    <meta name="robots" content="noindex">
+    <script>var anchor=window.location.hash.substr(1);location.href="{url}"+(anchor?"#"+anchor:"")</script>
+    <meta http-equiv="refresh" content="0; url={url}">
+</head>
+<body>
+Redirecting...
+</body>
+</html>
+"""
+
+
 def write_html(site_dir, old_path, new_path):
     """Write an HTML file in the site_dir with a meta redirect to the new page"""
     # Determine all relevant paths
     old_path_abs = os.path.join(site_dir, old_path)
     old_dir = os.path.dirname(old_path)
     old_dir_abs = os.path.dirname(old_path_abs)
 
     # Create parent directories if they don't exist
     if not os.path.exists(old_dir_abs):
         log.debug("Creating directory '%s'", old_dir)
         os.makedirs(old_dir_abs)
 
     # Write the HTML redirect file in place of the old file
+    log.debug("Creating redirect: '%s' -> '%s'", old_path, new_path)
+    content = HTML_TEMPLATE.format(url=new_path)
     with open(old_path_abs, 'w', encoding='utf-8') as f:
-        log.debug("Creating redirect: '%s' -> '%s'", old_path, new_path)
-        content = textwrap.dedent(
-            """
-            <!doctype html>
-            <html lang="en">
-            <head>
-                <meta charset="utf-8">
-                <title>Redirecting...</title>
-                <link rel="canonical" href="{url}">
-                <meta name="robots" content="noindex">
-                <script>var anchor=window.location.hash.substr(1);location.href="{url}"+(anchor?"#"+anchor:"")</script>
-                <meta http-equiv="refresh" content="0; url={url}">
-            </head>
-            <body>
-            Redirecting...
-            </body>
-            </html>
-            """
-        ).format(url=new_path)
         f.write(content)
 
 
 def get_relative_html_path(old_page, new_page, use_directory_urls):
     """Return the relative path from the old html path to the new html path"""
     old_path = get_html_path(old_page, use_directory_urls)
     new_path, new_hash_fragment = _split_hash_fragment(new_page)
-    new_path = get_html_path(new_path, use_directory_urls)
-
-    if use_directory_urls:
-        # remove /index.html from end of path
-        new_path = posixpath.dirname(new_path) or './'
 
     relative_path = posixpath.relpath(new_path, start=posixpath.dirname(old_path))
-
     if use_directory_urls:
         relative_path = relative_path + '/'
 
     return relative_path + new_hash_fragment
 
 
 def get_html_path(path, use_directory_urls):
     """Return the HTML file path for a given markdown file"""
-    parent, filename = posixpath.split(path)
-    name_orig = posixpath.splitext(filename)[0]
-
-    # Both `index.md` and `README.md` files are normalized to `index.html` during build
-    name = 'index' if name_orig in ('index', 'README') else name_orig
-
-    # Directory URLs require some different logic. This mirrors mkdocs' internal logic.
-    if use_directory_urls:
-
-        # If it's name is `index`, then that means it's the "homepage" of a directory, so should get placed in that dir
-        if name == 'index':
-            return posixpath.join(parent, 'index.html')
-
-        # Otherwise, it's a file within that folder, so it should go in its own directory to resolve properly
-        else:
-            return posixpath.join(parent, name, 'index.html')
-
-    # Just use the original name if Directory URLs aren't used
-    else:
-        return posixpath.join(parent, (name + '.html'))
+    f = File(path, '', '', use_directory_urls)
+    return f.dest_path.replace(os.sep, '/')
 
 
 class RedirectPlugin(BasePlugin):
     # Any options that this plugin supplies should go here.
     config_scheme = (
         ('redirect_maps', config_options.Type(dict, default={})),  # note the trailing comma
     )
 
     # Build a list of redirects on file generation
     def on_files(self, files, config, **kwargs):
         self.redirects = self.config.get('redirect_maps', {})
 
-        # SHIM! Produce a warning if the old root-level 'redirects' config is present
-        if config.get('redirects'):
-            log.warning(
-                "The root-level 'redirects:' setting is not valid and has been changed in version 1.0! "
-                "The plugin-level 'redirect-map' must be used instead. See https://git.io/fjdBN"
-            )
-
         # Validate user-provided redirect "old files"
         for page_old in self.redirects.keys():
             if not utils.is_markdown_file(page_old):
                 log.warning("redirects plugin: '%s' is not a valid markdown file!", page_old)
 
         # Build a dict of known document pages to validate against later
         self.doc_pages = {}
@@ -125,22 +95,23 @@
 
         # Determine if 'use_directory_urls' is set
         use_directory_urls = config.get('use_directory_urls')
 
         # Walk through the redirect map and write their HTML files
         for page_old, page_new in self.redirects.items():
             # Need to remove hash fragment from new page to verify existence
-            page_new_without_hash, _ = _split_hash_fragment(str(page_new))
+            page_new_without_hash, hash = _split_hash_fragment(str(page_new))
 
             # External redirect targets are easy, just use it as the target path
             if page_new.lower().startswith(('http://', 'https://')):
                 dest_path = page_new
 
             elif page_new_without_hash in self.doc_pages:
-                dest_path = get_relative_html_path(page_old, page_new, use_directory_urls)
+                file = self.doc_pages[page_new_without_hash]
+                dest_path = get_relative_html_path(page_old, file.url + hash, use_directory_urls)
 
             # If the redirect target isn't external or a valid internal page, throw an error
             # Note: we use 'warn' here specifically; mkdocs treats warnings specially when in strict mode
             else:
                 log.warning("Redirect target '%s' does not exist!", page_new)
                 continue
```

### Comparing `mkdocs-redirects-1.1.0/mkdocs_redirects.egg-info/PKG-INFO` & `mkdocs-redirects-1.2.0/mkdocs_redirects.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 Metadata-Version: 2.1
 Name: mkdocs-redirects
-Version: 1.1.0
+Version: 1.2.0
 Summary: A MkDocs plugin for dynamic page redirects to prevent broken links.
 Home-page: https://github.com/datarobot/mkdocs-redirects
 Author: Dustin Burke
 Author-email: dustin@datarobot.com
 License: MIT
 Keywords: mkdocs redirect
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=2.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: release
 License-File: LICENSE
 
 # mkdocs-redirects
@@ -117,9 +114,7 @@
 
 It will prompt you for your PyPI user and password.
 
 See:
 
 - <https://packaging.python.org/tutorials/packaging-projects/>
 - <https://packaging.python.org/guides/migrating-to-pypi-org/>
-
-
```

### Comparing `mkdocs-redirects-1.1.0/setup.py` & `mkdocs-redirects-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,52 +9,51 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 test_requirements = [
     'pytest',
-    'pytest <5; python_version < "3.0"',
+    'black',
+    'isort',
+    'autoflake',
 ]
 
 release_requirements = [
     'twine>=1.13.0',
-    'twine>=1.13.0,<2; python_version < "3.0"',
 ]
 
 
 setup(
     name='mkdocs-redirects',
-    version='1.1.0',
+    version='1.2.0',
     description='A MkDocs plugin for dynamic page redirects to prevent broken links.',
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     keywords='mkdocs redirect',
     url='https://github.com/datarobot/mkdocs-redirects',
     author='Dustin Burke',
     author_email='dustin@datarobot.com',
     license='MIT',
     license_files=['LICENSE'],
-    python_requires='>=2.7',
+    python_requires='>=3.6',
     install_requires=[
-        'mkdocs>=1.0.4,<2',
+        'mkdocs>=1.1.1',
     ],
     extras_require={
         'dev': test_requirements + release_requirements,
         'test': test_requirements,
         'release': release_requirements,
     },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
```

