# Comparing `tmp/edc-protocol-0.3.8.tar.gz` & `tmp/edc-protocol-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-protocol-0.3.8.tar", last modified: Fri Oct  7 02:42:58 2022, max compression
+gzip compressed data, was "edc-protocol-0.3.9.tar", last modified: Wed May 24 16:54:42 2023, max compression
```

## Comparing `edc-protocol-0.3.8.tar` & `edc-protocol-0.3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.439464 edc-protocol-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       95 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 01:23:09.000000 edc-protocol-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.431947 edc-protocol-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.435218 edc-protocol-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 00:37:20.000000 edc-protocol-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      969 2022-06-04 21:23:22.000000 edc-protocol-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1040 2022-10-07 02:42:50.000000 edc-protocol-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:37:20.000000 edc-protocol-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-04 21:23:22.000000 edc-protocol-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-04 21:23:22.000000 edc-protocol-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:13:12.000000 edc-protocol-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      117 2022-06-04 21:23:22.000000 edc-protocol-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1628 2022-10-07 02:42:58.439574 edc-protocol-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      650 2021-02-08 01:23:09.000000 edc-protocol-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-07 02:42:51.000000 edc-protocol-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:37:20.000000 edc-protocol-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.436979 edc-protocol-0.3.8/edc_protocol/
--rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-10-07 02:42:50.000000 edc-protocol-0.3.8/edc_protocol/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      704 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/address.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1078 2022-10-07 02:42:50.000000 edc-protocol-0.3.8/edc_protocol/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      730 2022-10-07 02:42:50.000000 edc-protocol-0.3.8/edc_protocol/middleware.py
--rw-r--r--   0 erikvw     (501) staff       (20)      343 2021-02-08 01:23:09.000000 edc-protocol-0.3.8/edc_protocol/navbars.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4124 2022-08-12 00:10:28.000000 edc-protocol-0.3.8/edc_protocol/protocol.py
--rw-r--r--   0 erikvw     (501) staff       (20)      394 2022-10-07 02:42:50.000000 edc-protocol-0.3.8/edc_protocol/system_checks.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.432161 edc-protocol-0.3.8/edc_protocol/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.432201 edc-protocol-0.3.8/edc_protocol/templates/edc_protocol/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.437821 edc-protocol-0.3.8/edc_protocol/templates/edc_protocol/bootstrap3/
--rw-r--r--   0 erikvw     (501) staff       (20)     1926 2022-08-10 00:37:20.000000 edc-protocol-0.3.8/edc_protocol/templates/edc_protocol/bootstrap3/home.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.438340 edc-protocol-0.3.8/edc_protocol/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.439345 edc-protocol-0.3.8/edc_protocol/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      681 2022-06-04 21:23:22.000000 edc-protocol-0.3.8/edc_protocol/tests/tests.py
--rw-r--r--   0 erikvw     (501) staff       (20)      252 2021-02-08 01:23:09.000000 edc-protocol-0.3.8/edc_protocol/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      153 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1317 2022-08-10 00:37:20.000000 edc-protocol-0.3.8/edc_protocol/validators.py
--rw-r--r--   0 erikvw     (501) staff       (20)      564 2021-02-08 01:23:09.000000 edc-protocol-0.3.8/edc_protocol/view_mixins.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1020 2022-06-23 21:59:56.000000 edc-protocol-0.3.8/edc_protocol/views.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-10-07 02:42:58.437721 edc-protocol-0.3.8/edc_protocol.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1628 2022-10-07 02:42:58.000000 edc-protocol-0.3.8/edc_protocol.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1186 2022-10-07 02:42:58.000000 edc-protocol-0.3.8/edc_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-10-07 02:42:58.000000 edc-protocol-0.3.8/edc_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:14:00.000000 edc-protocol-0.3.8/edc_protocol.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       13 2022-10-07 02:42:58.000000 edc-protocol-0.3.8/edc_protocol.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1727 2022-08-10 00:37:20.000000 edc-protocol-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1684 2022-06-04 21:23:22.000000 edc-protocol-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1242 2022-10-07 02:42:58.440047 edc-protocol-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.298771 edc-protocol-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       95 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 01:23:09.000000 edc-protocol-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.290329 edc-protocol-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.294295 edc-protocol-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2021 2023-05-24 16:54:33.000000 edc-protocol-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      969 2022-06-04 21:23:22.000000 edc-protocol-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1077 2023-05-24 16:54:33.000000 edc-protocol-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 00:37:20.000000 edc-protocol-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-04 21:23:22.000000 edc-protocol-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-04 21:23:22.000000 edc-protocol-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35141 2020-03-04 23:13:12.000000 edc-protocol-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      117 2022-06-04 21:23:22.000000 edc-protocol-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1502 2023-05-24 16:54:42.298862 edc-protocol-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      650 2021-02-08 01:23:09.000000 edc-protocol-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-10-07 02:42:51.000000 edc-protocol-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 00:37:20.000000 edc-protocol-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.296119 edc-protocol-0.3.9/edc_protocol/
+-rw-r--r--   0 erikvw     (501) staff       (20)      295 2022-10-07 02:42:50.000000 edc-protocol-0.3.9/edc_protocol/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      704 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/address.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1078 2022-10-07 02:42:50.000000 edc-protocol-0.3.9/edc_protocol/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      730 2022-10-07 02:42:50.000000 edc-protocol-0.3.9/edc_protocol/middleware.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      343 2021-02-08 01:23:09.000000 edc-protocol-0.3.9/edc_protocol/navbars.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4124 2022-08-12 00:10:28.000000 edc-protocol-0.3.9/edc_protocol/protocol.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      394 2022-10-07 02:42:50.000000 edc-protocol-0.3.9/edc_protocol/system_checks.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.290595 edc-protocol-0.3.9/edc_protocol/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.290642 edc-protocol-0.3.9/edc_protocol/templates/edc_protocol/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.296987 edc-protocol-0.3.9/edc_protocol/templates/edc_protocol/bootstrap3/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1926 2022-08-10 00:37:20.000000 edc-protocol-0.3.9/edc_protocol/templates/edc_protocol/bootstrap3/home.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.297445 edc-protocol-0.3.9/edc_protocol/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.298630 edc-protocol-0.3.9/edc_protocol/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      681 2022-06-04 21:23:22.000000 edc-protocol-0.3.9/edc_protocol/tests/tests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      252 2021-02-08 01:23:09.000000 edc-protocol-0.3.9/edc_protocol/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      153 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1317 2022-08-10 00:37:20.000000 edc-protocol-0.3.9/edc_protocol/validators.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      564 2021-02-08 01:23:09.000000 edc-protocol-0.3.9/edc_protocol/view_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1020 2022-06-23 21:59:56.000000 edc-protocol-0.3.9/edc_protocol/views.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 16:54:42.296873 edc-protocol-0.3.9/edc_protocol.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1502 2023-05-24 16:54:42.000000 edc-protocol-0.3.9/edc_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1186 2023-05-24 16:54:42.000000 edc-protocol-0.3.9/edc_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 16:54:42.000000 edc-protocol-0.3.9/edc_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:14:00.000000 edc-protocol-0.3.9/edc_protocol.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       13 2023-05-24 16:54:42.000000 edc-protocol-0.3.9/edc_protocol.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1770 2023-05-24 16:54:33.000000 edc-protocol-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1684 2022-06-04 21:23:22.000000 edc-protocol-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1149 2023-05-24 16:54:42.299154 edc-protocol-0.3.9/setup.cfg
```

### Comparing `edc-protocol-0.3.8/.github/workflows/build.yml` & `edc-protocol-0.3.9/.github/workflows/build.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,20 @@
   build:
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.9', '3.10']
-        django-version: ['3.2', '4.0', '4.1', 'dev']
-
+        python-version: ['3.10', '3.11']
+        django-version: ['4.1', '4.2', 'dev']
+        exclude:
+          - python-version: '3.10'
+            django-version: 'dev'
     services:
