# Comparing `tmp/starred_repo_finder-0.4.0.tar.gz` & `tmp/starred_repo_finder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starred_repo_finder-0.4.0.tar", last modified: Mon Jul 10 04:13:26 2023, max compression
+gzip compressed data, was "starred_repo_finder-0.5.0.tar", last modified: Tue Jul 18 11:36:06 2023, max compression
```

## Comparing `starred_repo_finder-0.4.0.tar` & `starred_repo_finder-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/starred_repo_finder/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/starred_repo_finder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/starred_repo_finder/starred_repo_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-10 04:13:26.000000 starred_repo_finder-0.4.0/starred_repo_finder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:26.498826 starred_repo_finder-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-10 04:13:15.000000 starred_repo_finder-0.4.0/tests/test_starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/starred_repo_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/starred_repo_finder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/starred_repo_finder/starred_repo_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 11:36:06.000000 starred_repo_finder-0.5.0/starred_repo_finder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:36:06.387688 starred_repo_finder-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-18 11:35:47.000000 starred_repo_finder-0.5.0/tests/test_starred_repo_finder.py
```

### Comparing `starred_repo_finder-0.4.0/LICENSE` & `starred_repo_finder-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starred_repo_finder-0.4.0/PKG-INFO` & `starred_repo_finder-0.5.0/starred_repo_finder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: starred_repo_finder
-Version: 0.4.0
+Name: starred-repo-finder
+Version: 0.5.0
 Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 Home-page: https://github.com/tylercb/starred_repo_finder
 Author: Tyler Hanway
 Author-email: hanway.tyler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -54,35 +54,43 @@
 
 ## Usage
 
 Command line usage:
 
 ```bash
 $ starred_repo_finder --help
-usage: starred_repo_finder [-h] [-l LIMIT] [-o {stargazers,forkers,ratio}] [-s STARGAZERS] [-f FORKERS] [-r RATIO]
+usage: starred_repo_finder [-h] [-l LIMIT]
+                           [-o {stargazers,forkers,ratio}]
+                           [-s STARGAZERS] [-f FORKERS] [-r RATIO]
                            [-fmt {table,csv,json,markdown}]
                            repo_name
 
 positional arguments:
   repo_name             The repository name like`<owner>/<repo>`
 
 options:
   -h, --help            show this help message and exit
   -l LIMIT, --limit LIMIT
-                        The maximum number of results to return (default: 100)
+                        The maximum number of results to return
+                        (default: 100)
   -o {stargazers,forkers,ratio}, --order {stargazers,forkers,ratio}
-                        Column to order by (default: stargazers). Options: stargazers, forkers, ratio
+                        Column to order by (default: stargazers).
+                        Options: stargazers, forkers, ratio
   -s STARGAZERS, --stargazers STARGAZERS
-                        Minimum number of stargazers to include (default: None)
+                        Minimum number of stargazers to include
+                        (default: None)
   -f FORKERS, --forkers FORKERS
-                        Minimum number of forkers to include (default: None)
+                        Minimum number of forkers to include
+                        (default: None)
   -r RATIO, --ratio RATIO
-                        Minimum ratio of stargazers to forkers to include (default: None)
+                        Minimum ratio of stargazers to forkers to
+                        include (default: None)
   -fmt {table,csv,json,markdown}, --format {table,csv,json,markdown}
-                        Output format (default: table). Options: table, csv, json, markdown
+                        Output format (default: table). Options:
+                        table, csv, json, markdown
 ```
 
 ## Examples
 
 #### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
 
 ```bash
```

