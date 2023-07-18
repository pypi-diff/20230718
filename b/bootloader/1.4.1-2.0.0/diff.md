# Comparing `tmp/bootloader-1.4.1.tar.gz` & `tmp/bootloader-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootloader-1.4.1.tar", max compression
+gzip compressed data, was "bootloader-2.0.0.tar", max compression
```

## Comparing `bootloader-1.4.1.tar` & `bootloader-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,33 @@
--rw-r--r--   0        0        0     1068 2022-12-19 18:58:28.870281 bootloader-1.4.1/LICENSE
--rw-r--r--   0        0        0     3239 2023-03-13 20:24:21.945906 bootloader-1.4.1/README.md
--rw-r--r--   0        0        0       22 2023-04-14 21:16:53.726064 bootloader-1.4.1/bootloader/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 17:44:46.556517 bootloader-1.4.1/bootloader/commands/__init__.py
--rw-r--r--   0        0        0     6999 2023-04-14 21:09:57.642446 bootloader-1.4.1/bootloader/commands/flash_bt121.py
--rw-r--r--   0        0        0     8588 2023-04-14 21:09:57.642446 bootloader-1.4.1/bootloader/commands/flash_microcontroller.py
--rw-r--r--   0        0        0     8126 2023-04-14 21:16:18.417382 bootloader-1.4.1/bootloader/commands/init.py
--rw-r--r--   0        0        0     3767 2023-04-14 21:09:57.646446 bootloader-1.4.1/bootloader/commands/list.py
--rw-r--r--   0        0        0        0 2023-03-24 17:39:39.085470 bootloader-1.4.1/bootloader/console/__init__.py
--rw-r--r--   0        0        0     1305 2023-04-14 21:09:57.650446 bootloader-1.4.1/bootloader/console/application.py
--rw-r--r--   0        0        0      342 2023-03-24 17:39:50.209378 bootloader-1.4.1/bootloader/console/main.py
--rw-r--r--   0        0        0        0 2023-04-14 21:09:57.650446 bootloader-1.4.1/bootloader/exceptions/__init__.py
--rw-r--r--   0        0        0     3993 2023-04-14 21:09:57.650446 bootloader-1.4.1/bootloader/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-27 18:32:24.861693 bootloader-1.4.1/bootloader/utilities/__init__.py
--rw-r--r--   0        0        0     4222 2023-04-14 21:09:57.654446 bootloader-1.4.1/bootloader/utilities/aws.py
--rw-r--r--   0        0        0     1747 2023-04-14 21:09:57.654446 bootloader-1.4.1/bootloader/utilities/config.py
--rw-r--r--   0        0        0      606 2023-04-14 21:09:57.654446 bootloader-1.4.1/bootloader/utilities/logo.py
--rw-r--r--   0        0        0     2323 2023-04-14 21:09:57.658446 bootloader-1.4.1/bootloader/utilities/system_utils.py
--rw-r--r--   0        0        0      978 2023-04-14 21:16:42.421845 bootloader-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     3830 1970-01-01 00:00:00.000000 bootloader-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0      300 2023-07-18 21:53:55.201198 bootloader-2.0.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-18 21:53:55.201198 bootloader-2.0.0/bootloader/__init__.py
+-rw-r--r--   0        0        0     4027 2023-07-18 21:53:55.205198 bootloader-2.0.0/bootloader/application.py
+-rw-r--r--   0        0        0      379 2023-07-18 21:53:55.205198 bootloader-2.0.0/bootloader/command_list.py
+-rw-r--r--   0        0        0        0 2023-06-07 20:21:29.921164 bootloader-2.0.0/bootloader/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:53:55.205198 bootloader-2.0.0/bootloader/commands/config/__init__.py
+-rw-r--r--   0        0        0     6690 2023-07-18 21:53:55.205198 bootloader-2.0.0/bootloader/commands/config/create.py
+-rw-r--r--   0        0        0     2012 2023-07-18 21:53:55.205198 bootloader-2.0.0/bootloader/commands/config/download.py
+-rw-r--r--   0        0        0     1703 2023-07-18 21:53:55.205198 bootloader-2.0.0/bootloader/commands/config/upload.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:53:55.209198 bootloader-2.0.0/bootloader/commands/download/__init__.py
+-rw-r--r--   0        0        0     2041 2023-07-18 21:53:55.209198 bootloader-2.0.0/bootloader/commands/download/tools.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:53:55.209198 bootloader-2.0.0/bootloader/commands/flash/__init__.py
+-rw-r--r--   0        0        0     7199 2023-07-18 21:53:55.209198 bootloader-2.0.0/bootloader/commands/flash/all.py
+-rw-r--r--   0        0        0    10399 2023-07-18 21:53:55.209198 bootloader-2.0.0/bootloader/commands/flash/base_flash.py
+-rw-r--r--   0        0        0     4258 2023-07-18 21:53:55.209198 bootloader-2.0.0/bootloader/commands/flash/bt121.py
+-rw-r--r--   0        0        0     6033 2023-07-18 21:53:55.209198 bootloader-2.0.0/bootloader/commands/flash/config.py
+-rw-r--r--   0        0        0     1884 2023-07-18 21:53:55.213198 bootloader-2.0.0/bootloader/commands/flash/ex.py
+-rw-r--r--   0        0        0     2329 2023-07-18 21:53:55.213198 bootloader-2.0.0/bootloader/commands/flash/habs.py
+-rw-r--r--   0        0        0     2082 2023-07-18 21:53:55.213198 bootloader-2.0.0/bootloader/commands/flash/mn.py
+-rw-r--r--   0        0        0     1881 2023-07-18 21:53:55.213198 bootloader-2.0.0/bootloader/commands/flash/re.py
+-rw-r--r--   0        0        0     2026 2023-07-18 21:53:55.213198 bootloader-2.0.0/bootloader/commands/flash/xbee.py
+-rw-r--r--   0        0        0     1210 2023-07-18 21:53:55.213198 bootloader-2.0.0/bootloader/commands/logo.py
+-rw-r--r--   0        0        0        0 2023-07-18 21:53:55.213198 bootloader-2.0.0/bootloader/commands/show/__init__.py
+-rw-r--r--   0        0        0     1728 2023-07-18 21:53:55.217198 bootloader-2.0.0/bootloader/commands/show/configs.py
+-rw-r--r--   0        0        0        0 2023-06-16 18:38:13.989941 bootloader-2.0.0/bootloader/exceptions/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-18 21:53:55.217198 bootloader-2.0.0/bootloader/exceptions/exceptions.py
+-rw-r--r--   0        0        0      309 2023-07-18 21:53:55.217198 bootloader-2.0.0/bootloader/main.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:37:46.558725 bootloader-2.0.0/bootloader/utilities/__init__.py
+-rw-r--r--   0        0        0     4503 2023-07-18 21:53:55.217198 bootloader-2.0.0/bootloader/utilities/constants.py
+-rw-r--r--   0        0        0     2717 2023-07-18 21:53:55.221197 bootloader-2.0.0/bootloader/utilities/help.py
+-rw-r--r--   0        0        0     2193 2023-07-18 21:53:55.221197 bootloader-2.0.0/bootloader/utilities/system_utils.py
+-rw-r--r--   0        0        0     1039 2023-07-18 21:53:55.225197 bootloader-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      949 1970-01-01 00:00:00.000000 bootloader-2.0.0/PKG-INFO
```

### Comparing `bootloader-1.4.1/pyproject.toml` & `bootloader-2.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 [tool.poetry]
 name = "bootloader"
