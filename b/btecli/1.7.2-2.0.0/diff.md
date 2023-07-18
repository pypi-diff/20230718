# Comparing `tmp/btecli-1.7.2.tar.gz` & `tmp/btecli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btecli-1.7.2.tar", last modified: Mon May 15 00:17:25 2023, max compression
+gzip compressed data, was "btecli-2.0.0.tar", last modified: Tue Jul 18 21:13:15 2023, max compression
```

## Comparing `btecli-1.7.2.tar` & `btecli-2.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.472223 btecli-1.7.2/
--rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-1.7.2/.gitignore
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/HISTORY.md
--rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-1.7.2/LICENSE
--rw-r--r--   0 etejeda    (501) staff       (20)     8647 2023-05-15 00:17:25.472575 btecli-1.7.2/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-1.7.2/README.md
--rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-05-15 00:14:22.000000 btecli-1.7.2/VERSION.txt
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.456904 btecli-1.7.2/btecli/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)    11075 2023-05-15 00:12:09.000000 btecli-1.7.2/btecli/cli.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.459812 btecli-1.7.2/btecli/lib/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.461053 btecli-1.7.2/btecli/lib/cryptography/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/cryptography/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/cryptography/aes.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/cryptography/wincred.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.461778 btecli-1.7.2/btecli/lib/defaults/
--rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/defaults/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.462301 btecli-1.7.2/btecli/lib/dictutils/
--rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-1.7.2/btecli/lib/dictutils/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.462707 btecli-1.7.2/btecli/lib/formatting/
--rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/formatting/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.463953 btecli-1.7.2/btecli/lib/input/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/input/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/input/streams.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.464581 btecli-1.7.2/btecli/lib/logger/
--rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/logger/__init__.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.465759 btecli-1.7.2/btecli/lib/options/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/options/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/options/mexclusive.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.468006 btecli-1.7.2/btecli/lib/plugin/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/plugin/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     3251 2023-05-12 18:51:57.000000 btecli-1.7.2/btecli/lib/plugin/finder.py
--rw-r--r--   0 etejeda    (501) staff       (20)     2013 2023-05-12 18:51:56.000000 btecli-1.7.2/btecli/lib/plugin/metadata.py
--rw-r--r--   0 etejeda    (501) staff       (20)     7626 2023-05-12 18:51:58.000000 btecli-1.7.2/btecli/lib/plugin/plugins.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.469077 btecli-1.7.2/btecli/lib/proc/
--rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/proc/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)     5064 2023-05-15 00:01:43.000000 btecli-1.7.2/btecli/lib/proc/local_invocation.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.470953 btecli-1.7.2/btecli/lib/shell/
--rw-r--r--   0 etejeda    (501) staff       (20)     2455 2023-05-12 18:51:54.000000 btecli-1.7.2/btecli/lib/shell/__init__.py
--rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/shell/bash_init.py
--rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-1.7.2/btecli/lib/shell/which.py
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.459431 btecli-1.7.2/btecli.egg-info/
--rw-r--r--   0 etejeda    (501) staff       (20)     8647 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/PKG-INFO
--rw-r--r--   0 etejeda    (501) staff       (20)     1027 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/SOURCES.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/dependency_links.txt
--rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/entry_points.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-05-15 00:15:16.000000 btecli-1.7.2/btecli.egg-info/not-zip-safe
--rw-r--r--   0 etejeda    (501) staff       (20)      375 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/requires.txt
--rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-05-15 00:17:25.000000 btecli-1.7.2/btecli.egg-info/top_level.txt
--rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-1.7.2/ecli.config.yaml.example
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.451713 btecli-1.7.2/resources/
-drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-05-15 00:17:25.471480 btecli-1.7.2/resources/icons/
--rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-1.7.2/resources/icons/admin.ico
--rw-r--r--   0 etejeda    (501) staff       (20)     1666 2023-05-15 00:17:25.474036 btecli-1.7.2/setup.cfg
--rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-1.7.2/setup.iss
--rw-r--r--   0 etejeda    (501) staff       (20)      810 2023-05-15 00:04:01.000000 btecli-1.7.2/setup.py
--rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 21:09:15.000000 btecli-1.7.2/version.rc
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.895379 btecli-2.0.0/
+-rw-r--r--   0 etejeda    (501) staff       (20)     1312 2023-05-10 18:51:52.000000 btecli-2.0.0/.gitignore
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/HISTORY.md
+-rw-r--r--   0 etejeda    (501) staff       (20)    35149 2023-05-10 17:31:13.000000 btecli-2.0.0/LICENSE
+-rw-r--r--   0 etejeda    (501) staff       (20)     8647 2023-07-18 21:13:15.895678 btecli-2.0.0/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     7703 2023-05-11 11:59:50.000000 btecli-2.0.0/README.md
+-rw-r--r--   0 etejeda    (501) staff       (20)        5 2023-07-18 20:58:49.000000 btecli-2.0.0/VERSION.txt
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.876697 btecli-2.0.0/btecli/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)    10405 2023-07-18 20:52:20.000000 btecli-2.0.0/btecli/cli.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.882012 btecli-2.0.0/btecli/lib/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.883361 btecli-2.0.0/btecli/lib/cryptography/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/cryptography/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     4586 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/cryptography/aes.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1837 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/cryptography/wincred.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.883960 btecli-2.0.0/btecli/lib/defaults/
+-rw-r--r--   0 etejeda    (501) staff       (20)      413 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/defaults/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.884641 btecli-2.0.0/btecli/lib/dictutils/
+-rw-r--r--   0 etejeda    (501) staff       (20)      424 2023-05-11 01:14:27.000000 btecli-2.0.0/btecli/lib/dictutils/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.885739 btecli-2.0.0/btecli/lib/formatting/
+-rw-r--r--   0 etejeda    (501) staff       (20)      651 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/formatting/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.886643 btecli-2.0.0/btecli/lib/input/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/input/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      272 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/input/streams.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.887150 btecli-2.0.0/btecli/lib/logger/
+-rw-r--r--   0 etejeda    (501) staff       (20)      660 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/logger/__init__.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.888063 btecli-2.0.0/btecli/lib/options/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/options/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     1140 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/options/mexclusive.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.890881 btecli-2.0.0/btecli/lib/plugin/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/plugin/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     3251 2023-05-12 18:51:57.000000 btecli-2.0.0/btecli/lib/plugin/finder.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     2013 2023-05-12 18:51:56.000000 btecli-2.0.0/btecli/lib/plugin/metadata.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     7626 2023-05-12 18:51:58.000000 btecli-2.0.0/btecli/lib/plugin/plugins.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.891875 btecli-2.0.0/btecli/lib/proc/
+-rw-r--r--   0 etejeda    (501) staff       (20)        0 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/proc/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)     5064 2023-05-15 00:01:43.000000 btecli-2.0.0/btecli/lib/proc/local_invocation.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.894044 btecli-2.0.0/btecli/lib/shell/
+-rw-r--r--   0 etejeda    (501) staff       (20)     2455 2023-05-12 18:51:54.000000 btecli-2.0.0/btecli/lib/shell/__init__.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      129 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/shell/bash_init.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      836 2023-05-10 17:31:13.000000 btecli-2.0.0/btecli/lib/shell/which.py
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.881220 btecli-2.0.0/btecli.egg-info/
+-rw-r--r--   0 etejeda    (501) staff       (20)     8647 2023-07-18 21:13:15.000000 btecli-2.0.0/btecli.egg-info/PKG-INFO
+-rw-r--r--   0 etejeda    (501) staff       (20)     1027 2023-07-18 21:13:15.000000 btecli-2.0.0/btecli.egg-info/SOURCES.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-18 21:13:15.000000 btecli-2.0.0/btecli.egg-info/dependency_links.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)       40 2023-07-18 21:13:15.000000 btecli-2.0.0/btecli.egg-info/entry_points.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        1 2023-07-18 21:13:15.000000 btecli-2.0.0/btecli.egg-info/not-zip-safe
+-rw-r--r--   0 etejeda    (501) staff       (20)      375 2023-07-18 21:13:15.000000 btecli-2.0.0/btecli.egg-info/requires.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)        7 2023-07-18 21:13:15.000000 btecli-2.0.0/btecli.egg-info/top_level.txt
+-rw-r--r--   0 etejeda    (501) staff       (20)      259 2023-05-10 17:31:13.000000 btecli-2.0.0/ecli.config.yaml.example
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.863000 btecli-2.0.0/resources/
+drwxr-xr-x   0 etejeda    (501) staff       (20)        0 2023-07-18 21:13:15.894728 btecli-2.0.0/resources/icons/
+-rw-r--r--   0 etejeda    (501) staff       (20)     9662 2023-05-10 17:31:13.000000 btecli-2.0.0/resources/icons/admin.ico
+-rw-r--r--   0 etejeda    (501) staff       (20)     1666 2023-07-18 21:13:15.897364 btecli-2.0.0/setup.cfg
+-rw-r--r--   0 etejeda    (501) staff       (20)     2372 2023-05-10 17:31:13.000000 btecli-2.0.0/setup.iss
+-rw-r--r--   0 etejeda    (501) staff       (20)      810 2023-05-15 00:04:01.000000 btecli-2.0.0/setup.py
+-rw-r--r--   0 etejeda    (501) staff       (20)      743 2023-05-12 21:09:15.000000 btecli-2.0.0/version.rc
```

### Comparing `btecli-1.7.2/.gitignore` & `btecli-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/LICENSE` & `btecli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/PKG-INFO` & `btecli-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btecli
-Version: 1.7.2
+Version: 2.0.0
 Summary: Extensible CLI
 Home-page: https://github.com/berttejeda/bert.ecli.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: bash,python,click,subprocess,yaml,cli,options,extensible,plugins,polyglot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: btecli Version: 1.7.2 Summary: Extensible CLI Home-