### Comparing `starred_repo_finder-0.4.0/README.md` & `starred_repo_finder-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,35 +39,43 @@
 
 ## Usage
 
 Command line usage:
 
 ```bash
 $ starred_repo_finder --help
-usage: starred_repo_finder [-h] [-l LIMIT] [-o {stargazers,forkers,ratio}] [-s STARGAZERS] [-f FORKERS] [-r RATIO]
+usage: starred_repo_finder [-h] [-l LIMIT]
+                           [-o {stargazers,forkers,ratio}]
+                           [-s STARGAZERS] [-f FORKERS] [-r RATIO]
                            [-fmt {table,csv,json,markdown}]
                            repo_name
 
 positional arguments:
   repo_name             The repository name like`<owner>/<repo>`
 
 options:
   -h, --help            show this help message and exit
   -l LIMIT, --limit LIMIT
-                        The maximum number of results to return (default: 100)
+                        The maximum number of results to return
+                        (default: 100)
   -o {stargazers,forkers,ratio}, --order {stargazers,forkers,ratio}
-                        Column to order by (default: stargazers). Options: stargazers, forkers, ratio
+                        Column to order by (default: stargazers).
+                        Options: stargazers, forkers, ratio
   -s STARGAZERS, --stargazers STARGAZERS
-                        Minimum number of stargazers to include (default: None)
+                        Minimum number of stargazers to include
+                        (default: None)
   -f FORKERS, --forkers FORKERS
-                        Minimum number of forkers to include (default: None)
+                        Minimum number of forkers to include
+                        (default: None)
   -r RATIO, --ratio RATIO
-                        Minimum ratio of stargazers to forkers to include (default: None)
+                        Minimum ratio of stargazers to forkers to
+                        include (default: None)
   -fmt {table,csv,json,markdown}, --format {table,csv,json,markdown}
-                        Output format (default: table). Options: table, csv, json, markdown
+                        Output format (default: table). Options:
+                        table, csv, json, markdown
 ```
 
 ## Examples
 
 #### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
 
 ```bash
```

