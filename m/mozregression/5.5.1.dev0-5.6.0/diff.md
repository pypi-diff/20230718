# Comparing `tmp/mozregression-5.5.1.dev0.tar.gz` & `tmp/mozregression-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozregression-5.5.1.dev0.tar", last modified: Fri Jul 14 12:27:49 2023, max compression
+gzip compressed data, was "mozregression-5.6.0.tar", last modified: Tue Jul 18 16:05:14 2023, max compression
```

## Comparing `mozregression-5.5.1.dev0.tar` & `mozregression-5.6.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:27:49.272857 mozregression-5.5.1.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.coveralls.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:27:49.264857 mozregression-5.5.1.dev0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:27:49.264857 mozregression-5.5.1.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.github/workflows/compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.github/workflows/deploy-gui.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.github/workflows/glean-probe-scraper.yml
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/.github/workflows/run-compile-requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-14 12:27:49.268857 mozregression-5.5.1.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:27:49.268857 mozregression-5.5.1.dev0/mozregression/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/approx_persist.py
--rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/bisector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/bugzilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/build_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/class_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23201 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/download_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/fetch_build_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/fetch_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/json_pushes.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/mach_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/persist_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/pings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/releases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/tc_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/tempdir.py
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/mozregression/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-14 12:27:49.000000 mozregression-5.5.1.dev0/mozregression/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:27:49.268857 mozregression-5.5.1.dev0/mozregression.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-14 12:27:49.000000 mozregression-5.5.1.dev0/mozregression.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-14 12:27:49.000000 mozregression-5.5.1.dev0/mozregression.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:27:49.000000 mozregression-5.5.1.dev0/mozregression.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 12:27:49.000000 mozregression-5.5.1.dev0/mozregression.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-14 12:27:49.000000 mozregression-5.5.1.dev0/mozregression.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 12:27:49.000000 mozregression-5.5.1.dev0/mozregression.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:27:49.272857 mozregression-5.5.1.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-14 12:26:46.000000 mozregression-5.5.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:05:14.748016 mozregression-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 16:04:17.000000 mozregression-5.6.0/.coveralls.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:05:14.740016 mozregression-5.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-18 16:04:17.000000 mozregression-5.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:05:14.740016 mozregression-5.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-18 16:04:17.000000 mozregression-5.6.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-07-18 16:04:17.000000 mozregression-5.6.0/.github/workflows/compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-18 16:04:17.000000 mozregression-5.6.0/.github/workflows/deploy-gui.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-07-18 16:04:17.000000 mozregression-5.6.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-18 16:04:17.000000 mozregression-5.6.0/.github/workflows/glean-probe-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-18 16:04:17.000000 mozregression-5.6.0/.github/workflows/run-compile-requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16726 2023-07-18 16:04:17.000000 mozregression-5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-18 16:04:17.000000 mozregression-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 16:05:14.748016 mozregression-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-07-18 16:04:17.000000 mozregression-5.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:05:14.744016 mozregression-5.6.0/mozregression/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/approx_persist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25458 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/bisector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/bugzilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/build_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23215 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/download_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11133 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/fetch_build_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21686 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/fetch_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/json_pushes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/mach_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/persist_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/pings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/releases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/tc_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/tempdir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-18 16:04:17.000000 mozregression-5.6.0/mozregression/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 16:05:14.000000 mozregression-5.6.0/mozregression/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 16:05:14.748016 mozregression-5.6.0/mozregression.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 16:05:14.000000 mozregression-5.6.0/mozregression.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-18 16:05:14.000000 mozregression-5.6.0/mozregression.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 16:05:14.000000 mozregression-5.6.0/mozregression.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 16:05:14.000000 mozregression-5.6.0/mozregression.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-18 16:05:14.000000 mozregression-5.6.0/mozregression.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 16:05:14.000000 mozregression-5.6.0/mozregression.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 16:04:17.000000 mozregression-5.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 16:05:14.748016 mozregression-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-18 16:04:17.000000 mozregression-5.6.0/setup.py
```

### Comparing `mozregression-5.5.1.dev0/.github/workflows/build.yml` & `mozregression-5.6.0/.github/workflows/build.yml`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     env:
       GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
     strategy:
       matrix:
         os:
           - ubuntu-20.04
           - ubuntu-22.04
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v2
       - name: setup
         run: |
           sudo apt-get update
           sudo apt-get install libegl-dev -y
       - name: Set up Python ${{ matrix.python-version }}
@@ -55,14 +55,33 @@
           python -m pip install -e .
       - name: Test
         run: |
           source env/bin/activate
           coverage run -m pytest tests
           coveralls --service=github
 
+  build-and-test-windows-cli:
+    runs-on: windows-latest
+    env:
+      GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+    steps:
+      - uses: actions/checkout@v2
+        with:
+          persist-credentials: false
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: "3.11"
+      - name: Install dependencies and run tests
+        run: |
+          python -m pip install --upgrade pip
+          python -m pip install -r requirements/requirements-3.11-Windows.txt
+          python -m pip install -e .
+          python -m pytest tests
+
   build-and-test-linux-gui:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os:
           - ubuntu-20.04
           - ubuntu-22.04
```