-
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
           MYSQL_ROOT_PASSWORD: mysql
         ports:
           - 3306:3306
@@ -28,28 +29,27 @@
     steps:
       - name: Install pycups and words dependency
         run: |
           sudo sed -i 's/azure\.//' /etc/apt/sources.list
           sudo apt-get -y update
           sudo apt-get install libcups2-dev wamerican
 
-      - uses: actions/checkout@v2
-
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Get pip cache dir
         id: pip-cache
         run: |
-          echo "::set-output name=dir::$(pip cache dir)"
+          echo "dir=$(pip cache dir)" >>$GITHUB_OUTPUT
 
       - name: Cache
-        uses: actions/cache@v2
+        uses: actions/cache@v3
         with:
           path: ${{ steps.pip-cache.outputs.dir }}
           key:
             ${{ matrix.python-version }}-v1-${{ hashFiles('**/setup.py') }}-${{ hashFiles('**/tox.ini') }}
           restore-keys: |
             ${{ matrix.python-version }}-v1-
 
@@ -61,11 +61,11 @@
 
       - name: Tox tests
         run: |
           tox -v
         env:
           DJANGO: ${{ matrix.django-version }}
 
-      - name: Upload coverage
-        uses: codecov/codecov-action@v1
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
         with:
           name: Python ${{ matrix.python-version }}