### Comparing `starred_repo_finder-0.4.0/setup.py` & `starred_repo_finder-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="starred_repo_finder",
-    version="0.4.0",
+    version="0.5.0",
     description="A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tylercb/starred_repo_finder",
     author="Tyler Hanway",
     author_email="hanway.tyler@gmail.com",
     license="MIT",
     packages=find_packages(),
     install_requires=[
-        "argparse",
+        "click",
         "requests",
         "rich",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `starred_repo_finder-0.4.0/starred_repo_finder/starred_repo_finder.py` & `starred_repo_finder-0.5.0/starred_repo_finder/starred_repo_finder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import requests
-import argparse
+import click
 import json
 from rich.console import Console
 from rich.table import Table
 
 console = Console()
 
 
@@ -183,72 +183,32 @@
 
     # Process the response
     results = process_response(response)
 
     # Print the results
     print_results(results, output_format)
 
-
-def main():
+@click.command()
+@click.argument('repo_name')
+@click.option('--limit', '-l', default=100, help='The maximum number of results to return (default: 100)', type=int)
+@click.option('--order', '-o', default='stargazers', help='Column to order by (default: stargazers). Options: stargazers, forkers, ratio', type=click.Choice(['stargazers', 'forkers', 'ratio'], case_sensitive=False))
+@click.option('--stargazers', '-s', default=None, help='Minimum number of stargazers to include (default: None)', type=int)
+@click.option('--forkers', '-f', default=None, help='Minimum number of forkers to include (default: None)', type=int)
+@click.option('--ratio', '-r', default=None, help='Minimum ratio of stargazers to forkers to include (default: None)', type=float)
+@click.option('--format', '-fmt', default='table', help='Output format (default: table). Options: table, csv, json, markdown', type=click.Choice(['table', 'csv', 'json', 'markdown'], case_sensitive=False))
+def main(repo_name, limit, order, stargazers, forkers, ratio, format):
     """
     Parse command line arguments
     """
-    parser = argparse.ArgumentParser()
-    parser.add_argument("repo_name", help="The repository name like`<owner>/<repo>`")
-    parser.add_argument(
-        "-l",
-        "--limit",
-        help="The maximum number of results to return (default: 100)",
-        default=100,
-        type=int,
-    )
-    parser.add_argument(
-        "-o",
-        "--order",
-        help="Column to order by (default: stargazers). Options: stargazers, forkers, ratio",
-        default="stargazers",
-        choices=["stargazers", "forkers", "ratio"],
-    )
-    parser.add_argument(
-        "-s",
-        "--stargazers",
-        help="Minimum number of stargazers to include (default: None)",
-        type=int,
-        default=None,
-    )
-    parser.add_argument(
-        "-f",
-        "--forkers",
-        help="Minimum number of forkers to include (default: None)",
-        type=int,
-        default=None,
-    )
-    parser.add_argument(
-        "-r",
-        "--ratio",
-        help="Minimum ratio of stargazers to forkers to include (default: None)",
-        type=float,
-        default=None,
-    )
-    parser.add_argument(
-        "-fmt",
-        "--format",
-        help="Output format (default: table). Options: table, csv, json, markdown",
-        default="table",
-        choices=["table", "csv", "json", "markdown"],
-    )
-    args = parser.parse_args()
-
-    # Run the script
     run(
-        args.repo_name,
-        args.limit,
-        args.order,
-        args.stargazers,
-        args.forkers,
-        args.ratio,
-        args.format,
+        repo_name,
+        limit,
+        order,
+        stargazers,
+        forkers,
+        ratio,
+        format,
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `starred_repo_finder-0.4.0/starred_repo_finder.egg-info/PKG-INFO` & `starred_repo_finder-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: starred-repo-finder
-Version: 0.4.0
+Name: starred_repo_finder
+Version: 0.5.0
 Summary: A simple command line tool to find and explore GitHub repositories through stargazers for a given repository.
 Home-page: https://github.com/tylercb/starred_repo_finder
 Author: Tyler Hanway
 Author-email: hanway.tyler@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -54,35 +54,43 @@
 
 ## Usage
 
 Command line usage:
 
 ```bash
 $ starred_repo_finder --help
-usage: starred_repo_finder [-h] [-l LIMIT] [-o {stargazers,forkers,ratio}] [-s STARGAZERS] [-f FORKERS] [-r RATIO]
+usage: starred_repo_finder [-h] [-l LIMIT]
+                           [-o {stargazers,forkers,ratio}]
+                           [-s STARGAZERS] [-f FORKERS] [-r RATIO]
                            [-fmt {table,csv,json,markdown}]
                            repo_name
 
 positional arguments:
   repo_name             The repository name like`<owner>/<repo>`
 
 options:
   -h, --help            show this help message and exit
   -l LIMIT, --limit LIMIT
-                        The maximum number of results to return (default: 100)
+                        The maximum number of results to return
+                        (default: 100)
   -o {stargazers,forkers,ratio}, --order {stargazers,forkers,ratio}
-                        Column to order by (default: stargazers). Options: stargazers, forkers, ratio
+                        Column to order by (default: stargazers).
+                        Options: stargazers, forkers, ratio
   -s STARGAZERS, --stargazers STARGAZERS
-                        Minimum number of stargazers to include (default: None)
+                        Minimum number of stargazers to include
+                        (default: None)
   -f FORKERS, --forkers FORKERS
-                        Minimum number of forkers to include (default: None)
+                        Minimum number of forkers to include
+                        (default: None)
   -r RATIO, --ratio RATIO
-                        Minimum ratio of stargazers to forkers to include (default: None)
+                        Minimum ratio of stargazers to forkers to
+                        include (default: None)
   -fmt {table,csv,json,markdown}, --format {table,csv,json,markdown}
-                        Output format (default: table). Options: table, csv, json, markdown
+                        Output format (default: table). Options:
+                        table, csv, json, markdown
 ```
 
 ## Examples
 
 #### Find the top 100 shared GitHub repositories by stars for stargazers of the `Elderjs/elderjs` repo:
 
 ```bash
```

### Comparing `starred_repo_finder-0.4.0/tests/test_starred_repo_finder.py` & `starred_repo_finder-0.5.0/tests/test_starred_repo_finder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 from unittest.mock import patch, Mock
+from click.testing import CliRunner
 from starred_repo_finder.starred_repo_finder import (
     build_query,
     make_request,
     process_response,
     print_results,
     run,
     convert_and_format_results,
@@ -87,34 +88,27 @@
         # action
         run("test_repo", 50, "stargazers", None, None, None, "table")
 
         # assert
         mock_request.assert_called_once()
         self.assertTrue(mock_print.called)
 
-    @patch("starred_repo_finder.starred_repo_finder.argparse.ArgumentParser.parse_args")
     @patch("starred_repo_finder.starred_repo_finder.run")
-    def test_main(self, mock_run, mock_parse_args):
-        # setup
-        mock_args = Mock()
-        mock_args.repo_name = "test_repo"
-        mock_args.limit = 50
-        mock_args.order = "stargazers"
-        mock_args.stargazers = None
-        mock_args.forkers = None
-        mock_args.ratio = None
-        mock_args.format = "table"
+    def test_main(self, mock_run):
+        runner = CliRunner()
 
-        mock_parse_args.return_value = mock_args
+        # setup
+        repo_name = "test_repo"
+        limit = 50
+        order = "stargazers"
+        format = "table"
 
         # action
-        main()
+        result = runner.invoke(main, [repo_name, '--limit', str(limit), '--order', order, '--format', format])
 
         # assert
-        mock_parse_args.assert_called_once()
-        mock_run.assert_called_once_with(
-            "test_repo", 50, "stargazers", None, None, None, "table"
-        )
+        self.assertEqual(result.exit_code, 0)
+        mock_run.assert_called_once_with(repo_name, limit, order, None, None, None, format)
 
 
 if __name__ == "__main__":
     unittest.main()
```