+Metadata-Version: 2.1 Name: btecli Version: 2.0.0 Summary: Extensible CLI Home-
 page: https://github.com/berttejeda/bert.ecli.git Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com Keywords:
 bash,python,click,subprocess,yaml,cli,options,extensible,plugins,polyglot
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
```

### Comparing `btecli-1.7.2/README.md` & `btecli-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/cli.py` & `btecli-2.0.0/btecli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,20 +117,14 @@
   help='git repo username')
 @click.option('--password', '-p',
   help='git repo password')
 @click.option('--token', '-t',
   help='git repo token')
 @click.option('--repo-url', '-r',
   required=True, help='git repo URL')
-@click.option('--public-repo', '-R', cls=MutuallyExclusiveOption,
-  is_flag=True, mutually_exclusive=["use_saved_credentials"],
-  help='Used when repo does not require credentials')
-@click.option('--use-saved-credentials', '-S', cls=MutuallyExclusiveOption,
-  mutually_exclusive=["public_repo"], 
-  is_flag=True, help='Use saved credentials')
 @click.option('--alternate-name', '-n',
   help='Specify a different name for the cloned ecli Plugin repo')
 @click.option('--plugin-path', '-T',
   help='Specify a different local path for the cloned ecli Plugin repo')
 @click.option('--prompt-for-credentials', '-P',
   is_flag=True, help='Prompt for credentials')
 def install_plugin(**kwargs):