-version = "1.4.1"
+version = "2.0.0"
 description = "A tool for loading firmware onto Dephy devices."
 authors = ["Jared <jcoughlin@dephy.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-cleo = "^2.0.1"
-pyserial = "^3.5"
-boto3 = "^1.26.44"
+flexsea = "^11.0.6"
 semantic-version = "^2.10.0"
-flexsea = "^10"
+cleo = "^2.0.1"
+pendulum = "^2.1.2"
+pyyaml = "^6.0"
+cloudpathlib = {extras = ["s3"], version = "^0.15.1"}
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 pylint = "^2.15.9"
-mypy = "^0.991"
-nox = "^2022.11.21"
-pytest = "^7.2.0"
-ipython = "^8.8.0"
-wrapt = "^1.14.1"
-dill = "^0.3.6"
+pre-commit = "^3.3.3"
+nox = "^2023.4.22"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-bootload = 'bootloader.console.main:main'
+bootloader = 'bootloader.main:main'
 
 
 [tool.pylint.messages_control]
 max-line-length = 88
 disable = [
   "missing-docstring",
   "too-few-public-methods",
   "invalid-name",
+  "too-many-instance-attributes",
+  "protected-access",
+  "duplicate-code",
 ]
 
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
 include = '\.pyi?$'
```