### Comparing `mozregression-5.5.1.dev0/.github/workflows/compile-requirements.yml` & `mozregression-5.6.0/.github/workflows/compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/.github/workflows/deploy-gui.yml` & `mozregression-5.6.0/.github/workflows/deploy-gui.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/.github/workflows/deploy.yml` & `mozregression-5.6.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/.github/workflows/run-compile-requirements.yml` & `mozregression-5.6.0/.github/workflows/run-compile-requirements.yml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/LICENSE` & `mozregression-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/PKG-INFO` & `mozregression-5.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.5.1.dev0
+Version: 5.6.0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Regression range finder for Mozilla nightly builds.
 For more information see the mozregression website:
 http://mozilla.github.io/mozregression/
```

### Comparing `mozregression-5.5.1.dev0/README.md` & `mozregression-5.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/approx_persist.py` & `mozregression-5.6.0/mozregression/approx_persist.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/bisector.py` & `mozregression-5.6.0/mozregression/bisector.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/branches.py` & `mozregression-5.6.0/mozregression/branches.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/bugzilla.py` & `mozregression-5.6.0/mozregression/bugzilla.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/build_info.py` & `mozregression-5.6.0/mozregression/build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/build_range.py` & `mozregression-5.6.0/mozregression/build_range.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/class_registry.py` & `mozregression-5.6.0/mozregression/class_registry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/cli.py` & `mozregression-5.6.0/mozregression/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,17 +272,17 @@
             " x86_64 boxes). Default: %s bits." % defaults["bits"]
             or mozinfo.bits
         ),
     )
 
     parser.add_argument(
         "--arch",
-        choices=("arm", "x86_64"),
+        choices=("arm", "x86_64", "aarch64"),
         default=None,
-        help=("Force x86_64 build (only applies to GVE app). Default: arm"),
+        help=("Force alternate build (only applies to GVE app). Default: arm"),
     )
 
     parser.add_argument(
         "-c",
         "--command",
         help=(
             "Test command to evaluate builds automatically."
```

### Comparing `mozregression-5.5.1.dev0/mozregression/config.py` & `mozregression-5.6.0/mozregression/config.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/dates.py` & `mozregression-5.6.0/mozregression/dates.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/download_manager.py` & `mozregression-5.6.0/mozregression/download_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,43 +145,63 @@
 
     def get_url(self):
         """
         Returns the url.
         """
         return self.__url
 
+    @staticmethod
+    def get_total_size(headers):
+        """
+        Returns content length (integer) from response headers, if available.
+
+        :param headers: A :class:`requests.structures.CaseInsensitiveDict` object
+                        representing response headers.
+        """
+        for header in ["content-length", "x-goog-stored-content-length"]:
+            if header in headers:
+                total_size = int(headers[header])
+                break
+        else:
+            total_size = 0
+        return total_size
+
     def _update_progress(self, current, total):
         with self._lock:
             if self.__progress:
                 self.__progress(self, current, total)
 
     def _download(self, url, dest, finished_callback, chunk_size, session):
         # save the file under a temporary name
         # this allow to not use a broken file in case things went really bad
         # while downloading the file (ie the python interpreter is killed
         # abruptly)
         temp = None
         bytes_so_far = 0
         try:
             with closing(session.get(url, stream=True)) as response:
-                total_size = int(response.headers["Content-length"].strip())
-                self._update_progress(bytes_so_far, total_size)
+                # GCP storage does not always return a content-length header, check alternates.
+                total_size = self.get_total_size(response.headers)
+
+                if total_size:
+                    self._update_progress(bytes_so_far, total_size)
                 # we use NamedTemporaryFile as raw open() call was causing
                 # issues on windows - see:
                 # https://bugzilla.mozilla.org/show_bug.cgi?id=1185756
                 with tempfile.NamedTemporaryFile(
                     delete=False, mode="wb", suffix=".tmp", dir=os.path.dirname(dest)
                 ) as temp:
                     for chunk in response.iter_content(chunk_size):
                         if self.is_canceled():
                             break
                         if chunk:
                             temp.write(chunk)
                         bytes_so_far += len(chunk)
-                        self._update_progress(bytes_so_far, total_size)
+                        if total_size:
+                            self._update_progress(bytes_so_far, total_size)
             response.raise_for_status()
         except Exception:
             self.__error = sys.exc_info()
         try:
             if temp is None:
                 pass  # not even opened the temp file, nothing to do
             elif self.is_canceled() or self.__error:
```

### Comparing `mozregression-5.5.1.dev0/mozregression/errors.py` & `mozregression-5.6.0/mozregression/errors.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/fetch_build_info.py` & `mozregression-5.6.0/mozregression/fetch_build_info.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/fetch_configs.py` & `mozregression-5.6.0/mozregression/fetch_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -621,19 +621,21 @@
     def build_info_regex(self):
         return r"(target|fennec-.*)\.txt"
 
     def available_bits(self):
         return ()
 
     def available_archs(self):
-        return ["arm", "x86_64"]
+        return ["arm", "x86_64", "aarch64"]
 
     def set_arch(self, arch):
         CommonConfig.set_arch(self, arch)
-        if arch == "x86_64":
+        if arch == "aarch64":
+            self.tk_name = "android-aarch64"
+        elif arch == "x86_64":
             self.tk_name = "android-x86_64"
         else:
             self.tk_name = "android-api-11"
 
     def should_use_archive(self):
         # GVE is not on archive.mozilla.org, only on taskcluster
         return False
```

### Comparing `mozregression-5.5.1.dev0/mozregression/history.py` & `mozregression-5.6.0/mozregression/history.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/json_pushes.py` & `mozregression-5.6.0/mozregression/json_pushes.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/launchers.py` & `mozregression-5.6.0/mozregression/launchers.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/log.py` & `mozregression-5.6.0/mozregression/log.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/mach_interface.py` & `mozregression-5.6.0/mozregression/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/main.py` & `mozregression-5.6.0/mozregression/main.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/metrics.yaml` & `mozregression-5.6.0/mozregression/metrics.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/network.py` & `mozregression-5.6.0/mozregression/network.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/persist_limit.py` & `mozregression-5.6.0/mozregression/persist_limit.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/pings.yaml` & `mozregression-5.6.0/mozregression/pings.yaml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/releases.py` & `mozregression-5.6.0/mozregression/releases.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/tc_authenticate.py` & `mozregression-5.6.0/mozregression/tc_authenticate.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/telemetry.py` & `mozregression-5.6.0/mozregression/telemetry.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/tempdir.py` & `mozregression-5.6.0/mozregression/tempdir.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression/test_runner.py` & `mozregression-5.6.0/mozregression/test_runner.py`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/mozregression.egg-info/PKG-INFO` & `mozregression-5.6.0/mozregression.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mozregression
-Version: 5.5.1.dev0
+Version: 5.6.0
 Summary: Regression range finder for Mozilla nightly builds
 Home-page: http://github.com/mozilla/mozregression
 Author: Mozilla Automation and Tools Team
 Author-email: tools@lists.mozilla.org
 License: MPL 2.0
 Platform: Any
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 License-File: LICENSE
 
 Regression range finder for Mozilla nightly builds.
 For more information see the mozregression website:
 http://mozilla.github.io/mozregression/
```

### Comparing `mozregression-5.5.1.dev0/mozregression.egg-info/SOURCES.txt` & `mozregression-5.6.0/mozregression.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/pyproject.toml` & `mozregression-5.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mozregression-5.5.1.dev0/setup.py` & `mozregression-5.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "configobj>=5.0.6",
     "distro>=1.8.0",
     "mozdevice>=4.1.0,<5",
     "mozfile>=2.0.0",
     "mozinfo>=1.1.0",
     "mozinstall>=2.0.0",
     "mozlog>=4.0",
-    "mozprocess>=1.2.0",
+    "mozprocess>=1.3.1",
     "mozprofile>=2.2.0",
     "mozrunner>=8.0.2",
     "mozversion>=2.1.0",
     "redo>=2.0.2",
     "requests>=2.21.0",
     "taskcluster>=6.0.0",
 ]
@@ -48,13 +48,14 @@
     install_requires=DEPENDENCIES,
     classifiers=[
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
 )
```