@@ -177,20 +171,15 @@
       ])
   token = first([
       kwargs['token'],
       os.environ.get('token'),
       config.get('plugins.auth.token')
       ])
 
-  # Fail if credentials not provided under certian conditios
-  if not any([kwargs['use_saved_credentials'], kwargs['public_repo']]) and not all([username, password]):
-    print('Error: Username and password can only be empty when')
-    print('using saved credentials or specifying a public repo, seek --help')
-    sys.exit()
-  elif kwargs['prompt_for_credentials'] and not all([username, password]):
+  if kwargs['prompt_for_credentials'] and not all([username, password]):
     sys.exit('Error: You specified an invalid username and/or password, seek --help')
 
   # Plugin Package Repo URL
   repo_url = kwargs['repo_url']
   # Reconstruct url if credentials provided
   if all([username,password]):
     repo_url = re.sub('(http://)(.*)|(https://)(.*)', '\\1%s:%s@\\2' % (username, password), repo_url)
```

### Comparing `btecli-1.7.2/btecli/lib/cryptography/aes.py` & `btecli-2.0.0/btecli/lib/cryptography/aes.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/cryptography/wincred.py` & `btecli-2.0.0/btecli/lib/cryptography/wincred.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/formatting/__init__.py` & `btecli-2.0.0/btecli/lib/formatting/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/logger/__init__.py` & `btecli-2.0.0/btecli/lib/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/options/mexclusive.py` & `btecli-2.0.0/btecli/lib/options/mexclusive.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/plugin/finder.py` & `btecli-2.0.0/btecli/lib/plugin/finder.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/plugin/metadata.py` & `btecli-2.0.0/btecli/lib/plugin/metadata.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/plugin/plugins.py` & `btecli-2.0.0/btecli/lib/plugin/plugins.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/proc/local_invocation.py` & `btecli-2.0.0/btecli/lib/proc/local_invocation.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/shell/__init__.py` & `btecli-2.0.0/btecli/lib/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli/lib/shell/which.py` & `btecli-2.0.0/btecli/lib/shell/which.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/btecli.egg-info/PKG-INFO` & `btecli-2.0.0/btecli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btecli
-Version: 1.7.2
+Version: 2.0.0
 Summary: Extensible CLI
 Home-page: https://github.com/berttejeda/bert.ecli.git
 Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com
 Keywords: bash,python,click,subprocess,yaml,cli,options,extensible,plugins,polyglot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: btecli Version: 1.7.2 Summary: Extensible CLI Home-
+Metadata-Version: 2.1 Name: btecli Version: 2.0.0 Summary: Extensible CLI Home-
 page: https://github.com/berttejeda/bert.ecli.git Author: Engelbert Tejeda
 Author-email: berttejeda@gmail.com Keywords:
 bash,python,click,subprocess,yaml,cli,options,extensible,plugins,polyglot
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
```

### Comparing `btecli-1.7.2/btecli.egg-info/SOURCES.txt` & `btecli-2.0.0/btecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/resources/icons/admin.ico` & `btecli-2.0.0/resources/icons/admin.ico`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/setup.cfg` & `btecli-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/setup.iss` & `btecli-2.0.0/setup.iss`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/setup.py` & `btecli-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `btecli-1.7.2/version.rc` & `btecli-2.0.0/version.rc`

 * *Files identical despite different names*

