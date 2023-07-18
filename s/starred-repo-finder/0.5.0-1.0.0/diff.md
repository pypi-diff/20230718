# Comparing `tmp/starred_repo_finder-0.5.0.tar.gz` & `tmp/starred_repo_finder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred_repo_finder-0.5.0.tar", last modified: Tue Jul 18 11:36:06 2023, max compression
+gzip compressed data, was "starred_repo_finder-1.0.0.tar", last modified: Tue Jul 18 14:47:32 2023, max compression
```

## Comparing `starred_repo_finder-0.5.0.tar` & `starred_repo_finder-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/starred_repo_finder/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/starred_repo_finder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/starred_repo_finder/starred_repo_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/tests/test_starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:47:32.989931 starred_repo_finder-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-18 14:47:32.989931 starred_repo_finder-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:47:32.989931 starred_repo_finder-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:47:32.985931 starred_repo_finder-1.0.0/starred_repo_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/starred_repo_finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/starred_repo_finder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/starred_repo_finder/starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:47:32.985931 starred_repo_finder-1.0.0/starred_repo_finder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-18 14:47:32.000000 starred_repo_finder-1.0.0/starred_repo_finder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-18 14:47:32.000000 starred_repo_finder-1.0.0/starred_repo_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:47:32.000000 starred_repo_finder-1.0.0/starred_repo_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-18 14:47:32.000000 starred_repo_finder-1.0.0/starred_repo_finder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 14:47:32.000000 starred_repo_finder-1.0.0/starred_repo_finder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 14:47:32.000000 starred_repo_finder-1.0.0/starred_repo_finder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:47:32.985931 starred_repo_finder-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-18 14:47:15.000000 starred_repo_finder-1.0.0/tests/test_starred_repo_finder.py
```

### Comparing `starred_repo_finder-0.5.0/LICENSE` & `starred_repo_finder-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starred_repo_finder-0.5.0/PKG-INFO` & `starred_repo_finder-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starred_repo_finder
-Version: 0.5.0
+Version: 1.0.0
 Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 Home-page: https://github.com/tylercb/starred_repo_finder
 Author: Tyler Hanway
 Author-email: hanway.tyler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `starred_repo_finder-0.5.0/README.md` & `starred_repo_finder-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `starred_repo_finder-0.5.0/starred_repo_finder/starred_repo_finder.py` & `starred_repo_finder-1.0.0/starred_repo_finder/starred_repo_finder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 
 import requests
-import click
 import json
 from rich.console import Console
 from rich.table import Table
 
 console = Console()
 
 
@@ -179,36 +178,8 @@
     # Ensure the response is not None and has a 200 status code
     if not response or response.status_code != 200:
         console.print("No response or bad response from server.", style="bold red")
         return
 
     # Process the response
     results = process_response(response)
-
-    # Print the results
-    print_results(results, output_format)
-
-@click.command()
-@click.argument('repo_name')
-@click.option('--limit', '-l', default=100, help='The maximum number of results to return (default: 100)', type=int)
-@click.option('--order', '-o', default='stargazers', help='Column to order by (default: stargazers). Options: stargazers, forkers, ratio', type=click.Choice(['stargazers', 'forkers', 'ratio'], case_sensitive=False))
-@click.option('--stargazers', '-s', default=None, help='Minimum number of stargazers to include (default: None)', type=int)
-@click.option('--forkers', '-f', default=None, help='Minimum number of forkers to include (default: None)', type=int)
-@click.option('--ratio', '-r', default=None, help='Minimum ratio of stargazers to forkers to include (default: None)', type=float)
-@click.option('--format', '-fmt', default='table', help='Output format (default: table). Options: table, csv, json, markdown', type=click.Choice(['table', 'csv', 'json', 'markdown'], case_sensitive=False))
-def main(repo_name, limit, order, stargazers, forkers, ratio, format):
-    """
-    Parse command line arguments
-    """
-    run(
-        repo_name,
-        limit,
-        order,
-        stargazers,
-        forkers,
-        ratio,
-        format,
-    )
-
-
-if __name__ == "__main__":
-    main()
+    return convert_and_format_results(results, output_format)
```

### Comparing `starred_repo_finder-0.5.0/starred_repo_finder.egg-info/PKG-INFO` & `starred_repo_finder-1.0.0/starred_repo_finder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starred-repo-finder
-Version: 0.5.0
+Version: 1.0.0
 Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 Home-page: https://github.com/tylercb/starred_repo_finder
 Author: Tyler Hanway
 Author-email: hanway.tyler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `starred_repo_finder-0.5.0/tests/test_starred_repo_finder.py` & `starred_repo_finder-1.0.0/tests/test_starred_repo_finder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import unittest
 from unittest.mock import patch, Mock
-from click.testing import CliRunner
 from starred_repo_finder.starred_repo_finder import (
     build_query,
     make_request,
     process_response,
     print_results,
     run,
     convert_and_format_results,
-    main,
 )
 
 
 class TestStarredRepoFinder(unittest.TestCase):
     def test_build_query(self):
         result_query = build_query("test_repo", 50, "stargazers", None, None, None)
         self.assertIn("test_repo", result_query)
@@ -74,41 +72,23 @@
         converted_and_formatted_results = convert_and_format_results(
             [["test_repo", "100", "20", "5"]], "json"
         )
         self.assertEqual(
             converted_and_formatted_results[0][0]["repo_name"], "test_repo"
         )
 
-    @patch("starred_repo_finder.starred_repo_finder.console.print")
     @patch("starred_repo_finder.starred_repo_finder.make_request")
-    def test_run(self, mock_request, mock_print):
+    def test_run(self, mock_request):
         # setup
         mock_request.return_value.status_code = 200
         mock_request.return_value.content = b"test_repo\t100\t20\t5\n"
 
         # action
-        run("test_repo", 50, "stargazers", None, None, None, "table")
+        result = run("test_repo", 50, "stargazers", None, None, None, "table")
 
         # assert
         mock_request.assert_called_once()
-        self.assertTrue(mock_print.called)
-
-    @patch("starred_repo_finder.starred_repo_finder.run")
-    def test_main(self, mock_run):
-        runner = CliRunner()
-
-        # setup
-        repo_name = "test_repo"
-        limit = 50
-        order = "stargazers"
-        format = "table"
-
-        # action
-        result = runner.invoke(main, [repo_name, '--limit', str(limit), '--order', order, '--format', format])
-
-        # assert
-        self.assertEqual(result.exit_code, 0)
-        mock_run.assert_called_once_with(repo_name, limit, order, None, None, None, format)
+        self.assertIsNotNone(result)
 
 
 if __name__ == "__main__":
     unittest.main()
```