```

### Comparing `edc-protocol-0.3.8/.gitignore` & `edc-protocol-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/.pre-commit-config.yaml` & `edc-protocol-0.3.9/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 ---
 exclude: tests/etc/user-*
 
 repos:
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
+        language_version: python3.10
 
   - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: requirements-txt-fixer
         files: requirements/.*\.txt$
       - id: trailing-whitespace
       - id: check-added-large-files
       - id: fix-byte-order-marker
       - id: check-docstring-first
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
       - id: detect-private-key
 
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.27.1
+    rev: v1.31.0
     hooks:
       - id: yamllint
         args:
           - "--strict"
```

### Comparing `edc-protocol-0.3.8/LICENSE` & `edc-protocol-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/PKG-INFO` & `edc-protocol-0.3.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-protocol
-Version: 0.3.8
+Version: 0.3.9
 Summary: Protocol specific variables for clinicedc/edc
 Home-page: https://github.com/clinicedc/edc-protocol
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |coverage|
 
 edc-protocol
```

### Comparing `edc-protocol-0.3.8/README.rst` & `edc-protocol-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/address.py` & `edc-protocol-0.3.9/edc_protocol/address.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/apps.py` & `edc-protocol-0.3.9/edc_protocol/apps.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/middleware.py` & `edc-protocol-0.3.9/edc_protocol/middleware.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/protocol.py` & `edc-protocol-0.3.9/edc_protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/templates/edc_protocol/bootstrap3/home.html` & `edc-protocol-0.3.9/edc_protocol/templates/edc_protocol/bootstrap3/home.html`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/tests/etc/user-rsa-local-private.pem` & `edc-protocol-0.3.9/edc_protocol/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/tests/etc/user-rsa-restricted-private.pem` & `edc-protocol-0.3.9/edc_protocol/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/tests/tests.py` & `edc-protocol-0.3.9/edc_protocol/tests/tests.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/validators.py` & `edc-protocol-0.3.9/edc_protocol/validators.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/view_mixins.py` & `edc-protocol-0.3.9/edc_protocol/view_mixins.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol/views.py` & `edc-protocol-0.3.9/edc_protocol/views.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/edc_protocol.egg-info/PKG-INFO` & `edc-protocol-0.3.9/edc_protocol.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 Metadata-Version: 2.1
 Name: edc-protocol
-Version: 0.3.8
+Version: 0.3.9
 Summary: Protocol specific variables for clinicedc/edc
 Home-page: https://github.com/clinicedc/edc-protocol
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc protocol,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 
 |pypi| |actions| |coverage|
 
 edc-protocol
```

### Comparing `edc-protocol-0.3.8/edc_protocol.egg-info/SOURCES.txt` & `edc-protocol-0.3.9/edc_protocol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/pyproject.toml` & `edc-protocol-0.3.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,70 +3,72 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "_version.py"
 
 [tool.black]
 line-length = 95
-target-version = ["py39"]
+target-version = ["py310"]
 extend-exclude = '''^(.*\/)*\b(migrations)\b($|\/.*$)'''
 
 [tool.isort]
 profile = "black"
-py_version = "39"
+py_version = "310"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
 parallel = false
 branch = true
 source = ["edc_protocol"]
 
 [tool.coverage.paths]
 source = ["edc_protocol"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 omit = ["requirements.txt"]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{38,39,310}-dj{32,40,41,dev},
+    py{310}-dj{41,42},
+    py{311}-dj{41,42,dev},
     lint
 
 isolated_build = true
 
 [gh-actions]
 python =
-    3.8: py38
-    3.9: py39, lint
     3.10: py310
+    3.11: py311, lint
 
 [gh-actions:env]
 DJANGO =
-    3.2: dj32, lint
-    4.0: dj40
     4.1: dj41
+    4.2: dj42, lint
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
-    dj32: Django>=3.2,<3.3
-    dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
+    dj42: Django>=4.2,<5.0
     djdev: https://github.com/django/django/tarball/main
 
 commands =
-    pip install -U pip
+    pip install -U pip coverage[toml]
     pip --version
     pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
```

### Comparing `edc-protocol-0.3.8/runtests.py` & `edc-protocol-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-protocol-0.3.8/setup.cfg` & `edc-protocol-0.3.9/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -8,27 +8,24 @@
 description = Protocol specific variables for clinicedc/edc
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = django Edc protocol, clinicedc, clinical trials
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
-	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 
 [options]
-python_requires = >=3.9
+python_requires = >=3.10
 zip_safe = False
 include_package_data = True
 packages = find:
 
 [options.packages.find]
 exclude = 
 	examples*
```

